# Comparing `tmp/whylabs-client-0.4.7.tar.gz` & `tmp/whylabs-client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.4.7.tar", last modified: Fri Apr 28 00:36:10 2023, max compression
+gzip compressed data, was "whylabs-client-0.5.0.tar", last modified: Tue May  2 15:18:36 2023, max compression
```

## Comparing `whylabs-client-0.4.7.tar` & `whylabs-client-0.5.0.tar`

### file list

```diff
@@ -1,154 +1,156 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/
--rw-r--r--   0 root         (0) root         (0)     3358 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    23249 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-28 00:36:10.881926 whylabs-client-0.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-04-28 00:36:09.000000 whylabs-client-0.4.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.830922 whylabs-client-0.4.7/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.836923 whylabs-client-0.4.7/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    28878 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20727 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    67177 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52337 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    48204 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    29965 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37575 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.836923 whylabs-client-0.4.7/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17084 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12005 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11342 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/batch_log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11655 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/batch_log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12443 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11207 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13099 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/databricks_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dataset_request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/datatype_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/distribution_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_auto_scale_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13257 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_attributes_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11739 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_availability_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11804 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12362 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_s3_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11745 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_ebs_volume_type_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_cron_schedule_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11934 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_data_security_mode_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11969 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12404 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_email_notifications_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    16133 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_settings_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    16932 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_new_cluster_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11603 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_notebook_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11707 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_jar_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_python_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11293 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_submit_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12313 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12718 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_search_result.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11507 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11411 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11485 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11379 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_monitor_config_v2_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_jobs_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11289 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_jobs_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11502 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11858 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11441 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12111 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11756 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12260 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/metric_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11120 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/missing_recent_data_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11132 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/missing_recent_profiles_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/missing_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    12569 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12219 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11783 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11982 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14425 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13737 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12319 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provided_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11680 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11657 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12387 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11188 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/refresh_access_token_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11444 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/refresh_connection_by_org_id_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11586 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/refresh_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13668 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11112 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13372 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/request_feature_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15325 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11922 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/run_job_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11089 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/run_job_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11471 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/search_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/seasonal_arima_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11948 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11652 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11670 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11917 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/unique_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/update_connection_changes.py
--rw-rw-rw-   0 root         (0) root         (0)    11816 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/update_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    13667 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/why_logs_metric.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)     9913 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.832923 whylabs-client-0.4.7/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3358 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6694 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    23347 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-02 15:18:36.518487 whylabs-client-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-05-02 15:18:35.000000 whylabs-client-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.469483 whylabs-client-0.5.0/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.475484 whylabs-client-0.5.0/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    28878 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20727 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    67177 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52337 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    48204 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    29965 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37575 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.476484 whylabs-client-0.5.0/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17084 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12005 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/batch_log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11655 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/batch_log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12443 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11207 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13099 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/databricks_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dataset_request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/datatype_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/distribution_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_auto_scale_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13257 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_attributes_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11739 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_availability_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11804 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_s3_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11745 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_ebs_volume_type_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_cron_schedule_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11934 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_data_security_mode_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11969 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_email_notifications_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16133 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_settings_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_new_cluster_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11603 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_notebook_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11707 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_jar_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_python_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11293 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_submit_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12313 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12718 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_search_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11507 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11411 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11379 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_monitor_config_v2_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_jobs_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11289 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_jobs_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11502 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11858 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11441 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12111 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11756 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11120 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/missing_recent_data_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11132 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/missing_recent_profiles_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/missing_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12569 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12219 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11783 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11982 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14425 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13737 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12319 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provided_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11680 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12387 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11188 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/refresh_access_token_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11444 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/refresh_connection_by_org_id_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11586 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/refresh_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13668 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11112 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13372 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/request_feature_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15325 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11922 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/run_job_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11089 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/run_job_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11471 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11447 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/search_index_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11787 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/search_index_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/search_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/seasonal_arima_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11948 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11652 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11610 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/unique_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/update_connection_changes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11816 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/update_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    13667 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/why_logs_metric.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10053 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.471484 whylabs-client-0.5.0/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6781 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.4.7/PKG-INFO` & `whylabs-client-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.4.7
+Version: 0.5.0
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.4.7/README.md` & `whylabs-client-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.4.7
+- Package version: 0.5.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -250,14 +250,16 @@
  - [RequestFeatureMonitorConfig](docs/RequestFeatureMonitorConfig.md)
  - [RequestMonitorConfig](docs/RequestMonitorConfig.md)
  - [Response](docs/Response.md)
  - [Role](docs/Role.md)
  - [RunJobRequest](docs/RunJobRequest.md)
  - [RunJobResponse](docs/RunJobResponse.md)
  - [SchemaMetadata](docs/SchemaMetadata.md)
