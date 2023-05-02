# Comparing `tmp/finbourne-insights-sdk-preview-0.0.543.tar.gz` & `tmp/finbourne-insights-sdk-preview-0.0.583.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/finbourne-insights-sdk-preview-0.0.543.tar", last modified: Wed Apr 26 11:07:23 2023, max compression
+gzip compressed data, was "dist/finbourne-insights-sdk-preview-0.0.583.tar", last modified: Tue May  2 13:42:06 2023, max compression
```

## Comparing `finbourne-insights-sdk-preview-0.0.543.tar` & `finbourne-insights-sdk-preview-0.0.583.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7610 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/
--rw-r--r--   0 root         (0) root         (0)     4102 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22053 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/access_evaluations_api.py
--rw-r--r--   0 root         (0) root         (0)     6842 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    20126 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/auditing_api.py
--rw-r--r--   0 root         (0) root         (0)    35292 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/requests_api.py
--rw-r--r--   0 root         (0) root         (0)    35457 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/vendor_logs_api.py
--rw-r--r--   0 root         (0) root         (0)    27426 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16624 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/
--rw-r--r--   0 root         (0) root         (0)     2822 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7249 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9012 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)    30629 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/access_evaluation_log.py
--rw-r--r--   0 root         (0) root         (0)     7226 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11102 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_data.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_data_summary.py
--rw-r--r--   0 root         (0) root         (0)     7641 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_entry.py
--rw-r--r--   0 root         (0) root         (0)     6257 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_entry_note.py
--rw-r--r--   0 root         (0) root         (0)     8061 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_process.py
--rw-r--r--   0 root         (0) root         (0)     5881 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_process_summary.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/bucket.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/create_audit_entry.py
--rw-r--r--   0 root         (0) root         (0)     4114 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/histogram.py
--rw-r--r--   0 root         (0) root         (0)     8016 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9505 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9534 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10699 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     6553 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10339 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/request.py
--rw-r--r--   0 root         (0) root         (0)    23331 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/request_log.py
--rw-r--r--   0 root         (0) root         (0)     5507 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource.py
--rw-r--r--   0 root         (0) root         (0)     7763 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7623 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_of_audit_process_summary.py
--rw-r--r--   0 root         (0) root         (0)     8928 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
--rw-r--r--   0 root         (0) root         (0)     8640 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
--rw-r--r--   0 root         (0) root         (0)     8608 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
--rw-r--r--   0 root         (0) root         (0)     9859 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/response.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/scrollable_collection_of_audit_entry.py
--rw-r--r--   0 root         (0) root         (0)    17885 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/vendor_log.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/vendor_request.py
--rw-r--r--   0 root         (0) root         (0)     6343 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/vendor_response.py
--rw-r--r--   0 root         (0) root         (0)    13555 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2523 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/finbourne_insights_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 11:07:23.000000 finbourne-insights-sdk-preview-0.0.543/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2270 2023-04-26 11:05:08.000000 finbourne-insights-sdk-preview-0.0.543/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7610 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/
+-rw-r--r--   0 root         (0) root         (0)     4102 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22053 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/access_evaluations_api.py
+-rw-r--r--   0 root         (0) root         (0)     6842 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    20126 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/auditing_api.py
+-rw-r--r--   0 root         (0) root         (0)    35292 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/requests_api.py
+-rw-r--r--   0 root         (0) root         (0)    35457 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/vendor_logs_api.py
+-rw-r--r--   0 root         (0) root         (0)    27426 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16624 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7249 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9012 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)    30629 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/access_evaluation_log.py
+-rw-r--r--   0 root         (0) root         (0)     7226 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11102 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_data.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_data_summary.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_entry.py
+-rw-r--r--   0 root         (0) root         (0)     6257 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_entry_note.py
+-rw-r--r--   0 root         (0) root         (0)     8061 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_process.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_process_summary.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     5122 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/create_audit_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/histogram.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9505 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9534 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10699 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/request.py
+-rw-r--r--   0 root         (0) root         (0)    23331 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/request_log.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource.py
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_of_audit_process_summary.py
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
+-rw-r--r--   0 root         (0) root         (0)     8640 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
+-rw-r--r--   0 root         (0) root         (0)     8608 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
+-rw-r--r--   0 root         (0) root         (0)     9859 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/response.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/scrollable_collection_of_audit_entry.py
+-rw-r--r--   0 root         (0) root         (0)    17885 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/vendor_log.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/vendor_request.py
+-rw-r--r--   0 root         (0) root         (0)     6343 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/vendor_response.py
+-rw-r--r--   0 root         (0) root         (0)    13555 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/finbourne_insights_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 13:42:06.000000 finbourne-insights-sdk-preview-0.0.583/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-05-02 13:39:48.000000 finbourne-insights-sdk-preview-0.0.583/setup.py
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/README.md` & `finbourne-insights-sdk-preview-0.0.583/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.543
-- Package version: 0.0.543
+- API version: 0.0.583
+- Package version: 0.0.583
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/__init__.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.0.543"
+__version__ = "0.0.583"
 
 # import apis into sdk package
 from finbourne_insights.api.access_evaluations_api import AccessEvaluationsApi
 from finbourne_insights.api.application_metadata_api import ApplicationMetadataApi
 from finbourne_insights.api.auditing_api import AuditingApi
 from finbourne_insights.api.requests_api import RequestsApi
 from finbourne_insights.api.vendor_logs_api import VendorLogsApi
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/access_evaluations_api.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/access_evaluations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "AccessEvaluationLog",
             400: "LusidValidationProblemDetails",
