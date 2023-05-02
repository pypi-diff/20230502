# Comparing `tmp/cognite_sdk-6.1.0.tar.gz` & `tmp/cognite_sdk-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.1.0.tar", max compression
+gzip compressed data, was "cognite_sdk-6.1.1.tar", max compression
```

## Comparing `cognite_sdk-6.1.0.tar` & `cognite_sdk-6.1.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11349 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/LICENSE
--rw-r--r--   0        0        0     3945 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/README.md
--rw-r--r--   0        0        0      503 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87464 2023-04-28 08:17:52.234420 cognite_sdk-6.1.0/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17436 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44656 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49923 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21039 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     2111 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/config.py
--rw-r--r--   0        0        0    16261 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34160 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-04-28 08:17:52.238420 cognite_sdk-6.1.0/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14287 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    22565 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    13108 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9511 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    23134 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2109 2023-04-28 08:17:52.242420 cognite_sdk-6.1.0/pyproject.toml
--rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 cognite_sdk-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/LICENSE
+-rw-r--r--   0        0        0     3945 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/README.md
+-rw-r--r--   0        0        0      503 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    11025 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87464 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17436 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44656 2023-05-02 15:05:28.832164 cognite_sdk-6.1.1/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49923 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32132 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21039 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     2111 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    36997 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5245 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/config.py
+-rw-r--r--   0        0        0    16261 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34160 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-05-02 15:05:28.836164 cognite_sdk-6.1.1/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14287 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    22565 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    13108 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/py.typed
+-rw-r--r--   0        0        0     8194 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9511 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5919 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24541 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-05-02 15:05:28.840164 cognite_sdk-6.1.1/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2109 2023-05-02 15:05:28.844164 cognite_sdk-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 cognite_sdk-6.1.1/PKG-INFO
```

### Comparing `cognite_sdk-6.1.0/LICENSE` & `cognite_sdk-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/README.md` & `cognite_sdk-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/annotations.py` & `cognite_sdk-6.1.1/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/assets.py` & `cognite_sdk-6.1.1/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/data_sets.py` & `cognite_sdk-6.1.1/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.1.1/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/datapoints.py` & `cognite_sdk-6.1.1/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/diagrams.py` & `cognite_sdk-6.1.1/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.1.1/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/events.py` & `cognite_sdk-6.1.1/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.1.1/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/files.py` & `cognite_sdk-6.1.1/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/functions.py` & `cognite_sdk-6.1.1/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/geospatial.py` & `cognite_sdk-6.1.1/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/iam.py` & `cognite_sdk-6.1.1/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/labels.py` & `cognite_sdk-6.1.1/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/raw.py` & `cognite_sdk-6.1.1/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/relationships.py` & `cognite_sdk-6.1.1/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/sequences.py` & `cognite_sdk-6.1.1/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.1.1/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/templates.py` & `cognite_sdk-6.1.1/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/three_d.py` & `cognite_sdk-6.1.1/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/time_series.py` & `cognite_sdk-6.1.1/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.1.1/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.1.1/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.1.1/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.1.1/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.1.1/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api/vision.py` & `cognite_sdk-6.1.1/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_api_client.py` & `cognite_sdk-6.1.1/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_cognite_client.py` & `cognite_sdk-6.1.1/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_http_client.py` & `cognite_sdk-6.1.1/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.1.1/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.1.1/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.1/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.1.1/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.1.1/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.1.1/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.1.1/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/config.py` & `cognite_sdk-6.1.1/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/credentials.py` & `cognite_sdk-6.1.1/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/_base.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/assets.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/events.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/files.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/functions.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/iam.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/labels.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/raw.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/shared.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/templates.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.1.1/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/exceptions.py` & `cognite_sdk-6.1.1/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/testing.py` & `cognite_sdk-6.1.1/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/__init__.py` & `cognite_sdk-6.1.1/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.1.1/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.1.1/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_graph.py` & `cognite_sdk-6.1.1/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_identifier.py` & `cognite_sdk-6.1.1/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_logging.py` & `cognite_sdk-6.1.1/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.1.1/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.1.1/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.1.1/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_text.py` & `cognite_sdk-6.1.1/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_time.py` & `cognite_sdk-6.1.1/cognite/client/utils/_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 
 import math
 import numbers
 import re
 import sys
 import time
 from abc import ABC, abstractmethod
