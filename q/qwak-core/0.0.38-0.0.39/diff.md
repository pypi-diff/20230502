# Comparing `tmp/qwak_core-0.0.38.tar.gz` & `tmp/qwak_core-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.38.tar", max compression
+gzip compressed data, was "qwak_core-0.0.39.tar", max compression
```

## Comparing `qwak_core-0.0.38.tar` & `qwak_core-0.0.39.tar`

### file list

```diff
@@ -1,543 +1,543 @@
--rw-r--r--   0        0        0      264 2023-05-01 12:10:43.828490 qwak_core-0.0.38/README.md
--rw-r--r--   0        0        0        0 2023-05-01 12:11:50.676659 qwak_core-0.0.38/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-01 12:11:50.704659 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-01 12:11:30.364605 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.704659 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-01 12:11:50.696659 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-01 12:11:30.004603 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.700659 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-01 12:11:50.700659 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-01 12:11:30.184604 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.700659 qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-01 12:11:50.692659 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-01 12:11:29.456599 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-01 12:11:50.692659 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-01 12:11:50.692659 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-01 12:11:29.640600 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.696659 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-01 12:11:50.696659 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-01 12:11:29.824601 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.696659 qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-01 12:11:50.676659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-01 12:11:29.276599 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-01 12:11:50.680659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-01 12:11:50.680659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-01 12:11:30.552606 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.680659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-01 12:11:50.684659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-01 12:11:30.932609 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.684659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-01 12:11:50.688659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-01 12:11:31.120611 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-01 12:11:50.688659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-01 12:11:50.680659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-01 12:11:30.744608 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.684659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-01 12:11:50.688659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-01 12:11:31.300612 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.688659 qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-01 12:11:50.736659 qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-01 12:11:33.852629 qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.736659 qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-01 12:11:50.736659 qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-01 12:11:34.036629 qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-01 12:11:50.736659 qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-01 12:11:50.804659 qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-01 12:11:39.036638 qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.804659 qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-01 12:11:50.808659 qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-01 12:11:39.216638 qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-01 12:11:50.808659 qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-01 12:11:50.812659 qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-01 12:11:40.140640 qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-01 12:11:50.812659 qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-01 12:11:50.808659 qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-01 12:11:39.956640 qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.808659 qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-01 12:11:50.812659 qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-01 12:11:40.320640 qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.816659 qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-01 12:11:50.816659 qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-01 12:11:40.500641 qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-01 12:11:50.816659 qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-05-01 12:11:50.880659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-05-01 12:11:46.176651 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.880659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-01 12:11:50.876659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-01 12:11:45.796650 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.876659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-01 12:11:50.876659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-01 12:11:45.988650 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.880659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-01 12:11:50.872659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-01 12:11:45.400649 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-01 12:11:50.872659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-01 12:11:50.872659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-01 12:11:45.604650 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.876659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-01 12:11:50.888659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-01 12:11:46.724652 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.888659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-01 12:11:50.884659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-01 12:11:46.544651 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.884659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-01 12:11:50.884659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-01 12:11:46.360651 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.884659 qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-01 12:11:50.928659 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-01 12:11:50.028658 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.928659 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-01 12:11:50.924659 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-01 12:11:49.652657 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.924659 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-05-01 12:11:50.924659 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-05-01 12:11:49.844657 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-01 12:11:50.928659 qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-01 12:11:50.844659 qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-01 12:11:42.432644 qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-01 12:11:50.844659 qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-01 12:11:50.840659 qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-01 12:11:42.232644 qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.844659 qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-01 12:11:50.832659 qwak_core-0.0.38/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-01 12:11:41.828643 qwak_core-0.0.38/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.832659 qwak_core-0.0.38/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-01 12:11:50.836659 qwak_core-0.0.38/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-01 12:11:42.024644 qwak_core-0.0.38/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.836659 qwak_core-0.0.38/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-01 12:11:50.836659 qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-01 12:11:42.636644 qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-01 12:11:50.836659 qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-01 12:11:50.840659 qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-01 12:11:43.120645 qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-01 12:11:50.840659 qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-01 12:11:50.852659 qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-01 12:11:43.556646 qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.852659 qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-01 12:11:50.852659 qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-01 12:11:43.760646 qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-01 12:11:50.852659 qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-01 12:11:50.824659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-01 12:11:41.260642 qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.824659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-01 12:11:50.828659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-01 12:11:41.444642 qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-01 12:11:50.828659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-01 12:11:50.820659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-01 12:11:40.884642 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.820659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-01 12:11:50.816659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-01 12:11:40.696641 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.820659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-01 12:11:50.824659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-01 12:11:41.076642 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-01 12:11:50.824659 qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-01 12:11:50.724659 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-01 12:11:32.936624 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.724659 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-01 12:11:50.724659 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-01 12:11:33.120625 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.728659 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-01 12:11:50.728659 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-01 12:11:33.304626 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-01 12:11:50.728659 qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-01 12:11:50.784659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-01 12:11:37.940636 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.784659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-01 12:11:50.780659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-01 12:11:37.736636 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-01 12:11:50.784659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-01 12:11:50.764659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-01 12:11:36.264633 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.764659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-01 12:11:50.760659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-01 12:11:36.080633 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.764659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-01 12:11:50.756659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-01 12:11:35.508632 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.756659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-01 12:11:50.760659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-01 12:11:35.896633 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-01 12:11:50.760659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-01 12:11:50.764659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-01 12:11:36.448634 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.768659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-01 12:11:50.768659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-01 12:11:36.632634 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-01 12:11:50.768659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-05-01 12:11:50.756659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-05-01 12:11:35.704632 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.756659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-01 12:11:50.772659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-01 12:11:36.808634 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.772659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-01 12:11:50.788659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-01 12:11:50.212658 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.788659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-01 12:11:50.788659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-01 12:11:50.396658 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-01 12:11:50.788659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-01 12:11:50.792659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-01 12:11:38.488637 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.792659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-01 12:11:50.792659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-01 12:11:38.672638 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-01 12:11:50.796659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-01 12:11:50.796659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-01 12:11:38.852638 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.796659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-01 12:11:50.800659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-01 12:11:39.592639 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.800659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-01 12:11:50.796659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-01 12:11:39.404639 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-01 12:11:50.800659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-01 12:11:50.800659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-01 12:11:39.772639 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.804659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-01 12:11:50.772659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-01 12:11:36.992635 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.772659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-01 12:11:50.776659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-01 12:11:37.172635 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.776659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-01 12:11:50.776659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-01 12:11:37.360635 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-01 12:11:50.780659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-01 12:11:50.780659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-01 12:11:37.544636 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.780659 qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-01 12:11:50.888659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-01 12:11:46.904652 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.892659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-01 12:11:50.892659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-01 12:11:47.080652 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-01 12:11:50.892659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-01 12:11:50.892659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-01 12:11:47.260653 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.896659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-01 12:11:50.896659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-01 12:11:47.448653 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-01 12:11:50.896659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-01 12:11:50.896659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-01 12:11:47.640653 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-01 12:11:50.900659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-01 12:11:50.900659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-01 12:11:47.820654 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.900659 qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-01 12:11:50.856659 qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-01 12:11:43.968647 qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.856659 qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-01 12:11:50.856659 qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-01 12:11:44.164647 qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-01 12:11:50.860659 qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-01 12:11:50.740659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-01 12:11:34.772631 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.740659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-01 12:11:50.744659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-01 12:11:34.956631 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.744659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-01 12:11:50.748659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-01 12:11:35.136631 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-01 12:11:50.748659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-01 12:11:50.752659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-01 12:11:35.320632 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.752659 qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-01 12:11:50.828659 qwak_core-0.0.38/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-01 12:11:41.624643 qwak_core-0.0.38/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-01 12:11:50.832659 qwak_core-0.0.38/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-01 12:11:50.904659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-01 12:11:48.000654 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.904659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-01 12:11:50.904659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-01 12:11:48.176654 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.904659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-01 12:11:50.908659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-01 12:11:48.360654 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.908659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-01 12:11:50.908659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-01 12:11:48.540655 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.912659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-01 12:11:50.912659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-01 12:11:48.724655 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.912659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-01 12:11:50.912659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-01 12:11:48.924656 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-01 12:11:50.916659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-01 12:11:50.916659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-01 12:11:49.104656 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.916659 qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-01 12:11:50.860659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-01 12:11:44.564648 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.864659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-01 12:11:50.868659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-01 12:11:45.196649 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.868659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-01 12:11:50.864659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-01 12:11:44.776648 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-01 12:11:50.864659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-01 12:11:50.868659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-01 12:11:45.000649 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.868659 qwak_core-0.0.38/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-01 12:11:50.848659 qwak_core-0.0.38/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-01 12:11:43.352646 qwak_core-0.0.38/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-01 12:11:50.848659 qwak_core-0.0.38/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-01 12:11:50.720659 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-01 12:11:34.408630 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-01 12:11:50.720659 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-01 12:11:50.716659 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-01 12:11:34.224630 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.716659 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-01 12:11:50.720659 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-01 12:11:34.592630 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-01 12:11:50.720659 qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-01 12:11:50.844659 qwak_core-0.0.38/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-01 12:11:42.888645 qwak_core-0.0.38/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-01 12:11:50.848659 qwak_core-0.0.38/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-01 12:11:50.860659 qwak_core-0.0.38/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-01 12:11:44.368647 qwak_core-0.0.38/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-01 12:11:50.860659 qwak_core-0.0.38/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-01 12:11:50.712659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-01 12:11:32.212618 qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.716659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-01 12:11:50.712659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-01 12:11:32.028617 qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-01 12:11:50.712659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-01 12:11:50.704659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-01 12:11:31.484613 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.704659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-01 12:11:50.708659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-01 12:11:31.664615 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.708659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-01 12:11:50.708659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-01 12:11:31.844616 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-01 12:11:50.712659 qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-01 12:11:50.920659 qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-01 12:11:49.472657 qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-01 12:11:50.920659 qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-01 12:11:50.920659 qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-01 12:11:49.288656 qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.920659 qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-05-01 12:11:50.728659 qwak_core-0.0.38/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-05-01 12:11:33.492628 qwak_core-0.0.38/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.732659 qwak_core-0.0.38/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3001 2023-05-01 12:11:50.732659 qwak_core-0.0.38/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2574 2023-05-01 12:11:33.668629 qwak_core-0.0.38/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-01 12:11:50.732659 qwak_core-0.0.38/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2485 2023-05-01 12:11:52.448662 qwak_core-0.0.38/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-01 12:11:52.448662 qwak_core-0.0.38/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4964 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3374 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-01 12:10:43.828490 qwak_core-0.0.38/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1201 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9443 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      829 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/schema.py
--rw-r--r--   0        0        0     2964 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/schema_entities.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-01 12:10:43.832490 qwak_core-0.0.38/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5776 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-01 12:10:43.836490 qwak_core-0.0.38/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 qwak_core-0.0.38/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-02 07:35:13.306937 qwak_core-0.0.39/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 07:36:20.659238 qwak_core-0.0.39/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-02 07:36:20.683239 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-02 07:36:00.515148 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.687239 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-02 07:36:20.679239 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-02 07:36:00.151146 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.683239 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-02 07:36:20.683239 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-02 07:36:00.331147 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.683239 qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-02 07:36:20.675239 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-02 07:35:59.603144 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-02 07:36:20.675239 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-02 07:36:20.675239 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-02 07:35:59.787145 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.679239 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-02 07:36:20.679239 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-02 07:35:59.967146 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.679239 qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-02 07:36:20.663239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-02 07:35:59.415143 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-02 07:36:20.663239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-02 07:36:20.663239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-02 07:36:00.695149 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.663239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-02 07:36:20.667239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-02 07:36:01.059150 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.667239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-02 07:36:20.671239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-02 07:36:01.247151 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-02 07:36:20.671239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-02 07:36:20.667239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-02 07:36:00.879150 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.667239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-02 07:36:20.671239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-02 07:36:01.427152 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.675239 qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-02 07:36:20.715239 qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-02 07:36:04.007164 qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.715239 qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-02 07:36:20.719239 qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-02 07:36:04.191164 qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-02 07:36:20.719239 qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-02 07:36:20.783239 qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-02 07:36:09.247187 qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.783239 qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-02 07:36:20.787239 qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-02 07:36:09.435188 qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-02 07:36:20.787239 qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-02 07:36:20.791239 qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-02 07:36:10.375192 qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-02 07:36:20.791239 qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-02 07:36:20.787239 qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-02 07:36:10.187191 qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.791239 qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-02 07:36:20.791239 qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-02 07:36:10.559193 qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.795239 qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-02 07:36:20.795239 qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-02 07:36:10.743194 qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-02 07:36:20.795239 qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-05-02 07:36:20.859239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-05-02 07:36:16.047218 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.859239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-02 07:36:20.855239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-02 07:36:15.675216 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.855239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-02 07:36:20.855239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-02 07:36:15.859217 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.855239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-02 07:36:20.847239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-02 07:36:15.299214 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-02 07:36:20.851239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-02 07:36:20.851239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-02 07:36:15.487215 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.851239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-02 07:36:20.863239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-02 07:36:16.599220 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.867240 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-02 07:36:20.863239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-02 07:36:16.415219 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.863239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-02 07:36:20.859239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-02 07:36:16.231219 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.863239 qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-02 07:36:20.907240 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-02 07:36:20.003236 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.907240 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-02 07:36:20.899240 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-02 07:36:19.619234 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.903240 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-05-02 07:36:20.903240 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-05-02 07:36:19.819235 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-02 07:36:20.903240 qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-02 07:36:20.823239 qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-02 07:36:12.647202 qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-02 07:36:20.823239 qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-02 07:36:20.819239 qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-02 07:36:12.455201 qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.823239 qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-02 07:36:20.811239 qwak_core-0.0.39/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-02 07:36:12.079200 qwak_core-0.0.39/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.811239 qwak_core-0.0.39/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-02 07:36:20.815239 qwak_core-0.0.39/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-02 07:36:12.263201 qwak_core-0.0.39/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.815239 qwak_core-0.0.39/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-02 07:36:20.815239 qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-02 07:36:12.835203 qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-02 07:36:20.815239 qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-02 07:36:20.819239 qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-02 07:36:13.239205 qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-02 07:36:20.819239 qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-02 07:36:20.827239 qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-02 07:36:13.623207 qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.831239 qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-02 07:36:20.831239 qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-02 07:36:13.803208 qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-02 07:36:20.831239 qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-02 07:36:20.803239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-02 07:36:11.515197 qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.807239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-02 07:36:20.807239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-02 07:36:11.703198 qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-02 07:36:20.807239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-02 07:36:20.799239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-02 07:36:11.135196 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.799239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-05-02 07:36:20.799239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-05-02 07:36:10.943195 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.799239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-02 07:36:20.803239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-02 07:36:11.331196 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-02 07:36:20.803239 qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-02 07:36:20.703239 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-02 07:36:03.079159 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.707239 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-02 07:36:20.707239 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-02 07:36:03.263160 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.707239 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-02 07:36:20.711239 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-02 07:36:03.447161 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-02 07:36:20.711239 qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-02 07:36:20.763239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-02 07:36:08.131182 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.767239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-02 07:36:20.763239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-02 07:36:07.947181 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-02 07:36:20.763239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-02 07:36:20.743239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-02 07:36:06.447175 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.747239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-02 07:36:20.743239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-02 07:36:06.259174 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.743239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-02 07:36:20.735239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-02 07:36:05.683171 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.735239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-02 07:36:20.739239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-02 07:36:06.075173 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-02 07:36:20.739239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-02 07:36:20.747239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-02 07:36:06.635175 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.747239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-02 07:36:20.747239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-02 07:36:06.823176 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-02 07:36:20.751239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-05-02 07:36:20.739239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-05-02 07:36:05.879172 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.739239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-02 07:36:20.751239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-02 07:36:07.007177 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.751239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-02 07:36:20.767239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-02 07:36:20.191236 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.767239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-02 07:36:20.767239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-02 07:36:20.379237 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-02 07:36:20.771239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-02 07:36:20.771239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-02 07:36:08.687185 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.771239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-02 07:36:20.771239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-02 07:36:08.875185 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-02 07:36:20.775239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-02 07:36:20.775239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-02 07:36:09.059186 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.775239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-02 07:36:20.779239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-02 07:36:09.815190 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.779239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-02 07:36:20.779239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-02 07:36:09.623189 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-02 07:36:20.779239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-02 07:36:20.783239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-02 07:36:09.999190 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.783239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-02 07:36:20.755239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-02 07:36:07.195178 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.755239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-02 07:36:20.755239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-02 07:36:07.383179 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.755239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-02 07:36:20.759239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-02 07:36:07.571179 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-02 07:36:20.759239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-02 07:36:20.759239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-02 07:36:07.759180 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.759239 qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-02 07:36:20.867240 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-02 07:36:16.783221 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.867240 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-02 07:36:20.871240 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-02 07:36:16.971222 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-02 07:36:20.871240 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-02 07:36:20.871240 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-02 07:36:17.155223 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.871240 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-02 07:36:20.875239 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-02 07:36:17.347224 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-02 07:36:20.875239 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-02 07:36:20.875239 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-02 07:36:17.543224 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-02 07:36:20.879239 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-02 07:36:20.879239 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-02 07:36:17.731225 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.879239 qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-02 07:36:20.835239 qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-02 07:36:14.003208 qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.835239 qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-02 07:36:20.835239 qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-02 07:36:14.187209 qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-02 07:36:20.835239 qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-02 07:36:20.723239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-02 07:36:04.935168 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.723239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-02 07:36:20.727239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-02 07:36:05.115169 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.727239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-02 07:36:20.727239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-02 07:36:05.303169 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-02 07:36:20.731239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-02 07:36:20.731239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-02 07:36:05.487170 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.735239 qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-02 07:36:20.807239 qwak_core-0.0.39/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-02 07:36:11.891199 qwak_core-0.0.39/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-02 07:36:20.811239 qwak_core-0.0.39/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-02 07:36:20.879239 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-02 07:36:17.915226 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.883240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-02 07:36:20.883240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-02 07:36:18.103227 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.883240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-02 07:36:20.883240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-02 07:36:18.291228 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.887240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-02 07:36:20.887240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-02 07:36:18.483229 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.887240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-02 07:36:20.891240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-02 07:36:18.675230 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.891240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-02 07:36:20.891240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-02 07:36:18.879231 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-02 07:36:20.891240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-02 07:36:20.895240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-02 07:36:19.063231 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.895240 qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-02 07:36:20.839239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-02 07:36:14.551211 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.843239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-02 07:36:20.847239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-02 07:36:15.111214 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.847239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-02 07:36:20.843239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-02 07:36:14.739212 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-02 07:36:20.843239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-02 07:36:20.843239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-02 07:36:14.927213 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.847239 qwak_core-0.0.39/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-02 07:36:20.827239 qwak_core-0.0.39/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-02 07:36:13.439206 qwak_core-0.0.39/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-02 07:36:20.827239 qwak_core-0.0.39/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-02 07:36:20.699239 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-02 07:36:04.563166 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-02 07:36:20.703239 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-02 07:36:20.699239 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-02 07:36:04.375165 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.699239 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-02 07:36:20.703239 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-02 07:36:04.751167 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-02 07:36:20.703239 qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-02 07:36:20.823239 qwak_core-0.0.39/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-02 07:36:13.035204 qwak_core-0.0.39/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-02 07:36:20.827239 qwak_core-0.0.39/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-02 07:36:20.839239 qwak_core-0.0.39/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-02 07:36:14.367210 qwak_core-0.0.39/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-02 07:36:20.839239 qwak_core-0.0.39/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-02 07:36:20.695239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-02 07:36:02.343156 qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.695239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-02 07:36:20.695239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-02 07:36:02.159155 qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-02 07:36:20.695239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-02 07:36:20.687239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-02 07:36:01.607153 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.687239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-02 07:36:20.691239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-02 07:36:01.791154 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.691239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-02 07:36:20.691239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-02 07:36:01.975154 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-02 07:36:20.691239 qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-02 07:36:20.899240 qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-02 07:36:19.435233 qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-02 07:36:20.899240 qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-02 07:36:20.895240 qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-02 07:36:19.251232 qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.899240 qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-05-02 07:36:20.711239 qwak_core-0.0.39/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-05-02 07:36:03.627162 qwak_core-0.0.39/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.711239 qwak_core-0.0.39/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-02 07:36:20.715239 qwak_core-0.0.39/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-02 07:36:03.807163 qwak_core-0.0.39/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-02 07:36:20.715239 qwak_core-0.0.39/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2485 2023-05-02 07:36:22.095245 qwak_core-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-02 07:36:22.095245 qwak_core-0.0.39/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-02 07:35:13.306937 qwak_core-0.0.39/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-02 07:35:13.306937 qwak_core-0.0.39/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4964 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3374 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1201 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     2006 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2961 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1730 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9443 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-02 07:35:13.310937 qwak_core-0.0.39/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      829 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/schema.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5776 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-02 07:35:13.314937 qwak_core-0.0.39/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 qwak_core-0.0.39/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.39/PKG-INFO
```

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.39/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/v0/user_application.proto\x12\x18qwak.user_application.v0\x1a\x1cgoogle/protobuf/struct.proto\".\n\x04Spec\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x06Status\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct*\xbf\x01\n\x04Type\x12!\n\x1dINVALID_USER_APPLICATION_TYPE\x10\x00\x12\x10\n\x0cREMOTE_BUILD\x10\x01\x12\x1b\n\x17\x42\x41TCH_FEATURE_PROCESSOR\x10\x02\x12\x1f\n\x1bSTREAMING_FEATURE_PROCESSOR\x10\x03\x12\x18\n\x14\x42\x41TCH_INFERENCE_TASK\x10\x04\x12\x14\n\x10MODEL_DEPLOYMENT\x10\x05\x12\x14\n\x10MODEL_MONITORING\x10\x06\x42\xaa\x01\n\x1f\x63om.qwak.ai.user_application.v0P\x01Z\x84\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/v0/user_application.proto\x12\x18qwak.user_application.v0\x1a\x1cgoogle/protobuf/struct.proto\".\n\x04Spec\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"0\n\x06Status\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct*\xbc\x01\n\x04Type\x12!\n\x1dINVALID_USER_APPLICATION_TYPE\x10\x00\x12\x10\n\x0cREMOTE_BUILD\x10\x01\x12\x1b\n\x17\x42\x41TCH_FEATURE_PROCESSOR\x10\x02\x12\x1f\n\x1bSTREAMING_FEATURE_PROCESSOR\x10\x03\x12\x18\n\x14\x42\x41TCH_INFERENCE_TASK\x10\x04\x12\x14\n\x10MODEL_DEPLOYMENT\x10\x05\x12\x11\n\rMODEL_MONITOR\x10\x06\x42\xaa\x01\n\x1f\x63om.qwak.ai.user_application.v0P\x01Z\x84\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0b\x06proto3')
 
 _TYPE = DESCRIPTOR.enum_types_by_name['Type']
 Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
 INVALID_USER_APPLICATION_TYPE = 0
 REMOTE_BUILD = 1
 BATCH_FEATURE_PROCESSOR = 2
 STREAMING_FEATURE_PROCESSOR = 3
 BATCH_INFERENCE_TASK = 4
 MODEL_DEPLOYMENT = 5
-MODEL_MONITORING = 6
+MODEL_MONITOR = 6
 
 
 _SPEC = DESCRIPTOR.message_types_by_name['Spec']
 _STATUS = DESCRIPTOR.message_types_by_name['Status']
 Spec = _reflection.GeneratedProtocolMessageType('Spec', (_message.Message,), {
   'DESCRIPTOR' : _SPEC,
   '__module__' : 'qwak.user_application.v0.user_application_pb2'
@@ -46,13 +46,13 @@
 _sym_db.RegisterMessage(Status)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\037com.qwak.ai.user_application.v0P\001Z\204\001github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application/v0;user_application_v0'
   _TYPE._serialized_start=206
-  _TYPE._serialized_end=397
+  _TYPE._serialized_end=394
   _SPEC._serialized_start=107
   _SPEC._serialized_end=153
   _STATUS._serialized_start=155
   _STATUS._serialized_end=203
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.38/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.39/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     INVALID_USER_APPLICATION_TYPE: _Type.ValueType  # 0
     REMOTE_BUILD: _Type.ValueType  # 1
     BATCH_FEATURE_PROCESSOR: _Type.ValueType  # 2
     STREAMING_FEATURE_PROCESSOR: _Type.ValueType  # 3
     BATCH_INFERENCE_TASK: _Type.ValueType  # 4
     MODEL_DEPLOYMENT: _Type.ValueType  # 5
-    MODEL_MONITORING: _Type.ValueType  # 6
+    MODEL_MONITOR: _Type.ValueType  # 6
 
 class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
 
 INVALID_USER_APPLICATION_TYPE: Type.ValueType  # 0
 REMOTE_BUILD: Type.ValueType  # 1
 BATCH_FEATURE_PROCESSOR: Type.ValueType  # 2
 STREAMING_FEATURE_PROCESSOR: Type.ValueType  # 3
 BATCH_INFERENCE_TASK: Type.ValueType  # 4
 MODEL_DEPLOYMENT: Type.ValueType  # 5
-MODEL_MONITORING: Type.ValueType  # 6
+MODEL_MONITOR: Type.ValueType  # 6
 global___Type = Type
 
 class Spec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `qwak_core-0.0.38/pyproject.toml` & `qwak_core-0.0.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.38"
