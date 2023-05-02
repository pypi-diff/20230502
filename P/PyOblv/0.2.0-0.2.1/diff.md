# Comparing `tmp/PyOblv-0.2.0.tar.gz` & `tmp/PyOblv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOblv-0.2.0.tar", last modified: Fri Feb 24 08:09:50 2023, max compression
+gzip compressed data, was "PyOblv-0.2.1.tar", last modified: Tue May  2 04:31:48 2023, max compression
```

## Comparing `PyOblv-0.2.0.tar` & `PyOblv-0.2.1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.497225 PyOblv-0.2.0/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)    11357 2022-12-14 12:27:17.000000 PyOblv-0.2.0/LICENSE
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     7319 2023-02-24 08:09:50.497225 PyOblv-0.2.0/PKG-INFO
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.475559 PyOblv-0.2.0/PyOblv.egg-info/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     7319 2023-02-24 08:09:50.000000 PyOblv-0.2.0/PyOblv.egg-info/PKG-INFO
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5104 2023-02-24 08:09:50.000000 PyOblv-0.2.0/PyOblv.egg-info/SOURCES.txt
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        1 2023-02-24 08:09:50.000000 PyOblv-0.2.0/PyOblv.egg-info/dependency_links.txt
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       42 2023-02-24 08:09:50.000000 PyOblv-0.2.0/PyOblv.egg-info/entry_points.txt
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)      115 2023-02-24 08:09:50.000000 PyOblv-0.2.0/PyOblv.egg-info/requires.txt
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       15 2023-02-24 08:09:50.000000 PyOblv-0.2.0/PyOblv.egg-info/top_level.txt
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     6442 2023-02-24 06:00:37.000000 PyOblv-0.2.0/README.md
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.475559 PyOblv-0.2.0/cli/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/cli/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4079 2022-11-18 10:31:51.000000 PyOblv-0.2.0/cli/deployment.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2668 2022-12-14 10:38:38.000000 PyOblv-0.2.0/cli/main.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3356 2022-11-18 10:31:51.000000 PyOblv-0.2.0/cli/service.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)      633 2022-11-18 10:31:51.000000 PyOblv-0.2.0/cli/utils.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.475559 PyOblv-0.2.0/oblv/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       90 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/__init__.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.475559 PyOblv-0.2.0/oblv/api/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       47 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/__init__.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.475559 PyOblv-0.2.0/oblv/api/account/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/account/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4966 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/account/get_user_accounts_account_get.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/oblv/api/auth/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/auth/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4855 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/auth/authenticate_key_login_apikey_post.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4833 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/auth/logout_session_logout_delete.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/oblv/api/deployment/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/deployment/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5543 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/deployment/create_new_deployment_deployment_post.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5048 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/deployment/delete_deployment_deployment_delete.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     8045 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/deployment/generate_build_args_deployment_arguments_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     6657 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/deployment/get_available_deployments_deployment_available_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5115 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/deployment/get_deployment_info_deployment_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5427 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/deployment/get_deployment_roles_deployment_roles_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3093 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/deployment/get_supported_regions_deployment_supported_regions_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     6507 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/deployment/get_user_owned_deployments_deployment_owned_get.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/oblv/api/notification/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/notification/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4973 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/notification/get_all_notifications_notification_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4936 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/notification/get_notification_details_notification_notification_id_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4326 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/notification/mark_all_notification_read_notification_delete.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4783 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/notification/mark_notification_read_notification_notification_id_delete.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/oblv/api/repo/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/repo/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5022 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/repo/get_all_repos_repo_linked_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5997 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/repo/get_repo_from_vcs_repo_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     7515 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/repo/get_repo_refs_repo_refs_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5866 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/repo/get_repo_repo_repo_id_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     6037 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/repo/get_repo_repo_repo_owner_repo_name_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5712 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/repo/search_repo_from_vcs_repo_search_get.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/oblv/api/service/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/service/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     7773 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/service/add_repo_service_repo_service_post.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     7024 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/service/delete_repo_services_repo_service_delete.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     7266 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     8101 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/service/get_repo_services_repo_service_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     6934 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/service/get_user_services_service_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     8272 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/service/update_repo_service_repo_service_put.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     8106 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/service/validate_repo_service_repo_service_validate_get.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/oblv/api/user/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/api/user/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4807 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/user/add_user_public_shared_key_user_psk_put.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4741 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4702 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/user/get_user_profile_view_user_profile_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4707 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/user/get_user_public_shared_key_user_psk_get.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4829 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/user/update_user_name_user_name_put.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4966 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/api/user/update_user_password_user_password_put.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)      376 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/auth.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1828 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/client.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       30 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/config.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3935 2022-12-14 08:58:11.000000 PyOblv-0.2.0/oblv/exceptions.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/oblv/models/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1539 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2523 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/access_history.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2246 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/account.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1469 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/api_key.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1905 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/available_deployment.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2313 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/available_deployment_list.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1903 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/build_args_schema.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3913 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/create_deployment_input.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2036 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/create_deployment_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     9889 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/deployment_complete.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2260 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/deployment_list.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     8547 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/deployment_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2175 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/http_validation_error.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3315 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/instance.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1640 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/message_model.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1592 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/name_input.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2962 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/notification_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1908 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/oblv_auth_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1521 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/psk.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2095 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/ref_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     4845 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/repo.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2258 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/repo_all_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2236 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/repo_service_list.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     5407 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/repo_services.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2028 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/role_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1356 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/service_content_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2352 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/service_validation_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1344 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/service_yaml_add_input.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1359 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/service_yaml_update_input.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2591 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/shared_users.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1323 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/supported_regions.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3089 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/user_credit_utilization.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1799 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/user_password_input.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2600 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/user_profile_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2208 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/user_service_list.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3332 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/models/user_services.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2456 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/validated_service.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1824 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/validation_error.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2638 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/models/vcs_repo_response.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)    21146 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/oblv_client.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       25 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/py.typed
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)      939 2022-11-18 10:31:51.000000 PyOblv-0.2.0/oblv/types.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1233 2023-02-24 06:00:37.000000 PyOblv-0.2.0/oblv/utils.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       38 2023-02-24 08:09:50.497225 PyOblv-0.2.0/setup.cfg
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1620 2023-02-24 06:00:37.000000 PyOblv-0.2.0/setup.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.486392 PyOblv-0.2.0/tests/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)       81 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/test_oblv.py
-drwxr-xr-x   0 bhaswar   (1000) bhaswar   (1000)        0 2023-02-24 08:09:50.497225 PyOblv-0.2.0/tests/unit/
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)        0 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/__init__.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     6994 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/constants.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3931 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_add_service.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3586 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_auth.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3153 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_available_deployments.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3498 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_create_deployment.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3092 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_deployment_info.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3169 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_deployment_roles.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3312 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_generate_deployment_build_args.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3172 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_link_repo.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2824 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_logout.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3144 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_remove_deployment.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3822 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_remove_service.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2975 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_repo_refs.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3124 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_repo_services.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2943 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_repo_vcs.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3004 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_repo_with_services.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3309 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_revalidate_service.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3040 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_search_repo.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3191 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_service_yaml_content.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     1805 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_supported_aws_regions.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3040 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_unlink_repo.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3705 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_update_service.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3110 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_update_user_password.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3098 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_accounts.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3236 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_credit_usage.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3035 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_deployments.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2961 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_linked_repos.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3018 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_name_update.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3234 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_profile.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2980 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_psk.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     3012 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_services.py
--rw-r--r--   0 bhaswar   (1000) bhaswar   (1000)     2956 2022-11-18 10:31:51.000000 PyOblv-0.2.0/tests/unit/test_user_set_psk.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:48.034003 PyOblv-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-01-05 11:33:47.000000 PyOblv-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     7474 2023-05-02 04:31:48.034003 PyOblv-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.512062 PyOblv-0.2.1/PyOblv.egg-info/
+-rw-rw-rw-   0        0        0     7474 2023-05-02 04:31:47.000000 PyOblv-0.2.1/PyOblv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2023-05-02 04:31:47.000000 PyOblv-0.2.1/PyOblv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 04:31:47.000000 PyOblv-0.2.1/PyOblv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-02 04:31:47.000000 PyOblv-0.2.1/PyOblv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2023-05-02 04:31:47.000000 PyOblv-0.2.1/PyOblv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 04:31:47.000000 PyOblv-0.2.1/PyOblv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6803 2023-05-02 04:26:52.000000 PyOblv-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.533061 PyOblv-0.2.1/cli/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/cli/__init__.py
+-rw-rw-rw-   0        0        0     4169 2023-05-02 04:26:52.000000 PyOblv-0.2.1/cli/deployment.py
+-rw-rw-rw-   0        0        0     2751 2023-05-02 04:26:52.000000 PyOblv-0.2.1/cli/main.py
+-rw-rw-rw-   0        0        0     3427 2023-05-02 04:26:52.000000 PyOblv-0.2.1/cli/service.py
+-rw-rw-rw-   0        0        0      658 2023-05-02 04:26:52.000000 PyOblv-0.2.1/cli/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.573941 PyOblv-0.2.1/oblv/
+-rw-rw-rw-   0        0        0       94 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.578938 PyOblv-0.2.1/oblv/api/
+-rw-rw-rw-   0        0        0       48 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.584939 PyOblv-0.2.1/oblv/api/account/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/account/__init__.py
+-rw-rw-rw-   0        0        0     5146 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/account/get_user_accounts_account_get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.596946 PyOblv-0.2.1/oblv/api/auth/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/auth/__init__.py
+-rw-rw-rw-   0        0        0     5029 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/auth/authenticate_key_login_apikey_post.py
+-rw-rw-rw-   0        0        0     5004 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/auth/logout_session_logout_delete.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.642454 PyOblv-0.2.1/oblv/api/deployment/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/__init__.py
+-rw-rw-rw-   0        0        0     5735 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/create_new_deployment_deployment_post.py
+-rw-rw-rw-   0        0        0     5233 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/delete_deployment_deployment_delete.py
+-rw-rw-rw-   0        0        0     8308 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/generate_build_args_deployment_arguments_get.py
+-rw-rw-rw-   0        0        0     6874 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/get_available_deployments_deployment_available_get.py
+-rw-rw-rw-   0        0        0     5302 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/get_deployment_info_deployment_get.py
+-rw-rw-rw-   0        0        0     5623 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/get_deployment_roles_deployment_roles_get.py
+-rw-rw-rw-   0        0        0     3227 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/get_supported_regions_deployment_supported_regions_get.py
+-rw-rw-rw-   0        0        0     6724 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/deployment/get_user_owned_deployments_deployment_owned_get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.666459 PyOblv-0.2.1/oblv/api/notification/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/notification/__init__.py
+-rw-rw-rw-   0        0        0     5145 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/notification/get_all_notifications_notification_get.py
+-rw-rw-rw-   0        0        0     5110 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/notification/get_notification_details_notification_notification_id_get.py
+-rw-rw-rw-   0        0        0     4484 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/notification/mark_all_notification_read_notification_delete.py
+-rw-rw-rw-   0        0        0     4954 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/notification/mark_notification_read_notification_notification_id_delete.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.702961 PyOblv-0.2.1/oblv/api/repo/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/repo/__init__.py
+-rw-rw-rw-   0        0        0     5202 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/repo/get_all_repos_repo_linked_get.py
+-rw-rw-rw-   0        0        0     6198 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/repo/get_repo_from_vcs_repo_get.py
+-rw-rw-rw-   0        0        0     7756 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/repo/get_repo_refs_repo_refs_get.py
+-rw-rw-rw-   0        0        0     6065 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/repo/get_repo_repo_repo_id_get.py
+-rw-rw-rw-   0        0        0     6245 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/repo/get_repo_repo_repo_owner_repo_name_get.py
+-rw-rw-rw-   0        0        0     5907 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/repo/search_repo_from_vcs_repo_search_get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.746229 PyOblv-0.2.1/oblv/api/service/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/__init__.py
+-rw-rw-rw-   0        0        0     8037 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/add_repo_service_repo_service_post.py
+-rw-rw-rw-   0        0        0     7266 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/delete_repo_services_repo_service_delete.py
+-rw-rw-rw-   0        0        0     7513 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/get_repo_service_yaml_form_content_repo_service_yaml_get.py
+-rw-rw-rw-   0        0        0     8367 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/get_repo_services_repo_service_get.py
+-rw-rw-rw-   0        0        0     7166 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/get_user_services_service_get.py
+-rw-rw-rw-   0        0        0     8539 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/update_repo_service_repo_service_put.py
+-rw-rw-rw-   0        0        0     8369 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/service/validate_repo_service_repo_service_validate_get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.782233 PyOblv-0.2.1/oblv/api/user/
+-rw-rw-rw-   0        0        0        0 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/user/__init__.py
+-rw-rw-rw-   0        0        0     4991 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/user/add_user_public_shared_key_user_psk_put.py
+-rw-rw-rw-   0        0        0     4913 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py
+-rw-rw-rw-   0        0        0     4874 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/user/get_user_profile_view_user_profile_get.py
+-rw-rw-rw-   0        0        0     4888 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/user/get_user_public_shared_key_user_psk_get.py
+-rw-rw-rw-   0        0        0     5013 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/user/update_user_name_user_name_put.py
+-rw-rw-rw-   0        0        0     5150 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/api/user/update_user_password_user_password_put.py
+-rw-rw-rw-   0        0        0      564 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/auth.py
+-rw-rw-rw-   0        0        0     1885 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/client.py
+-rw-rw-rw-   0        0        0       30 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/config.py
+-rw-rw-rw-   0        0        0     4062 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.996353 PyOblv-0.2.1/oblv/models/
+-rw-rw-rw-   0        0        0     1573 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/__init__.py
+-rw-rw-rw-   0        0        0     2611 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/access_history.py
+-rw-rw-rw-   0        0        0     2326 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/account.py
+-rw-rw-rw-   0        0        0     1533 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/api_key.py
+-rw-rw-rw-   0        0        0     1979 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/available_deployment.py
+-rw-rw-rw-   0        0        0     2395 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/available_deployment_list.py
+-rw-rw-rw-   0        0        0     1975 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/build_args_schema.py
+-rw-rw-rw-   0        0        0     4051 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/create_deployment_input.py
+-rw-rw-rw-   0        0        0     2108 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/create_deployment_response.py
+-rw-rw-rw-   0        0        0    10161 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/deployment_complete.py
+-rw-rw-rw-   0        0        0     2342 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/deployment_list.py
+-rw-rw-rw-   0        0        0     8783 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/deployment_response.py
+-rw-rw-rw-   0        0        0     2251 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/http_validation_error.py
+-rw-rw-rw-   0        0        0     3419 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/instance.py
+-rw-rw-rw-   0        0        0     1704 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/message_model.py
+-rw-rw-rw-   0        0        0     1656 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/name_input.py
+-rw-rw-rw-   0        0        0     3066 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/notification_response.py
+-rw-rw-rw-   0        0        0     1980 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/oblv_auth_response.py
+-rw-rw-rw-   0        0        0     1585 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/psk.py
+-rw-rw-rw-   0        0        0     2172 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/ref_response.py
+-rw-rw-rw-   0        0        0     4997 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/repo.py
+-rw-rw-rw-   0        0        0     2338 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/repo_all_response.py
+-rw-rw-rw-   0        0        0     2319 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/repo_service_list.py
+-rw-rw-rw-   0        0        0     5571 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/repo_services.py
+-rw-rw-rw-   0        0        0     2100 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/role_response.py
+-rw-rw-rw-   0        0        0     1407 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/service_content_response.py
+-rw-rw-rw-   0        0        0     2432 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/service_validation_response.py
+-rw-rw-rw-   0        0        0     1395 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/service_yaml_add_input.py
+-rw-rw-rw-   0        0        0     1410 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/service_yaml_update_input.py
+-rw-rw-rw-   0        0        0     2682 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/shared_users.py
+-rw-rw-rw-   0        0        0     1374 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/supported_regions.py
+-rw-rw-rw-   0        0        0     3177 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/user_credit_utilization.py
+-rw-rw-rw-   0        0        0     1870 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/user_password_input.py
+-rw-rw-rw-   0        0        0     2688 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/user_profile_response.py
+-rw-rw-rw-   0        0        0     2291 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/user_service_list.py
+-rw-rw-rw-   0        0        0     3444 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/user_services.py
+-rw-rw-rw-   0        0        0     2544 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/validated_service.py
+-rw-rw-rw-   0        0        0     1903 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/validation_error.py
+-rw-rw-rw-   0        0        0     2731 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/models/vcs_repo_response.py
+-rw-rw-rw-   0        0        0    21942 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/oblv_client.py
+-rw-rw-rw-   0        0        0       25 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/py.typed
+-rw-rw-rw-   0        0        0      982 2023-05-02 04:26:52.000000 PyOblv-0.2.1/oblv/types.py
+-rw-rw-rw-   0        0        0     1283 2023-05-02 04:26:53.000000 PyOblv-0.2.1/oblv/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 04:31:48.034003 PyOblv-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2023-05-02 04:26:53.000000 PyOblv-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:47.997366 PyOblv-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-08 17:43:31.000000 PyOblv-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0       84 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/test_oblv.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:31:48.033003 PyOblv-0.2.1/tests/unit/
+-rw-rw-rw-   0        0        0        0 2022-11-22 05:48:14.000000 PyOblv-0.2.1/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     7211 2023-05-01 13:28:03.000000 PyOblv-0.2.1/tests/unit/constants.py
+-rw-rw-rw-   0        0        0     4032 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_add_service.py
+-rw-rw-rw-   0        0        0     3683 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_auth.py
+-rw-rw-rw-   0        0        0     3247 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_available_deployments.py
+-rw-rw-rw-   0        0        0     3598 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_create_deployment.py
+-rw-rw-rw-   0        0        0     3185 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_deployment_info.py
+-rw-rw-rw-   0        0        0     3264 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_deployment_roles.py
+-rw-rw-rw-   0        0        0     3406 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_generate_deployment_build_args.py
+-rw-rw-rw-   0        0        0     3265 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_link_repo.py
+-rw-rw-rw-   0        0        0     2910 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_logout.py
+-rw-rw-rw-   0        0        0     3237 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_remove_deployment.py
+-rw-rw-rw-   0        0        0     3920 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_remove_service.py
+-rw-rw-rw-   0        0        0     3067 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_repo_refs.py
+-rw-rw-rw-   0        0        0     3219 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_repo_services.py
+-rw-rw-rw-   0        0        0     3034 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_repo_vcs.py
+-rw-rw-rw-   0        0        0     3096 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_repo_with_services.py
+-rw-rw-rw-   0        0        0     3405 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_revalidate_service.py
+-rw-rw-rw-   0        0        0     3132 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_search_repo.py
+-rw-rw-rw-   0        0        0     3285 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_service_yaml_content.py
+-rw-rw-rw-   0        0        0     1854 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_supported_aws_regions.py
+-rw-rw-rw-   0        0        0     3132 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_unlink_repo.py
+-rw-rw-rw-   0        0        0     3801 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_update_service.py
+-rw-rw-rw-   0        0        0     3205 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_update_user_password.py
+-rw-rw-rw-   0        0        0     3195 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_accounts.py
+-rw-rw-rw-   0        0        0     3333 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_credit_usage.py
+-rw-rw-rw-   0        0        0     3128 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_deployments.py
+-rw-rw-rw-   0        0        0     3052 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_linked_repos.py
+-rw-rw-rw-   0        0        0     3111 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_name_update.py
+-rw-rw-rw-   0        0        0     3335 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_profile.py
+-rw-rw-rw-   0        0        0     3071 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_psk.py
+-rw-rw-rw-   0        0        0     3105 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_services.py
+-rw-rw-rw-   0        0        0     3044 2023-05-02 04:26:53.000000 PyOblv-0.2.1/tests/unit/test_user_set_psk.py
```

### Comparing `PyOblv-0.2.0/LICENSE` & `PyOblv-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `PyOblv-0.2.0/PKG-INFO` & `PyOblv-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,235 +1,237 @@
-Metadata-Version: 2.1
-Name: PyOblv
-Version: 0.2.0
-Summary: A client library for accessing Oblivious OpenAPIs
-Home-page: https://github.com/ObliviousAI/PyOblv
-Author: Oblivious
-Author-email: hello@oblivious.ai
-License: Apache License 2.0
-Project-URL: Documentation, https://github.com/ObliviousAI/PyOblv/tree/master/README.md
-Project-URL: Source, https://github.com/ObliviousAI/PyOblv
-Project-URL: Tracker, https://github.com/ObliviousAI/PyOblv/issues
-Keywords: Oblivious python package
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyOblv
-
-A Python library to access Oblivious OpenAPIs.
-
-## Usage
-
-First, create a client, with your API key. This key can be created in the
-[Oblivious Console UI](https://console.oblivious.ai/). Go to the
-settings page, and create your ApiKey. Once done, the client can be
-created as follows
-
-``` {.python}
-from oblv import authenticate
-client = authenticate(apikey=*your_key_here*)
-```
-
-
-Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
-
-
-
-### 1 Create a service
-
-A service refers to a branch/tag of your repository that needs to be
-deployed. For your first service. you can use the repository
-[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
-Execute the below command to create the service.
-
-``` {.python}
-client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
-    "auth": [
-        {
-            "auth_name": "auth_name",
-            "auth_type": "signed_headers"
-        }
-    ],
-    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
-    "build_args": [],
-    "meta": {
-        "author": "Team Oblivious",
-        "author_email": "hello@oblivious.ai",
-        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
-        "version": "0.1.0"
-    },
-    "paths": [
-        {
-            "access": "user",
-            "path": "/hello/",
-            "short_description": "Hello world example"
-        }
-    ],
-    "roles": [
-        {
-            "role_auth": "auth_name",
-            "role_cardinality": 1,
-            "role_description": "Role for the data scientist",
-            "role_name": "user"
-        }
-    ],
-    "traffic": {
-        "inbound": [
-            {
-                "name": "main_io",
-                "port": 80,
-                "type": "tcp"
-            }
-        ],
-        "outbound": [
-            {
-                "domain": "example.com",
-                "name": "example",
-                "port": 443,
-                "type": "tcp"
-            }
-        ]
-    }
-})
-```
-
-The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
-The response for the call above gives results as follows - 
-
-
->{ \
->&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
->&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
->&nbsp;&nbsp;&nbsp;&nbsp;} \
->} 
-
-
-You have now successfully created your first service, and it can be now deployed to an enclave.
-
-### 2 Enclave Creation
-
-To create an enclave, you need to decide on a few of the parameters -
-
--   **deployment_name** - A unique deployment name. You cannot have two
-    running deployments with the same name.
--   **region_name** - could be one of the AWS regions from
-    - ***us-east-1*** (N. Virginia) 
-    - ***us-west-2*** (Oregon)
-    - ***eu-central-1*** (Frankfurt)
-    - ***eu-west-2*** (London)
--   **visibility** - ***private*** or ***public***
--   **is_dev_env** - ***True*** or ***False***.
--   **tags** - A list of tags for your deployment
--   **account_type** - This is the VCS type, and only GitHub*** is
-    supported for now.
--   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
-    any additional arguments for your build. It also includes the infra
-    size needed for the deployment. The options are -
-    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
-    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
-        76.8/hr
-    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
-        100.8/hr
-    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
-        136.0/hr
-    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
-        153.6/hr
-
-A valid example for *build_args* for the service you created -
-
-
-```
-args = {
-    "users": {
-      "admin": [
-        {
-          "user_name": "<your name>",
-          "public key": "<your public key>"
-        }
-      ]
-    },
-    "infra_reqs": "m5.xlarge",  
-}
-
-```
-
-> 📝 **Note:**
->
-> <b>admin</b> here
-> is the role defined for the deployment in service.yaml
-> file
->
-> The service used,
-> does not have requirements for any runtime or build arguments, so not
-> needed here.
-
-``` {.python}
-from oblv.models import CreateDeploymentInput
-input = CreateDeploymentInput(
-    owner="ObliviousAI",
-    repo="FastAPI-Enclave-Services",
-    account_type="github",
-    ref="master",
-    ref_type="branch",
-    region_name="us-east-1",
-    deployment_name="Depl",
-    visibility="private",
-    is_dev_env=True,
-    tags=[],
-    build_args=args
-)
-response = client.create_deployment(input)
-```
-
-
-On successful request, enclave creation is initiated, and it returns an
-id for the deployment, which can be later used to track the status and
-connection details for the enclave.
-
-To check the state of the deployment, run
-
-``` {.python}
-client.deployment_info(response.deployment_id).current_state
-```
-
-> 'CFT Initiated'
-
-
-When the deployment state becomes ***Running***, it indicates that the
-enclave is now available for connection.
-
-To connect to the enclave, you need **Oblv CLI** installed in your
-system. The commands to use the CLI can be found in this
-[documentation](https://docs.oblivious.ai/cli/usage_examples).
-
-Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
-
-The URL to connect to the enclave using CLI can be accessed using
-
-``` {.python}
-client.deployment_info(response.deployment_id).instance.service_url
-```
-
->
->'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
->
-
-
-The PCR codes can be found using
-
-``` {.python}
-client.deployment_info(response.deployment_id).pcr_codes
-```
-
->['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
-'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+Metadata-Version: 2.1
+Name: PyOblv
+Version: 0.2.1
+Summary: A client library for accessing Oblivious APIs
+Home-page: UNKNOWN
+Author: Oblivious
+Author-email: hello@oblivious.ai
+License: Apache License 2.0
+Keywords: Oblivious python package
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+***PyOblv is deprecated, and will not be supported in future. Kindly use [oblv-ctl](https://pypi.org/project/oblv-ctl/) to access Oblivious APIs.***
+
+# PyOblv
+
+A Python library to access Oblivious APIs.
+
+## Usage
+
+First, create a client, with your API key. This key can be created in the
+[Oblivious Console UI](https://console.oblivious.ai/). Go to the
+settings page, and create your ApiKey. Once done, the client can be
+created as follows
+
+``` {.python}
+from oblv import authenticate
+client = authenticate(apikey=*your_key_here*)
+```
+
+
+Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
+
+
+
+### 1 Create a service
+
+A service refers to a branch/tag of your repository that needs to be
+deployed. For your first service. you can use the repository
+[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
+Execute the below command to create the service.
+
+``` {.python}
+client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
+    "auth": [
+        {
+            "auth_name": "auth_name",
+            "auth_type": "signed_headers"
+        }
+    ],
+    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
+    "build_args": [],
+    "meta": {
+        "author": "Team Oblivious",
+        "author_email": "hello@oblivious.ai",
+        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
+        "version": "0.1.0"
+    },
+    "paths": [
+        {
+            "access": "user",
+            "path": "/hello/",
+            "short_description": "Hello world example"
+        }
+    ],
+    "roles": [
+        {
+            "role_auth": "auth_name",
+            "role_cardinality": 1,
+            "role_description": "Role for the data scientist",
+            "role_name": "user"
+        }
+    ],
+    "traffic": {
+        "inbound": [
+            {
+                "name": "main_io",
+                "port": 80,
+                "type": "tcp"
+            }
+        ],
+        "outbound": [
+            {
+                "domain": "example.com",
+                "name": "example",
+                "port": 443,
+                "type": "tcp"
+            }
+        ]
+    }
+})
+```
+
+The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
+The response for the call above gives results as follows - 
+
+
+>{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
+>&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
+>&nbsp;&nbsp;&nbsp;&nbsp;} \
+>} 
+
+
+You have now successfully created your first service, and it can be now deployed to an enclave.
+
+### 2 Enclave Creation
+
+To create an enclave, you need to decide on a few of the parameters -
+
+-   **deployment_name** - A unique deployment name. You cannot have two
+    running deployments with the same name.
+-   **region_name** - could be one of the AWS regions from
+    - ***us-east-1*** (N. Virginia) 
+    - ***us-west-2*** (Oregon)
+    - ***eu-central-1*** (Frankfurt)
+    - ***eu-west-2*** (London)
+-   **visibility** - ***private*** or ***public***
+-   **is_dev_env** - ***True*** or ***False***.
+-   **tags** - A list of tags for your deployment
+-   **account_type** - This is the VCS type, and only GitHub*** is
+    supported for now.
+-   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
+    any additional arguments for your build. It also includes the infra
+    size needed for the deployment. The options are -
+    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
+    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
+        76.8/hr
+    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
+        100.8/hr
+    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
+        136.0/hr
+    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
+        153.6/hr
+
+A valid example for *build_args* for the service you created -
+
+
+```
+args = {
+    "users": {
+      "admin": [
+        {
+          "user_name": "<your name>",
+          "public key": "<your public key>"
+        }
+      ]
+    },
+    "infra_reqs": "m5.xlarge",  
+}
+
+```
+
+> 📝 **Note:**
+>
+> <b>admin</b> here
+> is the role defined for the deployment in service.yaml
+> file
+>
+> The service used,
+> does not have requirements for any runtime or build arguments, so not
+> needed here.
+
+``` {.python}
+from oblv.models import CreateDeploymentInput
+input = CreateDeploymentInput(
+    owner="ObliviousAI",
+    repo="FastAPI-Enclave-Services",
+    account_type="github",
+    ref="master",
+    ref_type="branch",
+    region_name="us-east-1",
+    deployment_name="Depl",
+    visibility="private",
+    is_dev_env=True,
+    tags=[],
+    build_args=args
+)
+response = client.create_deployment(input)
+```
+
+
+On successful request, enclave creation is initiated, and it returns an
+id for the deployment, which can be later used to track the status and
+connection details for the enclave.
+
+To check the state of the deployment, run
+
+``` {.python}
+client.deployment_info(response.deployment_id).current_state
+```
+
+> 'CFT Initiated'
+
+
+When the deployment state becomes ***Running***, it indicates that the
+enclave is now available for connection.
+
+To connect to the enclave, you need **Oblv CLI** installed in your
+system. The commands to use the CLI can be found in this
+[documentation](https://docs.oblivious.ai/cli/usage_examples).
+
+Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
+
+The URL to connect to the enclave using CLI can be accessed using
+
+``` {.python}
+client.deployment_info(response.deployment_id).instance.service_url
+```
+
+>
+>'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
+>
+
+
+The PCR codes can be found using
+
+``` {.python}
+client.deployment_info(response.deployment_id).pcr_codes
+```
+
+>['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
+'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+
+
```

### Comparing `PyOblv-0.2.0/PyOblv.egg-info/PKG-INFO` & `PyOblv-0.2.1/PyOblv.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,235 +1,237 @@
-Metadata-Version: 2.1
-Name: PyOblv
-Version: 0.2.0
-Summary: A client library for accessing Oblivious OpenAPIs
-Home-page: https://github.com/ObliviousAI/PyOblv
-Author: Oblivious
-Author-email: hello@oblivious.ai
-License: Apache License 2.0
-Project-URL: Documentation, https://github.com/ObliviousAI/PyOblv/tree/master/README.md
-Project-URL: Source, https://github.com/ObliviousAI/PyOblv
-Project-URL: Tracker, https://github.com/ObliviousAI/PyOblv/issues
-Keywords: Oblivious python package
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyOblv
-
-A Python library to access Oblivious OpenAPIs.
-
-## Usage
-
-First, create a client, with your API key. This key can be created in the
-[Oblivious Console UI](https://console.oblivious.ai/). Go to the
-settings page, and create your ApiKey. Once done, the client can be
-created as follows
-
-``` {.python}
-from oblv import authenticate
-client = authenticate(apikey=*your_key_here*)
-```
-
-
-Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
-
-
-
-### 1 Create a service
-
-A service refers to a branch/tag of your repository that needs to be
-deployed. For your first service. you can use the repository
-[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
-Execute the below command to create the service.
-
-``` {.python}
-client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
-    "auth": [
-        {
-            "auth_name": "auth_name",
-            "auth_type": "signed_headers"
-        }
-    ],
-    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
-    "build_args": [],
-    "meta": {
-        "author": "Team Oblivious",
-        "author_email": "hello@oblivious.ai",
-        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
-        "version": "0.1.0"
-    },
-    "paths": [
-        {
-            "access": "user",
-            "path": "/hello/",
-            "short_description": "Hello world example"
-        }
-    ],
-    "roles": [
-        {
-            "role_auth": "auth_name",
-            "role_cardinality": 1,
-            "role_description": "Role for the data scientist",
-            "role_name": "user"
-        }
-    ],
-    "traffic": {
-        "inbound": [
-            {
-                "name": "main_io",
-                "port": 80,
-                "type": "tcp"
-            }
-        ],
-        "outbound": [
-            {
-                "domain": "example.com",
-                "name": "example",
-                "port": 443,
-                "type": "tcp"
-            }
-        ]
-    }
-})
-```
-
-The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
-The response for the call above gives results as follows - 
-
-
->{ \
->&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
->&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
->&nbsp;&nbsp;&nbsp;&nbsp;} \
->} 
-
-
-You have now successfully created your first service, and it can be now deployed to an enclave.
-
-### 2 Enclave Creation
-
-To create an enclave, you need to decide on a few of the parameters -
-
--   **deployment_name** - A unique deployment name. You cannot have two
-    running deployments with the same name.
--   **region_name** - could be one of the AWS regions from
-    - ***us-east-1*** (N. Virginia) 
-    - ***us-west-2*** (Oregon)
-    - ***eu-central-1*** (Frankfurt)
-    - ***eu-west-2*** (London)
--   **visibility** - ***private*** or ***public***
--   **is_dev_env** - ***True*** or ***False***.
--   **tags** - A list of tags for your deployment
--   **account_type** - This is the VCS type, and only GitHub*** is
-    supported for now.
--   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
-    any additional arguments for your build. It also includes the infra
-    size needed for the deployment. The options are -
-    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
-    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
-        76.8/hr
-    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
-        100.8/hr
-    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
-        136.0/hr
-    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
-        153.6/hr
-
-A valid example for *build_args* for the service you created -
-
-
-```
-args = {
-    "users": {
-      "admin": [
-        {
-          "user_name": "<your name>",
-          "public key": "<your public key>"
-        }
-      ]
-    },
-    "infra_reqs": "m5.xlarge",  
-}
-
-```
-
-> 📝 **Note:**
->
-> <b>admin</b> here
-> is the role defined for the deployment in service.yaml
-> file
->
-> The service used,
-> does not have requirements for any runtime or build arguments, so not
-> needed here.
-
-``` {.python}
-from oblv.models import CreateDeploymentInput
-input = CreateDeploymentInput(
-    owner="ObliviousAI",
-    repo="FastAPI-Enclave-Services",
-    account_type="github",
-    ref="master",
-    ref_type="branch",
-    region_name="us-east-1",
-    deployment_name="Depl",
-    visibility="private",
-    is_dev_env=True,
-    tags=[],
-    build_args=args
-)
-response = client.create_deployment(input)
-```
-
-
-On successful request, enclave creation is initiated, and it returns an
-id for the deployment, which can be later used to track the status and
-connection details for the enclave.
-
-To check the state of the deployment, run
-
-``` {.python}
-client.deployment_info(response.deployment_id).current_state
-```
-
-> 'CFT Initiated'
-
-
-When the deployment state becomes ***Running***, it indicates that the
-enclave is now available for connection.
-
-To connect to the enclave, you need **Oblv CLI** installed in your
-system. The commands to use the CLI can be found in this
-[documentation](https://docs.oblivious.ai/cli/usage_examples).
-
-Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
-
-The URL to connect to the enclave using CLI can be accessed using
-
-``` {.python}
-client.deployment_info(response.deployment_id).instance.service_url
-```
-
->
->'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
->
-
-
-The PCR codes can be found using
-
-``` {.python}
-client.deployment_info(response.deployment_id).pcr_codes
-```
-
->['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
-'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+Metadata-Version: 2.1
+Name: PyOblv
+Version: 0.2.1
+Summary: A client library for accessing Oblivious APIs
+Home-page: UNKNOWN
+Author: Oblivious
+Author-email: hello@oblivious.ai
+License: Apache License 2.0
+Keywords: Oblivious python package
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+***PyOblv is deprecated, and will not be supported in future. Kindly use [oblv-ctl](https://pypi.org/project/oblv-ctl/) to access Oblivious APIs.***
+
+# PyOblv
+
+A Python library to access Oblivious APIs.
+
+## Usage
+
+First, create a client, with your API key. This key can be created in the
+[Oblivious Console UI](https://console.oblivious.ai/). Go to the
+settings page, and create your ApiKey. Once done, the client can be
+created as follows
+
+``` {.python}
+from oblv import authenticate
+client = authenticate(apikey=*your_key_here*)
+```
+
+
+Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
+
+
+
+### 1 Create a service
+
+A service refers to a branch/tag of your repository that needs to be
+deployed. For your first service. you can use the repository
+[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
+Execute the below command to create the service.
+
+``` {.python}
+client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
+    "auth": [
+        {
+            "auth_name": "auth_name",
+            "auth_type": "signed_headers"
+        }
+    ],
+    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
+    "build_args": [],
+    "meta": {
+        "author": "Team Oblivious",
+        "author_email": "hello@oblivious.ai",
+        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
+        "version": "0.1.0"
+    },
+    "paths": [
+        {
+            "access": "user",
+            "path": "/hello/",
+            "short_description": "Hello world example"
+        }
+    ],
+    "roles": [
+        {
+            "role_auth": "auth_name",
+            "role_cardinality": 1,
+            "role_description": "Role for the data scientist",
+            "role_name": "user"
+        }
+    ],
+    "traffic": {
+        "inbound": [
+            {
+                "name": "main_io",
+                "port": 80,
+                "type": "tcp"
+            }
+        ],
+        "outbound": [
+            {
+                "domain": "example.com",
+                "name": "example",
+                "port": 443,
+                "type": "tcp"
+            }
+        ]
+    }
+})
+```
+
+The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
+The response for the call above gives results as follows - 
+
+
+>{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
+>&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
+>&nbsp;&nbsp;&nbsp;&nbsp;} \
+>} 
+
+
+You have now successfully created your first service, and it can be now deployed to an enclave.
+
+### 2 Enclave Creation
+
+To create an enclave, you need to decide on a few of the parameters -
+
+-   **deployment_name** - A unique deployment name. You cannot have two
+    running deployments with the same name.
+-   **region_name** - could be one of the AWS regions from
+    - ***us-east-1*** (N. Virginia) 
+    - ***us-west-2*** (Oregon)
+    - ***eu-central-1*** (Frankfurt)
+    - ***eu-west-2*** (London)
+-   **visibility** - ***private*** or ***public***
+-   **is_dev_env** - ***True*** or ***False***.
+-   **tags** - A list of tags for your deployment
+-   **account_type** - This is the VCS type, and only GitHub*** is
+    supported for now.
+-   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
+    any additional arguments for your build. It also includes the infra
+    size needed for the deployment. The options are -
+    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
+    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
+        76.8/hr
+    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
+        100.8/hr
+    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
+        136.0/hr
+    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
+        153.6/hr
+
+A valid example for *build_args* for the service you created -
+
+
+```
+args = {
+    "users": {
+      "admin": [
+        {
+          "user_name": "<your name>",
+          "public key": "<your public key>"
+        }
+      ]
+    },
+    "infra_reqs": "m5.xlarge",  
+}
+
+```
+
+> 📝 **Note:**
+>
+> <b>admin</b> here
+> is the role defined for the deployment in service.yaml
+> file
+>
+> The service used,
+> does not have requirements for any runtime or build arguments, so not
+> needed here.
+
+``` {.python}
+from oblv.models import CreateDeploymentInput
+input = CreateDeploymentInput(
+    owner="ObliviousAI",
+    repo="FastAPI-Enclave-Services",
+    account_type="github",
+    ref="master",
+    ref_type="branch",
+    region_name="us-east-1",
+    deployment_name="Depl",
+    visibility="private",
+    is_dev_env=True,
+    tags=[],
+    build_args=args
+)
+response = client.create_deployment(input)
+```
+
+
+On successful request, enclave creation is initiated, and it returns an
+id for the deployment, which can be later used to track the status and
+connection details for the enclave.
+
+To check the state of the deployment, run
+
+``` {.python}
+client.deployment_info(response.deployment_id).current_state
+```
+
+> 'CFT Initiated'
+
+
+When the deployment state becomes ***Running***, it indicates that the
+enclave is now available for connection.
+
+To connect to the enclave, you need **Oblv CLI** installed in your
+system. The commands to use the CLI can be found in this
+[documentation](https://docs.oblivious.ai/cli/usage_examples).
+
+Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
+
+The URL to connect to the enclave using CLI can be accessed using
+
+``` {.python}
+client.deployment_info(response.deployment_id).instance.service_url
+```
+
+>
+>'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
+>
+
+
+The PCR codes can be found using
+
+``` {.python}
+client.deployment_info(response.deployment_id).pcr_codes
+```
+
+>['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
+'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+
+
```

### Comparing `PyOblv-0.2.0/PyOblv.egg-info/SOURCES.txt` & `PyOblv-0.2.1/PyOblv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyOblv-0.2.0/README.md` & `PyOblv-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,213 +1,215 @@
-# PyOblv
-
-A Python library to access Oblivious OpenAPIs.
-
-## Usage
-
-First, create a client, with your API key. This key can be created in the
-[Oblivious Console UI](https://console.oblivious.ai/). Go to the
-settings page, and create your ApiKey. Once done, the client can be
-created as follows
-
-``` {.python}
-from oblv import authenticate
-client = authenticate(apikey=*your_key_here*)
-```
-
-
-Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
-
-
-
-### 1 Create a service
-
-A service refers to a branch/tag of your repository that needs to be
-deployed. For your first service. you can use the repository
-[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
-Execute the below command to create the service.
-
-``` {.python}
-client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
-    "auth": [
-        {
-            "auth_name": "auth_name",
-            "auth_type": "signed_headers"
-        }
-    ],
-    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
-    "build_args": [],
-    "meta": {
-        "author": "Team Oblivious",
-        "author_email": "hello@oblivious.ai",
-        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
-        "version": "0.1.0"
-    },
-    "paths": [
-        {
-            "access": "user",
-            "path": "/hello/",
-            "short_description": "Hello world example"
-        }
-    ],
-    "roles": [
-        {
-            "role_auth": "auth_name",
-            "role_cardinality": 1,
-            "role_description": "Role for the data scientist",
-            "role_name": "user"
-        }
-    ],
-    "traffic": {
-        "inbound": [
-            {
-                "name": "main_io",
-                "port": 80,
-                "type": "tcp"
-            }
-        ],
-        "outbound": [
-            {
-                "domain": "example.com",
-                "name": "example",
-                "port": 443,
-                "type": "tcp"
-            }
-        ]
-    }
-})
-```
-
-The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
-The response for the call above gives results as follows - 
-
-
->{ \
->&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
->&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
->&nbsp;&nbsp;&nbsp;&nbsp;} \
->} 
-
-
-You have now successfully created your first service, and it can be now deployed to an enclave.
-
-### 2 Enclave Creation
-
-To create an enclave, you need to decide on a few of the parameters -
-
--   **deployment_name** - A unique deployment name. You cannot have two
-    running deployments with the same name.
--   **region_name** - could be one of the AWS regions from
-    - ***us-east-1*** (N. Virginia) 
-    - ***us-west-2*** (Oregon)
-    - ***eu-central-1*** (Frankfurt)
-    - ***eu-west-2*** (London)
--   **visibility** - ***private*** or ***public***
--   **is_dev_env** - ***True*** or ***False***.
--   **tags** - A list of tags for your deployment
--   **account_type** - This is the VCS type, and only GitHub*** is
-    supported for now.
--   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
-    any additional arguments for your build. It also includes the infra
-    size needed for the deployment. The options are -
-    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
-    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
-        76.8/hr
-    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
-        100.8/hr
-    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
-        136.0/hr
-    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
-        153.6/hr
-
-A valid example for *build_args* for the service you created -
-
-
-```
-args = {
-    "users": {
-      "admin": [
-        {
-          "user_name": "<your name>",
-          "public key": "<your public key>"
-        }
-      ]
-    },
-    "infra_reqs": "m5.xlarge",  
-}
-
-```
-
-> 📝 **Note:**
->
-> <b>admin</b> here
-> is the role defined for the deployment in service.yaml
-> file
->
-> The service used,
-> does not have requirements for any runtime or build arguments, so not
-> needed here.
-
-``` {.python}
-from oblv.models import CreateDeploymentInput
-input = CreateDeploymentInput(
-    owner="ObliviousAI",
-    repo="FastAPI-Enclave-Services",
-    account_type="github",
-    ref="master",
-    ref_type="branch",
-    region_name="us-east-1",
-    deployment_name="Depl",
-    visibility="private",
-    is_dev_env=True,
-    tags=[],
-    build_args=args
-)
-response = client.create_deployment(input)
-```
-
-
-On successful request, enclave creation is initiated, and it returns an
-id for the deployment, which can be later used to track the status and
-connection details for the enclave.
-
-To check the state of the deployment, run
-
-``` {.python}
-client.deployment_info(response.deployment_id).current_state
-```
-
-> 'CFT Initiated'
-
-
-When the deployment state becomes ***Running***, it indicates that the
-enclave is now available for connection.
-
-To connect to the enclave, you need **Oblv CLI** installed in your
-system. The commands to use the CLI can be found in this
-[documentation](https://docs.oblivious.ai/cli/usage_examples).
-
-Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
-
-The URL to connect to the enclave using CLI can be accessed using
-
-``` {.python}
-client.deployment_info(response.deployment_id).instance.service_url
-```
-
->
->'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
->
-
-
-The PCR codes can be found using
-
-``` {.python}
-client.deployment_info(response.deployment_id).pcr_codes
-```
-
->['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
-'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
+***PyOblv is deprecated, and will not be supported in future. Kindly use [oblv-ctl](https://pypi.org/project/oblv-ctl/) to access Oblivious APIs.***
+
+# PyOblv
+
+A Python library to access Oblivious APIs.
+
+## Usage
+
+First, create a client, with your API key. This key can be created in the
+[Oblivious Console UI](https://console.oblivious.ai/). Go to the
+settings page, and create your ApiKey. Once done, the client can be
+created as follows
+
+``` {.python}
+from oblv import authenticate
+client = authenticate(apikey=*your_key_here*)
+```
+
+
+Using this client, all the Oblivious actions can be performed, including the deployment of enclaves. Below is a step-by-step guide, to creating your first deployment.
+
+
+
+### 1 Create a service
+
+A service refers to a branch/tag of your repository that needs to be
+deployed. For your first service. you can use the repository
+[ObliviousAI/FastAPI-Enclave-Services](https://github.com/ObliviousAI/FastAPI-Enclave-Services).
+Execute the below command to create the service.
+
+``` {.python}
+client.add_service(repo_owner="ObliviousAI",repo_name="FastAPI-Enclave-Services", ref="master", data = {
+    "auth": [
+        {
+            "auth_name": "auth_name",
+            "auth_type": "signed_headers"
+        }
+    ],
+    "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
+    "build_args": [],
+    "meta": {
+        "author": "Team Oblivious",
+        "author_email": "hello@oblivious.ai",
+        "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
+        "version": "0.1.0"
+    },
+    "paths": [
+        {
+            "access": "user",
+            "path": "/hello/",
+            "short_description": "Hello world example"
+        }
+    ],
+    "roles": [
+        {
+            "role_auth": "auth_name",
+            "role_cardinality": 1,
+            "role_description": "Role for the data scientist",
+            "role_name": "user"
+        }
+    ],
+    "traffic": {
+        "inbound": [
+            {
+                "name": "main_io",
+                "port": 80,
+                "type": "tcp"
+            }
+        ],
+        "outbound": [
+            {
+                "domain": "example.com",
+                "name": "example",
+                "port": 443,
+                "type": "tcp"
+            }
+        ]
+    }
+})
+```
+
+The data provided here is sample service data. You can update the data as per your requirements, adhering to the schema.
+The response for the call above gives results as follows - 
+
+
+>{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;"message": "Success", \
+>&nbsp;&nbsp;&nbsp;&nbsp;"service":&nbsp;&nbsp;&nbsp;&nbsp;{ \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"ref": "master", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"service_validated": true, \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"sha": "6b1b3e9cf6b0cb7264aad2fc80d91a009ccf0fc1", \
+>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "branch" \
+>&nbsp;&nbsp;&nbsp;&nbsp;} \
+>} 
+
+
+You have now successfully created your first service, and it can be now deployed to an enclave.
+
+### 2 Enclave Creation
+
+To create an enclave, you need to decide on a few of the parameters -
+
+-   **deployment_name** - A unique deployment name. You cannot have two
+    running deployments with the same name.
+-   **region_name** - could be one of the AWS regions from
+    - ***us-east-1*** (N. Virginia) 
+    - ***us-west-2*** (Oregon)
+    - ***eu-central-1*** (Frankfurt)
+    - ***eu-west-2*** (London)
+-   **visibility** - ***private*** or ***public***
+-   **is_dev_env** - ***True*** or ***False***.
+-   **tags** - A list of tags for your deployment
+-   **account_type** - This is the VCS type, and only GitHub*** is
+    supported for now.
+-   **build_args** - Arguments specific to your deployment. It includes adding users to their roles with their public keys, runtime arguments and
+    any additional arguments for your build. It also includes the infra
+    size needed for the deployment. The options are -
+    -   ***c5.xlarge*** - CPU:4 RAM:8 GB \-- Credit Utilization: 68.0/hr
+    -   ***m5.xlarge*** - CPU:4 RAM:16 GB \-- Credit Utilization:
+        76.8/hr
+    -   ***r5.xlarge*** - CPU:4 RAM:32 GB \-- Credit Utilization:
+        100.8/hr
+    -   ***c5.2xlarge*** - CPU:8 RAM:16 GB \-- Credit Utilization:
+        136.0/hr
+    -   ***m5.2xlarge*** - CPU:8 RAM:32 GB \-- Credit Utilization:
+        153.6/hr
+
+A valid example for *build_args* for the service you created -
+
+
+```
+args = {
+    "users": {
+      "admin": [
+        {
+          "user_name": "<your name>",
+          "public key": "<your public key>"
+        }
+      ]
+    },
+    "infra_reqs": "m5.xlarge",  
+}
+
+```
+
+> 📝 **Note:**
+>
+> <b>admin</b> here
+> is the role defined for the deployment in service.yaml
+> file
+>
+> The service used,
+> does not have requirements for any runtime or build arguments, so not
+> needed here.
+
+``` {.python}
+from oblv.models import CreateDeploymentInput
+input = CreateDeploymentInput(
+    owner="ObliviousAI",
+    repo="FastAPI-Enclave-Services",
+    account_type="github",
+    ref="master",
+    ref_type="branch",
+    region_name="us-east-1",
+    deployment_name="Depl",
+    visibility="private",
+    is_dev_env=True,
+    tags=[],
+    build_args=args
+)
+response = client.create_deployment(input)
+```
+
+
+On successful request, enclave creation is initiated, and it returns an
+id for the deployment, which can be later used to track the status and
+connection details for the enclave.
+
+To check the state of the deployment, run
+
+``` {.python}
+client.deployment_info(response.deployment_id).current_state
+```
+
+> 'CFT Initiated'
+
+
+When the deployment state becomes ***Running***, it indicates that the
+enclave is now available for connection.
+
+To connect to the enclave, you need **Oblv CLI** installed in your
+system. The commands to use the CLI can be found in this
+[documentation](https://docs.oblivious.ai/cli/usage_examples).
+
+Cli binaries can be found [here](https://docs.oblivious.ai/cli/binaries)
+
+The URL to connect to the enclave using CLI can be accessed using
+
+``` {.python}
+client.deployment_info(response.deployment_id).instance.service_url
+```
+
+>
+>'https://conso-appli-15aiaxip9pcxk-94364694.enclave.oblivious.ai'
+>
+
+
+The PCR codes can be found using
+
+``` {.python}
+client.deployment_info(response.deployment_id).pcr_codes
+```
+
+>['d8dd856bacf4a8f0840ab530579b906091803e818e01dc4b8f51c247a7adfcfe55b4ef5f17be6d53bb952d92d87a376c',
+'bcdf05fefccaa8e55bf2c8d6dee9e79bbff31e34bf28a99aa19e6b29c37ee80b214a414b7607236edf26fcb78654e63f','79477bad9504a347afb557a8ccd6f62ea61243311dff39f66944f5150242128da0cd070f0ce629c6beb6bb4f0b52f5ed' ]
```

### Comparing `PyOblv-0.2.0/cli/deployment.py` & `PyOblv-0.2.1/cli/deployment.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import enum
-import json
-
-import typer
-
-from oblv.models.create_deployment_input import CreateDeploymentInput
-
-from . import utils
-
-app = typer.Typer()
-
-regions = ["us-east-1","us-west-2","eu-central-1","eu-west-2"]
-
-class reg(enum.Enum):
-    N_Virginia ="us-east-1"
-    Oregon ="us-west-2"
-    Frankfurt= "eu-central-1"
-    London = "eu-west-2"
-
-@app.command(help="To create a deployment")
-def create(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(..., help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), name: str = typer.Argument(..., help=("Deployment Name")), public: bool = typer.Option(False, "--public", help="If provided, the deployment is made public"), is_dev: bool = typer.Option(False, "--is-dev", help="Sets the environment of the deployment as DEV"),region: reg = typer.Option("us-east-1",help="Region where enclave will be deployed. The options include [\"us-east-1\" (N. Virginia),  \"us-west-2\" (Oregon), \"eu-central-1\" (Frankfurt), \"eu-west-2\" (London)]"),args_file : str = typer.Option(None,help="arguments file path for enclave deployment")):
-    try:
-        client = utils.read_credentials()
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    try:
-        visibility = "public" if public else "private"
-        if args_file==None:
-            args_file = typer.prompt("Provide the arguments file for enclave deployment ")
-        with open(args_file,"r") as f:
-            args = json.load(f)
-        input = CreateDeploymentInput(repo_owner,repo_name,"github",ref,region._value_,name,visibility,is_dev,[],args)
-        res = client.create_deployment(input)
-        # print(res.message)
-        print("Deployment created successfully with id - {}".format(res.deployment_id))
-    except FileNotFoundError as e:
-        print("Could not find the arguments file at \""+args_file+"\"")
-    except Exception as e:
-        print(e)
-
-@app.command(help="To terminate a deployment")
-def terminate(deployment_id: str = typer.Argument(...,help="Deployment Id to terminate")):
-    try:
-        client = utils.read_credentials()
-        client.remove_deployment(deployment_id)
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-    else:
-        print("Terminating deployment with id {}".format(deployment_id))
-
-@app.command(help="To get the deployment information.\n\nIf no option is provided, complete information of the deployment is shown")
-def info(deployment_id: str = typer.Argument(...,help="Deployment Id for which information is requested"),state: bool = typer.Option(False,"--state",help="To get the current state of deployment"),instance: bool = typer.Option(False,"--instance",help="To get the instance info of deployment"),pcrs: bool = typer.Option(False,"--pcrs",help="To get the pcrs of deployment")):
-    try:
-        client = utils.read_credentials()
-        depl = client.deployment_info(deployment_id)
-        if not state and not instance and not pcrs:
-            print(depl)
-        else:
-            resp = {}
-            if state:
-                resp["state"]=depl.current_state
-            if pcrs:
-                resp["pcr_codes"]=depl.pcr_codes
-            if instance:
-                resp["instance"]=depl.instance
-            print(resp)
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-        
-@app.command(help="To get the owned deployments")
-def owned():
-    try:
-        client = utils.read_credentials()
-        depl_l = client.deployments()
-        depl = []
-        for d in depl_l if depl_l != None else []:
-            depl.append({
-                "deployment_id": d.deployment_id,
-                "deployment_name": d.deployment_name
-            })
-        print(depl)
-
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
+import enum
+import json
+
+import typer
+
+from oblv.models.create_deployment_input import CreateDeploymentInput
+
+from . import utils
+
+app = typer.Typer()
+
+regions = ["us-east-1","us-west-2","eu-central-1","eu-west-2"]
+
+class reg(enum.Enum):
+    N_Virginia ="us-east-1"
+    Oregon ="us-west-2"
+    Frankfurt= "eu-central-1"
+    London = "eu-west-2"
+
+@app.command(help="To create a deployment")
+def create(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(..., help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), name: str = typer.Argument(..., help=("Deployment Name")), public: bool = typer.Option(False, "--public", help="If provided, the deployment is made public"), is_dev: bool = typer.Option(False, "--is-dev", help="Sets the environment of the deployment as DEV"),region: reg = typer.Option("us-east-1",help="Region where enclave will be deployed. The options include [\"us-east-1\" (N. Virginia),  \"us-west-2\" (Oregon), \"eu-central-1\" (Frankfurt), \"eu-west-2\" (London)]"),args_file : str = typer.Option(None,help="arguments file path for enclave deployment")):
+    try:
+        client = utils.read_credentials()
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    try:
+        visibility = "public" if public else "private"
+        if args_file==None:
+            args_file = typer.prompt("Provide the arguments file for enclave deployment ")
+        with open(args_file,"r") as f:
+            args = json.load(f)
+        input = CreateDeploymentInput(repo_owner,repo_name,"github",ref,region._value_,name,visibility,is_dev,[],args)
+        res = client.create_deployment(input)
+        # print(res.message)
+        print("Deployment created successfully with id - {}".format(res.deployment_id))
+    except FileNotFoundError as e:
+        print("Could not find the arguments file at \""+args_file+"\"")
+    except Exception as e:
+        print(e)
+
+@app.command(help="To terminate a deployment")
+def terminate(deployment_id: str = typer.Argument(...,help="Deployment Id to terminate")):
+    try:
+        client = utils.read_credentials()
+        client.remove_deployment(deployment_id)
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+    else:
+        print("Terminating deployment with id {}".format(deployment_id))
+
+@app.command(help="To get the deployment information.\n\nIf no option is provided, complete information of the deployment is shown")
+def info(deployment_id: str = typer.Argument(...,help="Deployment Id for which information is requested"),state: bool = typer.Option(False,"--state",help="To get the current state of deployment"),instance: bool = typer.Option(False,"--instance",help="To get the instance info of deployment"),pcrs: bool = typer.Option(False,"--pcrs",help="To get the pcrs of deployment")):
+    try:
+        client = utils.read_credentials()
+        depl = client.deployment_info(deployment_id)
+        if not state and not instance and not pcrs:
+            print(depl)
+        else:
+            resp = {}
+            if state:
+                resp["state"]=depl.current_state
+            if pcrs:
+                resp["pcr_codes"]=depl.pcr_codes
+            if instance:
+                resp["instance"]=depl.instance
+            print(resp)
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+        
+@app.command(help="To get the owned deployments")
+def owned():
+    try:
+        client = utils.read_credentials()
+        depl_l = client.deployments()
+        depl = []
+        for d in depl_l if depl_l != None else []:
+            depl.append({
+                "deployment_id": d.deployment_id,
+                "deployment_name": d.deployment_name
+            })
+        print(depl)
+
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
```

### Comparing `PyOblv-0.2.0/cli/main.py` & `PyOblv-0.2.1/cli/main.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import os
-
-import typer
-from rich.text import Text
-
-from oblv import __version__, authenticate
-
-from . import deployment, service, utils
-
-app = typer.Typer(no_args_is_help=True, rich_markup_mode="markdown", help="""**Oblvious Controller v{}**   
-**Oblivious Software Ltd. <oblivious.ai>**  
-======
-  
-__Description__  
-
----
-
-The Oblivious Controller is a command line tool to manage your Oblivious services.
- """.format(__version__),add_completion=False)
-
-
-@app.command(help="Command to login to oblv")
-def login(apikey: str):
-    if apikey=="":
-        apikey = typer.prompt("Kindly provide your api key ")
-    try:
-        client = authenticate(apikey)
-        credentials = "oblivious_user_id = {}\ntoken = {}".format(client.oblivious_user_id,client.token)
-        os.makedirs(os.path.dirname(utils.cred_file_path), exist_ok=True)
-        with open(utils.cred_file_path,'w') as f:
-            f.write(credentials)
-    except Exception as e:
-        print(e)
-    else:
-        print("Successfully logged in")
-        
-@app.command(help="Command to clear and invalidate the token")
-def logout():
-    try:
-        if os.path.exists(utils.cred_file_path):
-            with open(utils.cred_file_path,'w') as f:
-                #Just overwriting the file, whether login exists or not
-                f.write("")
-    except FileNotFoundError as e:
-        #Case where .oblv folder was never generated
-        #With the check of path exists makes no sense
-        print(".oblv folder not found")
-    except Exception as e:
-        print(e)
-    else:
-        print("Successfully logged out")
-    
-@app.command(help="Command to fetch the VCS accounts")
-def accounts():
-    try:
-        client = utils.read_credentials()
-        # console.print("["+",\n".join([x.__repr__() for x in client.accounts()])+"]")
-        utils.render_output(client.accounts())
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-    
-@app.command(help="Command to fetch/set the Public Key")
-def psk(set_key : str = typer.Option(None, help="Public key to be set")):
-    try:
-        client = utils.read_credentials()
-        if set_key!=None:
-            client.set_psk(set_key)
-        else:
-            utils.render_output(client.psk())
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-    
-app.add_typer(service.app, name="service", help="Commands to interact with the services")
-app.add_typer(deployment.app, name="deployment", help="Commands to interact with the deployments")
-
-
-
-if __name__ == "__main__":
-    app()
+import os
+
+import typer
+from rich.text import Text
+
+from oblv import __version__, authenticate
+
+from . import deployment, service, utils
+
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="markdown", help="""**Oblvious Controller v{}**   
+**Oblivious Software Ltd. <oblivious.ai>**  
+======
+  
+__Description__  
+
+---
+
+The Oblivious Controller is a command line tool to manage your Oblivious services.
+ """.format(__version__),add_completion=False)
+
+
+@app.command(help="Command to login to oblv")
+def login(apikey: str):
+    if apikey=="":
+        apikey = typer.prompt("Kindly provide your api key ")
+    try:
+        client = authenticate(apikey)
+        credentials = "oblivious_user_id = {}\ntoken = {}".format(client.oblivious_user_id,client.token)
+        os.makedirs(os.path.dirname(utils.cred_file_path), exist_ok=True)
+        with open(utils.cred_file_path,'w') as f:
+            f.write(credentials)
+    except Exception as e:
+        print(e)
+    else:
+        print("Successfully logged in")
+        
+@app.command(help="Command to clear and invalidate the token")
+def logout():
+    try:
+        if os.path.exists(utils.cred_file_path):
+            with open(utils.cred_file_path,'w') as f:
+                #Just overwriting the file, whether login exists or not
+                f.write("")
+    except FileNotFoundError as e:
+        #Case where .oblv folder was never generated
+        #With the check of path exists makes no sense
+        print(".oblv folder not found")
+    except Exception as e:
+        print(e)
+    else:
+        print("Successfully logged out")
+    
+@app.command(help="Command to fetch the VCS accounts")
+def accounts():
+    try:
+        client = utils.read_credentials()
+        # console.print("["+",\n".join([x.__repr__() for x in client.accounts()])+"]")
+        utils.render_output(client.accounts())
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+    
+@app.command(help="Command to fetch/set the Public Key")
+def psk(set_key : str = typer.Option(None, help="Public key to be set")):
+    try:
+        client = utils.read_credentials()
+        if set_key!=None:
+            client.set_psk(set_key)
+        else:
+            utils.render_output(client.psk())
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+    
+app.add_typer(service.app, name="service", help="Commands to interact with the services")
+app.add_typer(deployment.app, name="deployment", help="Commands to interact with the deployments")
+
+
+
+if __name__ == "__main__":
+    app()
```

### Comparing `PyOblv-0.2.0/cli/service.py` & `PyOblv-0.2.1/cli/service.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import json
-
-import typer
-
-from . import utils
-
-app = typer.Typer()
-
-
-@app.command(help="To create a new service")
-def create(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag",help="If provided, the ref is considered to be a tag on repository"), service_file : str = typer.Option(None,help="Service yaml file in json format. Not allowed with --tag")):
-    try:
-        client = utils.read_credentials()
-        if tag:
-            client.add_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
-        else:
-            args = {}
-            if service_file!=None:
-                with open(service_file,"r") as f:
-                    args = json.load(f)
-            client.add_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref, data=args)
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-    else:
-        print("Successfully added the service")
-
-@app.command(help="To remove an existing service")
-def remove(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag", help="If provided, the ref is considered to be a tag on repository")):
-    try:
-        client = utils.read_credentials()
-        if tag:
-            client.remove_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
-        else:
-            client.remove_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref)
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-    else:
-        print("Successfully removed the service")
-
-@app.command(help="To fetch user's services list")
-def fetch():
-    try:
-        client = utils.read_credentials()
-        print(client.user_services())
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-
-@app.command(help="To updates user's service")
-def update(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag", help="If provided, the ref is considered to be a tag on repository"), service_file : str = typer.Option(None,help="Service yaml file in json format. Not allowed with --tag")):
-    try:
-        client = utils.read_credentials()
-        if tag:
-            client.update_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
-        else:
-            args = {}
-            if service_file!=None:
-                with open(service_file,"r") as f:
-                    args = json.load(f)
-            client.update_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref, data=args)
-    except FileNotFoundError as e:
-        print("Kindly login before performing this action")
-    except Exception as e:
-        print(e)
-    else:
-        print("Successfully updated the service")
+import json
+
+import typer
+
+from . import utils
+
+app = typer.Typer()
+
+
+@app.command(help="To create a new service")
+def create(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag",help="If provided, the ref is considered to be a tag on repository"), service_file : str = typer.Option(None,help="Service yaml file in json format. Not allowed with --tag")):
+    try:
+        client = utils.read_credentials()
+        if tag:
+            client.add_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
+        else:
+            args = {}
+            if service_file!=None:
+                with open(service_file,"r") as f:
+                    args = json.load(f)
+            client.add_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref, data=args)
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+    else:
+        print("Successfully added the service")
+
+@app.command(help="To remove an existing service")
+def remove(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag", help="If provided, the ref is considered to be a tag on repository")):
+    try:
+        client = utils.read_credentials()
+        if tag:
+            client.remove_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
+        else:
+            client.remove_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref)
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+    else:
+        print("Successfully removed the service")
+
+@app.command(help="To fetch user's services list")
+def fetch():
+    try:
+        client = utils.read_credentials()
+        print(client.user_services())
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+
+@app.command(help="To updates user's service")
+def update(repo_owner: str = typer.Argument(..., help=("Repository Owner")), repo_name: str = typer.Argument(...,help=("Repository Name")), ref: str = typer.Argument(..., help=("Service ref name")), tag : bool = typer.Option(False, "--tag", help="If provided, the ref is considered to be a tag on repository"), service_file : str = typer.Option(None,help="Service yaml file in json format. Not allowed with --tag")):
+    try:
+        client = utils.read_credentials()
+        if tag:
+            client.update_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref,ref_type="tag")
+        else:
+            args = {}
+            if service_file!=None:
+                with open(service_file,"r") as f:
+                    args = json.load(f)
+            client.update_service(repo_owner=repo_owner,repo_name=repo_name,ref=ref, data=args)
+    except FileNotFoundError as e:
+        print("Kindly login before performing this action")
+    except Exception as e:
+        print(e)
+    else:
+        print("Successfully updated the service")
```

### Comparing `PyOblv-0.2.0/oblv/api/account/get_user_accounts_account_get.py` & `PyOblv-0.2.1/oblv/api/account/get_user_accounts_account_get.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-from typing import Any, Dict, List, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.account import Account
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/account".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
-    if response.status_code == 200:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = Account.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
-
-        return response_200
-    if response.status_code == 204:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
-    """Get User Accounts
-
-     API to fetch user's linked VCS accounts
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
-    """Get User Accounts
-
-     API to fetch user's linked VCS accounts
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
-    """Get User Accounts
-
-     API to fetch user's linked VCS accounts
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
-    """Get User Accounts
-
-     API to fetch user's linked VCS accounts
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, List, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.account import Account
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/account".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
+    if response.status_code == 200:
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = Account.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
+
+        return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
+    """Get User Accounts
+
+     API to fetch user's linked VCS accounts
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
+    """Get User Accounts
+
+     API to fetch user's linked VCS accounts
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
+    """Get User Accounts
+
+     API to fetch user's linked VCS accounts
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[Any, HTTPValidationError, List[Account], MessageModel]]:
+    """Get User Accounts
+
+     API to fetch user's linked VCS accounts
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/auth/logout_session_logout_delete.py` & `PyOblv-0.2.1/oblv/api/auth/logout_session_logout_delete.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/logout".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "delete",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = MessageModel.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
-
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
-
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
-
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Logout Session
-
-     This API invalidates the user's token. After a successul response, the user will not be able to use
-    the auth token provided in the auth APIs.
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/logout".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = MessageModel.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Logout Session
+
+     This API invalidates the user's token. After a successul response, the user will not be able to use
+    the auth token provided in the auth APIs.
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Logout Session
+
+     This API invalidates the user's token. After a successul response, the user will not be able to use
+    the auth token provided in the auth APIs.
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Logout Session
+
+     This API invalidates the user's token. After a successul response, the user will not be able to use
+    the auth token provided in the auth APIs.
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Logout Session
+
+     This API invalidates the user's token. After a successul response, the user will not be able to use
+    the auth token provided in the auth APIs.
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/deployment/create_new_deployment_deployment_post.py` & `PyOblv-0.2.1/oblv/api/user/add_user_public_shared_key_user_psk_put.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,192 +1,184 @@
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.create_deployment_input import CreateDeploymentInput
-from ...models.create_deployment_response import CreateDeploymentResponse
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/deployment".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    json_json_body = json_body.to_dict()
-
-    return {
-        "method": "post",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "json": json_json_body,
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == 201:
-        response_201 = CreateDeploymentResponse.from_dict(response.json())
-
-        return response_201
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
-    oblivious_user_id: str,
-) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
-
-     API to create a new deployment.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
-
-    Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
-
-     API to create a new deployment.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
-
-    Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
-    oblivious_user_id: str,
-) -> Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
-
-     API to create a new deployment.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
-
-    Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    json_body: CreateDeploymentInput,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Create Deployment
-
-     API to create a new deployment.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (CreateDeploymentInput):
-
-    Returns:
-        Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            json_body=json_body,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.psk import PSK
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    json_body: PSK,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/user/psk".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    json_json_body = json_body.to_dict()
+
+    return {
+        "method": "put",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "json": json_json_body,
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, PSK]]:
+    if response.status_code == 200:
+        response_200 = response.json()
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    json_body: PSK,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
+    """Update User PSK
+
+     API to update user's psk
+
+    Args:
+        oblivious_user_id (str):
+        json_body (PSK):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, PSK]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    json_body: PSK,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, PSK]]:
+    """Update User PSK
+
+     API to update user's psk
+
+    Args:
+        oblivious_user_id (str):
+        json_body (PSK):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, PSK]]
+    """
+
+    return sync_detailed(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    json_body: PSK,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
+    """Update User PSK
+
+     API to update user's psk
+
+    Args:
+        oblivious_user_id (str):
+        json_body (PSK):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, PSK]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    json_body: PSK,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, PSK]]:
+    """Update User PSK
+
+     API to update user's psk
+
+    Args:
+        oblivious_user_id (str):
+        json_body (PSK):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, PSK]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/deployment/delete_deployment_deployment_delete.py` & `PyOblv-0.2.1/oblv/api/deployment/delete_deployment_deployment_delete.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Dict[str, Any]:
-    url = "{}/deployment".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["deployment_id"] = deployment_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "delete",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = cast(Any, response.json())
-        return response_200
-    if response.status_code == 201:
-        response_201 = MessageModel.from_dict(response.json())
-
-        return response_201
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Delete Deployment
-
-     API to initiate termination of a deployment.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Delete Deployment
-
-     API to initiate termination of a deployment.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Delete Deployment
-
-     API to initiate termination of a deployment.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Delete Deployment
-
-     API to initiate termination of a deployment.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            deployment_id=deployment_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Dict[str, Any]:
+    url = "{}/deployment".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["deployment_id"] = deployment_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = cast(Any, response.json())
+        return response_200
+    if response.status_code == 201:
+        response_201 = MessageModel.from_dict(response.json())
+
+        return response_201
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
+    """Delete Deployment
+
+     API to initiate termination of a deployment.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    """Delete Deployment
+
+     API to initiate termination of a deployment.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
+    """Delete Deployment
+
+     API to initiate termination of a deployment.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    """Delete Deployment
+
+     API to initiate termination of a deployment.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            deployment_id=deployment_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/deployment/generate_build_args_deployment_arguments_get.py` & `PyOblv-0.2.1/oblv/api/deployment/generate_build_args_deployment_arguments_get.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.build_args_schema import BuildArgsSchema
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    owner: str,
-    repo: str,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-) -> Dict[str, Any]:
-    url = "{}/deployment/arguments".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["owner"] = owner
-
-    params["repo"] = repo
-
-    params["ref"] = ref
-
-    params["ref_type"] = ref_type
-
-    params["account_type"] = account_type
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = BuildArgsSchema.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 409:
-        response_409 = MessageModel.from_dict(response.json())
-
-        return response_409
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, BuildArgsSchema, HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    owner: str,
-    repo: str,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
-    """Get Build Deployment Arguments
-
-     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
-    at which point it was generated. This is to be passed to the create deployment API.
-
-    Note - A service could have different build args schema depending on the service's commit history.
-
-    Args:
-        oblivious_user_id (str):
-        owner (str):
-        repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        owner=owner,
-        repo=repo,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    owner: str,
-    repo: str,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
-    """Get Build Deployment Arguments
-
-     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
-    at which point it was generated. This is to be passed to the create deployment API.
-
-    Note - A service could have different build args schema depending on the service's commit history.
-
-    Args:
-        oblivious_user_id (str):
-        owner (str):
-        repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        owner=owner,
-        repo=repo,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    owner: str,
-    repo: str,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
-    """Get Build Deployment Arguments
-
-     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
-    at which point it was generated. This is to be passed to the create deployment API.
-
-    Note - A service could have different build args schema depending on the service's commit history.
-
-    Args:
-        oblivious_user_id (str):
-        owner (str):
-        repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        owner=owner,
-        repo=repo,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    owner: str,
-    repo: str,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
-    """Get Build Deployment Arguments
-
-     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
-    at which point it was generated. This is to be passed to the create deployment API.
-
-    Note - A service could have different build args schema depending on the service's commit history.
-
-    Args:
-        oblivious_user_id (str):
-        owner (str):
-        repo (str):
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            owner=owner,
-            repo=repo,
-            ref=ref,
-            ref_type=ref_type,
-            account_type=account_type,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.build_args_schema import BuildArgsSchema
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    owner: str,
+    repo: str,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+) -> Dict[str, Any]:
+    url = "{}/deployment/arguments".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["owner"] = owner
+
+    params["repo"] = repo
+
+    params["ref"] = ref
+
+    params["ref_type"] = ref_type
+
+    params["account_type"] = account_type
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = BuildArgsSchema.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 409:
+        response_409 = MessageModel.from_dict(response.json())
+
+        return response_409
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, BuildArgsSchema, HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    owner: str,
+    repo: str,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
+    """Get Build Deployment Arguments
+
+     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
+    at which point it was generated. This is to be passed to the create deployment API.
+
+    Note - A service could have different build args schema depending on the service's commit history.
+
+    Args:
+        oblivious_user_id (str):
+        owner (str):
+        repo (str):
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        owner=owner,
+        repo=repo,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    owner: str,
+    repo: str,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
+    """Get Build Deployment Arguments
+
+     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
+    at which point it was generated. This is to be passed to the create deployment API.
+
+    Note - A service could have different build args schema depending on the service's commit history.
+
+    Args:
+        oblivious_user_id (str):
+        owner (str):
+        repo (str):
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        owner=owner,
+        repo=repo,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    owner: str,
+    repo: str,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
+    """Get Build Deployment Arguments
+
+     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
+    at which point it was generated. This is to be passed to the create deployment API.
+
+    Note - A service could have different build args schema depending on the service's commit history.
+
+    Args:
+        oblivious_user_id (str):
+        owner (str):
+        repo (str):
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        owner=owner,
+        repo=repo,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    owner: str,
+    repo: str,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]:
+    """Get Build Deployment Arguments
+
+     API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
+    at which point it was generated. This is to be passed to the create deployment API.
+
+    Note - A service could have different build args schema depending on the service's commit history.
+
+    Args:
+        oblivious_user_id (str):
+        owner (str):
+        repo (str):
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[BuildArgsSchema, HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            owner=owner,
+            repo=repo,
+            ref=ref,
+            ref_type=ref_type,
+            account_type=account_type,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/deployment/get_available_deployments_deployment_available_get.py` & `PyOblv-0.2.1/oblv/api/deployment/get_available_deployments_deployment_available_get.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.available_deployment_list import AvailableDeploymentList
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Dict[str, Any]:
-    url = "{}/deployment/available".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["page"] = page
-
-    params["per_page"] = per_page
-
-    params["search_term"] = search_term
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = AvailableDeploymentList.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
-
-     API to fetch all the deployments the user can connect to.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
-
-     API to fetch all the deployments the user can connect to.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
-
-     API to fetch all the deployments the user can connect to.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Available Deployments
-
-     API to fetch all the deployments the user can connect to.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            page=page,
-            per_page=per_page,
-            search_term=search_term,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.available_deployment_list import AvailableDeploymentList
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Dict[str, Any]:
+    url = "{}/deployment/available".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["page"] = page
+
+    params["per_page"] = per_page
+
+    params["search_term"] = search_term
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = AvailableDeploymentList.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Available Deployments
+
+     API to fetch all the deployments the user can connect to.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Available Deployments
+
+     API to fetch all the deployments the user can connect to.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Available Deployments
+
+     API to fetch all the deployments the user can connect to.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Optional[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Available Deployments
+
+     API to fetch all the deployments the user can connect to.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[AvailableDeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            page=page,
+            per_page=per_page,
+            search_term=search_term,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/deployment/get_deployment_info_deployment_get.py` & `PyOblv-0.2.1/oblv/api/deployment/get_deployment_info_deployment_get.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.deployment_response import DeploymentResponse
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Dict[str, Any]:
-    url = "{}/deployment".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["deployment_id"] = deployment_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, DeploymentResponse, HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = DeploymentResponse.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
-    """Get Deployment
-
-     API to fetch a deployment's details.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            deployment_id=deployment_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.deployment_response import DeploymentResponse
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Dict[str, Any]:
+    url = "{}/deployment".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["deployment_id"] = deployment_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, DeploymentResponse, HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = DeploymentResponse.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
+
+     API to fetch a deployment's details.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
+
+     API to fetch a deployment's details.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
+
+     API to fetch a deployment's details.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Optional[Union[DeploymentResponse, HTTPValidationError, MessageModel]]:
+    """Get Deployment
+
+     API to fetch a deployment's details.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[DeploymentResponse, HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            deployment_id=deployment_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/deployment/get_deployment_roles_deployment_roles_get.py` & `PyOblv-0.2.1/oblv/api/repo/search_repo_from_vcs_repo_search_get.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,196 +1,195 @@
-from typing import Any, Dict, List, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.role_response import RoleResponse
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Dict[str, Any]:
-    url = "{}/deployment/roles".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["deployment_id"] = deployment_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    if response.status_code == 200:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = RoleResponse.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 501:
-        response_501 = MessageModel.from_dict(response.json())
-
-        return response_501
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
-
-     API to get a deployment's roles.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
-
-     API to get a deployment's roles.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
-
-     API to get a deployment's roles.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        deployment_id=deployment_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    deployment_id: str,
-) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
-    """Get Deployment Roles
-
-     API to get a deployment's roles.
-
-    Args:
-        oblivious_user_id (str):
-        deployment_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            deployment_id=deployment_id,
-        )
-    ).parsed
+from typing import Any, Dict, List, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.repo import Repo
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    search_string: str,
+) -> Dict[str, Any]:
+    url = "{}/repo/search".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["search_string"] = search_string
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+    if response.status_code == 200:
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = Repo.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
+
+        return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    search_string: str,
+) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+    """Search Repo
+
+     API to search a repository in VCS, on which the user has access (via their own account, or by any
+    organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        search_string (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        search_string=search_string,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    search_string: str,
+) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+    """Search Repo
+
+     API to search a repository in VCS, on which the user has access (via their own account, or by any
+    organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        search_string (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        search_string=search_string,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    search_string: str,
+) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+    """Search Repo
+
+     API to search a repository in VCS, on which the user has access (via their own account, or by any
+    organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        search_string (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        search_string=search_string,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    search_string: str,
+) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
+    """Search Repo
+
+     API to search a repository in VCS, on which the user has access (via their own account, or by any
+    organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        search_string (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            search_string=search_string,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/deployment/get_user_owned_deployments_deployment_owned_get.py` & `PyOblv-0.2.1/oblv/api/deployment/get_user_owned_deployments_deployment_owned_get.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.deployment_list import DeploymentList
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Dict[str, Any]:
-    url = "{}/deployment/owned".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["page"] = page
-
-    params["per_page"] = per_page
-
-    params["search_term"] = search_term
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = DeploymentList.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
-
-     API to fetch a user's owned deployments.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
-
-     API to fetch a user's owned deployments.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
-
-     API to fetch a user's owned deployments.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
-    """Get Owned Deployments
-
-     API to fetch a user's owned deployments.
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-
-    Returns:
-        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            page=page,
-            per_page=per_page,
-            search_term=search_term,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.deployment_list import DeploymentList
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Dict[str, Any]:
+    url = "{}/deployment/owned".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["page"] = page
+
+    params["per_page"] = per_page
+
+    params["search_term"] = search_term
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = DeploymentList.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Owned Deployments
+
+     API to fetch a user's owned deployments.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Owned Deployments
+
+     API to fetch a user's owned deployments.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Owned Deployments
+
+     API to fetch a user's owned deployments.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+) -> Optional[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]:
+    """Get Owned Deployments
+
+     API to fetch a user's owned deployments.
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+
+    Returns:
+        Response[Union[Any, DeploymentList, HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            page=page,
+            per_page=per_page,
+            search_term=search_term,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/notification/get_all_notifications_notification_get.py` & `PyOblv-0.2.1/oblv/api/notification/get_all_notifications_notification_get.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-from typing import Any, Dict, List, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.notification_response import NotificationResponse
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/notification".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    if response.status_code == 200:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = NotificationResponse.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
-
-        return response_200
-    if response.status_code == 204:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
-    """Get All Notifications
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, List, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.notification_response import NotificationResponse
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/notification".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+    if response.status_code == 200:
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = NotificationResponse.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
+
+        return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+    """Get All Notifications
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+    """Get All Notifications
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+    """Get All Notifications
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]:
+    """Get All Notifications
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, List[NotificationResponse], MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/notification/get_notification_details_notification_notification_id_get.py` & `PyOblv-0.2.1/oblv/api/notification/mark_all_notification_read_notification_delete.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,174 +1,158 @@
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/notification/{notification_id}".format(client.base_url, notification_id=notification_id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    if response.status_code == 200:
-        response_200 = cast(str, response.json())
-        return response_200
-    if response.status_code == 204:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        notification_id=notification_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
-    """
-
-    return sync_detailed(
-        notification_id=notification_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        notification_id=notification_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    """Get Notification Details
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, str]]
-    """
-
-    return (
-        await asyncio_detailed(
-            notification_id=notification_id,
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/notification".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    if response.status_code == 200:
+        response_200 = cast(str, response.json())
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark All Notification Read
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/notification/mark_all_notification_read_notification_delete.py` & `PyOblv-0.2.1/oblv/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,158 +1,172 @@
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/notification".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "delete",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    if response.status_code == 200:
-        response_200 = cast(str, response.json())
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark All Notification Read
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.user_credit_utilization import UserCreditUtilization
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/user/credit_usage".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, UserCreditUtilization]]:
+    if response.status_code == 200:
+        response_200 = UserCreditUtilization.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
+    """Get User Credit Usage
+
+     API to fetch user's credit usage
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
+    """Get User Credit Usage
+
+     API to fetch user's credit usage
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
+    """Get User Credit Usage
+
+     API to fetch user's credit usage
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
+    """Get User Credit Usage
+
+     API to fetch user's credit usage
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/notification/mark_notification_read_notification_notification_id_delete.py` & `PyOblv-0.2.1/oblv/api/repo/get_all_repos_repo_linked_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,180 @@
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/notification/{notification_id}".format(client.base_url, notification_id=notification_id)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "delete",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    if response.status_code == 200:
-        response_200 = cast(str, response.json())
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark Notification Read
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        notification_id=notification_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark Notification Read
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    return sync_detailed(
-        notification_id=notification_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark Notification Read
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        notification_id=notification_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    notification_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Mark Notification Read
-
-    Args:
-        notification_id (str):
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    return (
-        await asyncio_detailed(
-            notification_id=notification_id,
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, List, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.repo_all_response import RepoAllResponse
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/repo/linked".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
+    if response.status_code == 200:
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = RepoAllResponse.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
+
+        return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
+    """Get User Repos
+
+     API to fetch user's repo without services
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
+    """Get User Repos
+
+     API to fetch user's repo without services
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
+    """Get User Repos
+
+     API to fetch user's repo without services
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
+    """Get User Repos
+
+     API to fetch user's repo without services
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/repo/get_all_repos_repo_linked_get.py` & `PyOblv-0.2.1/oblv/api/notification/mark_notification_read_notification_notification_id_delete.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,180 +1,171 @@
-from typing import Any, Dict, List, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.repo_all_response import RepoAllResponse
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/repo/linked".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
-    if response.status_code == 200:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = RepoAllResponse.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
-
-        return response_200
-    if response.status_code == 204:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
-    """Get User Repos
-
-     API to fetch user's repo without services
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
-    """Get User Repos
-
-     API to fetch user's repo without services
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
-    """Get User Repos
-
-     API to fetch user's repo without services
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]:
-    """Get User Repos
-
-     API to fetch user's repo without services
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, List[RepoAllResponse], MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/notification/{notification_id}".format(client.base_url, notification_id=notification_id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    if response.status_code == 200:
+        response_200 = cast(str, response.json())
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark Notification Read
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        notification_id=notification_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark Notification Read
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    return sync_detailed(
+        notification_id=notification_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark Notification Read
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        notification_id=notification_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Mark Notification Read
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    return (
+        await asyncio_detailed(
+            notification_id=notification_id,
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/repo/get_repo_from_vcs_repo_get.py` & `PyOblv-0.2.1/oblv/api/repo/get_repo_from_vcs_repo_get.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.vcs_repo_response import VCSRepoResponse
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-) -> Dict[str, Any]:
-    url = "{}/repo".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["page"] = page
-
-    params["per_page"] = per_page
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, VCSRepoResponse]]:
-    if response.status_code == 200:
-        response_200 = VCSRepoResponse.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, VCSRepoResponse]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-) -> Response[Union[HTTPValidationError, VCSRepoResponse]]:
-    """Get Repos From VCS
-
-     API to get all the repositories from VCS, on which the user has access (via their own account, or by
-    any organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-
-    Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-) -> Optional[Union[HTTPValidationError, VCSRepoResponse]]:
-    """Get Repos From VCS
-
-     API to get all the repositories from VCS, on which the user has access (via their own account, or by
-    any organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-
-    Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-) -> Response[Union[HTTPValidationError, VCSRepoResponse]]:
-    """Get Repos From VCS
-
-     API to get all the repositories from VCS, on which the user has access (via their own account, or by
-    any organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-
-    Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-) -> Optional[Union[HTTPValidationError, VCSRepoResponse]]:
-    """Get Repos From VCS
-
-     API to get all the repositories from VCS, on which the user has access (via their own account, or by
-    any organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-
-    Returns:
-        Response[Union[HTTPValidationError, VCSRepoResponse]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            page=page,
-            per_page=per_page,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.vcs_repo_response import VCSRepoResponse
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+) -> Dict[str, Any]:
+    url = "{}/repo".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["page"] = page
+
+    params["per_page"] = per_page
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, VCSRepoResponse]]:
+    if response.status_code == 200:
+        response_200 = VCSRepoResponse.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, VCSRepoResponse]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+) -> Response[Union[HTTPValidationError, VCSRepoResponse]]:
+    """Get Repos From VCS
+
+     API to get all the repositories from VCS, on which the user has access (via their own account, or by
+    any organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+
+    Returns:
+        Response[Union[HTTPValidationError, VCSRepoResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+) -> Optional[Union[HTTPValidationError, VCSRepoResponse]]:
+    """Get Repos From VCS
+
+     API to get all the repositories from VCS, on which the user has access (via their own account, or by
+    any organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+
+    Returns:
+        Response[Union[HTTPValidationError, VCSRepoResponse]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+) -> Response[Union[HTTPValidationError, VCSRepoResponse]]:
+    """Get Repos From VCS
+
+     API to get all the repositories from VCS, on which the user has access (via their own account, or by
+    any organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+
+    Returns:
+        Response[Union[HTTPValidationError, VCSRepoResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+) -> Optional[Union[HTTPValidationError, VCSRepoResponse]]:
+    """Get Repos From VCS
+
+     API to get all the repositories from VCS, on which the user has access (via their own account, or by
+    any organization they are member of).
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+
+    Returns:
+        Response[Union[HTTPValidationError, VCSRepoResponse]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            page=page,
+            per_page=per_page,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/repo/get_repo_refs_repo_refs_get.py` & `PyOblv-0.2.1/oblv/api/repo/get_repo_refs_repo_refs_get.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.ref_response import RefResponse
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Dict[str, Any]:
-    url = "{}/repo/refs".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["account_type"] = account_type
-
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["repo_owner"] = repo_owner
-
-    params["repo_name"] = repo_name
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RefResponse]]:
-    if response.status_code == 200:
-        response_200 = RefResponse.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
-
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
-
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
-    """
-
-    return sync_detailed(
-        client=client,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
-
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
-    """Get Repo Refs
-
-     API to fetch the repository refs (branches and tags).
-
-    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
-    owner and name is given, then the repo is searched in the VCS (all public repos included).
-
-    Note - Either repo id must be provided or its owner and name must be given. A failed response is
-    provided if both or none of them are given.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            account_type=account_type,
-            oblivious_user_id=oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.ref_response import RefResponse
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Dict[str, Any]:
+    url = "{}/repo/refs".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["account_type"] = account_type
+
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["repo_owner"] = repo_owner
+
+    params["repo_name"] = repo_name
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, RefResponse]]:
+    if response.status_code == 200:
+        response_200 = RefResponse.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
+
+     API to fetch the repository refs (branches and tags).
+
+    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
+    owner and name is given, then the repo is searched in the VCS (all public repos included).
+
+    Note - Either repo id must be provided or its owner and name must be given. A failed response is
+    provided if both or none of them are given.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
+
+     API to fetch the repository refs (branches and tags).
+
+    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
+    owner and name is given, then the repo is searched in the VCS (all public repos included).
+
+    Note - Either repo id must be provided or its owner and name must be given. A failed response is
+    provided if both or none of them are given.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+    """
+
+    return sync_detailed(
+        client=client,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
+
+     API to fetch the repository refs (branches and tags).
+
+    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
+    owner and name is given, then the repo is searched in the VCS (all public repos included).
+
+    Note - Either repo id must be provided or its owner and name must be given. A failed response is
+    provided if both or none of them are given.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, RefResponse]]:
+    """Get Repo Refs
+
+     API to fetch the repository refs (branches and tags).
+
+    If parameter **repo_id** is provided, then it checks for a linked user repo, otherwise, if repo's
+    owner and name is given, then the repo is searched in the VCS (all public repos included).
+
+    Note - Either repo id must be provided or its owner and name must be given. A failed response is
+    provided if both or none of them are given.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, RefResponse]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            account_type=account_type,
+            oblivious_user_id=oblivious_user_id,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/repo/get_repo_repo_repo_id_get.py` & `PyOblv-0.2.1/oblv/api/repo/get_repo_repo_repo_id_get.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.repo_services import RepoServices
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    repo_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Dict[str, Any]:
-    url = "{}/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_id=repo_id)
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["account_type"] = account_type
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    if response.status_code == 200:
-        response_200 = RepoServices.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    repo_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
-    """
-
-    kwargs = _get_kwargs(
-        repo_id=repo_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    repo_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
-    """
-
-    return sync_detailed(
-        repo_id=repo_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
-    ).parsed
-
-
-async def asyncio_detailed(
-    repo_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
-    """
-
-    kwargs = _get_kwargs(
-        repo_id=repo_id,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    repo_id: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
-    """Get User Repos with Services
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_id (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
-    """
-
-    return (
-        await asyncio_detailed(
-            repo_id=repo_id,
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            account_type=account_type,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.repo_services import RepoServices
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    repo_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Dict[str, Any]:
+    url = "{}/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_id=repo_id)
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["account_type"] = account_type
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+    if response.status_code == 200:
+        response_200 = RepoServices.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    repo_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+    """Get User Repos with Services
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_id (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+    """
+
+    kwargs = _get_kwargs(
+        repo_id=repo_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    repo_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+    """Get User Repos with Services
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_id (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+    """
+
+    return sync_detailed(
+        repo_id=repo_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
+    ).parsed
+
+
+async def asyncio_detailed(
+    repo_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+    """Get User Repos with Services
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_id (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+    """
+
+    kwargs = _get_kwargs(
+        repo_id=repo_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    repo_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, RepoServices]]:
+    """Get User Repos with Services
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_id (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, RepoServices]]
+    """
+
+    return (
+        await asyncio_detailed(
+            repo_id=repo_id,
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            account_type=account_type,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/repo/get_repo_repo_repo_owner_repo_name_get.py` & `PyOblv-0.2.1/oblv/api/repo/get_repo_repo_repo_owner_repo_name_get.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.repo import Repo
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    repo_owner: str,
-    repo_name: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Dict[str, Any]:
-    url = "{}/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_owner=repo_owner, repo_name=repo_name)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["account_type"] = account_type
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
-    if response.status_code == 200:
-        response_200 = Repo.from_dict(response.json())
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    repo_owner: str,
-    repo_name: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
-    """Get User Repo
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
-    """
-
-    kwargs = _get_kwargs(
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    repo_owner: str,
-    repo_name: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
-    """Get User Repo
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
-    """
-
-    return sync_detailed(
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
-    ).parsed
-
-
-async def asyncio_detailed(
-    repo_owner: str,
-    repo_name: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
-    """Get User Repo
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
-    """
-
-    kwargs = _get_kwargs(
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        account_type=account_type,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    repo_owner: str,
-    repo_name: str,
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    account_type: Union[Unset, None, str] = "github",
-) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
-    """Get User Repo
-
-     API to fetch user's repo with services created for every repo.
-
-    Args:
-        repo_owner (str):
-        repo_name (str):
-        oblivious_user_id (str):
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, Repo]]
-    """
-
-    return (
-        await asyncio_detailed(
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            account_type=account_type,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.repo import Repo
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    repo_owner: str,
+    repo_name: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Dict[str, Any]:
+    url = "{}/repo/{repo_owner}/{repo_name}".format(client.base_url, repo_owner=repo_owner, repo_name=repo_name)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["account_type"] = account_type
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
+    if response.status_code == 200:
+        response_200 = Repo.from_dict(response.json())
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    repo_owner: str,
+    repo_name: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_owner (str):
+        repo_name (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, Repo]]
+    """
+
+    kwargs = _get_kwargs(
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    repo_owner: str,
+    repo_name: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_owner (str):
+        repo_name (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, Repo]]
+    """
+
+    return sync_detailed(
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
+    ).parsed
+
+
+async def asyncio_detailed(
+    repo_owner: str,
+    repo_name: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Response[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_owner (str):
+        repo_name (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, Repo]]
+    """
+
+    kwargs = _get_kwargs(
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        account_type=account_type,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    repo_owner: str,
+    repo_name: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    account_type: Union[Unset, None, str] = "github",
+) -> Optional[Union[HTTPValidationError, MessageModel, Repo]]:
+    """Get User Repo
+
+     API to fetch user's repo with services created for every repo.
+
+    Args:
+        repo_owner (str):
+        repo_name (str):
+        oblivious_user_id (str):
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, Repo]]
+    """
+
+    return (
+        await asyncio_detailed(
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            account_type=account_type,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/repo/search_repo_from_vcs_repo_search_get.py` & `PyOblv-0.2.1/oblv/api/user/update_user_password_user_password_put.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,184 @@
-from typing import Any, Dict, List, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.repo import Repo
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    search_string: str,
-) -> Dict[str, Any]:
-    url = "{}/repo/search".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["search_string"] = search_string
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    if response.status_code == 200:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = Repo.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
-
-        return response_200
-    if response.status_code == 204:
-        response_204 = cast(Any, None)
-        return response_204
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    search_string: str,
-) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
-
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        search_string (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        search_string=search_string,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    search_string: str,
-) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
-
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        search_string (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        search_string=search_string,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    search_string: str,
-) -> Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
-
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        search_string (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        search_string=search_string,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    search_string: str,
-) -> Optional[Union[Any, HTTPValidationError, List[Repo], MessageModel]]:
-    """Search Repo
-
-     API to search a repository in VCS, on which the user has access (via their own account, or by any
-    organization they are member of).
-
-    Args:
-        oblivious_user_id (str):
-        search_string (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            search_string=search_string,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.user_password_input import UserPasswordInput
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    json_body: UserPasswordInput,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/user/password".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    json_json_body = json_body.to_dict()
+
+    return {
+        "method": "put",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "json": json_json_body,
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = response.json()
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    json_body: UserPasswordInput,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Update User's Password
+
+     API to update user's password
+
+    Args:
+        oblivious_user_id (str):
+        json_body (UserPasswordInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    json_body: UserPasswordInput,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Update User's Password
+
+     API to update user's password
+
+    Args:
+        oblivious_user_id (str):
+        json_body (UserPasswordInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    json_body: UserPasswordInput,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Update User's Password
+
+     API to update user's password
+
+    Args:
+        oblivious_user_id (str):
+        json_body (UserPasswordInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    json_body: UserPasswordInput,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Update User's Password
+
+     API to update user's password
+
+    Args:
+        oblivious_user_id (str):
+        json_body (UserPasswordInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/service/add_repo_service_repo_service_post.py` & `PyOblv-0.2.1/oblv/api/service/delete_repo_services_repo_service_delete.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,264 +1,242 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.service_validation_response import ServiceValidationResponse
-from ...models.service_yaml_add_input import ServiceYamlAddInput
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Dict[str, Any]:
-    url = "{}/repo/service".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["ref"] = ref
-
-    params["ref_type"] = ref_type
-
-    params["account_type"] = account_type
-
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["repo_owner"] = repo_owner
-
-    params["repo_name"] = repo_name
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    json_json_body = json_body.to_dict()
-
-    return {
-        "method": "post",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "json": json_json_body,
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    if response.status_code == 200:
-        response_200 = ServiceValidationResponse.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
-
-     API to create a service after validation.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
-
-     API to create a service after validation.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    return sync_detailed(
-        client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
-
-     API to create a service after validation.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlAddInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Add Repo Service
-
-     API to create a service after validation.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlAddInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            json_body=json_body,
-            ref=ref,
-            ref_type=ref_type,
-            account_type=account_type,
-            oblivious_user_id=oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Dict[str, Any]:
+    url = "{}/repo/service".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["ref"] = ref
+
+    params["ref_type"] = ref_type
+
+    params["account_type"] = account_type
+
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["repo_owner"] = repo_owner
+
+    params["repo_name"] = repo_name
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "delete",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = MessageModel.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Delete Repo Service
+
+     API to delete a service. It does not delete the existing deployments created from this service.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Delete Repo Service
+
+     API to delete a service. It does not delete the existing deployments created from this service.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Delete Repo Service
+
+     API to delete a service. It does not delete the existing deployments created from this service.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Delete Repo Service
+
+     API to delete a service. It does not delete the existing deployments created from this service.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            ref=ref,
+            ref_type=ref_type,
+            account_type=account_type,
+            oblivious_user_id=oblivious_user_id,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/service/get_repo_services_repo_service_get.py` & `PyOblv-0.2.1/oblv/api/service/get_repo_services_repo_service_get.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-from typing import Any, Dict, List, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.repo_service_list import RepoServiceList
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Dict[str, Any]:
-    url = "{}/repo/service".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["account_type"] = account_type
-
-    params["page"] = page
-
-    params["per_page"] = per_page
-
-    params["get_all"] = get_all
-
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["repo_owner"] = repo_owner
-
-    params["repo_name"] = repo_name
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = RepoServiceList.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
-
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        account_type=account_type,
-        page=page,
-        per_page=per_page,
-        get_all=get_all,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
-
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        account_type=account_type,
-        page=page,
-        per_page=per_page,
-        get_all=get_all,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
-
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        account_type=account_type,
-        page=page,
-        per_page=per_page,
-        get_all=get_all,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    account_type: Union[Unset, None, str] = "github",
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    get_all: Union[Unset, None, bool] = False,
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get Repo Services
-
-     API to fetch all the services available for the given repository. This API is valid only for linked
-    repositories.
-
-    Args:
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        get_all (Union[Unset, None, bool]):
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            account_type=account_type,
-            page=page,
-            per_page=per_page,
-            get_all=get_all,
-            oblivious_user_id=oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-        )
-    ).parsed
+from typing import Any, Dict, List, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.repo_service_list import RepoServiceList
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    get_all: Union[Unset, None, bool] = False,
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Dict[str, Any]:
+    url = "{}/repo/service".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["account_type"] = account_type
+
+    params["page"] = page
+
+    params["per_page"] = per_page
+
+    params["get_all"] = get_all
+
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["repo_owner"] = repo_owner
+
+    params["repo_name"] = repo_name
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = RepoServiceList.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    get_all: Union[Unset, None, bool] = False,
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get Repo Services
+
+     API to fetch all the services available for the given repository. This API is valid only for linked
+    repositories.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        get_all (Union[Unset, None, bool]):
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        account_type=account_type,
+        page=page,
+        per_page=per_page,
+        get_all=get_all,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    get_all: Union[Unset, None, bool] = False,
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get Repo Services
+
+     API to fetch all the services available for the given repository. This API is valid only for linked
+    repositories.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        get_all (Union[Unset, None, bool]):
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        account_type=account_type,
+        page=page,
+        per_page=per_page,
+        get_all=get_all,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    get_all: Union[Unset, None, bool] = False,
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get Repo Services
+
+     API to fetch all the services available for the given repository. This API is valid only for linked
+    repositories.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        get_all (Union[Unset, None, bool]):
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        account_type=account_type,
+        page=page,
+        per_page=per_page,
+        get_all=get_all,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    account_type: Union[Unset, None, str] = "github",
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    get_all: Union[Unset, None, bool] = False,
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get Repo Services
+
+     API to fetch all the services available for the given repository. This API is valid only for linked
+    repositories.
+
+    Args:
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        get_all (Union[Unset, None, bool]):
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, RepoServiceList, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            account_type=account_type,
+            page=page,
+            per_page=per_page,
+            get_all=get_all,
+            oblivious_user_id=oblivious_user_id,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/service/get_user_services_service_get.py` & `PyOblv-0.2.1/oblv/api/service/get_user_services_service_get.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-from typing import Any, Dict, List, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.user_service_list import UserServiceList
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-    get_all: Union[Unset, None, bool] = False,
-) -> Dict[str, Any]:
-    url = "{}/service".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["page"] = page
-
-    params["per_page"] = per_page
-
-    params["search_term"] = search_term
-
-    params["get_all"] = get_all
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = UserServiceList.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-    get_all: Union[Unset, None, bool] = False,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get User Services
-
-     API to fetch user's services
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-        get_all (Union[Unset, None, bool]):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-        get_all=get_all,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-    get_all: Union[Unset, None, bool] = False,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get User Services
-
-     API to fetch user's services
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-        get_all (Union[Unset, None, bool]):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-        get_all=get_all,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-    get_all: Union[Unset, None, bool] = False,
-) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get User Services
-
-     API to fetch user's services
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-        get_all (Union[Unset, None, bool]):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        page=page,
-        per_page=per_page,
-        search_term=search_term,
-        get_all=get_all,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    page: Union[Unset, None, int] = 1,
-    per_page: Union[Unset, None, int] = 10,
-    search_term: Union[Unset, None, str] = "",
-    get_all: Union[Unset, None, bool] = False,
-) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    """Get User Services
-
-     API to fetch user's services
-
-    Args:
-        oblivious_user_id (str):
-        page (Union[Unset, None, int]):  Default: 1.
-        per_page (Union[Unset, None, int]):  Default: 10.
-        search_term (Union[Unset, None, str]):  Default: ''.
-        get_all (Union[Unset, None, bool]):
-
-    Returns:
-        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            page=page,
-            per_page=per_page,
-            search_term=search_term,
-            get_all=get_all,
-        )
-    ).parsed
+from typing import Any, Dict, List, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.user_service_list import UserServiceList
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+    get_all: Union[Unset, None, bool] = False,
+) -> Dict[str, Any]:
+    url = "{}/service".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["page"] = page
+
+    params["per_page"] = per_page
+
+    params["search_term"] = search_term
+
+    params["get_all"] = get_all
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = UserServiceList.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+    get_all: Union[Unset, None, bool] = False,
+) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get User Services
+
+     API to fetch user's services
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+        get_all (Union[Unset, None, bool]):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+        get_all=get_all,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+    get_all: Union[Unset, None, bool] = False,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get User Services
+
+     API to fetch user's services
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+        get_all (Union[Unset, None, bool]):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+        get_all=get_all,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+    get_all: Union[Unset, None, bool] = False,
+) -> Response[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get User Services
+
+     API to fetch user's services
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+        get_all (Union[Unset, None, bool]):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        page=page,
+        per_page=per_page,
+        search_term=search_term,
+        get_all=get_all,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    page: Union[Unset, None, int] = 1,
+    per_page: Union[Unset, None, int] = 10,
+    search_term: Union[Unset, None, str] = "",
+    get_all: Union[Unset, None, bool] = False,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    """Get User Services
+
+     API to fetch user's services
+
+    Args:
+        oblivious_user_id (str):
+        page (Union[Unset, None, int]):  Default: 1.
+        per_page (Union[Unset, None, int]):  Default: 10.
+        search_term (Union[Unset, None, str]):  Default: ''.
+        get_all (Union[Unset, None, bool]):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, UserServiceList, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            page=page,
+            per_page=per_page,
+            search_term=search_term,
+            get_all=get_all,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/service/update_repo_service_repo_service_put.py` & `PyOblv-0.2.1/oblv/api/service/validate_repo_service_repo_service_validate_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,267 +1,263 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.service_validation_response import ServiceValidationResponse
-from ...models.service_yaml_update_input import ServiceYamlUpdateInput
-from ...types import UNSET, Response, Unset
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Dict[str, Any]:
-    url = "{}/repo/service".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["ref"] = ref
-
-    params["ref_type"] = ref_type
-
-    params["account_type"] = account_type
-
-    params["oblivious_user_id"] = oblivious_user_id
-    params["repo_owner"] = repo_owner
-
-    params["repo_name"] = repo_name
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    json_json_body = json_body.to_dict()
-
-    return {
-        "method": "put",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "json": json_json_body,
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    if response.status_code == 200:
-        response_200 = ServiceValidationResponse.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
-
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
-
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    return sync_detailed(
-        client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
-
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        ref=ref,
-        ref_type=ref_type,
-        account_type=account_type,
-        oblivious_user_id=oblivious_user_id,
-        repo_owner=repo_owner,
-        repo_name=repo_name,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    json_body: ServiceYamlUpdateInput,
-    ref: str,
-    ref_type: Union[Unset, None, str] = "branch",
-    account_type: Union[Unset, None, str] = "github",
-    oblivious_user_id: str,
-    repo_owner: str,
-    repo_name: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
-    """Update Repo Service
-
-     API to update a service. It fetches the current service.yaml file from VCS and validate it. It works
-    in a similar way as **Validate Repo Service** API.
-
-    Args:
-        ref (str):
-        ref_type (Union[Unset, None, str]):  Default: 'branch'.
-        account_type (Union[Unset, None, str]):  Default: 'github'.
-        oblivious_user_id (str):
-        repo_owner (str):
-        repo_name (str):
-        json_body (ServiceYamlUpdateInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            json_body=json_body,
-            ref=ref,
-            ref_type=ref_type,
-            account_type=account_type,
-            oblivious_user_id=oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.service_validation_response import ServiceValidationResponse
+from ...types import UNSET, Response, Unset
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Dict[str, Any]:
+    url = "{}/repo/service/validate".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["ref"] = ref
+
+    params["ref_type"] = ref_type
+
+    params["account_type"] = account_type
+
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["repo_owner"] = repo_owner
+
+    params["repo_name"] = repo_name
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+    if response.status_code == 200:
+        response_200 = ServiceValidationResponse.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+    """Validate Repo Service
+
+     API to validate a service with supported service schema. The checks include
+
+    - Presence of service.yaml in ./oblivious folder.
+    - Presence of Dockerfile in ./oblivious folder.
+    - Content of service.yaml must be valid with respect to supported service schema.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+    """Validate Repo Service
+
+     API to validate a service with supported service schema. The checks include
+
+    - Presence of service.yaml in ./oblivious folder.
+    - Presence of Dockerfile in ./oblivious folder.
+    - Content of service.yaml must be valid with respect to supported service schema.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+    """
+
+    return sync_detailed(
+        client=client,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+    """Validate Repo Service
+
+     API to validate a service with supported service schema. The checks include
+
+    - Presence of service.yaml in ./oblivious folder.
+    - Presence of Dockerfile in ./oblivious folder.
+    - Content of service.yaml must be valid with respect to supported service schema.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        ref=ref,
+        ref_type=ref_type,
+        account_type=account_type,
+        oblivious_user_id=oblivious_user_id,
+        repo_owner=repo_owner,
+        repo_name=repo_name,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    ref: str,
+    ref_type: Union[Unset, None, str] = "branch",
+    account_type: Union[Unset, None, str] = "github",
+    oblivious_user_id: str,
+    repo_owner: str,
+    repo_name: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]:
+    """Validate Repo Service
+
+     API to validate a service with supported service schema. The checks include
+
+    - Presence of service.yaml in ./oblivious folder.
+    - Presence of Dockerfile in ./oblivious folder.
+    - Content of service.yaml must be valid with respect to supported service schema.
+
+    Args:
+        ref (str):
+        ref_type (Union[Unset, None, str]):  Default: 'branch'.
+        account_type (Union[Unset, None, str]):  Default: 'github'.
+        oblivious_user_id (str):
+        repo_owner (str):
+        repo_name (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, ServiceValidationResponse]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            ref=ref,
+            ref_type=ref_type,
+            account_type=account_type,
+            oblivious_user_id=oblivious_user_id,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/user/add_user_public_shared_key_user_psk_put.py` & `PyOblv-0.2.1/oblv/api/user/get_user_profile_view_user_profile_get.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,184 +1,172 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.psk import PSK
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    json_body: PSK,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/user/psk".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    json_json_body = json_body.to_dict()
-
-    return {
-        "method": "put",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "json": json_json_body,
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, PSK]]:
-    if response.status_code == 200:
-        response_200 = response.json()
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: PSK,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
-
-     API to update user's psk
-
-    Args:
-        oblivious_user_id (str):
-        json_body (PSK):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    json_body: PSK,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
-
-     API to update user's psk
-
-    Args:
-        oblivious_user_id (str):
-        json_body (PSK):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
-    """
-
-    return sync_detailed(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: PSK,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
-
-     API to update user's psk
-
-    Args:
-        oblivious_user_id (str):
-        json_body (PSK):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    json_body: PSK,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, PSK]]:
-    """Update User PSK
-
-     API to update user's psk
-
-    Args:
-        oblivious_user_id (str):
-        json_body (PSK):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, PSK]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            json_body=json_body,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.user_profile_response import UserProfileResponse
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/user/profile".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, UserProfileResponse]]:
+    if response.status_code == 200:
+        response_200 = UserProfileResponse.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
+
+     API to fetch user's profile details
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
+
+     API to fetch user's profile details
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
+
+     API to fetch user's profile details
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
+    """Get User Profile
+
+     API to fetch user's profile details
+
+    Args:
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/user/get_user_deployment_credit_usage_user_credit_usage_get.py` & `PyOblv-0.2.1/oblv/api/user/update_user_name_user_name_put.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,172 +1,184 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.user_credit_utilization import UserCreditUtilization
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/user/credit_usage".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, UserCreditUtilization]]:
-    if response.status_code == 200:
-        response_200 = UserCreditUtilization.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
-    """Get User Credit Usage
-
-     API to fetch user's credit usage
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
-    """Get User Credit Usage
-
-     API to fetch user's credit usage
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
-    """Get User Credit Usage
-
-     API to fetch user's credit usage
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]:
-    """Get User Credit Usage
-
-     API to fetch user's credit usage
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserCreditUtilization]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.name_input import NameInput
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    json_body: NameInput,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/user/name".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    json_json_body = json_body.to_dict()
+
+    return {
+        "method": "put",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "json": json_json_body,
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
+    if response.status_code == 200:
+        response_200 = MessageModel.from_dict(response.json())
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    json_body: NameInput,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Update Name
+
+     API to update the name.
+
+    Args:
+        oblivious_user_id (str):
+        json_body (NameInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    json_body: NameInput,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Update Name
+
+     API to update the name.
+
+    Args:
+        oblivious_user_id (str):
+        json_body (NameInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    json_body: NameInput,
+    oblivious_user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel]]:
+    """Update Name
+
+     API to update the name.
+
+    Args:
+        oblivious_user_id (str):
+        json_body (NameInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        json_body=json_body,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    json_body: NameInput,
+    oblivious_user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel]]:
+    """Update Name
+
+     API to update the name.
+
+    Args:
+        oblivious_user_id (str):
+        json_body (NameInput):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/user/get_user_profile_view_user_profile_get.py` & `PyOblv-0.2.1/oblv/api/user/get_user_public_shared_key_user_psk_get.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,181 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.user_profile_response import UserProfileResponse
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/user/profile".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[Any, HTTPValidationError, MessageModel, UserProfileResponse]]:
-    if response.status_code == 200:
-        response_200 = UserProfileResponse.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
-    """Get User Profile
-
-     API to fetch user's profile details
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
-    """Get User Profile
-
-     API to fetch user's profile details
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
-    """Get User Profile
-
-     API to fetch user's profile details
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, UserProfileResponse]]:
-    """Get User Profile
-
-     API to fetch user's profile details
-
-    Args:
-        oblivious_user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, UserProfileResponse]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/user/psk".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["user_id"] = user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    if response.status_code == 200:
+        response_200 = cast(str, response.json())
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Get User PSK
+
+     API to fetch user's psk
+
+    Args:
+        oblivious_user_id (str):
+        user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        user_id=user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Get User PSK
+
+     API to fetch user's psk
+
+    Args:
+        oblivious_user_id (str):
+        user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        user_id=user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    user_id: str,
+) -> Response[Union[HTTPValidationError, MessageModel, str]]:
+    """Get User PSK
+
+     API to fetch user's psk
+
+    Args:
+        oblivious_user_id (str):
+        user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        user_id=user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    user_id: str,
+) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
+    """Get User PSK
+
+     API to fetch user's psk
+
+    Args:
+        oblivious_user_id (str):
+        user_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, MessageModel, str]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            user_id=user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/user/get_user_public_shared_key_user_psk_get.py` & `PyOblv-0.2.1/oblv/api/deployment/get_deployment_roles_deployment_roles_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,196 @@
-from typing import Any, Dict, Optional, Union, cast
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/user/psk".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params["user_id"] = user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
-    if response.status_code == 200:
-        response_200 = cast(str, response.json())
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Get User PSK
-
-     API to fetch user's psk
-
-    Args:
-        oblivious_user_id (str):
-        user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        user_id=user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Get User PSK
-
-     API to fetch user's psk
-
-    Args:
-        oblivious_user_id (str):
-        user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    return sync_detailed(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        user_id=user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel, str]]:
-    """Get User PSK
-
-     API to fetch user's psk
-
-    Args:
-        oblivious_user_id (str):
-        user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        oblivious_user_id=oblivious_user_id,
-        user_id=user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    oblivious_user_id: str,
-    user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel, str]]:
-    """Get User PSK
-
-     API to fetch user's psk
-
-    Args:
-        oblivious_user_id (str):
-        user_id (str):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel, str]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            oblivious_user_id=oblivious_user_id,
-            user_id=user_id,
-        )
-    ).parsed
+from typing import Any, Dict, List, Optional, Union
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...models.role_response import RoleResponse
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Dict[str, Any]:
+    url = "{}/deployment/roles".format(client.base_url)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params["deployment_id"] = deployment_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+    if response.status_code == 200:
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = RoleResponse.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
+
+        return response_200
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 501:
+        response_501 = MessageModel.from_dict(response.json())
+
+        return response_501
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+    """Get Deployment Roles
+
+     API to get a deployment's roles.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+    """Get Deployment Roles
+
+     API to get a deployment's roles.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+    """
+
+    return sync_detailed(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+    """Get Deployment Roles
+
+     API to get a deployment's roles.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+    """
+
+    kwargs = _get_kwargs(
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+        deployment_id=deployment_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+    deployment_id: str,
+) -> Optional[Union[HTTPValidationError, List[RoleResponse], MessageModel]]:
+    """Get Deployment Roles
+
+     API to get a deployment's roles.
+
+    Args:
+        oblivious_user_id (str):
+        deployment_id (str):
+
+    Returns:
+        Response[Union[HTTPValidationError, List[RoleResponse], MessageModel]]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+            deployment_id=deployment_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/api/user/update_user_name_user_name_put.py` & `PyOblv-0.2.1/oblv/api/notification/get_notification_details_notification_notification_id_get.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,184 +1,174 @@
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ...client import AuthenticatedClient
-from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from ...models.http_validation_error import HTTPValidationError
-from ...models.message_model import MessageModel
-from ...models.name_input import NameInput
-from ...types import UNSET, Response
-
-
-def _get_kwargs(
-    *,
-    client: AuthenticatedClient,
-    json_body: NameInput,
-    oblivious_user_id: str,
-) -> Dict[str, Any]:
-    url = "{}/user/name".format(client.base_url)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    params: Dict[str, Any] = {}
-    params["oblivious_user_id"] = oblivious_user_id
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
-    json_json_body = json_body.to_dict()
-
-    return {
-        "method": "put",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "json": json_json_body,
-        "params": params,
-    }
-
-
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel]]:
-    if response.status_code == 200:
-        response_200 = MessageModel.from_dict(response.json())
-
-        return response_200
-    if response.status_code == 400:
-        response_400_message = response.json()["message"]
-        raise BadRequestError(message=response_400_message)
-    if response.status_code == 500:
-        response_500_request_id = response.headers["apigw-requestid"]
-        raise HTTPClientError(request_id=response_500_request_id)
-    if response.status_code == 422:
-        response_422 = HTTPValidationError.from_dict(response.json())
-        if response_422.detail[0].type.__contains__("regex"):
-            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
-        raise ParamValidationError(report=report)
-    if response.status_code == 403:
-        raise UnauthorizedTokenError()
-    return None
-
-
-def _build_response(*, response: httpx.Response) -> Response[Union[HTTPValidationError, MessageModel]]:
-    return Response(
-        status_code=response.status_code,
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: NameInput,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Update Name
-
-     API to update the name.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (NameInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(response=response)
-
-
-def sync(
-    *,
-    client: AuthenticatedClient,
-    json_body: NameInput,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Update Name
-
-     API to update the name.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (NameInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    return sync_detailed(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: AuthenticatedClient,
-    json_body: NameInput,
-    oblivious_user_id: str,
-) -> Response[Union[HTTPValidationError, MessageModel]]:
-    """Update Name
-
-     API to update the name.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (NameInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    kwargs = _get_kwargs(
-        client=client,
-        json_body=json_body,
-        oblivious_user_id=oblivious_user_id,
-    )
-
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
-
-    return _build_response(response=response)
-
-
-async def asyncio(
-    *,
-    client: AuthenticatedClient,
-    json_body: NameInput,
-    oblivious_user_id: str,
-) -> Optional[Union[HTTPValidationError, MessageModel]]:
-    """Update Name
-
-     API to update the name.
-
-    Args:
-        oblivious_user_id (str):
-        json_body (NameInput):
-
-    Returns:
-        Response[Union[HTTPValidationError, MessageModel]]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            json_body=json_body,
-            oblivious_user_id=oblivious_user_id,
-        )
-    ).parsed
+from typing import Any, Dict, Optional, Union, cast
+
+import httpx
+
+from ...client import AuthenticatedClient
+from ...exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from ...models.http_validation_error import HTTPValidationError
+from ...models.message_model import MessageModel
+from ...types import UNSET, Response
+
+
+def _get_kwargs(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Dict[str, Any]:
+    url = "{}/notification/{notification_id}".format(client.base_url, notification_id=notification_id)
+
+    headers: Dict[str, str] = client.get_headers()
+    cookies: Dict[str, Any] = client.get_cookies()
+
+    params: Dict[str, Any] = {}
+    params["oblivious_user_id"] = oblivious_user_id
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
+    return {
+        "method": "get",
+        "url": url,
+        "headers": headers,
+        "cookies": cookies,
+        "timeout": client.get_timeout(),
+        "params": params,
+    }
+
+
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    if response.status_code == 200:
+        response_200 = cast(str, response.json())
+        return response_200
+    if response.status_code == 204:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == 400:
+        response_400_message = response.json()["message"]
+        raise BadRequestError(message=response_400_message)
+    if response.status_code == 500:
+        response_500_request_id = response.headers["apigw-requestid"]
+        raise HTTPClientError(request_id=response_500_request_id)
+    if response.status_code == 422:
+        response_422 = HTTPValidationError.from_dict(response.json())
+        if response_422.detail[0].type.__contains__("regex"):
+            report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        report = "Invalid " + response_422.detail[0].loc[-1] + " provided"
+        raise ParamValidationError(report=report)
+    if response.status_code == 403:
+        raise UnauthorizedTokenError()
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
+    return Response(
+        status_code=response.status_code,
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(response=response),
+    )
+
+
+def sync_detailed(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        notification_id=notification_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    response = httpx.request(
+        verify=client.verify_ssl,
+        **kwargs,
+    )
+
+    return _build_response(response=response)
+
+
+def sync(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+    """
+
+    return sync_detailed(
+        notification_id=notification_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    ).parsed
+
+
+async def asyncio_detailed(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Response[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+    """
+
+    kwargs = _get_kwargs(
+        notification_id=notification_id,
+        client=client,
+        oblivious_user_id=oblivious_user_id,
+    )
+
+    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+        response = await _client.request(**kwargs)
+
+    return _build_response(response=response)
+
+
+async def asyncio(
+    notification_id: str,
+    *,
+    client: AuthenticatedClient,
+    oblivious_user_id: str,
+) -> Optional[Union[Any, HTTPValidationError, MessageModel, str]]:
+    """Get Notification Details
+
+    Args:
+        notification_id (str):
+        oblivious_user_id (str):
+
+    Returns:
+        Response[Union[Any, HTTPValidationError, MessageModel, str]]
+    """
+
+    return (
+        await asyncio_detailed(
+            notification_id=notification_id,
+            client=client,
+            oblivious_user_id=oblivious_user_id,
+        )
+    ).parsed
```

### Comparing `PyOblv-0.2.0/oblv/client.py` & `PyOblv-0.2.1/oblv/client.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import ssl
-from typing import Dict, Union
-
-import attr
-
-from .config import URL
-
-
-@attr.s(auto_attribs=True, repr=False)
-class Client:
-    """A class for keeping track of data related to the API"""
-        
-    cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
-    headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
-    timeout: float = attr.ib(20.0, kw_only=True)
-    verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
-    
-    @property
-    def base_url(self):
-        return URL
-
-    def get_headers(self) -> Dict[str, str]:
-        """Get headers to be used in all endpoints"""
-        return {**self.headers}
-
-    def with_headers(self, headers: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional headers"""
-        return attr.evolve(self, headers={**self.headers, **headers})
-
-    def get_cookies(self) -> Dict[str, str]:
-        return {**self.cookies}
-
-    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional cookies"""
-        return attr.evolve(self, cookies={**self.cookies, **cookies})
-
-    def get_timeout(self) -> float:
-        return self.timeout
-
-    def with_timeout(self, timeout: float) -> "Client":
-        """Get a new client matching this one with a new timeout (in seconds)"""
-        return attr.evolve(self, timeout=timeout)
-
-
-@attr.s(auto_attribs=True, repr=False)
-class AuthenticatedClient(Client):
-    """A Client which has been authenticated for use on secured endpoints"""
-
-    def __init__(self):
-        super()
-    token: str
-
-    oblivious_user_id: str
-
-    def get_headers(self) -> Dict[str, str]:
-        """Get headers to be used in authenticated endpoints"""
-        return {"AuthorizationToken": f"{self.token}", **self.headers}
+import ssl
+from typing import Dict, Union
+
+import attr
+
+from .config import URL
+
+
+@attr.s(auto_attribs=True, repr=False)
+class Client:
+    """A class for keeping track of data related to the API"""
+        
+    cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
+    headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
+    timeout: float = attr.ib(20.0, kw_only=True)
+    verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
+    
+    @property
+    def base_url(self):
+        return URL
+
+    def get_headers(self) -> Dict[str, str]:
+        """Get headers to be used in all endpoints"""
+        return {**self.headers}
+
+    def with_headers(self, headers: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional headers"""
+        return attr.evolve(self, headers={**self.headers, **headers})
+
+    def get_cookies(self) -> Dict[str, str]:
+        return {**self.cookies}
+
+    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional cookies"""
+        return attr.evolve(self, cookies={**self.cookies, **cookies})
+
+    def get_timeout(self) -> float:
+        return self.timeout
+
+    def with_timeout(self, timeout: float) -> "Client":
+        """Get a new client matching this one with a new timeout (in seconds)"""
+        return attr.evolve(self, timeout=timeout)
+
+
+@attr.s(auto_attribs=True, repr=False)
+class AuthenticatedClient(Client):
+    """A Client which has been authenticated for use on secured endpoints"""
+
+    def __init__(self):
+        super()
+    token: str
+
+    oblivious_user_id: str
+
+    def get_headers(self) -> Dict[str, str]:
+        """Get headers to be used in authenticated endpoints"""
+        return {"AuthorizationToken": f"{self.token}", **self.headers}
```

### Comparing `PyOblv-0.2.0/oblv/exceptions.py` & `PyOblv-0.2.1/oblv/exceptions.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-
-def _exception_from_packed_args(exception_cls, args=None, kwargs=None):
-    # This is helpful for reducing Exceptions that only accept kwargs as
-    # only positional arguments can be provided for __reduce__
-    # Ideally, this would also be a class method on the OblvError
-    # but instance methods cannot be pickled.
-    if args is None:
-        args = ()
-    if kwargs is None:
-        kwargs = {}
-    return exception_cls(*args, **kwargs)
-
-
-class OblvError(Exception):
-    """
-    The base exception class for Oblivious exceptions.
-
-    :ivar msg: The descriptive message associated with the error.
-    """
-
-    fmt = 'An unspecified error occurred'
-
-    def __init__(self, **kwargs):
-        msg = self.fmt.format(**kwargs)
-        Exception.__init__(self, msg)
-        self.kwargs = kwargs
-
-    def __reduce__(self):
-        return _exception_from_packed_args, (self.__class__, None, self.kwargs)
-
-
-class HTTPClientError(OblvError):
-    fmt = 'An HTTP Client raised an unhandled exception. Kindly raise a request to the support team, along with the {request_id} for resolution.'
-
-    def __init__(self,request_id=""):
-        super().__init__(request_id=request_id)
-
-    # def __init__(self, request=None, response=None, **kwargs):
-    #     self.request = request
-    #     self.response = response
-    #     super().__init__(**kwargs)
-
-    # def __reduce__(self):
-    #     return _exception_from_packed_args, (
-    #         self.__class__,
-    #         (self.request, self.response),
-    #         self.kwargs,
-    #     )
-
-
-class ConnectionError(OblvError):
-    fmt = 'An HTTP Client failed to establish a connection: {error}'
-
-class MissingParametersError(OblvError):
-    """
-    One or more required parameters were not supplied.
-
-    :ivar object: The object that has missing parameters.
-        This can be an operation or a parameter (in the
-        case of inner params).  The str() of this object
-        will be used so it doesn't need to implement anything
-        other than str().
-    :ivar missing: The names of the missing parameters.
-    """
-
-    fmt = (
-        'The following required parameters are missing for '
-        '{object_name}: {missing}'
-    )
-    
-    
-    def __init__(self,object_name="",missing=""):
-        super().__init__(object_name=object_name,missing=missing)
-
-
-class ValidationError(OblvError):
-    """
-    An exception occurred validating parameters.
-
-    Subclasses must accept a ``value`` and ``param``
-    argument in their ``__init__``.
-
-    :ivar value: The value that was being validated.
-    :ivar param: The parameter that failed validation.
-    :ivar type_name: The name of the underlying type.
-    """
-
-    fmt = "Invalid value ('{value}') for param {param} " "of type {type_name} "
-    
-    def __init__(self,value="",param="",type_name=""):
-        super().__init__(value=value,param=param,type_name=type_name)
-
-
-class ParamValidationError(OblvError):
-    fmt = '{report}'
-
-class MissingServiceIdError(OblvError):
-    fmt = (
-        "The model being used for the service {service_name} is missing the "
-        "serviceId metadata property, which is required."
-    )
-
-    def __init__(self, service_name):
-        super().__init__(service_name=service_name)
-class UnauthorizedTokenError(OblvError):
-    fmt = (
-        "The session associated with this profile has expired or is "
-        "otherwise invalid. To refresh this session use the authenticate method "
-        "with the corresponding profile."
-    )
-
-class BadRequestError(OblvError):
-    fmt = '{message}'
-    
-    def __init__(self,message=""):
-        super().__init__(message=message)
-    
-class AuthenticationError(OblvError):
-    fmt = 'Invalid credentials provided. Kindly verify the same and try again.'
-
-
-class BadYamlData(OblvError):
-    fmt = 'Validation failed for service yaml data with message - {message}'
-    
-    
-    def __init__(self,message=""):
-        super().__init__(message=message)
+
+def _exception_from_packed_args(exception_cls, args=None, kwargs=None):
+    # This is helpful for reducing Exceptions that only accept kwargs as
+    # only positional arguments can be provided for __reduce__
+    # Ideally, this would also be a class method on the OblvError
+    # but instance methods cannot be pickled.
+    if args is None:
+        args = ()
+    if kwargs is None:
+        kwargs = {}
+    return exception_cls(*args, **kwargs)
+
+
+class OblvError(Exception):
+    """
+    The base exception class for Oblivious exceptions.
+
+    :ivar msg: The descriptive message associated with the error.
+    """
+
+    fmt = 'An unspecified error occurred'
+
+    def __init__(self, **kwargs):
+        msg = self.fmt.format(**kwargs)
+        Exception.__init__(self, msg)
+        self.kwargs = kwargs
+
+    def __reduce__(self):
+        return _exception_from_packed_args, (self.__class__, None, self.kwargs)
+
+
+class HTTPClientError(OblvError):
+    fmt = 'An HTTP Client raised an unhandled exception. Kindly raise a request to the support team, along with the {request_id} for resolution.'
+
+    def __init__(self,request_id=""):
+        super().__init__(request_id=request_id)
+
+    # def __init__(self, request=None, response=None, **kwargs):
+    #     self.request = request
+    #     self.response = response
+    #     super().__init__(**kwargs)
+
+    # def __reduce__(self):
+    #     return _exception_from_packed_args, (
+    #         self.__class__,
+    #         (self.request, self.response),
+    #         self.kwargs,
+    #     )
+
+
+class ConnectionError(OblvError):
+    fmt = 'An HTTP Client failed to establish a connection: {error}'
+
+class MissingParametersError(OblvError):
+    """
+    One or more required parameters were not supplied.
+
+    :ivar object: The object that has missing parameters.
+        This can be an operation or a parameter (in the
+        case of inner params).  The str() of this object
+        will be used so it doesn't need to implement anything
+        other than str().
+    :ivar missing: The names of the missing parameters.
+    """
+
+    fmt = (
+        'The following required parameters are missing for '
+        '{object_name}: {missing}'
+    )
+    
+    
+    def __init__(self,object_name="",missing=""):
+        super().__init__(object_name=object_name,missing=missing)
+
+
+class ValidationError(OblvError):
+    """
+    An exception occurred validating parameters.
+
+    Subclasses must accept a ``value`` and ``param``
+    argument in their ``__init__``.
+
+    :ivar value: The value that was being validated.
+    :ivar param: The parameter that failed validation.
+    :ivar type_name: The name of the underlying type.
+    """
+
+    fmt = "Invalid value ('{value}') for param {param} " "of type {type_name} "
+    
+    def __init__(self,value="",param="",type_name=""):
+        super().__init__(value=value,param=param,type_name=type_name)
+
+
+class ParamValidationError(OblvError):
+    fmt = '{report}'
+
+class MissingServiceIdError(OblvError):
+    fmt = (
+        "The model being used for the service {service_name} is missing the "
+        "serviceId metadata property, which is required."
+    )
+
+    def __init__(self, service_name):
+        super().__init__(service_name=service_name)
+class UnauthorizedTokenError(OblvError):
+    fmt = (
+        "The session associated with this profile has expired or is "
+        "otherwise invalid. To refresh this session use the authenticate method "
+        "with the corresponding profile."
+    )
+
+class BadRequestError(OblvError):
+    fmt = '{message}'
+    
+    def __init__(self,message=""):
+        super().__init__(message=message)
+    
+class AuthenticationError(OblvError):
+    fmt = 'Invalid credentials provided. Kindly verify the same and try again.'
+
+
+class BadYamlData(OblvError):
+    fmt = 'Validation failed for service yaml data with message - {message}'
+    
+    
+    def __init__(self,message=""):
+        super().__init__(message=message)
```

### Comparing `PyOblv-0.2.0/oblv/models/__init__.py` & `PyOblv-0.2.1/oblv/models/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-""" Contains all the data models used in inputs/outputs """
-
-from .access_history import AccessHistory
-from .account import Account
-from .api_key import APIKey
-from .build_args_schema import BuildArgsSchema
-from .create_deployment_input import CreateDeploymentInput
-from .create_deployment_response import CreateDeploymentResponse
-from .deployment_complete import DeploymentComplete
-from .deployment_response import DeploymentResponse
-from .http_validation_error import HTTPValidationError
-from .instance import Instance
-from .message_model import MessageModel
-from .name_input import NameInput
-from .notification_response import NotificationResponse
-from .oblv_auth_response import OblvAuthResponse
-from .psk import PSK
-from .ref_response import RefResponse
-from .repo import Repo
-from .repo_all_response import RepoAllResponse
-from .repo_services import RepoServices
-from .role_response import RoleResponse
-from .service_content_response import ServiceContentResponse
-from .service_validation_response import ServiceValidationResponse
-from .service_yaml_add_input import ServiceYamlAddInput
-from .service_yaml_update_input import ServiceYamlUpdateInput
-from .shared_users import SharedUsers
-from .user_credit_utilization import UserCreditUtilization
-from .user_password_input import UserPasswordInput
-from .user_profile_response import UserProfileResponse
-from .user_services import UserServices
-from .validated_service import ValidatedService
-from .validation_error import ValidationError
-from .vcs_repo_response import VCSRepoResponse
+""" Contains all the data models used in inputs/outputs """
+
+from .access_history import AccessHistory
+from .account import Account
+from .api_key import APIKey
+from .build_args_schema import BuildArgsSchema
+from .create_deployment_input import CreateDeploymentInput
+from .create_deployment_response import CreateDeploymentResponse
+from .deployment_complete import DeploymentComplete
+from .deployment_response import DeploymentResponse
+from .http_validation_error import HTTPValidationError
+from .instance import Instance
+from .message_model import MessageModel
+from .name_input import NameInput
+from .notification_response import NotificationResponse
+from .oblv_auth_response import OblvAuthResponse
+from .psk import PSK
+from .ref_response import RefResponse
+from .repo import Repo
+from .repo_all_response import RepoAllResponse
+from .repo_services import RepoServices
+from .role_response import RoleResponse
+from .service_content_response import ServiceContentResponse
+from .service_validation_response import ServiceValidationResponse
+from .service_yaml_add_input import ServiceYamlAddInput
+from .service_yaml_update_input import ServiceYamlUpdateInput
+from .shared_users import SharedUsers
+from .user_credit_utilization import UserCreditUtilization
+from .user_password_input import UserPasswordInput
+from .user_profile_response import UserProfileResponse
+from .user_services import UserServices
+from .validated_service import ValidatedService
+from .validation_error import ValidationError
+from .vcs_repo_response import VCSRepoResponse
```

### Comparing `PyOblv-0.2.0/oblv/models/access_history.py` & `PyOblv-0.2.1/oblv/models/access_history.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="AccessHistory")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class AccessHistory:
-    """
-    Attributes:
-        action (Union[Unset, str]):  Default: ''.
-        timestamp (Union[Unset, str]):  Default: ''.
-        oblivious_user_id (Union[Unset, str]):  Default: ''.
-        role (Union[Unset, str]):
-    """
-
-    action: Union[Unset, str] = ""
-    timestamp: Union[Unset, str] = ""
-    oblivious_user_id: Union[Unset, str] = ""
-    role: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        action = self.action
-        timestamp = self.timestamp
-        oblivious_user_id = self.oblivious_user_id
-        role = self.role
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if action is not UNSET:
-            field_dict["action"] = action
-        if timestamp is not UNSET:
-            field_dict["timestamp"] = timestamp
-        if oblivious_user_id is not UNSET:
-            field_dict["oblivious_user_id"] = oblivious_user_id
-        if role is not UNSET:
-            field_dict["role"] = role
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        action = d.pop("action", UNSET)
-
-        timestamp = d.pop("timestamp", UNSET)
-
-        oblivious_user_id = d.pop("oblivious_user_id", UNSET)
-
-        role = d.pop("role", UNSET)
-
-        access_history = cls(
-            action=action,
-            timestamp=timestamp,
-            oblivious_user_id=oblivious_user_id,
-            role=role,
-        )
-
-        access_history.additional_properties = d
-        return access_history
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="AccessHistory")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class AccessHistory:
+    """
+    Attributes:
+        action (Union[Unset, str]):  Default: ''.
+        timestamp (Union[Unset, str]):  Default: ''.
+        oblivious_user_id (Union[Unset, str]):  Default: ''.
+        role (Union[Unset, str]):
+    """
+
+    action: Union[Unset, str] = ""
+    timestamp: Union[Unset, str] = ""
+    oblivious_user_id: Union[Unset, str] = ""
+    role: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        action = self.action
+        timestamp = self.timestamp
+        oblivious_user_id = self.oblivious_user_id
+        role = self.role
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if action is not UNSET:
+            field_dict["action"] = action
+        if timestamp is not UNSET:
+            field_dict["timestamp"] = timestamp
+        if oblivious_user_id is not UNSET:
+            field_dict["oblivious_user_id"] = oblivious_user_id
+        if role is not UNSET:
+            field_dict["role"] = role
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        action = d.pop("action", UNSET)
+
+        timestamp = d.pop("timestamp", UNSET)
+
+        oblivious_user_id = d.pop("oblivious_user_id", UNSET)
+
+        role = d.pop("role", UNSET)
+
+        access_history = cls(
+            action=action,
+            timestamp=timestamp,
+            oblivious_user_id=oblivious_user_id,
+            role=role,
+        )
+
+        access_history.additional_properties = d
+        return access_history
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/account.py` & `PyOblv-0.2.1/oblv/models/account.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="Account")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class Account:
-    """
-    Attributes:
-        user_id (Union[Unset, str]):  Default: ''.
-        user_login (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: 'github'.
-    """
-
-    user_id: Union[Unset, str] = ""
-    user_login: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = "github"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        user_id = self.user_id
-        user_login = self.user_login
-        account_type = self.account_type
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if user_id is not UNSET:
-            field_dict["user_id"] = user_id
-        if user_login is not UNSET:
-            field_dict["user_login"] = user_login
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        user_id = d.pop("user_id", UNSET)
-
-        user_login = d.pop("user_login", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
-        account = cls(
-            user_id=user_id,
-            user_login=user_login,
-            account_type=account_type,
-        )
-
-        account.additional_properties = d
-        return account
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="Account")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class Account:
+    """
+    Attributes:
+        user_id (Union[Unset, str]):  Default: ''.
+        user_login (Union[Unset, str]):  Default: ''.
+        account_type (Union[Unset, str]):  Default: 'github'.
+    """
+
+    user_id: Union[Unset, str] = ""
+    user_login: Union[Unset, str] = ""
+    account_type: Union[Unset, str] = "github"
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        user_id = self.user_id
+        user_login = self.user_login
+        account_type = self.account_type
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if user_id is not UNSET:
+            field_dict["user_id"] = user_id
+        if user_login is not UNSET:
+            field_dict["user_login"] = user_login
+        if account_type is not UNSET:
+            field_dict["account_type"] = account_type
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        user_id = d.pop("user_id", UNSET)
+
+        user_login = d.pop("user_login", UNSET)
+
+        account_type = d.pop("account_type", UNSET)
+
+        account = cls(
+            user_id=user_id,
+            user_login=user_login,
+            account_type=account_type,
+        )
+
+        account.additional_properties = d
+        return account
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/api_key.py` & `PyOblv-0.2.1/oblv/models/api_key.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="APIKey")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class APIKey:
-    """
-    Attributes:
-        key (str):
-    """
-
-    key: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        key = self.key
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "key": key,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        key = d.pop("key")
-
-        api_key = cls(
-            key=key,
-        )
-
-        api_key.additional_properties = d
-        return api_key
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="APIKey")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class APIKey:
+    """
+    Attributes:
+        key (str):
+    """
+
+    key: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        key = self.key
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "key": key,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        key = d.pop("key")
+
+        api_key = cls(
+            key=key,
+        )
+
+        api_key.additional_properties = d
+        return api_key
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/available_deployment.py` & `PyOblv-0.2.1/oblv/models/create_deployment_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, cast
-
-import attr
-
-from .deployment_complete import DeploymentComplete
-
-T = TypeVar("T", bound="AvailableDeployment")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class AvailableDeployment:
-    """
-    Attributes:
-        role (List[str]):
-        deployment (DeploymentComplete):
-    """
-
-    role: List[str]
-    deployment: DeploymentComplete
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        role = self.role
-
-        deployment = self.deployment.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "role": role,
-                "deployment": deployment,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        role = cast(List[str], d.pop("role"))
-
-        deployment = DeploymentComplete.from_dict(d.pop("deployment"))
-
-        available_deployment = cls(
-            role=role,
-            deployment=deployment,
-        )
-
-        available_deployment.additional_properties = d
-        return available_deployment
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="CreateDeploymentResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class CreateDeploymentResponse:
+    """
+    Attributes:
+        deployment_id (Union[Unset, str]):  Default: ''.
+        message (Union[Unset, str]):  Default: ''.
+    """
+
+    deployment_id: Union[Unset, str] = ""
+    message: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        deployment_id = self.deployment_id
+        message = self.message
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if deployment_id is not UNSET:
+            field_dict["deployment_id"] = deployment_id
+        if message is not UNSET:
+            field_dict["message"] = message
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        deployment_id = d.pop("deployment_id", UNSET)
+
+        message = d.pop("message", UNSET)
+
+        create_deployment_response = cls(
+            deployment_id=deployment_id,
+            message=message,
+        )
+
+        create_deployment_response.additional_properties = d
+        return create_deployment_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/available_deployment_list.py` & `PyOblv-0.2.1/oblv/models/deployment_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-from .available_deployment import AvailableDeployment
-
-T = TypeVar("T", bound="AvailableDeploymentList")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class AvailableDeploymentList:
-    """
-    Attributes:
-        total_pages (int):
-        deployments (List[AvailableDeployment]):
-    """
-
-    total_pages: int
-    deployments: List[AvailableDeployment]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        total_pages = self.total_pages
-        deployments = []
-        for deployments_item_data in self.deployments:
-            deployments_item = deployments_item_data.to_dict()
-
-            deployments.append(deployments_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "total_pages": total_pages,
-                "deployments": deployments,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        total_pages = d.pop("total_pages")
-
-        deployments = []
-        _deployments = d.pop("deployments")
-        for deployments_item_data in _deployments:
-            deployments_item = AvailableDeployment.from_dict(deployments_item_data)
-
-            deployments.append(deployments_item)
-
-        available_deployment_list = cls(
-            total_pages=total_pages,
-            deployments=deployments,
-        )
-
-        available_deployment_list.additional_properties = d
-        return available_deployment_list
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+from .deployment_complete import DeploymentComplete
+
+T = TypeVar("T", bound="DeploymentList")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class DeploymentList:
+    """
+    Attributes:
+        total_pages (int):
+        deployments (List[DeploymentComplete]):
+    """
+
+    total_pages: int
+    deployments: List[DeploymentComplete]
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        total_pages = self.total_pages
+        deployments = []
+        for deployments_item_data in self.deployments:
+            deployments_item = deployments_item_data.to_dict()
+
+            deployments.append(deployments_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "total_pages": total_pages,
+                "deployments": deployments,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        total_pages = d.pop("total_pages")
+
+        deployments = []
+        _deployments = d.pop("deployments")
+        for deployments_item_data in _deployments:
+            deployments_item = DeploymentComplete.from_dict(deployments_item_data)
+
+            deployments.append(deployments_item)
+
+        deployment_list = cls(
+            total_pages=total_pages,
+            deployments=deployments,
+        )
+
+        deployment_list.additional_properties = d
+        return deployment_list
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/build_args_schema.py` & `PyOblv-0.2.1/oblv/models/build_args_schema.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="BuildArgsSchema")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class BuildArgsSchema:
-    """
-    Attributes:
-        sha (Union[Unset, str]):  Default: ''.
-        arg_schema (Union[Unset, Any]):
-    """
-
-    sha: Union[Unset, str] = ""
-    arg_schema: Union[Unset, Any] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        sha = self.sha
-        arg_schema = self.arg_schema
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if sha is not UNSET:
-            field_dict["sha"] = sha
-        if arg_schema is not UNSET:
-            field_dict["arg_schema"] = arg_schema
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        sha = d.pop("sha", UNSET)
-
-        arg_schema = d.pop("arg_schema", UNSET)
-
-        build_args_schema = cls(
-            sha=sha,
-            arg_schema=arg_schema,
-        )
-
-        build_args_schema.additional_properties = d
-        return build_args_schema
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="BuildArgsSchema")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class BuildArgsSchema:
+    """
+    Attributes:
+        sha (Union[Unset, str]):  Default: ''.
+        arg_schema (Union[Unset, Any]):
+    """
+
+    sha: Union[Unset, str] = ""
+    arg_schema: Union[Unset, Any] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        sha = self.sha
+        arg_schema = self.arg_schema
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if sha is not UNSET:
+            field_dict["sha"] = sha
+        if arg_schema is not UNSET:
+            field_dict["arg_schema"] = arg_schema
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        sha = d.pop("sha", UNSET)
+
+        arg_schema = d.pop("arg_schema", UNSET)
+
+        build_args_schema = cls(
+            sha=sha,
+            arg_schema=arg_schema,
+        )
+
+        build_args_schema.additional_properties = d
+        return build_args_schema
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/create_deployment_input.py` & `PyOblv-0.2.1/oblv/models/create_deployment_input.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="CreateDeploymentInput")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class CreateDeploymentInput:
-    """
-    Attributes:
-        owner (str): Repository Owner
-        repo (str): Repository Name
-        account_type (str): VCS Account (Only 'github' supported as of now)
-        ref (str): Service ref
-        ref_type (str): Service ref type
-        region_name (str): AWS supported region the deployment must be deployed in.
-        deployment_name (str): Deployment Name
-        is_dev_env (bool): Deployment Environment
-        tags (List[str]): Deployment Tags
-        build_args (Any): Deployment build args
-        visibility (Union[Unset, str]): Deployment Visibility Default: 'private'.
-    """
-
-    owner: str
-    repo: str
-    account_type: str
-    ref: str
-    ref_type: str
-    region_name: str
-    deployment_name: str
-    is_dev_env: bool
-    tags: List[str]
-    build_args: Any
-    visibility: Union[Unset, str] = "private"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        owner = self.owner
-        repo = self.repo
-        account_type = self.account_type
-        ref = self.ref
-        ref_type = self.ref_type
-        region_name = self.region_name
-        deployment_name = self.deployment_name
-        is_dev_env = self.is_dev_env
-        tags = self.tags
-
-        build_args = self.build_args
-        visibility = self.visibility
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "owner": owner,
-                "repo": repo,
-                "account_type": account_type,
-                "ref": ref,
-                "ref_type": ref_type,
-                "region_name": region_name,
-                "deployment_name": deployment_name,
-                "is_dev_env": is_dev_env,
-                "tags": tags,
-                "build_args": build_args,
-            }
-        )
-        if visibility is not UNSET:
-            field_dict["visibility"] = visibility
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        owner = d.pop("owner")
-
-        repo = d.pop("repo")
-
-        account_type = d.pop("account_type")
-
-        ref = d.pop("ref")
-
-        ref_type = d.pop("ref_type")
-
-        region_name = d.pop("region_name")
-
-        deployment_name = d.pop("deployment_name")
-
-        is_dev_env = d.pop("is_dev_env")
-
-        tags = cast(List[str], d.pop("tags"))
-
-        build_args = d.pop("build_args")
-
-        visibility = d.pop("visibility", UNSET)
-
-        create_deployment_input = cls(
-            owner=owner,
-            repo=repo,
-            account_type=account_type,
-            ref=ref,
-            ref_type=ref_type,
-            region_name=region_name,
-            deployment_name=deployment_name,
-            is_dev_env=is_dev_env,
-            tags=tags,
-            build_args=build_args,
-            visibility=visibility,
-        )
-
-        create_deployment_input.additional_properties = d
-        return create_deployment_input
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="CreateDeploymentInput")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class CreateDeploymentInput:
+    """
+    Attributes:
+        owner (str): Repository Owner
+        repo (str): Repository Name
+        account_type (str): VCS Account (Only 'github' supported as of now)
+        ref (str): Service ref
+        ref_type (str): Service ref type
+        region_name (str): AWS supported region the deployment must be deployed in.
+        deployment_name (str): Deployment Name
+        is_dev_env (bool): Deployment Environment
+        tags (List[str]): Deployment Tags
+        build_args (Any): Deployment build args
+        visibility (Union[Unset, str]): Deployment Visibility Default: 'private'.
+    """
+
+    owner: str
+    repo: str
+    account_type: str
+    ref: str
+    ref_type: str
+    region_name: str
+    deployment_name: str
+    is_dev_env: bool
+    tags: List[str]
+    build_args: Any
+    visibility: Union[Unset, str] = "private"
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        owner = self.owner
+        repo = self.repo
+        account_type = self.account_type
+        ref = self.ref
+        ref_type = self.ref_type
+        region_name = self.region_name
+        deployment_name = self.deployment_name
+        is_dev_env = self.is_dev_env
+        tags = self.tags
+
+        build_args = self.build_args
+        visibility = self.visibility
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "owner": owner,
+                "repo": repo,
+                "account_type": account_type,
+                "ref": ref,
+                "ref_type": ref_type,
+                "region_name": region_name,
+                "deployment_name": deployment_name,
+                "is_dev_env": is_dev_env,
+                "tags": tags,
+                "build_args": build_args,
+            }
+        )
+        if visibility is not UNSET:
+            field_dict["visibility"] = visibility
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        owner = d.pop("owner")
+
+        repo = d.pop("repo")
+
+        account_type = d.pop("account_type")
+
+        ref = d.pop("ref")
+
+        ref_type = d.pop("ref_type")
+
+        region_name = d.pop("region_name")
+
+        deployment_name = d.pop("deployment_name")
+
+        is_dev_env = d.pop("is_dev_env")
+
+        tags = cast(List[str], d.pop("tags"))
+
+        build_args = d.pop("build_args")
+
+        visibility = d.pop("visibility", UNSET)
+
+        create_deployment_input = cls(
+            owner=owner,
+            repo=repo,
+            account_type=account_type,
+            ref=ref,
+            ref_type=ref_type,
+            region_name=region_name,
+            deployment_name=deployment_name,
+            is_dev_env=is_dev_env,
+            tags=tags,
+            build_args=build_args,
+            visibility=visibility,
+        )
+
+        create_deployment_input.additional_properties = d
+        return create_deployment_input
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/deployment_complete.py` & `PyOblv-0.2.1/oblv/models/deployment_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,272 +1,236 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
-
-import attr
-
-from ..models.access_history import AccessHistory
-from ..models.instance import Instance
-from ..models.shared_users import SharedUsers
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="DeploymentComplete")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class DeploymentComplete:
-    """
-    Attributes:
-        deployment_id (Union[Unset, str]):  Default: ''.
-        deployment_name (Union[Unset, str]):  Default: ''.
-        owner (Union[Unset, str]):  Default: ''.
-        repo_name (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: ''.
-        repo_owner (Union[Unset, str]):  Default: ''.
-        tags (Union[Unset, List[str]]):
-        branch_release (Union[Unset, str]):  Default: ''.
-        current_state (Union[Unset, str]):  Default: ''.
-        visibility (Union[Unset, str]):  Default: ''.
-        is_dev_env (Union[Unset, bool]):  Default: True.
-        creation_time (Union[Unset, str]):  Default: ''.
-        sha (Union[Unset, str]):  Default: ''.
-        owner_login (Union[Unset, str]):  Default: ''.
-        is_deleted (Union[Unset, bool]):
-        instance (Union[Unset, Instance]):
-        pcr_codes (Union[Unset, List[str]]):
-        credit_utilization_per_hour (Union[Unset, float]):
-        total_credits_used (Union[Unset, float]):
-        build_args (Union[Unset, Any]):
-        shared_users (Union[Unset, List[SharedUsers]]):
-        history (Union[Unset, List[AccessHistory]]):
-    """
-
-    deployment_id: Union[Unset, str] = ""
-    deployment_name: Union[Unset, str] = ""
-    owner: Union[Unset, str] = ""
-    repo_name: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = ""
-    repo_owner: Union[Unset, str] = ""
-    tags: Union[Unset, List[str]] = UNSET
-    branch_release: Union[Unset, str] = ""
-    current_state: Union[Unset, str] = ""
-    visibility: Union[Unset, str] = ""
-    is_dev_env: Union[Unset, bool] = True
-    creation_time: Union[Unset, str] = ""
-    sha: Union[Unset, str] = ""
-    owner_login: Union[Unset, str] = ""
-    is_deleted: Union[Unset, bool] = False
-    instance: Union[Unset, Instance] = UNSET
-    pcr_codes: Union[Unset, List[str]] = UNSET
-    credit_utilization_per_hour: Union[Unset, float] = 0.0
-    total_credits_used: Union[Unset, float] = 0.0
-    build_args: Union[Unset, Any] = UNSET
-    shared_users: Union[Unset, List[SharedUsers]] = UNSET
-    history: Union[Unset, List[AccessHistory]] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        deployment_id = self.deployment_id
-        deployment_name = self.deployment_name
-        owner = self.owner
-        repo_name = self.repo_name
-        account_type = self.account_type
-        repo_owner = self.repo_owner
-        tags: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.tags, Unset):
-            tags = self.tags
-
-        branch_release = self.branch_release
-        current_state = self.current_state
-        visibility = self.visibility
-        is_dev_env = self.is_dev_env
-        creation_time = self.creation_time
-        sha = self.sha
-        owner_login = self.owner_login
-        is_deleted = self.is_deleted
-        instance: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.instance, Unset):
-            instance = self.instance.to_dict()
-
-        pcr_codes: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.pcr_codes, Unset):
-            pcr_codes = self.pcr_codes
-
-        credit_utilization_per_hour = self.credit_utilization_per_hour
-        total_credits_used = self.total_credits_used
-        build_args = self.build_args
-        shared_users: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.shared_users, Unset):
-            shared_users = []
-            for shared_users_item_data in self.shared_users:
-                shared_users_item = shared_users_item_data.to_dict()
-
-                shared_users.append(shared_users_item)
-
-        history: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.history, Unset):
-            history = []
-            for history_item_data in self.history:
-                history_item = history_item_data.to_dict()
-
-                history.append(history_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if deployment_id is not UNSET:
-            field_dict["deployment_id"] = deployment_id
-        if deployment_name is not UNSET:
-            field_dict["deployment_name"] = deployment_name
-        if owner is not UNSET:
-            field_dict["owner"] = owner
-        if repo_name is not UNSET:
-            field_dict["repo_name"] = repo_name
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
-        if repo_owner is not UNSET:
-            field_dict["repo_owner"] = repo_owner
-        if tags is not UNSET:
-            field_dict["tags"] = tags
-        if branch_release is not UNSET:
-            field_dict["branch_release"] = branch_release
-        if current_state is not UNSET:
-            field_dict["current_state"] = current_state
-        if visibility is not UNSET:
-            field_dict["visibility"] = visibility
-        if is_dev_env is not UNSET:
-            field_dict["is_dev_env"] = is_dev_env
-        if creation_time is not UNSET:
-            field_dict["creation_time"] = creation_time
-        if sha is not UNSET:
-            field_dict["sha"] = sha
-        if owner_login is not UNSET:
-            field_dict["owner_login"] = owner_login
-        if is_deleted is not UNSET:
-            field_dict["is_deleted"] = is_deleted
-        if instance is not UNSET:
-            field_dict["instance"] = instance
-        if pcr_codes is not UNSET:
-            field_dict["pcr_codes"] = pcr_codes
-        if credit_utilization_per_hour is not UNSET:
-            field_dict["credit_utilization_per_hour"] = credit_utilization_per_hour
-        if total_credits_used is not UNSET:
-            field_dict["total_credits_used"] = total_credits_used
-        if build_args is not UNSET:
-            field_dict["build_args"] = build_args
-        if shared_users is not UNSET:
-            field_dict["shared_users"] = shared_users
-        if history is not UNSET:
-            field_dict["history"] = history
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        deployment_id = d.pop("deployment_id", UNSET)
-
-        deployment_name = d.pop("deployment_name", UNSET)
-
-        owner = d.pop("owner", UNSET)
-
-        repo_name = d.pop("repo_name", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
-        repo_owner = d.pop("repo_owner", UNSET)
-
-        tags = cast(List[str], d.pop("tags", UNSET))
-
-        branch_release = d.pop("branch_release", UNSET)
-
-        current_state = d.pop("current_state", UNSET)
-
-        visibility = d.pop("visibility", UNSET)
-
-        is_dev_env = d.pop("is_dev_env", UNSET)
-
-        creation_time = d.pop("creation_time", UNSET)
-
-        sha = d.pop("sha", UNSET)
-
-        owner_login = d.pop("owner_login", UNSET)
-
-        is_deleted = d.pop("is_deleted", UNSET)
-
-        _instance = d.pop("instance", UNSET)
-        instance: Union[Unset, Instance]
-        if isinstance(_instance, Unset):
-            instance = UNSET
-        else:
-            instance = Instance.from_dict(_instance)
-
-        pcr_codes = cast(List[str], d.pop("pcr_codes", UNSET))
-
-        credit_utilization_per_hour = d.pop("credit_utilization_per_hour", UNSET)
-
-        total_credits_used = d.pop("total_credits_used", UNSET)
-
-        build_args = d.pop("build_args", UNSET)
-
-        shared_users = []
-        _shared_users = d.pop("shared_users", UNSET)
-        for shared_users_item_data in _shared_users or []:
-            shared_users_item = SharedUsers.from_dict(shared_users_item_data)
-
-            shared_users.append(shared_users_item)
-
-        history = []
-        _history = d.pop("history", UNSET)
-        for history_item_data in _history or []:
-            history_item = AccessHistory.from_dict(history_item_data)
-
-            history.append(history_item)
-
-        deployment_complete = cls(
-            deployment_id=deployment_id,
-            deployment_name=deployment_name,
-            owner=owner,
-            repo_name=repo_name,
-            account_type=account_type,
-            repo_owner=repo_owner,
-            tags=tags,
-            branch_release=branch_release,
-            current_state=current_state,
-            visibility=visibility,
-            is_dev_env=is_dev_env,
-            creation_time=creation_time,
-            sha=sha,
-            owner_login=owner_login,
-            is_deleted=is_deleted,
-            instance=instance,
-            pcr_codes=pcr_codes,
-            credit_utilization_per_hour=credit_utilization_per_hour,
-            total_credits_used=total_credits_used,
-            build_args=build_args,
-            shared_users=shared_users,
-            history=history,
-        )
-
-        deployment_complete.additional_properties = d
-        return deployment_complete
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
+
+import attr
+
+from ..models.instance import Instance
+from ..models.shared_users import SharedUsers
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="DeploymentResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class DeploymentResponse:
+    """
+    Attributes:
+        deployment_id (Union[Unset, str]):  Default: ''.
+        deployment_name (Union[Unset, str]):  Default: ''.
+        owner_login (Union[Unset, str]):  Default: ''.
+        repo_name (Union[Unset, str]):  Default: ''.
+        account_type (Union[Unset, str]):  Default: ''.
+        repo_owner (Union[Unset, str]):  Default: ''.
+        tags (Union[Unset, List[str]]):
+        branch_release (Union[Unset, str]):  Default: ''.
+        current_state (Union[Unset, str]):  Default: ''.
+        visibility (Union[Unset, str]):  Default: ''.
+        is_dev_env (Union[Unset, bool]):  Default: True.
+        pcr_codes (Union[Unset, List[str]]):
+        credit_utilization_per_hour (Union[Unset, float]):
+        creation_time (Union[Unset, str]):  Default: ''.
+        sha (Union[Unset, str]):  Default: ''.
+        is_deleted (Union[Unset, bool]):
+        build_args (Union[Unset, Any]):
+        instance (Union[Unset, Instance]):
+        shared_users (Union[Unset, List[SharedUsers]]):
+    """
+
+    deployment_id: Union[Unset, str] = ""
+    deployment_name: Union[Unset, str] = ""
+    owner_login: Union[Unset, str] = ""
+    repo_name: Union[Unset, str] = ""
+    account_type: Union[Unset, str] = ""
+    repo_owner: Union[Unset, str] = ""
+    tags: Union[Unset, List[str]] = UNSET
+    branch_release: Union[Unset, str] = ""
+    current_state: Union[Unset, str] = ""
+    visibility: Union[Unset, str] = ""
+    is_dev_env: Union[Unset, bool] = True
+    pcr_codes: Union[Unset, List[str]] = UNSET
+    credit_utilization_per_hour: Union[Unset, float] = 0.0
+    creation_time: Union[Unset, str] = ""
+    sha: Union[Unset, str] = ""
+    is_deleted: Union[Unset,bool] = UNSET
+    build_args: Union[Unset, Any] = UNSET
+    instance: Union[Unset, Instance] = UNSET
+    shared_users: Union[Unset, List[SharedUsers]] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        deployment_id = self.deployment_id
+        deployment_name = self.deployment_name
+        owner_login = self.owner_login
+        repo_name = self.repo_name
+        account_type = self.account_type
+        repo_owner = self.repo_owner
+        tags: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.tags, Unset):
+            tags = self.tags
+
+        branch_release = self.branch_release
+        current_state = self.current_state
+        visibility = self.visibility
+        is_dev_env = self.is_dev_env
+        pcr_codes: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.pcr_codes, Unset):
+            pcr_codes = self.pcr_codes
+
+        credit_utilization_per_hour = self.credit_utilization_per_hour
+        creation_time = self.creation_time
+        sha = self.sha
+        if not isinstance(self.is_deleted, Unset):
+            is_deleted = self.is_deleted
+        build_args = self.build_args
+        instance: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.instance, Unset):
+            instance = self.instance.to_dict()
+
+        shared_users: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.shared_users, Unset):
+            shared_users = []
+            for shared_users_item_data in self.shared_users:
+                shared_users_item = shared_users_item_data.to_dict()
+
+                shared_users.append(shared_users_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if deployment_id is not UNSET:
+            field_dict["deployment_id"] = deployment_id
+        if deployment_name is not UNSET:
+            field_dict["deployment_name"] = deployment_name
+        if owner_login is not UNSET:
+            field_dict["owner_login"] = owner_login
+        if repo_name is not UNSET:
+            field_dict["repo_name"] = repo_name
+        if account_type is not UNSET:
+            field_dict["account_type"] = account_type
+        if repo_owner is not UNSET:
+            field_dict["repo_owner"] = repo_owner
+        if tags is not UNSET:
+            field_dict["tags"] = tags
+        if branch_release is not UNSET:
+            field_dict["branch_release"] = branch_release
+        if current_state is not UNSET:
+            field_dict["current_state"] = current_state
+        if visibility is not UNSET:
+            field_dict["visibility"] = visibility
+        if is_dev_env is not UNSET:
+            field_dict["is_dev_env"] = is_dev_env
+        if pcr_codes is not UNSET:
+            field_dict["pcr_codes"] = pcr_codes
+        if credit_utilization_per_hour is not UNSET:
+            field_dict["credit_utilization_per_hour"] = credit_utilization_per_hour
+        if creation_time is not UNSET:
+            field_dict["creation_time"] = creation_time
+        if sha is not UNSET:
+            field_dict["sha"] = sha
+        if is_deleted is not UNSET:
+            field_dict["is_deleted"] = is_deleted
+        if build_args is not UNSET:
+            field_dict["build_args"] = build_args
+        if instance is not UNSET:
+            field_dict["instance"] = instance
+        if shared_users is not UNSET:
+            field_dict["shared_users"] = shared_users
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        deployment_id = d.pop("deployment_id", UNSET)
+
+        deployment_name = d.pop("deployment_name", UNSET)
+
+        owner_login = d.pop("owner_login", UNSET)
+
+        repo_name = d.pop("repo_name", UNSET)
+
+        account_type = d.pop("account_type", UNSET)
+
+        repo_owner = d.pop("repo_owner", UNSET)
+
+        tags = cast(List[str], d.pop("tags", UNSET))
+
+        branch_release = d.pop("branch_release", UNSET)
+
+        current_state = d.pop("current_state", UNSET)
+
+        visibility = d.pop("visibility", UNSET)
+
+        is_dev_env = d.pop("is_dev_env", UNSET)
+
+        pcr_codes = cast(List[str], d.pop("pcr_codes", UNSET))
+
+        credit_utilization_per_hour = d.pop("credit_utilization_per_hour", UNSET)
+
+        creation_time = d.pop("creation_time", UNSET)
+
+        sha = d.pop("sha", UNSET)
+        
+        is_deleted = d.pop("is_deleted", UNSET)
+
+        build_args = d.pop("build_args", UNSET)
+
+        _instance = d.pop("instance", UNSET)
+        instance: Union[Unset, Instance]
+        if isinstance(_instance, Unset):
+            instance = UNSET
+        else:
+            instance = Instance.from_dict(_instance)
+
+        shared_users = []
+        _shared_users = d.pop("shared_users", UNSET)
+        for shared_users_item_data in _shared_users or []:
+            shared_users_item = SharedUsers.from_dict(shared_users_item_data)
+
+            shared_users.append(shared_users_item)
+
+        deployment_response = cls(
+            deployment_id=deployment_id,
+            deployment_name=deployment_name,
+            owner_login=owner_login,
+            repo_name=repo_name,
+            account_type=account_type,
+            repo_owner=repo_owner,
+            tags=tags,
+            branch_release=branch_release,
+            current_state=current_state,
+            visibility=visibility,
+            is_dev_env=is_dev_env,
+            pcr_codes=pcr_codes,
+            credit_utilization_per_hour=credit_utilization_per_hour,
+            creation_time=creation_time,
+            sha=sha,
+            is_deleted=is_deleted,
+            build_args=build_args,
+            instance=instance,
+            shared_users=shared_users,
+        )
+
+        deployment_response.additional_properties = d
+        return deployment_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/deployment_list.py` & `PyOblv-0.2.1/oblv/models/available_deployment_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-from .deployment_complete import DeploymentComplete
-
-T = TypeVar("T", bound="DeploymentList")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class DeploymentList:
-    """
-    Attributes:
-        total_pages (int):
-        deployments (List[DeploymentComplete]):
-    """
-
-    total_pages: int
-    deployments: List[DeploymentComplete]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        total_pages = self.total_pages
-        deployments = []
-        for deployments_item_data in self.deployments:
-            deployments_item = deployments_item_data.to_dict()
-
-            deployments.append(deployments_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "total_pages": total_pages,
-                "deployments": deployments,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        total_pages = d.pop("total_pages")
-
-        deployments = []
-        _deployments = d.pop("deployments")
-        for deployments_item_data in _deployments:
-            deployments_item = DeploymentComplete.from_dict(deployments_item_data)
-
-            deployments.append(deployments_item)
-
-        deployment_list = cls(
-            total_pages=total_pages,
-            deployments=deployments,
-        )
-
-        deployment_list.additional_properties = d
-        return deployment_list
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+from .available_deployment import AvailableDeployment
+
+T = TypeVar("T", bound="AvailableDeploymentList")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class AvailableDeploymentList:
+    """
+    Attributes:
+        total_pages (int):
+        deployments (List[AvailableDeployment]):
+    """
+
+    total_pages: int
+    deployments: List[AvailableDeployment]
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        total_pages = self.total_pages
+        deployments = []
+        for deployments_item_data in self.deployments:
+            deployments_item = deployments_item_data.to_dict()
+
+            deployments.append(deployments_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "total_pages": total_pages,
+                "deployments": deployments,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        total_pages = d.pop("total_pages")
+
+        deployments = []
+        _deployments = d.pop("deployments")
+        for deployments_item_data in _deployments:
+            deployments_item = AvailableDeployment.from_dict(deployments_item_data)
+
+            deployments.append(deployments_item)
+
+        available_deployment_list = cls(
+            total_pages=total_pages,
+            deployments=deployments,
+        )
+
+        available_deployment_list.additional_properties = d
+        return available_deployment_list
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/deployment_response.py` & `PyOblv-0.2.1/oblv/models/deployment_complete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,236 +1,272 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
-
-import attr
-
-from ..models.instance import Instance
-from ..models.shared_users import SharedUsers
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="DeploymentResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class DeploymentResponse:
-    """
-    Attributes:
-        deployment_id (Union[Unset, str]):  Default: ''.
-        deployment_name (Union[Unset, str]):  Default: ''.
-        owner_login (Union[Unset, str]):  Default: ''.
-        repo_name (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: ''.
-        repo_owner (Union[Unset, str]):  Default: ''.
-        tags (Union[Unset, List[str]]):
-        branch_release (Union[Unset, str]):  Default: ''.
-        current_state (Union[Unset, str]):  Default: ''.
-        visibility (Union[Unset, str]):  Default: ''.
-        is_dev_env (Union[Unset, bool]):  Default: True.
-        pcr_codes (Union[Unset, List[str]]):
-        credit_utilization_per_hour (Union[Unset, float]):
-        creation_time (Union[Unset, str]):  Default: ''.
-        sha (Union[Unset, str]):  Default: ''.
-        is_deleted (Union[Unset, bool]):
-        build_args (Union[Unset, Any]):
-        instance (Union[Unset, Instance]):
-        shared_users (Union[Unset, List[SharedUsers]]):
-    """
-
-    deployment_id: Union[Unset, str] = ""
-    deployment_name: Union[Unset, str] = ""
-    owner_login: Union[Unset, str] = ""
-    repo_name: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = ""
-    repo_owner: Union[Unset, str] = ""
-    tags: Union[Unset, List[str]] = UNSET
-    branch_release: Union[Unset, str] = ""
-    current_state: Union[Unset, str] = ""
-    visibility: Union[Unset, str] = ""
-    is_dev_env: Union[Unset, bool] = True
-    pcr_codes: Union[Unset, List[str]] = UNSET
-    credit_utilization_per_hour: Union[Unset, float] = 0.0
-    creation_time: Union[Unset, str] = ""
-    sha: Union[Unset, str] = ""
-    is_deleted: Union[Unset,bool] = UNSET
-    build_args: Union[Unset, Any] = UNSET
-    instance: Union[Unset, Instance] = UNSET
-    shared_users: Union[Unset, List[SharedUsers]] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        deployment_id = self.deployment_id
-        deployment_name = self.deployment_name
-        owner_login = self.owner_login
-        repo_name = self.repo_name
-        account_type = self.account_type
-        repo_owner = self.repo_owner
-        tags: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.tags, Unset):
-            tags = self.tags
-
-        branch_release = self.branch_release
-        current_state = self.current_state
-        visibility = self.visibility
-        is_dev_env = self.is_dev_env
-        pcr_codes: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.pcr_codes, Unset):
-            pcr_codes = self.pcr_codes
-
-        credit_utilization_per_hour = self.credit_utilization_per_hour
-        creation_time = self.creation_time
-        sha = self.sha
-        if not isinstance(self.is_deleted, Unset):
-            is_deleted = self.is_deleted
-        build_args = self.build_args
-        instance: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.instance, Unset):
-            instance = self.instance.to_dict()
-
-        shared_users: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.shared_users, Unset):
-            shared_users = []
-            for shared_users_item_data in self.shared_users:
-                shared_users_item = shared_users_item_data.to_dict()
-
-                shared_users.append(shared_users_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if deployment_id is not UNSET:
-            field_dict["deployment_id"] = deployment_id
-        if deployment_name is not UNSET:
-            field_dict["deployment_name"] = deployment_name
-        if owner_login is not UNSET:
-            field_dict["owner_login"] = owner_login
-        if repo_name is not UNSET:
-            field_dict["repo_name"] = repo_name
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
-        if repo_owner is not UNSET:
-            field_dict["repo_owner"] = repo_owner
-        if tags is not UNSET:
-            field_dict["tags"] = tags
-        if branch_release is not UNSET:
-            field_dict["branch_release"] = branch_release
-        if current_state is not UNSET:
-            field_dict["current_state"] = current_state
-        if visibility is not UNSET:
-            field_dict["visibility"] = visibility
-        if is_dev_env is not UNSET:
-            field_dict["is_dev_env"] = is_dev_env
-        if pcr_codes is not UNSET:
-            field_dict["pcr_codes"] = pcr_codes
-        if credit_utilization_per_hour is not UNSET:
-            field_dict["credit_utilization_per_hour"] = credit_utilization_per_hour
-        if creation_time is not UNSET:
-            field_dict["creation_time"] = creation_time
-        if sha is not UNSET:
-            field_dict["sha"] = sha
-        if is_deleted is not UNSET:
-            field_dict["is_deleted"] = is_deleted
-        if build_args is not UNSET:
-            field_dict["build_args"] = build_args
-        if instance is not UNSET:
-            field_dict["instance"] = instance
-        if shared_users is not UNSET:
-            field_dict["shared_users"] = shared_users
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        deployment_id = d.pop("deployment_id", UNSET)
-
-        deployment_name = d.pop("deployment_name", UNSET)
-
-        owner_login = d.pop("owner_login", UNSET)
-
-        repo_name = d.pop("repo_name", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
-        repo_owner = d.pop("repo_owner", UNSET)
-
-        tags = cast(List[str], d.pop("tags", UNSET))
-
-        branch_release = d.pop("branch_release", UNSET)
-
-        current_state = d.pop("current_state", UNSET)
-
-        visibility = d.pop("visibility", UNSET)
-
-        is_dev_env = d.pop("is_dev_env", UNSET)
-
-        pcr_codes = cast(List[str], d.pop("pcr_codes", UNSET))
-
-        credit_utilization_per_hour = d.pop("credit_utilization_per_hour", UNSET)
-
-        creation_time = d.pop("creation_time", UNSET)
-
-        sha = d.pop("sha", UNSET)
-        
-        is_deleted = d.pop("is_deleted", UNSET)
-
-        build_args = d.pop("build_args", UNSET)
-
-        _instance = d.pop("instance", UNSET)
-        instance: Union[Unset, Instance]
-        if isinstance(_instance, Unset):
-            instance = UNSET
-        else:
-            instance = Instance.from_dict(_instance)
-
-        shared_users = []
-        _shared_users = d.pop("shared_users", UNSET)
-        for shared_users_item_data in _shared_users or []:
-            shared_users_item = SharedUsers.from_dict(shared_users_item_data)
-
-            shared_users.append(shared_users_item)
-
-        deployment_response = cls(
-            deployment_id=deployment_id,
-            deployment_name=deployment_name,
-            owner_login=owner_login,
-            repo_name=repo_name,
-            account_type=account_type,
-            repo_owner=repo_owner,
-            tags=tags,
-            branch_release=branch_release,
-            current_state=current_state,
-            visibility=visibility,
-            is_dev_env=is_dev_env,
-            pcr_codes=pcr_codes,
-            credit_utilization_per_hour=credit_utilization_per_hour,
-            creation_time=creation_time,
-            sha=sha,
-            is_deleted=is_deleted,
-            build_args=build_args,
-            instance=instance,
-            shared_users=shared_users,
-        )
-
-        deployment_response.additional_properties = d
-        return deployment_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
+
+import attr
+
+from ..models.access_history import AccessHistory
+from ..models.instance import Instance
+from ..models.shared_users import SharedUsers
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="DeploymentComplete")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class DeploymentComplete:
+    """
+    Attributes:
+        deployment_id (Union[Unset, str]):  Default: ''.
+        deployment_name (Union[Unset, str]):  Default: ''.
+        owner (Union[Unset, str]):  Default: ''.
+        repo_name (Union[Unset, str]):  Default: ''.
+        account_type (Union[Unset, str]):  Default: ''.
+        repo_owner (Union[Unset, str]):  Default: ''.
+        tags (Union[Unset, List[str]]):
+        branch_release (Union[Unset, str]):  Default: ''.
+        current_state (Union[Unset, str]):  Default: ''.
+        visibility (Union[Unset, str]):  Default: ''.
+        is_dev_env (Union[Unset, bool]):  Default: True.
+        creation_time (Union[Unset, str]):  Default: ''.
+        sha (Union[Unset, str]):  Default: ''.
+        owner_login (Union[Unset, str]):  Default: ''.
+        is_deleted (Union[Unset, bool]):
+        instance (Union[Unset, Instance]):
+        pcr_codes (Union[Unset, List[str]]):
+        credit_utilization_per_hour (Union[Unset, float]):
+        total_credits_used (Union[Unset, float]):
+        build_args (Union[Unset, Any]):
+        shared_users (Union[Unset, List[SharedUsers]]):
+        history (Union[Unset, List[AccessHistory]]):
+    """
+
+    deployment_id: Union[Unset, str] = ""
+    deployment_name: Union[Unset, str] = ""
+    owner: Union[Unset, str] = ""
+    repo_name: Union[Unset, str] = ""
+    account_type: Union[Unset, str] = ""
+    repo_owner: Union[Unset, str] = ""
+    tags: Union[Unset, List[str]] = UNSET
+    branch_release: Union[Unset, str] = ""
+    current_state: Union[Unset, str] = ""
+    visibility: Union[Unset, str] = ""
+    is_dev_env: Union[Unset, bool] = True
+    creation_time: Union[Unset, str] = ""
+    sha: Union[Unset, str] = ""
+    owner_login: Union[Unset, str] = ""
+    is_deleted: Union[Unset, bool] = False
+    instance: Union[Unset, Instance] = UNSET
+    pcr_codes: Union[Unset, List[str]] = UNSET
+    credit_utilization_per_hour: Union[Unset, float] = 0.0
+    total_credits_used: Union[Unset, float] = 0.0
+    build_args: Union[Unset, Any] = UNSET
+    shared_users: Union[Unset, List[SharedUsers]] = UNSET
+    history: Union[Unset, List[AccessHistory]] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        deployment_id = self.deployment_id
+        deployment_name = self.deployment_name
+        owner = self.owner
+        repo_name = self.repo_name
+        account_type = self.account_type
+        repo_owner = self.repo_owner
+        tags: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.tags, Unset):
+            tags = self.tags
+
+        branch_release = self.branch_release
+        current_state = self.current_state
+        visibility = self.visibility
+        is_dev_env = self.is_dev_env
+        creation_time = self.creation_time
+        sha = self.sha
+        owner_login = self.owner_login
+        is_deleted = self.is_deleted
+        instance: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.instance, Unset):
+            instance = self.instance.to_dict()
+
+        pcr_codes: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.pcr_codes, Unset):
+            pcr_codes = self.pcr_codes
+
+        credit_utilization_per_hour = self.credit_utilization_per_hour
+        total_credits_used = self.total_credits_used
+        build_args = self.build_args
+        shared_users: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.shared_users, Unset):
+            shared_users = []
+            for shared_users_item_data in self.shared_users:
+                shared_users_item = shared_users_item_data.to_dict()
+
+                shared_users.append(shared_users_item)
+
+        history: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.history, Unset):
+            history = []
+            for history_item_data in self.history:
+                history_item = history_item_data.to_dict()
+
+                history.append(history_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if deployment_id is not UNSET:
+            field_dict["deployment_id"] = deployment_id
+        if deployment_name is not UNSET:
+            field_dict["deployment_name"] = deployment_name
+        if owner is not UNSET:
+            field_dict["owner"] = owner
+        if repo_name is not UNSET:
+            field_dict["repo_name"] = repo_name
+        if account_type is not UNSET:
+            field_dict["account_type"] = account_type
+        if repo_owner is not UNSET:
+            field_dict["repo_owner"] = repo_owner
+        if tags is not UNSET:
+            field_dict["tags"] = tags
+        if branch_release is not UNSET:
+            field_dict["branch_release"] = branch_release
+        if current_state is not UNSET:
+            field_dict["current_state"] = current_state
+        if visibility is not UNSET:
+            field_dict["visibility"] = visibility
+        if is_dev_env is not UNSET:
+            field_dict["is_dev_env"] = is_dev_env
+        if creation_time is not UNSET:
+            field_dict["creation_time"] = creation_time
+        if sha is not UNSET:
+            field_dict["sha"] = sha
+        if owner_login is not UNSET:
+            field_dict["owner_login"] = owner_login
+        if is_deleted is not UNSET:
+            field_dict["is_deleted"] = is_deleted
+        if instance is not UNSET:
+            field_dict["instance"] = instance
+        if pcr_codes is not UNSET:
+            field_dict["pcr_codes"] = pcr_codes
+        if credit_utilization_per_hour is not UNSET:
+            field_dict["credit_utilization_per_hour"] = credit_utilization_per_hour
+        if total_credits_used is not UNSET:
+            field_dict["total_credits_used"] = total_credits_used
+        if build_args is not UNSET:
+            field_dict["build_args"] = build_args
+        if shared_users is not UNSET:
+            field_dict["shared_users"] = shared_users
+        if history is not UNSET:
+            field_dict["history"] = history
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        deployment_id = d.pop("deployment_id", UNSET)
+
+        deployment_name = d.pop("deployment_name", UNSET)
+
+        owner = d.pop("owner", UNSET)
+
+        repo_name = d.pop("repo_name", UNSET)
+
+        account_type = d.pop("account_type", UNSET)
+
+        repo_owner = d.pop("repo_owner", UNSET)
+
+        tags = cast(List[str], d.pop("tags", UNSET))
+
+        branch_release = d.pop("branch_release", UNSET)
+
+        current_state = d.pop("current_state", UNSET)
+
+        visibility = d.pop("visibility", UNSET)
+
+        is_dev_env = d.pop("is_dev_env", UNSET)
+
+        creation_time = d.pop("creation_time", UNSET)
+
+        sha = d.pop("sha", UNSET)
+
+        owner_login = d.pop("owner_login", UNSET)
+
+        is_deleted = d.pop("is_deleted", UNSET)
+
+        _instance = d.pop("instance", UNSET)
+        instance: Union[Unset, Instance]
+        if isinstance(_instance, Unset):
+            instance = UNSET
+        else:
+            instance = Instance.from_dict(_instance)
+
+        pcr_codes = cast(List[str], d.pop("pcr_codes", UNSET))
+
+        credit_utilization_per_hour = d.pop("credit_utilization_per_hour", UNSET)
+
+        total_credits_used = d.pop("total_credits_used", UNSET)
+
+        build_args = d.pop("build_args", UNSET)
+
+        shared_users = []
+        _shared_users = d.pop("shared_users", UNSET)
+        for shared_users_item_data in _shared_users or []:
+            shared_users_item = SharedUsers.from_dict(shared_users_item_data)
+
+            shared_users.append(shared_users_item)
+
+        history = []
+        _history = d.pop("history", UNSET)
+        for history_item_data in _history or []:
+            history_item = AccessHistory.from_dict(history_item_data)
+
+            history.append(history_item)
+
+        deployment_complete = cls(
+            deployment_id=deployment_id,
+            deployment_name=deployment_name,
+            owner=owner,
+            repo_name=repo_name,
+            account_type=account_type,
+            repo_owner=repo_owner,
+            tags=tags,
+            branch_release=branch_release,
+            current_state=current_state,
+            visibility=visibility,
+            is_dev_env=is_dev_env,
+            creation_time=creation_time,
+            sha=sha,
+            owner_login=owner_login,
+            is_deleted=is_deleted,
+            instance=instance,
+            pcr_codes=pcr_codes,
+            credit_utilization_per_hour=credit_utilization_per_hour,
+            total_credits_used=total_credits_used,
+            build_args=build_args,
+            shared_users=shared_users,
+            history=history,
+        )
+
+        deployment_complete.additional_properties = d
+        return deployment_complete
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/http_validation_error.py` & `PyOblv-0.2.1/oblv/models/http_validation_error.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..models.validation_error import ValidationError
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="HTTPValidationError")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class HTTPValidationError:
-    """
-    Attributes:
-        detail (Union[Unset, List[ValidationError]]):
-    """
-
-    detail: Union[Unset, List[ValidationError]] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        detail: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.detail, Unset):
-            detail = []
-            for detail_item_data in self.detail:
-                detail_item = detail_item_data.to_dict()
-
-                detail.append(detail_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if detail is not UNSET:
-            field_dict["detail"] = detail
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        detail = []
-        _detail = d.pop("detail", UNSET)
-        for detail_item_data in _detail or []:
-            detail_item = ValidationError.from_dict(detail_item_data)
-
-            detail.append(detail_item)
-
-        http_validation_error = cls(
-            detail=detail,
-        )
-
-        http_validation_error.additional_properties = d
-        return http_validation_error
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..models.validation_error import ValidationError
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="HTTPValidationError")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class HTTPValidationError:
+    """
+    Attributes:
+        detail (Union[Unset, List[ValidationError]]):
+    """
+
+    detail: Union[Unset, List[ValidationError]] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        detail: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.detail, Unset):
+            detail = []
+            for detail_item_data in self.detail:
+                detail_item = detail_item_data.to_dict()
+
+                detail.append(detail_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if detail is not UNSET:
+            field_dict["detail"] = detail
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        detail = []
+        _detail = d.pop("detail", UNSET)
+        for detail_item_data in _detail or []:
+            detail_item = ValidationError.from_dict(detail_item_data)
+
+            detail.append(detail_item)
+
+        http_validation_error = cls(
+            detail=detail,
+        )
+
+        http_validation_error.additional_properties = d
+        return http_validation_error
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/instance.py` & `PyOblv-0.2.1/oblv/models/instance.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="Instance")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class Instance:
-    """
-    Attributes:
-        region_name (Union[Unset, str]):  Default: ''.
-        stack_name (Union[Unset, str]):  Default: ''.
-        instance_type (Union[Unset, str]):  Default: ''.
-        instance_url (Union[Unset, str]):  Default: ''.
-        service_url (Union[Unset, str]):  Default: ''.
-        build_log_location (Union[Unset, str]):  Default: ''.
-    """
-
-    region_name: Union[Unset, str] = ""
-    stack_name: Union[Unset, str] = ""
-    instance_type: Union[Unset, str] = ""
-    instance_url: Union[Unset, str] = ""
-    service_url: Union[Unset, str] = ""
-    build_log_location: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        region_name = self.region_name
-        stack_name = self.stack_name
-        instance_type = self.instance_type
-        instance_url = self.instance_url
-        service_url = self.service_url
-        build_log_location = self.build_log_location
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if region_name is not UNSET:
-            field_dict["region_name"] = region_name
-        if stack_name is not UNSET:
-            field_dict["stack_name"] = stack_name
-        if instance_type is not UNSET:
-            field_dict["instance_type"] = instance_type
-        if instance_url is not UNSET:
-            field_dict["instance_url"] = instance_url
-        if service_url is not UNSET:
-            field_dict["service_url"] = service_url
-        if build_log_location is not UNSET:
-            field_dict["build_log_location"] = build_log_location
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        region_name = d.pop("region_name", UNSET)
-
-        stack_name = d.pop("stack_name", UNSET)
-
-        instance_type = d.pop("instance_type", UNSET)
-
-        instance_url = d.pop("instance_url", UNSET)
-
-        service_url = d.pop("service_url", UNSET)
-
-        build_log_location = d.pop("build_log_location", UNSET)
-
-        instance = cls(
-            region_name=region_name,
-            stack_name=stack_name,
-            instance_type=instance_type,
-            instance_url=instance_url,
-            service_url=service_url,
-            build_log_location=build_log_location,
-        )
-
-        instance.additional_properties = d
-        return instance
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="Instance")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class Instance:
+    """
+    Attributes:
+        region_name (Union[Unset, str]):  Default: ''.
+        stack_name (Union[Unset, str]):  Default: ''.
+        instance_type (Union[Unset, str]):  Default: ''.
+        instance_url (Union[Unset, str]):  Default: ''.
+        service_url (Union[Unset, str]):  Default: ''.
+        build_log_location (Union[Unset, str]):  Default: ''.
+    """
+
+    region_name: Union[Unset, str] = ""
+    stack_name: Union[Unset, str] = ""
+    instance_type: Union[Unset, str] = ""
+    instance_url: Union[Unset, str] = ""
+    service_url: Union[Unset, str] = ""
+    build_log_location: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        region_name = self.region_name
+        stack_name = self.stack_name
+        instance_type = self.instance_type
+        instance_url = self.instance_url
+        service_url = self.service_url
+        build_log_location = self.build_log_location
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if region_name is not UNSET:
+            field_dict["region_name"] = region_name
+        if stack_name is not UNSET:
+            field_dict["stack_name"] = stack_name
+        if instance_type is not UNSET:
+            field_dict["instance_type"] = instance_type
+        if instance_url is not UNSET:
+            field_dict["instance_url"] = instance_url
+        if service_url is not UNSET:
+            field_dict["service_url"] = service_url
+        if build_log_location is not UNSET:
+            field_dict["build_log_location"] = build_log_location
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        region_name = d.pop("region_name", UNSET)
+
+        stack_name = d.pop("stack_name", UNSET)
+
+        instance_type = d.pop("instance_type", UNSET)
+
+        instance_url = d.pop("instance_url", UNSET)
+
+        service_url = d.pop("service_url", UNSET)
+
+        build_log_location = d.pop("build_log_location", UNSET)
+
+        instance = cls(
+            region_name=region_name,
+            stack_name=stack_name,
+            instance_type=instance_type,
+            instance_url=instance_url,
+            service_url=service_url,
+            build_log_location=build_log_location,
+        )
+
+        instance.additional_properties = d
+        return instance
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/message_model.py` & `PyOblv-0.2.1/oblv/models/message_model.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="MessageModel")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class MessageModel:
-    """
-    Attributes:
-        message (Union[Unset, str]):  Default: ''.
-    """
-
-    message: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        message = self.message
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if message is not UNSET:
-            field_dict["message"] = message
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        message = d.pop("message", UNSET)
-
-        message_model = cls(
-            message=message,
-        )
-
-        message_model.additional_properties = d
-        return message_model
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="MessageModel")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class MessageModel:
+    """
+    Attributes:
+        message (Union[Unset, str]):  Default: ''.
+    """
+
+    message: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        message = self.message
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if message is not UNSET:
+            field_dict["message"] = message
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        message = d.pop("message", UNSET)
+
+        message_model = cls(
+            message=message,
+        )
+
+        message_model.additional_properties = d
+        return message_model
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/name_input.py` & `PyOblv-0.2.1/oblv/models/name_input.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="NameInput")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class NameInput:
-    """
-    Attributes:
-        name (Union[Unset, str]):  Default: ''.
-    """
-
-    name: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if name is not UNSET:
-            field_dict["name"] = name
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        name = d.pop("name", UNSET)
-
-        name_input = cls(
-            name=name,
-        )
-
-        name_input.additional_properties = d
-        return name_input
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="NameInput")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class NameInput:
+    """
+    Attributes:
+        name (Union[Unset, str]):  Default: ''.
+    """
+
+    name: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        name = self.name
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if name is not UNSET:
+            field_dict["name"] = name
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        name = d.pop("name", UNSET)
+
+        name_input = cls(
+            name=name,
+        )
+
+        name_input.additional_properties = d
+        return name_input
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/notification_response.py` & `PyOblv-0.2.1/oblv/models/notification_response.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="NotificationResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class NotificationResponse:
-    """
-    Attributes:
-        id (Union[Unset, str]):  Default: ''.
-        summary (Union[Unset, str]):  Default: ''.
-        type (Union[Unset, str]):  Default: ''.
-        description (Union[Unset, str]):  Default: ''.
-        created_at (Union[Unset, str]):  Default: ''.
-        seen (Union[Unset, bool]):
-    """
-
-    id: Union[Unset, str] = ""
-    summary: Union[Unset, str] = ""
-    type: Union[Unset, str] = ""
-    description: Union[Unset, str] = ""
-    created_at: Union[Unset, str] = ""
-    seen: Union[Unset, bool] = False
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        summary = self.summary
-        type = self.type
-        description = self.description
-        created_at = self.created_at
-        seen = self.seen
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
-        if summary is not UNSET:
-            field_dict["summary"] = summary
-        if type is not UNSET:
-            field_dict["type"] = type
-        if description is not UNSET:
-            field_dict["description"] = description
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if seen is not UNSET:
-            field_dict["seen"] = seen
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
-
-        summary = d.pop("summary", UNSET)
-
-        type = d.pop("type", UNSET)
-
-        description = d.pop("description", UNSET)
-
-        created_at = d.pop("created_at", UNSET)
-
-        seen = d.pop("seen", UNSET)
-
-        notification_response = cls(
-            id=id,
-            summary=summary,
-            type=type,
-            description=description,
-            created_at=created_at,
-            seen=seen,
-        )
-
-        notification_response.additional_properties = d
-        return notification_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="NotificationResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class NotificationResponse:
+    """
+    Attributes:
+        id (Union[Unset, str]):  Default: ''.
+        summary (Union[Unset, str]):  Default: ''.
+        type (Union[Unset, str]):  Default: ''.
+        description (Union[Unset, str]):  Default: ''.
+        created_at (Union[Unset, str]):  Default: ''.
+        seen (Union[Unset, bool]):
+    """
+
+    id: Union[Unset, str] = ""
+    summary: Union[Unset, str] = ""
+    type: Union[Unset, str] = ""
+    description: Union[Unset, str] = ""
+    created_at: Union[Unset, str] = ""
+    seen: Union[Unset, bool] = False
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+        summary = self.summary
+        type = self.type
+        description = self.description
+        created_at = self.created_at
+        seen = self.seen
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if id is not UNSET:
+            field_dict["id"] = id
+        if summary is not UNSET:
+            field_dict["summary"] = summary
+        if type is not UNSET:
+            field_dict["type"] = type
+        if description is not UNSET:
+            field_dict["description"] = description
+        if created_at is not UNSET:
+            field_dict["created_at"] = created_at
+        if seen is not UNSET:
+            field_dict["seen"] = seen
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        id = d.pop("id", UNSET)
+
+        summary = d.pop("summary", UNSET)
+
+        type = d.pop("type", UNSET)
+
+        description = d.pop("description", UNSET)
+
+        created_at = d.pop("created_at", UNSET)
+
+        seen = d.pop("seen", UNSET)
+
+        notification_response = cls(
+            id=id,
+            summary=summary,
+            type=type,
+            description=description,
+            created_at=created_at,
+            seen=seen,
+        )
+
+        notification_response.additional_properties = d
+        return notification_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/oblv_auth_response.py` & `PyOblv-0.2.1/oblv/models/validated_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,88 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="OblvAuthResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class OblvAuthResponse:
-    """
-    Attributes:
-        token (Union[Unset, str]):  Default: ''.
-        user_id (Union[Unset, str]):  Default: ''.
-    """
-
-    token: Union[Unset, str] = ""
-    user_id: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        token = self.token
-        user_id = self.user_id
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if token is not UNSET:
-            field_dict["token"] = token
-        if user_id is not UNSET:
-            field_dict["user_id"] = user_id
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        token = d.pop("token", UNSET)
-
-        user_id = d.pop("user_id", UNSET)
-
-        oblv_auth_response = cls(
-            token=token,
-            user_id=user_id,
-        )
-
-        oblv_auth_response.additional_properties = d
-        return oblv_auth_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="ValidatedService")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class ValidatedService:
+    """
+    Attributes:
+        ref (Union[Unset, str]):  Default: ''.
+        service_validated (Union[Unset, bool]):  Default: True.
+        sha (Union[Unset, str]):  Default: ''.
+        type (Union[Unset, str]):  Default: ''.
+    """
+
+    ref: Union[Unset, str] = ""
+    service_validated: Union[Unset, bool] = True
+    sha: Union[Unset, str] = ""
+    type: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        ref = self.ref
+        service_validated = self.service_validated
+        sha = self.sha
+        type = self.type
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if ref is not UNSET:
+            field_dict["ref"] = ref
+        if service_validated is not UNSET:
+            field_dict["service_validated"] = service_validated
+        if sha is not UNSET:
+            field_dict["sha"] = sha
+        if type is not UNSET:
+            field_dict["type"] = type
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        ref = d.pop("ref", UNSET)
+
+        service_validated = d.pop("service_validated", UNSET)
+
+        sha = d.pop("sha", UNSET)
+
+        type = d.pop("type", UNSET)
+
+        validated_service = cls(
+            ref=ref,
+            service_validated=service_validated,
+            sha=sha,
+            type=type,
+        )
+
+        validated_service.additional_properties = d
+        return validated_service
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/psk.py` & `PyOblv-0.2.1/oblv/models/service_yaml_update_input.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,51 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="PSK")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class PSK:
-    """
-    Attributes:
-        public_key (str):
-    """
-
-    public_key: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        public_key = self.public_key
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "public_key": public_key,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        public_key = d.pop("public_key")
-
-        psk = cls(
-            public_key=public_key,
-        )
-
-        psk.additional_properties = d
-        return psk
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="ServiceYamlUpdateInput")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class ServiceYamlUpdateInput:
+    """ """
+
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        service_yaml_update_input = cls()
+
+        service_yaml_update_input.additional_properties = d
+        return service_yaml_update_input
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/ref_response.py` & `PyOblv-0.2.1/oblv/models/ref_response.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="RefResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class RefResponse:
-    """
-    Attributes:
-        tags (Union[Unset, List[str]]):
-        branch (Union[Unset, List[str]]):
-    """
-
-    tags: Union[Unset, List[str]] = UNSET
-    branch: Union[Unset, List[str]] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        tags: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.tags, Unset):
-            tags = self.tags
-
-        branch: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.branch, Unset):
-            branch = self.branch
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if tags is not UNSET:
-            field_dict["tags"] = tags
-        if branch is not UNSET:
-            field_dict["branch"] = branch
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        tags = cast(List[str], d.pop("tags", UNSET))
-
-        branch = cast(List[str], d.pop("branch", UNSET))
-
-        ref_response = cls(
-            tags=tags,
-            branch=branch,
-        )
-
-        ref_response.additional_properties = d
-        return ref_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="RefResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class RefResponse:
+    """
+    Attributes:
+        tags (Union[Unset, List[str]]):
+        branch (Union[Unset, List[str]]):
+    """
+
+    tags: Union[Unset, List[str]] = UNSET
+    branch: Union[Unset, List[str]] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        tags: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.tags, Unset):
+            tags = self.tags
+
+        branch: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.branch, Unset):
+            branch = self.branch
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if tags is not UNSET:
+            field_dict["tags"] = tags
+        if branch is not UNSET:
+            field_dict["branch"] = branch
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        tags = cast(List[str], d.pop("tags", UNSET))
+
+        branch = cast(List[str], d.pop("branch", UNSET))
+
+        ref_response = cls(
+            tags=tags,
+            branch=branch,
+        )
+
+        ref_response.additional_properties = d
+        return ref_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/repo.py` & `PyOblv-0.2.1/oblv/models/repo.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="Repo")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class Repo:
-    """
-    Attributes:
-        repo_id (Union[Unset, str]):  Default: ''.
-        name (Union[Unset, str]):  Default: ''.
-        full_name (Union[Unset, str]):  Default: ''.
-        is_private (Union[Unset, bool]):
-        owner_login (Union[Unset, str]):  Default: ''.
-        description (Union[Unset, str]):  Default: ''.
-        html_url (Union[Unset, str]):  Default: ''.
-        git_url (Union[Unset, str]):  Default: ''.
-        clone_url (Union[Unset, str]):  Default: ''.
-        default_branch (Union[Unset, str]):  Default: ''.
-        updated_at (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: 'github'.
-    """
-
-    repo_id: Union[Unset, str] = ""
-    name: Union[Unset, str] = ""
-    full_name: Union[Unset, str] = ""
-    is_private: Union[Unset, bool] = False
-    owner_login: Union[Unset, str] = ""
-    description: Union[Unset, str] = ""
-    html_url: Union[Unset, str] = ""
-    git_url: Union[Unset, str] = ""
-    clone_url: Union[Unset, str] = ""
-    default_branch: Union[Unset, str] = ""
-    updated_at: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = "github"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        repo_id = self.repo_id
-        name = self.name
-        full_name = self.full_name
-        is_private = self.is_private
-        owner_login = self.owner_login
-        description = self.description
-        html_url = self.html_url
-        git_url = self.git_url
-        clone_url = self.clone_url
-        default_branch = self.default_branch
-        updated_at = self.updated_at
-        account_type = self.account_type
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if repo_id is not UNSET:
-            field_dict["repo_id"] = repo_id
-        if name is not UNSET:
-            field_dict["name"] = name
-        if full_name is not UNSET:
-            field_dict["full_name"] = full_name
-        if is_private is not UNSET:
-            field_dict["is_private"] = is_private
-        if owner_login is not UNSET:
-            field_dict["owner_login"] = owner_login
-        if description is not UNSET:
-            field_dict["description"] = description
-        if html_url is not UNSET:
-            field_dict["html_url"] = html_url
-        if git_url is not UNSET:
-            field_dict["git_url"] = git_url
-        if clone_url is not UNSET:
-            field_dict["clone_url"] = clone_url
-        if default_branch is not UNSET:
-            field_dict["default_branch"] = default_branch
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        repo_id = d.pop("repo_id", UNSET)
-
-        name = d.pop("name", UNSET)
-
-        full_name = d.pop("full_name", UNSET)
-
-        is_private = d.pop("is_private", UNSET)
-
-        owner_login = d.pop("owner_login", UNSET)
-
-        description = d.pop("description", UNSET)
-
-        html_url = d.pop("html_url", UNSET)
-
-        git_url = d.pop("git_url", UNSET)
-
-        clone_url = d.pop("clone_url", UNSET)
-
-        default_branch = d.pop("default_branch", UNSET)
-
-        updated_at = d.pop("updated_at", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
-        repo = cls(
-            repo_id=repo_id,
-            name=name,
-            full_name=full_name,
-            is_private=is_private,
-            owner_login=owner_login,
-            description=description,
-            html_url=html_url,
-            git_url=git_url,
-            clone_url=clone_url,
-            default_branch=default_branch,
-            updated_at=updated_at,
-            account_type=account_type,
-        )
-
-        repo.additional_properties = d
-        return repo
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="Repo")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class Repo:
+    """
+    Attributes:
+        repo_id (Union[Unset, str]):  Default: ''.
+        name (Union[Unset, str]):  Default: ''.
+        full_name (Union[Unset, str]):  Default: ''.
+        is_private (Union[Unset, bool]):
+        owner_login (Union[Unset, str]):  Default: ''.
+        description (Union[Unset, str]):  Default: ''.
+        html_url (Union[Unset, str]):  Default: ''.
+        git_url (Union[Unset, str]):  Default: ''.
+        clone_url (Union[Unset, str]):  Default: ''.
+        default_branch (Union[Unset, str]):  Default: ''.
+        updated_at (Union[Unset, str]):  Default: ''.
+        account_type (Union[Unset, str]):  Default: 'github'.
+    """
+
+    repo_id: Union[Unset, str] = ""
+    name: Union[Unset, str] = ""
+    full_name: Union[Unset, str] = ""
+    is_private: Union[Unset, bool] = False
+    owner_login: Union[Unset, str] = ""
+    description: Union[Unset, str] = ""
+    html_url: Union[Unset, str] = ""
+    git_url: Union[Unset, str] = ""
+    clone_url: Union[Unset, str] = ""
+    default_branch: Union[Unset, str] = ""
+    updated_at: Union[Unset, str] = ""
+    account_type: Union[Unset, str] = "github"
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        repo_id = self.repo_id
+        name = self.name
+        full_name = self.full_name
+        is_private = self.is_private
+        owner_login = self.owner_login
+        description = self.description
+        html_url = self.html_url
+        git_url = self.git_url
+        clone_url = self.clone_url
+        default_branch = self.default_branch
+        updated_at = self.updated_at
+        account_type = self.account_type
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if repo_id is not UNSET:
+            field_dict["repo_id"] = repo_id
+        if name is not UNSET:
+            field_dict["name"] = name
+        if full_name is not UNSET:
+            field_dict["full_name"] = full_name
+        if is_private is not UNSET:
+            field_dict["is_private"] = is_private
+        if owner_login is not UNSET:
+            field_dict["owner_login"] = owner_login
+        if description is not UNSET:
+            field_dict["description"] = description
+        if html_url is not UNSET:
+            field_dict["html_url"] = html_url
+        if git_url is not UNSET:
+            field_dict["git_url"] = git_url
+        if clone_url is not UNSET:
+            field_dict["clone_url"] = clone_url
+        if default_branch is not UNSET:
+            field_dict["default_branch"] = default_branch
+        if updated_at is not UNSET:
+            field_dict["updated_at"] = updated_at
+        if account_type is not UNSET:
+            field_dict["account_type"] = account_type
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        repo_id = d.pop("repo_id", UNSET)
+
+        name = d.pop("name", UNSET)
+
+        full_name = d.pop("full_name", UNSET)
+
+        is_private = d.pop("is_private", UNSET)
+
+        owner_login = d.pop("owner_login", UNSET)
+
+        description = d.pop("description", UNSET)
+
+        html_url = d.pop("html_url", UNSET)
+
+        git_url = d.pop("git_url", UNSET)
+
+        clone_url = d.pop("clone_url", UNSET)
+
+        default_branch = d.pop("default_branch", UNSET)
+
+        updated_at = d.pop("updated_at", UNSET)
+
+        account_type = d.pop("account_type", UNSET)
+
+        repo = cls(
+            repo_id=repo_id,
+            name=name,
+            full_name=full_name,
+            is_private=is_private,
+            owner_login=owner_login,
+            description=description,
+            html_url=html_url,
+            git_url=git_url,
+            clone_url=clone_url,
+            default_branch=default_branch,
+            updated_at=updated_at,
+            account_type=account_type,
+        )
+
+        repo.additional_properties = d
+        return repo
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/repo_all_response.py` & `PyOblv-0.2.1/oblv/models/repo_all_response.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="RepoAllResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class RepoAllResponse:
-    """
-    Attributes:
-        name (Union[Unset, str]):  Default: ''.
-        owner_login (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: ''.
-    """
-
-    name: Union[Unset, str] = ""
-    owner_login: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        owner_login = self.owner_login
-        account_type = self.account_type
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if name is not UNSET:
-            field_dict["name"] = name
-        if owner_login is not UNSET:
-            field_dict["owner_login"] = owner_login
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        name = d.pop("name", UNSET)
-
-        owner_login = d.pop("owner_login", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
-        repo_all_response = cls(
-            name=name,
-            owner_login=owner_login,
-            account_type=account_type,
-        )
-
-        repo_all_response.additional_properties = d
-        return repo_all_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="RepoAllResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class RepoAllResponse:
+    """
+    Attributes:
+        name (Union[Unset, str]):  Default: ''.
+        owner_login (Union[Unset, str]):  Default: ''.
+        account_type (Union[Unset, str]):  Default: ''.
+    """
+
+    name: Union[Unset, str] = ""
+    owner_login: Union[Unset, str] = ""
+    account_type: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        name = self.name
+        owner_login = self.owner_login
+        account_type = self.account_type
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if name is not UNSET:
+            field_dict["name"] = name
+        if owner_login is not UNSET:
+            field_dict["owner_login"] = owner_login
+        if account_type is not UNSET:
+            field_dict["account_type"] = account_type
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        name = d.pop("name", UNSET)
+
+        owner_login = d.pop("owner_login", UNSET)
+
+        account_type = d.pop("account_type", UNSET)
+
+        repo_all_response = cls(
+            name=name,
+            owner_login=owner_login,
+            account_type=account_type,
+        )
+
+        repo_all_response.additional_properties = d
+        return repo_all_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/repo_service_list.py` & `PyOblv-0.2.1/oblv/models/repo_service_list.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-from ..models.validated_service import ValidatedService
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="RepoServiceList")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class RepoServiceList:
-    """
-    Attributes:
-        total_pages (int):
-        services (List[ValidatedService]):
-    """
-
-    total_pages: int
-    services: List[ValidatedService]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        total_pages = self.total_pages
-        services = []
-        for services_item_data in self.services:
-            services_item = services_item_data.to_dict()
-
-            services.append(services_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "total_pages": total_pages,
-                "services": services,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        total_pages = d.pop("total_pages")
-
-        services = []
-        _services = d.pop("services")
-        for services_item_data in _services:
-            services_item = ValidatedService.from_dict(services_item_data)
-
-            services.append(services_item)
-
-        repo_services_list = cls(
-            total_pages=total_pages,
-            services=services,
-        )
-
-        repo_services_list.additional_properties = d
-        return repo_services_list
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+from ..models.validated_service import ValidatedService
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="RepoServiceList")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class RepoServiceList:
+    """
+    Attributes:
+        total_pages (int):
+        services (List[ValidatedService]):
+    """
+
+    total_pages: int
+    services: List[ValidatedService]
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        total_pages = self.total_pages
+        services = []
+        for services_item_data in self.services:
+            services_item = services_item_data.to_dict()
+
+            services.append(services_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "total_pages": total_pages,
+                "services": services,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        total_pages = d.pop("total_pages")
+
+        services = []
+        _services = d.pop("services")
+        for services_item_data in _services:
+            services_item = ValidatedService.from_dict(services_item_data)
+
+            services.append(services_item)
+
+        repo_services_list = cls(
+            total_pages=total_pages,
+            services=services,
+        )
+
+        repo_services_list.additional_properties = d
+        return repo_services_list
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/repo_services.py` & `PyOblv-0.2.1/oblv/models/repo_services.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..models.validated_service import ValidatedService
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="RepoServices")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class RepoServices:
-    """
-    Attributes:
-        repo_id (Union[Unset, str]):  Default: ''.
-        name (Union[Unset, str]):  Default: ''.
-        full_name (Union[Unset, str]):  Default: ''.
-        is_private (Union[Unset, bool]):
-        owner_login (Union[Unset, str]):  Default: ''.
-        description (Union[Unset, str]):  Default: ''.
-        html_url (Union[Unset, str]):  Default: ''.
-        git_url (Union[Unset, str]):  Default: ''.
-        clone_url (Union[Unset, str]):  Default: ''.
-        default_branch (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: 'github'.
-        services (Union[Unset, List[ValidatedService]]):
-    """
-
-    repo_id: Union[Unset, str] = ""
-    name: Union[Unset, str] = ""
-    full_name: Union[Unset, str] = ""
-    is_private: Union[Unset, bool] = False
-    owner_login: Union[Unset, str] = ""
-    description: Union[Unset, str] = ""
-    html_url: Union[Unset, str] = ""
-    git_url: Union[Unset, str] = ""
-    clone_url: Union[Unset, str] = ""
-    default_branch: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = "github"
-    services: Union[Unset, List[ValidatedService]] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        repo_id = self.repo_id
-        name = self.name
-        full_name = self.full_name
-        is_private = self.is_private
-        owner_login = self.owner_login
-        description = self.description
-        html_url = self.html_url
-        git_url = self.git_url
-        clone_url = self.clone_url
-        default_branch = self.default_branch
-        account_type = self.account_type
-        services: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.services, Unset):
-            services = []
-            for services_item_data in self.services:
-                services_item = services_item_data.to_dict()
-
-                services.append(services_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if repo_id is not UNSET:
-            field_dict["repo_id"] = repo_id
-        if name is not UNSET:
-            field_dict["name"] = name
-        if full_name is not UNSET:
-            field_dict["full_name"] = full_name
-        if is_private is not UNSET:
-            field_dict["is_private"] = is_private
-        if owner_login is not UNSET:
-            field_dict["owner_login"] = owner_login
-        if description is not UNSET:
-            field_dict["description"] = description
-        if html_url is not UNSET:
-            field_dict["html_url"] = html_url
-        if git_url is not UNSET:
-            field_dict["git_url"] = git_url
-        if clone_url is not UNSET:
-            field_dict["clone_url"] = clone_url
-        if default_branch is not UNSET:
-            field_dict["default_branch"] = default_branch
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
-        if services is not UNSET:
-            field_dict["services"] = services
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        repo_id = d.pop("repo_id", UNSET)
-
-        name = d.pop("name", UNSET)
-
-        full_name = d.pop("full_name", UNSET)
-
-        is_private = d.pop("is_private", UNSET)
-
-        owner_login = d.pop("owner_login", UNSET)
-
-        description = d.pop("description", UNSET)
-
-        html_url = d.pop("html_url", UNSET)
-
-        git_url = d.pop("git_url", UNSET)
-
-        clone_url = d.pop("clone_url", UNSET)
-
-        default_branch = d.pop("default_branch", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
-        services = []
-        _services = d.pop("services", UNSET)
-        for services_item_data in _services or []:
-            services_item = ValidatedService.from_dict(services_item_data)
-
-            services.append(services_item)
-
-        repo_services = cls(
-            repo_id=repo_id,
-            name=name,
-            full_name=full_name,
-            is_private=is_private,
-            owner_login=owner_login,
-            description=description,
-            html_url=html_url,
-            git_url=git_url,
-            clone_url=clone_url,
-            default_branch=default_branch,
-            account_type=account_type,
-            services=services,
-        )
-
-        repo_services.additional_properties = d
-        return repo_services
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..models.validated_service import ValidatedService
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="RepoServices")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class RepoServices:
+    """
+    Attributes:
+        repo_id (Union[Unset, str]):  Default: ''.
+        name (Union[Unset, str]):  Default: ''.
+        full_name (Union[Unset, str]):  Default: ''.
+        is_private (Union[Unset, bool]):
+        owner_login (Union[Unset, str]):  Default: ''.
+        description (Union[Unset, str]):  Default: ''.
+        html_url (Union[Unset, str]):  Default: ''.
+        git_url (Union[Unset, str]):  Default: ''.
+        clone_url (Union[Unset, str]):  Default: ''.
+        default_branch (Union[Unset, str]):  Default: ''.
+        account_type (Union[Unset, str]):  Default: 'github'.
+        services (Union[Unset, List[ValidatedService]]):
+    """
+
+    repo_id: Union[Unset, str] = ""
+    name: Union[Unset, str] = ""
+    full_name: Union[Unset, str] = ""
+    is_private: Union[Unset, bool] = False
+    owner_login: Union[Unset, str] = ""
+    description: Union[Unset, str] = ""
+    html_url: Union[Unset, str] = ""
+    git_url: Union[Unset, str] = ""
+    clone_url: Union[Unset, str] = ""
+    default_branch: Union[Unset, str] = ""
+    account_type: Union[Unset, str] = "github"
+    services: Union[Unset, List[ValidatedService]] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        repo_id = self.repo_id
+        name = self.name
+        full_name = self.full_name
+        is_private = self.is_private
+        owner_login = self.owner_login
+        description = self.description
+        html_url = self.html_url
+        git_url = self.git_url
+        clone_url = self.clone_url
+        default_branch = self.default_branch
+        account_type = self.account_type
+        services: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.services, Unset):
+            services = []
+            for services_item_data in self.services:
+                services_item = services_item_data.to_dict()
+
+                services.append(services_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if repo_id is not UNSET:
+            field_dict["repo_id"] = repo_id
+        if name is not UNSET:
+            field_dict["name"] = name
+        if full_name is not UNSET:
+            field_dict["full_name"] = full_name
+        if is_private is not UNSET:
+            field_dict["is_private"] = is_private
+        if owner_login is not UNSET:
+            field_dict["owner_login"] = owner_login
+        if description is not UNSET:
+            field_dict["description"] = description
+        if html_url is not UNSET:
+            field_dict["html_url"] = html_url
+        if git_url is not UNSET:
+            field_dict["git_url"] = git_url
+        if clone_url is not UNSET:
+            field_dict["clone_url"] = clone_url
+        if default_branch is not UNSET:
+            field_dict["default_branch"] = default_branch
+        if account_type is not UNSET:
+            field_dict["account_type"] = account_type
+        if services is not UNSET:
+            field_dict["services"] = services
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        repo_id = d.pop("repo_id", UNSET)
+
+        name = d.pop("name", UNSET)
+
+        full_name = d.pop("full_name", UNSET)
+
+        is_private = d.pop("is_private", UNSET)
+
+        owner_login = d.pop("owner_login", UNSET)
+
+        description = d.pop("description", UNSET)
+
+        html_url = d.pop("html_url", UNSET)
+
+        git_url = d.pop("git_url", UNSET)
+
+        clone_url = d.pop("clone_url", UNSET)
+
+        default_branch = d.pop("default_branch", UNSET)
+
+        account_type = d.pop("account_type", UNSET)
+
+        services = []
+        _services = d.pop("services", UNSET)
+        for services_item_data in _services or []:
+            services_item = ValidatedService.from_dict(services_item_data)
+
+            services.append(services_item)
+
+        repo_services = cls(
+            repo_id=repo_id,
+            name=name,
+            full_name=full_name,
+            is_private=is_private,
+            owner_login=owner_login,
+            description=description,
+            html_url=html_url,
+            git_url=git_url,
+            clone_url=clone_url,
+            default_branch=default_branch,
+            account_type=account_type,
+            services=services,
+        )
+
+        repo_services.additional_properties = d
+        return repo_services
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/role_response.py` & `PyOblv-0.2.1/oblv/models/role_response.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="RoleResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class RoleResponse:
-    """
-    Attributes:
-        role_name (Union[Unset, str]):  Default: ''.
-        role_description (Union[Unset, str]):  Default: ''.
-    """
-
-    role_name: Union[Unset, str] = ""
-    role_description: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        role_name = self.role_name
-        role_description = self.role_description
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if role_name is not UNSET:
-            field_dict["role_name"] = role_name
-        if role_description is not UNSET:
-            field_dict["role_description"] = role_description
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        role_name = d.pop("role_name", UNSET)
-
-        role_description = d.pop("role_description", UNSET)
-
-        role_response = cls(
-            role_name=role_name,
-            role_description=role_description,
-        )
-
-        role_response.additional_properties = d
-        return role_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="RoleResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class RoleResponse:
+    """
+    Attributes:
+        role_name (Union[Unset, str]):  Default: ''.
+        role_description (Union[Unset, str]):  Default: ''.
+    """
+
+    role_name: Union[Unset, str] = ""
+    role_description: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        role_name = self.role_name
+        role_description = self.role_description
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if role_name is not UNSET:
+            field_dict["role_name"] = role_name
+        if role_description is not UNSET:
+            field_dict["role_description"] = role_description
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        role_name = d.pop("role_name", UNSET)
+
+        role_description = d.pop("role_description", UNSET)
+
+        role_response = cls(
+            role_name=role_name,
+            role_description=role_description,
+        )
+
+        role_response.additional_properties = d
+        return role_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/service_content_response.py` & `PyOblv-0.2.1/oblv/models/service_content_response.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="ServiceContentResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class ServiceContentResponse:
-    """ """
-
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        service_content_response = cls()
-
-        service_content_response.additional_properties = d
-        return service_content_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="ServiceContentResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class ServiceContentResponse:
+    """ """
+
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        service_content_response = cls()
+
+        service_content_response.additional_properties = d
+        return service_content_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/service_validation_response.py` & `PyOblv-0.2.1/oblv/models/service_validation_response.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..models.validated_service import ValidatedService
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="ServiceValidationResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class ServiceValidationResponse:
-    """
-    Attributes:
-        message (Union[Unset, str]):  Default: ''.
-        service (Union[Unset, ValidatedService]):
-    """
-
-    message: Union[Unset, str] = ""
-    service: Union[Unset, ValidatedService] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        message = self.message
-        service: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.service, Unset):
-            service = self.service.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if message is not UNSET:
-            field_dict["message"] = message
-        if service is not UNSET:
-            field_dict["service"] = service
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        message = d.pop("message", UNSET)
-
-        _service = d.pop("service", UNSET)
-        service: Union[Unset, ValidatedService]
-        if isinstance(_service, Unset):
-            service = UNSET
-        else:
-            service = ValidatedService.from_dict(_service)
-
-        service_validation_response = cls(
-            message=message,
-            service=service,
-        )
-
-        service_validation_response.additional_properties = d
-        return service_validation_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..models.validated_service import ValidatedService
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="ServiceValidationResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class ServiceValidationResponse:
+    """
+    Attributes:
+        message (Union[Unset, str]):  Default: ''.
+        service (Union[Unset, ValidatedService]):
+    """
+
+    message: Union[Unset, str] = ""
+    service: Union[Unset, ValidatedService] = UNSET
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        message = self.message
+        service: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.service, Unset):
+            service = self.service.to_dict()
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if message is not UNSET:
+            field_dict["message"] = message
+        if service is not UNSET:
+            field_dict["service"] = service
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        message = d.pop("message", UNSET)
+
+        _service = d.pop("service", UNSET)
+        service: Union[Unset, ValidatedService]
+        if isinstance(_service, Unset):
+            service = UNSET
+        else:
+            service = ValidatedService.from_dict(_service)
+
+        service_validation_response = cls(
+            message=message,
+            service=service,
+        )
+
+        service_validation_response.additional_properties = d
+        return service_validation_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/service_yaml_add_input.py` & `PyOblv-0.2.1/oblv/models/service_yaml_add_input.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="ServiceYamlAddInput")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class ServiceYamlAddInput:
-    """ """
-
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        service_yaml_add_input = cls()
-
-        service_yaml_add_input.additional_properties = d
-        return service_yaml_add_input
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="ServiceYamlAddInput")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class ServiceYamlAddInput:
+    """ """
+
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        service_yaml_add_input = cls()
+
+        service_yaml_add_input.additional_properties = d
+        return service_yaml_add_input
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/service_yaml_update_input.py` & `PyOblv-0.2.1/oblv/models/supported_regions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="ServiceYamlUpdateInput")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class ServiceYamlUpdateInput:
-    """ """
-
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        service_yaml_update_input = cls()
-
-        service_yaml_update_input.additional_properties = d
-        return service_yaml_update_input
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="SupportedRegions")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class SupportedRegions:
+    """ """
+
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        supported_regions = cls()
+
+        supported_regions.additional_properties = d
+        return supported_regions
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/shared_users.py` & `PyOblv-0.2.1/oblv/models/shared_users.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="SharedUsers")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class SharedUsers:
-    """
-    Attributes:
-        role (List[str]):
-        oblivious_user_id (Union[Unset, str]):  Default: ''.
-        use_case (Union[Unset, str]):  Default: ''.
-        oblivious_login (Union[Unset, str]):  Default: ''.
-    """
-
-    role: List[str]
-    oblivious_user_id: Union[Unset, str] = ""
-    use_case: Union[Unset, str] = ""
-    oblivious_login: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        role = self.role
-
-        oblivious_user_id = self.oblivious_user_id
-        use_case = self.use_case
-        oblivious_login = self.oblivious_login
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "role": role,
-            }
-        )
-        if oblivious_user_id is not UNSET:
-            field_dict["oblivious_user_id"] = oblivious_user_id
-        if use_case is not UNSET:
-            field_dict["use_case"] = use_case
-        if oblivious_login is not UNSET:
-            field_dict["oblivious_login"] = oblivious_login
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        role = cast(List[str], d.pop("role"))
-
-        oblivious_user_id = d.pop("oblivious_user_id", UNSET)
-
-        use_case = d.pop("use_case", UNSET)
-
-        oblivious_login = d.pop("oblivious_login", UNSET)
-
-        shared_users = cls(
-            role=role,
-            oblivious_user_id=oblivious_user_id,
-            use_case=use_case,
-            oblivious_login=oblivious_login,
-        )
-
-        shared_users.additional_properties = d
-        return shared_users
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="SharedUsers")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class SharedUsers:
+    """
+    Attributes:
+        role (List[str]):
+        oblivious_user_id (Union[Unset, str]):  Default: ''.
+        use_case (Union[Unset, str]):  Default: ''.
+        oblivious_login (Union[Unset, str]):  Default: ''.
+    """
+
+    role: List[str]
+    oblivious_user_id: Union[Unset, str] = ""
+    use_case: Union[Unset, str] = ""
+    oblivious_login: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        role = self.role
+
+        oblivious_user_id = self.oblivious_user_id
+        use_case = self.use_case
+        oblivious_login = self.oblivious_login
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "role": role,
+            }
+        )
+        if oblivious_user_id is not UNSET:
+            field_dict["oblivious_user_id"] = oblivious_user_id
+        if use_case is not UNSET:
+            field_dict["use_case"] = use_case
+        if oblivious_login is not UNSET:
+            field_dict["oblivious_login"] = oblivious_login
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        role = cast(List[str], d.pop("role"))
+
+        oblivious_user_id = d.pop("oblivious_user_id", UNSET)
+
+        use_case = d.pop("use_case", UNSET)
+
+        oblivious_login = d.pop("oblivious_login", UNSET)
+
+        shared_users = cls(
+            role=role,
+            oblivious_user_id=oblivious_user_id,
+            use_case=use_case,
+            oblivious_login=oblivious_login,
+        )
+
+        shared_users.additional_properties = d
+        return shared_users
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/user_credit_utilization.py` & `PyOblv-0.2.1/oblv/models/user_credit_utilization.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UserCreditUtilization")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class UserCreditUtilization:
-    """
-    Attributes:
-        total_credits (Union[Unset, int]):
-        total_running_deployments (Union[Unset, int]):
-        esitmated_hours_remaining (Union[Unset, int]):
-        hourly_credit_utilization (Union[Unset, int]):
-    """
-
-    total_credits: Union[Unset, int] = 0
-    total_running_deployments: Union[Unset, int] = 0
-    esitmated_hours_remaining: Union[Unset, int] = 0
-    hourly_credit_utilization: Union[Unset, int] = 0
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        total_credits = self.total_credits
-        total_running_deployments = self.total_running_deployments
-        esitmated_hours_remaining = self.esitmated_hours_remaining
-        hourly_credit_utilization = self.hourly_credit_utilization
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if total_credits is not UNSET:
-            field_dict["total_credits"] = total_credits
-        if total_running_deployments is not UNSET:
-            field_dict["total_running_deployments"] = total_running_deployments
-        if esitmated_hours_remaining is not UNSET:
-            field_dict["esitmated_hours_remaining"] = esitmated_hours_remaining
-        if hourly_credit_utilization is not UNSET:
-            field_dict["hourly_credit_utilization"] = hourly_credit_utilization
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        total_credits = d.pop("total_credits", UNSET)
-
-        total_running_deployments = d.pop("total_running_deployments", UNSET)
-
-        esitmated_hours_remaining = d.pop("esitmated_hours_remaining", UNSET)
-
-        hourly_credit_utilization = d.pop("hourly_credit_utilization", UNSET)
-
-        user_credit_utilization = cls(
-            total_credits=total_credits,
-            total_running_deployments=total_running_deployments,
-            esitmated_hours_remaining=esitmated_hours_remaining,
-            hourly_credit_utilization=hourly_credit_utilization,
-        )
-
-        user_credit_utilization.additional_properties = d
-        return user_credit_utilization
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="UserCreditUtilization")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class UserCreditUtilization:
+    """
+    Attributes:
+        total_credits (Union[Unset, int]):
+        total_running_deployments (Union[Unset, int]):
+        esitmated_hours_remaining (Union[Unset, int]):
+        hourly_credit_utilization (Union[Unset, int]):
+    """
+
+    total_credits: Union[Unset, int] = 0
+    total_running_deployments: Union[Unset, int] = 0
+    esitmated_hours_remaining: Union[Unset, int] = 0
+    hourly_credit_utilization: Union[Unset, int] = 0
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        total_credits = self.total_credits
+        total_running_deployments = self.total_running_deployments
+        esitmated_hours_remaining = self.esitmated_hours_remaining
+        hourly_credit_utilization = self.hourly_credit_utilization
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if total_credits is not UNSET:
+            field_dict["total_credits"] = total_credits
+        if total_running_deployments is not UNSET:
+            field_dict["total_running_deployments"] = total_running_deployments
+        if esitmated_hours_remaining is not UNSET:
+            field_dict["esitmated_hours_remaining"] = esitmated_hours_remaining
+        if hourly_credit_utilization is not UNSET:
+            field_dict["hourly_credit_utilization"] = hourly_credit_utilization
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        total_credits = d.pop("total_credits", UNSET)
+
+        total_running_deployments = d.pop("total_running_deployments", UNSET)
+
+        esitmated_hours_remaining = d.pop("esitmated_hours_remaining", UNSET)
+
+        hourly_credit_utilization = d.pop("hourly_credit_utilization", UNSET)
+
+        user_credit_utilization = cls(
+            total_credits=total_credits,
+            total_running_deployments=total_running_deployments,
+            esitmated_hours_remaining=esitmated_hours_remaining,
+            hourly_credit_utilization=hourly_credit_utilization,
+        )
+
+        user_credit_utilization.additional_properties = d
+        return user_credit_utilization
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/user_password_input.py` & `PyOblv-0.2.1/oblv/models/user_password_input.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-T = TypeVar("T", bound="UserPasswordInput")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class UserPasswordInput:
-    """
-    Attributes:
-        old_password (str):
-        password (str):
-    """
-
-    old_password: str
-    password: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        old_password = self.old_password
-        password = self.password
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "old_password": old_password,
-                "password": password,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        old_password = d.pop("old_password")
-
-        password = d.pop("password")
-
-        user_password_input = cls(
-            old_password=old_password,
-            password=password,
-        )
-
-        user_password_input.additional_properties = d
-        return user_password_input
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+T = TypeVar("T", bound="UserPasswordInput")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class UserPasswordInput:
+    """
+    Attributes:
+        old_password (str):
+        password (str):
+    """
+
+    old_password: str
+    password: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        old_password = self.old_password
+        password = self.password
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "old_password": old_password,
+                "password": password,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        old_password = d.pop("old_password")
+
+        password = d.pop("password")
+
+        user_password_input = cls(
+            old_password=old_password,
+            password=password,
+        )
+
+        user_password_input.additional_properties = d
+        return user_password_input
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/user_profile_response.py` & `PyOblv-0.2.1/oblv/models/user_profile_response.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UserProfileResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class UserProfileResponse:
-    """
-    Attributes:
-        oblivious_login (Union[Unset, str]):  Default: ''.
-        email (Union[Unset, str]):  Default: ''.
-        user_name (Union[Unset, str]):  Default: ''.
-        public_key (Union[Unset, str]):  Default: ''.
-    """
-
-    oblivious_login: Union[Unset, str] = ""
-    email: Union[Unset, str] = ""
-    user_name: Union[Unset, str] = ""
-    public_key: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        oblivious_login = self.oblivious_login
-        email = self.email
-        user_name = self.user_name
-        public_key = self.public_key
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if oblivious_login is not UNSET:
-            field_dict["oblivious_login"] = oblivious_login
-        if email is not UNSET:
-            field_dict["email"] = email
-        if user_name is not UNSET:
-            field_dict["user_name"] = user_name
-        if public_key is not UNSET:
-            field_dict["public_key"] = public_key
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        oblivious_login = d.pop("oblivious_login", UNSET)
-
-        email = d.pop("email", UNSET)
-
-        user_name = d.pop("user_name", UNSET)
-
-        public_key = d.pop("public_key", UNSET)
-
-        user_profile_response = cls(
-            oblivious_login=oblivious_login,
-            email=email,
-            user_name=user_name,
-            public_key=public_key,
-        )
-
-        user_profile_response.additional_properties = d
-        return user_profile_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="UserProfileResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class UserProfileResponse:
+    """
+    Attributes:
+        oblivious_login (Union[Unset, str]):  Default: ''.
+        email (Union[Unset, str]):  Default: ''.
+        user_name (Union[Unset, str]):  Default: ''.
+        public_key (Union[Unset, str]):  Default: ''.
+    """
+
+    oblivious_login: Union[Unset, str] = ""
+    email: Union[Unset, str] = ""
+    user_name: Union[Unset, str] = ""
+    public_key: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        oblivious_login = self.oblivious_login
+        email = self.email
+        user_name = self.user_name
+        public_key = self.public_key
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if oblivious_login is not UNSET:
+            field_dict["oblivious_login"] = oblivious_login
+        if email is not UNSET:
+            field_dict["email"] = email
+        if user_name is not UNSET:
+            field_dict["user_name"] = user_name
+        if public_key is not UNSET:
+            field_dict["public_key"] = public_key
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        oblivious_login = d.pop("oblivious_login", UNSET)
+
+        email = d.pop("email", UNSET)
+
+        user_name = d.pop("user_name", UNSET)
+
+        public_key = d.pop("public_key", UNSET)
+
+        user_profile_response = cls(
+            oblivious_login=oblivious_login,
+            email=email,
+            user_name=user_name,
+            public_key=public_key,
+        )
+
+        user_profile_response.additional_properties = d
+        return user_profile_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/user_service_list.py` & `PyOblv-0.2.1/oblv/models/user_service_list.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar
-
-import attr
-
-from .user_services import UserServices
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UserServiceList")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class UserServiceList:
-    """
-    Attributes:
-        total_pages (int):
-        services (List[UserServices]):
-    """
-
-    total_pages: int
-    services: List[UserServices]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        total_pages = self.total_pages
-        services = []
-        for services_item_data in self.services:
-            services_item = services_item_data.to_dict()
-
-            services.append(services_item)
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "total_pages": total_pages,
-                "services": services,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        total_pages = d.pop("total_pages")
-
-        services = []
-        _services = d.pop("services")
-        for services_item_data in _services:
-            services_item = UserServices.from_dict(services_item_data)
-
-            services.append(services_item)
-
-        user_services_list = cls(
-            total_pages=total_pages,
-            services=services,
-        )
-
-        user_services_list.additional_properties = d
-        return user_services_list
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar
+
+import attr
+
+from .user_services import UserServices
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="UserServiceList")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class UserServiceList:
+    """
+    Attributes:
+        total_pages (int):
+        services (List[UserServices]):
+    """
+
+    total_pages: int
+    services: List[UserServices]
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        total_pages = self.total_pages
+        services = []
+        for services_item_data in self.services:
+            services_item = services_item_data.to_dict()
+
+            services.append(services_item)
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "total_pages": total_pages,
+                "services": services,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        total_pages = d.pop("total_pages")
+
+        services = []
+        _services = d.pop("services")
+        for services_item_data in _services:
+            services_item = UserServices.from_dict(services_item_data)
+
+            services.append(services_item)
+
+        user_services_list = cls(
+            total_pages=total_pages,
+            services=services,
+        )
+
+        user_services_list.additional_properties = d
+        return user_services_list
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/user_services.py` & `PyOblv-0.2.1/oblv/models/user_services.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UserServices")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class UserServices:
-    """
-    Attributes:
-        repo_name (Union[Unset, str]):  Default: ''.
-        repo_owner (Union[Unset, str]):  Default: ''.
-        account_type (Union[Unset, str]):  Default: ''.
-        ref (Union[Unset, str]):  Default: ''.
-        service_validated (Union[Unset, bool]):
-        sha (Union[Unset, str]):  Default: ''.
-        type (Union[Unset, str]):  Default: ''.
-    """
-
-    repo_name: Union[Unset, str] = ""
-    repo_owner: Union[Unset, str] = ""
-    account_type: Union[Unset, str] = ""
-    ref: Union[Unset, str] = ""
-    service_validated: Union[Unset, bool] = False
-    sha: Union[Unset, str] = ""
-    type: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        repo_name = self.repo_name
-        repo_owner = self.repo_owner
-        account_type = self.account_type
-        ref = self.ref
-        service_validated = self.service_validated
-        sha = self.sha
-        type = self.type
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if repo_name is not UNSET:
-            field_dict["repo_name"] = repo_name
-        if repo_owner is not UNSET:
-            field_dict["repo_owner"] = repo_owner
-        if account_type is not UNSET:
-            field_dict["account_type"] = account_type
-        if ref is not UNSET:
-            field_dict["ref"] = ref
-        if service_validated is not UNSET:
-            field_dict["service_validated"] = service_validated
-        if sha is not UNSET:
-            field_dict["sha"] = sha
-        if type is not UNSET:
-            field_dict["type"] = type
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        repo_name = d.pop("repo_name", UNSET)
-
-        repo_owner = d.pop("repo_owner", UNSET)
-
-        account_type = d.pop("account_type", UNSET)
-
-        ref = d.pop("ref", UNSET)
-
-        service_validated = d.pop("service_validated", UNSET)
-
-        sha = d.pop("sha", UNSET)
-
-        type = d.pop("type", UNSET)
-
-        user_services = cls(
-            repo_name=repo_name,
-            repo_owner=repo_owner,
-            account_type=account_type,
-            ref=ref,
-            service_validated=service_validated,
-            sha=sha,
-            type=type,
-        )
-
-        user_services.additional_properties = d
-        return user_services
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="UserServices")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class UserServices:
+    """
+    Attributes:
+        repo_name (Union[Unset, str]):  Default: ''.
+        repo_owner (Union[Unset, str]):  Default: ''.
+        account_type (Union[Unset, str]):  Default: ''.
+        ref (Union[Unset, str]):  Default: ''.
+        service_validated (Union[Unset, bool]):
+        sha (Union[Unset, str]):  Default: ''.
+        type (Union[Unset, str]):  Default: ''.
+    """
+
+    repo_name: Union[Unset, str] = ""
+    repo_owner: Union[Unset, str] = ""
+    account_type: Union[Unset, str] = ""
+    ref: Union[Unset, str] = ""
+    service_validated: Union[Unset, bool] = False
+    sha: Union[Unset, str] = ""
+    type: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        repo_name = self.repo_name
+        repo_owner = self.repo_owner
+        account_type = self.account_type
+        ref = self.ref
+        service_validated = self.service_validated
+        sha = self.sha
+        type = self.type
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if repo_name is not UNSET:
+            field_dict["repo_name"] = repo_name
+        if repo_owner is not UNSET:
+            field_dict["repo_owner"] = repo_owner
+        if account_type is not UNSET:
+            field_dict["account_type"] = account_type
+        if ref is not UNSET:
+            field_dict["ref"] = ref
+        if service_validated is not UNSET:
+            field_dict["service_validated"] = service_validated
+        if sha is not UNSET:
+            field_dict["sha"] = sha
+        if type is not UNSET:
+            field_dict["type"] = type
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        repo_name = d.pop("repo_name", UNSET)
+
+        repo_owner = d.pop("repo_owner", UNSET)
+
+        account_type = d.pop("account_type", UNSET)
+
+        ref = d.pop("ref", UNSET)
+
+        service_validated = d.pop("service_validated", UNSET)
+
+        sha = d.pop("sha", UNSET)
+
+        type = d.pop("type", UNSET)
+
+        user_services = cls(
+            repo_name=repo_name,
+            repo_owner=repo_owner,
+            account_type=account_type,
+            ref=ref,
+            service_validated=service_validated,
+            sha=sha,
+            type=type,
+        )
+
+        user_services.additional_properties = d
+        return user_services
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/validated_service.py` & `PyOblv-0.2.1/oblv/models/oblv_auth_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,72 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="ValidatedService")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class ValidatedService:
-    """
-    Attributes:
-        ref (Union[Unset, str]):  Default: ''.
-        service_validated (Union[Unset, bool]):  Default: True.
-        sha (Union[Unset, str]):  Default: ''.
-        type (Union[Unset, str]):  Default: ''.
-    """
-
-    ref: Union[Unset, str] = ""
-    service_validated: Union[Unset, bool] = True
-    sha: Union[Unset, str] = ""
-    type: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        ref = self.ref
-        service_validated = self.service_validated
-        sha = self.sha
-        type = self.type
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if ref is not UNSET:
-            field_dict["ref"] = ref
-        if service_validated is not UNSET:
-            field_dict["service_validated"] = service_validated
-        if sha is not UNSET:
-            field_dict["sha"] = sha
-        if type is not UNSET:
-            field_dict["type"] = type
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        ref = d.pop("ref", UNSET)
-
-        service_validated = d.pop("service_validated", UNSET)
-
-        sha = d.pop("sha", UNSET)
-
-        type = d.pop("type", UNSET)
-
-        validated_service = cls(
-            ref=ref,
-            service_validated=service_validated,
-            sha=sha,
-            type=type,
-        )
-
-        validated_service.additional_properties = d
-        return validated_service
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="OblvAuthResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class OblvAuthResponse:
+    """
+    Attributes:
+        token (Union[Unset, str]):  Default: ''.
+        user_id (Union[Unset, str]):  Default: ''.
+    """
+
+    token: Union[Unset, str] = ""
+    user_id: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        token = self.token
+        user_id = self.user_id
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if token is not UNSET:
+            field_dict["token"] = token
+        if user_id is not UNSET:
+            field_dict["user_id"] = user_id
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        token = d.pop("token", UNSET)
+
+        user_id = d.pop("user_id", UNSET)
+
+        oblv_auth_response = cls(
+            token=token,
+            user_id=user_id,
+        )
+
+        oblv_auth_response.additional_properties = d
+        return oblv_auth_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/validation_error.py` & `PyOblv-0.2.1/oblv/models/validation_error.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, cast
-
-import attr
-
-T = TypeVar("T", bound="ValidationError")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class ValidationError:
-    """
-    Attributes:
-        loc (List[str]):
-        msg (str):
-        type (str):
-    """
-
-    loc: List[str]
-    msg: str
-    type: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        loc = self.loc
-
-        msg = self.msg
-        type = self.type
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "loc": loc,
-                "msg": msg,
-                "type": type,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        loc = cast(List[str], d.pop("loc"))
-
-        msg = d.pop("msg")
-
-        type = d.pop("type")
-
-        validation_error = cls(
-            loc=loc,
-            msg=msg,
-            type=type,
-        )
-
-        validation_error.additional_properties = d
-        return validation_error
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, cast
+
+import attr
+
+T = TypeVar("T", bound="ValidationError")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class ValidationError:
+    """
+    Attributes:
+        loc (List[str]):
+        msg (str):
+        type (str):
+    """
+
+    loc: List[str]
+    msg: str
+    type: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        loc = self.loc
+
+        msg = self.msg
+        type = self.type
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "loc": loc,
+                "msg": msg,
+                "type": type,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        loc = cast(List[str], d.pop("loc"))
+
+        msg = d.pop("msg")
+
+        type = d.pop("type")
+
+        validation_error = cls(
+            loc=loc,
+            msg=msg,
+            type=type,
+        )
+
+        validation_error.additional_properties = d
+        return validation_error
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/models/vcs_repo_response.py` & `PyOblv-0.2.1/oblv/models/vcs_repo_response.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import json
-from typing import Any, Dict, List, Type, TypeVar, Union
-
-import attr
-
-from ..models.repo import Repo
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="VCSRepoResponse")
-
-
-@attr.s(auto_attribs=True, repr=False)
-class VCSRepoResponse:
-    """
-    Attributes:
-        repos (Union[Unset, List[Repo]]):
-        total_pages (Union[Unset, int]):
-        message (Union[Unset, str]):  Default: ''.
-    """
-
-    repos: Union[Unset, List[Repo]] = UNSET
-    total_pages: Union[Unset, int] = 0
-    message: Union[Unset, str] = ""
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        repos: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.repos, Unset):
-            repos = []
-            for repos_item_data in self.repos:
-                repos_item = repos_item_data.to_dict()
-
-                repos.append(repos_item)
-
-        total_pages = self.total_pages
-        message = self.message
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if repos is not UNSET:
-            field_dict["repos"] = repos
-        if total_pages is not UNSET:
-            field_dict["total_pages"] = total_pages
-        if message is not UNSET:
-            field_dict["message"] = message
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        repos = []
-        _repos = d.pop("repos", UNSET)
-        for repos_item_data in _repos or []:
-            repos_item = Repo.from_dict(repos_item_data)
-
-            repos.append(repos_item)
-
-        total_pages = d.pop("total_pages", UNSET)
-
-        message = d.pop("message", UNSET)
-
-        vcs_repo_response = cls(
-            repos=repos,
-            total_pages=total_pages,
-            message=message,
-        )
-
-        vcs_repo_response.additional_properties = d
-        return vcs_repo_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-    def __str__(self):
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __repr__(self):
-        return str(self)
+import json
+from typing import Any, Dict, List, Type, TypeVar, Union
+
+import attr
+
+from ..models.repo import Repo
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="VCSRepoResponse")
+
+
+@attr.s(auto_attribs=True, repr=False)
+class VCSRepoResponse:
+    """
+    Attributes:
+        repos (Union[Unset, List[Repo]]):
+        total_pages (Union[Unset, int]):
+        message (Union[Unset, str]):  Default: ''.
+    """
+
+    repos: Union[Unset, List[Repo]] = UNSET
+    total_pages: Union[Unset, int] = 0
+    message: Union[Unset, str] = ""
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        repos: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.repos, Unset):
+            repos = []
+            for repos_item_data in self.repos:
+                repos_item = repos_item_data.to_dict()
+
+                repos.append(repos_item)
+
+        total_pages = self.total_pages
+        message = self.message
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if repos is not UNSET:
+            field_dict["repos"] = repos
+        if total_pages is not UNSET:
+            field_dict["total_pages"] = total_pages
+        if message is not UNSET:
+            field_dict["message"] = message
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        repos = []
+        _repos = d.pop("repos", UNSET)
+        for repos_item_data in _repos or []:
+            repos_item = Repo.from_dict(repos_item_data)
+
+            repos.append(repos_item)
+
+        total_pages = d.pop("total_pages", UNSET)
+
+        message = d.pop("message", UNSET)
+
+        vcs_repo_response = cls(
+            repos=repos,
+            total_pages=total_pages,
+            message=message,
+        )
+
+        vcs_repo_response.additional_properties = d
+        return vcs_repo_response
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
+
+    def __str__(self):
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __repr__(self):
+        return str(self)
```

### Comparing `PyOblv-0.2.0/oblv/oblv_client.py` & `PyOblv-0.2.1/oblv/oblv_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,605 +1,607 @@
-import requests
-import sys
-from jsonschema import validate
-from jsonschema.exceptions import ValidationError
-from oblv.models.name_input import NameInput
-from .api.account import get_user_accounts_account_get
-from .api.auth import logout_session_logout_delete
-from .api.deployment import (
-    create_new_deployment_deployment_post,
-    delete_deployment_deployment_delete,
-    generate_build_args_deployment_arguments_get,
-    get_available_deployments_deployment_available_get,
-    get_deployment_info_deployment_get,
-    get_deployment_roles_deployment_roles_get,
-    get_supported_regions_deployment_supported_regions_get,
-    get_user_owned_deployments_deployment_owned_get,
-)
-from .api.repo import (
-    get_all_repos_repo_linked_get,
-    get_repo_from_vcs_repo_get,
-    get_repo_refs_repo_refs_get,
-    get_repo_repo_repo_owner_repo_name_get,
-    search_repo_from_vcs_repo_search_get,
-)
-from .api.service import (
-    add_repo_service_repo_service_post,
-    delete_repo_services_repo_service_delete,
-    get_repo_service_yaml_form_content_repo_service_yaml_get,
-    get_repo_services_repo_service_get,
-    get_user_services_service_get,
-    update_repo_service_repo_service_put,
-    validate_repo_service_repo_service_validate_get,
-)
-from .api.user import (
-    add_user_public_shared_key_user_psk_put,
-    get_user_deployment_credit_usage_user_credit_usage_get,
-    get_user_profile_view_user_profile_get,
-    get_user_public_shared_key_user_psk_get,
-    update_user_name_user_name_put,
-    update_user_password_user_password_put,
-)
-from .client import AuthenticatedClient
-from .config import URL
-from .exceptions import BadYamlData
-from .models import (
-    PSK,
-    CreateDeploymentInput,
-    ServiceYamlAddInput,
-    ServiceYamlUpdateInput,
-    UserPasswordInput,
-)
-from .utils import bcolors
-
-
-class OblvClient(AuthenticatedClient):
-    def _method_wrapper(function):
-        def wrap(*args, **kwargs):
-            try:
-                return function(*args, **kwargs)
-            except Exception as e:
-                reason = e.__str__()
-                print(
-                bcolors.RED
-                + bcolors.BOLD
-                + "Exception"
-                + bcolors.BLACK
-                + bcolors.ENDC
-                + f": {e}",
-                file=sys.stderr,
-            )
-                raise Exception(reason)
-
-        return wrap
-
-    @_method_wrapper
-    def logout(self):
-        """Logout Session
-
-         This API invalidates the user's token. After a successul response, the user will not be able to use
-        the auth token provided in the auth APIs.
-
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
-        """
-        try:
-            logout_session_logout_delete.sync(
-                client=self, oblivious_user_id=self.oblivious_user_id
-            )
-        except Exception as e:
-            raise e
-        finally:
-            self.token = ""
-            self.oblivious_user_id = ""
-
-    ###### Account Method ######
-
-    @_method_wrapper
-    def accounts(self):
-        """Get User Accounts
-         API to fetch user's linked VCS accounts
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
-        """
-        return get_user_accounts_account_get.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id
-        )
-
-    ############################
-
-    ####### User Methods #######
-    @_method_wrapper
-    def psk(self):
-        """Get User PSK
-         API to fetch user's psk
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, str]]
-        """
-        return get_user_public_shared_key_user_psk_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            user_id=self.oblivious_user_id,
-        )
-
-    @_method_wrapper
-    def credit_usage(self):
-        """Get User Credit Usage
-         API to fetch user's credit usage
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, UserCreditUtilization]]
-        """
-        return get_user_deployment_credit_usage_user_credit_usage_get.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id
-        )
-
-    @_method_wrapper
-    def set_psk(self, public_key):
-        """Update user's publically shareable key
-        API to update user's publically shareable key
-        Args:
-            public_key (str): Public Key to be shared
-        Returns:
-            Response[Union[None, HTTPValidationError, MessageModel]]
-            None is returned if successful
-        """
-
-        input = PSK(public_key)
-        return add_user_public_shared_key_user_psk_put.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id, json_body=input
-        )
-
-    @_method_wrapper
-    def update_name(self, name):
-        """Update Name
-        API to update the name.
-        Args:
-            name (str): User Name
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
-        """
-        update_user_name_user_name_put.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            json_body=NameInput(name),
-        )
-        print("Name updated successfully")
-
-    @_method_wrapper
-    def update_password(self, old_pass, new_pass):
-        """Update User's Password
-         API to update user's password
-        Args:
-            old_pass (str): Old Password
-            new_pass (str): New Password
-        Returns:
-            Response[Union[None, HTTPValidationError, MessageModel]]
-                None is returned if successful
-        """
-        input = UserPasswordInput(old_password=old_pass, password=new_pass)
-        update_user_password_user_password_put.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id, json_body=input
-        )
-        print("Password updated successfully")
-
-    @_method_wrapper
-    def user_profile(self):
-        """Get User Profile
-         API to fetch user's profile details
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, UserProfileResponse]]
-        """
-        return get_user_profile_view_user_profile_get.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id
-        )
-
-    ############################
-
-    ####### Repo Methods #######
-    @_method_wrapper
-    def get_repo(self, owner, name):
-        """Get User Repo
-         API to fetch user's repo information
-        Args:
-            owner (str): Repo Owner
-            name (str): Repo Name
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, Repo]]
-        """
-        return get_repo_repo_repo_owner_repo_name_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            repo_owner=owner,
-            repo_name=name,
-        )
-
-    @_method_wrapper
-    def search_repo(self, keyword):
-        """Add Repo Service With Yaml
-         API to search a repository in VCS, on which the user has access (via their own account, or by any
-        organization they are member of).
-        Args:
-            keyword (str): Search Keyword
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
-        """
-        return search_repo_from_vcs_repo_search_get.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id, search_string=keyword
-        )
-
-    @_method_wrapper
-    def linked_repos(self):
-        """Get User Repos
-         API to fetch user's repo without services
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[RepoAllResponse], MessageModel]]
-        """
-        return get_all_repos_repo_linked_get.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id
-        )
-
-    @_method_wrapper
-    def repo_refs(self, owner, name):
-        """Get Repo Refs
-         API to fetch the repository refs (branches and tags).
-        Args:
-            owner (str): Repo Owner
-            name (str): Repo Name
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, RefResponse]]
-        """
-        return get_repo_refs_repo_refs_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            repo_owner=owner,
-            repo_name=name,
-        )
-
-    @_method_wrapper
-    def repos(self, page: int = 1, per_page: int = 10):
-        """Get Repos From VCS
-         API to get all the repositories from VCS, on which the user has access (via their own account, or by
-        any organization they are member of).
-        Args:
-            page (int):  Page (Default 1)
-            per_page (int):  Repositiories Per Page (Default 10)
-        Returns:
-            Response[Union[Any, HTTPValidationError, VCSRepoResponse]]
-        """
-        return get_repo_from_vcs_repo_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            page=page,
-            per_page=per_page,
-        )
-
-    ############################
-
-    ##### Services Methods #####
-    @_method_wrapper
-    def add_service(
-        self,
-        repo_owner: str,
-        repo_name: str,
-        ref: str,
-        ref_type: str = "branch",
-        data: dict = {},
-    ):
-        """Add Repo Service
-         API to create a service after validation.
-        Args:
-            repo_owner (str): Repo's Owner Name
-            repo_name (str): Repo Name
-            ref (str): Service Ref
-            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
-            data (dict): Service Yaml Content in dictionary format. If provided, service.yaml file will be created/updated based on its existence.
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
-        """
-        if data != {}:
-            try:
-                req = requests.get(URL + "/service_schema")
-                if req.status_code != 200:
-                    raise Exception("Failed to validate service yaml data")
-                validate(data, req.json())
-            except ValidationError as e:
-                raise BadYamlData(e.message)
-            except Exception as e:
-                raise e
-        input = ServiceYamlAddInput.from_dict(data)
-        return add_repo_service_repo_service_post.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            ref=ref,
-            ref_type=ref_type,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-            json_body=input,
-        )
-
-    @_method_wrapper
-    def remove_service(
-        self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
-    ):
-        """Delete Repo Service
-         API to delete a service. It does not delete the existing deployments created from this service.
-        Args:
-            repo_owner (str): Repo's Owner Name
-            repo_name (str): Repo Name
-            ref (str): Service Ref
-            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
-        """
-        delete_repo_services_repo_service_delete.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            ref=ref,
-            ref_type=ref_type,
-            repo_name=repo_name,
-            repo_owner=repo_owner,
-        )
-        print("Successfully removed service")
-
-    @_method_wrapper
-    def service_content(
-        self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
-    ):
-        """Get Repo Service Yaml
-         API to fetch the service.yaml content as object for the given service.
-        Args:
-            repo_id (Union[Unset, str]): Repo Id
-            ref (str): Service Ref
-            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceContentResponse]]
-        """
-        return get_repo_service_yaml_form_content_repo_service_yaml_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-            ref=ref,
-            ref_type=ref_type,
-        )
-
-    @_method_wrapper
-    def repo_services(
-        self,
-        repo_owner: str,
-        repo_name: str,
-        page: int = 1,
-        per_page: int = 10,
-        get_all: bool = False,
-    ):
-        """Get Repo Services
-         API to fetch all the services available for the given repository. This API is valid only for linked
-        repositories.
-        Args:
-            repo_id (str): Repo Id
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[ValidatedService], MessageModel]]
-        """
-        return get_repo_services_repo_service_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-            page=page,
-            per_page=per_page,
-            get_all=get_all,
-        )
-
-    @_method_wrapper
-    def user_services(
-        self,
-        page: int = 1,
-        per_page: int = 10,
-        get_all: bool = False,
-        search_keyword: str = "",
-    ):
-        """Get User Services
-         API to fetch user's services
-        Args:
-            page (int):  Page (Default 1)
-            per_page (str): services per page (Default 10)
-            search_keyword (str): Search Keyword and is applied on repo full name (Default "")
-            get_all (bool): To fetch all services at once (Default False)
-
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[UserServices], MessageModel]]
-        """
-        return get_user_services_service_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            page=page,
-            per_page=per_page,
-            get_all=get_all,
-            search_term=search_keyword,
-        )
-
-    @_method_wrapper
-    def update_service(
-        self,
-        repo_owner: str,
-        repo_name: str,
-        ref,
-        ref_type: str = "branch",
-        data: dict = {},
-    ):
-        """Update Repo Service With Yaml
-         API to update a service, along with updating the service.yaml file. After updating the service.yaml file, the service is validate as well (for missing Dockerfile).
-        Args:
-            repo_owner (str): Repo's Owner Name
-            repo_name (str): Repo Name
-            ref (str): Service Ref
-            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
-            data (dict): Service Yaml Content in dictionary format. If provided, service.yaml file will be created/updated based on its existence.
-
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
-        """
-        if data != {}:
-            try:
-                req = requests.get(URL + "/service_schema")
-                if req.status_code != 200:
-                    raise Exception("Failed to validate service yaml data")
-                validate(data, req.json())
-            except ValidationError as e:
-                raise BadYamlData(e.message)
-            except Exception as e:
-                raise e
-        input = ServiceYamlUpdateInput.from_dict(data)
-        return update_repo_service_repo_service_put.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            ref=ref,
-            ref_type=ref_type,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-            json_body=input,
-        )
-
-    @_method_wrapper
-    def revalidate_service(
-        self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
-    ):
-        """Validate Repo Service
-         API to validate a service with supported service schema. The checks include
-        - Presence of service.yaml in ./oblivious folder.
-        - Presence of Dockerfile in ./oblivious folder.
-        - Content of service.yaml must be valid with respect to supported service schema.
-        Args:
-            repo_owner (str): Repo's Owner Name
-            repo_name (str): Repo Name
-            ref (str): Service Ref
-            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
-        """
-        return validate_repo_service_repo_service_validate_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            repo_owner=repo_owner,
-            repo_name=repo_name,
-            ref=ref,
-            ref_type=ref_type,
-        )
-
-    ############################
-
-    #### Deployment Methods ####
-
-    @_method_wrapper
-    def deployment_info(self, deployment_id):
-        """Get Deployment
-         API to fetch a deployment's details.
-        Args:
-            deployment_id (str): Deployment Id
-        Returns:
-            Response[Union[Any, DeploymentResponse, HTTPValidationError, MessageModel]]
-        """
-        return get_deployment_info_deployment_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            deployment_id=deployment_id,
-        )
-
-    @_method_wrapper
-    def create_deployment(self, deployment: CreateDeploymentInput):
-        """Create Deployment
-         API to create a new deployment.
-        Args:
-            deployment (CreateDeploymentInput): Deployment Details Input
-        Returns:
-            Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
-        """
-        return create_new_deployment_deployment_post.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id, json_body=deployment
-        )
-
-    @_method_wrapper
-    def remove_deployment(self, deployment_id):
-        """Delete Deployment
-         API to initiate termination of a deployment.
-        Args:
-            deployment_id (str): Deployment Id
-        Returns:
-            Response[Union[Any, HTTPValidationError, MessageModel]]
-        """
-        return delete_deployment_deployment_delete.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            deployment_id=deployment_id,
-        )
-
-    @_method_wrapper
-    def generate_deployment_build_args(
-        self, owner: str, repo: str, ref: str, ref_type: str = "branch"
-    ):
-        """Get Build Deployment Arguments
-        API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
-        at which point it was generated. This is to be passed to the create deployment API.
-        Note - A service could have different build args schema depending on the service's commit history.
-        Args:
-            owner (str): Repo Owner
-            repo (str): Repo Name
-            ref (str): Service Ref
-            ref_type (str): Ref Type branch/tag (Default 'branch')
-        Returns:
-            Response[Union[Any, BuildArgsSchema, HTTPValidationError, MessageModel]]
-        """
-        return generate_build_args_deployment_arguments_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            repo=repo,
-            owner=owner,
-            ref=ref,
-        )
-
-    @_method_wrapper
-    def available_deployments(self):
-        """Get Available Deployments
-         API to fetch all the deployments the user can connect to.
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[DeploymentComplete], MessageModel]]
-        """
-        return get_available_deployments_deployment_available_get.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id
-        )
-
-    @_method_wrapper
-    def deployment_roles(self, deployment_id):
-        """Get Deployment Roles
-         API to get a deployment's roles.
-        Args:
-            deployment_id (str): Deployment Id
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[RoleResponse], MessageModel]]
-        """
-        return get_deployment_roles_deployment_roles_get.sync(
-            client=self,
-            oblivious_user_id=self.oblivious_user_id,
-            deployment_id=deployment_id,
-        )
-
-    @_method_wrapper
-    def supported_aws_regions(self):
-        """Deployment Supported Regions
-         API to fetch a deployment's details.
-        Returns:
-            Response[Union[Any, MessageModel]]
-        """
-        return get_supported_regions_deployment_supported_regions_get.sync(client=self)
-
-    @_method_wrapper
-    def deployments(self):
-        """Get Owned Deployments
-         API to fetch a user's owned deployments.
-        Returns:
-            Response[Union[Any, HTTPValidationError, List[DeploymentResponse], MessageModel]]
-        """
-        return get_user_owned_deployments_deployment_owned_get.sync(
-            client=self, oblivious_user_id=self.oblivious_user_id
-        )
-
-    ############################
+import requests
+import sys
+from jsonschema import validate
+from jsonschema.exceptions import ValidationError
+from oblv.models.name_input import NameInput
+from .api.account import get_user_accounts_account_get
+from .api.auth import logout_session_logout_delete
+from .api.deployment import (
+    create_new_deployment_deployment_post,
+    delete_deployment_deployment_delete,
+    generate_build_args_deployment_arguments_get,
+    get_available_deployments_deployment_available_get,
+    get_deployment_info_deployment_get,
+    get_deployment_roles_deployment_roles_get,
+    get_supported_regions_deployment_supported_regions_get,
+    get_user_owned_deployments_deployment_owned_get,
+)
+from .api.repo import (
+    get_all_repos_repo_linked_get,
+    get_repo_from_vcs_repo_get,
+    get_repo_refs_repo_refs_get,
+    get_repo_repo_repo_owner_repo_name_get,
+    search_repo_from_vcs_repo_search_get,
+)
+from .api.service import (
+    add_repo_service_repo_service_post,
+    delete_repo_services_repo_service_delete,
+    get_repo_service_yaml_form_content_repo_service_yaml_get,
+    get_repo_services_repo_service_get,
+    get_user_services_service_get,
+    update_repo_service_repo_service_put,
+    validate_repo_service_repo_service_validate_get,
+)
+from .api.user import (
+    add_user_public_shared_key_user_psk_put,
+    get_user_deployment_credit_usage_user_credit_usage_get,
+    get_user_profile_view_user_profile_get,
+    get_user_public_shared_key_user_psk_get,
+    update_user_name_user_name_put,
+    update_user_password_user_password_put,
+)
+from .client import AuthenticatedClient
+from .config import URL
+from .exceptions import BadYamlData
+from .models import (
+    PSK,
+    CreateDeploymentInput,
+    ServiceYamlAddInput,
+    ServiceYamlUpdateInput,
+    UserPasswordInput,
+)
+from .utils import bcolors
+import logging
+
+
+class OblvClient(AuthenticatedClient):
+    def _method_wrapper(function):
+        def wrap(*args, **kwargs):
+            try:
+                logging.warn("PyOblv is deprecated, and will not be supported in future. Kindly use oblv-ctl (https://pypi.org/project/oblv-ctl/) to access Oblivious APIs.")
+                return function(*args, **kwargs)
+            except Exception as e:
+                reason = e.__str__()
+                print(
+                bcolors.RED
+                + bcolors.BOLD
+                + "Exception"
+                + bcolors.BLACK
+                + bcolors.ENDC
+                + f": {e}",
+                file=sys.stderr,
+            )
+                raise Exception(reason)
+
+        return wrap
+
+    @_method_wrapper
+    def logout(self):
+        """Logout Session
+
+         This API invalidates the user's token. After a successul response, the user will not be able to use
+        the auth token provided in the auth APIs.
+
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel]]
+        """
+        try:
+            logout_session_logout_delete.sync(
+                client=self, oblivious_user_id=self.oblivious_user_id
+            )
+        except Exception as e:
+            raise e
+        finally:
+            self.token = ""
+            self.oblivious_user_id = ""
+
+    ###### Account Method ######
+
+    @_method_wrapper
+    def accounts(self):
+        """Get User Accounts
+         API to fetch user's linked VCS accounts
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[Account], MessageModel]]
+        """
+        return get_user_accounts_account_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id
+        )
+
+    ############################
+
+    ####### User Methods #######
+    @_method_wrapper
+    def psk(self):
+        """Get User PSK
+         API to fetch user's psk
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, str]]
+        """
+        return get_user_public_shared_key_user_psk_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            user_id=self.oblivious_user_id,
+        )
+
+    @_method_wrapper
+    def credit_usage(self):
+        """Get User Credit Usage
+         API to fetch user's credit usage
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, UserCreditUtilization]]
+        """
+        return get_user_deployment_credit_usage_user_credit_usage_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id
+        )
+
+    @_method_wrapper
+    def set_psk(self, public_key):
+        """Update user's publically shareable key
+        API to update user's publically shareable key
+        Args:
+            public_key (str): Public Key to be shared
+        Returns:
+            Response[Union[None, HTTPValidationError, MessageModel]]
+            None is returned if successful
+        """
+
+        input = PSK(public_key)
+        return add_user_public_shared_key_user_psk_put.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, json_body=input
+        )
+
+    @_method_wrapper
+    def update_name(self, name):
+        """Update Name
+        API to update the name.
+        Args:
+            name (str): User Name
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel]]
+        """
+        update_user_name_user_name_put.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            json_body=NameInput(name),
+        )
+        print("Name updated successfully")
+
+    @_method_wrapper
+    def update_password(self, old_pass, new_pass):
+        """Update User's Password
+         API to update user's password
+        Args:
+            old_pass (str): Old Password
+            new_pass (str): New Password
+        Returns:
+            Response[Union[None, HTTPValidationError, MessageModel]]
+                None is returned if successful
+        """
+        input = UserPasswordInput(old_password=old_pass, password=new_pass)
+        update_user_password_user_password_put.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, json_body=input
+        )
+        print("Password updated successfully")
+
+    @_method_wrapper
+    def user_profile(self):
+        """Get User Profile
+         API to fetch user's profile details
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, UserProfileResponse]]
+        """
+        return get_user_profile_view_user_profile_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id
+        )
+
+    ############################
+
+    ####### Repo Methods #######
+    @_method_wrapper
+    def get_repo(self, owner, name):
+        """Get User Repo
+         API to fetch user's repo information
+        Args:
+            owner (str): Repo Owner
+            name (str): Repo Name
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, Repo]]
+        """
+        return get_repo_repo_repo_owner_repo_name_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            repo_owner=owner,
+            repo_name=name,
+        )
+
+    @_method_wrapper
+    def search_repo(self, keyword):
+        """Add Repo Service With Yaml
+         API to search a repository in VCS, on which the user has access (via their own account, or by any
+        organization they are member of).
+        Args:
+            keyword (str): Search Keyword
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[Repo], MessageModel]]
+        """
+        return search_repo_from_vcs_repo_search_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, search_string=keyword
+        )
+
+    @_method_wrapper
+    def linked_repos(self):
+        """Get User Repos
+         API to fetch user's repo without services
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[RepoAllResponse], MessageModel]]
+        """
+        return get_all_repos_repo_linked_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id
+        )
+
+    @_method_wrapper
+    def repo_refs(self, owner, name):
+        """Get Repo Refs
+         API to fetch the repository refs (branches and tags).
+        Args:
+            owner (str): Repo Owner
+            name (str): Repo Name
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, RefResponse]]
+        """
+        return get_repo_refs_repo_refs_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            repo_owner=owner,
+            repo_name=name,
+        )
+
+    @_method_wrapper
+    def repos(self, page: int = 1, per_page: int = 10):
+        """Get Repos From VCS
+         API to get all the repositories from VCS, on which the user has access (via their own account, or by
+        any organization they are member of).
+        Args:
+            page (int):  Page (Default 1)
+            per_page (int):  Repositiories Per Page (Default 10)
+        Returns:
+            Response[Union[Any, HTTPValidationError, VCSRepoResponse]]
+        """
+        return get_repo_from_vcs_repo_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            page=page,
+            per_page=per_page,
+        )
+
+    ############################
+
+    ##### Services Methods #####
+    @_method_wrapper
+    def add_service(
+        self,
+        repo_owner: str,
+        repo_name: str,
+        ref: str,
+        ref_type: str = "branch",
+        data: dict = {},
+    ):
+        """Add Repo Service
+         API to create a service after validation.
+        Args:
+            repo_owner (str): Repo's Owner Name
+            repo_name (str): Repo Name
+            ref (str): Service Ref
+            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
+            data (dict): Service Yaml Content in dictionary format. If provided, service.yaml file will be created/updated based on its existence.
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        """
+        if data != {}:
+            try:
+                req = requests.get(URL + "/service_schema")
+                if req.status_code != 200:
+                    raise Exception("Failed to validate service yaml data")
+                validate(data, req.json())
+            except ValidationError as e:
+                raise BadYamlData(e.message)
+            except Exception as e:
+                raise e
+        input = ServiceYamlAddInput.from_dict(data)
+        return add_repo_service_repo_service_post.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            ref=ref,
+            ref_type=ref_type,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+            json_body=input,
+        )
+
+    @_method_wrapper
+    def remove_service(
+        self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
+    ):
+        """Delete Repo Service
+         API to delete a service. It does not delete the existing deployments created from this service.
+        Args:
+            repo_owner (str): Repo's Owner Name
+            repo_name (str): Repo Name
+            ref (str): Service Ref
+            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel]]
+        """
+        delete_repo_services_repo_service_delete.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            ref=ref,
+            ref_type=ref_type,
+            repo_name=repo_name,
+            repo_owner=repo_owner,
+        )
+        print("Successfully removed service")
+
+    @_method_wrapper
+    def service_content(
+        self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
+    ):
+        """Get Repo Service Yaml
+         API to fetch the service.yaml content as object for the given service.
+        Args:
+            repo_id (Union[Unset, str]): Repo Id
+            ref (str): Service Ref
+            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, ServiceContentResponse]]
+        """
+        return get_repo_service_yaml_form_content_repo_service_yaml_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+            ref=ref,
+            ref_type=ref_type,
+        )
+
+    @_method_wrapper
+    def repo_services(
+        self,
+        repo_owner: str,
+        repo_name: str,
+        page: int = 1,
+        per_page: int = 10,
+        get_all: bool = False,
+    ):
+        """Get Repo Services
+         API to fetch all the services available for the given repository. This API is valid only for linked
+        repositories.
+        Args:
+            repo_id (str): Repo Id
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[ValidatedService], MessageModel]]
+        """
+        return get_repo_services_repo_service_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+            page=page,
+            per_page=per_page,
+            get_all=get_all,
+        )
+
+    @_method_wrapper
+    def user_services(
+        self,
+        page: int = 1,
+        per_page: int = 10,
+        get_all: bool = False,
+        search_keyword: str = "",
+    ):
+        """Get User Services
+         API to fetch user's services
+        Args:
+            page (int):  Page (Default 1)
+            per_page (str): services per page (Default 10)
+            search_keyword (str): Search Keyword and is applied on repo full name (Default "")
+            get_all (bool): To fetch all services at once (Default False)
+
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[UserServices], MessageModel]]
+        """
+        return get_user_services_service_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            page=page,
+            per_page=per_page,
+            get_all=get_all,
+            search_term=search_keyword,
+        )
+
+    @_method_wrapper
+    def update_service(
+        self,
+        repo_owner: str,
+        repo_name: str,
+        ref,
+        ref_type: str = "branch",
+        data: dict = {},
+    ):
+        """Update Repo Service With Yaml
+         API to update a service, along with updating the service.yaml file. After updating the service.yaml file, the service is validate as well (for missing Dockerfile).
+        Args:
+            repo_owner (str): Repo's Owner Name
+            repo_name (str): Repo Name
+            ref (str): Service Ref
+            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
+            data (dict): Service Yaml Content in dictionary format. If provided, service.yaml file will be created/updated based on its existence.
+
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        """
+        if data != {}:
+            try:
+                req = requests.get(URL + "/service_schema")
+                if req.status_code != 200:
+                    raise Exception("Failed to validate service yaml data")
+                validate(data, req.json())
+            except ValidationError as e:
+                raise BadYamlData(e.message)
+            except Exception as e:
+                raise e
+        input = ServiceYamlUpdateInput.from_dict(data)
+        return update_repo_service_repo_service_put.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            ref=ref,
+            ref_type=ref_type,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+            json_body=input,
+        )
+
+    @_method_wrapper
+    def revalidate_service(
+        self, repo_owner: str, repo_name: str, ref: str, ref_type: str = "branch"
+    ):
+        """Validate Repo Service
+         API to validate a service with supported service schema. The checks include
+        - Presence of service.yaml in ./oblivious folder.
+        - Presence of Dockerfile in ./oblivious folder.
+        - Content of service.yaml must be valid with respect to supported service schema.
+        Args:
+            repo_owner (str): Repo's Owner Name
+            repo_name (str): Repo Name
+            ref (str): Service Ref
+            ref_type (Union[Unset, None, str]):  Ref Type branch/tag (Default 'branch')
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel, ServiceValidationResponse]]
+        """
+        return validate_repo_service_repo_service_validate_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            repo_owner=repo_owner,
+            repo_name=repo_name,
+            ref=ref,
+            ref_type=ref_type,
+        )
+
+    ############################
+
+    #### Deployment Methods ####
+
+    @_method_wrapper
+    def deployment_info(self, deployment_id):
+        """Get Deployment
+         API to fetch a deployment's details.
+        Args:
+            deployment_id (str): Deployment Id
+        Returns:
+            Response[Union[Any, DeploymentResponse, HTTPValidationError, MessageModel]]
+        """
+        return get_deployment_info_deployment_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            deployment_id=deployment_id,
+        )
+
+    @_method_wrapper
+    def create_deployment(self, deployment: CreateDeploymentInput):
+        """Create Deployment
+         API to create a new deployment.
+        Args:
+            deployment (CreateDeploymentInput): Deployment Details Input
+        Returns:
+            Response[Union[Any, CreateDeploymentResponse, HTTPValidationError, MessageModel]]
+        """
+        return create_new_deployment_deployment_post.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id, json_body=deployment
+        )
+
+    @_method_wrapper
+    def remove_deployment(self, deployment_id):
+        """Delete Deployment
+         API to initiate termination of a deployment.
+        Args:
+            deployment_id (str): Deployment Id
+        Returns:
+            Response[Union[Any, HTTPValidationError, MessageModel]]
+        """
+        return delete_deployment_deployment_delete.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            deployment_id=deployment_id,
+        )
+
+    @_method_wrapper
+    def generate_deployment_build_args(
+        self, owner: str, repo: str, ref: str, ref_type: str = "branch"
+    ):
+        """Get Build Deployment Arguments
+        API to fetch the arguments schema necessary for creating a deployment. It also gives the commit sha,
+        at which point it was generated. This is to be passed to the create deployment API.
+        Note - A service could have different build args schema depending on the service's commit history.
+        Args:
+            owner (str): Repo Owner
+            repo (str): Repo Name
+            ref (str): Service Ref
+            ref_type (str): Ref Type branch/tag (Default 'branch')
+        Returns:
+            Response[Union[Any, BuildArgsSchema, HTTPValidationError, MessageModel]]
+        """
+        return generate_build_args_deployment_arguments_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            repo=repo,
+            owner=owner,
+            ref=ref,
+        )
+
+    @_method_wrapper
+    def available_deployments(self):
+        """Get Available Deployments
+         API to fetch all the deployments the user can connect to.
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[DeploymentComplete], MessageModel]]
+        """
+        return get_available_deployments_deployment_available_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id
+        )
+
+    @_method_wrapper
+    def deployment_roles(self, deployment_id):
+        """Get Deployment Roles
+         API to get a deployment's roles.
+        Args:
+            deployment_id (str): Deployment Id
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[RoleResponse], MessageModel]]
+        """
+        return get_deployment_roles_deployment_roles_get.sync(
+            client=self,
+            oblivious_user_id=self.oblivious_user_id,
+            deployment_id=deployment_id,
+        )
+
+    @_method_wrapper
+    def supported_aws_regions(self):
+        """Deployment Supported Regions
+         API to fetch a deployment's details.
+        Returns:
+            Response[Union[Any, MessageModel]]
+        """
+        return get_supported_regions_deployment_supported_regions_get.sync(client=self)
+
+    @_method_wrapper
+    def deployments(self):
+        """Get Owned Deployments
+         API to fetch a user's owned deployments.
+        Returns:
+            Response[Union[Any, HTTPValidationError, List[DeploymentResponse], MessageModel]]
+        """
+        return get_user_owned_deployments_deployment_owned_get.sync(
+            client=self, oblivious_user_id=self.oblivious_user_id
+        )
+
+    ############################
```

### Comparing `PyOblv-0.2.0/oblv/types.py` & `PyOblv-0.2.1/oblv/types.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-""" Contains some shared types for properties """
-from typing import BinaryIO, Generic, MutableMapping, Optional, Tuple, TypeVar
-
-import attr
-
-
-class Unset:
-    def __bool__(self) -> bool:
-        return False
-
-
-UNSET: Unset = Unset()
-
-FileJsonType = Tuple[Optional[str], BinaryIO, Optional[str]]
-
-
-@attr.s(auto_attribs=True)
-class File:
-    """Contains information for file uploads"""
-
-    payload: BinaryIO
-    file_name: Optional[str] = None
-    mime_type: Optional[str] = None
-
-    def to_tuple(self) -> FileJsonType:
-        """Return a tuple representation that httpx will accept for multipart/form-data"""
-        return self.file_name, self.payload, self.mime_type
-
-
-T = TypeVar("T")
-
-
-@attr.s(auto_attribs=True)
-class Response(Generic[T]):
-    """A response from an endpoint"""
-
-    status_code: int
-    content: bytes
-    headers: MutableMapping[str, str]
-    parsed: Optional[T]
-
-
-__all__ = ["File", "Response", "FileJsonType"]
+""" Contains some shared types for properties """
+from typing import BinaryIO, Generic, MutableMapping, Optional, Tuple, TypeVar
+
+import attr
+
+
+class Unset:
+    def __bool__(self) -> bool:
+        return False
+
+
+UNSET: Unset = Unset()
+
+FileJsonType = Tuple[Optional[str], BinaryIO, Optional[str]]
+
+
+@attr.s(auto_attribs=True)
+class File:
+    """Contains information for file uploads"""
+
+    payload: BinaryIO
+    file_name: Optional[str] = None
+    mime_type: Optional[str] = None
+
+    def to_tuple(self) -> FileJsonType:
+        """Return a tuple representation that httpx will accept for multipart/form-data"""
+        return self.file_name, self.payload, self.mime_type
+
+
+T = TypeVar("T")
+
+
+@attr.s(auto_attribs=True)
+class Response(Generic[T]):
+    """A response from an endpoint"""
+
+    status_code: int
+    content: bytes
+    headers: MutableMapping[str, str]
+    parsed: Optional[T]
+
+
+__all__ = ["File", "Response", "FileJsonType"]
```

### Comparing `PyOblv-0.2.0/oblv/utils.py` & `PyOblv-0.2.1/oblv/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-
-
-
-class bcolors:
-    HEADER = "\033[95m"
-    BLUE = "\033[94m"
-    GREEN = "\033[92m"
-    YELLOW = "\033[93m"
-    RED = "\033[91m"
-    ENDC = "\033[0m"
-    BOLD = "\033[1m"
-    UNDERLINE = "\033[4m"
-    BLACK = "\033[99m"
-
-    @staticmethod
-    def green(message: str) -> str:
-        return bcolors.GREEN + message + bcolors.ENDC
-
-    @staticmethod
-    def red(message: str) -> str:
-        return bcolors.RED + message + bcolors.ENDC
-
-    @staticmethod
-    def yellow(message: str) -> str:
-        return bcolors.YELLOW + message + bcolors.ENDC
-
-    @staticmethod
-    def bold(message: str, end_color: bool = False) -> str:
-        msg = bcolors.BOLD + message
-        if end_color:
-            msg += bcolors.ENDC
-        return msg
-
-    @staticmethod
-    def underline(message: str, end_color: bool = False) -> str:
-        msg = bcolors.UNDERLINE + message
-        if end_color:
-            msg += bcolors.ENDC
-        return msg
-
-    @staticmethod
-    def warning(message: str) -> str:
-        return bcolors.bold(bcolors.yellow(message))
-
-    @staticmethod
-    def success(message: str) -> str:
-        return bcolors.green(message)
-
-    @staticmethod
-    def failure(message: str) -> str:
+
+
+
+class bcolors:
+    HEADER = "\033[95m"
+    BLUE = "\033[94m"
+    GREEN = "\033[92m"
+    YELLOW = "\033[93m"
+    RED = "\033[91m"
+    ENDC = "\033[0m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+    BLACK = "\033[99m"
+
+    @staticmethod
+    def green(message: str) -> str:
+        return bcolors.GREEN + message + bcolors.ENDC
+
+    @staticmethod
+    def red(message: str) -> str:
+        return bcolors.RED + message + bcolors.ENDC
+
+    @staticmethod
+    def yellow(message: str) -> str:
+        return bcolors.YELLOW + message + bcolors.ENDC
+
+    @staticmethod
+    def bold(message: str, end_color: bool = False) -> str:
+        msg = bcolors.BOLD + message
+        if end_color:
+            msg += bcolors.ENDC
+        return msg
+
+    @staticmethod
+    def underline(message: str, end_color: bool = False) -> str:
+        msg = bcolors.UNDERLINE + message
+        if end_color:
+            msg += bcolors.ENDC
+        return msg
+
+    @staticmethod
+    def warning(message: str) -> str:
+        return bcolors.bold(bcolors.yellow(message))
+
+    @staticmethod
+    def success(message: str) -> str:
+        return bcolors.green(message)
+
+    @staticmethod
+    def failure(message: str) -> str:
         return bcolors.red(message)
```

### Comparing `PyOblv-0.2.0/tests/unit/constants.py` & `PyOblv-0.2.1/tests/unit/constants.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-USER_ID = "user_id"
-USER_LOGIN = "user_login"
-USER_TOKEN = "user_token"
-USER_EMAIL = "user_email"
-USER_NAME = "user_name"
-BAD_REQUEST_MESSAGE = "Bad Request"
-API_GW_REQUEST_ID = "dummy-request-id"
-EXCEPTION_OCCURED = "Exception Occured"
-FORBIDDEN = "Forbidden"
-SUCCESS="Success"
-KEY_MESSAGE = "message"
-KEY_APIGW_REQUESTID = "apigw-requestid"
-KEY_VALID_ERROR_LOC = "location"
-VALID_ERROR_MESSAGE = "Invalid Message"
-VALID_ERROR_VALUE = "value"
-GITHUB_USER_ID = "123456"
-GITHUB_USER_LOGIN = "github_user_login"
-OLD_PASS="Oldpass123#"
-NEW_PASS="Newpass123#"
-GITHUB = "github"
-RANDOM_PUBLIC_KEY = "MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnLMkUkUTDrI2QIkyzF9iULdvjzpJHDIjV1r9X1R9D4wbzpC8cmwblSOD9gS9iZQaEijBzlc1gbe3fXMhwM6XImVQ7xn1lfQ7WZcfwTLK+V1lqIBIqn/Y+hxhecbWKM25RIRoAJ/jIfL608ltydbsl0oaMaEnU1r5PwNh5vGp8vVPsEN0DwgyJjrA6qTv1ZqeSoPuNwcQJH07U9tRngIABf5mKzUfRphX011CqISgKh8drwtac7nRxL452fD5eErRVTa6vrTfvKV5H4SUM3uJIuLE718xEM0QRaWfSSBD2hPCbpCSqaaAUFGgI3oEJ7LbA3z3pGmcKAUTVIwIDAQAB"
-INVALID_PUBLIC_KEY = "MIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEf452fD5eErRVTa6vrTfvKV5H4SUM3uJIuLE718xEM0QRaWfSSBD2hPCbpCSqaaAUFGgI3oEJ7LbA3z3pGmcKAUTVIwIDAQAB"
-USER_REPO = {
-    "repo_id": 123456,
-    "name": "Repo_Name",
-    "is_private": False,
-    "owner_login": "Owner_Login",
-    "account_type": "github"
-}
-VCS_REPO_RESPONSE = {
-    "repos": [{
-        "repo_id": 506983974,
-        "name": "Oblivious",
-        "full_name": "ObliviousAI/Oblivious",
-        "is_private": False,
-        "owner_login": "ObliviousAI",
-        "description": "\u2728 A single place to post issues & feature requests",
-        "html_url": "https://github.com/ObliviousAI/Oblivious",
-        "git_url": "git://github.com/ObliviousAI/Oblivious.git",
-        "clone_url": "https://github.com/ObliviousAI/Oblivious.git",
-        "default_branch": "master",
-        "updated_at": "2022-09-01T20:29:36Z",
-        "account_type": "github"
-    },
-        {
-        "repo_id": 123456,
-        "name": "Repo_Name",
-                "full_name": "Owner_Login/Repo_Name",
-                "is_private": False,
-                "owner_login": "Owner_Login",
-                "account_type": "github",
-        "description": "Some Description",
-        "html_url": "https://github.com/Owner_Login/Repo_Name",
-        "git_url": "git://github.com/Owner_Login/Repo_Name.git",
-        "clone_url": "https://github.com/Owner_Login/Repo_Name.git",
-        "default_branch": "master",
-        "updated_at": "2022-09-12T20:29:36Z",
-        "account_type": "github"
-    }],
-  "total_pages": 1,
-  "message": ""
-}
-REPO_WITH_SERVICE={
-        "repo_id": 123456,
-        "name": "Repo_Name",
-                "full_name": "Owner_Login/Repo_Name",
-                "is_private": False,
-                "owner_login": "Owner_Login",
-                "account_type": "github",
-        "description": "Some Description",
-        "html_url": "https://github.com/Owner_Login/Repo_Name",
-        "git_url": "git://github.com/Owner_Login/Repo_Name.git",
-        "clone_url": "https://github.com/Owner_Login/Repo_Name.git",
-        "default_branch": "master",
-        "updated_at": "2022-09-12T20:29:36Z",
-        "account_type": "github",
-        "services": [{
-            "ref": "master",
-            "sha": "some sha",
-            "type": "branch",
-            "service_validated": True
-        }]
-    }
-
-REPO_REFS={"branch":["master","dummy"],"tags":["v1.0"]}
-USER_SERVICES = [{
-    "repo_id": "123456",
-    "repo_name": "Repo_Name",
-    "repo_owner": "Owner_Name",
-    "account_type": "github",
-    "ref": "master",
-    "sha": "some sha",
-    "type": "branch",
-    "service_validated": True
-}]
-REPO_SERVICES = [{
-    "ref": "master",
-    "sha": "some sha",
-    "type": "branch",
-    "service_validated": True
-}]
-SERVICE_YAML_CONTENT={
-  "auth": [
-    {
-      "auth_name": "Auth",
-      "auth_type": "signed_headers"
-    }
-  ],
-  "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
-  "build_args": [],
-  "meta": {
-    "author": "Team Oblivious",
-    "author_email": "hello@oblivious.ai",
-    "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
-    "version": "0.1.0"
-  },
-  "paths": [
-    {
-      "access": "user",
-      "path": "/hello/",
-      "short_description": "Hello world example"
-    }
-    ],
-    "outbound": [
-      {
-        "domain": "example.com",
-        "name": "example",
-        "port": 443,
-        "type": "tcp"
-      }
-    ]
-  }
-DEPLOYMENT_ID="deployment_id"
-DEPLOYMENT={
-    "deployment_id": DEPLOYMENT_ID,
-    "deployment_name": "deployment_name",
-    "account_type": "github",
-    "owner": USER_ID,
-    "owner_login": USER_LOGIN,
-    "repo_name": "Repo_Name",
-    "repo_owner": "Owner_Name",
-    "tags": [],
-    "branch_release": "master",
-    "current_state": "Running",
-    "visibility": "private",
-    "is_dev_env": True,
-    "creation_time": "01-06-2022 19:50:02",
-    "sha": "some sha",
-    "is_deleted": True,
-    "instance": {
-        "region_name": "us-east-1",
-        "stack_name": "stack name",
-        "instance_type": "c5.xlarge",
-        "instance_url": "instance url",
-        "service_url": "service url",
-        "build_log_location": ""
-    },
-    "pcr_codes": ["pcr0codeletters","pcr1codeletters","pcr2codeletters"],
-    "credit_utilization_per_hour": 68,
-    "build_args": {
-        "auth": {},
-        "users": {
-            "user": [{
-                "user_name": "some_user",
-                "public key": "MIIBCgKCAQEA1MuTZlPrs845FZOFm8TTeakJKr1FmW3JxAc64IafZw3WYvP1wtQOH4eSgJm5138RG1Hdg4gmWkS/4PbstxTpciwX80ARKbi8Jv7UkayeKBeLT7j7B+aRxebIJUH0THstST9nFO+10MTuNY7+AXNzfYR6PihtfmQIDAQAA",
-                "user_login": "u-185b6de2-837a-4cbb-93fc-d1c9f96f3b04"
-            }]
-        },
-        "infra_reqs": {
-            "CPUs": 2,
-            "RAM": 4000
-        }
-    },
-    "shared_users": [],
-    "history": [{
-        "action": "STARTED",
-        "timestamp": "01-06-2022 19:55:42"
-    }]
-}
-SUPPORTED_REGIONS={
-  "us-east-1": "US East (N. Virginia)",
-  "us-west-2": "US West (Oregon)",
-  "eu-central-1": "Europe (Frankfurt)",
-  "eu-west-2": "Europe (London)"
-}
-DEPLOYMENT_ROLES=[{
-    "role_name": "user",
-    "role_description": "User Role"
-}]
-ARGUMENTS_RESPONSE={
-  "sha": "some_sha",
-  "arg_schema": {
-    "some_key": "some_value"
-  }
-}
-CREATE_DEPLOYMENT_INPUT= {
-    "owner": "Owner Name",
-    "repo": "Repo Name",
-    "account_type": "github",
-    "ref": "master",
-    "region_name": "us-east-2",
-    "deployment_name": "deployment name",
-    "visibility": "private",
-    "is_dev_env": True,
-    "tags": [],
-    "build_args": {
-        "auth": {},
-        "users": {
-            "user": [{
-                "user_name": "some_user",
-                "public key": "MIIBCgKCAQEA1MuTZlPrs845FZOFm8TTeakJKr1FmW3JxAc64IafZw3WYvP1wtQOH4eSgJm5138RG1Hdg4gmWkS/4PbstxTpciwX80ARKbi8Jv7UkayeKBeLT7j7B+aRxebIJUH0THstST9nFO+10MTuNY7+AXNzfYR6PihtfmQIDAQAA",
-                "user_login": "u-185b6de2-837a-4cbb-93fc-d1c9f96f3b04"
-            }]
-        },
-        "infra_reqs":"c5.xlarge"
-    }
-}
+USER_ID = "user_id"
+USER_LOGIN = "user_login"
+USER_TOKEN = "user_token"
+USER_EMAIL = "user_email"
+USER_NAME = "user_name"
+BAD_REQUEST_MESSAGE = "Bad Request"
+API_GW_REQUEST_ID = "dummy-request-id"
+EXCEPTION_OCCURED = "Exception Occured"
+FORBIDDEN = "Forbidden"
+SUCCESS="Success"
+KEY_MESSAGE = "message"
+KEY_APIGW_REQUESTID = "apigw-requestid"
+KEY_VALID_ERROR_LOC = "location"
+VALID_ERROR_MESSAGE = "Invalid Message"
+VALID_ERROR_VALUE = "value"
+GITHUB_USER_ID = "123456"
+GITHUB_USER_LOGIN = "github_user_login"
+OLD_PASS="Oldpass123#"
+NEW_PASS="Newpass123#"
+GITHUB = "github"
+RANDOM_PUBLIC_KEY = "MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAnLMkUkUTDrI2QIkyzF9iULdvjzpJHDIjV1r9X1R9D4wbzpC8cmwblSOD9gS9iZQaEijBzlc1gbe3fXMhwM6XImVQ7xn1lfQ7WZcfwTLK+V1lqIBIqn/Y+hxhecbWKM25RIRoAJ/jIfL608ltydbsl0oaMaEnU1r5PwNh5vGp8vVPsEN0DwgyJjrA6qTv1ZqeSoPuNwcQJH07U9tRngIABf5mKzUfRphX011CqISgKh8drwtac7nRxL452fD5eErRVTa6vrTfvKV5H4SUM3uJIuLE718xEM0QRaWfSSBD2hPCbpCSqaaAUFGgI3oEJ7LbA3z3pGmcKAUTVIwIDAQAB"
+INVALID_PUBLIC_KEY = "MIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEf452fD5eErRVTa6vrTfvKV5H4SUM3uJIuLE718xEM0QRaWfSSBD2hPCbpCSqaaAUFGgI3oEJ7LbA3z3pGmcKAUTVIwIDAQAB"
+USER_REPO = {
+    "repo_id": 123456,
+    "name": "Repo_Name",
+    "is_private": False,
+    "owner_login": "Owner_Login",
+    "account_type": "github"
+}
+VCS_REPO_RESPONSE = {
+    "repos": [{
+        "repo_id": 506983974,
+        "name": "Oblivious",
+        "full_name": "ObliviousAI/Oblivious",
+        "is_private": False,
+        "owner_login": "ObliviousAI",
+        "description": "\u2728 A single place to post issues & feature requests",
+        "html_url": "https://github.com/ObliviousAI/Oblivious",
+        "git_url": "git://github.com/ObliviousAI/Oblivious.git",
+        "clone_url": "https://github.com/ObliviousAI/Oblivious.git",
+        "default_branch": "master",
+        "updated_at": "2022-09-01T20:29:36Z",
+        "account_type": "github"
+    },
+        {
+        "repo_id": 123456,
+        "name": "Repo_Name",
+                "full_name": "Owner_Login/Repo_Name",
+                "is_private": False,
+                "owner_login": "Owner_Login",
+                "account_type": "github",
+        "description": "Some Description",
+        "html_url": "https://github.com/Owner_Login/Repo_Name",
+        "git_url": "git://github.com/Owner_Login/Repo_Name.git",
+        "clone_url": "https://github.com/Owner_Login/Repo_Name.git",
+        "default_branch": "master",
+        "updated_at": "2022-09-12T20:29:36Z",
+        "account_type": "github"
+    }],
+  "total_pages": 1,
+  "message": ""
+}
+REPO_WITH_SERVICE={
+        "repo_id": 123456,
+        "name": "Repo_Name",
+                "full_name": "Owner_Login/Repo_Name",
+                "is_private": False,
+                "owner_login": "Owner_Login",
+                "account_type": "github",
+        "description": "Some Description",
+        "html_url": "https://github.com/Owner_Login/Repo_Name",
+        "git_url": "git://github.com/Owner_Login/Repo_Name.git",
+        "clone_url": "https://github.com/Owner_Login/Repo_Name.git",
+        "default_branch": "master",
+        "updated_at": "2022-09-12T20:29:36Z",
+        "account_type": "github",
+        "services": [{
+            "ref": "master",
+            "sha": "some sha",
+            "type": "branch",
+            "service_validated": True
+        }]
+    }
+
+REPO_REFS={"branch":["master","dummy"],"tags":["v1.0"]}
+USER_SERVICES = [{
+    "repo_id": "123456",
+    "repo_name": "Repo_Name",
+    "repo_owner": "Owner_Name",
+    "account_type": "github",
+    "ref": "master",
+    "sha": "some sha",
+    "type": "branch",
+    "service_validated": True
+}]
+REPO_SERVICES = [{
+    "ref": "master",
+    "sha": "some sha",
+    "type": "branch",
+    "service_validated": True
+}]
+SERVICE_YAML_CONTENT={
+  "auth": [
+    {
+      "auth_name": "Auth",
+      "auth_type": "signed_headers"
+    }
+  ],
+  "base_image": "oblv_ubuntu_18_04_proxy_nsm_api_python_3_8",
+  "build_args": [],
+  "meta": {
+    "author": "Team Oblivious",
+    "author_email": "hello@oblivious.ai",
+    "git": "https://github.com/ObliviousAI/FastAPI-Enclave-Services.git",
+    "version": "0.1.0"
+  },
+  "paths": [
+    {
+      "access": "user",
+      "path": "/hello/",
+      "short_description": "Hello world example"
+    }
+    ],
+    "outbound": [
+      {
+        "domain": "example.com",
+        "name": "example",
+        "port": 443,
+        "type": "tcp"
+      }
+    ]
+  }
+DEPLOYMENT_ID="deployment_id"
+DEPLOYMENT={
+    "deployment_id": DEPLOYMENT_ID,
+    "deployment_name": "deployment_name",
+    "account_type": "github",
+    "owner": USER_ID,
+    "owner_login": USER_LOGIN,
+    "repo_name": "Repo_Name",
+    "repo_owner": "Owner_Name",
+    "tags": [],
+    "branch_release": "master",
+    "current_state": "Running",
+    "visibility": "private",
+    "is_dev_env": True,
+    "creation_time": "01-06-2022 19:50:02",
+    "sha": "some sha",
+    "is_deleted": True,
+    "instance": {
+        "region_name": "us-east-1",
+        "stack_name": "stack name",
+        "instance_type": "c5.xlarge",
+        "instance_url": "instance url",
+        "service_url": "service url",
+        "build_log_location": ""
+    },
+    "pcr_codes": ["pcr0codeletters","pcr1codeletters","pcr2codeletters"],
+    "credit_utilization_per_hour": 68,
+    "build_args": {
+        "auth": {},
+        "users": {
+            "user": [{
+                "user_name": "some_user",
+                "public key": "MIIBCgKCAQEA1MuTZlPrs845FZOFm8TTeakJKr1FmW3JxAc64IafZw3WYvP1wtQOH4eSgJm5138RG1Hdg4gmWkS/4PbstxTpciwX80ARKbi8Jv7UkayeKBeLT7j7B+aRxebIJUH0THstST9nFO+10MTuNY7+AXNzfYR6PihtfmQIDAQAA",
+                "user_login": "u-185b6de2-837a-4cbb-93fc-d1c9f96f3b04"
+            }]
+        },
+        "infra_reqs": {
+            "CPUs": 2,
+            "RAM": 4000
+        }
+    },
+    "shared_users": [],
+    "history": [{
+        "action": "STARTED",
+        "timestamp": "01-06-2022 19:55:42"
+    }]
+}
+SUPPORTED_REGIONS={
+  "us-east-1": "US East (N. Virginia)",
+  "us-west-2": "US West (Oregon)",
+  "eu-central-1": "Europe (Frankfurt)",
+  "eu-west-2": "Europe (London)"
+}
+DEPLOYMENT_ROLES=[{
+    "role_name": "user",
+    "role_description": "User Role"
+}]
+ARGUMENTS_RESPONSE={
+  "sha": "some_sha",
+  "arg_schema": {
+    "some_key": "some_value"
+  }
+}
+CREATE_DEPLOYMENT_INPUT= {
+    "owner": "Owner Name",
+    "repo": "Repo Name",
+    "account_type": "github",
+    "ref": "master",
+    "region_name": "us-east-2",
+    "deployment_name": "deployment name",
+    "visibility": "private",
+    "is_dev_env": True,
+    "tags": [],
+    "build_args": {
+        "auth": {},
+        "users": {
+            "user": [{
+                "user_name": "some_user",
+                "public key": "MIIBCgKCAQEA1MuTZlPrs845FZOFm8TTeakJKr1FmW3JxAc64IafZw3WYvP1wtQOH4eSgJm5138RG1Hdg4gmWkS/4PbstxTpciwX80ARKbi8Jv7UkayeKBeLT7j7B+aRxebIJUH0THstST9nFO+10MTuNY7+AXNzfYR6PihtfmQIDAQAA",
+                "user_login": "u-185b6de2-837a-4cbb-93fc-d1c9f96f3b04"
+            }]
+        },
+        "infra_reqs":"c5.xlarge"
+    }
+}
```

### Comparing `PyOblv-0.2.0/tests/unit/test_add_service.py` & `PyOblv-0.2.1/tests/unit/test_add_service.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.service_validation_response import ServiceValidationResponse
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    INVALID_PUBLIC_KEY,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    REPO_SERVICES,
-    SERVICE_YAML_CONTENT,
-    SUCCESS,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestAddService(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN,oblivious_user_id=USER_ID)
-    
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-    
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json={KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.add_service(ref="master",repo_id="123456")
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.add_service(ref="master",repo_id="123456")
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.add_service(ref="master",repo_id="123456")
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(), "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.add_service(ref="master",repo_id="123456")
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = ServiceValidationResponse.from_dict({KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
-        self.assertEqual(self.client.add_service(ref="master",repo_id="123456",repo_name="Repo_Name",repo_owner="Owner_Name"),obj)
-        self.assertEqual(self.client.add_service(ref="master",repo_name="Repo_Name",repo_owner="Owner_Name"),obj)
-        self.assertEqual(self.client.add_service(ref="master",repo_id="123456"),obj)
-        self.assertEqual(self.client.add_service(ref="master",repo_id="123456",data=SERVICE_YAML_CONTENT),obj)
-        with self.assertRaises(BadRequestError):
-            self.client.add_service(ref="master")
-        with self.assertRaises(BadRequestError):
-            self.client.add_service(ref="master",repo_name="Repo_Name")
-        with self.assertRaises(BadRequestError):
-            self.client.add_service(ref="master",repo_owner="Owner_Name")
-        
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.service_validation_response import ServiceValidationResponse
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    INVALID_PUBLIC_KEY,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_SERVICES,
+    SERVICE_YAML_CONTENT,
+    SUCCESS,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestAddService(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN,oblivious_user_id=USER_ID)
+    
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+    
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.add_service(ref="master",repo_id="123456")
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.add_service(ref="master",repo_id="123456")
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.add_service(ref="master",repo_id="123456")
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(), "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.add_service(ref="master",repo_id="123456")
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = ServiceValidationResponse.from_dict({KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
+        self.assertEqual(self.client.add_service(ref="master",repo_id="123456",repo_name="Repo_Name",repo_owner="Owner_Name"),obj)
+        self.assertEqual(self.client.add_service(ref="master",repo_name="Repo_Name",repo_owner="Owner_Name"),obj)
+        self.assertEqual(self.client.add_service(ref="master",repo_id="123456"),obj)
+        self.assertEqual(self.client.add_service(ref="master",repo_id="123456",data=SERVICE_YAML_CONTENT),obj)
+        with self.assertRaises(BadRequestError):
+            self.client.add_service(ref="master")
+        with self.assertRaises(BadRequestError):
+            self.client.add_service(ref="master",repo_name="Repo_Name")
+        with self.assertRaises(BadRequestError):
+            self.client.add_service(ref="master",repo_owner="Owner_Name")
+        
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_available_deployments.py` & `PyOblv-0.2.1/tests/unit/test_user_accounts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,97 @@
-import imp
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.account import Account
-from oblv.models.deployment_complete import DeploymentComplete
-from oblv.models.deployment_response import DeploymentResponse
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    DEPLOYMENT,
-    EXCEPTION_OCCURED,
-    GITHUB,
-    GITHUB_USER_ID,
-    GITHUB_USER_LOGIN,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestAvailableDeployments(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=[DEPLOYMENT])
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.available_deployments()
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.available_deployments()
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.available_deployments()
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.available_deployments()
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        deployments = [DeploymentComplete.from_dict(DEPLOYMENT)]
-        self.assertEqual(self.client.available_deployments(), deployments)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import imp
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.account import Account
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    GITHUB,
+    GITHUB_USER_ID,
+    GITHUB_USER_LOGIN,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestUserAccounts(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=[
+            {
+                "user_id": GITHUB_USER_ID,
+                "user_login": GITHUB_USER_LOGIN,
+                "account_type": GITHUB
+            }
+        ])
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.accounts()
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.accounts()
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.accounts()
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.accounts()
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        accounts = [Account(GITHUB_USER_ID,GITHUB_USER_LOGIN,GITHUB)]
+        self.assertEqual(self.client.accounts(), accounts)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_create_deployment.py` & `PyOblv-0.2.1/tests/unit/test_generate_deployment_build_args.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,100 +1,94 @@
-import imp
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.account import Account
-from oblv.models.create_deployment_input import CreateDeploymentInput
-from oblv.models.deployment_response import DeploymentResponse
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    CREATE_DEPLOYMENT_INPUT,
-    DEPLOYMENT,
-    DEPLOYMENT_ID,
-    EXCEPTION_OCCURED,
-    GITHUB,
-    GITHUB_USER_ID,
-    GITHUB_USER_LOGIN,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestCreateDeployments(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    deployment_input = CreateDeploymentInput.from_dict(CREATE_DEPLOYMENT_INPUT)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(201, json={KEY_MESSAGE: "Create Deployment Initiated", "deployment_id": DEPLOYMENT_ID})
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.create_deployment(self.deployment_input)
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.create_deployment(self.deployment_input)
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.create_deployment(self.deployment_input)
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.create_deployment(self.deployment_input)
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        res = self.client.create_deployment(self.deployment_input)
-        print(type(res))
-        self.assertEqual(res.message, "Create Deployment Initiated")
-        self.assertEqual(res.deployment_id, DEPLOYMENT_ID)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import imp
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.account import Account
+from oblv.models.build_args_schema import BuildArgsSchema
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    ARGUMENTS_RESPONSE,
+    BAD_REQUEST_MESSAGE,
+    DEPLOYMENT,
+    EXCEPTION_OCCURED,
+    GITHUB,
+    GITHUB_USER_ID,
+    GITHUB_USER_LOGIN,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestAvailableDeployments(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=ARGUMENTS_RESPONSE)
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = BuildArgsSchema.from_dict(ARGUMENTS_RESPONSE)
+        self.assertEqual(self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master"), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_deployment_info.py` & `PyOblv-0.2.1/tests/unit/test_remove_deployment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import imp
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.deployment_response import DeploymentResponse
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    DEPLOYMENT,
-    DEPLOYMENT_ID,
-    EXCEPTION_OCCURED,
-    GITHUB,
-    GITHUB_USER_ID,
-    GITHUB_USER_LOGIN,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestDeploymentInfo(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=DEPLOYMENT)
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.deployment_info(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.deployment_info(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.deployment_info(DEPLOYMENT_ID)
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.deployment_info(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        deployment = DeploymentResponse.from_dict(DEPLOYMENT)
-        self.assertEqual(self.client.deployment_info(DEPLOYMENT_ID), deployment)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import imp
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.account import Account
+from oblv.models.deployment_response import DeploymentResponse
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    DEPLOYMENT,
+    DEPLOYMENT_ID,
+    EXCEPTION_OCCURED,
+    GITHUB,
+    GITHUB_USER_ID,
+    GITHUB_USER_LOGIN,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestRemoveDeployments(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(201, json={KEY_MESSAGE: "Delete Deployment Initiated"})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.remove_deployment(DEPLOYMENT_ID)
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.remove_deployment(DEPLOYMENT_ID)
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.remove_deployment(DEPLOYMENT_ID)
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.remove_deployment(DEPLOYMENT_ID)
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        self.assertEqual(self.client.remove_deployment(DEPLOYMENT_ID).message, "Delete Deployment Initiated")
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_deployment_roles.py` & `PyOblv-0.2.1/tests/unit/test_user_deployments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,93 @@
-import imp
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.account import Account
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.role_response import RoleResponse
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    DEPLOYMENT,
-    DEPLOYMENT_ID,
-    DEPLOYMENT_ROLES,
-    EXCEPTION_OCCURED,
-    GITHUB,
-    GITHUB_USER_ID,
-    GITHUB_USER_LOGIN,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestDeploymentRoles(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=DEPLOYMENT_ROLES)
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.deployment_roles(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.deployment_roles(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.deployment_roles(DEPLOYMENT_ID)
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.deployment_roles(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        deployments = [RoleResponse.from_dict(x) for x in DEPLOYMENT_ROLES]
-        self.assertEqual(self.client.deployment_roles(DEPLOYMENT_ID), deployments)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import imp
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.account import Account
+from oblv.models.deployment_response import DeploymentResponse
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    DEPLOYMENT,
+    EXCEPTION_OCCURED,
+    GITHUB,
+    GITHUB_USER_ID,
+    GITHUB_USER_LOGIN,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestUserDeployments(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=[DEPLOYMENT])
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.deployments()
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.deployments()
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.deployments()
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.deployments()
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        deployments = [DeploymentResponse.from_dict(DEPLOYMENT)]
+        self.assertEqual(self.client.deployments(), deployments)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_generate_deployment_build_args.py` & `PyOblv-0.2.1/tests/unit/test_user_services.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,93 @@
-import imp
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.account import Account
-from oblv.models.build_args_schema import BuildArgsSchema
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    ARGUMENTS_RESPONSE,
-    BAD_REQUEST_MESSAGE,
-    DEPLOYMENT,
-    EXCEPTION_OCCURED,
-    GITHUB,
-    GITHUB_USER_ID,
-    GITHUB_USER_LOGIN,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestAvailableDeployments(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=ARGUMENTS_RESPONSE)
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master")
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = BuildArgsSchema.from_dict(ARGUMENTS_RESPONSE)
-        self.assertEqual(self.client.generate_deployment_build_args("Owner_Name","Repo_Name","master"), obj)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.user_services import UserServices
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_REFS,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_SERVICES,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+    VCS_REPO_RESPONSE,
+)
+
+
+class TestUserServices(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=USER_SERVICES)
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.user_services()
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.user_services()
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.user_services()
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.user_services()
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = [UserServices.from_dict(x) for x in USER_SERVICES]
+        self.assertEqual(self.client.user_services(), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_link_repo.py` & `PyOblv-0.2.1/tests/unit/test_repo_services.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,95 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.repo import Repo
-from oblv.models.repo_all_response import RepoAllResponse
-from oblv.models.user_credit_utilization import UserCreditUtilization
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    USER_EMAIL,
-    USER_ID,
-    USER_NAME,
-    USER_REPO,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestUserLinkRepo(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=[USER_REPO])
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.link_repo("Owner_Login","Repo_Name")
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.link_repo("Owner_Login","Repo_Name")
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.link_repo("Owner_Login","Repo_Name")
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.link_repo("Owner_Login","Repo_Name")
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = RepoAllResponse.from_dict(USER_REPO)
-        self.assertEqual(self.client.link_repo("Owner_Login","Repo_Name"), [obj])
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.user_services import UserServices
+from oblv.models.validated_service import ValidatedService
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_REFS,
+    REPO_SERVICES,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_SERVICES,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+    VCS_REPO_RESPONSE,
+)
+
+
+class TestRepoServices(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=REPO_SERVICES)
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.repo_services(123456)
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.repo_services(123456)
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.repo_services(123456)
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.repo_services(123456)
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = [ValidatedService.from_dict(x) for x in REPO_SERVICES]
+        self.assertEqual(self.client.repo_services(123456), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_logout.py` & `PyOblv-0.2.1/tests/unit/test_repo_with_services.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,92 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestLogout(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN,oblivious_user_id=USER_ID)
-    
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-    
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json={KEY_MESSAGE: KEY_MESSAGE})
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.logout()
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.logout()
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.logout()
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(), "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.logout()
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        self.client.logout()
-        self.assertEqual(self.client.token, "")
-        self.assertEqual(self.client.oblivious_user_id, "")
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.repo_services import RepoServices
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_WITH_SERVICE,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+    VCS_REPO_RESPONSE,
+)
+
+
+class TestRepoWithService(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=REPO_WITH_SERVICE)
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.get_repo(123456)
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.get_repo(123456)
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.get_repo(123456)
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.get_repo(123456)
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = RepoServices.from_dict(REPO_WITH_SERVICE)
+        self.assertEqual(self.client.get_repo(123456), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_remove_deployment.py` & `PyOblv-0.2.1/tests/unit/test_available_deployments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,94 @@
-import imp
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.account import Account
-from oblv.models.deployment_response import DeploymentResponse
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    DEPLOYMENT,
-    DEPLOYMENT_ID,
-    EXCEPTION_OCCURED,
-    GITHUB,
-    GITHUB_USER_ID,
-    GITHUB_USER_LOGIN,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestRemoveDeployments(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(201, json={KEY_MESSAGE: "Delete Deployment Initiated"})
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.remove_deployment(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.remove_deployment(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.remove_deployment(DEPLOYMENT_ID)
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.remove_deployment(DEPLOYMENT_ID)
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        self.assertEqual(self.client.remove_deployment(DEPLOYMENT_ID).message, "Delete Deployment Initiated")
-
-
-if __name__ == '__main__':
-    unittest.main()
+import imp
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.account import Account
+from oblv.models.deployment_complete import DeploymentComplete
+from oblv.models.deployment_response import DeploymentResponse
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    DEPLOYMENT,
+    EXCEPTION_OCCURED,
+    GITHUB,
+    GITHUB_USER_ID,
+    GITHUB_USER_LOGIN,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestAvailableDeployments(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=[DEPLOYMENT])
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.available_deployments()
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.available_deployments()
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.available_deployments()
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.available_deployments()
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        deployments = [DeploymentComplete.from_dict(DEPLOYMENT)]
+        self.assertEqual(self.client.available_deployments(), deployments)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_remove_service.py` & `PyOblv-0.2.1/tests/unit/test_update_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,96 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.service_validation_response import ServiceValidationResponse
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    INVALID_PUBLIC_KEY,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    REPO_SERVICES,
-    SUCCESS,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestRemoveService(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN,oblivious_user_id=USER_ID)
-    
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-    
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json={KEY_MESSAGE: SUCCESS})
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.remove_service(ref="master",repo_id="123456")
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.remove_service(ref="master",repo_id="123456")
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.remove_service(ref="master",repo_id="123456")
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(), "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.remove_service(ref="master",repo_id="123456")
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        self.assertEqual(self.client.remove_service(ref="master",repo_id="123456",repo_name="Repo_Name",repo_owner="Owner_Name").message,SUCCESS)
-        self.assertEqual(self.client.remove_service(ref="master",repo_name="Repo_Name",repo_owner="Owner_Name").message,SUCCESS)
-        self.assertEqual(self.client.remove_service(ref="master",repo_id="123456").message,SUCCESS)
-        self.assertEqual(self.client.remove_service(ref="master",repo_id="123456").message,SUCCESS)
-        with self.assertRaises(BadRequestError):
-            self.client.remove_service(ref="master")
-        with self.assertRaises(BadRequestError):
-            self.client.remove_service(ref="master",repo_name="Repo_Name")
-        with self.assertRaises(BadRequestError):
-            self.client.remove_service(ref="master",repo_owner="Owner_Name")
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.service_validation_response import ServiceValidationResponse
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    INVALID_PUBLIC_KEY,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_SERVICES,
+    SERVICE_YAML_CONTENT,
+    SUCCESS,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestAddService(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN,oblivious_user_id=USER_ID)
+    
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+    
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.update_service(ref="master",repo_id="123456")
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.update_service(ref="master",repo_id="123456")
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.update_service(ref="master",repo_id="123456")
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(), "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.update_service(ref="master",repo_id="123456")
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = ServiceValidationResponse.from_dict({KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
+        self.assertEqual(self.client.update_service(ref="master",repo_id="123456",repo_name="Repo_Name",repo_owner="Owner_Name"),obj)
+        self.assertEqual(self.client.update_service(ref="master",repo_name="Repo_Name",repo_owner="Owner_Name"),obj)
+        self.assertEqual(self.client.update_service(ref="master",repo_id="123456"),obj)
+        self.assertEqual(self.client.update_service(ref="master",repo_id="123456",data=SERVICE_YAML_CONTENT),obj)
+        with self.assertRaises(BadRequestError):
+            self.client.update_service(ref="master")
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_repo_refs.py` & `PyOblv-0.2.1/tests/unit/test_user_name_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,93 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.ref_response import RefResponse
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    REPO_REFS,
-    USER_EMAIL,
-    USER_ID,
-    USER_NAME,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-    VCS_REPO_RESPONSE,
-)
-
-
-class TestRepoRefs(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=REPO_REFS)
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.repo_refs(123456)
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.repo_refs(123456)
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.repo_refs(123456)
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.repo_refs(123456)
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = RefResponse.from_dict(REPO_REFS)
-        self.assertEqual(self.client.repo_refs(123456), obj)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.user_services import UserServices
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_REFS,
+    SUCCESS,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_SERVICES,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+    VCS_REPO_RESPONSE,
+)
+
+
+class TestUserNameUpdate(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={KEY_MESSAGE: SUCCESS})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.update_name(USER_NAME)
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.update_name(USER_NAME)
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.update_name(USER_NAME)
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.update_name(USER_NAME)
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        self.assertEqual(self.client.update_name(USER_NAME).message, SUCCESS)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_repo_vcs.py` & `PyOblv-0.2.1/tests/unit/test_update_user_password.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,95 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.models.vcs_repo_response import VCSRepoResponse
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    USER_EMAIL,
-    USER_ID,
-    USER_NAME,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-    VCS_REPO_RESPONSE,
-)
-
-
-class TestUserVCSRepos(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=VCS_REPO_RESPONSE)
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.repos()
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.repos()
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.repos()
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.repos()
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = VCSRepoResponse.from_dict(VCS_REPO_RESPONSE)
-        self.assertEqual(self.client.repos(), obj)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.user_services import UserServices
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    NEW_PASS,
+    OLD_PASS,
+    RANDOM_PUBLIC_KEY,
+    REPO_REFS,
+    SUCCESS,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_SERVICES,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+    VCS_REPO_RESPONSE,
+)
+
+
+class TestUserPasswordUpdate(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={KEY_MESSAGE: SUCCESS})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.update_password(OLD_PASS,NEW_PASS)
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.update_password(OLD_PASS,NEW_PASS)
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.update_password(OLD_PASS,NEW_PASS)
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.update_password(OLD_PASS,NEW_PASS)
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        self.assertEqual(self.client.update_password(OLD_PASS,NEW_PASS).message, SUCCESS)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_revalidate_service.py` & `PyOblv-0.2.1/tests/unit/test_revalidate_service.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.ref_response import RefResponse
-from oblv.models.service_validation_response import ServiceValidationResponse
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    REPO_REFS,
-    REPO_SERVICES,
-    SERVICE_YAML_CONTENT,
-    SUCCESS,
-    USER_EMAIL,
-    USER_ID,
-    USER_NAME,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-    VCS_REPO_RESPONSE,
-)
-
-
-class TestServiceYamlContent(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json={KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.revalidate_service(123456,"master")
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.revalidate_service(123456,"master")
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.revalidate_service(123456,"master")
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.revalidate_service(123456,"master")
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = ServiceValidationResponse.from_dict({KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
-        self.assertEqual(self.client.revalidate_service(123456,"master"), obj)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.ref_response import RefResponse
+from oblv.models.service_validation_response import ServiceValidationResponse
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_REFS,
+    REPO_SERVICES,
+    SERVICE_YAML_CONTENT,
+    SUCCESS,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+    VCS_REPO_RESPONSE,
+)
+
+
+class TestServiceYamlContent(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.revalidate_service(123456,"master")
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.revalidate_service(123456,"master")
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.revalidate_service(123456,"master")
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.revalidate_service(123456,"master")
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = ServiceValidationResponse.from_dict({KEY_MESSAGE: SUCCESS, "service": REPO_SERVICES[0]})
+        self.assertEqual(self.client.revalidate_service(123456,"master"), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_service_yaml_content.py` & `PyOblv-0.2.1/tests/unit/test_user_profile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,101 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.ref_response import RefResponse
-from oblv.models.service_content_response import ServiceContentResponse
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    REPO_REFS,
-    SERVICE_YAML_CONTENT,
-    USER_EMAIL,
-    USER_ID,
-    USER_NAME,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-    VCS_REPO_RESPONSE,
-)
-
-
-class TestServiceYamlContent(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=SERVICE_YAML_CONTENT)
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.service_content(123456,"master")
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.service_content(123456,"master")
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.service_content(123456,"master")
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.service_content(123456,"master")
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = ServiceContentResponse.from_dict(SERVICE_YAML_CONTENT)
-        self.assertEqual(self.client.service_content(123456,"master"), obj)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.user_credit_utilization import UserCreditUtilization
+from oblv.models.user_profile_response import UserProfileResponse
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestUserProfile(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={
+  "oblivious_login": USER_ID,
+  "email": USER_EMAIL,
+  "user_name": USER_NAME,
+  "public_key": RANDOM_PUBLIC_KEY
+})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.user_profile()
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.user_profile()
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.user_profile()
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.user_profile()
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = UserProfileResponse.from_dict({
+  "oblivious_login": USER_ID,
+  "email": USER_EMAIL,
+  "user_name": USER_NAME,
+  "public_key": RANDOM_PUBLIC_KEY
+})
+        self.assertEqual(self.client.user_profile(), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_user_credit_usage.py` & `PyOblv-0.2.1/tests/unit/test_user_credit_usage.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.user_credit_utilization import UserCreditUtilization
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestUserCreditUsage(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json={
-            "total_credits": 0,
-            "total_running_deployments": 0,
-            "esitmated_hours_remaining": 0,
-            "hourly_credit_utilization": 0
-        })
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.credit_usage()
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.credit_usage()
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.credit_usage()
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.credit_usage()
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = UserCreditUtilization.from_dict({
-            "total_credits": 0,
-            "total_running_deployments": 0,
-            "esitmated_hours_remaining": 0,
-            "hourly_credit_utilization": 0
-        })
-        self.assertEqual(self.client.credit_usage(), obj)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.user_credit_utilization import UserCreditUtilization
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestUserCreditUsage(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={
+            "total_credits": 0,
+            "total_running_deployments": 0,
+            "esitmated_hours_remaining": 0,
+            "hourly_credit_utilization": 0
+        })
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.credit_usage()
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.credit_usage()
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.credit_usage()
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.credit_usage()
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = UserCreditUtilization.from_dict({
+            "total_credits": 0,
+            "total_running_deployments": 0,
+            "esitmated_hours_remaining": 0,
+            "hourly_credit_utilization": 0
+        })
+        self.assertEqual(self.client.credit_usage(), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_user_linked_repos.py` & `PyOblv-0.2.1/tests/unit/test_user_set_psk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,88 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.repo_all_response import RepoAllResponse
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    USER_EMAIL,
-    USER_ID,
-    USER_NAME,
-    USER_REPO,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestUserLinkedRepos(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json=[USER_REPO])
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.linked_repos()
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.linked_repos()
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.linked_repos()
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.linked_repos()
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        obj = RepoAllResponse.from_dict(USER_REPO)
-        self.assertEqual(self.client.linked_repos(), [obj])
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.psk import PSK
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    INVALID_PUBLIC_KEY,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    USER_ID,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestUserSetPsk(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN,oblivious_user_id=USER_ID)
+    
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+    
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json={"public_key": RANDOM_PUBLIC_KEY})
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.set_psk(RANDOM_PUBLIC_KEY)
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.set_psk(RANDOM_PUBLIC_KEY)
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.set_psk(INVALID_PUBLIC_KEY)
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(), "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.set_psk(RANDOM_PUBLIC_KEY)
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        psk = PSK(RANDOM_PUBLIC_KEY)
+        self.assertEqual(self.client.set_psk(RANDOM_PUBLIC_KEY),psk)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_user_name_update.py` & `PyOblv-0.2.1/tests/unit/test_link_repo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.user_services import UserServices
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    RANDOM_PUBLIC_KEY,
-    REPO_REFS,
-    SUCCESS,
-    USER_EMAIL,
-    USER_ID,
-    USER_NAME,
-    USER_SERVICES,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-    VCS_REPO_RESPONSE,
-)
-
-
-class TestUserNameUpdate(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
-
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json={KEY_MESSAGE: SUCCESS})
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.update_name(USER_NAME)
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.update_name(USER_NAME)
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.update_name(USER_NAME)
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(),
-                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.update_name(USER_NAME)
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        self.assertEqual(self.client.update_name(USER_NAME).message, SUCCESS)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.repo import Repo
+from oblv.models.repo_all_response import RepoAllResponse
+from oblv.models.user_credit_utilization import UserCreditUtilization
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_REPO,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+)
+
+
+class TestUserLinkRepo(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=[USER_REPO])
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.link_repo("Owner_Login","Repo_Name")
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.link_repo("Owner_Login","Repo_Name")
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.link_repo("Owner_Login","Repo_Name")
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.link_repo("Owner_Login","Repo_Name")
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = RepoAllResponse.from_dict(USER_REPO)
+        self.assertEqual(self.client.link_repo("Owner_Login","Repo_Name"), [obj])
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `PyOblv-0.2.0/tests/unit/test_user_psk.py` & `PyOblv-0.2.1/tests/unit/test_repo_refs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,92 @@
-import unittest
-from http.client import FORBIDDEN
-from unittest.mock import patch
-
-from httpx import Response
-
-from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
-from oblv.models.http_validation_error import HTTPValidationError
-from oblv.models.validation_error import ValidationError
-from oblv.oblv_client import OblvClient
-from tests.unit.constants import (
-    API_GW_REQUEST_ID,
-    BAD_REQUEST_MESSAGE,
-    EXCEPTION_OCCURED,
-    KEY_APIGW_REQUESTID,
-    KEY_MESSAGE,
-    KEY_VALID_ERROR_LOC,
-    USER_ID,
-    USER_TOKEN,
-    VALID_ERROR_MESSAGE,
-    VALID_ERROR_VALUE,
-)
-
-
-class TestUserPsk(unittest.TestCase):
-
-    client = OblvClient(token=USER_TOKEN,oblivious_user_id=USER_ID)
-    
-    def setUp(self) -> None:
-        super().setUp()
-
-    def getBadRequestResponse():
-        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
-        return res
-
-    def getHTTPExceptionResponse():
-        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
-                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
-        return res
-
-    def getFailedValidationResponse():
-        data = HTTPValidationError(
-            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
-        res = Response(422, json=data.to_dict())
-        return res
-    
-    def getForbiddenResponse():
-        res = Response(403, json=FORBIDDEN)
-        return res
-
-    def getSuccessResponse():
-        res = Response(200, json="user_psk")
-        return res
-    def getSuccessResponseEmpty():
-        res = Response(200, json="")
-        return res
-
-    @patch("httpx.request", return_value=getBadRequestResponse())
-    def test_bad_request(self, sync):
-        with self.assertRaises(BadRequestError) as cm:
-            self.client.psk()
-
-    @patch("httpx.request", return_value=getHTTPExceptionResponse())
-    def test_http_exception_request(self, sync):
-        with self.assertRaises(HTTPClientError) as cm:
-            self.client.psk()
-
-    @patch("httpx.request", return_value=getFailedValidationResponse())
-    def test_failed_validation_request(self, sync):
-        with self.assertRaises(ParamValidationError) as cm:
-            self.client.psk()
-
-        the_exception = cm.exception
-        self.assertEqual(the_exception.__str__(), "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
-
-    @patch("httpx.request", return_value=getForbiddenResponse())
-    def test_bad_authentication_request(self, sync):
-        with self.assertRaises(UnauthorizedTokenError):
-            self.client.psk()
-
-    @patch("httpx.request", return_value=getSuccessResponse())
-    def test_success_request(self, sync):
-        self.assertEqual(self.client.psk(), "user_psk")
-        
-    @patch("httpx.request", return_value=getSuccessResponseEmpty())
-    def test_success_request_empty(self, sync):
-        self.assertEqual(self.client.psk(), "")
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from http.client import FORBIDDEN
+from unittest.mock import patch
+
+from httpx import Response
+
+from oblv.exceptions import BadRequestError, HTTPClientError, ParamValidationError, UnauthorizedTokenError
+from oblv.models.http_validation_error import HTTPValidationError
+from oblv.models.ref_response import RefResponse
+from oblv.models.validation_error import ValidationError
+from oblv.oblv_client import OblvClient
+from tests.unit.constants import (
+    API_GW_REQUEST_ID,
+    BAD_REQUEST_MESSAGE,
+    EXCEPTION_OCCURED,
+    KEY_APIGW_REQUESTID,
+    KEY_MESSAGE,
+    KEY_VALID_ERROR_LOC,
+    RANDOM_PUBLIC_KEY,
+    REPO_REFS,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
+    USER_TOKEN,
+    VALID_ERROR_MESSAGE,
+    VALID_ERROR_VALUE,
+    VCS_REPO_RESPONSE,
+)
+
+
+class TestRepoRefs(unittest.TestCase):
+
+    client = OblvClient(token=USER_TOKEN, oblivious_user_id=USER_ID)
+
+    def setUp(self) -> None:
+        super().setUp()
+
+    def getBadRequestResponse():
+        res = Response(400, json={KEY_MESSAGE: BAD_REQUEST_MESSAGE})
+        return res
+
+    def getHTTPExceptionResponse():
+        res = Response(500, json={KEY_MESSAGE: EXCEPTION_OCCURED}, headers={
+                       KEY_APIGW_REQUESTID: API_GW_REQUEST_ID})
+        return res
+
+    def getFailedValidationResponse():
+        data = HTTPValidationError(
+            [ValidationError([KEY_VALID_ERROR_LOC], VALID_ERROR_MESSAGE, VALID_ERROR_VALUE)])
+        res = Response(422, json=data.to_dict())
+        return res
+
+    def getForbiddenResponse():
+        res = Response(403, json=FORBIDDEN)
+        return res
+
+    def getSuccessResponse():
+        res = Response(200, json=REPO_REFS)
+        return res
+
+    @patch("httpx.request", return_value=getBadRequestResponse())
+    def test_bad_request(self, sync):
+        with self.assertRaises(BadRequestError) as cm:
+            self.client.repo_refs(123456)
+
+    @patch("httpx.request", return_value=getHTTPExceptionResponse())
+    def test_http_exception_request(self, sync):
+        with self.assertRaises(HTTPClientError) as cm:
+            self.client.repo_refs(123456)
+
+    @patch("httpx.request", return_value=getFailedValidationResponse())
+    def test_failed_validation_request(self, sync):
+        with self.assertRaises(ParamValidationError) as cm:
+            self.client.repo_refs(123456)
+
+        the_exception = cm.exception
+        self.assertEqual(the_exception.__str__(),
+                         "Invalid {} provided".format(KEY_VALID_ERROR_LOC))
+
+    @patch("httpx.request", return_value=getForbiddenResponse())
+    def test_bad_authentication_request(self, sync):
+        with self.assertRaises(UnauthorizedTokenError):
+            self.client.repo_refs(123456)
+
+    @patch("httpx.request", return_value=getSuccessResponse())
+    def test_success_request(self, sync):
+        obj = RefResponse.from_dict(REPO_REFS)
+        self.assertEqual(self.client.repo_refs(123456), obj)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