+from contextlib import suppress
 from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast, overload
 
 from cognite.client.exceptions import CogniteImportError
 from cognite.client.utils._auxiliary import local_import
 
 if TYPE_CHECKING:
+    from datetime import tzinfo
+
     import pandas
 
     if sys.version_info >= (3, 9):
-        from zoneinfo import ZoneInfo
+        from zoneinfo import ZoneInfo, ZoneInfoNotFoundError
     else:
-        from backports.zoneinfo import ZoneInfo
+        from backports.zoneinfo import ZoneInfo, ZoneInfoNotFoundError
 
 
 UNIT_IN_MS_WITHOUT_WEEK = {"s": 1000, "m": 60000, "h": 3600000, "d": 86400000}
 UNIT_IN_MS = {**UNIT_IN_MS_WITHOUT_WEEK, "w": 604800000}
 VARIABLE_LENGTH_UNITS = {"month", "quarter", "year"}
 GRANULARITY_IN_HOURS = {"w": 168, "d": 24, "h": 1}
 GRANULARITY_IN_TIMEDELTA_UNIT = {"w": "weeks", "d": "days", "h": "hours", "m": "minutes", "s": "seconds"}
 MIN_TIMESTAMP_MS = -2208988800000  # 1900-01-01 00:00:00.000
 MAX_TIMESTAMP_MS = 4102444799999  # 2099-12-31 23:59:59.999
 
 
-def import_zoneinfo() -> ZoneInfo:
+def import_zoneinfo() -> type[ZoneInfo]:
     try:
         if sys.version_info >= (3, 9):
             from zoneinfo import ZoneInfo
         else:
             from backports.zoneinfo import ZoneInfo
         return ZoneInfo  # type: ignore [return-value]
 
@@ -42,14 +45,22 @@
         raise CogniteImportError(
             "ZoneInfo is part of the standard library starting with Python >=3.9. In earlier versions "
             "you need to install a backport. This is done automatically for you when installing with the pandas "
             "group: 'cognite-sdk[pandas]', or with poetry: 'poetry install -E pandas'"
         ) from e
 
 