+version = "0.0.39"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.38/qwak/automations/__init__.py` & `qwak_core-0.0.39/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/automations/automation_executions.py` & `qwak_core-0.0.39/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/automations/automations.py` & `qwak_core-0.0.39/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.39/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.39/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.39/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.39/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.39/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/alert_management/client.py` & `qwak_core-0.0.39/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/analytics/client.py` & `qwak_core-0.0.39/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/audience/client.py` & `qwak_core-0.0.39/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/automation_management/client.py` & `qwak_core-0.0.39/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.39/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.39/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.39/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.39/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/build_management/client.py` & `qwak_core-0.0.39/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.39/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.39/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/deployment/client.py` & `qwak_core-0.0.39/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.39/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.39/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.39/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.39/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.39/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/logging_client/client.py` & `qwak_core-0.0.39/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/model_management/client.py` & `qwak_core-0.0.39/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/project/client.py` & `qwak_core-0.0.39/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/secret_service/client.py` & `qwak_core-0.0.39/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.39/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.39/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.39/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.39/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.39/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.39/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.39/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.39/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.39/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.39/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.39/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.39/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.39/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.39/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.39/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/offline/client.py` & `qwak_core-0.0.39/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/feature_store/online/client.py` & `qwak_core-0.0.39/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/const.py` & `qwak_core-0.0.39/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.39/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.39/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.39/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.39/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/singleton_meta.py` & `qwak_core-0.0.39/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/tool/auth.py` & `qwak_core-0.0.39/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.39/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.39/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.39/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.39/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/adapters/__init__.py` & `qwak_core-0.0.39/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.39/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.39/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.39/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.39/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.39/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/base.py` & `qwak_core-0.0.39/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/decorators/api.py` & `qwak_core-0.0.39/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.39/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/experiment_tracking.py` & `qwak_core-0.0.39/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/schema.py` & `qwak_core-0.0.39/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model/schema_entities.py` & `qwak_core-0.0.39/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.39/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.39/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.39/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.39/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.39/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.39/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/client.py` & `qwak_core-0.0.39/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.39/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/models/model.py` & `qwak_core-0.0.39/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.39/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.39/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.39/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/qwak_services_mock/services_mock.py` & `qwak_core-0.0.39/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.38/setup.py` & `qwak_core-0.0.39/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.38',
+    'version': '0.0.39',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.38/PKG-INFO` & `qwak_core-0.0.39/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.38
+Version: 0.0.39
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