+ - [SearchIndexRequest](docs/SearchIndexRequest.md)
+ - [SearchIndexType](docs/SearchIndexType.md)
  - [SearchResponse](docs/SearchResponse.md)
  - [SeasonalARIMARequestConfig](docs/SeasonalARIMARequestConfig.md)
  - [Segment](docs/Segment.md)
  - [SegmentTag](docs/SegmentTag.md)
  - [SegmentWeight](docs/SegmentWeight.md)
  - [SessionMetadata](docs/SessionMetadata.md)
  - [SetDefaultMembershipRequest](docs/SetDefaultMembershipRequest.md)
```

### Comparing `whylabs-client-0.4.7/setup.py` & `whylabs-client-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "RELEASE.md").read_text()
 
 NAME = "whylabs-client"
-VERSION = "0.4.7"
+VERSION = "0.5.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `whylabs-client-0.4.7/whylabs_client/__init__.py` & `whylabs-client-0.5.0/whylabs_client/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.7"
+__version__ = "0.5.0"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.4.7/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.5.0/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.5.0/whylabs_client/api/dataset_profile_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.5.0/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/log_api.py` & `whylabs-client-0.5.0/whylabs_client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/membership_api.py` & `whylabs-client-0.5.0/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/models_api.py` & `whylabs-client-0.5.0/whylabs_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/monitor_api.py` & `whylabs-client-0.5.0/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.5.0/whylabs_client/api/notification_settings_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/schema_api.py` & `whylabs-client-0.5.0/whylabs_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api/sessions_api.py` & `whylabs-client-0.5.0/whylabs_client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/api_client.py` & `whylabs-client-0.5.0/whylabs_client/api_client.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/apis/__init__.py` & `whylabs-client-0.5.0/whylabs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/configuration.py` & `whylabs-client-0.5.0/whylabs_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.4.7".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.4.7/whylabs_client/exceptions.py` & `whylabs-client-0.5.0/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/action_type.py` & `whylabs-client-0.5.0/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.5.0/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/async_log_response.py` & `whylabs-client-0.5.0/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.5.0/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/batch_log_reference_request.py` & `whylabs-client-0.5.0/whylabs_client/model/batch_log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/batch_log_session_reference_response.py` & `whylabs-client-0.5.0/whylabs_client/model/batch_log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/column_schema.py` & `whylabs-client-0.5.0/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/create_session_request.py` & `whylabs-client-0.5.0/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/create_session_response.py` & `whylabs-client-0.5.0/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/create_user_request.py` & `whylabs-client-0.5.0/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/databricks_connection.py` & `whylabs-client-0.5.0/whylabs_client/model/databricks_connection.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dataset_request_monitor_config.py` & `whylabs-client-0.5.0/whylabs_client/model/dataset_request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/datatype_monitor_request_config.py` & `whylabs-client-0.5.0/whylabs_client/model/datatype_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.5.0/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.5.0/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/distribution_monitor_request_config.py` & `whylabs-client-0.5.0/whylabs_client/model/distribution_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_auto_scale_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_auto_scale_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_attributes_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_attributes_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_availability_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_availability_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_s3_storage_info_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_s3_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_ebs_volume_type_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_ebs_volume_type_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_cron_schedule_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_cron_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_data_security_mode_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_data_security_mode_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_email_notifications_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_email_notifications_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_settings_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_settings_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_new_cluster_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_new_cluster_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_notebook_task_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_notebook_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_jar_task_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_jar_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_python_task_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_python_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_submit_task_dto.py` & `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_submit_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.5.0/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/entity_schema.py` & `whylabs-client-0.5.0/whylabs_client/model/entity_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/entity_search_result.py` & `whylabs-client-0.5.0/whylabs_client/model/entity_search_result.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.5.0/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.5.0/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/feature_flags.py` & `whylabs-client-0.5.0/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_connection_request.py` & `whylabs-client-0.5.0/whylabs_client/model/get_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_connection_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_monitor_config_v2_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_monitor_config_v2_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/get_session_response.py` & `whylabs-client-0.5.0/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/list_jobs_request.py` & `whylabs-client-0.5.0/whylabs_client/model/list_jobs_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/list_jobs_response.py` & `whylabs-client-0.5.0/whylabs_client/model/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/list_models_response.py` & `whylabs-client-0.5.0/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.5.0/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.5.0/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/log_async_request.py` & `whylabs-client-0.5.0/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.5.0/whylabs_client/model/log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.5.0/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/log_response.py` & `whylabs-client-0.5.0/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/log_session_reference_response.py` & `whylabs-client-0.5.0/whylabs_client/model/log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.5.0/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/membership.py` & `whylabs-client-0.5.0/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.5.0/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/metric_schema.py` & `whylabs-client-0.5.0/whylabs_client/model/metric_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/missing_recent_data_request_config.py` & `whylabs-client-0.5.0/whylabs_client/model/missing_recent_data_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/missing_recent_profiles_request_config.py` & `whylabs-client-0.5.0/whylabs_client/model/missing_recent_profiles_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/missing_values_monitor_request_config.py` & `whylabs-client-0.5.0/whylabs_client/model/missing_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.5.0/whylabs_client/model/model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/model_type.py` & `whylabs-client-0.5.0/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/monitor_config.py` & `whylabs-client-0.5.0/whylabs_client/model/monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.5.0/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference.py` & `whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference_type.py` & `whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/notification_action.py` & `whylabs-client-0.5.0/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/notification_settings.py` & `whylabs-client-0.5.0/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.5.0/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.5.0/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.5.0/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/organization_summary.py` & `whylabs-client-0.5.0/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.5.0/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/provided_config.py` & `whylabs-client-0.5.0/whylabs_client/model/provided_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_request.py` & `whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_response.py` & `whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.5.0/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.5.0/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.5.0/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.5.0/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.5.0/whylabs_client/model/reference_profile_item_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/refresh_access_token_request.py` & `whylabs-client-0.5.0/whylabs_client/model/refresh_access_token_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/refresh_connection_by_org_id_response.py` & `whylabs-client-0.5.0/whylabs_client/model/refresh_connection_by_org_id_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/refresh_connection_request.py` & `whylabs-client-0.5.0/whylabs_client/model/refresh_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_request.py` & `whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_response.py` & `whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.5.0/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/request_feature_monitor_config.py` & `whylabs-client-0.5.0/whylabs_client/model/request_feature_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/request_monitor_config.py` & `whylabs-client-0.5.0/whylabs_client/model/request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/response.py` & `whylabs-client-0.5.0/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/role.py` & `whylabs-client-0.5.0/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/run_job_request.py` & `whylabs-client-0.5.0/whylabs_client/model/run_job_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/run_job_response.py` & `whylabs-client-0.5.0/whylabs_client/model/run_job_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.5.0/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/search_response.py` & `whylabs-client-0.5.0/whylabs_client/model/search_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/seasonal_arima_request_config.py` & `whylabs-client-0.5.0/whylabs_client/model/seasonal_arima_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/segment.py` & `whylabs-client-0.5.0/whylabs_client/model/segment.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/segment_tag.py` & `whylabs-client-0.5.0/whylabs_client/model/segment_tag.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/segment_weight.py` & `whylabs-client-0.5.0/whylabs_client/model/segment_weight.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/session_metadata.py` & `whylabs-client-0.5.0/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.5.0/whylabs_client/model/set_default_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.5.0/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.5.0/whylabs_client/model/subscription_tier.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/time_period.py` & `whylabs-client-0.5.0/whylabs_client/model/time_period.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
     allowed_values = {
         ('value',): {
             'P1M': "P1M",
             'P1W': "P1W",
             'P1D': "P1D",
             'PT1H': "PT1H",
-            'PT5M': "PT5M",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -105,18 +104,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """TimePeriod - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", "PT5M", ]  # noqa: E501
+            args[0] (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", "PT5M", ]  # noqa: E501
+            value (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -195,18 +194,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """TimePeriod - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", "PT5M", ]  # noqa: E501
+            args[0] (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", "PT5M", ]  # noqa: E501
+            value (str):, must be one of ["P1M", "P1W", "P1D", "PT1H", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `whylabs-client-0.4.7/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.5.0/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/unique_values_monitor_request_config.py` & `whylabs-client-0.5.0/whylabs_client/model/unique_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/update_connection_changes.py` & `whylabs-client-0.5.0/whylabs_client/model/update_connection_changes.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/update_connection_request.py` & `whylabs-client-0.5.0/whylabs_client/model/update_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.5.0/whylabs_client/model/update_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/user.py` & `whylabs-client-0.5.0/whylabs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/user_api_key.py` & `whylabs-client-0.5.0/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.5.0/whylabs_client/model/user_api_key_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model/why_logs_metric.py` & `whylabs-client-0.5.0/whylabs_client/model/why_logs_metric.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/model_utils.py` & `whylabs-client-0.5.0/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client/models/__init__.py` & `whylabs-client-0.5.0/whylabs_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 from whylabs_client.model.request_feature_monitor_config import RequestFeatureMonitorConfig
 from whylabs_client.model.request_monitor_config import RequestMonitorConfig
 from whylabs_client.model.response import Response
 from whylabs_client.model.role import Role
 from whylabs_client.model.run_job_request import RunJobRequest
 from whylabs_client.model.run_job_response import RunJobResponse
 from whylabs_client.model.schema_metadata import SchemaMetadata
+from whylabs_client.model.search_index_request import SearchIndexRequest
+from whylabs_client.model.search_index_type import SearchIndexType
 from whylabs_client.model.search_response import SearchResponse
 from whylabs_client.model.seasonal_arima_request_config import SeasonalARIMARequestConfig
 from whylabs_client.model.segment import Segment
 from whylabs_client.model.segment_tag import SegmentTag
 from whylabs_client.model.segment_weight import SegmentWeight
 from whylabs_client.model.session_metadata import SessionMetadata
 from whylabs_client.model.set_default_membership_request import SetDefaultMembershipRequest
```

### Comparing `whylabs-client-0.4.7/whylabs_client/rest.py` & `whylabs-client-0.5.0/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.7/whylabs_client.egg-info/PKG-INFO` & `whylabs-client-0.5.0/whylabs_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.4.7
+Version: 0.5.0
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.4.7/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.5.0/whylabs_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,16 @@
 whylabs_client/model/request_feature_monitor_config.py
 whylabs_client/model/request_monitor_config.py
 whylabs_client/model/response.py
 whylabs_client/model/role.py
 whylabs_client/model/run_job_request.py
 whylabs_client/model/run_job_response.py
 whylabs_client/model/schema_metadata.py
+whylabs_client/model/search_index_request.py
+whylabs_client/model/search_index_type.py
 whylabs_client/model/search_response.py
 whylabs_client/model/seasonal_arima_request_config.py
 whylabs_client/model/segment.py
 whylabs_client/model/segment_tag.py
 whylabs_client/model/segment_weight.py
 whylabs_client/model/session_metadata.py
 whylabs_client/model/set_default_membership_request.py
```

