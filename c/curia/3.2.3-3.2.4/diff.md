# Comparing `tmp/curia-3.2.3.tar.gz` & `tmp/curia-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curia-3.2.3.tar", last modified: Fri Mar 31 00:31:33 2023, max compression
+gzip compressed data, was "curia-3.2.4.tar", last modified: Mon Apr  3 17:15:52 2023, max compression
```

## Comparing `curia-3.2.3.tar` & `curia-3.2.4.tar`

### file list

```diff
@@ -1,945 +1,945 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.488830 curia-3.2.3/
--rw-r--r--   0 root         (0) root         (0)     6254 2023-03-31 00:31:33.488830 curia-3.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5770 2023-03-31 00:29:11.000000 curia-3.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)      581 2023-03-31 00:31:33.488830 curia-3.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2801 2023-03-31 00:29:11.000000 curia-3.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.324827 curia-3.2.3/src/
--rw-r--r--   0 root         (0) root         (0)       39 2023-03-31 00:29:11.000000 curia-3.2.3/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.324827 curia-3.2.3/src/curia/
--rw-r--r--   0 root         (0) root         (0)       45 2023-03-31 00:31:24.000000 curia-3.2.3/src/curia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.324827 curia-3.2.3/src/curia/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.324827 curia-3.2.3/src/curia/api/swagger_client/
--rw-r--r--   0 root         (0) root         (0)    30976 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.332827 curia-3.2.3/src/curia/api/swagger_client/api/
--rw-r--r--   0 root         (0) root         (0)     2001 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33298 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/analyses_api.py
--rw-r--r--   0 root         (0) root         (0)    35010 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/analysis_job_outputs_api.py
--rw-r--r--   0 root         (0) root         (0)    35022 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/analysis_job_statuses_api.py
--rw-r--r--   0 root         (0) root         (0)    40916 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/analysis_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    39712 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/cohorts_api.py
--rw-r--r--   0 root         (0) root         (0)    37575 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/data_queries_api.py
--rw-r--r--   0 root         (0) root         (0)    33593 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/data_stores_api.py
--rw-r--r--   0 root         (0) root         (0)    13411 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/data_tables_api.py
--rw-r--r--   0 root         (0) root         (0)    19429 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/databases_api.py
--rw-r--r--   0 root         (0) root         (0)    34241 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/dataset_columns_api.py
--rw-r--r--   0 root         (0) root         (0)    63633 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/datasets_api.py
--rw-r--r--   0 root         (0) root         (0)    34079 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/feature_stores_api.py
--rw-r--r--   0 root         (0) root         (0)    33148 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/features_api.py
--rw-r--r--   0 root         (0) root         (0)    40503 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/internal_api.py
--rw-r--r--   0 root         (0) root         (0)    45617 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/model_batch_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    33767 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/model_batches_api.py
--rw-r--r--   0 root         (0) root         (0)    34473 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/model_job_outputs_api.py
--rw-r--r--   0 root         (0) root         (0)    17675 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/model_job_statuses_api.py
--rw-r--r--   0 root         (0) root         (0)    48175 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/model_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    38506 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/model_populations_api.py
--rw-r--r--   0 root         (0) root         (0)    43110 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/models_api.py
--rw-r--r--   0 root         (0) root         (0)    41832 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/organization_settings_api.py
--rw-r--r--   0 root         (0) root         (0)    34015 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/organizations_api.py
--rw-r--r--   0 root         (0) root         (0)  1096890 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/platform_api.py
--rw-r--r--   0 root         (0) root         (0)    34565 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/population_stores_api.py
--rw-r--r--   0 root         (0) root         (0)    34848 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/process_job_outputs_api.py
--rw-r--r--   0 root         (0) root         (0)    34860 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/process_job_statuses_api.py
--rw-r--r--   0 root         (0) root         (0)    40756 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/process_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    33160 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/processes_api.py
--rw-r--r--   0 root         (0) root         (0)    34241 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/project_members_api.py
--rw-r--r--   0 root         (0) root         (0)    43621 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/projects_api.py
--rw-r--r--   0 root         (0) root         (0)    33471 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/scheduler_api.py
--rw-r--r--   0 root         (0) root         (0)    13655 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/user_audit_trail_api.py
--rw-r--r--   0 root         (0) root         (0)    34079 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/user_favorites_api.py
--rw-r--r--   0 root         (0) root         (0)    60845 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/user_management_api.py
--rw-r--r--   0 root         (0) root         (0)    74947 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api/workflows_api.py
--rw-r--r--   0 root         (0) root         (0)    24814 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/api_client.py
--rw-r--r--   0 root         (0) root         (0)     8233 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.400829 curia-3.2.3/src/curia/api/swagger_client/models/
--rw-r--r--   0 root         (0) root         (0)    28890 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/aggregation_type.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_cohort_model.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_cohort_organization.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_data_table_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_cohorts.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2854 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_environment.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_model.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_project.py
--rw-r--r--   0 root         (0) root         (0)     2811 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_model_jobs.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_project.py
--rw-r--r--   0 root         (0) root         (0)    13573 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis.py
--rw-r--r--   0 root         (0) root         (0)    18641 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job.py
--rw-r--r--   0 root         (0) root         (0)     5946 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_config.py
--rw-r--r--   0 root         (0) root         (0)    12323 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11100 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output.py
--rw-r--r--   0 root         (0) root         (0)    13519 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    16307 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11639 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14674 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15317 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_status.py
--rw-r--r--   0 root         (0) root         (0)    12635 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15431 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_type.py
--rw-r--r--   0 root         (0) root         (0)    12167 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11343 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2521 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/analysis_type.py
--rw-r--r--   0 root         (0) root         (0)     2514 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py
--rw-r--r--   0 root         (0) root         (0)     2586 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/any_of_condition_value.py
--rw-r--r--   0 root         (0) root         (0)     4625 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/arithmetic_expression.py
--rw-r--r--   0 root         (0) root         (0)     2685 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/arithmetic_operator.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/body.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/body1.py
--rw-r--r--   0 root         (0) root         (0)     4870 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/body2.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/body3.py
--rw-r--r--   0 root         (0) root         (0)     6737 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/boolean_expression.py
--rw-r--r--   0 root         (0) root         (0)    15654 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/code.py
--rw-r--r--   0 root         (0) root         (0)    15737 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort.py
--rw-r--r--   0 root         (0) root         (0)    15741 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_definition.py
--rw-r--r--   0 root         (0) root         (0)    10323 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_filter.py
--rw-r--r--   0 root         (0) root         (0)     5712 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_filter_condition.py
--rw-r--r--   0 root         (0) root         (0)    12758 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    19264 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14674 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    22215 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_results.py
--rw-r--r--   0 root         (0) root         (0)    10728 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_set.py
--rw-r--r--   0 root         (0) root         (0)    24277 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/cohort_window.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/condition.py
--rw-r--r--   0 root         (0) root         (0)     2702 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/condition_operator.py
--rw-r--r--   0 root         (0) root         (0)     5531 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_dto.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     9264 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     6164 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_cohort_dto.py
--rw-r--r--   0 root         (0) root         (0)     6662 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_data_query_dto.py
--rw-r--r--   0 root         (0) root         (0)     4455 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_data_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     6088 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_data_table_dto.py
--rw-r--r--   0 root         (0) root         (0)     5363 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_database_dto.py
--rw-r--r--   0 root         (0) root         (0)     5401 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_dataset_column_dto.py
--rw-r--r--   0 root         (0) root         (0)    13535 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)    12439 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_feature_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_dto.py
--rw-r--r--   0 root         (0) root         (0)     3237 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     3303 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     3303 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_code_dto.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_cohort_dto.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_data_query_dto.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_data_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     3237 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_environment_dto.py
--rw-r--r--   0 root         (0) root         (0)     3282 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_category_dto.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     3248 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_batch_dto.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     3248 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)     3171 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_dto.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_population_dto.py
--rw-r--r--   0 root         (0) root         (0)     3248 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_organization_dto.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py
--rw-r--r--   0 root         (0) root         (0)     3325 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_population_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_dto.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_project_dto.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_project_member_dto.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_scheduler_dto.py
--rw-r--r--   0 root         (0) root         (0)     3160 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_task_dto.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_task_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     3325 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     3248 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_dto.py
--rw-r--r--   0 root         (0) root         (0)     3303 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     3347 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py
--rw-r--r--   0 root         (0) root         (0)     4024 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_model_batch_dto.py
--rw-r--r--   0 root         (0) root         (0)     9127 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_model_batch_job_dto.py
--rw-r--r--   0 root         (0) root         (0)    10392 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_model_dto.py
--rw-r--r--   0 root         (0) root         (0)    13124 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_model_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_model_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     8913 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_model_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)    17020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_model_population_dto.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_organization_dto.py
--rw-r--r--   0 root         (0) root         (0)    10363 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_organization_setting_dto.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_population_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     5717 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_process_dto.py
--rw-r--r--   0 root         (0) root         (0)     8417 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_process_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_process_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     8770 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_process_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     5493 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_project_dto.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_project_member_dto.py
--rw-r--r--   0 root         (0) root         (0)     8771 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_scheduler_dto.py
--rw-r--r--   0 root         (0) root         (0)     6081 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_task_dto.py
--rw-r--r--   0 root         (0) root         (0)     9906 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_task_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     5635 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_task_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     7636 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py
--rw-r--r--   0 root         (0) root         (0)     4929 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_user_favorite_dto.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_dto.py
--rw-r--r--   0 root         (0) root         (0)     6958 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     5175 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py
--rw-r--r--   0 root         (0) root         (0)     5715 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     5697 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_template_dto.py
--rw-r--r--   0 root         (0) root         (0)    12698 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_query.py
--rw-r--r--   0 root         (0) root         (0)    21009 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12684 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10681 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_store.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12118 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_table.py
--rw-r--r--   0 root         (0) root         (0)    12202 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    21009 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12892 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/data_table_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12235 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/database.py
--rw-r--r--   0 root         (0) root         (0)    12079 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12160 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/database_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    23650 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset.py
--rw-r--r--   0 root         (0) root         (0)    10726 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_column.py
--rw-r--r--   0 root         (0) root         (0)    21393 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11388 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_column_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11516 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_job.py
--rw-r--r--   0 root         (0) root         (0)    11875 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_job_status.py
--rw-r--r--   0 root         (0) root         (0)    12653 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11225 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    21301 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     3997 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py
--rw-r--r--   0 root         (0) root         (0)    14049 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/environment.py
--rw-r--r--   0 root         (0) root         (0)     9848 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/environment_activity.py
--rw-r--r--   0 root         (0) root         (0)    19669 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature.py
--rw-r--r--   0 root         (0) root         (0)    10464 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_category.py
--rw-r--r--   0 root         (0) root         (0)     9759 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11212 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    24524 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10632 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    20817 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10837 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_store.py
--rw-r--r--   0 root         (0) root         (0)    10601 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10723 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_sub_category.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/feature_table.py
--rw-r--r--   0 root         (0) root         (0)     8393 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/geographic_counts.py
--rw-r--r--   0 root         (0) root         (0)     8937 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/geographic_queries.py
--rw-r--r--   0 root         (0) root         (0)     6575 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6413 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6575 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_code_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6278 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_database_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6467 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6353 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6515 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6305 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6380 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_environment_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6489 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6305 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6570 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6467 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6386 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6407 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6651 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6494 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6494 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6521 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6251 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6840 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_organization_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6629 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6521 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6548 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6386 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6548 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6305 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6467 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6305 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6467 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6629 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6224 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_task_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6494 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6575 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6683 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6737 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     6548 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     5229 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/inline_response200.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/inline_response200_info.py
--rw-r--r--   0 root         (0) root         (0)     5229 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/inline_response503.py
--rw-r--r--   0 root         (0) root         (0)    12246 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/intervention_definition.py
--rw-r--r--   0 root         (0) root         (0)     2409 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/json.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/logical_operator.py
--rw-r--r--   0 root         (0) root         (0)    18323 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model.py
--rw-r--r--   0 root         (0) root         (0)    11239 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_batch.py
--rw-r--r--   0 root         (0) root         (0)    18191 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job.py
--rw-r--r--   0 root         (0) root         (0)    13259 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10783 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15234 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12271 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     9890 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_batch_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10328 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10092 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    25040 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job.py
--rw-r--r--   0 root         (0) root         (0)     8058 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_config.py
--rw-r--r--   0 root         (0) root         (0)    12586 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_event.py
--rw-r--r--   0 root         (0) root         (0)    12870 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12709 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    20913 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10136 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11419 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15133 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    13067 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15358 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    24369 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14889 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11893 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14938 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    28487 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    16360 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12167 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11575 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_output.py
--rw-r--r--   0 root         (0) root         (0)     9880 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_feature.py
--rw-r--r--   0 root         (0) root         (0)    21489 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    13207 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    20828 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12377 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    26332 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14789 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_status.py
--rw-r--r--   0 root         (0) root         (0)    13207 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    20828 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15017 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    20188 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    13579 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    13486 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    21969 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10576 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    21975 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    27646 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12011 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10577 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    25985 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_output_details.py
--rw-r--r--   0 root         (0) root         (0)    30079 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population.py
--rw-r--r--   0 root         (0) root         (0)    12451 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14532 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    17046 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    23025 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14007 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    19123 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11277 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    17788 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    20873 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14154 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    30721 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    19567 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/object.py
--rw-r--r--   0 root         (0) root         (0)    23654 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/organization.py
--rw-r--r--   0 root         (0) root         (0)    11102 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py
--rw-r--r--   0 root         (0) root         (0)    11213 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/organization_feature_exclusion.py
--rw-r--r--   0 root         (0) root         (0)     9760 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/organization_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    16733 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/organization_setting.py
--rw-r--r--   0 root         (0) root         (0)    16733 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/organization_setting_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14679 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/outcome_definition.py
--rw-r--r--   0 root         (0) root         (0)     5139 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/period_definition.py
--rw-r--r--   0 root         (0) root         (0)     2751 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/period_type.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/person_set.py
--rw-r--r--   0 root         (0) root         (0)    15181 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/population.py
--rw-r--r--   0 root         (0) root         (0)    11761 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/population_store.py
--rw-r--r--   0 root         (0) root         (0)    10745 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/population_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12257 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process.py
--rw-r--r--   0 root         (0) root         (0)    16287 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job.py
--rw-r--r--   0 root         (0) root         (0)     4858 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_config.py
--rw-r--r--   0 root         (0) root         (0)    12271 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10479 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_output.py
--rw-r--r--   0 root         (0) root         (0)    13415 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15893 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11016 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14331 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14764 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_status.py
--rw-r--r--   0 root         (0) root         (0)    12583 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14902 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12115 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11494 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/process_type.py
--rw-r--r--   0 root         (0) root         (0)    17750 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project.py
--rw-r--r--   0 root         (0) root         (0)    13430 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    17111 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12115 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10665 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10969 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_member.py
--rw-r--r--   0 root         (0) root         (0)    12427 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11631 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_member_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14885 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15477 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/scheduler.py
--rw-r--r--   0 root         (0) root         (0)    14813 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/scheduler_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     5765 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/select_expression.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/set_operator.py
--rw-r--r--   0 root         (0) root         (0)     5727 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/state_data.py
--rw-r--r--   0 root         (0) root         (0)    12768 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task.py
--rw-r--r--   0 root         (0) root         (0)    16575 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution.py
--rw-r--r--   0 root         (0) root         (0)    13003 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14380 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    16908 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11210 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status.py
--rw-r--r--   0 root         (0) root         (0)    15880 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    18165 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11890 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_inputs.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_outputs.py
--rw-r--r--   0 root         (0) root         (0)    11939 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/task_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     5276 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_dto.py
--rw-r--r--   0 root         (0) root         (0)     8382 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     8830 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     6071 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_cohort_dto.py
--rw-r--r--   0 root         (0) root         (0)     6574 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_data_query_dto.py
--rw-r--r--   0 root         (0) root         (0)     4455 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_data_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     5915 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_data_table_dto.py
--rw-r--r--   0 root         (0) root         (0)     5280 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_database_dto.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_dataset_column_dto.py
--rw-r--r--   0 root         (0) root         (0)    13369 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)    11522 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_feature_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     3935 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_model_batch_dto.py
--rw-r--r--   0 root         (0) root         (0)     8867 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_model_batch_job_dto.py
--rw-r--r--   0 root         (0) root         (0)    10045 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_model_dto.py
--rw-r--r--   0 root         (0) root         (0)    12865 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_model_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     5262 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_model_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     8650 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_model_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)    17020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_model_population_dto.py
--rw-r--r--   0 root         (0) root         (0)     4513 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_organization_dto.py
--rw-r--r--   0 root         (0) root         (0)    10266 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_organization_setting_dto.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_population_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     5545 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_process_dto.py
--rw-r--r--   0 root         (0) root         (0)     8239 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_process_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     4585 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_process_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     8770 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_process_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     5410 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_project_dto.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_project_member_dto.py
--rw-r--r--   0 root         (0) root         (0)     8423 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_scheduler_dto.py
--rw-r--r--   0 root         (0) root         (0)     5915 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_task_dto.py
--rw-r--r--   0 root         (0) root         (0)     9720 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_task_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     5375 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_task_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     7190 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py
--rw-r--r--   0 root         (0) root         (0)     9800 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_user_dto.py
--rw-r--r--   0 root         (0) root         (0)     4929 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_user_favorite_dto.py
--rw-r--r--   0 root         (0) root         (0)     4529 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_dto.py
--rw-r--r--   0 root         (0) root         (0)     6868 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     4995 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py
--rw-r--r--   0 root         (0) root         (0)     5455 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     5525 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_template_dto.py
--rw-r--r--   0 root         (0) root         (0)    10477 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/user_audit_trail.py
--rw-r--r--   0 root         (0) root         (0)    11549 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10861 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/user_favorite.py
--rw-r--r--   0 root         (0) root         (0)    12947 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    17489 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10827 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    13030 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow.py
--rw-r--r--   0 root         (0) root         (0)    15462 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution.py
--rw-r--r--   0 root         (0) root         (0)    13240 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    10862 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_spec.py
--rw-r--r--   0 root         (0) root         (0)    14860 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11504 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    11430 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_status.py
--rw-r--r--   0 root         (0) root         (0)    14980 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    15765 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    14080 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12659 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    13131 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_response_dto.py
--rw-r--r--   0 root         (0) root         (0)    12827 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_template.py
--rw-r--r--   0 root         (0) root         (0)     5357 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_template_definition.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_template_parameters.py
--rw-r--r--   0 root         (0) root         (0)    11931 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/workflow_template_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     5645 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/models/zip_data.py
--rw-r--r--   0 root         (0) root         (0)    13198 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/swagger_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.484830 curia-3.2.3/src/curia/api/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      971 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_aggregation_type.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_cohort_model.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_cohort_organization.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_cohort_train_cohort.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_data_table_dataset.py
--rw-r--r--   0 root         (0) root         (0)      990 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_model_cohorts.py
--rw-r--r--   0 root         (0) root         (0)     1016 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_model_job_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_model_job_environment.py
--rw-r--r--   0 root         (0) root         (0)     1000 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_model_job_model.py
--rw-r--r--   0 root         (0) root         (0)     1016 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_model_job_project.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_model_model_jobs.py
--rw-r--r--   0 root         (0) root         (0)      990 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_all_of_model_project.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analyses_api.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_config.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_output.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1236 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1094 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_outputs_api.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_status.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1094 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_statuses_api.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_job_type.py
--rw-r--r--   0 root         (0) root         (0)     2659 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_analysis_type.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_any_of_arithmetic_expression_value.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_any_of_boolean_expression_value.py
--rw-r--r--   0 root         (0) root         (0)     1247 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_any_of_condition_value.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_arithmetic_expression.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_arithmetic_operator.py
--rw-r--r--   0 root         (0) root         (0)      880 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_body.py
--rw-r--r--   0 root         (0) root         (0)      889 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_body1.py
--rw-r--r--   0 root         (0) root         (0)      888 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_body2.py
--rw-r--r--   0 root         (0) root         (0)      888 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_body3.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_boolean_expression.py
--rw-r--r--   0 root         (0) root         (0)      880 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_code.py
--rw-r--r--   0 root         (0) root         (0)      896 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_definition.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_filter.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_filter_condition.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_results.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_set.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohort_window.py
--rw-r--r--   0 root         (0) root         (0)     2421 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_cohorts_api.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_condition.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_condition_operator.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_analysis_dto.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_analysis_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1078 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_analysis_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1078 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_analysis_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_cohort_dto.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_data_query_dto.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_data_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_data_table_dto.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_database_dto.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_dataset_column_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_feature_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_analysis_dto.py
--rw-r--r--   0 root         (0) root         (0)     1049 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_analysis_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_analysis_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_analysis_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)      990 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_code_dto.py
--rw-r--r--   0 root         (0) root         (0)     1006 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_cohort_dto.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_data_query_dto.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_data_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_dataset_column_dto.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_dataset_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_environment_dto.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_feature_category_dto.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_feature_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_feature_sub_category_dto.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_batch_dto.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_batch_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_dto.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_endpoint_dto.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_job_output_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_model_population_dto.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_organization_dto.py
--rw-r--r--   0 root         (0) root         (0)     1186 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py
--rw-r--r--   0 root         (0) root         (0)     1112 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_organization_setting_dto.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_population_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_process_dto.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_process_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_process_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_process_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_project_dto.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_project_member_dto.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_scheduler_dto.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_task_dto.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_task_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_task_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_user_favorite_dto.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_workflow_dto.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_workflow_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_many_workflow_template_dto.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_model_batch_dto.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_model_batch_job_dto.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_model_dto.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_model_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_model_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_model_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_model_population_dto.py
--rw-r--r--   0 root         (0) root         (0)     1034 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_organization_dto.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_organization_setting_dto.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_population_store_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_process_dto.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_process_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_process_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_process_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_project_dto.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_project_member_dto.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_scheduler_dto.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_task_dto.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_task_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     1094 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_task_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_user_audit_trail_dto.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_user_favorite_dto.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_workflow_dto.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_workflow_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_workflow_execution_spec_dto.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_workflow_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_create_workflow_template_dto.py
--rw-r--r--   0 root         (0) root         (0)     2414 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_queries_api.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_query.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_query_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_store.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_stores_api.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_table.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_table_joined_database_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_table_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_table_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_data_tables_api.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_database.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_database_joined_data_table_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_database_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_databases_api.py
--rw-r--r--   0 root         (0) root         (0)      904 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_column.py
--rw-r--r--   0 root         (0) root         (0)     1168 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_column_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_columns_api.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_job.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_job_status.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1168 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_datasets_api.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_environment.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_environment_activity.py
--rw-r--r--   0 root         (0) root         (0)      904 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_category.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1210 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1184 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_joined_model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1290 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_store.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_stores_api.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_sub_category.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_feature_table.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_features_api.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_geographic_counts.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_geographic_queries.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_analysis_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_analysis_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_code_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_data_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_data_table_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_database_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_dataset_column_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_dataset_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_environment_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_feature_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1098 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_feature_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1109 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_batch_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_batch_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1098 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_endpoint_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_job_event_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1116 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1066 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1116 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1123 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_organization_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_organization_setting_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_population_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_process_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_process_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_process_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_process_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_project_member_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_scheduler_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_task_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_task_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_task_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1098 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_workflow_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_get_many_workflow_template_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_inline_response200.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_inline_response200_info.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_inline_response503.py
--rw-r--r--   0 root         (0) root         (0)     7508 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_internal_api.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_intervention_definition.py
--rw-r--r--   0 root         (0) root         (0)      881 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_json.py
--rw-r--r--   0 root         (0) root         (0)      971 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_logical_operator.py
--rw-r--r--   0 root         (0) root         (0)      888 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch_job.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1062 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batch_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_batches_api.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_dataset.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_endpoint.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_config.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_event.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1424 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1112 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_output.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_output_feature.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_outputs_api.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_status.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_job_statuses_api.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1094 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1112 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_model_output_details_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_joined_user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_output_details.py
--rw-r--r--   0 root         (0) root         (0)      971 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1234 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1310 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_data_query_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1184 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_feature_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1306 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_model_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_population_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_populations_api.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2805 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_models_api.py
--rw-r--r--   0 root         (0) root         (0)      896 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_object.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organization.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organization_feature_category_exclusion.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organization_feature_exclusion.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organization_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organization_setting.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organization_setting_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organization_settings_api.py
--rw-r--r--   0 root         (0) root         (0)     2341 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_organizations_api.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_outcome_definition.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_period_definition.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_period_type.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_person_set.py
--rw-r--r--   0 root         (0) root         (0)    26517 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_platform_api.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_population.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_population_store.py
--rw-r--r--   0 root         (0) root         (0)     1062 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_population_store_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2510 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_population_stores_api.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_config.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_output.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_output_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_outputs_api.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_status.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_status_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2550 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_job_statuses_api.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_process_type.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_processes_api.py
--rw-r--r--   0 root         (0) root         (0)      904 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_joined_user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_member.py
--rw-r--r--   0 root         (0) root         (0)     1168 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_member_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_member_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_members_api.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_projects_api.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_scheduler_api.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_scheduler_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_select_expression.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_set_operator.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_state_data.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution_joined_task_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1236 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution_status.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_inputs.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_outputs.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_task_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_analysis_dto.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_analysis_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1078 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_analysis_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1078 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_analysis_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_cohort_dto.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_data_query_dto.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_data_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_data_table_dto.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_database_dto.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_dataset_column_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_dataset_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_feature_dto.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_feature_store_dto.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_model_batch_dto.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_model_batch_job_dto.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_model_dto.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_model_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_model_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_model_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_model_population_dto.py
--rw-r--r--   0 root         (0) root         (0)     1034 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_organization_dto.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_organization_setting_dto.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_population_store_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_process_dto.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_process_job_dto.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_process_job_output_dto.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_process_job_status_dto.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_project_dto.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_project_member_dto.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_scheduler_dto.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_task_dto.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_task_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     1094 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_task_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_user_audit_trail_dto.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_user_favorite_dto.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_workflow_dto.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_workflow_execution_dto.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_workflow_execution_spec_dto.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_workflow_execution_status_dto.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_update_workflow_template_dto.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_audit_trail.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_audit_trail_api.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_audit_trail_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_favorite.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_favorite_joined_model_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_favorite_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_favorites_api.py
--rw-r--r--   0 root         (0) root         (0)     4382 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_user_management_api.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution_spec.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1112 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution_spec_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution_status.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_execution_status_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_response_dto.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_template.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_template_definition.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_template_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1084 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflow_template_response_dto.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_workflows_api.py
--rw-r--r--   0 root         (0) root         (0)      920 2023-03-31 00:31:19.000000 curia-3.2.3/src/curia/api/test/test_zip_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.488830 curia-3.2.3/src/curia/mock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22897 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/mock/api.py
--rw-r--r--   0 root         (0) root         (0)    17122 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/mock/api_server.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/mock/moto.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/mock/s3.py
--rw-r--r--   0 root         (0) root         (0)    13216 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/mock/server.py
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/mock/session.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/session.py
--rw-r--r--   0 root         (0) root         (0)    14586 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/synthetic_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.488830 curia-3.2.3/src/curia/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1276 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/utils/dataset.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/utils/job.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/utils/python.py
--rw-r--r--   0 root         (0) root         (0)     7202 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/utils/s3.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-03-31 00:29:11.000000 curia-3.2.3/src/curia/utils/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.324827 curia-3.2.3/src/curia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6254 2023-03-31 00:31:33.000000 curia-3.2.3/src/curia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    56511 2023-03-31 00:31:33.000000 curia-3.2.3/src/curia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 00:31:33.000000 curia-3.2.3/src/curia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      350 2023-03-31 00:31:33.000000 curia-3.2.3/src/curia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-31 00:31:33.000000 curia-3.2.3/src/curia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 00:31:33.488830 curia-3.2.3/test/
--rw-r--r--   0 root         (0) root         (0)      498 2023-03-31 00:29:12.000000 curia-3.2.3/test/test_session.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-03-31 00:29:12.000000 curia-3.2.3/test/test_synthetic_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.274062 curia-3.2.4/
+-rw-r--r--   0 root         (0) root         (0)     6254 2023-04-03 17:15:52.274062 curia-3.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5770 2023-04-03 17:12:57.000000 curia-3.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      581 2023-04-03 17:15:52.274062 curia-3.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2801 2023-04-03 17:12:57.000000 curia-3.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.010059 curia-3.2.4/src/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-03 17:12:57.000000 curia-3.2.4/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.010059 curia-3.2.4/src/curia/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-03 17:15:41.000000 curia-3.2.4/src/curia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.010059 curia-3.2.4/src/curia/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.010059 curia-3.2.4/src/curia/api/swagger_client/
+-rw-r--r--   0 root         (0) root         (0)    30976 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.022060 curia-3.2.4/src/curia/api/swagger_client/api/
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33298 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/analyses_api.py
+-rw-r--r--   0 root         (0) root         (0)    35010 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/analysis_job_outputs_api.py
+-rw-r--r--   0 root         (0) root         (0)    35022 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/analysis_job_statuses_api.py
+-rw-r--r--   0 root         (0) root         (0)    40916 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/analysis_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    39712 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/cohorts_api.py
+-rw-r--r--   0 root         (0) root         (0)    37575 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/data_queries_api.py
+-rw-r--r--   0 root         (0) root         (0)    33593 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/data_stores_api.py
+-rw-r--r--   0 root         (0) root         (0)    13411 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/data_tables_api.py
+-rw-r--r--   0 root         (0) root         (0)    19429 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/databases_api.py
+-rw-r--r--   0 root         (0) root         (0)    34241 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/dataset_columns_api.py
+-rw-r--r--   0 root         (0) root         (0)    63633 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/datasets_api.py
+-rw-r--r--   0 root         (0) root         (0)    34079 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/feature_stores_api.py
+-rw-r--r--   0 root         (0) root         (0)    33148 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/features_api.py
+-rw-r--r--   0 root         (0) root         (0)    40503 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/internal_api.py
+-rw-r--r--   0 root         (0) root         (0)    45617 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/model_batch_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    33767 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/model_batches_api.py
+-rw-r--r--   0 root         (0) root         (0)    34473 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/model_job_outputs_api.py
+-rw-r--r--   0 root         (0) root         (0)    17675 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/model_job_statuses_api.py
+-rw-r--r--   0 root         (0) root         (0)    48175 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/model_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    38506 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/model_populations_api.py
+-rw-r--r--   0 root         (0) root         (0)    43110 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/models_api.py
+-rw-r--r--   0 root         (0) root         (0)    41832 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/organization_settings_api.py
+-rw-r--r--   0 root         (0) root         (0)    34015 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/organizations_api.py
+-rw-r--r--   0 root         (0) root         (0)  1096890 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/platform_api.py
+-rw-r--r--   0 root         (0) root         (0)    34565 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/population_stores_api.py
+-rw-r--r--   0 root         (0) root         (0)    34848 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/process_job_outputs_api.py
+-rw-r--r--   0 root         (0) root         (0)    34860 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/process_job_statuses_api.py
+-rw-r--r--   0 root         (0) root         (0)    40756 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/process_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    33160 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/processes_api.py
+-rw-r--r--   0 root         (0) root         (0)    34241 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/project_members_api.py
+-rw-r--r--   0 root         (0) root         (0)    43621 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/projects_api.py
+-rw-r--r--   0 root         (0) root         (0)    33471 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/scheduler_api.py
+-rw-r--r--   0 root         (0) root         (0)    13655 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/user_audit_trail_api.py
+-rw-r--r--   0 root         (0) root         (0)    34079 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/user_favorites_api.py
+-rw-r--r--   0 root         (0) root         (0)    60845 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)    74947 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api/workflows_api.py
+-rw-r--r--   0 root         (0) root         (0)    24814 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.114061 curia-3.2.4/src/curia/api/swagger_client/models/
+-rw-r--r--   0 root         (0) root         (0)    28890 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/aggregation_type.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_cohort_model.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_cohort_organization.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_data_table_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_cohorts.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_environment.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_model.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_project.py
+-rw-r--r--   0 root         (0) root         (0)     2811 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_model_jobs.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_project.py
+-rw-r--r--   0 root         (0) root         (0)    13573 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis.py
+-rw-r--r--   0 root         (0) root         (0)    18641 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job.py
+-rw-r--r--   0 root         (0) root         (0)     5946 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_config.py
+-rw-r--r--   0 root         (0) root         (0)    12323 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11100 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output.py
+-rw-r--r--   0 root         (0) root         (0)    13519 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    16307 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11639 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14674 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15317 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_status.py
+-rw-r--r--   0 root         (0) root         (0)    12635 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15431 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_type.py
+-rw-r--r--   0 root         (0) root         (0)    12167 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/analysis_type.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/any_of_condition_value.py
+-rw-r--r--   0 root         (0) root         (0)     4625 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/arithmetic_expression.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/arithmetic_operator.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/body.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/body1.py
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/body2.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/body3.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/boolean_expression.py
+-rw-r--r--   0 root         (0) root         (0)    15654 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/code.py
+-rw-r--r--   0 root         (0) root         (0)    15737 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort.py
+-rw-r--r--   0 root         (0) root         (0)    15741 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10323 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_filter.py
+-rw-r--r--   0 root         (0) root         (0)     5712 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_filter_condition.py
+-rw-r--r--   0 root         (0) root         (0)    12758 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    19264 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14674 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    22215 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_results.py
+-rw-r--r--   0 root         (0) root         (0)    10728 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_set.py
+-rw-r--r--   0 root         (0) root         (0)    24277 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/cohort_window.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/condition.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/condition_operator.py
+-rw-r--r--   0 root         (0) root         (0)     5531 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     9264 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6164 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_cohort_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6662 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_data_query_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4455 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_data_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_data_table_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_database_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_dataset_column_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13535 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12439 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_feature_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_code_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_cohort_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_data_query_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_data_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_environment_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_category_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_batch_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3171 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_population_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_organization_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3325 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_population_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_project_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_project_member_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_scheduler_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_task_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_task_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3325 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4024 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_model_batch_dto.py
+-rw-r--r--   0 root         (0) root         (0)     9127 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_model_batch_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10392 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_model_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13124 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_model_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_model_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8913 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_model_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)    17020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_model_population_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_organization_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10363 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_organization_setting_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_population_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5717 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_process_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8417 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_process_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_process_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8770 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_process_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5493 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_project_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_project_member_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8771 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_scheduler_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6081 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_task_dto.py
+-rw-r--r--   0 root         (0) root         (0)     9906 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_task_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5635 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_task_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7636 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_user_favorite_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6958 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5175 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5715 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_template_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12698 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_query.py
+-rw-r--r--   0 root         (0) root         (0)    21009 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12684 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10681 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_store.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12118 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_table.py
+-rw-r--r--   0 root         (0) root         (0)    12202 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    21009 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12892 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/data_table_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12235 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/database.py
+-rw-r--r--   0 root         (0) root         (0)    12079 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12160 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/database_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    23650 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10726 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_column.py
+-rw-r--r--   0 root         (0) root         (0)    21393 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11388 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_column_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11516 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_job.py
+-rw-r--r--   0 root         (0) root         (0)    11875 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_job_status.py
+-rw-r--r--   0 root         (0) root         (0)    12653 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11225 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    21301 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py
+-rw-r--r--   0 root         (0) root         (0)    14049 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/environment.py
+-rw-r--r--   0 root         (0) root         (0)     9848 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/environment_activity.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature.py
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_category.py
+-rw-r--r--   0 root         (0) root         (0)     9759 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11212 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    24524 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10632 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    20817 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10837 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_store.py
+-rw-r--r--   0 root         (0) root         (0)    10601 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10723 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_sub_category.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/feature_table.py
+-rw-r--r--   0 root         (0) root         (0)     8393 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/geographic_counts.py
+-rw-r--r--   0 root         (0) root         (0)     8937 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/geographic_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_code_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6278 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_database_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6353 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6515 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6305 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6380 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_environment_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6489 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6305 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6570 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6386 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6407 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6494 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6494 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6840 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_organization_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6629 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6548 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6386 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6548 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6305 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6305 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6629 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_task_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6494 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6683 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6548 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5229 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/inline_response200_info.py
+-rw-r--r--   0 root         (0) root         (0)     5229 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/inline_response503.py
+-rw-r--r--   0 root         (0) root         (0)    12246 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/intervention_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/json.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/logical_operator.py
+-rw-r--r--   0 root         (0) root         (0)    18323 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model.py
+-rw-r--r--   0 root         (0) root         (0)    11239 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_batch.py
+-rw-r--r--   0 root         (0) root         (0)    18191 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job.py
+-rw-r--r--   0 root         (0) root         (0)    13259 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10783 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15234 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12271 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     9890 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_batch_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10328 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10092 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    25040 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job.py
+-rw-r--r--   0 root         (0) root         (0)     8058 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_config.py
+-rw-r--r--   0 root         (0) root         (0)    12586 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_event.py
+-rw-r--r--   0 root         (0) root         (0)    12870 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12709 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    20913 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10136 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11419 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15133 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13067 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15358 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    24369 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14889 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11893 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14938 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    28487 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    16360 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12167 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11575 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_output.py
+-rw-r--r--   0 root         (0) root         (0)     9880 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_feature.py
+-rw-r--r--   0 root         (0) root         (0)    21489 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13207 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    20828 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12377 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    26332 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14789 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_status.py
+-rw-r--r--   0 root         (0) root         (0)    13207 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    20828 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15017 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    20188 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13579 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13486 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    21969 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10576 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    21975 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    27646 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12011 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10577 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    25985 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_output_details.py
+-rw-r--r--   0 root         (0) root         (0)    30079 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population.py
+-rw-r--r--   0 root         (0) root         (0)    12451 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14532 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    17046 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    23025 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14007 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    19123 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11277 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    17788 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    20873 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14154 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    30721 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    19567 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/object.py
+-rw-r--r--   0 root         (0) root         (0)    23654 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/organization.py
+-rw-r--r--   0 root         (0) root         (0)    11102 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py
+-rw-r--r--   0 root         (0) root         (0)    11213 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/organization_feature_exclusion.py
+-rw-r--r--   0 root         (0) root         (0)     9760 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/organization_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    16733 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/organization_setting.py
+-rw-r--r--   0 root         (0) root         (0)    16733 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/organization_setting_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/outcome_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5139 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/period_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/period_type.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/person_set.py
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/population.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/population_store.py
+-rw-r--r--   0 root         (0) root         (0)    10745 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/population_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12257 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job.py
+-rw-r--r--   0 root         (0) root         (0)     4858 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_config.py
+-rw-r--r--   0 root         (0) root         (0)    12271 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10479 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_output.py
+-rw-r--r--   0 root         (0) root         (0)    13415 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15893 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11016 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14331 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14764 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_status.py
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14902 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12115 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11494 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/process_type.py
+-rw-r--r--   0 root         (0) root         (0)    17750 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project.py
+-rw-r--r--   0 root         (0) root         (0)    13430 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    17111 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12115 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10665 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10969 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_member.py
+-rw-r--r--   0 root         (0) root         (0)    12427 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11631 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_member_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14885 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15477 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    14813 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/scheduler_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5765 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/select_expression.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/set_operator.py
+-rw-r--r--   0 root         (0) root         (0)     5727 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/state_data.py
+-rw-r--r--   0 root         (0) root         (0)    12768 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    16575 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution.py
+-rw-r--r--   0 root         (0) root         (0)    13003 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14380 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    16908 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11210 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status.py
+-rw-r--r--   0 root         (0) root         (0)    15880 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    18165 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11890 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_inputs.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_outputs.py
+-rw-r--r--   0 root         (0) root         (0)    11939 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/task_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8382 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8830 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_cohort_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_data_query_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4455 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_data_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5915 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_data_table_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_database_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_dataset_column_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11522 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_feature_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3935 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_model_batch_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8867 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_model_batch_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10045 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_model_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12865 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_model_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5262 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_model_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8650 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_model_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)    17020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_model_population_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_organization_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10266 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_organization_setting_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_population_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5545 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_process_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8239 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_process_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_process_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8770 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_process_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5410 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_project_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_project_member_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_scheduler_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5915 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_task_dto.py
+-rw-r--r--   0 root         (0) root         (0)     9720 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_task_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5375 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_task_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7190 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py
+-rw-r--r--   0 root         (0) root         (0)     9800 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_user_favorite_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4529 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4995 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5525 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_template_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10477 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/user_audit_trail.py
+-rw-r--r--   0 root         (0) root         (0)    11549 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10861 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/user_favorite.py
+-rw-r--r--   0 root         (0) root         (0)    12947 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    17489 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10827 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13030 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    15462 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution.py
+-rw-r--r--   0 root         (0) root         (0)    13240 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    10862 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_spec.py
+-rw-r--r--   0 root         (0) root         (0)    14860 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11504 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    11430 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_status.py
+-rw-r--r--   0 root         (0) root         (0)    14980 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    15765 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    14080 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12659 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    13131 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12827 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_template.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_template_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_template_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    11931 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/workflow_template_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5645 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/models/zip_data.py
+-rw-r--r--   0 root         (0) root         (0)    13198 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/swagger_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.270062 curia-3.2.4/src/curia/api/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_aggregation_type.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_cohort_model.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_cohort_organization.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_cohort_train_cohort.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_data_table_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_model_cohorts.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_model_job_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_model_job_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_model_job_model.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_model_job_project.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_model_model_jobs.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_all_of_model_project.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analyses_api.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_config.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_output.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_outputs_api.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_status.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_statuses_api.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_job_type.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_analysis_type.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_any_of_arithmetic_expression_value.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_any_of_boolean_expression_value.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_any_of_condition_value.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_arithmetic_expression.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_arithmetic_operator.py
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_body.py
+-rw-r--r--   0 root         (0) root         (0)      889 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_body1.py
+-rw-r--r--   0 root         (0) root         (0)      888 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_body2.py
+-rw-r--r--   0 root         (0) root         (0)      888 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_body3.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_boolean_expression.py
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_code.py
+-rw-r--r--   0 root         (0) root         (0)      896 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_definition.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_filter_condition.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_results.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_set.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohort_window.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_cohorts_api.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_condition.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_condition_operator.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_analysis_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_analysis_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_analysis_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_analysis_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_cohort_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_data_query_dto.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_data_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_data_table_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_database_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_dataset_column_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_feature_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_analysis_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_analysis_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_analysis_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_analysis_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_code_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_cohort_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_data_query_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_data_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_dataset_column_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_dataset_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_environment_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_feature_category_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_feature_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_feature_sub_category_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_batch_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_batch_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_endpoint_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_job_output_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_model_population_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_organization_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_organization_setting_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_population_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_process_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_process_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_process_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_process_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_project_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_project_member_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_scheduler_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_task_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_task_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_task_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_user_favorite_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_workflow_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_workflow_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_many_workflow_template_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_model_batch_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_model_batch_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_model_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_model_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_model_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_model_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_model_population_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_organization_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_organization_setting_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_population_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_process_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_process_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_process_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_process_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_project_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_project_member_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_scheduler_dto.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_task_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_task_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_task_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_user_audit_trail_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_user_favorite_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_workflow_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_workflow_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_workflow_execution_spec_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_workflow_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_create_workflow_template_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_queries_api.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_query.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      922 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_store.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_stores_api.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_table.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_table_joined_database_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_table_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_table_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_data_tables_api.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_database.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_database_joined_data_table_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_database_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_databases_api.py
+-rw-r--r--   0 root         (0) root         (0)      904 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_column.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_column_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_columns_api.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_job.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_job_status.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_datasets_api.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_environment_activity.py
+-rw-r--r--   0 root         (0) root         (0)      904 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_category.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_joined_model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_store.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_stores_api.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_sub_category.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_feature_table.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_features_api.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_geographic_counts.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_geographic_queries.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_analysis_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_analysis_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_code_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_data_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_data_table_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_database_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_dataset_column_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_dataset_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_environment_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_feature_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_feature_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_batch_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_batch_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_endpoint_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_job_event_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_organization_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_organization_setting_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_population_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_process_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_process_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_process_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_process_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_project_member_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_scheduler_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_task_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_task_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_task_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_workflow_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_get_many_workflow_template_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_inline_response200_info.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_inline_response503.py
+-rw-r--r--   0 root         (0) root         (0)     7508 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_internal_api.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_intervention_definition.py
+-rw-r--r--   0 root         (0) root         (0)      881 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_json.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_logical_operator.py
+-rw-r--r--   0 root         (0) root         (0)      888 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch_job.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batch_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_batches_api.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_config.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_event.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_output.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_output_feature.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_outputs_api.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_status.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_job_statuses_api.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_model_output_details_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_joined_user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_output_details.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_data_query_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_feature_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_model_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_population_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_populations_api.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_models_api.py
+-rw-r--r--   0 root         (0) root         (0)      896 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_object.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organization.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organization_feature_category_exclusion.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organization_feature_exclusion.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organization_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organization_setting.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organization_setting_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organization_settings_api.py
+-rw-r--r--   0 root         (0) root         (0)     2341 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_organizations_api.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_outcome_definition.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_period_definition.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_period_type.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_person_set.py
+-rw-r--r--   0 root         (0) root         (0)    26517 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_platform_api.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_population.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_population_store.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_population_store_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2510 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_population_stores_api.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_config.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_output.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_output_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_outputs_api.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_status.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_status_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_job_statuses_api.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_process_type.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_processes_api.py
+-rw-r--r--   0 root         (0) root         (0)      904 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_joined_user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_member.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_member_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_member_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_members_api.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_projects_api.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_scheduler_api.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_scheduler_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_select_expression.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_set_operator.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_state_data.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution_joined_task_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution_status.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_inputs.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_outputs.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_task_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_analysis_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_analysis_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_analysis_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_analysis_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_cohort_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_data_query_dto.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_data_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_data_table_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_database_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_dataset_column_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_dataset_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_feature_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_feature_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_model_batch_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_model_batch_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_model_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_model_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_model_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_model_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_model_population_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_organization_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_organization_setting_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_population_store_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_process_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_process_job_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_process_job_output_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_process_job_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_project_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_project_member_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_scheduler_dto.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_task_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_task_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_task_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_user_audit_trail_dto.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_user_favorite_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_workflow_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_workflow_execution_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_workflow_execution_spec_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_workflow_execution_status_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_update_workflow_template_dto.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_audit_trail.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_audit_trail_api.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_audit_trail_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_favorite.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_favorite_joined_model_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_favorite_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_favorites_api.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution_spec.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution_spec_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution_status.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_execution_status_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_template.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_template_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_template_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflow_template_response_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_workflows_api.py
+-rw-r--r--   0 root         (0) root         (0)      920 2023-04-03 17:15:34.000000 curia-3.2.4/src/curia/api/test/test_zip_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.270062 curia-3.2.4/src/curia/mock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22897 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/mock/api.py
+-rw-r--r--   0 root         (0) root         (0)    17122 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/mock/api_server.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/mock/moto.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/mock/s3.py
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/mock/server.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/mock/session.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/session.py
+-rw-r--r--   0 root         (0) root         (0)    14586 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/synthetic_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.274062 curia-3.2.4/src/curia/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/utils/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/utils/job.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/utils/python.py
+-rw-r--r--   0 root         (0) root         (0)     7202 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/utils/s3.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-04-03 17:12:57.000000 curia-3.2.4/src/curia/utils/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.010059 curia-3.2.4/src/curia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6254 2023-04-03 17:15:51.000000 curia-3.2.4/src/curia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    56511 2023-04-03 17:15:51.000000 curia-3.2.4/src/curia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 17:15:51.000000 curia-3.2.4/src/curia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-03 17:15:51.000000 curia-3.2.4/src/curia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-03 17:15:51.000000 curia-3.2.4/src/curia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:15:52.274062 curia-3.2.4/test/
+-rw-r--r--   0 root         (0) root         (0)      498 2023-04-03 17:12:57.000000 curia-3.2.4/test/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-04-03 17:12:57.000000 curia-3.2.4/test/test_synthetic_data.py
```

### Comparing `curia-3.2.3/PKG-INFO` & `curia-3.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curia
-Version: 3.2.3
+Version: 3.2.4
 Summary: A library for training and using risk & impactability models on Curia
 Home-page: https://github.com/Curia-ai/curia-python-sdk
 Author: Curia.ai
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `curia-3.2.3/README.md` & `curia-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/setup.cfg` & `curia-3.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/setup.py` & `curia-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/setup.py` & `curia-3.2.4/src/curia/api/setup.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/__init__.py` & `curia-3.2.4/src/curia/api/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/__init__.py` & `curia-3.2.4/src/curia/api/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/analyses_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/analyses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/analysis_job_outputs_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/analysis_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/analysis_job_statuses_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/analysis_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/analysis_jobs_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/analysis_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/cohorts_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/cohorts_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/data_queries_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/data_queries_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/data_stores_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/data_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/data_tables_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/data_tables_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/databases_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/databases_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/dataset_columns_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/dataset_columns_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/datasets_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/feature_stores_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/feature_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/features_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/features_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/internal_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/internal_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/model_batch_jobs_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/model_batch_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/model_batches_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/model_batches_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/model_job_outputs_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/model_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/model_job_statuses_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/model_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/model_jobs_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/model_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/model_populations_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/model_populations_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/models_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/organization_settings_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/organization_settings_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/organizations_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/platform_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/platform_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/population_stores_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/population_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/process_job_outputs_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/process_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/process_job_statuses_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/process_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/process_jobs_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/process_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/processes_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/processes_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/project_members_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/project_members_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/projects_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/scheduler_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/user_audit_trail_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/user_audit_trail_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/user_favorites_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/user_favorites_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/user_management_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/user_management_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api/workflows_api.py` & `curia-3.2.4/src/curia/api/swagger_client/api/workflows_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/api_client.py` & `curia-3.2.4/src/curia/api/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/configuration.py` & `curia-3.2.4/src/curia/api/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/__init__.py` & `curia-3.2.4/src/curia/api/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/aggregation_type.py` & `curia-3.2.4/src/curia/api/swagger_client/models/aggregation_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_cohort_model.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_cohort_model.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_cohort_organization.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_cohort_organization.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_cohort_train_cohort.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_data_table_dataset.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_data_table_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_cohorts.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_cohorts.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_dataset.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_environment.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_environment.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_model.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_model.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_job_project.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_job_project.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_model_jobs.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_model_jobs.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/all_of_model_project.py` & `curia-3.2.4/src/curia/api/swagger_client/models/all_of_model_project.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_config.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output_joined_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_status.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_job_type.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_job_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/analysis_type.py` & `curia-3.2.4/src/curia/api/swagger_client/models/analysis_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py` & `curia-3.2.4/src/curia/api/swagger_client/models/any_of_arithmetic_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py` & `curia-3.2.4/src/curia/api/swagger_client/models/any_of_boolean_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py` & `curia-3.2.4/src/curia/api/swagger_client/models/any_of_cohort_definition_patient_metadata_filters_items.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/any_of_condition_value.py` & `curia-3.2.4/src/curia/api/swagger_client/models/any_of_condition_value.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/arithmetic_expression.py` & `curia-3.2.4/src/curia/api/swagger_client/models/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/arithmetic_operator.py` & `curia-3.2.4/src/curia/api/swagger_client/models/arithmetic_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/body.py` & `curia-3.2.4/src/curia/api/swagger_client/models/body.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/body1.py` & `curia-3.2.4/src/curia/api/swagger_client/models/body1.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/body2.py` & `curia-3.2.4/src/curia/api/swagger_client/models/body2.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/body3.py` & `curia-3.2.4/src/curia/api/swagger_client/models/body3.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/boolean_expression.py` & `curia-3.2.4/src/curia/api/swagger_client/models/boolean_expression.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/code.py` & `curia-3.2.4/src/curia/api/swagger_client/models/code.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_definition.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_filter.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_filter.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_filter_condition.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_filter_condition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_results.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_results.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_set.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_set.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/cohort_window.py` & `curia-3.2.4/src/curia/api/swagger_client/models/cohort_window.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/condition.py` & `curia-3.2.4/src/curia/api/swagger_client/models/condition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/condition_operator.py` & `curia-3.2.4/src/curia/api/swagger_client/models/condition_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_cohort_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_data_query_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_data_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_data_table_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_database_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_dataset_column_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_dataset_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_feature_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_feature_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_code_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_code_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_cohort_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_data_query_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_data_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_dataset_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_dataset_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_environment_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_environment_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_category_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_feature_sub_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_batch_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_endpoint_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_job_output_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_model_population_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_organization_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_organization_feature_exclusion_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_population_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_project_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_project_member_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_scheduler_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_task_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_task_execution_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_many_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_model_batch_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_model_batch_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_model_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_model_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_model_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_model_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_model_population_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_organization_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_organization_setting_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_population_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_process_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_process_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_process_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_process_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_project_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_project_member_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_scheduler_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_task_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_task_execution_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_task_execution_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_user_favorite_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_execution_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/create_workflow_template_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/create_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_query.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_query.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_query_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_store.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_store.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_store_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_table.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_table.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_table_joined_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_table_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/data_table_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/database.py` & `curia-3.2.4/src/curia/api/swagger_client/models/database.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/database_joined_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/database_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_column.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_column.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_column_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_column_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_job.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_job_status.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_joined_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py` & `curia-3.2.4/src/curia/api/swagger_client/models/datasetsuploadlargecomplete_parts.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/environment.py` & `curia-3.2.4/src/curia/api/swagger_client/models/environment.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/environment_activity.py` & `curia-3.2.4/src/curia/api/swagger_client/models/environment_activity.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_category.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_category.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_joined_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_joined_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_store.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_store_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_sub_category.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_sub_category.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/feature_table.py` & `curia-3.2.4/src/curia/api/swagger_client/models/feature_table.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/geographic_counts.py` & `curia-3.2.4/src/curia/api/swagger_client/models/geographic_counts.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/geographic_queries.py` & `curia-3.2.4/src/curia/api/swagger_client/models/geographic_queries.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_code_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_code_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_database_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_environment_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_environment_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_endpoint_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_event_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_output_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_model_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_organization_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_process_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_task_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/get_many_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/inline_response200.py` & `curia-3.2.4/src/curia/api/swagger_client/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/inline_response200_info.py` & `curia-3.2.4/src/curia/api/swagger_client/models/inline_response200_info.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/inline_response503.py` & `curia-3.2.4/src/curia/api/swagger_client/models/inline_response503.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/intervention_definition.py` & `curia-3.2.4/src/curia/api/swagger_client/models/intervention_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/json.py` & `curia-3.2.4/src/curia/api/swagger_client/models/json.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/logical_operator.py` & `curia-3.2.4/src/curia/api/swagger_client/models/logical_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_batch.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_batch.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job_joined_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_batch_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_batch_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_dataset.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_endpoint.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_endpoint.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_config.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_event.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_event.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_output.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_feature.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_feature.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_status.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_status_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_status_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_model_output_details_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_output_details.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_output_details.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_cohort_results_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_population_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/model_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/object.py` & `curia-3.2.4/src/curia/api/swagger_client/models/object.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/organization.py` & `curia-3.2.4/src/curia/api/swagger_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py` & `curia-3.2.4/src/curia/api/swagger_client/models/organization_feature_category_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/organization_feature_exclusion.py` & `curia-3.2.4/src/curia/api/swagger_client/models/organization_feature_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/organization_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/organization_setting.py` & `curia-3.2.4/src/curia/api/swagger_client/models/organization_setting.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/organization_setting_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/outcome_definition.py` & `curia-3.2.4/src/curia/api/swagger_client/models/outcome_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/period_definition.py` & `curia-3.2.4/src/curia/api/swagger_client/models/period_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/period_type.py` & `curia-3.2.4/src/curia/api/swagger_client/models/period_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/person_set.py` & `curia-3.2.4/src/curia/api/swagger_client/models/person_set.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/population.py` & `curia-3.2.4/src/curia/api/swagger_client/models/population.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/population_store.py` & `curia-3.2.4/src/curia/api/swagger_client/models/population_store.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/population_store_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_config.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_output.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_output_joined_process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_output_joined_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_status.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/process_type.py` & `curia-3.2.4/src/curia/api/swagger_client/models/process_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_joined_model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_member.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_member.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_member_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_member_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/scheduler.py` & `curia-3.2.4/src/curia/api/swagger_client/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/scheduler_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/select_expression.py` & `curia-3.2.4/src/curia/api/swagger_client/models/select_expression.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/set_operator.py` & `curia-3.2.4/src/curia/api/swagger_client/models/set_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/state_data.py` & `curia-3.2.4/src/curia/api/swagger_client/models/state_data.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution_joined_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status_joined_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_inputs.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_inputs.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_outputs.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_outputs.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/task_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_cohort_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_data_query_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_data_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_data_table_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_database_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_dataset_column_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_dataset_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_feature_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_feature_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_model_batch_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_model_batch_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_model_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_model_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_model_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_model_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_model_population_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_organization_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_organization_setting_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_population_store_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_process_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_process_job_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_process_job_output_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_process_job_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_project_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_project_member_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_scheduler_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_task_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_task_execution_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_task_execution_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_user_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_user_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_user_favorite_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_execution_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/update_workflow_template_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/update_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/user_audit_trail.py` & `curia-3.2.4/src/curia/api/swagger_client/models/user_audit_trail.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/user_favorite.py` & `curia-3.2.4/src/curia/api/swagger_client/models/user_favorite.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/user_favorite_joined_model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/user_favorite_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_spec.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_spec.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_spec_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_status.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_status_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_joined_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_joined_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_template.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_template.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_template_definition.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_template_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_template_parameters.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_template_parameters.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/workflow_template_response_dto.py` & `curia-3.2.4/src/curia/api/swagger_client/models/workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/models/zip_data.py` & `curia-3.2.4/src/curia/api/swagger_client/models/zip_data.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/swagger_client/rest.py` & `curia-3.2.4/src/curia/api/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_aggregation_type.py` & `curia-3.2.4/src/curia/api/test/test_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_cohort_model.py` & `curia-3.2.4/src/curia/api/test/test_all_of_cohort_model.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_cohort_organization.py` & `curia-3.2.4/src/curia/api/test/test_all_of_cohort_organization.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_cohort_train_cohort.py` & `curia-3.2.4/src/curia/api/test/test_all_of_cohort_train_cohort.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_data_table_dataset.py` & `curia-3.2.4/src/curia/api/test/test_all_of_data_table_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_model_cohorts.py` & `curia-3.2.4/src/curia/api/test/test_all_of_model_cohorts.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_model_job_dataset.py` & `curia-3.2.4/src/curia/api/test/test_all_of_model_job_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_model_job_environment.py` & `curia-3.2.4/src/curia/api/test/test_all_of_model_job_environment.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_model_job_model.py` & `curia-3.2.4/src/curia/api/test/test_all_of_model_job_model.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_model_job_project.py` & `curia-3.2.4/src/curia/api/test/test_all_of_model_job_project.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_model_model_jobs.py` & `curia-3.2.4/src/curia/api/test/test_all_of_model_model_jobs.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_all_of_model_project.py` & `curia-3.2.4/src/curia/api/test/test_all_of_model_project.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analyses_api.py` & `curia-3.2.4/src/curia/api/test/test_analyses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis.py` & `curia-3.2.4/src/curia/api/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_config.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_output.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_output_joined_analysis_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_output_joined_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_outputs_api.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_status.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_statuses_api.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_job_type.py` & `curia-3.2.4/src/curia/api/test/test_analysis_job_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_jobs_api.py` & `curia-3.2.4/src/curia/api/test/test_analysis_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_analysis_type.py` & `curia-3.2.4/src/curia/api/test/test_analysis_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_any_of_arithmetic_expression_value.py` & `curia-3.2.4/src/curia/api/test/test_any_of_arithmetic_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_any_of_boolean_expression_value.py` & `curia-3.2.4/src/curia/api/test/test_any_of_boolean_expression_value.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py` & `curia-3.2.4/src/curia/api/test/test_any_of_cohort_definition_patient_metadata_filters_items.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_any_of_condition_value.py` & `curia-3.2.4/src/curia/api/test/test_any_of_condition_value.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_arithmetic_expression.py` & `curia-3.2.4/src/curia/api/test/test_arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_arithmetic_operator.py` & `curia-3.2.4/src/curia/api/test/test_arithmetic_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_body.py` & `curia-3.2.4/src/curia/api/test/test_body.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_body1.py` & `curia-3.2.4/src/curia/api/test/test_body1.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_body2.py` & `curia-3.2.4/src/curia/api/test/test_body2.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_body3.py` & `curia-3.2.4/src/curia/api/test/test_body3.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_boolean_expression.py` & `curia-3.2.4/src/curia/api/test/test_boolean_expression.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_code.py` & `curia-3.2.4/src/curia/api/test/test_code.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort.py` & `curia-3.2.4/src/curia/api/test/test_cohort.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_definition.py` & `curia-3.2.4/src/curia/api/test/test_cohort_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_filter.py` & `curia-3.2.4/src/curia/api/test/test_cohort_filter.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_filter_condition.py` & `curia-3.2.4/src/curia/api/test/test_cohort_filter_condition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_cohort_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_results.py` & `curia-3.2.4/src/curia/api/test/test_cohort_results.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_set.py` & `curia-3.2.4/src/curia/api/test/test_cohort_set.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohort_window.py` & `curia-3.2.4/src/curia/api/test/test_cohort_window.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_cohorts_api.py` & `curia-3.2.4/src/curia/api/test/test_cohorts_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_condition.py` & `curia-3.2.4/src/curia/api/test/test_condition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_condition_operator.py` & `curia-3.2.4/src/curia/api/test/test_condition_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_analysis_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_analysis_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_analysis_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_analysis_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_cohort_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_data_query_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_data_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_data_table_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_database_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_dataset_column_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_dataset_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_feature_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_feature_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_analysis_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_analysis_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_analysis_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_analysis_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_code_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_code_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_cohort_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_data_query_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_data_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_dataset_column_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_dataset_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_dataset_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_dataset_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_environment_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_environment_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_feature_category_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_feature_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_feature_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_feature_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_feature_sub_category_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_feature_sub_category_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_batch_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_batch_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_dataset_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_endpoint_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_endpoint_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_job_output_feature_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_job_output_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_model_population_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_organization_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_organization_feature_exclusion_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_organization_setting_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_population_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_process_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_process_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_process_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_process_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_project_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_project_member_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_scheduler_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_task_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_task_execution_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_task_execution_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_user_favorite_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_workflow_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_workflow_execution_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_many_workflow_template_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_many_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_model_batch_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_model_batch_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_model_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_model_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_model_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_model_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_model_population_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_organization_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_organization_setting_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_population_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_process_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_process_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_process_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_process_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_project_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_project_member_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_scheduler_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_task_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_task_execution_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_task_execution_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_user_audit_trail_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_user_favorite_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_workflow_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_workflow_execution_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_workflow_execution_spec_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_workflow_execution_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_create_workflow_template_dto.py` & `curia-3.2.4/src/curia/api/test/test_create_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_queries_api.py` & `curia-3.2.4/src/curia/api/test/test_data_queries_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_query.py` & `curia-3.2.4/src/curia/api/test/test_data_query.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_query_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_store.py` & `curia-3.2.4/src/curia/api/test/test_data_store.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_store_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_stores_api.py` & `curia-3.2.4/src/curia/api/test/test_data_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_table.py` & `curia-3.2.4/src/curia/api/test/test_data_table.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_table_joined_database_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_data_table_joined_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_table_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_data_table_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_table_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_data_tables_api.py` & `curia-3.2.4/src/curia/api/test/test_data_tables_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_database.py` & `curia-3.2.4/src/curia/api/test/test_database.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_database_joined_data_table_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_database_joined_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_database_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_databases_api.py` & `curia-3.2.4/src/curia/api/test/test_databases_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset.py` & `curia-3.2.4/src/curia/api/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_column.py` & `curia-3.2.4/src/curia/api/test/test_dataset_column.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_dataset_column_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_column_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_columns_api.py` & `curia-3.2.4/src/curia/api/test/test_dataset_columns_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_job.py` & `curia-3.2.4/src/curia/api/test/test_dataset_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_job_status.py` & `curia-3.2.4/src/curia/api/test/test_dataset_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_dataset_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_dataset_joined_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_datasets_api.py` & `curia-3.2.4/src/curia/api/test/test_datasets_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py` & `curia-3.2.4/src/curia/api/test/test_datasetsuploadlargecomplete_parts.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_environment.py` & `curia-3.2.4/src/curia/api/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_environment_activity.py` & `curia-3.2.4/src/curia/api/test/test_environment_activity.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature.py` & `curia-3.2.4/src/curia/api/test/test_feature.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_category.py` & `curia-3.2.4/src/curia/api/test/test_feature_category.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_feature_joined_feature_sub_category_joined_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_feature_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_joined_model_population_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_feature_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_feature_joined_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_store.py` & `curia-3.2.4/src/curia/api/test/test_feature_store.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_store_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_stores_api.py` & `curia-3.2.4/src/curia/api/test/test_feature_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_sub_category.py` & `curia-3.2.4/src/curia/api/test/test_feature_sub_category.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_feature_table.py` & `curia-3.2.4/src/curia/api/test/test_feature_table.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_features_api.py` & `curia-3.2.4/src/curia/api/test/test_features_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_geographic_counts.py` & `curia-3.2.4/src/curia/api/test/test_geographic_counts.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_geographic_queries.py` & `curia-3.2.4/src/curia/api/test/test_geographic_queries.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_analysis_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_analysis_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_analysis_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_analysis_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_analysis_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_analysis_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_code_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_code_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_data_store_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_data_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_data_table_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_data_table_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_database_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_database_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_dataset_column_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_dataset_column_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_dataset_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_dataset_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_dataset_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_environment_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_environment_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_feature_category_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_feature_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_feature_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_feature_store_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_feature_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_batch_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_batch_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_endpoint_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_endpoint_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_job_event_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_job_event_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_job_output_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_population_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_model_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_organization_feature_exclusion_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_organization_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_organization_setting_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_population_store_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_process_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_process_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_process_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_process_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_project_member_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_scheduler_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_task_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_task_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_task_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_workflow_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_get_many_workflow_template_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_get_many_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_inline_response200.py` & `curia-3.2.4/src/curia/api/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_inline_response200_info.py` & `curia-3.2.4/src/curia/api/test/test_inline_response200_info.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_inline_response503.py` & `curia-3.2.4/src/curia/api/test/test_inline_response503.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_internal_api.py` & `curia-3.2.4/src/curia/api/test/test_internal_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_intervention_definition.py` & `curia-3.2.4/src/curia/api/test/test_intervention_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_json.py` & `curia-3.2.4/src/curia/api/test/test_json.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_logical_operator.py` & `curia-3.2.4/src/curia/api/test/test_logical_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model.py` & `curia-3.2.4/src/curia/api/test/test_model.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch.py` & `curia-3.2.4/src/curia/api/test/test_model_batch.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch_job.py` & `curia-3.2.4/src/curia/api/test/test_model_batch_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_batch_job_joined_model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_batch_job_joined_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_batch_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch_jobs_api.py` & `curia-3.2.4/src/curia/api/test/test_model_batch_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_batch_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batch_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_batch_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_batches_api.py` & `curia-3.2.4/src/curia/api/test/test_model_batches_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_dataset.py` & `curia-3.2.4/src/curia/api/test/test_model_dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_endpoint.py` & `curia-3.2.4/src/curia/api/test/test_model_endpoint.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job.py` & `curia-3.2.4/src/curia/api/test/test_model_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_config.py` & `curia-3.2.4/src/curia/api/test/test_model_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_event.py` & `curia-3.2.4/src/curia/api/test/test_model_job_event.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_population_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_output.py` & `curia-3.2.4/src/curia/api/test/test_model_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_output_feature.py` & `curia-3.2.4/src/curia/api/test/test_model_job_output_feature.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_output_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_output_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_output_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_outputs_api.py` & `curia-3.2.4/src/curia/api/test/test_model_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_status.py` & `curia-3.2.4/src/curia/api/test/test_model_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_status_joined_model_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_status_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_job_statuses_api.py` & `curia-3.2.4/src/curia/api/test/test_model_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_jobs_api.py` & `curia-3.2.4/src/curia/api/test/test_model_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_cohort_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_model_job_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_model_job_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_model_job_joined_feature_sub_category_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_model_output_details_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_model_output_details_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_joined_user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_output_details.py` & `curia-3.2.4/src/curia/api/test/test_model_output_details.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population.py` & `curia-3.2.4/src/curia/api/test/test_model_population.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_cohort_definition_joined_period_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_cohort_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_cohort_results_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_data_query_joined_dataset_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_data_query_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_data_query_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_feature_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_feature_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_intervention_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_model_job_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_model_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_model_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_joined_outcome_definition_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_population_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_population_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_populations_api.py` & `curia-3.2.4/src/curia/api/test/test_model_populations_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_model_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_models_api.py` & `curia-3.2.4/src/curia/api/test/test_models_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_object.py` & `curia-3.2.4/src/curia/api/test/test_object.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organization.py` & `curia-3.2.4/src/curia/api/test/test_organization.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organization_feature_category_exclusion.py` & `curia-3.2.4/src/curia/api/test/test_organization_feature_category_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organization_feature_exclusion.py` & `curia-3.2.4/src/curia/api/test/test_organization_feature_exclusion.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organization_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_organization_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organization_setting.py` & `curia-3.2.4/src/curia/api/test/test_organization_setting.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organization_setting_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_organization_setting_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organization_settings_api.py` & `curia-3.2.4/src/curia/api/test/test_organization_settings_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_organizations_api.py` & `curia-3.2.4/src/curia/api/test/test_organizations_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_outcome_definition.py` & `curia-3.2.4/src/curia/api/test/test_outcome_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_period_definition.py` & `curia-3.2.4/src/curia/api/test/test_period_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_period_type.py` & `curia-3.2.4/src/curia/api/test/test_period_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_person_set.py` & `curia-3.2.4/src/curia/api/test/test_person_set.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_platform_api.py` & `curia-3.2.4/src/curia/api/test/test_platform_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_population.py` & `curia-3.2.4/src/curia/api/test/test_population.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_population_store.py` & `curia-3.2.4/src/curia/api/test/test_population_store.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_population_store_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_population_store_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_population_stores_api.py` & `curia-3.2.4/src/curia/api/test/test_population_stores_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process.py` & `curia-3.2.4/src/curia/api/test/test_process.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job.py` & `curia-3.2.4/src/curia/api/test/test_process_job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_config.py` & `curia-3.2.4/src/curia/api/test/test_process_job_config.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_output.py` & `curia-3.2.4/src/curia/api/test/test_process_job_output.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_job_output_joined_process_job_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_job_output_joined_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_output_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_job_output_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_outputs_api.py` & `curia-3.2.4/src/curia/api/test/test_process_job_outputs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_job_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_status.py` & `curia-3.2.4/src/curia/api/test/test_process_job_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_status_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_job_status_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_job_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_job_statuses_api.py` & `curia-3.2.4/src/curia/api/test/test_process_job_statuses_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_jobs_api.py` & `curia-3.2.4/src/curia/api/test/test_process_jobs_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_process_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_process_type.py` & `curia-3.2.4/src/curia/api/test/test_process_type.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_processes_api.py` & `curia-3.2.4/src/curia/api/test/test_processes_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project.py` & `curia-3.2.4/src/curia/api/test/test_project.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_project_joined_model_joined_cohort_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_project_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_project_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_joined_user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_project_joined_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_member.py` & `curia-3.2.4/src/curia/api/test/test_project_member.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_member_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_project_member_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_member_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_project_member_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_members_api.py` & `curia-3.2.4/src/curia/api/test/test_project_members_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_projects_api.py` & `curia-3.2.4/src/curia/api/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_scheduler.py` & `curia-3.2.4/src/curia/api/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_scheduler_api.py` & `curia-3.2.4/src/curia/api/test/test_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_scheduler_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_select_expression.py` & `curia-3.2.4/src/curia/api/test/test_select_expression.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_set_operator.py` & `curia-3.2.4/src/curia/api/test/test_set_operator.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_state_data.py` & `curia-3.2.4/src/curia/api/test/test_state_data.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task.py` & `curia-3.2.4/src/curia/api/test/test_task.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution.py` & `curia-3.2.4/src/curia/api/test/test_task_execution.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution_joined_task_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_task_execution_joined_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution_status.py` & `curia-3.2.4/src/curia/api/test/test_task_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_task_execution_status_joined_task_execution_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_task_execution_status_joined_task_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_task_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_inputs.py` & `curia-3.2.4/src/curia/api/test/test_task_inputs.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_outputs.py` & `curia-3.2.4/src/curia/api/test/test_task_outputs.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_task_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_task_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_analysis_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_analysis_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_analysis_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_analysis_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_analysis_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_analysis_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_analysis_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_analysis_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_cohort_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_cohort_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_data_query_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_data_query_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_data_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_data_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_data_table_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_data_table_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_database_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_database_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_dataset_column_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_dataset_column_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_dataset_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_dataset_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_feature_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_feature_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_feature_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_feature_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_model_batch_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_model_batch_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_model_batch_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_model_batch_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_model_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_model_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_model_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_model_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_model_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_model_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_model_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_model_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_model_population_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_model_population_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_organization_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_organization_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_organization_setting_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_organization_setting_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_population_store_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_population_store_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_process_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_process_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_process_job_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_process_job_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_process_job_output_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_process_job_output_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_process_job_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_process_job_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_project_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_project_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_project_member_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_project_member_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_scheduler_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_scheduler_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_task_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_task_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_task_execution_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_task_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_task_execution_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_task_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_user_audit_trail_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_user_audit_trail_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_user_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_user_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_user_favorite_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_user_favorite_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_workflow_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_workflow_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_workflow_execution_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_workflow_execution_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_workflow_execution_spec_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_workflow_execution_spec_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_workflow_execution_status_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_workflow_execution_status_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_update_workflow_template_dto.py` & `curia-3.2.4/src/curia/api/test/test_update_workflow_template_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_audit_trail.py` & `curia-3.2.4/src/curia/api/test/test_user_audit_trail.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_audit_trail_api.py` & `curia-3.2.4/src/curia/api/test/test_user_audit_trail_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_audit_trail_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_user_audit_trail_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_favorite.py` & `curia-3.2.4/src/curia/api/test/test_user_favorite.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_user_favorite_joined_model_joined_project_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_favorite_joined_model_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_user_favorite_joined_model_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_favorite_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_user_favorite_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_favorites_api.py` & `curia-3.2.4/src/curia/api/test/test_user_favorites_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_user_management_api.py` & `curia-3.2.4/src/curia/api/test/test_user_management_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow.py` & `curia-3.2.4/src/curia/api/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution_spec.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution_spec.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution_spec_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution_spec_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution_spec_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution_status.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution_status.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution_status_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_execution_status_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_execution_status_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_joined_scheduler_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_joined_workflow_execution_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_joined_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_template.py` & `curia-3.2.4/src/curia/api/test/test_workflow_template.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_template_definition.py` & `curia-3.2.4/src/curia/api/test/test_workflow_template_definition.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_template_parameters.py` & `curia-3.2.4/src/curia/api/test/test_workflow_template_parameters.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflow_template_response_dto.py` & `curia-3.2.4/src/curia/api/test/test_workflow_template_response_dto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_workflows_api.py` & `curia-3.2.4/src/curia/api/test/test_workflows_api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/api/test/test_zip_data.py` & `curia-3.2.4/src/curia/api/test/test_zip_data.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/mock/api.py` & `curia-3.2.4/src/curia/mock/api.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/mock/api_server.py` & `curia-3.2.4/src/curia/mock/api_server.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/mock/moto.py` & `curia-3.2.4/src/curia/mock/moto.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/mock/s3.py` & `curia-3.2.4/src/curia/mock/s3.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/mock/server.py` & `curia-3.2.4/src/curia/mock/server.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/session.py` & `curia-3.2.4/src/curia/session.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/synthetic_data.py` & `curia-3.2.4/src/curia/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/utils/dataset.py` & `curia-3.2.4/src/curia/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/utils/job.py` & `curia-3.2.4/src/curia/utils/job.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/utils/python.py` & `curia-3.2.4/src/curia/utils/python.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/utils/s3.py` & `curia-3.2.4/src/curia/utils/s3.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia/utils/string.py` & `curia-3.2.4/src/curia/utils/string.py`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/src/curia.egg-info/PKG-INFO` & `curia-3.2.4/src/curia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curia
-Version: 3.2.3
+Version: 3.2.4
 Summary: A library for training and using risk & impactability models on Curia
 Home-page: https://github.com/Curia-ai/curia-python-sdk
 Author: Curia.ai
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `curia-3.2.3/src/curia.egg-info/SOURCES.txt` & `curia-3.2.4/src/curia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curia-3.2.3/test/test_synthetic_data.py` & `curia-3.2.4/test/test_synthetic_data.py`

 * *Files identical despite different names*