+def _import_zoneinfo_not_found_error() -> type[ZoneInfoNotFoundError]:
+    if sys.version_info >= (3, 9):
+        from zoneinfo import ZoneInfoNotFoundError
+    else:
+        from backports.zoneinfo import ZoneInfoNotFoundError
+    return ZoneInfoNotFoundError
+
+
 def get_utc_zoneinfo() -> ZoneInfo:
     return import_zoneinfo()("UTC")  # type: ignore [operator]
 
 
 def datetime_to_ms(dt: datetime) -> int:
     """Converts datetime object to milliseconds since epoch.
 
@@ -537,32 +548,55 @@
         freq=freq,
         inclusive=inclusive,
         nonexistent="shift_forward",
         ambiguous=True,
     )
 
 
-def validate_timezone(start: datetime, end: datetime) -> ZoneInfo:
-    ZoneInfo = import_zoneinfo()
-    pd = cast(Any, local_import("pandas"))
+def _timezones_are_equal(start_tz: tzinfo, end_tz: tzinfo) -> bool:
+    """There are unfortunately several ways to pass/represent the same timezone (without it being a user error).
+    For example pandas uses 'pytz' under the hood -except- for UTC, then it uses the built-in `datetime.timezone.utc`
+    -except- when given something concrete like pytz.UTC or ZoneInfo(...).
+
+    To make sure we don't raise something silly like 'UTC != UTC', we convert both to ZoneInfo for comparison
+    via str(). This is safe as all return the lookup key (for the IANA time zone database).
+
+    Note:
+        We do not consider timezones with different keys, but equal fixed offsets from UTC to be equal. An example
+        would be Zulu Time (which is +00:00 ahead of UTC) and UTC.
+    """
+    if start_tz is end_tz:
+        return True
+    ZoneInfo, ZoneInfoNotFoundError = import_zoneinfo(), _import_zoneinfo_not_found_error()
+    with suppress(ValueError, ZoneInfoNotFoundError):
+        # ValueError is raised for non-conforming keys (ZoneInfoNotFoundError is self-explanatory)
+        if ZoneInfo(str(start_tz)) is ZoneInfo(str(end_tz)):
+            return True
+    return False
 
-    if missing := [name for name, timestamp in zip(("start", "end"), (start, end)) if not timestamp.tzinfo]:
+
+def validate_timezone(start: datetime, end: datetime) -> ZoneInfo:
+    if (start_tz := start.tzinfo) is None or (end_tz := end.tzinfo) is None:
+        missing = [name for name, timestamp in zip(("start", "end"), (start, end)) if not timestamp.tzinfo]
         names = " and ".join(missing)
         end_sentence = " do not have timezones." if len(missing) >= 2 else " does not have a timezone."
-        raise ValueError(f"All times must be time zone aware, {names}{end_sentence}")
+        raise ValueError(f"All times must be timezone aware, {names}{end_sentence}")
 
-    is_start_valid = isinstance(start, pd.Timestamp) or isinstance(start.tzinfo, ZoneInfo)  # type: ignore [arg-type]
-    is_end_valid = isinstance(end, pd.Timestamp) or isinstance(end.tzinfo, ZoneInfo)  # type: ignore [arg-type]
-    if not is_start_valid or not is_end_valid:
-        raise ValueError("Only pandas.Timestamp or datetime with ZoneInfo implementation of tzinfo are supported.")
+    if not _timezones_are_equal(start_tz, end_tz):
+        raise ValueError(f"'start' and 'end' represent different timezones: '{start_tz}' and '{end_tz}'.")
 
-    if start.tzinfo is not end.tzinfo:
-        raise ValueError(f"start and end have different timezones, {start.tzinfo.key!r} and {end.tzinfo.key!r}.")  # type: ignore [union-attr]
+    ZoneInfo = import_zoneinfo()
+    if isinstance(start_tz, ZoneInfo):
+        return start_tz
+
+    pd = cast(Any, local_import("pandas"))
+    if isinstance(start, pd.Timestamp):
+        return ZoneInfo(str(start_tz))
 
-    return start.tzinfo  # type: ignore [return-value]
+    raise ValueError("Only tz-aware pandas.Timestamp and datetime (must be using ZoneInfo) are supported.")
 
 
 def to_pandas_freq(granularity: str, start: datetime) -> str:
     multiplier, unit = get_granularity_multiplier_and_unit(granularity, standardize=True)
 
     unit = {"s": "S", "m": "T", "h": "H", "d": "D", "w": "W-MON", "month": "MS", "quarter": "QS", "year": "AS"}.get(
         unit, unit
```

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_validation.py` & `cognite_sdk-6.1.1/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.1.1/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.0/pyproject.toml` & `cognite_sdk-6.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.1.0"
+version = "6.1.1"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
```

### Comparing `cognite_sdk-6.1.0/PKG-INFO` & `cognite_sdk-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.1.0
+Version: 6.1.1
 Summary: Cognite Python SDK
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.0 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.1 Summary: Cognite Python
 SDK Author: Erlend Vollset Author-email: erlend.vollset@cognite.com Requires-
 Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
 functions Provides-Extra: geo Provides-Extra: numpy Provides-Extra: pandas
 Provides-Extra: pyodide Provides-Extra: sympy Requires-Dist: backports-zoneinfo
```