@@ -368,15 +368,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListWithHistogramOfAccessEvaluationLog",
             400: "LusidValidationProblemDetails",
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/application_metadata_api.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/auditing_api.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/auditing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -154,15 +154,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/json-patch+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "AuditEntry",
             429: "ProblemDetails",
@@ -288,15 +288,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAuditProcessSummary",
         }
@@ -448,15 +448,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ScrollableCollectionOfAuditEntry",
             400: "LusidValidationProblemDetails",
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/requests_api.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -162,15 +162,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Request",
             400: "LusidValidationProblemDetails",
@@ -312,15 +312,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RequestLog",
             400: "LusidValidationProblemDetails",
@@ -462,15 +462,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Response",
             400: "LusidValidationProblemDetails",
@@ -656,15 +656,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListWithHistogramOfRequestLog",
             400: "LusidValidationProblemDetails",
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api/vendor_logs_api.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api/vendor_logs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -162,15 +162,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VendorLog",
             400: "LusidValidationProblemDetails",
@@ -312,15 +312,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VendorRequest",
             400: "LusidValidationProblemDetails",
@@ -462,15 +462,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "VendorResponse",
             400: "LusidValidationProblemDetails",
@@ -656,15 +656,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.543'
+        header_params['X-LUSID-SDK-Version'] = '0.0.583'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListWithHistogramOfVendorLog",
             400: "LusidValidationProblemDetails",
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/api_client.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.543/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.583/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/configuration.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.543\n"\
-               "SDK Package Version: 0.0.543".\
+               "Version of the API: 0.0.583\n"\
+               "SDK Package Version: 0.0.583".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/exceptions.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/__init__.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/access_controlled_action.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/access_controlled_resource.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/access_controlled_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/access_evaluation_log.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/access_evaluation_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/action_id.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_data.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_data_summary.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_data_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_entry.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_entry_note.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_entry_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_process.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/audit_process_summary.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/audit_process_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/bucket.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/create_audit_entry.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/create_audit_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/histogram.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/id_selector_definition.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/identifier_part_schema.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/link.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/lusid_problem_details.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/lusid_validation_problem_details.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/lusid_validation_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/problem_details.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/request.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/request_log.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/request_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_of_access_controlled_resource.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_of_audit_process_summary.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_of_audit_process_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_with_histogram_of_request_log.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_with_histogram_of_request_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/response.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/scrollable_collection_of_audit_entry.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/scrollable_collection_of_audit_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/vendor_log.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/vendor_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/vendor_request.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/vendor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/models/vendor_response.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/models/vendor_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/rest.py` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Insights API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.543
+    The version of the OpenAPI document: 0.0.583
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights/utilities/config_keys.json` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `finbourne-insights-sdk-preview-0.0.543/finbourne_insights_sdk_preview.egg-info/SOURCES.txt` & `finbourne-insights-sdk-preview-0.0.583/finbourne_insights_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finbourne-insights-sdk-preview-0.0.543/setup.py` & `finbourne-insights-sdk-preview-0.0.583/setup.py`

 * *Files identical despite different names*

