# Comparing `tmp/flyteidl-1.4.2.tar.gz` & `tmp/flyteidl-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flyteidl-1.4.2.tar", last modified: Wed Jan  4 19:07:41 2023, max compression
+gzip compressed data, was "flyteidl-1.5.0.tar", last modified: Tue May  2 01:19:18 2023, max compression
```

## Comparing `flyteidl-1.4.2.tar` & `flyteidl-1.5.0.tar`

### file list

```diff
@@ -1,193 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.776791 flyteidl-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-01-04 19:07:33.000000 flyteidl-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-04 19:07:33.000000 flyteidl-1.4.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-04 19:07:41.776791 flyteidl-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-01-04 19:07:33.000000 flyteidl-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.756791 flyteidl-1.4.2/gen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.756791 flyteidl-1.4.2/gen/pb_python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.756791 flyteidl-1.4.2/gen/pb_python/flyteidl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.764791 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/cluster_assignment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/description_entity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/description_entity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/description_entity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/event_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/execution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/execution_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/execution_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/launch_plan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/launch_plan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/launch_plan_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/matchable_resource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/matchable_resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/node_execution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/node_execution_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/node_execution_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_attributes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_attributes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/schedule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/schedule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/schedule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/signal_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/signal_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/signal_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_execution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_execution_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_execution_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/version_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_attributes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.768791 flyteidl-1.4.2/gen/pb_python/flyteidl/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/catalog_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/catalog_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/catalog_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/compiler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/compiler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/compiler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/condition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/condition_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/condition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/dynamic_job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/dynamic_job_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/dynamic_job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/errors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/errors_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/errors_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/execution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/execution_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/execution_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/identifier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/identifier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/identifier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/interface_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/interface_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/interface_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/literals_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/literals_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/literals_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/security_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/security_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/security_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/tasks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/tasks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/tasks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/types_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_closure_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_closure_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_closure_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.768791 flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.768791 flyteidl-1.4.2/gen/pb_python/flyteidl/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/event/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/event/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/event/event_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.772791 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/array_job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/array_job_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/array_job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/dask_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/dask_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/dask_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/mpi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/mpi_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/mpi_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/presto_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/presto_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/presto_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/pytorch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/pytorch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/pytorch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/qubole_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/qubole_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/qubole_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/ray_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/ray_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/ray_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.772791 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/spark_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/spark_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/spark_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/tensorflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/tensorflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/tensorflow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/waitable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/waitable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/waitable_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.776791 flyteidl-1.4.2/gen/pb_python/flyteidl/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28969 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    97782 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/admin_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/auth_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/dataproxy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/dataproxy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/dataproxy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/identity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/identity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/identity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/signal_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/signal_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/flyteidl/service/signal_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.756791 flyteidl-1.4.2/gen/pb_python/flyteidl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-04 19:07:41.000000 flyteidl-1.4.2/gen/pb_python/flyteidl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-01-04 19:07:41.000000 flyteidl-1.4.2/gen/pb_python/flyteidl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 19:07:41.000000 flyteidl-1.4.2/gen/pb_python/flyteidl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-04 19:07:41.000000 flyteidl-1.4.2/gen/pb_python/flyteidl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-04 19:07:41.000000 flyteidl-1.4.2/gen/pb_python/flyteidl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:41.776791 flyteidl-1.4.2/gen/pb_python/validate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   110884 2023-01-04 19:07:33.000000 flyteidl-1.4.2/gen/pb_python/validate/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-01-04 19:07:41.776791 flyteidl-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-04 19:07:41.000000 flyteidl-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.349968 flyteidl-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-02 01:19:02.000000 flyteidl-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 01:19:02.000000 flyteidl-1.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 01:19:18.349968 flyteidl-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-02 01:19:02.000000 flyteidl-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.333968 flyteidl-1.5.0/gen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.333968 flyteidl-1.5.0/gen/pb_python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.333968 flyteidl-1.5.0/gen/pb_python/flyteidl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.337968 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/cluster_assignment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/description_entity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/description_entity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/description_entity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/event_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/execution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/execution_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/execution_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/launch_plan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/launch_plan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/launch_plan_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/matchable_resource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/matchable_resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/node_execution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/node_execution_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/node_execution_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_attributes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_attributes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/schedule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/schedule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/schedule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/signal_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/signal_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/signal_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_execution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_execution_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_execution_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.341968 flyteidl-1.5.0/gen/pb_python/flyteidl/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/catalog_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/catalog_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/catalog_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/compiler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/compiler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/compiler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/condition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/condition_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/condition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/dynamic_job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/dynamic_job_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/dynamic_job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/errors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/errors_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/errors_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/execution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/execution_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/execution_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/identifier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/identifier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/identifier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/interface_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/interface_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/interface_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/literals_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/literals_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/literals_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/metrics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/security_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/security_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/security_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/tasks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/tasks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/tasks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/types_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_closure_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_closure_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_closure_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.345968 flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.345968 flyteidl-1.5.0/gen/pb_python/flyteidl/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/event/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/event/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/event/event_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.345968 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/array_job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/array_job_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/array_job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/dask_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/dask_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/dask_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/mpi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/mpi_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/mpi_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/presto_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/presto_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/presto_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/pytorch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/pytorch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/pytorch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/qubole_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/qubole_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/qubole_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/ray_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/ray_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/ray_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.349968 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/spark_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/spark_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/spark_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/tensorflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/tensorflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/tensorflow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/waitable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/waitable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/waitable_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.349968 flyteidl-1.5.0/gen/pb_python/flyteidl/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29372 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    99655 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/admin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/auth_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/dataproxy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/dataproxy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/dataproxy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/external_plugin_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/external_plugin_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/external_plugin_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/identity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/identity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/identity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/signal_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/signal_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/flyteidl/service/signal_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.333968 flyteidl-1.5.0/gen/pb_python/flyteidl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 01:19:18.000000 flyteidl-1.5.0/gen/pb_python/flyteidl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-02 01:19:18.000000 flyteidl-1.5.0/gen/pb_python/flyteidl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:19:18.000000 flyteidl-1.5.0/gen/pb_python/flyteidl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 01:19:18.000000 flyteidl-1.5.0/gen/pb_python/flyteidl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 01:19:18.000000 flyteidl-1.5.0/gen/pb_python/flyteidl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:18.349968 flyteidl-1.5.0/gen/pb_python/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110884 2023-05-02 01:19:02.000000 flyteidl-1.5.0/gen/pb_python/validate/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-02 01:19:18.349968 flyteidl-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-02 01:19:15.000000 flyteidl-1.5.0/setup.py
```

### Comparing `flyteidl-1.4.2/LICENSE` & `flyteidl-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/README.md` & `flyteidl-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'flyteidl/admin/cluster_assignment.proto\x12\x0e\x66lyteidl.admin\"K\n\x11\x43lusterAssignment\x12*\n\x11\x63luster_pool_name\x18\x03 \x01(\tR\x0f\x63lusterPoolNameJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\x42\xbc\x01\n\x12\x63om.flyteidl.adminB\x16\x43lusterAssignmentProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.cluster_assignment_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.cluster_assignment_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\026ClusterAssignmentProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _CLUSTERASSIGNMENT._serialized_start=59
-  _CLUSTERASSIGNMENT._serialized_end=134
+  _globals['_CLUSTERASSIGNMENT']._serialized_start=59
+  _globals['_CLUSTERASSIGNMENT']._serialized_end=134
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/common_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/common_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,78 +9,82 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from flyteidl.core import execution_pb2 as flyteidl_dot_core_dot_execution__pb2
 from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/admin/common.proto\x12\x0e\x66lyteidl.admin\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\"]\n\x15NamedEntityIdentifier\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\"o\n\x13NamedEntityMetadata\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x36\n\x05state\x18\x02 \x01(\x0e\x32 .flyteidl.admin.NamedEntityStateR\x05state\"\xc7\x01\n\x0bNamedEntity\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x35\n\x02id\x18\x02 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\x12?\n\x08metadata\x18\x03 \x01(\x0b\x32#.flyteidl.admin.NamedEntityMetadataR\x08metadata\"\x82\x01\n\x04Sort\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12<\n\tdirection\x18\x02 \x01(\x0e\x32\x1e.flyteidl.admin.Sort.DirectionR\tdirection\"*\n\tDirection\x12\x0e\n\nDESCENDING\x10\x00\x12\r\n\tASCENDING\x10\x01\"\xc9\x01\n NamedEntityIdentifierListRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x14\n\x05limit\x18\x03 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x04 \x01(\tR\x05token\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\x12\x18\n\x07\x66ilters\x18\x06 \x01(\tR\x07\x66ilters\"\x81\x02\n\x16NamedEntityListRequest\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x18\n\x07project\x18\x02 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x03 \x01(\tR\x06\x64omain\x12\x14\n\x05limit\x18\x04 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x05 \x01(\tR\x05token\x12-\n\x07sort_by\x18\x06 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\x12\x18\n\x07\x66ilters\x18\x07 \x01(\tR\x07\x66ilters\"t\n\x19NamedEntityIdentifierList\x12\x41\n\x08\x65ntities\x18\x01 \x03(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x08\x65ntities\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"`\n\x0fNamedEntityList\x12\x37\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1b.flyteidl.admin.NamedEntityR\x08\x65ntities\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x90\x01\n\x15NamedEntityGetRequest\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x35\n\x02id\x18\x02 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\"\xd4\x01\n\x18NamedEntityUpdateRequest\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x35\n\x02id\x18\x02 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\x12?\n\x08metadata\x18\x03 \x01(\x0b\x32#.flyteidl.admin.NamedEntityMetadataR\x08metadata\"\x1b\n\x19NamedEntityUpdateResponse\"=\n\x10ObjectGetRequest\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\"\xc1\x01\n\x13ResourceListRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\">\n\x11\x45mailNotification\x12)\n\x10recipients_email\x18\x01 \x03(\tR\x0frecipientsEmail\"B\n\x15PagerDutyNotification\x12)\n\x10recipients_email\x18\x01 \x03(\tR\x0frecipientsEmail\">\n\x11SlackNotification\x12)\n\x10recipients_email\x18\x01 \x03(\tR\x0frecipientsEmail\"\x94\x02\n\x0cNotification\x12>\n\x06phases\x18\x01 \x03(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x06phases\x12\x39\n\x05\x65mail\x18\x02 \x01(\x0b\x32!.flyteidl.admin.EmailNotificationH\x00R\x05\x65mail\x12\x46\n\npager_duty\x18\x03 \x01(\x0b\x32%.flyteidl.admin.PagerDutyNotificationH\x00R\tpagerDuty\x12\x39\n\x05slack\x18\x04 \x01(\x0b\x32!.flyteidl.admin.SlackNotificationH\x00R\x05slackB\x06\n\x04type\"5\n\x07UrlBlob\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\x12\x14\n\x05\x62ytes\x18\x02 \x01(\x03R\x05\x62ytes:\x02\x18\x01\"\x7f\n\x06Labels\x12:\n\x06values\x18\x01 \x03(\x0b\x32\".flyteidl.admin.Labels.ValuesEntryR\x06values\x1a\x39\n\x0bValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\x89\x01\n\x0b\x41nnotations\x12?\n\x06values\x18\x01 \x03(\x0b\x32\'.flyteidl.admin.Annotations.ValuesEntryR\x06values\x1a\x39\n\x0bValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"z\n\x08\x41uthRole\x12,\n\x12\x61ssumable_iam_role\x18\x01 \x01(\tR\x10\x61ssumableIamRole\x12<\n\x1akubernetes_service_account\x18\x02 \x01(\tR\x18kubernetesServiceAccount:\x02\x18\x01\"K\n\x13RawOutputDataConfig\x12\x34\n\x16output_location_prefix\x18\x01 \x01(\tR\x14outputLocationPrefix*\\\n\x10NamedEntityState\x12\x17\n\x13NAMED_ENTITY_ACTIVE\x10\x00\x12\x19\n\x15NAMED_ENTITY_ARCHIVED\x10\x01\x12\x14\n\x10SYSTEM_GENERATED\x10\x02\x42\xb1\x01\n\x12\x63om.flyteidl.adminB\x0b\x43ommonProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/admin/common.proto\x12\x0e\x66lyteidl.admin\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"]\n\x15NamedEntityIdentifier\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\"o\n\x13NamedEntityMetadata\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x36\n\x05state\x18\x02 \x01(\x0e\x32 .flyteidl.admin.NamedEntityStateR\x05state\"\xc7\x01\n\x0bNamedEntity\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x35\n\x02id\x18\x02 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\x12?\n\x08metadata\x18\x03 \x01(\x0b\x32#.flyteidl.admin.NamedEntityMetadataR\x08metadata\"\x82\x01\n\x04Sort\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12<\n\tdirection\x18\x02 \x01(\x0e\x32\x1e.flyteidl.admin.Sort.DirectionR\tdirection\"*\n\tDirection\x12\x0e\n\nDESCENDING\x10\x00\x12\r\n\tASCENDING\x10\x01\"\xc9\x01\n NamedEntityIdentifierListRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x14\n\x05limit\x18\x03 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x04 \x01(\tR\x05token\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\x12\x18\n\x07\x66ilters\x18\x06 \x01(\tR\x07\x66ilters\"\x81\x02\n\x16NamedEntityListRequest\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x18\n\x07project\x18\x02 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x03 \x01(\tR\x06\x64omain\x12\x14\n\x05limit\x18\x04 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x05 \x01(\tR\x05token\x12-\n\x07sort_by\x18\x06 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\x12\x18\n\x07\x66ilters\x18\x07 \x01(\tR\x07\x66ilters\"t\n\x19NamedEntityIdentifierList\x12\x41\n\x08\x65ntities\x18\x01 \x03(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x08\x65ntities\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"`\n\x0fNamedEntityList\x12\x37\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1b.flyteidl.admin.NamedEntityR\x08\x65ntities\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x90\x01\n\x15NamedEntityGetRequest\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x35\n\x02id\x18\x02 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\"\xd4\x01\n\x18NamedEntityUpdateRequest\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x35\n\x02id\x18\x02 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\x12?\n\x08metadata\x18\x03 \x01(\x0b\x32#.flyteidl.admin.NamedEntityMetadataR\x08metadata\"\x1b\n\x19NamedEntityUpdateResponse\"=\n\x10ObjectGetRequest\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\"\xc1\x01\n\x13ResourceListRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\">\n\x11\x45mailNotification\x12)\n\x10recipients_email\x18\x01 \x03(\tR\x0frecipientsEmail\"B\n\x15PagerDutyNotification\x12)\n\x10recipients_email\x18\x01 \x03(\tR\x0frecipientsEmail\">\n\x11SlackNotification\x12)\n\x10recipients_email\x18\x01 \x03(\tR\x0frecipientsEmail\"\x94\x02\n\x0cNotification\x12>\n\x06phases\x18\x01 \x03(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x06phases\x12\x39\n\x05\x65mail\x18\x02 \x01(\x0b\x32!.flyteidl.admin.EmailNotificationH\x00R\x05\x65mail\x12\x46\n\npager_duty\x18\x03 \x01(\x0b\x32%.flyteidl.admin.PagerDutyNotificationH\x00R\tpagerDuty\x12\x39\n\x05slack\x18\x04 \x01(\x0b\x32!.flyteidl.admin.SlackNotificationH\x00R\x05slackB\x06\n\x04type\"5\n\x07UrlBlob\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\x12\x14\n\x05\x62ytes\x18\x02 \x01(\x03R\x05\x62ytes:\x02\x18\x01\"\x7f\n\x06Labels\x12:\n\x06values\x18\x01 \x03(\x0b\x32\".flyteidl.admin.Labels.ValuesEntryR\x06values\x1a\x39\n\x0bValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\x89\x01\n\x0b\x41nnotations\x12?\n\x06values\x18\x01 \x03(\x0b\x32\'.flyteidl.admin.Annotations.ValuesEntryR\x06values\x1a\x39\n\x0bValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"z\n\x08\x41uthRole\x12,\n\x12\x61ssumable_iam_role\x18\x01 \x01(\tR\x10\x61ssumableIamRole\x12<\n\x1akubernetes_service_account\x18\x02 \x01(\tR\x18kubernetesServiceAccount:\x02\x18\x01\"K\n\x13RawOutputDataConfig\x12\x34\n\x16output_location_prefix\x18\x01 \x01(\tR\x14outputLocationPrefix\"Q\n\tFlyteURLs\x12\x16\n\x06inputs\x18\x01 \x01(\tR\x06inputs\x12\x18\n\x07outputs\x18\x02 \x01(\tR\x07outputs\x12\x12\n\x04\x64\x65\x63k\x18\x03 \x01(\tR\x04\x64\x65\x63k*\\\n\x10NamedEntityState\x12\x17\n\x13NAMED_ENTITY_ACTIVE\x10\x00\x12\x19\n\x15NAMED_ENTITY_ARCHIVED\x10\x01\x12\x14\n\x10SYSTEM_GENERATED\x10\x02\x42\xb1\x01\n\x12\x63om.flyteidl.adminB\x0b\x43ommonProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\013CommonProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
   _URLBLOB._options = None
   _URLBLOB._serialized_options = b'\030\001'
   _LABELS_VALUESENTRY._options = None
   _LABELS_VALUESENTRY._serialized_options = b'8\001'
   _ANNOTATIONS_VALUESENTRY._options = None
   _ANNOTATIONS_VALUESENTRY._serialized_options = b'8\001'
   _AUTHROLE._options = None
   _AUTHROLE._serialized_options = b'\030\001'
-  _NAMEDENTITYSTATE._serialized_start=2983
-  _NAMEDENTITYSTATE._serialized_end=3075
-  _NAMEDENTITYIDENTIFIER._serialized_start=110
-  _NAMEDENTITYIDENTIFIER._serialized_end=203
-  _NAMEDENTITYMETADATA._serialized_start=205
-  _NAMEDENTITYMETADATA._serialized_end=316
-  _NAMEDENTITY._serialized_start=319
-  _NAMEDENTITY._serialized_end=518
-  _SORT._serialized_start=521
-  _SORT._serialized_end=651
-  _SORT_DIRECTION._serialized_start=609
-  _SORT_DIRECTION._serialized_end=651
-  _NAMEDENTITYIDENTIFIERLISTREQUEST._serialized_start=654
-  _NAMEDENTITYIDENTIFIERLISTREQUEST._serialized_end=855
-  _NAMEDENTITYLISTREQUEST._serialized_start=858
-  _NAMEDENTITYLISTREQUEST._serialized_end=1115
-  _NAMEDENTITYIDENTIFIERLIST._serialized_start=1117
-  _NAMEDENTITYIDENTIFIERLIST._serialized_end=1233
-  _NAMEDENTITYLIST._serialized_start=1235
-  _NAMEDENTITYLIST._serialized_end=1331
-  _NAMEDENTITYGETREQUEST._serialized_start=1334
-  _NAMEDENTITYGETREQUEST._serialized_end=1478
-  _NAMEDENTITYUPDATEREQUEST._serialized_start=1481
-  _NAMEDENTITYUPDATEREQUEST._serialized_end=1693
-  _NAMEDENTITYUPDATERESPONSE._serialized_start=1695
-  _NAMEDENTITYUPDATERESPONSE._serialized_end=1722
-  _OBJECTGETREQUEST._serialized_start=1724
-  _OBJECTGETREQUEST._serialized_end=1785
-  _RESOURCELISTREQUEST._serialized_start=1788
-  _RESOURCELISTREQUEST._serialized_end=1981
-  _EMAILNOTIFICATION._serialized_start=1983
-  _EMAILNOTIFICATION._serialized_end=2045
-  _PAGERDUTYNOTIFICATION._serialized_start=2047
-  _PAGERDUTYNOTIFICATION._serialized_end=2113
-  _SLACKNOTIFICATION._serialized_start=2115
-  _SLACKNOTIFICATION._serialized_end=2177
-  _NOTIFICATION._serialized_start=2180
-  _NOTIFICATION._serialized_end=2456
-  _URLBLOB._serialized_start=2458
-  _URLBLOB._serialized_end=2511
-  _LABELS._serialized_start=2513
-  _LABELS._serialized_end=2640
-  _LABELS_VALUESENTRY._serialized_start=2583
-  _LABELS_VALUESENTRY._serialized_end=2640
-  _ANNOTATIONS._serialized_start=2643
-  _ANNOTATIONS._serialized_end=2780
-  _ANNOTATIONS_VALUESENTRY._serialized_start=2583
-  _ANNOTATIONS_VALUESENTRY._serialized_end=2640
-  _AUTHROLE._serialized_start=2782
-  _AUTHROLE._serialized_end=2904
-  _RAWOUTPUTDATACONFIG._serialized_start=2906
-  _RAWOUTPUTDATACONFIG._serialized_end=2981
+  _globals['_NAMEDENTITYSTATE']._serialized_start=3099
+  _globals['_NAMEDENTITYSTATE']._serialized_end=3191
+  _globals['_NAMEDENTITYIDENTIFIER']._serialized_start=143
+  _globals['_NAMEDENTITYIDENTIFIER']._serialized_end=236
+  _globals['_NAMEDENTITYMETADATA']._serialized_start=238
+  _globals['_NAMEDENTITYMETADATA']._serialized_end=349
+  _globals['_NAMEDENTITY']._serialized_start=352
+  _globals['_NAMEDENTITY']._serialized_end=551
+  _globals['_SORT']._serialized_start=554
+  _globals['_SORT']._serialized_end=684
+  _globals['_SORT_DIRECTION']._serialized_start=642
+  _globals['_SORT_DIRECTION']._serialized_end=684
+  _globals['_NAMEDENTITYIDENTIFIERLISTREQUEST']._serialized_start=687
+  _globals['_NAMEDENTITYIDENTIFIERLISTREQUEST']._serialized_end=888
+  _globals['_NAMEDENTITYLISTREQUEST']._serialized_start=891
+  _globals['_NAMEDENTITYLISTREQUEST']._serialized_end=1148
+  _globals['_NAMEDENTITYIDENTIFIERLIST']._serialized_start=1150
+  _globals['_NAMEDENTITYIDENTIFIERLIST']._serialized_end=1266
+  _globals['_NAMEDENTITYLIST']._serialized_start=1268
+  _globals['_NAMEDENTITYLIST']._serialized_end=1364
+  _globals['_NAMEDENTITYGETREQUEST']._serialized_start=1367
+  _globals['_NAMEDENTITYGETREQUEST']._serialized_end=1511
+  _globals['_NAMEDENTITYUPDATEREQUEST']._serialized_start=1514
+  _globals['_NAMEDENTITYUPDATEREQUEST']._serialized_end=1726
+  _globals['_NAMEDENTITYUPDATERESPONSE']._serialized_start=1728
+  _globals['_NAMEDENTITYUPDATERESPONSE']._serialized_end=1755
+  _globals['_OBJECTGETREQUEST']._serialized_start=1757
+  _globals['_OBJECTGETREQUEST']._serialized_end=1818
+  _globals['_RESOURCELISTREQUEST']._serialized_start=1821
+  _globals['_RESOURCELISTREQUEST']._serialized_end=2014
+  _globals['_EMAILNOTIFICATION']._serialized_start=2016
+  _globals['_EMAILNOTIFICATION']._serialized_end=2078
+  _globals['_PAGERDUTYNOTIFICATION']._serialized_start=2080
+  _globals['_PAGERDUTYNOTIFICATION']._serialized_end=2146
+  _globals['_SLACKNOTIFICATION']._serialized_start=2148
+  _globals['_SLACKNOTIFICATION']._serialized_end=2210
+  _globals['_NOTIFICATION']._serialized_start=2213
+  _globals['_NOTIFICATION']._serialized_end=2489
+  _globals['_URLBLOB']._serialized_start=2491
+  _globals['_URLBLOB']._serialized_end=2544
+  _globals['_LABELS']._serialized_start=2546
+  _globals['_LABELS']._serialized_end=2673
+  _globals['_LABELS_VALUESENTRY']._serialized_start=2616
+  _globals['_LABELS_VALUESENTRY']._serialized_end=2673
+  _globals['_ANNOTATIONS']._serialized_start=2676
+  _globals['_ANNOTATIONS']._serialized_end=2813
+  _globals['_ANNOTATIONS_VALUESENTRY']._serialized_start=2616
+  _globals['_ANNOTATIONS_VALUESENTRY']._serialized_end=2673
+  _globals['_AUTHROLE']._serialized_start=2815
+  _globals['_AUTHROLE']._serialized_end=2937
+  _globals['_RAWOUTPUTDATACONFIG']._serialized_start=2939
+  _globals['_RAWOUTPUTDATACONFIG']._serialized_end=3014
+  _globals['_FLYTEURLS']._serialized_start=3016
+  _globals['_FLYTEURLS']._serialized_end=3097
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/common_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/common_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,225 +1,241 @@
 from flyteidl.core import execution_pb2 as _execution_pb2
 from flyteidl.core import identifier_pb2 as _identifier_pb2
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+
+class NamedEntityState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    NAMED_ENTITY_ACTIVE: _ClassVar[NamedEntityState]
+    NAMED_ENTITY_ARCHIVED: _ClassVar[NamedEntityState]
+    SYSTEM_GENERATED: _ClassVar[NamedEntityState]
 NAMED_ENTITY_ACTIVE: NamedEntityState
 NAMED_ENTITY_ARCHIVED: NamedEntityState
 SYSTEM_GENERATED: NamedEntityState
 
-class Annotations(_message.Message):
-    __slots__ = ["values"]
-    class ValuesEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    VALUES_FIELD_NUMBER: _ClassVar[int]
-    values: _containers.ScalarMap[str, str]
-    def __init__(self, values: _Optional[_Mapping[str, str]] = ...) -> None: ...
-
-class AuthRole(_message.Message):
-    __slots__ = ["assumable_iam_role", "kubernetes_service_account"]
-    ASSUMABLE_IAM_ROLE_FIELD_NUMBER: _ClassVar[int]
-    KUBERNETES_SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    assumable_iam_role: str
-    kubernetes_service_account: str
-    def __init__(self, assumable_iam_role: _Optional[str] = ..., kubernetes_service_account: _Optional[str] = ...) -> None: ...
-
-class EmailNotification(_message.Message):
-    __slots__ = ["recipients_email"]
-    RECIPIENTS_EMAIL_FIELD_NUMBER: _ClassVar[int]
-    recipients_email: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, recipients_email: _Optional[_Iterable[str]] = ...) -> None: ...
+class NamedEntityIdentifier(_message.Message):
+    __slots__ = ["project", "domain", "name"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    name: str
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
 
-class Labels(_message.Message):
-    __slots__ = ["values"]
-    class ValuesEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    VALUES_FIELD_NUMBER: _ClassVar[int]
-    values: _containers.ScalarMap[str, str]
-    def __init__(self, values: _Optional[_Mapping[str, str]] = ...) -> None: ...
+class NamedEntityMetadata(_message.Message):
+    __slots__ = ["description", "state"]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    STATE_FIELD_NUMBER: _ClassVar[int]
+    description: str
+    state: NamedEntityState
+    def __init__(self, description: _Optional[str] = ..., state: _Optional[_Union[NamedEntityState, str]] = ...) -> None: ...
 
 class NamedEntity(_message.Message):
-    __slots__ = ["id", "metadata", "resource_type"]
+    __slots__ = ["resource_type", "id", "metadata"]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    resource_type: _identifier_pb2.ResourceType
     id: NamedEntityIdentifier
     metadata: NamedEntityMetadata
-    resource_type: _identifier_pb2.ResourceType
     def __init__(self, resource_type: _Optional[_Union[_identifier_pb2.ResourceType, str]] = ..., id: _Optional[_Union[NamedEntityIdentifier, _Mapping]] = ..., metadata: _Optional[_Union[NamedEntityMetadata, _Mapping]] = ...) -> None: ...
 
-class NamedEntityGetRequest(_message.Message):
-    __slots__ = ["id", "resource_type"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    id: NamedEntityIdentifier
-    resource_type: _identifier_pb2.ResourceType
-    def __init__(self, resource_type: _Optional[_Union[_identifier_pb2.ResourceType, str]] = ..., id: _Optional[_Union[NamedEntityIdentifier, _Mapping]] = ...) -> None: ...
+class Sort(_message.Message):
+    __slots__ = ["key", "direction"]
+    class Direction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        DESCENDING: _ClassVar[Sort.Direction]
+        ASCENDING: _ClassVar[Sort.Direction]
+    DESCENDING: Sort.Direction
+    ASCENDING: Sort.Direction
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    DIRECTION_FIELD_NUMBER: _ClassVar[int]
+    key: str
+    direction: Sort.Direction
+    def __init__(self, key: _Optional[str] = ..., direction: _Optional[_Union[Sort.Direction, str]] = ...) -> None: ...
 
-class NamedEntityIdentifier(_message.Message):
-    __slots__ = ["domain", "name", "project"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+class NamedEntityIdentifierListRequest(_message.Message):
+    __slots__ = ["project", "domain", "limit", "token", "sort_by", "filters"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    name: str
-    project: str
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
-
-class NamedEntityIdentifierList(_message.Message):
-    __slots__ = ["entities", "token"]
-    ENTITIES_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
-    entities: _containers.RepeatedCompositeFieldContainer[NamedEntityIdentifier]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    limit: int
     token: str
-    def __init__(self, entities: _Optional[_Iterable[_Union[NamedEntityIdentifier, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
+    sort_by: Sort
+    filters: str
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., sort_by: _Optional[_Union[Sort, _Mapping]] = ..., filters: _Optional[str] = ...) -> None: ...
 
-class NamedEntityIdentifierListRequest(_message.Message):
-    __slots__ = ["domain", "filters", "limit", "project", "sort_by", "token"]
+class NamedEntityListRequest(_message.Message):
+    __slots__ = ["resource_type", "project", "domain", "limit", "token", "sort_by", "filters"]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
     DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
     LIMIT_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    resource_type: _identifier_pb2.ResourceType
+    project: str
     domain: str
-    filters: str
     limit: int
-    project: str
+    token: str
     sort_by: Sort
+    filters: str
+    def __init__(self, resource_type: _Optional[_Union[_identifier_pb2.ResourceType, str]] = ..., project: _Optional[str] = ..., domain: _Optional[str] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., sort_by: _Optional[_Union[Sort, _Mapping]] = ..., filters: _Optional[str] = ...) -> None: ...
+
+class NamedEntityIdentifierList(_message.Message):
+    __slots__ = ["entities", "token"]
+    ENTITIES_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    entities: _containers.RepeatedCompositeFieldContainer[NamedEntityIdentifier]
     token: str
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., sort_by: _Optional[_Union[Sort, _Mapping]] = ..., filters: _Optional[str] = ...) -> None: ...
+    def __init__(self, entities: _Optional[_Iterable[_Union[NamedEntityIdentifier, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
 
 class NamedEntityList(_message.Message):
     __slots__ = ["entities", "token"]
     ENTITIES_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     entities: _containers.RepeatedCompositeFieldContainer[NamedEntity]
     token: str
     def __init__(self, entities: _Optional[_Iterable[_Union[NamedEntity, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
 
-class NamedEntityListRequest(_message.Message):
-    __slots__ = ["domain", "filters", "limit", "project", "resource_type", "sort_by", "token"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
+class NamedEntityGetRequest(_message.Message):
+    __slots__ = ["resource_type", "id"]
     RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    filters: str
-    limit: int
-    project: str
+    ID_FIELD_NUMBER: _ClassVar[int]
     resource_type: _identifier_pb2.ResourceType
-    sort_by: Sort
-    token: str
-    def __init__(self, resource_type: _Optional[_Union[_identifier_pb2.ResourceType, str]] = ..., project: _Optional[str] = ..., domain: _Optional[str] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., sort_by: _Optional[_Union[Sort, _Mapping]] = ..., filters: _Optional[str] = ...) -> None: ...
-
-class NamedEntityMetadata(_message.Message):
-    __slots__ = ["description", "state"]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    STATE_FIELD_NUMBER: _ClassVar[int]
-    description: str
-    state: NamedEntityState
-    def __init__(self, description: _Optional[str] = ..., state: _Optional[_Union[NamedEntityState, str]] = ...) -> None: ...
+    id: NamedEntityIdentifier
+    def __init__(self, resource_type: _Optional[_Union[_identifier_pb2.ResourceType, str]] = ..., id: _Optional[_Union[NamedEntityIdentifier, _Mapping]] = ...) -> None: ...
 
 class NamedEntityUpdateRequest(_message.Message):
-    __slots__ = ["id", "metadata", "resource_type"]
+    __slots__ = ["resource_type", "id", "metadata"]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    resource_type: _identifier_pb2.ResourceType
     id: NamedEntityIdentifier
     metadata: NamedEntityMetadata
-    resource_type: _identifier_pb2.ResourceType
     def __init__(self, resource_type: _Optional[_Union[_identifier_pb2.ResourceType, str]] = ..., id: _Optional[_Union[NamedEntityIdentifier, _Mapping]] = ..., metadata: _Optional[_Union[NamedEntityMetadata, _Mapping]] = ...) -> None: ...
 
 class NamedEntityUpdateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class Notification(_message.Message):
-    __slots__ = ["email", "pager_duty", "phases", "slack"]
-    EMAIL_FIELD_NUMBER: _ClassVar[int]
-    PAGER_DUTY_FIELD_NUMBER: _ClassVar[int]
-    PHASES_FIELD_NUMBER: _ClassVar[int]
-    SLACK_FIELD_NUMBER: _ClassVar[int]
-    email: EmailNotification
-    pager_duty: PagerDutyNotification
-    phases: _containers.RepeatedScalarFieldContainer[_execution_pb2.WorkflowExecution.Phase]
-    slack: SlackNotification
-    def __init__(self, phases: _Optional[_Iterable[_Union[_execution_pb2.WorkflowExecution.Phase, str]]] = ..., email: _Optional[_Union[EmailNotification, _Mapping]] = ..., pager_duty: _Optional[_Union[PagerDutyNotification, _Mapping]] = ..., slack: _Optional[_Union[SlackNotification, _Mapping]] = ...) -> None: ...
-
 class ObjectGetRequest(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ...) -> None: ...
 
-class PagerDutyNotification(_message.Message):
-    __slots__ = ["recipients_email"]
-    RECIPIENTS_EMAIL_FIELD_NUMBER: _ClassVar[int]
-    recipients_email: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, recipients_email: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class RawOutputDataConfig(_message.Message):
-    __slots__ = ["output_location_prefix"]
-    OUTPUT_LOCATION_PREFIX_FIELD_NUMBER: _ClassVar[int]
-    output_location_prefix: str
-    def __init__(self, output_location_prefix: _Optional[str] = ...) -> None: ...
-
 class ResourceListRequest(_message.Message):
-    __slots__ = ["filters", "id", "limit", "sort_by", "token"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "limit", "token", "filters", "sort_by"]
     ID_FIELD_NUMBER: _ClassVar[int]
     LIMIT_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
-    filters: str
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
     id: NamedEntityIdentifier
     limit: int
-    sort_by: Sort
     token: str
+    filters: str
+    sort_by: Sort
     def __init__(self, id: _Optional[_Union[NamedEntityIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[Sort, _Mapping]] = ...) -> None: ...
 
+class EmailNotification(_message.Message):
+    __slots__ = ["recipients_email"]
+    RECIPIENTS_EMAIL_FIELD_NUMBER: _ClassVar[int]
+    recipients_email: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, recipients_email: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class PagerDutyNotification(_message.Message):
+    __slots__ = ["recipients_email"]
+    RECIPIENTS_EMAIL_FIELD_NUMBER: _ClassVar[int]
+    recipients_email: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, recipients_email: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class SlackNotification(_message.Message):
     __slots__ = ["recipients_email"]
     RECIPIENTS_EMAIL_FIELD_NUMBER: _ClassVar[int]
     recipients_email: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, recipients_email: _Optional[_Iterable[str]] = ...) -> None: ...
 
-class Sort(_message.Message):
-    __slots__ = ["direction", "key"]
-    class Direction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    ASCENDING: Sort.Direction
-    DESCENDING: Sort.Direction
-    DIRECTION_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    direction: Sort.Direction
-    key: str
-    def __init__(self, key: _Optional[str] = ..., direction: _Optional[_Union[Sort.Direction, str]] = ...) -> None: ...
+class Notification(_message.Message):
+    __slots__ = ["phases", "email", "pager_duty", "slack"]
+    PHASES_FIELD_NUMBER: _ClassVar[int]
+    EMAIL_FIELD_NUMBER: _ClassVar[int]
+    PAGER_DUTY_FIELD_NUMBER: _ClassVar[int]
+    SLACK_FIELD_NUMBER: _ClassVar[int]
+    phases: _containers.RepeatedScalarFieldContainer[_execution_pb2.WorkflowExecution.Phase]
+    email: EmailNotification
+    pager_duty: PagerDutyNotification
+    slack: SlackNotification
+    def __init__(self, phases: _Optional[_Iterable[_Union[_execution_pb2.WorkflowExecution.Phase, str]]] = ..., email: _Optional[_Union[EmailNotification, _Mapping]] = ..., pager_duty: _Optional[_Union[PagerDutyNotification, _Mapping]] = ..., slack: _Optional[_Union[SlackNotification, _Mapping]] = ...) -> None: ...
 
 class UrlBlob(_message.Message):
-    __slots__ = ["bytes", "url"]
-    BYTES_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["url", "bytes"]
     URL_FIELD_NUMBER: _ClassVar[int]
-    bytes: int
+    BYTES_FIELD_NUMBER: _ClassVar[int]
     url: str
+    bytes: int
     def __init__(self, url: _Optional[str] = ..., bytes: _Optional[int] = ...) -> None: ...
 
-class NamedEntityState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class Labels(_message.Message):
+    __slots__ = ["values"]
+    class ValuesEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.ScalarMap[str, str]
+    def __init__(self, values: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class Annotations(_message.Message):
+    __slots__ = ["values"]
+    class ValuesEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.ScalarMap[str, str]
+    def __init__(self, values: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class AuthRole(_message.Message):
+    __slots__ = ["assumable_iam_role", "kubernetes_service_account"]
+    ASSUMABLE_IAM_ROLE_FIELD_NUMBER: _ClassVar[int]
+    KUBERNETES_SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
+    assumable_iam_role: str
+    kubernetes_service_account: str
+    def __init__(self, assumable_iam_role: _Optional[str] = ..., kubernetes_service_account: _Optional[str] = ...) -> None: ...
+
+class RawOutputDataConfig(_message.Message):
+    __slots__ = ["output_location_prefix"]
+    OUTPUT_LOCATION_PREFIX_FIELD_NUMBER: _ClassVar[int]
+    output_location_prefix: str
+    def __init__(self, output_location_prefix: _Optional[str] = ...) -> None: ...
+
+class FlyteURLs(_message.Message):
+    __slots__ = ["inputs", "outputs", "deck"]
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
+    OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    DECK_FIELD_NUMBER: _ClassVar[int]
+    inputs: str
+    outputs: str
+    deck: str
+    def __init__(self, inputs: _Optional[str] = ..., outputs: _Optional[str] = ..., deck: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/description_entity_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/description_entity_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 
 from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 from flyteidl.admin import common_pb2 as flyteidl_dot_admin_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'flyteidl/admin/description_entity.proto\x12\x0e\x66lyteidl.admin\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1b\x66lyteidl/admin/common.proto\"\x84\x02\n\x11\x44\x65scriptionEntity\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12+\n\x11short_description\x18\x02 \x01(\tR\x10shortDescription\x12\x46\n\x10long_description\x18\x03 \x01(\x0b\x32\x1b.flyteidl.admin.DescriptionR\x0flongDescription\x12;\n\x0bsource_code\x18\x04 \x01(\x0b\x32\x1a.flyteidl.admin.SourceCodeR\nsourceCode\x12\x12\n\x04tags\x18\x05 \x03(\tR\x04tags\"\x9c\x01\n\x0b\x44\x65scription\x12\x16\n\x05value\x18\x01 \x01(\tH\x00R\x05value\x12\x12\n\x03uri\x18\x02 \x01(\tH\x00R\x03uri\x12\x39\n\x06\x66ormat\x18\x03 \x01(\x0e\x32!.flyteidl.admin.DescriptionFormatR\x06\x66ormat\x12\x1b\n\ticon_link\x18\x04 \x01(\tR\x08iconLinkB\t\n\x07\x63ontent\" \n\nSourceCode\x12\x12\n\x04link\x18\x01 \x01(\tR\x04link\"\x82\x01\n\x15\x44\x65scriptionEntityList\x12S\n\x13\x64\x65scriptionEntities\x18\x01 \x03(\x0b\x32!.flyteidl.admin.DescriptionEntityR\x13\x64\x65scriptionEntities\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x8c\x02\n\x1c\x44\x65scriptionEntityListRequest\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x35\n\x02id\x18\x02 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\x12\x14\n\x05limit\x18\x03 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x04 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x05 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x06 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy*\x8d\x01\n\x11\x44\x65scriptionFormat\x12\x1e\n\x1a\x44\x45SCRIPTION_FORMAT_UNKNOWN\x10\x00\x12\x1f\n\x1b\x44\x45SCRIPTION_FORMAT_MARKDOWN\x10\x01\x12\x1b\n\x17\x44\x45SCRIPTION_FORMAT_HTML\x10\x02\x12\x1a\n\x16\x44\x45SCRIPTION_FORMAT_RST\x10\x03\x42\xbc\x01\n\x12\x63om.flyteidl.adminB\x16\x44\x65scriptionEntityProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.description_entity_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.description_entity_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\026DescriptionEntityProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _DESCRIPTIONFORMAT._serialized_start=981
-  _DESCRIPTIONFORMAT._serialized_end=1122
-  _DESCRIPTIONENTITY._serialized_start=121
-  _DESCRIPTIONENTITY._serialized_end=381
-  _DESCRIPTION._serialized_start=384
-  _DESCRIPTION._serialized_end=540
-  _SOURCECODE._serialized_start=542
-  _SOURCECODE._serialized_end=574
-  _DESCRIPTIONENTITYLIST._serialized_start=577
-  _DESCRIPTIONENTITYLIST._serialized_end=707
-  _DESCRIPTIONENTITYLISTREQUEST._serialized_start=710
-  _DESCRIPTIONENTITYLISTREQUEST._serialized_end=978
+  _globals['_DESCRIPTIONFORMAT']._serialized_start=981
+  _globals['_DESCRIPTIONFORMAT']._serialized_end=1122
+  _globals['_DESCRIPTIONENTITY']._serialized_start=121
+  _globals['_DESCRIPTIONENTITY']._serialized_end=381
+  _globals['_DESCRIPTION']._serialized_start=384
+  _globals['_DESCRIPTION']._serialized_end=540
+  _globals['_SOURCECODE']._serialized_start=542
+  _globals['_SOURCECODE']._serialized_end=574
+  _globals['_DESCRIPTIONENTITYLIST']._serialized_start=577
+  _globals['_DESCRIPTIONENTITYLIST']._serialized_end=707
+  _globals['_DESCRIPTIONENTITYLISTREQUEST']._serialized_start=710
+  _globals['_DESCRIPTIONENTITYLISTREQUEST']._serialized_end=978
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/description_entity_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/description_entity_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,71 +2,75 @@
 from flyteidl.admin import common_pb2 as _common_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-DESCRIPTION_FORMAT_HTML: DescriptionFormat
-DESCRIPTION_FORMAT_MARKDOWN: DescriptionFormat
-DESCRIPTION_FORMAT_RST: DescriptionFormat
-DESCRIPTION_FORMAT_UNKNOWN: DescriptionFormat
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Description(_message.Message):
-    __slots__ = ["format", "icon_link", "uri", "value"]
-    FORMAT_FIELD_NUMBER: _ClassVar[int]
-    ICON_LINK_FIELD_NUMBER: _ClassVar[int]
-    URI_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    format: DescriptionFormat
-    icon_link: str
-    uri: str
-    value: str
-    def __init__(self, value: _Optional[str] = ..., uri: _Optional[str] = ..., format: _Optional[_Union[DescriptionFormat, str]] = ..., icon_link: _Optional[str] = ...) -> None: ...
+class DescriptionFormat(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    DESCRIPTION_FORMAT_UNKNOWN: _ClassVar[DescriptionFormat]
+    DESCRIPTION_FORMAT_MARKDOWN: _ClassVar[DescriptionFormat]
+    DESCRIPTION_FORMAT_HTML: _ClassVar[DescriptionFormat]
+    DESCRIPTION_FORMAT_RST: _ClassVar[DescriptionFormat]
+DESCRIPTION_FORMAT_UNKNOWN: DescriptionFormat
+DESCRIPTION_FORMAT_MARKDOWN: DescriptionFormat
+DESCRIPTION_FORMAT_HTML: DescriptionFormat
+DESCRIPTION_FORMAT_RST: DescriptionFormat
 
 class DescriptionEntity(_message.Message):
-    __slots__ = ["id", "long_description", "short_description", "source_code", "tags"]
+    __slots__ = ["id", "short_description", "long_description", "source_code", "tags"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    LONG_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     SHORT_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    LONG_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     SOURCE_CODE_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
-    long_description: Description
     short_description: str
+    long_description: Description
     source_code: SourceCode
     tags: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., short_description: _Optional[str] = ..., long_description: _Optional[_Union[Description, _Mapping]] = ..., source_code: _Optional[_Union[SourceCode, _Mapping]] = ..., tags: _Optional[_Iterable[str]] = ...) -> None: ...
 
+class Description(_message.Message):
+    __slots__ = ["value", "uri", "format", "icon_link"]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    URI_FIELD_NUMBER: _ClassVar[int]
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
+    ICON_LINK_FIELD_NUMBER: _ClassVar[int]
+    value: str
+    uri: str
+    format: DescriptionFormat
+    icon_link: str
+    def __init__(self, value: _Optional[str] = ..., uri: _Optional[str] = ..., format: _Optional[_Union[DescriptionFormat, str]] = ..., icon_link: _Optional[str] = ...) -> None: ...
+
+class SourceCode(_message.Message):
+    __slots__ = ["link"]
+    LINK_FIELD_NUMBER: _ClassVar[int]
+    link: str
+    def __init__(self, link: _Optional[str] = ...) -> None: ...
+
 class DescriptionEntityList(_message.Message):
     __slots__ = ["descriptionEntities", "token"]
     DESCRIPTIONENTITIES_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     descriptionEntities: _containers.RepeatedCompositeFieldContainer[DescriptionEntity]
     token: str
     def __init__(self, descriptionEntities: _Optional[_Iterable[_Union[DescriptionEntity, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
 
 class DescriptionEntityListRequest(_message.Message):
-    __slots__ = ["filters", "id", "limit", "resource_type", "sort_by", "token"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["resource_type", "id", "limit", "token", "filters", "sort_by"]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     LIMIT_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
-    filters: str
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    resource_type: _identifier_pb2.ResourceType
     id: _common_pb2.NamedEntityIdentifier
     limit: int
-    resource_type: _identifier_pb2.ResourceType
-    sort_by: _common_pb2.Sort
     token: str
+    filters: str
+    sort_by: _common_pb2.Sort
     def __init__(self, resource_type: _Optional[_Union[_identifier_pb2.ResourceType, str]] = ..., id: _Optional[_Union[_common_pb2.NamedEntityIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
-
-class SourceCode(_message.Message):
-    __slots__ = ["link"]
-    LINK_FIELD_NUMBER: _ClassVar[int]
-    link: str
-    def __init__(self, link: _Optional[str] = ...) -> None: ...
-
-class DescriptionFormat(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/event_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/external_plugin_service_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/admin/event.proto
+# source: flyteidl/service/external_plugin_service.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from flyteidl.event import event_pb2 as flyteidl_dot_event_dot_event__pb2
+from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
+from flyteidl.core import tasks_pb2 as flyteidl_dot_core_dot_tasks__pb2
+from flyteidl.core import interface_pb2 as flyteidl_dot_core_dot_interface__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66lyteidl/admin/event.proto\x12\x0e\x66lyteidl.admin\x1a\x1a\x66lyteidl/event/event.proto\"G\n EventErrorAlreadyInTerminalState\x12#\n\rcurrent_phase\x18\x01 \x01(\tR\x0c\x63urrentPhase\"9\n\x1d\x45ventErrorIncompatibleCluster\x12\x18\n\x07\x63luster\x18\x01 \x01(\tR\x07\x63luster\"\xf1\x01\n\x12\x45ventFailureReason\x12m\n\x19\x61lready_in_terminal_state\x18\x01 \x01(\x0b\x32\x30.flyteidl.admin.EventErrorAlreadyInTerminalStateH\x00R\x16\x61lreadyInTerminalState\x12\x62\n\x14incompatible_cluster\x18\x02 \x01(\x0b\x32-.flyteidl.admin.EventErrorIncompatibleClusterH\x00R\x13incompatibleClusterB\x08\n\x06reason\"|\n\x1dWorkflowExecutionEventRequest\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId\x12<\n\x05\x65vent\x18\x02 \x01(\x0b\x32&.flyteidl.event.WorkflowExecutionEventR\x05\x65vent\" \n\x1eWorkflowExecutionEventResponse\"t\n\x19NodeExecutionEventRequest\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId\x12\x38\n\x05\x65vent\x18\x02 \x01(\x0b\x32\".flyteidl.event.NodeExecutionEventR\x05\x65vent\"\x1c\n\x1aNodeExecutionEventResponse\"t\n\x19TaskExecutionEventRequest\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId\x12\x38\n\x05\x65vent\x18\x02 \x01(\x0b\x32\".flyteidl.event.TaskExecutionEventR\x05\x65vent\"\x1c\n\x1aTaskExecutionEventResponseB\xb0\x01\n\x12\x63om.flyteidl.adminB\nEventProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.flyteidl/service/external_plugin_service.proto\x12\x10\x66lyteidl.service\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x19\x66lyteidl/core/tasks.proto\x1a\x1d\x66lyteidl/core/interface.proto\"\xa4\x01\n\x11TaskCreateRequest\x12\x31\n\x06inputs\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x06inputs\x12\x37\n\x08template\x18\x02 \x01(\x0b\x32\x1b.flyteidl.core.TaskTemplateR\x08template\x12#\n\routput_prefix\x18\x03 \x01(\tR\x0coutputPrefix\"+\n\x12TaskCreateResponse\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"D\n\x0eTaskGetRequest\x12\x1b\n\ttask_type\x18\x01 \x01(\tR\x08taskType\x12\x15\n\x06job_id\x18\x02 \x01(\tR\x05jobId\"u\n\x0fTaskGetResponse\x12-\n\x05state\x18\x01 \x01(\x0e\x32\x17.flyteidl.service.StateR\x05state\x12\x33\n\x07outputs\x18\x02 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x07outputs\"G\n\x11TaskDeleteRequest\x12\x1b\n\ttask_type\x18\x01 \x01(\tR\x08taskType\x12\x15\n\x06job_id\x18\x02 \x01(\tR\x05jobId\"\x14\n\x12TaskDeleteResponse*^\n\x05State\x12\x15\n\x11RETRYABLE_FAILURE\x10\x00\x12\x15\n\x11PERMANENT_FAILURE\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\x0b\n\x07RUNNING\x10\x03\x12\r\n\tSUCCEEDED\x10\x04\x32\x9f\x02\n\x15\x45xternalPluginService\x12Y\n\nCreateTask\x12#.flyteidl.service.TaskCreateRequest\x1a$.flyteidl.service.TaskCreateResponse\"\x00\x12P\n\x07GetTask\x12 .flyteidl.service.TaskGetRequest\x1a!.flyteidl.service.TaskGetResponse\"\x00\x12Y\n\nDeleteTask\x12#.flyteidl.service.TaskDeleteRequest\x1a$.flyteidl.service.TaskDeleteResponse\"\x00\x42\xcc\x01\n\x14\x63om.flyteidl.serviceB\x1a\x45xternalPluginServiceProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.event_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.external_plugin_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\nEventProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _EVENTERRORALREADYINTERMINALSTATE._serialized_start=74
-  _EVENTERRORALREADYINTERMINALSTATE._serialized_end=145
-  _EVENTERRORINCOMPATIBLECLUSTER._serialized_start=147
-  _EVENTERRORINCOMPATIBLECLUSTER._serialized_end=204
-  _EVENTFAILUREREASON._serialized_start=207
-  _EVENTFAILUREREASON._serialized_end=448
-  _WORKFLOWEXECUTIONEVENTREQUEST._serialized_start=450
-  _WORKFLOWEXECUTIONEVENTREQUEST._serialized_end=574
-  _WORKFLOWEXECUTIONEVENTRESPONSE._serialized_start=576
-  _WORKFLOWEXECUTIONEVENTRESPONSE._serialized_end=608
-  _NODEEXECUTIONEVENTREQUEST._serialized_start=610
-  _NODEEXECUTIONEVENTREQUEST._serialized_end=726
-  _NODEEXECUTIONEVENTRESPONSE._serialized_start=728
-  _NODEEXECUTIONEVENTRESPONSE._serialized_end=756
-  _TASKEXECUTIONEVENTREQUEST._serialized_start=758
-  _TASKEXECUTIONEVENTREQUEST._serialized_end=874
-  _TASKEXECUTIONEVENTRESPONSE._serialized_start=876
-  _TASKEXECUTIONEVENTRESPONSE._serialized_end=904
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.serviceB\032ExternalPluginServiceProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\242\002\003FSX\252\002\020Flyteidl.Service\312\002\020Flyteidl\\Service\342\002\034Flyteidl\\Service\\GPBMetadata\352\002\021Flyteidl::Service'
+  _globals['_STATE']._serialized_start=652
+  _globals['_STATE']._serialized_end=746
+  _globals['_TASKCREATEREQUEST']._serialized_start=157
+  _globals['_TASKCREATEREQUEST']._serialized_end=321
+  _globals['_TASKCREATERESPONSE']._serialized_start=323
+  _globals['_TASKCREATERESPONSE']._serialized_end=366
+  _globals['_TASKGETREQUEST']._serialized_start=368
+  _globals['_TASKGETREQUEST']._serialized_end=436
+  _globals['_TASKGETRESPONSE']._serialized_start=438
+  _globals['_TASKGETRESPONSE']._serialized_end=555
+  _globals['_TASKDELETEREQUEST']._serialized_start=557
+  _globals['_TASKDELETEREQUEST']._serialized_end=628
+  _globals['_TASKDELETERESPONSE']._serialized_start=630
+  _globals['_TASKDELETERESPONSE']._serialized_end=650
+  _globals['_EXTERNALPLUGINSERVICE']._serialized_start=749
+  _globals['_EXTERNALPLUGINSERVICE']._serialized_end=1036
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/event_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/event_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -21,42 +21,42 @@
     __slots__ = ["already_in_terminal_state", "incompatible_cluster"]
     ALREADY_IN_TERMINAL_STATE_FIELD_NUMBER: _ClassVar[int]
     INCOMPATIBLE_CLUSTER_FIELD_NUMBER: _ClassVar[int]
     already_in_terminal_state: EventErrorAlreadyInTerminalState
     incompatible_cluster: EventErrorIncompatibleCluster
     def __init__(self, already_in_terminal_state: _Optional[_Union[EventErrorAlreadyInTerminalState, _Mapping]] = ..., incompatible_cluster: _Optional[_Union[EventErrorIncompatibleCluster, _Mapping]] = ...) -> None: ...
 
-class NodeExecutionEventRequest(_message.Message):
-    __slots__ = ["event", "request_id"]
-    EVENT_FIELD_NUMBER: _ClassVar[int]
+class WorkflowExecutionEventRequest(_message.Message):
+    __slots__ = ["request_id", "event"]
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
-    event: _event_pb2.NodeExecutionEvent
+    EVENT_FIELD_NUMBER: _ClassVar[int]
     request_id: str
-    def __init__(self, request_id: _Optional[str] = ..., event: _Optional[_Union[_event_pb2.NodeExecutionEvent, _Mapping]] = ...) -> None: ...
+    event: _event_pb2.WorkflowExecutionEvent
+    def __init__(self, request_id: _Optional[str] = ..., event: _Optional[_Union[_event_pb2.WorkflowExecutionEvent, _Mapping]] = ...) -> None: ...
 
-class NodeExecutionEventResponse(_message.Message):
+class WorkflowExecutionEventResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class TaskExecutionEventRequest(_message.Message):
-    __slots__ = ["event", "request_id"]
-    EVENT_FIELD_NUMBER: _ClassVar[int]
+class NodeExecutionEventRequest(_message.Message):
+    __slots__ = ["request_id", "event"]
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
-    event: _event_pb2.TaskExecutionEvent
+    EVENT_FIELD_NUMBER: _ClassVar[int]
     request_id: str
-    def __init__(self, request_id: _Optional[str] = ..., event: _Optional[_Union[_event_pb2.TaskExecutionEvent, _Mapping]] = ...) -> None: ...
+    event: _event_pb2.NodeExecutionEvent
+    def __init__(self, request_id: _Optional[str] = ..., event: _Optional[_Union[_event_pb2.NodeExecutionEvent, _Mapping]] = ...) -> None: ...
 
-class TaskExecutionEventResponse(_message.Message):
+class NodeExecutionEventResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class WorkflowExecutionEventRequest(_message.Message):
-    __slots__ = ["event", "request_id"]
-    EVENT_FIELD_NUMBER: _ClassVar[int]
+class TaskExecutionEventRequest(_message.Message):
+    __slots__ = ["request_id", "event"]
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
-    event: _event_pb2.WorkflowExecutionEvent
+    EVENT_FIELD_NUMBER: _ClassVar[int]
     request_id: str
-    def __init__(self, request_id: _Optional[str] = ..., event: _Optional[_Union[_event_pb2.WorkflowExecutionEvent, _Mapping]] = ...) -> None: ...
+    event: _event_pb2.TaskExecutionEvent
+    def __init__(self, request_id: _Optional[str] = ..., event: _Optional[_Union[_event_pb2.TaskExecutionEvent, _Mapping]] = ...) -> None: ...
 
-class WorkflowExecutionEventResponse(_message.Message):
+class TaskExecutionEventResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/execution_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/execution_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 
 
 from flyteidl.admin import cluster_assignment_pb2 as flyteidl_dot_admin_dot_cluster__assignment__pb2
 from flyteidl.admin import common_pb2 as flyteidl_dot_admin_dot_common__pb2
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 from flyteidl.core import execution_pb2 as flyteidl_dot_core_dot_execution__pb2
 from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
+from flyteidl.core import metrics_pb2 as flyteidl_dot_core_dot_metrics__pb2
 from flyteidl.core import security_pb2 as flyteidl_dot_core_dot_security__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x66lyteidl/admin/execution.proto\x12\x0e\x66lyteidl.admin\x1a\'flyteidl/admin/cluster_assignment.proto\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1c\x66lyteidl/core/security.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xc4\x01\n\x16\x45xecutionCreateRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x31\n\x04spec\x18\x04 \x01(\x0b\x32\x1d.flyteidl.admin.ExecutionSpecR\x04spec\x12\x31\n\x06inputs\x18\x05 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x06inputs\"\x99\x01\n\x18\x45xecutionRelaunchRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\'\n\x0foverwrite_cache\x18\x04 \x01(\x08R\x0eoverwriteCacheJ\x04\x08\x02\x10\x03\"\xa8\x01\n\x17\x45xecutionRecoverRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12=\n\x08metadata\x18\x03 \x01(\x0b\x32!.flyteidl.admin.ExecutionMetadataR\x08metadata\"U\n\x17\x45xecutionCreateResponse\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\"Y\n\x1bWorkflowExecutionGetRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\"\xb6\x01\n\tExecution\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x31\n\x04spec\x18\x02 \x01(\x0b\x32\x1d.flyteidl.admin.ExecutionSpecR\x04spec\x12:\n\x07\x63losure\x18\x03 \x01(\x0b\x32 .flyteidl.admin.ExecutionClosureR\x07\x63losure\"`\n\rExecutionList\x12\x39\n\nexecutions\x18\x01 \x03(\x0b\x32\x19.flyteidl.admin.ExecutionR\nexecutions\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"e\n\x0eLiteralMapBlob\x12\x37\n\x06values\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\x06values\x12\x12\n\x03uri\x18\x02 \x01(\tH\x00R\x03uriB\x06\n\x04\x64\x61ta\"C\n\rAbortMetadata\x12\x14\n\x05\x63\x61use\x18\x01 \x01(\tR\x05\x63\x61use\x12\x1c\n\tprincipal\x18\x02 \x01(\tR\tprincipal\"\x98\x07\n\x10\x45xecutionClosure\x12>\n\x07outputs\x18\x01 \x01(\x0b\x32\x1e.flyteidl.admin.LiteralMapBlobB\x02\x18\x01H\x00R\x07outputs\x12\x35\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12%\n\x0b\x61\x62ort_cause\x18\n \x01(\tB\x02\x18\x01H\x00R\nabortCause\x12\x46\n\x0e\x61\x62ort_metadata\x18\x0c \x01(\x0b\x32\x1d.flyteidl.admin.AbortMetadataH\x00R\rabortMetadata\x12@\n\x0boutput_data\x18\r \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\noutputData\x12\x46\n\x0f\x63omputed_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01R\x0e\x63omputedInputs\x12<\n\x05phase\x18\x04 \x01(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x05phase\x12\x39\n\nstarted_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartedAt\x12\x35\n\x08\x64uration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08\x64uration\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x42\n\rnotifications\x18\t \x03(\x0b\x32\x1c.flyteidl.admin.NotificationR\rnotifications\x12:\n\x0bworkflow_id\x18\x0b \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\nworkflowId\x12]\n\x14state_change_details\x18\x0e \x01(\x0b\x32+.flyteidl.admin.ExecutionStateChangeDetailsR\x12stateChangeDetailsB\x0f\n\routput_result\"=\n\x0eSystemMetadata\x12+\n\x11\x65xecution_cluster\x18\x01 \x01(\tR\x10\x65xecutionCluster\"\xba\x04\n\x11\x45xecutionMetadata\x12\x43\n\x04mode\x18\x01 \x01(\x0e\x32/.flyteidl.admin.ExecutionMetadata.ExecutionModeR\x04mode\x12\x1c\n\tprincipal\x18\x02 \x01(\tR\tprincipal\x12\x18\n\x07nesting\x18\x03 \x01(\rR\x07nesting\x12=\n\x0cscheduled_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0bscheduledAt\x12Z\n\x15parent_node_execution\x18\x05 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x13parentNodeExecution\x12[\n\x13reference_execution\x18\x10 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x12referenceExecution\x12G\n\x0fsystem_metadata\x18\x11 \x01(\x0b\x32\x1e.flyteidl.admin.SystemMetadataR\x0esystemMetadata\"g\n\rExecutionMode\x12\n\n\x06MANUAL\x10\x00\x12\r\n\tSCHEDULED\x10\x01\x12\n\n\x06SYSTEM\x10\x02\x12\x0c\n\x08RELAUNCH\x10\x03\x12\x12\n\x0e\x43HILD_WORKFLOW\x10\x04\x12\r\n\tRECOVERED\x10\x05\"V\n\x10NotificationList\x12\x42\n\rnotifications\x18\x01 \x03(\x0b\x32\x1c.flyteidl.admin.NotificationR\rnotifications\"\xd2\x07\n\rExecutionSpec\x12:\n\x0blaunch_plan\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\nlaunchPlan\x12\x35\n\x06inputs\x18\x02 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01R\x06inputs\x12=\n\x08metadata\x18\x03 \x01(\x0b\x32!.flyteidl.admin.ExecutionMetadataR\x08metadata\x12H\n\rnotifications\x18\x05 \x01(\x0b\x32 .flyteidl.admin.NotificationListH\x00R\rnotifications\x12!\n\x0b\x64isable_all\x18\x06 \x01(\x08H\x00R\ndisableAll\x12.\n\x06labels\x18\x07 \x01(\x0b\x32\x16.flyteidl.admin.LabelsR\x06labels\x12=\n\x0b\x61nnotations\x18\x08 \x01(\x0b\x32\x1b.flyteidl.admin.AnnotationsR\x0b\x61nnotations\x12I\n\x10security_context\x18\n \x01(\x0b\x32\x1e.flyteidl.core.SecurityContextR\x0fsecurityContext\x12\x39\n\tauth_role\x18\x10 \x01(\x0b\x32\x18.flyteidl.admin.AuthRoleB\x02\x18\x01R\x08\x61uthRole\x12M\n\x12quality_of_service\x18\x11 \x01(\x0b\x32\x1f.flyteidl.core.QualityOfServiceR\x10qualityOfService\x12\'\n\x0fmax_parallelism\x18\x12 \x01(\x05R\x0emaxParallelism\x12X\n\x16raw_output_data_config\x18\x13 \x01(\x0b\x32#.flyteidl.admin.RawOutputDataConfigR\x13rawOutputDataConfig\x12P\n\x12\x63luster_assignment\x18\x14 \x01(\x0b\x32!.flyteidl.admin.ClusterAssignmentR\x11\x63lusterAssignment\x12@\n\rinterruptible\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\rinterruptible\x12\'\n\x0foverwrite_cache\x18\x16 \x01(\x08R\x0eoverwriteCacheB\x18\n\x16notification_overridesJ\x04\x08\x04\x10\x05\"m\n\x19\x45xecutionTerminateRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x14\n\x05\x63\x61use\x18\x02 \x01(\tR\x05\x63\x61use\"\x1c\n\x1a\x45xecutionTerminateResponse\"]\n\x1fWorkflowExecutionGetDataRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\"\x88\x02\n WorkflowExecutionGetDataResponse\x12\x35\n\x07outputs\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x07outputs\x12\x33\n\x06inputs\x18\x02 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x06inputs\x12:\n\x0b\x66ull_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\nfullInputs\x12<\n\x0c\x66ull_outputs\x18\x04 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x0b\x66ullOutputs\"\x8a\x01\n\x16\x45xecutionUpdateRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x34\n\x05state\x18\x02 \x01(\x0e\x32\x1e.flyteidl.admin.ExecutionStateR\x05state\"\xae\x01\n\x1b\x45xecutionStateChangeDetails\x12\x34\n\x05state\x18\x01 \x01(\x0e\x32\x1e.flyteidl.admin.ExecutionStateR\x05state\x12;\n\x0boccurred_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1c\n\tprincipal\x18\x03 \x01(\tR\tprincipal\"\x19\n\x17\x45xecutionUpdateResponse*>\n\x0e\x45xecutionState\x12\x14\n\x10\x45XECUTION_ACTIVE\x10\x00\x12\x16\n\x12\x45XECUTION_ARCHIVED\x10\x01\x42\xb4\x01\n\x12\x63om.flyteidl.adminB\x0e\x45xecutionProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x66lyteidl/admin/execution.proto\x12\x0e\x66lyteidl.admin\x1a\'flyteidl/admin/cluster_assignment.proto\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1b\x66lyteidl/core/metrics.proto\x1a\x1c\x66lyteidl/core/security.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xc4\x01\n\x16\x45xecutionCreateRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x31\n\x04spec\x18\x04 \x01(\x0b\x32\x1d.flyteidl.admin.ExecutionSpecR\x04spec\x12\x31\n\x06inputs\x18\x05 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x06inputs\"\x99\x01\n\x18\x45xecutionRelaunchRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\'\n\x0foverwrite_cache\x18\x04 \x01(\x08R\x0eoverwriteCacheJ\x04\x08\x02\x10\x03\"\xa8\x01\n\x17\x45xecutionRecoverRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12=\n\x08metadata\x18\x03 \x01(\x0b\x32!.flyteidl.admin.ExecutionMetadataR\x08metadata\"U\n\x17\x45xecutionCreateResponse\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\"Y\n\x1bWorkflowExecutionGetRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\"\xb6\x01\n\tExecution\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x31\n\x04spec\x18\x02 \x01(\x0b\x32\x1d.flyteidl.admin.ExecutionSpecR\x04spec\x12:\n\x07\x63losure\x18\x03 \x01(\x0b\x32 .flyteidl.admin.ExecutionClosureR\x07\x63losure\"`\n\rExecutionList\x12\x39\n\nexecutions\x18\x01 \x03(\x0b\x32\x19.flyteidl.admin.ExecutionR\nexecutions\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"e\n\x0eLiteralMapBlob\x12\x37\n\x06values\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\x06values\x12\x12\n\x03uri\x18\x02 \x01(\tH\x00R\x03uriB\x06\n\x04\x64\x61ta\"C\n\rAbortMetadata\x12\x14\n\x05\x63\x61use\x18\x01 \x01(\tR\x05\x63\x61use\x12\x1c\n\tprincipal\x18\x02 \x01(\tR\tprincipal\"\x98\x07\n\x10\x45xecutionClosure\x12>\n\x07outputs\x18\x01 \x01(\x0b\x32\x1e.flyteidl.admin.LiteralMapBlobB\x02\x18\x01H\x00R\x07outputs\x12\x35\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12%\n\x0b\x61\x62ort_cause\x18\n \x01(\tB\x02\x18\x01H\x00R\nabortCause\x12\x46\n\x0e\x61\x62ort_metadata\x18\x0c \x01(\x0b\x32\x1d.flyteidl.admin.AbortMetadataH\x00R\rabortMetadata\x12@\n\x0boutput_data\x18\r \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\noutputData\x12\x46\n\x0f\x63omputed_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01R\x0e\x63omputedInputs\x12<\n\x05phase\x18\x04 \x01(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x05phase\x12\x39\n\nstarted_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartedAt\x12\x35\n\x08\x64uration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08\x64uration\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x42\n\rnotifications\x18\t \x03(\x0b\x32\x1c.flyteidl.admin.NotificationR\rnotifications\x12:\n\x0bworkflow_id\x18\x0b \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\nworkflowId\x12]\n\x14state_change_details\x18\x0e \x01(\x0b\x32+.flyteidl.admin.ExecutionStateChangeDetailsR\x12stateChangeDetailsB\x0f\n\routput_result\"=\n\x0eSystemMetadata\x12+\n\x11\x65xecution_cluster\x18\x01 \x01(\tR\x10\x65xecutionCluster\"\xba\x04\n\x11\x45xecutionMetadata\x12\x43\n\x04mode\x18\x01 \x01(\x0e\x32/.flyteidl.admin.ExecutionMetadata.ExecutionModeR\x04mode\x12\x1c\n\tprincipal\x18\x02 \x01(\tR\tprincipal\x12\x18\n\x07nesting\x18\x03 \x01(\rR\x07nesting\x12=\n\x0cscheduled_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0bscheduledAt\x12Z\n\x15parent_node_execution\x18\x05 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x13parentNodeExecution\x12[\n\x13reference_execution\x18\x10 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x12referenceExecution\x12G\n\x0fsystem_metadata\x18\x11 \x01(\x0b\x32\x1e.flyteidl.admin.SystemMetadataR\x0esystemMetadata\"g\n\rExecutionMode\x12\n\n\x06MANUAL\x10\x00\x12\r\n\tSCHEDULED\x10\x01\x12\n\n\x06SYSTEM\x10\x02\x12\x0c\n\x08RELAUNCH\x10\x03\x12\x12\n\x0e\x43HILD_WORKFLOW\x10\x04\x12\r\n\tRECOVERED\x10\x05\"V\n\x10NotificationList\x12\x42\n\rnotifications\x18\x01 \x03(\x0b\x32\x1c.flyteidl.admin.NotificationR\rnotifications\"\xd2\x07\n\rExecutionSpec\x12:\n\x0blaunch_plan\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\nlaunchPlan\x12\x35\n\x06inputs\x18\x02 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01R\x06inputs\x12=\n\x08metadata\x18\x03 \x01(\x0b\x32!.flyteidl.admin.ExecutionMetadataR\x08metadata\x12H\n\rnotifications\x18\x05 \x01(\x0b\x32 .flyteidl.admin.NotificationListH\x00R\rnotifications\x12!\n\x0b\x64isable_all\x18\x06 \x01(\x08H\x00R\ndisableAll\x12.\n\x06labels\x18\x07 \x01(\x0b\x32\x16.flyteidl.admin.LabelsR\x06labels\x12=\n\x0b\x61nnotations\x18\x08 \x01(\x0b\x32\x1b.flyteidl.admin.AnnotationsR\x0b\x61nnotations\x12I\n\x10security_context\x18\n \x01(\x0b\x32\x1e.flyteidl.core.SecurityContextR\x0fsecurityContext\x12\x39\n\tauth_role\x18\x10 \x01(\x0b\x32\x18.flyteidl.admin.AuthRoleB\x02\x18\x01R\x08\x61uthRole\x12M\n\x12quality_of_service\x18\x11 \x01(\x0b\x32\x1f.flyteidl.core.QualityOfServiceR\x10qualityOfService\x12\'\n\x0fmax_parallelism\x18\x12 \x01(\x05R\x0emaxParallelism\x12X\n\x16raw_output_data_config\x18\x13 \x01(\x0b\x32#.flyteidl.admin.RawOutputDataConfigR\x13rawOutputDataConfig\x12P\n\x12\x63luster_assignment\x18\x14 \x01(\x0b\x32!.flyteidl.admin.ClusterAssignmentR\x11\x63lusterAssignment\x12@\n\rinterruptible\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\rinterruptible\x12\'\n\x0foverwrite_cache\x18\x16 \x01(\x08R\x0eoverwriteCacheB\x18\n\x16notification_overridesJ\x04\x08\x04\x10\x05\"m\n\x19\x45xecutionTerminateRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x14\n\x05\x63\x61use\x18\x02 \x01(\tR\x05\x63\x61use\"\x1c\n\x1a\x45xecutionTerminateResponse\"]\n\x1fWorkflowExecutionGetDataRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\"\x88\x02\n WorkflowExecutionGetDataResponse\x12\x35\n\x07outputs\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x07outputs\x12\x33\n\x06inputs\x18\x02 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x06inputs\x12:\n\x0b\x66ull_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\nfullInputs\x12<\n\x0c\x66ull_outputs\x18\x04 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x0b\x66ullOutputs\"\x8a\x01\n\x16\x45xecutionUpdateRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x34\n\x05state\x18\x02 \x01(\x0e\x32\x1e.flyteidl.admin.ExecutionStateR\x05state\"\xae\x01\n\x1b\x45xecutionStateChangeDetails\x12\x34\n\x05state\x18\x01 \x01(\x0e\x32\x1e.flyteidl.admin.ExecutionStateR\x05state\x12;\n\x0boccurred_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1c\n\tprincipal\x18\x03 \x01(\tR\tprincipal\"\x19\n\x17\x45xecutionUpdateResponse\"v\n\"WorkflowExecutionGetMetricsRequest\x12:\n\x02id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x02id\x12\x14\n\x05\x64\x65pth\x18\x02 \x01(\x05R\x05\x64\x65pth\"N\n#WorkflowExecutionGetMetricsResponse\x12\'\n\x04span\x18\x01 \x01(\x0b\x32\x13.flyteidl.core.SpanR\x04span*>\n\x0e\x45xecutionState\x12\x14\n\x10\x45XECUTION_ACTIVE\x10\x00\x12\x16\n\x12\x45XECUTION_ARCHIVED\x10\x01\x42\xb4\x01\n\x12\x63om.flyteidl.adminB\x0e\x45xecutionProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.execution_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.execution_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\016ExecutionProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
   _LITERALMAPBLOB.fields_by_name['values']._options = None
   _LITERALMAPBLOB.fields_by_name['values']._serialized_options = b'\030\001'
   _EXECUTIONCLOSURE.fields_by_name['outputs']._options = None
@@ -44,54 +46,58 @@
   _EXECUTIONSPEC.fields_by_name['inputs']._serialized_options = b'\030\001'
   _EXECUTIONSPEC.fields_by_name['auth_role']._options = None
   _EXECUTIONSPEC.fields_by_name['auth_role']._serialized_options = b'\030\001'
   _WORKFLOWEXECUTIONGETDATARESPONSE.fields_by_name['outputs']._options = None
   _WORKFLOWEXECUTIONGETDATARESPONSE.fields_by_name['outputs']._serialized_options = b'\030\001'
   _WORKFLOWEXECUTIONGETDATARESPONSE.fields_by_name['inputs']._options = None
   _WORKFLOWEXECUTIONGETDATARESPONSE.fields_by_name['inputs']._serialized_options = b'\030\001'
-  _EXECUTIONSTATE._serialized_start=4975
-  _EXECUTIONSTATE._serialized_end=5037
-  _EXECUTIONCREATEREQUEST._serialized_start=341
-  _EXECUTIONCREATEREQUEST._serialized_end=537
-  _EXECUTIONRELAUNCHREQUEST._serialized_start=540
-  _EXECUTIONRELAUNCHREQUEST._serialized_end=693
-  _EXECUTIONRECOVERREQUEST._serialized_start=696
-  _EXECUTIONRECOVERREQUEST._serialized_end=864
-  _EXECUTIONCREATERESPONSE._serialized_start=866
-  _EXECUTIONCREATERESPONSE._serialized_end=951
-  _WORKFLOWEXECUTIONGETREQUEST._serialized_start=953
-  _WORKFLOWEXECUTIONGETREQUEST._serialized_end=1042
-  _EXECUTION._serialized_start=1045
-  _EXECUTION._serialized_end=1227
-  _EXECUTIONLIST._serialized_start=1229
-  _EXECUTIONLIST._serialized_end=1325
-  _LITERALMAPBLOB._serialized_start=1327
-  _LITERALMAPBLOB._serialized_end=1428
-  _ABORTMETADATA._serialized_start=1430
-  _ABORTMETADATA._serialized_end=1497
-  _EXECUTIONCLOSURE._serialized_start=1500
-  _EXECUTIONCLOSURE._serialized_end=2420
-  _SYSTEMMETADATA._serialized_start=2422
-  _SYSTEMMETADATA._serialized_end=2483
-  _EXECUTIONMETADATA._serialized_start=2486
-  _EXECUTIONMETADATA._serialized_end=3056
-  _EXECUTIONMETADATA_EXECUTIONMODE._serialized_start=2953
-  _EXECUTIONMETADATA_EXECUTIONMODE._serialized_end=3056
-  _NOTIFICATIONLIST._serialized_start=3058
-  _NOTIFICATIONLIST._serialized_end=3144
-  _EXECUTIONSPEC._serialized_start=3147
-  _EXECUTIONSPEC._serialized_end=4125
-  _EXECUTIONTERMINATEREQUEST._serialized_start=4127
-  _EXECUTIONTERMINATEREQUEST._serialized_end=4236
-  _EXECUTIONTERMINATERESPONSE._serialized_start=4238
-  _EXECUTIONTERMINATERESPONSE._serialized_end=4266
-  _WORKFLOWEXECUTIONGETDATAREQUEST._serialized_start=4268
-  _WORKFLOWEXECUTIONGETDATAREQUEST._serialized_end=4361
-  _WORKFLOWEXECUTIONGETDATARESPONSE._serialized_start=4364
-  _WORKFLOWEXECUTIONGETDATARESPONSE._serialized_end=4628
-  _EXECUTIONUPDATEREQUEST._serialized_start=4631
-  _EXECUTIONUPDATEREQUEST._serialized_end=4769
-  _EXECUTIONSTATECHANGEDETAILS._serialized_start=4772
-  _EXECUTIONSTATECHANGEDETAILS._serialized_end=4946
-  _EXECUTIONUPDATERESPONSE._serialized_start=4948
-  _EXECUTIONUPDATERESPONSE._serialized_end=4973
+  _globals['_EXECUTIONSTATE']._serialized_start=5204
+  _globals['_EXECUTIONSTATE']._serialized_end=5266
+  _globals['_EXECUTIONCREATEREQUEST']._serialized_start=370
+  _globals['_EXECUTIONCREATEREQUEST']._serialized_end=566
+  _globals['_EXECUTIONRELAUNCHREQUEST']._serialized_start=569
+  _globals['_EXECUTIONRELAUNCHREQUEST']._serialized_end=722
+  _globals['_EXECUTIONRECOVERREQUEST']._serialized_start=725
+  _globals['_EXECUTIONRECOVERREQUEST']._serialized_end=893
+  _globals['_EXECUTIONCREATERESPONSE']._serialized_start=895
+  _globals['_EXECUTIONCREATERESPONSE']._serialized_end=980
+  _globals['_WORKFLOWEXECUTIONGETREQUEST']._serialized_start=982
+  _globals['_WORKFLOWEXECUTIONGETREQUEST']._serialized_end=1071
+  _globals['_EXECUTION']._serialized_start=1074
+  _globals['_EXECUTION']._serialized_end=1256
+  _globals['_EXECUTIONLIST']._serialized_start=1258
+  _globals['_EXECUTIONLIST']._serialized_end=1354
+  _globals['_LITERALMAPBLOB']._serialized_start=1356
+  _globals['_LITERALMAPBLOB']._serialized_end=1457
+  _globals['_ABORTMETADATA']._serialized_start=1459
+  _globals['_ABORTMETADATA']._serialized_end=1526
+  _globals['_EXECUTIONCLOSURE']._serialized_start=1529
+  _globals['_EXECUTIONCLOSURE']._serialized_end=2449
+  _globals['_SYSTEMMETADATA']._serialized_start=2451
+  _globals['_SYSTEMMETADATA']._serialized_end=2512
+  _globals['_EXECUTIONMETADATA']._serialized_start=2515
+  _globals['_EXECUTIONMETADATA']._serialized_end=3085
+  _globals['_EXECUTIONMETADATA_EXECUTIONMODE']._serialized_start=2982
+  _globals['_EXECUTIONMETADATA_EXECUTIONMODE']._serialized_end=3085
+  _globals['_NOTIFICATIONLIST']._serialized_start=3087
+  _globals['_NOTIFICATIONLIST']._serialized_end=3173
+  _globals['_EXECUTIONSPEC']._serialized_start=3176
+  _globals['_EXECUTIONSPEC']._serialized_end=4154
+  _globals['_EXECUTIONTERMINATEREQUEST']._serialized_start=4156
+  _globals['_EXECUTIONTERMINATEREQUEST']._serialized_end=4265
+  _globals['_EXECUTIONTERMINATERESPONSE']._serialized_start=4267
+  _globals['_EXECUTIONTERMINATERESPONSE']._serialized_end=4295
+  _globals['_WORKFLOWEXECUTIONGETDATAREQUEST']._serialized_start=4297
+  _globals['_WORKFLOWEXECUTIONGETDATAREQUEST']._serialized_end=4390
+  _globals['_WORKFLOWEXECUTIONGETDATARESPONSE']._serialized_start=4393
+  _globals['_WORKFLOWEXECUTIONGETDATARESPONSE']._serialized_end=4657
+  _globals['_EXECUTIONUPDATEREQUEST']._serialized_start=4660
+  _globals['_EXECUTIONUPDATEREQUEST']._serialized_end=4798
+  _globals['_EXECUTIONSTATECHANGEDETAILS']._serialized_start=4801
+  _globals['_EXECUTIONSTATECHANGEDETAILS']._serialized_end=4975
+  _globals['_EXECUTIONUPDATERESPONSE']._serialized_start=4977
+  _globals['_EXECUTIONUPDATERESPONSE']._serialized_end=5002
+  _globals['_WORKFLOWEXECUTIONGETMETRICSREQUEST']._serialized_start=5004
+  _globals['_WORKFLOWEXECUTIONGETMETRICSREQUEST']._serialized_end=5122
+  _globals['_WORKFLOWEXECUTIONGETMETRICSRESPONSE']._serialized_start=5124
+  _globals['_WORKFLOWEXECUTIONGETMETRICSRESPONSE']._serialized_end=5202
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/execution_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/execution_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,257 +1,280 @@
 from flyteidl.admin import cluster_assignment_pb2 as _cluster_assignment_pb2
 from flyteidl.admin import common_pb2 as _common_pb2
 from flyteidl.core import literals_pb2 as _literals_pb2
 from flyteidl.core import execution_pb2 as _execution_pb2
 from flyteidl.core import identifier_pb2 as _identifier_pb2
+from flyteidl.core import metrics_pb2 as _metrics_pb2
 from flyteidl.core import security_pb2 as _security_pb2
 from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+
+class ExecutionState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    EXECUTION_ACTIVE: _ClassVar[ExecutionState]
+    EXECUTION_ARCHIVED: _ClassVar[ExecutionState]
 EXECUTION_ACTIVE: ExecutionState
 EXECUTION_ARCHIVED: ExecutionState
 
-class AbortMetadata(_message.Message):
-    __slots__ = ["cause", "principal"]
-    CAUSE_FIELD_NUMBER: _ClassVar[int]
-    PRINCIPAL_FIELD_NUMBER: _ClassVar[int]
-    cause: str
-    principal: str
-    def __init__(self, cause: _Optional[str] = ..., principal: _Optional[str] = ...) -> None: ...
+class ExecutionCreateRequest(_message.Message):
+    __slots__ = ["project", "domain", "name", "spec", "inputs"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    SPEC_FIELD_NUMBER: _ClassVar[int]
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    name: str
+    spec: ExecutionSpec
+    inputs: _literals_pb2.LiteralMap
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., name: _Optional[str] = ..., spec: _Optional[_Union[ExecutionSpec, _Mapping]] = ..., inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ...) -> None: ...
+
+class ExecutionRelaunchRequest(_message.Message):
+    __slots__ = ["id", "name", "overwrite_cache"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    OVERWRITE_CACHE_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.WorkflowExecutionIdentifier
+    name: str
+    overwrite_cache: bool
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., name: _Optional[str] = ..., overwrite_cache: bool = ...) -> None: ...
+
+class ExecutionRecoverRequest(_message.Message):
+    __slots__ = ["id", "name", "metadata"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.WorkflowExecutionIdentifier
+    name: str
+    metadata: ExecutionMetadata
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., name: _Optional[str] = ..., metadata: _Optional[_Union[ExecutionMetadata, _Mapping]] = ...) -> None: ...
+
+class ExecutionCreateResponse(_message.Message):
+    __slots__ = ["id"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.WorkflowExecutionIdentifier
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
+
+class WorkflowExecutionGetRequest(_message.Message):
+    __slots__ = ["id"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.WorkflowExecutionIdentifier
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
 class Execution(_message.Message):
-    __slots__ = ["closure", "id", "spec"]
-    CLOSURE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "spec", "closure"]
     ID_FIELD_NUMBER: _ClassVar[int]
     SPEC_FIELD_NUMBER: _ClassVar[int]
-    closure: ExecutionClosure
+    CLOSURE_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.WorkflowExecutionIdentifier
     spec: ExecutionSpec
+    closure: ExecutionClosure
     def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., spec: _Optional[_Union[ExecutionSpec, _Mapping]] = ..., closure: _Optional[_Union[ExecutionClosure, _Mapping]] = ...) -> None: ...
 
+class ExecutionList(_message.Message):
+    __slots__ = ["executions", "token"]
+    EXECUTIONS_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    executions: _containers.RepeatedCompositeFieldContainer[Execution]
+    token: str
+    def __init__(self, executions: _Optional[_Iterable[_Union[Execution, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
+
+class LiteralMapBlob(_message.Message):
+    __slots__ = ["values", "uri"]
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    URI_FIELD_NUMBER: _ClassVar[int]
+    values: _literals_pb2.LiteralMap
+    uri: str
+    def __init__(self, values: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., uri: _Optional[str] = ...) -> None: ...
+
+class AbortMetadata(_message.Message):
+    __slots__ = ["cause", "principal"]
+    CAUSE_FIELD_NUMBER: _ClassVar[int]
+    PRINCIPAL_FIELD_NUMBER: _ClassVar[int]
+    cause: str
+    principal: str
+    def __init__(self, cause: _Optional[str] = ..., principal: _Optional[str] = ...) -> None: ...
+
 class ExecutionClosure(_message.Message):
-    __slots__ = ["abort_cause", "abort_metadata", "computed_inputs", "created_at", "duration", "error", "notifications", "output_data", "outputs", "phase", "started_at", "state_change_details", "updated_at", "workflow_id"]
+    __slots__ = ["outputs", "error", "abort_cause", "abort_metadata", "output_data", "computed_inputs", "phase", "started_at", "duration", "created_at", "updated_at", "notifications", "workflow_id", "state_change_details"]
+    OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
     ABORT_CAUSE_FIELD_NUMBER: _ClassVar[int]
     ABORT_METADATA_FIELD_NUMBER: _ClassVar[int]
-    COMPUTED_INPUTS_FIELD_NUMBER: _ClassVar[int]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    DURATION_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    NOTIFICATIONS_FIELD_NUMBER: _ClassVar[int]
-    OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
+    COMPUTED_INPUTS_FIELD_NUMBER: _ClassVar[int]
     PHASE_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
-    STATE_CHANGE_DETAILS_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
+    NOTIFICATIONS_FIELD_NUMBER: _ClassVar[int]
     WORKFLOW_ID_FIELD_NUMBER: _ClassVar[int]
+    STATE_CHANGE_DETAILS_FIELD_NUMBER: _ClassVar[int]
+    outputs: LiteralMapBlob
+    error: _execution_pb2.ExecutionError
     abort_cause: str
     abort_metadata: AbortMetadata
-    computed_inputs: _literals_pb2.LiteralMap
-    created_at: _timestamp_pb2.Timestamp
-    duration: _duration_pb2.Duration
-    error: _execution_pb2.ExecutionError
-    notifications: _containers.RepeatedCompositeFieldContainer[_common_pb2.Notification]
     output_data: _literals_pb2.LiteralMap
-    outputs: LiteralMapBlob
+    computed_inputs: _literals_pb2.LiteralMap
     phase: _execution_pb2.WorkflowExecution.Phase
     started_at: _timestamp_pb2.Timestamp
-    state_change_details: ExecutionStateChangeDetails
+    duration: _duration_pb2.Duration
+    created_at: _timestamp_pb2.Timestamp
     updated_at: _timestamp_pb2.Timestamp
+    notifications: _containers.RepeatedCompositeFieldContainer[_common_pb2.Notification]
     workflow_id: _identifier_pb2.Identifier
+    state_change_details: ExecutionStateChangeDetails
     def __init__(self, outputs: _Optional[_Union[LiteralMapBlob, _Mapping]] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., abort_cause: _Optional[str] = ..., abort_metadata: _Optional[_Union[AbortMetadata, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., computed_inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., phase: _Optional[_Union[_execution_pb2.WorkflowExecution.Phase, str]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., notifications: _Optional[_Iterable[_Union[_common_pb2.Notification, _Mapping]]] = ..., workflow_id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., state_change_details: _Optional[_Union[ExecutionStateChangeDetails, _Mapping]] = ...) -> None: ...
 
-class ExecutionCreateRequest(_message.Message):
-    __slots__ = ["domain", "inputs", "name", "project", "spec"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    INPUTS_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    SPEC_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    inputs: _literals_pb2.LiteralMap
-    name: str
-    project: str
-    spec: ExecutionSpec
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., name: _Optional[str] = ..., spec: _Optional[_Union[ExecutionSpec, _Mapping]] = ..., inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ...) -> None: ...
-
-class ExecutionCreateResponse(_message.Message):
-    __slots__ = ["id"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.WorkflowExecutionIdentifier
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
-
-class ExecutionList(_message.Message):
-    __slots__ = ["executions", "token"]
-    EXECUTIONS_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    executions: _containers.RepeatedCompositeFieldContainer[Execution]
-    token: str
-    def __init__(self, executions: _Optional[_Iterable[_Union[Execution, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
+class SystemMetadata(_message.Message):
+    __slots__ = ["execution_cluster"]
+    EXECUTION_CLUSTER_FIELD_NUMBER: _ClassVar[int]
+    execution_cluster: str
+    def __init__(self, execution_cluster: _Optional[str] = ...) -> None: ...
 
 class ExecutionMetadata(_message.Message):
-    __slots__ = ["mode", "nesting", "parent_node_execution", "principal", "reference_execution", "scheduled_at", "system_metadata"]
+    __slots__ = ["mode", "principal", "nesting", "scheduled_at", "parent_node_execution", "reference_execution", "system_metadata"]
     class ExecutionMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    CHILD_WORKFLOW: ExecutionMetadata.ExecutionMode
+        MANUAL: _ClassVar[ExecutionMetadata.ExecutionMode]
+        SCHEDULED: _ClassVar[ExecutionMetadata.ExecutionMode]
+        SYSTEM: _ClassVar[ExecutionMetadata.ExecutionMode]
+        RELAUNCH: _ClassVar[ExecutionMetadata.ExecutionMode]
+        CHILD_WORKFLOW: _ClassVar[ExecutionMetadata.ExecutionMode]
+        RECOVERED: _ClassVar[ExecutionMetadata.ExecutionMode]
     MANUAL: ExecutionMetadata.ExecutionMode
+    SCHEDULED: ExecutionMetadata.ExecutionMode
+    SYSTEM: ExecutionMetadata.ExecutionMode
+    RELAUNCH: ExecutionMetadata.ExecutionMode
+    CHILD_WORKFLOW: ExecutionMetadata.ExecutionMode
+    RECOVERED: ExecutionMetadata.ExecutionMode
     MODE_FIELD_NUMBER: _ClassVar[int]
+    PRINCIPAL_FIELD_NUMBER: _ClassVar[int]
     NESTING_FIELD_NUMBER: _ClassVar[int]
+    SCHEDULED_AT_FIELD_NUMBER: _ClassVar[int]
     PARENT_NODE_EXECUTION_FIELD_NUMBER: _ClassVar[int]
-    PRINCIPAL_FIELD_NUMBER: _ClassVar[int]
-    RECOVERED: ExecutionMetadata.ExecutionMode
     REFERENCE_EXECUTION_FIELD_NUMBER: _ClassVar[int]
-    RELAUNCH: ExecutionMetadata.ExecutionMode
-    SCHEDULED: ExecutionMetadata.ExecutionMode
-    SCHEDULED_AT_FIELD_NUMBER: _ClassVar[int]
-    SYSTEM: ExecutionMetadata.ExecutionMode
     SYSTEM_METADATA_FIELD_NUMBER: _ClassVar[int]
     mode: ExecutionMetadata.ExecutionMode
+    principal: str
     nesting: int
+    scheduled_at: _timestamp_pb2.Timestamp
     parent_node_execution: _identifier_pb2.NodeExecutionIdentifier
-    principal: str
     reference_execution: _identifier_pb2.WorkflowExecutionIdentifier
-    scheduled_at: _timestamp_pb2.Timestamp
     system_metadata: SystemMetadata
     def __init__(self, mode: _Optional[_Union[ExecutionMetadata.ExecutionMode, str]] = ..., principal: _Optional[str] = ..., nesting: _Optional[int] = ..., scheduled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., parent_node_execution: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., reference_execution: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., system_metadata: _Optional[_Union[SystemMetadata, _Mapping]] = ...) -> None: ...
 
-class ExecutionRecoverRequest(_message.Message):
-    __slots__ = ["id", "metadata", "name"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.WorkflowExecutionIdentifier
-    metadata: ExecutionMetadata
-    name: str
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., name: _Optional[str] = ..., metadata: _Optional[_Union[ExecutionMetadata, _Mapping]] = ...) -> None: ...
-
-class ExecutionRelaunchRequest(_message.Message):
-    __slots__ = ["id", "name", "overwrite_cache"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OVERWRITE_CACHE_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.WorkflowExecutionIdentifier
-    name: str
-    overwrite_cache: bool
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., name: _Optional[str] = ..., overwrite_cache: bool = ...) -> None: ...
+class NotificationList(_message.Message):
+    __slots__ = ["notifications"]
+    NOTIFICATIONS_FIELD_NUMBER: _ClassVar[int]
+    notifications: _containers.RepeatedCompositeFieldContainer[_common_pb2.Notification]
+    def __init__(self, notifications: _Optional[_Iterable[_Union[_common_pb2.Notification, _Mapping]]] = ...) -> None: ...
 
 class ExecutionSpec(_message.Message):
-    __slots__ = ["annotations", "auth_role", "cluster_assignment", "disable_all", "inputs", "interruptible", "labels", "launch_plan", "max_parallelism", "metadata", "notifications", "overwrite_cache", "quality_of_service", "raw_output_data_config", "security_context"]
-    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
-    AUTH_ROLE_FIELD_NUMBER: _ClassVar[int]
-    CLUSTER_ASSIGNMENT_FIELD_NUMBER: _ClassVar[int]
-    DISABLE_ALL_FIELD_NUMBER: _ClassVar[int]
-    INPUTS_FIELD_NUMBER: _ClassVar[int]
-    INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
-    LABELS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["launch_plan", "inputs", "metadata", "notifications", "disable_all", "labels", "annotations", "security_context", "auth_role", "quality_of_service", "max_parallelism", "raw_output_data_config", "cluster_assignment", "interruptible", "overwrite_cache"]
     LAUNCH_PLAN_FIELD_NUMBER: _ClassVar[int]
-    MAX_PARALLELISM_FIELD_NUMBER: _ClassVar[int]
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     NOTIFICATIONS_FIELD_NUMBER: _ClassVar[int]
-    OVERWRITE_CACHE_FIELD_NUMBER: _ClassVar[int]
+    DISABLE_ALL_FIELD_NUMBER: _ClassVar[int]
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
+    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    AUTH_ROLE_FIELD_NUMBER: _ClassVar[int]
     QUALITY_OF_SERVICE_FIELD_NUMBER: _ClassVar[int]
+    MAX_PARALLELISM_FIELD_NUMBER: _ClassVar[int]
     RAW_OUTPUT_DATA_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    annotations: _common_pb2.Annotations
-    auth_role: _common_pb2.AuthRole
-    cluster_assignment: _cluster_assignment_pb2.ClusterAssignment
-    disable_all: bool
-    inputs: _literals_pb2.LiteralMap
-    interruptible: _wrappers_pb2.BoolValue
-    labels: _common_pb2.Labels
+    CLUSTER_ASSIGNMENT_FIELD_NUMBER: _ClassVar[int]
+    INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
+    OVERWRITE_CACHE_FIELD_NUMBER: _ClassVar[int]
     launch_plan: _identifier_pb2.Identifier
-    max_parallelism: int
+    inputs: _literals_pb2.LiteralMap
     metadata: ExecutionMetadata
     notifications: NotificationList
-    overwrite_cache: bool
+    disable_all: bool
+    labels: _common_pb2.Labels
+    annotations: _common_pb2.Annotations
+    security_context: _security_pb2.SecurityContext
+    auth_role: _common_pb2.AuthRole
     quality_of_service: _execution_pb2.QualityOfService
+    max_parallelism: int
     raw_output_data_config: _common_pb2.RawOutputDataConfig
-    security_context: _security_pb2.SecurityContext
+    cluster_assignment: _cluster_assignment_pb2.ClusterAssignment
+    interruptible: _wrappers_pb2.BoolValue
+    overwrite_cache: bool
     def __init__(self, launch_plan: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., metadata: _Optional[_Union[ExecutionMetadata, _Mapping]] = ..., notifications: _Optional[_Union[NotificationList, _Mapping]] = ..., disable_all: bool = ..., labels: _Optional[_Union[_common_pb2.Labels, _Mapping]] = ..., annotations: _Optional[_Union[_common_pb2.Annotations, _Mapping]] = ..., security_context: _Optional[_Union[_security_pb2.SecurityContext, _Mapping]] = ..., auth_role: _Optional[_Union[_common_pb2.AuthRole, _Mapping]] = ..., quality_of_service: _Optional[_Union[_execution_pb2.QualityOfService, _Mapping]] = ..., max_parallelism: _Optional[int] = ..., raw_output_data_config: _Optional[_Union[_common_pb2.RawOutputDataConfig, _Mapping]] = ..., cluster_assignment: _Optional[_Union[_cluster_assignment_pb2.ClusterAssignment, _Mapping]] = ..., interruptible: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., overwrite_cache: bool = ...) -> None: ...
 
-class ExecutionStateChangeDetails(_message.Message):
-    __slots__ = ["occurred_at", "principal", "state"]
-    OCCURRED_AT_FIELD_NUMBER: _ClassVar[int]
-    PRINCIPAL_FIELD_NUMBER: _ClassVar[int]
-    STATE_FIELD_NUMBER: _ClassVar[int]
-    occurred_at: _timestamp_pb2.Timestamp
-    principal: str
-    state: ExecutionState
-    def __init__(self, state: _Optional[_Union[ExecutionState, str]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., principal: _Optional[str] = ...) -> None: ...
-
 class ExecutionTerminateRequest(_message.Message):
-    __slots__ = ["cause", "id"]
-    CAUSE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "cause"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    cause: str
+    CAUSE_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.WorkflowExecutionIdentifier
+    cause: str
     def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., cause: _Optional[str] = ...) -> None: ...
 
 class ExecutionTerminateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class ExecutionUpdateRequest(_message.Message):
-    __slots__ = ["id", "state"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    STATE_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.WorkflowExecutionIdentifier
-    state: ExecutionState
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., state: _Optional[_Union[ExecutionState, str]] = ...) -> None: ...
-
-class ExecutionUpdateResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class LiteralMapBlob(_message.Message):
-    __slots__ = ["uri", "values"]
-    URI_FIELD_NUMBER: _ClassVar[int]
-    VALUES_FIELD_NUMBER: _ClassVar[int]
-    uri: str
-    values: _literals_pb2.LiteralMap
-    def __init__(self, values: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., uri: _Optional[str] = ...) -> None: ...
-
-class NotificationList(_message.Message):
-    __slots__ = ["notifications"]
-    NOTIFICATIONS_FIELD_NUMBER: _ClassVar[int]
-    notifications: _containers.RepeatedCompositeFieldContainer[_common_pb2.Notification]
-    def __init__(self, notifications: _Optional[_Iterable[_Union[_common_pb2.Notification, _Mapping]]] = ...) -> None: ...
-
-class SystemMetadata(_message.Message):
-    __slots__ = ["execution_cluster"]
-    EXECUTION_CLUSTER_FIELD_NUMBER: _ClassVar[int]
-    execution_cluster: str
-    def __init__(self, execution_cluster: _Optional[str] = ...) -> None: ...
-
 class WorkflowExecutionGetDataRequest(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.WorkflowExecutionIdentifier
     def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
 class WorkflowExecutionGetDataResponse(_message.Message):
-    __slots__ = ["full_inputs", "full_outputs", "inputs", "outputs"]
+    __slots__ = ["outputs", "inputs", "full_inputs", "full_outputs"]
+    OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
     FULL_INPUTS_FIELD_NUMBER: _ClassVar[int]
     FULL_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
-    INPUTS_FIELD_NUMBER: _ClassVar[int]
-    OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    outputs: _common_pb2.UrlBlob
+    inputs: _common_pb2.UrlBlob
     full_inputs: _literals_pb2.LiteralMap
     full_outputs: _literals_pb2.LiteralMap
-    inputs: _common_pb2.UrlBlob
-    outputs: _common_pb2.UrlBlob
     def __init__(self, outputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., inputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., full_inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., full_outputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ...) -> None: ...
 
-class WorkflowExecutionGetRequest(_message.Message):
-    __slots__ = ["id"]
+class ExecutionUpdateRequest(_message.Message):
+    __slots__ = ["id", "state"]
     ID_FIELD_NUMBER: _ClassVar[int]
+    STATE_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.WorkflowExecutionIdentifier
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
+    state: ExecutionState
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., state: _Optional[_Union[ExecutionState, str]] = ...) -> None: ...
 
-class ExecutionState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+class ExecutionStateChangeDetails(_message.Message):
+    __slots__ = ["state", "occurred_at", "principal"]
+    STATE_FIELD_NUMBER: _ClassVar[int]
+    OCCURRED_AT_FIELD_NUMBER: _ClassVar[int]
+    PRINCIPAL_FIELD_NUMBER: _ClassVar[int]
+    state: ExecutionState
+    occurred_at: _timestamp_pb2.Timestamp
+    principal: str
+    def __init__(self, state: _Optional[_Union[ExecutionState, str]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., principal: _Optional[str] = ...) -> None: ...
+
+class ExecutionUpdateResponse(_message.Message):
     __slots__ = []
+    def __init__(self) -> None: ...
+
+class WorkflowExecutionGetMetricsRequest(_message.Message):
+    __slots__ = ["id", "depth"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    DEPTH_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.WorkflowExecutionIdentifier
+    depth: int
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., depth: _Optional[int] = ...) -> None: ...
+
+class WorkflowExecutionGetMetricsResponse(_message.Message):
+    __slots__ = ["span"]
+    SPAN_FIELD_NUMBER: _ClassVar[int]
+    span: _metrics_pb2.Span
+    def __init__(self, span: _Optional[_Union[_metrics_pb2.Span, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/launch_plan_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/launch_plan_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,48 +20,49 @@
 from flyteidl.admin import common_pb2 as flyteidl_dot_admin_dot_common__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n flyteidl/admin/launch_plan.proto\x12\x0e\x66lyteidl.admin\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1d\x66lyteidl/core/interface.proto\x1a\x1c\x66lyteidl/core/security.proto\x1a\x1d\x66lyteidl/admin/schedule.proto\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"x\n\x17LaunchPlanCreateRequest\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12\x32\n\x04spec\x18\x02 \x01(\x0b\x32\x1e.flyteidl.admin.LaunchPlanSpecR\x04spec\"\x1a\n\x18LaunchPlanCreateResponse\"\xa8\x01\n\nLaunchPlan\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12\x32\n\x04spec\x18\x02 \x01(\x0b\x32\x1e.flyteidl.admin.LaunchPlanSpecR\x04spec\x12;\n\x07\x63losure\x18\x03 \x01(\x0b\x32!.flyteidl.admin.LaunchPlanClosureR\x07\x63losure\"e\n\x0eLaunchPlanList\x12=\n\x0claunch_plans\x18\x01 \x03(\x0b\x32\x1a.flyteidl.admin.LaunchPlanR\x0blaunchPlans\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"v\n\x04\x41uth\x12,\n\x12\x61ssumable_iam_role\x18\x01 \x01(\tR\x10\x61ssumableIamRole\x12<\n\x1akubernetes_service_account\x18\x02 \x01(\tR\x18kubernetesServiceAccount:\x02\x18\x01\"\x93\x07\n\x0eLaunchPlanSpec\x12:\n\x0bworkflow_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\nworkflowId\x12K\n\x0f\x65ntity_metadata\x18\x02 \x01(\x0b\x32\".flyteidl.admin.LaunchPlanMetadataR\x0e\x65ntityMetadata\x12\x42\n\x0e\x64\x65\x66\x61ult_inputs\x18\x03 \x01(\x0b\x32\x1b.flyteidl.core.ParameterMapR\rdefaultInputs\x12<\n\x0c\x66ixed_inputs\x18\x04 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x0b\x66ixedInputs\x12\x16\n\x04role\x18\x05 \x01(\tB\x02\x18\x01R\x04role\x12.\n\x06labels\x18\x06 \x01(\x0b\x32\x16.flyteidl.admin.LabelsR\x06labels\x12=\n\x0b\x61nnotations\x18\x07 \x01(\x0b\x32\x1b.flyteidl.admin.AnnotationsR\x0b\x61nnotations\x12,\n\x04\x61uth\x18\x08 \x01(\x0b\x32\x14.flyteidl.admin.AuthB\x02\x18\x01R\x04\x61uth\x12\x39\n\tauth_role\x18\t \x01(\x0b\x32\x18.flyteidl.admin.AuthRoleB\x02\x18\x01R\x08\x61uthRole\x12I\n\x10security_context\x18\n \x01(\x0b\x32\x1e.flyteidl.core.SecurityContextR\x0fsecurityContext\x12M\n\x12quality_of_service\x18\x10 \x01(\x0b\x32\x1f.flyteidl.core.QualityOfServiceR\x10qualityOfService\x12X\n\x16raw_output_data_config\x18\x11 \x01(\x0b\x32#.flyteidl.admin.RawOutputDataConfigR\x13rawOutputDataConfig\x12\'\n\x0fmax_parallelism\x18\x12 \x01(\x05R\x0emaxParallelism\x12@\n\rinterruptible\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\rinterruptible\x12\'\n\x0foverwrite_cache\x18\x14 \x01(\x08R\x0eoverwriteCache\"\xcd\x02\n\x11LaunchPlanClosure\x12\x35\n\x05state\x18\x01 \x01(\x0e\x32\x1f.flyteidl.admin.LaunchPlanStateR\x05state\x12\x44\n\x0f\x65xpected_inputs\x18\x02 \x01(\x0b\x32\x1b.flyteidl.core.ParameterMapR\x0e\x65xpectedInputs\x12\x45\n\x10\x65xpected_outputs\x18\x03 \x01(\x0b\x32\x1a.flyteidl.core.VariableMapR\x0f\x65xpectedOutputs\x12\x39\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\"\x8e\x01\n\x12LaunchPlanMetadata\x12\x34\n\x08schedule\x18\x01 \x01(\x0b\x32\x18.flyteidl.admin.ScheduleR\x08schedule\x12\x42\n\rnotifications\x18\x02 \x03(\x0b\x32\x1c.flyteidl.admin.NotificationR\rnotifications\"{\n\x17LaunchPlanUpdateRequest\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12\x35\n\x05state\x18\x02 \x01(\x0e\x32\x1f.flyteidl.admin.LaunchPlanStateR\x05state\"\x1a\n\x18LaunchPlanUpdateResponse\"P\n\x17\x41\x63tiveLaunchPlanRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32%.flyteidl.admin.NamedEntityIdentifierR\x02id\"\xaa\x01\n\x1b\x41\x63tiveLaunchPlanListRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x14\n\x05limit\x18\x03 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x04 \x01(\tR\x05token\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy*+\n\x0fLaunchPlanState\x12\x0c\n\x08INACTIVE\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x42\xb5\x01\n\x12\x63om.flyteidl.adminB\x0fLaunchPlanProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.launch_plan_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.launch_plan_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\017LaunchPlanProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
   _AUTH._options = None
   _AUTH._serialized_options = b'\030\001'
   _LAUNCHPLANSPEC.fields_by_name['role']._options = None
   _LAUNCHPLANSPEC.fields_by_name['role']._serialized_options = b'\030\001'
   _LAUNCHPLANSPEC.fields_by_name['auth']._options = None
   _LAUNCHPLANSPEC.fields_by_name['auth']._serialized_options = b'\030\001'
   _LAUNCHPLANSPEC.fields_by_name['auth_role']._options = None
   _LAUNCHPLANSPEC.fields_by_name['auth_role']._serialized_options = b'\030\001'
-  _LAUNCHPLANSTATE._serialized_start=2682
-  _LAUNCHPLANSTATE._serialized_end=2725
-  _LAUNCHPLANCREATEREQUEST._serialized_start=331
-  _LAUNCHPLANCREATEREQUEST._serialized_end=451
-  _LAUNCHPLANCREATERESPONSE._serialized_start=453
-  _LAUNCHPLANCREATERESPONSE._serialized_end=479
-  _LAUNCHPLAN._serialized_start=482
-  _LAUNCHPLAN._serialized_end=650
-  _LAUNCHPLANLIST._serialized_start=652
-  _LAUNCHPLANLIST._serialized_end=753
-  _AUTH._serialized_start=755
-  _AUTH._serialized_end=873
-  _LAUNCHPLANSPEC._serialized_start=876
-  _LAUNCHPLANSPEC._serialized_end=1791
-  _LAUNCHPLANCLOSURE._serialized_start=1794
-  _LAUNCHPLANCLOSURE._serialized_end=2127
-  _LAUNCHPLANMETADATA._serialized_start=2130
-  _LAUNCHPLANMETADATA._serialized_end=2272
-  _LAUNCHPLANUPDATEREQUEST._serialized_start=2274
-  _LAUNCHPLANUPDATEREQUEST._serialized_end=2397
-  _LAUNCHPLANUPDATERESPONSE._serialized_start=2399
-  _LAUNCHPLANUPDATERESPONSE._serialized_end=2425
-  _ACTIVELAUNCHPLANREQUEST._serialized_start=2427
-  _ACTIVELAUNCHPLANREQUEST._serialized_end=2507
-  _ACTIVELAUNCHPLANLISTREQUEST._serialized_start=2510
-  _ACTIVELAUNCHPLANLISTREQUEST._serialized_end=2680
+  _globals['_LAUNCHPLANSTATE']._serialized_start=2682
+  _globals['_LAUNCHPLANSTATE']._serialized_end=2725
+  _globals['_LAUNCHPLANCREATEREQUEST']._serialized_start=331
+  _globals['_LAUNCHPLANCREATEREQUEST']._serialized_end=451
+  _globals['_LAUNCHPLANCREATERESPONSE']._serialized_start=453
+  _globals['_LAUNCHPLANCREATERESPONSE']._serialized_end=479
+  _globals['_LAUNCHPLAN']._serialized_start=482
+  _globals['_LAUNCHPLAN']._serialized_end=650
+  _globals['_LAUNCHPLANLIST']._serialized_start=652
+  _globals['_LAUNCHPLANLIST']._serialized_end=753
+  _globals['_AUTH']._serialized_start=755
+  _globals['_AUTH']._serialized_end=873
+  _globals['_LAUNCHPLANSPEC']._serialized_start=876
+  _globals['_LAUNCHPLANSPEC']._serialized_end=1791
+  _globals['_LAUNCHPLANCLOSURE']._serialized_start=1794
+  _globals['_LAUNCHPLANCLOSURE']._serialized_end=2127
+  _globals['_LAUNCHPLANMETADATA']._serialized_start=2130
+  _globals['_LAUNCHPLANMETADATA']._serialized_end=2272
+  _globals['_LAUNCHPLANUPDATEREQUEST']._serialized_start=2274
+  _globals['_LAUNCHPLANUPDATEREQUEST']._serialized_end=2397
+  _globals['_LAUNCHPLANUPDATERESPONSE']._serialized_start=2399
+  _globals['_LAUNCHPLANUPDATERESPONSE']._serialized_end=2425
+  _globals['_ACTIVELAUNCHPLANREQUEST']._serialized_start=2427
+  _globals['_ACTIVELAUNCHPLANREQUEST']._serialized_end=2507
+  _globals['_ACTIVELAUNCHPLANLISTREQUEST']._serialized_start=2510
+  _globals['_ACTIVELAUNCHPLANLISTREQUEST']._serialized_end=2680
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/launch_plan_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/launch_plan_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,139 +9,141 @@
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-ACTIVE: LaunchPlanState
 DESCRIPTOR: _descriptor.FileDescriptor
-INACTIVE: LaunchPlanState
-
-class ActiveLaunchPlanListRequest(_message.Message):
-    __slots__ = ["domain", "limit", "project", "sort_by", "token"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    limit: int
-    project: str
-    sort_by: _common_pb2.Sort
-    token: str
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
 
-class ActiveLaunchPlanRequest(_message.Message):
-    __slots__ = ["id"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    id: _common_pb2.NamedEntityIdentifier
-    def __init__(self, id: _Optional[_Union[_common_pb2.NamedEntityIdentifier, _Mapping]] = ...) -> None: ...
-
-class Auth(_message.Message):
-    __slots__ = ["assumable_iam_role", "kubernetes_service_account"]
-    ASSUMABLE_IAM_ROLE_FIELD_NUMBER: _ClassVar[int]
-    KUBERNETES_SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    assumable_iam_role: str
-    kubernetes_service_account: str
-    def __init__(self, assumable_iam_role: _Optional[str] = ..., kubernetes_service_account: _Optional[str] = ...) -> None: ...
-
-class LaunchPlan(_message.Message):
-    __slots__ = ["closure", "id", "spec"]
-    CLOSURE_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    SPEC_FIELD_NUMBER: _ClassVar[int]
-    closure: LaunchPlanClosure
-    id: _identifier_pb2.Identifier
-    spec: LaunchPlanSpec
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., spec: _Optional[_Union[LaunchPlanSpec, _Mapping]] = ..., closure: _Optional[_Union[LaunchPlanClosure, _Mapping]] = ...) -> None: ...
-
-class LaunchPlanClosure(_message.Message):
-    __slots__ = ["created_at", "expected_inputs", "expected_outputs", "state", "updated_at"]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    EXPECTED_INPUTS_FIELD_NUMBER: _ClassVar[int]
-    EXPECTED_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
-    STATE_FIELD_NUMBER: _ClassVar[int]
-    UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
-    created_at: _timestamp_pb2.Timestamp
-    expected_inputs: _interface_pb2.ParameterMap
-    expected_outputs: _interface_pb2.VariableMap
-    state: LaunchPlanState
-    updated_at: _timestamp_pb2.Timestamp
-    def __init__(self, state: _Optional[_Union[LaunchPlanState, str]] = ..., expected_inputs: _Optional[_Union[_interface_pb2.ParameterMap, _Mapping]] = ..., expected_outputs: _Optional[_Union[_interface_pb2.VariableMap, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+class LaunchPlanState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    INACTIVE: _ClassVar[LaunchPlanState]
+    ACTIVE: _ClassVar[LaunchPlanState]
+INACTIVE: LaunchPlanState
+ACTIVE: LaunchPlanState
 
 class LaunchPlanCreateRequest(_message.Message):
     __slots__ = ["id", "spec"]
     ID_FIELD_NUMBER: _ClassVar[int]
     SPEC_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
     spec: LaunchPlanSpec
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., spec: _Optional[_Union[LaunchPlanSpec, _Mapping]] = ...) -> None: ...
 
 class LaunchPlanCreateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
+class LaunchPlan(_message.Message):
+    __slots__ = ["id", "spec", "closure"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    SPEC_FIELD_NUMBER: _ClassVar[int]
+    CLOSURE_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.Identifier
+    spec: LaunchPlanSpec
+    closure: LaunchPlanClosure
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., spec: _Optional[_Union[LaunchPlanSpec, _Mapping]] = ..., closure: _Optional[_Union[LaunchPlanClosure, _Mapping]] = ...) -> None: ...
+
 class LaunchPlanList(_message.Message):
     __slots__ = ["launch_plans", "token"]
     LAUNCH_PLANS_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     launch_plans: _containers.RepeatedCompositeFieldContainer[LaunchPlan]
     token: str
     def __init__(self, launch_plans: _Optional[_Iterable[_Union[LaunchPlan, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
 
-class LaunchPlanMetadata(_message.Message):
-    __slots__ = ["notifications", "schedule"]
-    NOTIFICATIONS_FIELD_NUMBER: _ClassVar[int]
-    SCHEDULE_FIELD_NUMBER: _ClassVar[int]
-    notifications: _containers.RepeatedCompositeFieldContainer[_common_pb2.Notification]
-    schedule: _schedule_pb2.Schedule
-    def __init__(self, schedule: _Optional[_Union[_schedule_pb2.Schedule, _Mapping]] = ..., notifications: _Optional[_Iterable[_Union[_common_pb2.Notification, _Mapping]]] = ...) -> None: ...
+class Auth(_message.Message):
+    __slots__ = ["assumable_iam_role", "kubernetes_service_account"]
+    ASSUMABLE_IAM_ROLE_FIELD_NUMBER: _ClassVar[int]
+    KUBERNETES_SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
+    assumable_iam_role: str
+    kubernetes_service_account: str
+    def __init__(self, assumable_iam_role: _Optional[str] = ..., kubernetes_service_account: _Optional[str] = ...) -> None: ...
 
 class LaunchPlanSpec(_message.Message):
-    __slots__ = ["annotations", "auth", "auth_role", "default_inputs", "entity_metadata", "fixed_inputs", "interruptible", "labels", "max_parallelism", "overwrite_cache", "quality_of_service", "raw_output_data_config", "role", "security_context", "workflow_id"]
-    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
-    AUTH_FIELD_NUMBER: _ClassVar[int]
-    AUTH_ROLE_FIELD_NUMBER: _ClassVar[int]
-    DEFAULT_INPUTS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["workflow_id", "entity_metadata", "default_inputs", "fixed_inputs", "role", "labels", "annotations", "auth", "auth_role", "security_context", "quality_of_service", "raw_output_data_config", "max_parallelism", "interruptible", "overwrite_cache"]
+    WORKFLOW_ID_FIELD_NUMBER: _ClassVar[int]
     ENTITY_METADATA_FIELD_NUMBER: _ClassVar[int]
+    DEFAULT_INPUTS_FIELD_NUMBER: _ClassVar[int]
     FIXED_INPUTS_FIELD_NUMBER: _ClassVar[int]
-    INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
+    ROLE_FIELD_NUMBER: _ClassVar[int]
     LABELS_FIELD_NUMBER: _ClassVar[int]
-    MAX_PARALLELISM_FIELD_NUMBER: _ClassVar[int]
-    OVERWRITE_CACHE_FIELD_NUMBER: _ClassVar[int]
+    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
+    AUTH_FIELD_NUMBER: _ClassVar[int]
+    AUTH_ROLE_FIELD_NUMBER: _ClassVar[int]
+    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
     QUALITY_OF_SERVICE_FIELD_NUMBER: _ClassVar[int]
     RAW_OUTPUT_DATA_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    ROLE_FIELD_NUMBER: _ClassVar[int]
-    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_ID_FIELD_NUMBER: _ClassVar[int]
-    annotations: _common_pb2.Annotations
-    auth: Auth
-    auth_role: _common_pb2.AuthRole
-    default_inputs: _interface_pb2.ParameterMap
+    MAX_PARALLELISM_FIELD_NUMBER: _ClassVar[int]
+    INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
+    OVERWRITE_CACHE_FIELD_NUMBER: _ClassVar[int]
+    workflow_id: _identifier_pb2.Identifier
     entity_metadata: LaunchPlanMetadata
+    default_inputs: _interface_pb2.ParameterMap
     fixed_inputs: _literals_pb2.LiteralMap
-    interruptible: _wrappers_pb2.BoolValue
+    role: str
     labels: _common_pb2.Labels
-    max_parallelism: int
-    overwrite_cache: bool
+    annotations: _common_pb2.Annotations
+    auth: Auth
+    auth_role: _common_pb2.AuthRole
+    security_context: _security_pb2.SecurityContext
     quality_of_service: _execution_pb2.QualityOfService
     raw_output_data_config: _common_pb2.RawOutputDataConfig
-    role: str
-    security_context: _security_pb2.SecurityContext
-    workflow_id: _identifier_pb2.Identifier
+    max_parallelism: int
+    interruptible: _wrappers_pb2.BoolValue
+    overwrite_cache: bool
     def __init__(self, workflow_id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., entity_metadata: _Optional[_Union[LaunchPlanMetadata, _Mapping]] = ..., default_inputs: _Optional[_Union[_interface_pb2.ParameterMap, _Mapping]] = ..., fixed_inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., role: _Optional[str] = ..., labels: _Optional[_Union[_common_pb2.Labels, _Mapping]] = ..., annotations: _Optional[_Union[_common_pb2.Annotations, _Mapping]] = ..., auth: _Optional[_Union[Auth, _Mapping]] = ..., auth_role: _Optional[_Union[_common_pb2.AuthRole, _Mapping]] = ..., security_context: _Optional[_Union[_security_pb2.SecurityContext, _Mapping]] = ..., quality_of_service: _Optional[_Union[_execution_pb2.QualityOfService, _Mapping]] = ..., raw_output_data_config: _Optional[_Union[_common_pb2.RawOutputDataConfig, _Mapping]] = ..., max_parallelism: _Optional[int] = ..., interruptible: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., overwrite_cache: bool = ...) -> None: ...
 
+class LaunchPlanClosure(_message.Message):
+    __slots__ = ["state", "expected_inputs", "expected_outputs", "created_at", "updated_at"]
+    STATE_FIELD_NUMBER: _ClassVar[int]
+    EXPECTED_INPUTS_FIELD_NUMBER: _ClassVar[int]
+    EXPECTED_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
+    state: LaunchPlanState
+    expected_inputs: _interface_pb2.ParameterMap
+    expected_outputs: _interface_pb2.VariableMap
+    created_at: _timestamp_pb2.Timestamp
+    updated_at: _timestamp_pb2.Timestamp
+    def __init__(self, state: _Optional[_Union[LaunchPlanState, str]] = ..., expected_inputs: _Optional[_Union[_interface_pb2.ParameterMap, _Mapping]] = ..., expected_outputs: _Optional[_Union[_interface_pb2.VariableMap, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+
+class LaunchPlanMetadata(_message.Message):
+    __slots__ = ["schedule", "notifications"]
+    SCHEDULE_FIELD_NUMBER: _ClassVar[int]
+    NOTIFICATIONS_FIELD_NUMBER: _ClassVar[int]
+    schedule: _schedule_pb2.Schedule
+    notifications: _containers.RepeatedCompositeFieldContainer[_common_pb2.Notification]
+    def __init__(self, schedule: _Optional[_Union[_schedule_pb2.Schedule, _Mapping]] = ..., notifications: _Optional[_Iterable[_Union[_common_pb2.Notification, _Mapping]]] = ...) -> None: ...
+
 class LaunchPlanUpdateRequest(_message.Message):
     __slots__ = ["id", "state"]
     ID_FIELD_NUMBER: _ClassVar[int]
     STATE_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
     state: LaunchPlanState
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., state: _Optional[_Union[LaunchPlanState, str]] = ...) -> None: ...
 
 class LaunchPlanUpdateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class LaunchPlanState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class ActiveLaunchPlanRequest(_message.Message):
+    __slots__ = ["id"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: _common_pb2.NamedEntityIdentifier
+    def __init__(self, id: _Optional[_Union[_common_pb2.NamedEntityIdentifier, _Mapping]] = ...) -> None: ...
+
+class ActiveLaunchPlanListRequest(_message.Message):
+    __slots__ = ["project", "domain", "limit", "token", "sort_by"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    limit: int
+    token: str
+    sort_by: _common_pb2.Sort
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,46 +16,47 @@
 from flyteidl.core import execution_pb2 as flyteidl_dot_core_dot_execution__pb2
 from flyteidl.core import security_pb2 as flyteidl_dot_core_dot_security__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'flyteidl/admin/matchable_resource.proto\x12\x0e\x66lyteidl.admin\x1a\x1b\x66lyteidl/admin/common.proto\x1a\'flyteidl/admin/cluster_assignment.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1c\x66lyteidl/core/security.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x95\x01\n\x10TaskResourceSpec\x12\x10\n\x03\x63pu\x18\x01 \x01(\tR\x03\x63pu\x12\x10\n\x03gpu\x18\x02 \x01(\tR\x03gpu\x12\x16\n\x06memory\x18\x03 \x01(\tR\x06memory\x12\x18\n\x07storage\x18\x04 \x01(\tR\x07storage\x12+\n\x11\x65phemeral_storage\x18\x05 \x01(\tR\x10\x65phemeralStorage\"\x90\x01\n\x16TaskResourceAttributes\x12<\n\x08\x64\x65\x66\x61ults\x18\x01 \x01(\x0b\x32 .flyteidl.admin.TaskResourceSpecR\x08\x64\x65\x66\x61ults\x12\x38\n\x06limits\x18\x02 \x01(\x0b\x32 .flyteidl.admin.TaskResourceSpecR\x06limits\"\xb5\x01\n\x19\x43lusterResourceAttributes\x12Y\n\nattributes\x18\x01 \x03(\x0b\x32\x39.flyteidl.admin.ClusterResourceAttributes.AttributesEntryR\nattributes\x1a=\n\x0f\x41ttributesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\".\n\x18\x45xecutionQueueAttributes\x12\x12\n\x04tags\x18\x01 \x03(\tR\x04tags\"-\n\x15\x45xecutionClusterLabel\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\"\xec\x01\n\x0ePluginOverride\x12\x1b\n\ttask_type\x18\x01 \x01(\tR\x08taskType\x12\x1b\n\tplugin_id\x18\x02 \x03(\tR\x08pluginId\x12l\n\x17missing_plugin_behavior\x18\x04 \x01(\x0e\x32\x34.flyteidl.admin.PluginOverride.MissingPluginBehaviorR\x15missingPluginBehavior\"2\n\x15MissingPluginBehavior\x12\x08\n\x04\x46\x41IL\x10\x00\x12\x0f\n\x0bUSE_DEFAULT\x10\x01\"O\n\x0fPluginOverrides\x12<\n\toverrides\x18\x01 \x03(\x0b\x32\x1e.flyteidl.admin.PluginOverrideR\toverrides\"\xc1\x03\n\x17WorkflowExecutionConfig\x12\'\n\x0fmax_parallelism\x18\x01 \x01(\x05R\x0emaxParallelism\x12I\n\x10security_context\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.SecurityContextR\x0fsecurityContext\x12X\n\x16raw_output_data_config\x18\x03 \x01(\x0b\x32#.flyteidl.admin.RawOutputDataConfigR\x13rawOutputDataConfig\x12.\n\x06labels\x18\x04 \x01(\x0b\x32\x16.flyteidl.admin.LabelsR\x06labels\x12=\n\x0b\x61nnotations\x18\x05 \x01(\x0b\x32\x1b.flyteidl.admin.AnnotationsR\x0b\x61nnotations\x12@\n\rinterruptible\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\rinterruptible\x12\'\n\x0foverwrite_cache\x18\x07 \x01(\x08R\x0eoverwriteCache\"\x94\x06\n\x12MatchingAttributes\x12\x62\n\x18task_resource_attributes\x18\x01 \x01(\x0b\x32&.flyteidl.admin.TaskResourceAttributesH\x00R\x16taskResourceAttributes\x12k\n\x1b\x63luster_resource_attributes\x18\x02 \x01(\x0b\x32).flyteidl.admin.ClusterResourceAttributesH\x00R\x19\x63lusterResourceAttributes\x12h\n\x1a\x65xecution_queue_attributes\x18\x03 \x01(\x0b\x32(.flyteidl.admin.ExecutionQueueAttributesH\x00R\x18\x65xecutionQueueAttributes\x12_\n\x17\x65xecution_cluster_label\x18\x04 \x01(\x0b\x32%.flyteidl.admin.ExecutionClusterLabelH\x00R\x15\x65xecutionClusterLabel\x12O\n\x12quality_of_service\x18\x05 \x01(\x0b\x32\x1f.flyteidl.core.QualityOfServiceH\x00R\x10qualityOfService\x12L\n\x10plugin_overrides\x18\x06 \x01(\x0b\x32\x1f.flyteidl.admin.PluginOverridesH\x00R\x0fpluginOverrides\x12\x65\n\x19workflow_execution_config\x18\x07 \x01(\x0b\x32\'.flyteidl.admin.WorkflowExecutionConfigH\x00R\x17workflowExecutionConfig\x12R\n\x12\x63luster_assignment\x18\x08 \x01(\x0b\x32!.flyteidl.admin.ClusterAssignmentH\x00R\x11\x63lusterAssignmentB\x08\n\x06target\"\xd5\x01\n MatchableAttributesConfiguration\x12\x42\n\nattributes\x18\x01 \x01(\x0b\x32\".flyteidl.admin.MatchingAttributesR\nattributes\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12\x1a\n\x08workflow\x18\x04 \x01(\tR\x08workflow\x12\x1f\n\x0blaunch_plan\x18\x05 \x01(\tR\nlaunchPlan\"h\n\x1eListMatchableAttributesRequest\x12\x46\n\rresource_type\x18\x01 \x01(\x0e\x32!.flyteidl.admin.MatchableResourceR\x0cresourceType\"{\n\x1fListMatchableAttributesResponse\x12X\n\x0e\x63onfigurations\x18\x01 \x03(\x0b\x32\x30.flyteidl.admin.MatchableAttributesConfigurationR\x0e\x63onfigurations*\xe0\x01\n\x11MatchableResource\x12\x11\n\rTASK_RESOURCE\x10\x00\x12\x14\n\x10\x43LUSTER_RESOURCE\x10\x01\x12\x13\n\x0f\x45XECUTION_QUEUE\x10\x02\x12\x1b\n\x17\x45XECUTION_CLUSTER_LABEL\x10\x03\x12$\n QUALITY_OF_SERVICE_SPECIFICATION\x10\x04\x12\x13\n\x0fPLUGIN_OVERRIDE\x10\x05\x12\x1d\n\x19WORKFLOW_EXECUTION_CONFIG\x10\x06\x12\x16\n\x12\x43LUSTER_ASSIGNMENT\x10\x07\x42\xbc\x01\n\x12\x63om.flyteidl.adminB\x16MatchableResourceProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.matchable_resource_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.matchable_resource_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\026MatchableResourceProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
   _CLUSTERRESOURCEATTRIBUTES_ATTRIBUTESENTRY._options = None
   _CLUSTERRESOURCEATTRIBUTES_ATTRIBUTESENTRY._serialized_options = b'8\001'
-  _MATCHABLERESOURCE._serialized_start=2811
-  _MATCHABLERESOURCE._serialized_end=3035
-  _TASKRESOURCESPEC._serialized_start=223
-  _TASKRESOURCESPEC._serialized_end=372
-  _TASKRESOURCEATTRIBUTES._serialized_start=375
-  _TASKRESOURCEATTRIBUTES._serialized_end=519
-  _CLUSTERRESOURCEATTRIBUTES._serialized_start=522
-  _CLUSTERRESOURCEATTRIBUTES._serialized_end=703
-  _CLUSTERRESOURCEATTRIBUTES_ATTRIBUTESENTRY._serialized_start=642
-  _CLUSTERRESOURCEATTRIBUTES_ATTRIBUTESENTRY._serialized_end=703
-  _EXECUTIONQUEUEATTRIBUTES._serialized_start=705
-  _EXECUTIONQUEUEATTRIBUTES._serialized_end=751
-  _EXECUTIONCLUSTERLABEL._serialized_start=753
-  _EXECUTIONCLUSTERLABEL._serialized_end=798
-  _PLUGINOVERRIDE._serialized_start=801
-  _PLUGINOVERRIDE._serialized_end=1037
-  _PLUGINOVERRIDE_MISSINGPLUGINBEHAVIOR._serialized_start=987
-  _PLUGINOVERRIDE_MISSINGPLUGINBEHAVIOR._serialized_end=1037
-  _PLUGINOVERRIDES._serialized_start=1039
-  _PLUGINOVERRIDES._serialized_end=1118
-  _WORKFLOWEXECUTIONCONFIG._serialized_start=1121
-  _WORKFLOWEXECUTIONCONFIG._serialized_end=1570
-  _MATCHINGATTRIBUTES._serialized_start=1573
-  _MATCHINGATTRIBUTES._serialized_end=2361
-  _MATCHABLEATTRIBUTESCONFIGURATION._serialized_start=2364
-  _MATCHABLEATTRIBUTESCONFIGURATION._serialized_end=2577
-  _LISTMATCHABLEATTRIBUTESREQUEST._serialized_start=2579
-  _LISTMATCHABLEATTRIBUTESREQUEST._serialized_end=2683
-  _LISTMATCHABLEATTRIBUTESRESPONSE._serialized_start=2685
-  _LISTMATCHABLEATTRIBUTESRESPONSE._serialized_end=2808
+  _globals['_MATCHABLERESOURCE']._serialized_start=2811
+  _globals['_MATCHABLERESOURCE']._serialized_end=3035
+  _globals['_TASKRESOURCESPEC']._serialized_start=223
+  _globals['_TASKRESOURCESPEC']._serialized_end=372
+  _globals['_TASKRESOURCEATTRIBUTES']._serialized_start=375
+  _globals['_TASKRESOURCEATTRIBUTES']._serialized_end=519
+  _globals['_CLUSTERRESOURCEATTRIBUTES']._serialized_start=522
+  _globals['_CLUSTERRESOURCEATTRIBUTES']._serialized_end=703
+  _globals['_CLUSTERRESOURCEATTRIBUTES_ATTRIBUTESENTRY']._serialized_start=642
+  _globals['_CLUSTERRESOURCEATTRIBUTES_ATTRIBUTESENTRY']._serialized_end=703
+  _globals['_EXECUTIONQUEUEATTRIBUTES']._serialized_start=705
+  _globals['_EXECUTIONQUEUEATTRIBUTES']._serialized_end=751
+  _globals['_EXECUTIONCLUSTERLABEL']._serialized_start=753
+  _globals['_EXECUTIONCLUSTERLABEL']._serialized_end=798
+  _globals['_PLUGINOVERRIDE']._serialized_start=801
+  _globals['_PLUGINOVERRIDE']._serialized_end=1037
+  _globals['_PLUGINOVERRIDE_MISSINGPLUGINBEHAVIOR']._serialized_start=987
+  _globals['_PLUGINOVERRIDE_MISSINGPLUGINBEHAVIOR']._serialized_end=1037
+  _globals['_PLUGINOVERRIDES']._serialized_start=1039
+  _globals['_PLUGINOVERRIDES']._serialized_end=1118
+  _globals['_WORKFLOWEXECUTIONCONFIG']._serialized_start=1121
+  _globals['_WORKFLOWEXECUTIONCONFIG']._serialized_end=1570
+  _globals['_MATCHINGATTRIBUTES']._serialized_start=1573
+  _globals['_MATCHINGATTRIBUTES']._serialized_end=2361
+  _globals['_MATCHABLEATTRIBUTESCONFIGURATION']._serialized_start=2364
+  _globals['_MATCHABLEATTRIBUTESCONFIGURATION']._serialized_end=2577
+  _globals['_LISTMATCHABLEATTRIBUTESREQUEST']._serialized_start=2579
+  _globals['_LISTMATCHABLEATTRIBUTESREQUEST']._serialized_end=2683
+  _globals['_LISTMATCHABLEATTRIBUTESRESPONSE']._serialized_start=2685
+  _globals['_LISTMATCHABLEATTRIBUTESRESPONSE']._serialized_end=2808
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/matchable_resource_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/matchable_resource_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -5,150 +5,160 @@
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-CLUSTER_ASSIGNMENT: MatchableResource
-CLUSTER_RESOURCE: MatchableResource
 DESCRIPTOR: _descriptor.FileDescriptor
-EXECUTION_CLUSTER_LABEL: MatchableResource
+
+class MatchableResource(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    TASK_RESOURCE: _ClassVar[MatchableResource]
+    CLUSTER_RESOURCE: _ClassVar[MatchableResource]
+    EXECUTION_QUEUE: _ClassVar[MatchableResource]
+    EXECUTION_CLUSTER_LABEL: _ClassVar[MatchableResource]
+    QUALITY_OF_SERVICE_SPECIFICATION: _ClassVar[MatchableResource]
+    PLUGIN_OVERRIDE: _ClassVar[MatchableResource]
+    WORKFLOW_EXECUTION_CONFIG: _ClassVar[MatchableResource]
+    CLUSTER_ASSIGNMENT: _ClassVar[MatchableResource]
+TASK_RESOURCE: MatchableResource
+CLUSTER_RESOURCE: MatchableResource
 EXECUTION_QUEUE: MatchableResource
-PLUGIN_OVERRIDE: MatchableResource
+EXECUTION_CLUSTER_LABEL: MatchableResource
 QUALITY_OF_SERVICE_SPECIFICATION: MatchableResource
-TASK_RESOURCE: MatchableResource
+PLUGIN_OVERRIDE: MatchableResource
 WORKFLOW_EXECUTION_CONFIG: MatchableResource
+CLUSTER_ASSIGNMENT: MatchableResource
+
+class TaskResourceSpec(_message.Message):
+    __slots__ = ["cpu", "gpu", "memory", "storage", "ephemeral_storage"]
+    CPU_FIELD_NUMBER: _ClassVar[int]
+    GPU_FIELD_NUMBER: _ClassVar[int]
+    MEMORY_FIELD_NUMBER: _ClassVar[int]
+    STORAGE_FIELD_NUMBER: _ClassVar[int]
+    EPHEMERAL_STORAGE_FIELD_NUMBER: _ClassVar[int]
+    cpu: str
+    gpu: str
+    memory: str
+    storage: str
+    ephemeral_storage: str
+    def __init__(self, cpu: _Optional[str] = ..., gpu: _Optional[str] = ..., memory: _Optional[str] = ..., storage: _Optional[str] = ..., ephemeral_storage: _Optional[str] = ...) -> None: ...
+
+class TaskResourceAttributes(_message.Message):
+    __slots__ = ["defaults", "limits"]
+    DEFAULTS_FIELD_NUMBER: _ClassVar[int]
+    LIMITS_FIELD_NUMBER: _ClassVar[int]
+    defaults: TaskResourceSpec
+    limits: TaskResourceSpec
+    def __init__(self, defaults: _Optional[_Union[TaskResourceSpec, _Mapping]] = ..., limits: _Optional[_Union[TaskResourceSpec, _Mapping]] = ...) -> None: ...
 
 class ClusterResourceAttributes(_message.Message):
     __slots__ = ["attributes"]
     class AttributesEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     attributes: _containers.ScalarMap[str, str]
     def __init__(self, attributes: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
-class ExecutionClusterLabel(_message.Message):
-    __slots__ = ["value"]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    value: str
-    def __init__(self, value: _Optional[str] = ...) -> None: ...
-
 class ExecutionQueueAttributes(_message.Message):
     __slots__ = ["tags"]
     TAGS_FIELD_NUMBER: _ClassVar[int]
     tags: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, tags: _Optional[_Iterable[str]] = ...) -> None: ...
 
-class ListMatchableAttributesRequest(_message.Message):
-    __slots__ = ["resource_type"]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    resource_type: MatchableResource
-    def __init__(self, resource_type: _Optional[_Union[MatchableResource, str]] = ...) -> None: ...
-
-class ListMatchableAttributesResponse(_message.Message):
-    __slots__ = ["configurations"]
-    CONFIGURATIONS_FIELD_NUMBER: _ClassVar[int]
-    configurations: _containers.RepeatedCompositeFieldContainer[MatchableAttributesConfiguration]
-    def __init__(self, configurations: _Optional[_Iterable[_Union[MatchableAttributesConfiguration, _Mapping]]] = ...) -> None: ...
-
-class MatchableAttributesConfiguration(_message.Message):
-    __slots__ = ["attributes", "domain", "launch_plan", "project", "workflow"]
-    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    LAUNCH_PLAN_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    attributes: MatchingAttributes
-    domain: str
-    launch_plan: str
-    project: str
-    workflow: str
-    def __init__(self, attributes: _Optional[_Union[MatchingAttributes, _Mapping]] = ..., domain: _Optional[str] = ..., project: _Optional[str] = ..., workflow: _Optional[str] = ..., launch_plan: _Optional[str] = ...) -> None: ...
-
-class MatchingAttributes(_message.Message):
-    __slots__ = ["cluster_assignment", "cluster_resource_attributes", "execution_cluster_label", "execution_queue_attributes", "plugin_overrides", "quality_of_service", "task_resource_attributes", "workflow_execution_config"]
-    CLUSTER_ASSIGNMENT_FIELD_NUMBER: _ClassVar[int]
-    CLUSTER_RESOURCE_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    EXECUTION_CLUSTER_LABEL_FIELD_NUMBER: _ClassVar[int]
-    EXECUTION_QUEUE_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    PLUGIN_OVERRIDES_FIELD_NUMBER: _ClassVar[int]
-    QUALITY_OF_SERVICE_FIELD_NUMBER: _ClassVar[int]
-    TASK_RESOURCE_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_EXECUTION_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    cluster_assignment: _cluster_assignment_pb2.ClusterAssignment
-    cluster_resource_attributes: ClusterResourceAttributes
-    execution_cluster_label: ExecutionClusterLabel
-    execution_queue_attributes: ExecutionQueueAttributes
-    plugin_overrides: PluginOverrides
-    quality_of_service: _execution_pb2.QualityOfService
-    task_resource_attributes: TaskResourceAttributes
-    workflow_execution_config: WorkflowExecutionConfig
-    def __init__(self, task_resource_attributes: _Optional[_Union[TaskResourceAttributes, _Mapping]] = ..., cluster_resource_attributes: _Optional[_Union[ClusterResourceAttributes, _Mapping]] = ..., execution_queue_attributes: _Optional[_Union[ExecutionQueueAttributes, _Mapping]] = ..., execution_cluster_label: _Optional[_Union[ExecutionClusterLabel, _Mapping]] = ..., quality_of_service: _Optional[_Union[_execution_pb2.QualityOfService, _Mapping]] = ..., plugin_overrides: _Optional[_Union[PluginOverrides, _Mapping]] = ..., workflow_execution_config: _Optional[_Union[WorkflowExecutionConfig, _Mapping]] = ..., cluster_assignment: _Optional[_Union[_cluster_assignment_pb2.ClusterAssignment, _Mapping]] = ...) -> None: ...
+class ExecutionClusterLabel(_message.Message):
+    __slots__ = ["value"]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    value: str
+    def __init__(self, value: _Optional[str] = ...) -> None: ...
 
 class PluginOverride(_message.Message):
-    __slots__ = ["missing_plugin_behavior", "plugin_id", "task_type"]
+    __slots__ = ["task_type", "plugin_id", "missing_plugin_behavior"]
     class MissingPluginBehavior(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        FAIL: _ClassVar[PluginOverride.MissingPluginBehavior]
+        USE_DEFAULT: _ClassVar[PluginOverride.MissingPluginBehavior]
     FAIL: PluginOverride.MissingPluginBehavior
-    MISSING_PLUGIN_BEHAVIOR_FIELD_NUMBER: _ClassVar[int]
-    PLUGIN_ID_FIELD_NUMBER: _ClassVar[int]
-    TASK_TYPE_FIELD_NUMBER: _ClassVar[int]
     USE_DEFAULT: PluginOverride.MissingPluginBehavior
-    missing_plugin_behavior: PluginOverride.MissingPluginBehavior
-    plugin_id: _containers.RepeatedScalarFieldContainer[str]
+    TASK_TYPE_FIELD_NUMBER: _ClassVar[int]
+    PLUGIN_ID_FIELD_NUMBER: _ClassVar[int]
+    MISSING_PLUGIN_BEHAVIOR_FIELD_NUMBER: _ClassVar[int]
     task_type: str
+    plugin_id: _containers.RepeatedScalarFieldContainer[str]
+    missing_plugin_behavior: PluginOverride.MissingPluginBehavior
     def __init__(self, task_type: _Optional[str] = ..., plugin_id: _Optional[_Iterable[str]] = ..., missing_plugin_behavior: _Optional[_Union[PluginOverride.MissingPluginBehavior, str]] = ...) -> None: ...
 
 class PluginOverrides(_message.Message):
     __slots__ = ["overrides"]
     OVERRIDES_FIELD_NUMBER: _ClassVar[int]
     overrides: _containers.RepeatedCompositeFieldContainer[PluginOverride]
     def __init__(self, overrides: _Optional[_Iterable[_Union[PluginOverride, _Mapping]]] = ...) -> None: ...
 
-class TaskResourceAttributes(_message.Message):
-    __slots__ = ["defaults", "limits"]
-    DEFAULTS_FIELD_NUMBER: _ClassVar[int]
-    LIMITS_FIELD_NUMBER: _ClassVar[int]
-    defaults: TaskResourceSpec
-    limits: TaskResourceSpec
-    def __init__(self, defaults: _Optional[_Union[TaskResourceSpec, _Mapping]] = ..., limits: _Optional[_Union[TaskResourceSpec, _Mapping]] = ...) -> None: ...
-
-class TaskResourceSpec(_message.Message):
-    __slots__ = ["cpu", "ephemeral_storage", "gpu", "memory", "storage"]
-    CPU_FIELD_NUMBER: _ClassVar[int]
-    EPHEMERAL_STORAGE_FIELD_NUMBER: _ClassVar[int]
-    GPU_FIELD_NUMBER: _ClassVar[int]
-    MEMORY_FIELD_NUMBER: _ClassVar[int]
-    STORAGE_FIELD_NUMBER: _ClassVar[int]
-    cpu: str
-    ephemeral_storage: str
-    gpu: str
-    memory: str
-    storage: str
-    def __init__(self, cpu: _Optional[str] = ..., gpu: _Optional[str] = ..., memory: _Optional[str] = ..., storage: _Optional[str] = ..., ephemeral_storage: _Optional[str] = ...) -> None: ...
-
 class WorkflowExecutionConfig(_message.Message):
-    __slots__ = ["annotations", "interruptible", "labels", "max_parallelism", "overwrite_cache", "raw_output_data_config", "security_context"]
+    __slots__ = ["max_parallelism", "security_context", "raw_output_data_config", "labels", "annotations", "interruptible", "overwrite_cache"]
+    MAX_PARALLELISM_FIELD_NUMBER: _ClassVar[int]
+    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    RAW_OUTPUT_DATA_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    LABELS_FIELD_NUMBER: _ClassVar[int]
     ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
     INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
-    LABELS_FIELD_NUMBER: _ClassVar[int]
-    MAX_PARALLELISM_FIELD_NUMBER: _ClassVar[int]
     OVERWRITE_CACHE_FIELD_NUMBER: _ClassVar[int]
-    RAW_OUTPUT_DATA_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    max_parallelism: int
+    security_context: _security_pb2.SecurityContext
+    raw_output_data_config: _common_pb2.RawOutputDataConfig
+    labels: _common_pb2.Labels
     annotations: _common_pb2.Annotations
     interruptible: _wrappers_pb2.BoolValue
-    labels: _common_pb2.Labels
-    max_parallelism: int
     overwrite_cache: bool
-    raw_output_data_config: _common_pb2.RawOutputDataConfig
-    security_context: _security_pb2.SecurityContext
     def __init__(self, max_parallelism: _Optional[int] = ..., security_context: _Optional[_Union[_security_pb2.SecurityContext, _Mapping]] = ..., raw_output_data_config: _Optional[_Union[_common_pb2.RawOutputDataConfig, _Mapping]] = ..., labels: _Optional[_Union[_common_pb2.Labels, _Mapping]] = ..., annotations: _Optional[_Union[_common_pb2.Annotations, _Mapping]] = ..., interruptible: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., overwrite_cache: bool = ...) -> None: ...
 
-class MatchableResource(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class MatchingAttributes(_message.Message):
+    __slots__ = ["task_resource_attributes", "cluster_resource_attributes", "execution_queue_attributes", "execution_cluster_label", "quality_of_service", "plugin_overrides", "workflow_execution_config", "cluster_assignment"]
+    TASK_RESOURCE_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    CLUSTER_RESOURCE_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    EXECUTION_QUEUE_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    EXECUTION_CLUSTER_LABEL_FIELD_NUMBER: _ClassVar[int]
+    QUALITY_OF_SERVICE_FIELD_NUMBER: _ClassVar[int]
+    PLUGIN_OVERRIDES_FIELD_NUMBER: _ClassVar[int]
+    WORKFLOW_EXECUTION_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    CLUSTER_ASSIGNMENT_FIELD_NUMBER: _ClassVar[int]
+    task_resource_attributes: TaskResourceAttributes
+    cluster_resource_attributes: ClusterResourceAttributes
+    execution_queue_attributes: ExecutionQueueAttributes
+    execution_cluster_label: ExecutionClusterLabel
+    quality_of_service: _execution_pb2.QualityOfService
+    plugin_overrides: PluginOverrides
+    workflow_execution_config: WorkflowExecutionConfig
+    cluster_assignment: _cluster_assignment_pb2.ClusterAssignment
+    def __init__(self, task_resource_attributes: _Optional[_Union[TaskResourceAttributes, _Mapping]] = ..., cluster_resource_attributes: _Optional[_Union[ClusterResourceAttributes, _Mapping]] = ..., execution_queue_attributes: _Optional[_Union[ExecutionQueueAttributes, _Mapping]] = ..., execution_cluster_label: _Optional[_Union[ExecutionClusterLabel, _Mapping]] = ..., quality_of_service: _Optional[_Union[_execution_pb2.QualityOfService, _Mapping]] = ..., plugin_overrides: _Optional[_Union[PluginOverrides, _Mapping]] = ..., workflow_execution_config: _Optional[_Union[WorkflowExecutionConfig, _Mapping]] = ..., cluster_assignment: _Optional[_Union[_cluster_assignment_pb2.ClusterAssignment, _Mapping]] = ...) -> None: ...
+
+class MatchableAttributesConfiguration(_message.Message):
+    __slots__ = ["attributes", "domain", "project", "workflow", "launch_plan"]
+    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    WORKFLOW_FIELD_NUMBER: _ClassVar[int]
+    LAUNCH_PLAN_FIELD_NUMBER: _ClassVar[int]
+    attributes: MatchingAttributes
+    domain: str
+    project: str
+    workflow: str
+    launch_plan: str
+    def __init__(self, attributes: _Optional[_Union[MatchingAttributes, _Mapping]] = ..., domain: _Optional[str] = ..., project: _Optional[str] = ..., workflow: _Optional[str] = ..., launch_plan: _Optional[str] = ...) -> None: ...
+
+class ListMatchableAttributesRequest(_message.Message):
+    __slots__ = ["resource_type"]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    resource_type: MatchableResource
+    def __init__(self, resource_type: _Optional[_Union[MatchableResource, str]] = ...) -> None: ...
+
+class ListMatchableAttributesResponse(_message.Message):
+    __slots__ = ["configurations"]
+    CONFIGURATIONS_FIELD_NUMBER: _ClassVar[int]
+    configurations: _containers.RepeatedCompositeFieldContainer[MatchableAttributesConfiguration]
+    def __init__(self, configurations: _Optional[_Iterable[_Union[MatchableAttributesConfiguration, _Mapping]]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/node_execution_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/node_execution_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,48 +17,49 @@
 from flyteidl.core import compiler_pb2 as flyteidl_dot_core_dot_compiler__pb2
 from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#flyteidl/admin/node_execution.proto\x12\x0e\x66lyteidl.admin\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1b\x66lyteidl/core/catalog.proto\x1a\x1c\x66lyteidl/core/compiler.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\"Q\n\x17NodeExecutionGetRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\"\x99\x02\n\x18NodeExecutionListRequest\x12^\n\x15workflow_execution_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x13workflowExecutionId\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\x12(\n\x10unique_parent_id\x18\x06 \x01(\tR\x0euniqueParentId\"\xea\x01\n\x1fNodeExecutionForTaskListRequest\x12R\n\x11task_execution_id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x0ftaskExecutionId\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\"\xe7\x01\n\rNodeExecution\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\x12\x1b\n\tinput_uri\x18\x02 \x01(\tR\x08inputUri\x12>\n\x07\x63losure\x18\x03 \x01(\x0b\x32$.flyteidl.admin.NodeExecutionClosureR\x07\x63losure\x12\x41\n\x08metadata\x18\x04 \x01(\x0b\x32%.flyteidl.admin.NodeExecutionMetaDataR\x08metadata\"\x9f\x01\n\x15NodeExecutionMetaData\x12\x1f\n\x0bretry_group\x18\x01 \x01(\tR\nretryGroup\x12$\n\x0eis_parent_node\x18\x02 \x01(\x08R\x0cisParentNode\x12 \n\x0cspec_node_id\x18\x03 \x01(\tR\nspecNodeId\x12\x1d\n\nis_dynamic\x18\x04 \x01(\x08R\tisDynamic\"q\n\x11NodeExecutionList\x12\x46\n\x0fnode_executions\x18\x01 \x03(\x0b\x32\x1d.flyteidl.admin.NodeExecutionR\x0enodeExecutions\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\xc5\x05\n\x14NodeExecutionClosure\x12#\n\noutput_uri\x18\x01 \x01(\tB\x02\x18\x01H\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12@\n\x0boutput_data\x18\n \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\noutputData\x12\x38\n\x05phase\x18\x03 \x01(\x0e\x32\".flyteidl.core.NodeExecution.PhaseR\x05phase\x12\x39\n\nstarted_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartedAt\x12\x35\n\x08\x64uration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08\x64uration\x12\x39\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\\\n\x16workflow_node_metadata\x18\x08 \x01(\x0b\x32$.flyteidl.admin.WorkflowNodeMetadataH\x01R\x14workflowNodeMetadata\x12P\n\x12task_node_metadata\x18\t \x01(\x0b\x32 .flyteidl.admin.TaskNodeMetadataH\x01R\x10taskNodeMetadata\x12\x19\n\x08\x64\x65\x63k_uri\x18\x0b \x01(\tR\x07\x64\x65\x63kUriB\x0f\n\routput_resultB\x11\n\x0ftarget_metadata\"d\n\x14WorkflowNodeMetadata\x12L\n\x0b\x65xecutionId\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\"\xc0\x01\n\x10TaskNodeMetadata\x12\x44\n\x0c\x63\x61\x63he_status\x18\x01 \x01(\x0e\x32!.flyteidl.core.CatalogCacheStatusR\x0b\x63\x61\x63heStatus\x12?\n\x0b\x63\x61talog_key\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.CatalogMetadataR\ncatalogKey\x12%\n\x0e\x63heckpoint_uri\x18\x04 \x01(\tR\rcheckpointUri\"\x9d\x01\n\x1b\x44ynamicWorkflowNodeMetadata\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12S\n\x11\x63ompiled_workflow\x18\x02 \x01(\x0b\x32&.flyteidl.core.CompiledWorkflowClosureR\x10\x63ompiledWorkflow\"U\n\x1bNodeExecutionGetDataRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\"\xdc\x02\n\x1cNodeExecutionGetDataResponse\x12\x33\n\x06inputs\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x06inputs\x12\x35\n\x07outputs\x18\x02 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x07outputs\x12:\n\x0b\x66ull_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\nfullInputs\x12<\n\x0c\x66ull_outputs\x18\x04 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x0b\x66ullOutputs\x12V\n\x10\x64ynamic_workflow\x18\x10 \x01(\x0b\x32+.flyteidl.admin.DynamicWorkflowNodeMetadataR\x0f\x64ynamicWorkflowB\xb8\x01\n\x12\x63om.flyteidl.adminB\x12NodeExecutionProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#flyteidl/admin/node_execution.proto\x12\x0e\x66lyteidl.admin\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1b\x66lyteidl/core/catalog.proto\x1a\x1c\x66lyteidl/core/compiler.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\"Q\n\x17NodeExecutionGetRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\"\x99\x02\n\x18NodeExecutionListRequest\x12^\n\x15workflow_execution_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x13workflowExecutionId\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\x12(\n\x10unique_parent_id\x18\x06 \x01(\tR\x0euniqueParentId\"\xea\x01\n\x1fNodeExecutionForTaskListRequest\x12R\n\x11task_execution_id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x0ftaskExecutionId\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\"\xe7\x01\n\rNodeExecution\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\x12\x1b\n\tinput_uri\x18\x02 \x01(\tR\x08inputUri\x12>\n\x07\x63losure\x18\x03 \x01(\x0b\x32$.flyteidl.admin.NodeExecutionClosureR\x07\x63losure\x12\x41\n\x08metadata\x18\x04 \x01(\x0b\x32%.flyteidl.admin.NodeExecutionMetaDataR\x08metadata\"\x9f\x01\n\x15NodeExecutionMetaData\x12\x1f\n\x0bretry_group\x18\x01 \x01(\tR\nretryGroup\x12$\n\x0eis_parent_node\x18\x02 \x01(\x08R\x0cisParentNode\x12 \n\x0cspec_node_id\x18\x03 \x01(\tR\nspecNodeId\x12\x1d\n\nis_dynamic\x18\x04 \x01(\x08R\tisDynamic\"q\n\x11NodeExecutionList\x12\x46\n\x0fnode_executions\x18\x01 \x03(\x0b\x32\x1d.flyteidl.admin.NodeExecutionR\x0enodeExecutions\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\xf6\x05\n\x14NodeExecutionClosure\x12#\n\noutput_uri\x18\x01 \x01(\tB\x02\x18\x01H\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12@\n\x0boutput_data\x18\n \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\noutputData\x12\x38\n\x05phase\x18\x03 \x01(\x0e\x32\".flyteidl.core.NodeExecution.PhaseR\x05phase\x12\x39\n\nstarted_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartedAt\x12\x35\n\x08\x64uration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08\x64uration\x12\x39\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\\\n\x16workflow_node_metadata\x18\x08 \x01(\x0b\x32$.flyteidl.admin.WorkflowNodeMetadataH\x01R\x14workflowNodeMetadata\x12P\n\x12task_node_metadata\x18\t \x01(\x0b\x32 .flyteidl.admin.TaskNodeMetadataH\x01R\x10taskNodeMetadata\x12\x19\n\x08\x64\x65\x63k_uri\x18\x0b \x01(\tR\x07\x64\x65\x63kUri\x12/\n\x14\x64ynamic_job_spec_uri\x18\x0c \x01(\tR\x11\x64ynamicJobSpecUriB\x0f\n\routput_resultB\x11\n\x0ftarget_metadata\"d\n\x14WorkflowNodeMetadata\x12L\n\x0b\x65xecutionId\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\"\xc0\x01\n\x10TaskNodeMetadata\x12\x44\n\x0c\x63\x61\x63he_status\x18\x01 \x01(\x0e\x32!.flyteidl.core.CatalogCacheStatusR\x0b\x63\x61\x63heStatus\x12?\n\x0b\x63\x61talog_key\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.CatalogMetadataR\ncatalogKey\x12%\n\x0e\x63heckpoint_uri\x18\x04 \x01(\tR\rcheckpointUri\"\xce\x01\n\x1b\x44ynamicWorkflowNodeMetadata\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12S\n\x11\x63ompiled_workflow\x18\x02 \x01(\x0b\x32&.flyteidl.core.CompiledWorkflowClosureR\x10\x63ompiledWorkflow\x12/\n\x14\x64ynamic_job_spec_uri\x18\x03 \x01(\tR\x11\x64ynamicJobSpecUri\"U\n\x1bNodeExecutionGetDataRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\"\x96\x03\n\x1cNodeExecutionGetDataResponse\x12\x33\n\x06inputs\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x06inputs\x12\x35\n\x07outputs\x18\x02 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x07outputs\x12:\n\x0b\x66ull_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\nfullInputs\x12<\n\x0c\x66ull_outputs\x18\x04 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x0b\x66ullOutputs\x12V\n\x10\x64ynamic_workflow\x18\x10 \x01(\x0b\x32+.flyteidl.admin.DynamicWorkflowNodeMetadataR\x0f\x64ynamicWorkflow\x12\x38\n\nflyte_urls\x18\x11 \x01(\x0b\x32\x19.flyteidl.admin.FlyteURLsR\tflyteUrlsB\xb8\x01\n\x12\x63om.flyteidl.adminB\x12NodeExecutionProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.node_execution_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.node_execution_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\022NodeExecutionProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
   _NODEEXECUTIONCLOSURE.fields_by_name['output_uri']._options = None
   _NODEEXECUTIONCLOSURE.fields_by_name['output_uri']._serialized_options = b'\030\001'
   _NODEEXECUTIONCLOSURE.fields_by_name['output_data']._options = None
   _NODEEXECUTIONCLOSURE.fields_by_name['output_data']._serialized_options = b'\030\001'
   _NODEEXECUTIONGETDATARESPONSE.fields_by_name['inputs']._options = None
   _NODEEXECUTIONGETDATARESPONSE.fields_by_name['inputs']._serialized_options = b'\030\001'
   _NODEEXECUTIONGETDATARESPONSE.fields_by_name['outputs']._options = None
   _NODEEXECUTIONGETDATARESPONSE.fields_by_name['outputs']._serialized_options = b'\030\001'
-  _NODEEXECUTIONGETREQUEST._serialized_start=301
-  _NODEEXECUTIONGETREQUEST._serialized_end=382
-  _NODEEXECUTIONLISTREQUEST._serialized_start=385
-  _NODEEXECUTIONLISTREQUEST._serialized_end=666
-  _NODEEXECUTIONFORTASKLISTREQUEST._serialized_start=669
-  _NODEEXECUTIONFORTASKLISTREQUEST._serialized_end=903
-  _NODEEXECUTION._serialized_start=906
-  _NODEEXECUTION._serialized_end=1137
-  _NODEEXECUTIONMETADATA._serialized_start=1140
-  _NODEEXECUTIONMETADATA._serialized_end=1299
-  _NODEEXECUTIONLIST._serialized_start=1301
-  _NODEEXECUTIONLIST._serialized_end=1414
-  _NODEEXECUTIONCLOSURE._serialized_start=1417
-  _NODEEXECUTIONCLOSURE._serialized_end=2126
-  _WORKFLOWNODEMETADATA._serialized_start=2128
-  _WORKFLOWNODEMETADATA._serialized_end=2228
-  _TASKNODEMETADATA._serialized_start=2231
-  _TASKNODEMETADATA._serialized_end=2423
-  _DYNAMICWORKFLOWNODEMETADATA._serialized_start=2426
-  _DYNAMICWORKFLOWNODEMETADATA._serialized_end=2583
-  _NODEEXECUTIONGETDATAREQUEST._serialized_start=2585
-  _NODEEXECUTIONGETDATAREQUEST._serialized_end=2670
-  _NODEEXECUTIONGETDATARESPONSE._serialized_start=2673
-  _NODEEXECUTIONGETDATARESPONSE._serialized_end=3021
+  _globals['_NODEEXECUTIONGETREQUEST']._serialized_start=301
+  _globals['_NODEEXECUTIONGETREQUEST']._serialized_end=382
+  _globals['_NODEEXECUTIONLISTREQUEST']._serialized_start=385
+  _globals['_NODEEXECUTIONLISTREQUEST']._serialized_end=666
+  _globals['_NODEEXECUTIONFORTASKLISTREQUEST']._serialized_start=669
+  _globals['_NODEEXECUTIONFORTASKLISTREQUEST']._serialized_end=903
+  _globals['_NODEEXECUTION']._serialized_start=906
+  _globals['_NODEEXECUTION']._serialized_end=1137
+  _globals['_NODEEXECUTIONMETADATA']._serialized_start=1140
+  _globals['_NODEEXECUTIONMETADATA']._serialized_end=1299
+  _globals['_NODEEXECUTIONLIST']._serialized_start=1301
+  _globals['_NODEEXECUTIONLIST']._serialized_end=1414
+  _globals['_NODEEXECUTIONCLOSURE']._serialized_start=1417
+  _globals['_NODEEXECUTIONCLOSURE']._serialized_end=2175
+  _globals['_WORKFLOWNODEMETADATA']._serialized_start=2177
+  _globals['_WORKFLOWNODEMETADATA']._serialized_end=2277
+  _globals['_TASKNODEMETADATA']._serialized_start=2280
+  _globals['_TASKNODEMETADATA']._serialized_end=2472
+  _globals['_DYNAMICWORKFLOWNODEMETADATA']._serialized_start=2475
+  _globals['_DYNAMICWORKFLOWNODEMETADATA']._serialized_end=2681
+  _globals['_NODEEXECUTIONGETDATAREQUEST']._serialized_start=2683
+  _globals['_NODEEXECUTIONGETDATAREQUEST']._serialized_end=2768
+  _globals['_NODEEXECUTIONGETDATARESPONSE']._serialized_start=2771
+  _globals['_NODEEXECUTIONGETDATARESPONSE']._serialized_end=3177
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/node_execution_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/node_execution_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,144 +9,150 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DynamicWorkflowNodeMetadata(_message.Message):
-    __slots__ = ["compiled_workflow", "id"]
-    COMPILED_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
+class NodeExecutionGetRequest(_message.Message):
+    __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    compiled_workflow: _compiler_pb2.CompiledWorkflowClosure
-    id: _identifier_pb2.Identifier
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., compiled_workflow: _Optional[_Union[_compiler_pb2.CompiledWorkflowClosure, _Mapping]] = ...) -> None: ...
+    id: _identifier_pb2.NodeExecutionIdentifier
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ...) -> None: ...
+
+class NodeExecutionListRequest(_message.Message):
+    __slots__ = ["workflow_execution_id", "limit", "token", "filters", "sort_by", "unique_parent_id"]
+    WORKFLOW_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    UNIQUE_PARENT_ID_FIELD_NUMBER: _ClassVar[int]
+    workflow_execution_id: _identifier_pb2.WorkflowExecutionIdentifier
+    limit: int
+    token: str
+    filters: str
+    sort_by: _common_pb2.Sort
+    unique_parent_id: str
+    def __init__(self, workflow_execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ..., unique_parent_id: _Optional[str] = ...) -> None: ...
+
+class NodeExecutionForTaskListRequest(_message.Message):
+    __slots__ = ["task_execution_id", "limit", "token", "filters", "sort_by"]
+    TASK_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    task_execution_id: _identifier_pb2.TaskExecutionIdentifier
+    limit: int
+    token: str
+    filters: str
+    sort_by: _common_pb2.Sort
+    def __init__(self, task_execution_id: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
 
 class NodeExecution(_message.Message):
-    __slots__ = ["closure", "id", "input_uri", "metadata"]
-    CLOSURE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "input_uri", "closure", "metadata"]
     ID_FIELD_NUMBER: _ClassVar[int]
     INPUT_URI_FIELD_NUMBER: _ClassVar[int]
+    CLOSURE_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
-    closure: NodeExecutionClosure
     id: _identifier_pb2.NodeExecutionIdentifier
     input_uri: str
+    closure: NodeExecutionClosure
     metadata: NodeExecutionMetaData
     def __init__(self, id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., input_uri: _Optional[str] = ..., closure: _Optional[_Union[NodeExecutionClosure, _Mapping]] = ..., metadata: _Optional[_Union[NodeExecutionMetaData, _Mapping]] = ...) -> None: ...
 
+class NodeExecutionMetaData(_message.Message):
+    __slots__ = ["retry_group", "is_parent_node", "spec_node_id", "is_dynamic"]
+    RETRY_GROUP_FIELD_NUMBER: _ClassVar[int]
+    IS_PARENT_NODE_FIELD_NUMBER: _ClassVar[int]
+    SPEC_NODE_ID_FIELD_NUMBER: _ClassVar[int]
+    IS_DYNAMIC_FIELD_NUMBER: _ClassVar[int]
+    retry_group: str
+    is_parent_node: bool
+    spec_node_id: str
+    is_dynamic: bool
+    def __init__(self, retry_group: _Optional[str] = ..., is_parent_node: bool = ..., spec_node_id: _Optional[str] = ..., is_dynamic: bool = ...) -> None: ...
+
+class NodeExecutionList(_message.Message):
+    __slots__ = ["node_executions", "token"]
+    NODE_EXECUTIONS_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    node_executions: _containers.RepeatedCompositeFieldContainer[NodeExecution]
+    token: str
+    def __init__(self, node_executions: _Optional[_Iterable[_Union[NodeExecution, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
+
 class NodeExecutionClosure(_message.Message):
-    __slots__ = ["created_at", "deck_uri", "duration", "error", "output_data", "output_uri", "phase", "started_at", "task_node_metadata", "updated_at", "workflow_node_metadata"]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    DECK_URI_FIELD_NUMBER: _ClassVar[int]
-    DURATION_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["output_uri", "error", "output_data", "phase", "started_at", "duration", "created_at", "updated_at", "workflow_node_metadata", "task_node_metadata", "deck_uri", "dynamic_job_spec_uri"]
+    OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
     PHASE_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
-    TASK_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
     WORKFLOW_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
-    created_at: _timestamp_pb2.Timestamp
-    deck_uri: str
-    duration: _duration_pb2.Duration
+    TASK_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
+    DECK_URI_FIELD_NUMBER: _ClassVar[int]
+    DYNAMIC_JOB_SPEC_URI_FIELD_NUMBER: _ClassVar[int]
+    output_uri: str
     error: _execution_pb2.ExecutionError
     output_data: _literals_pb2.LiteralMap
-    output_uri: str
     phase: _execution_pb2.NodeExecution.Phase
     started_at: _timestamp_pb2.Timestamp
-    task_node_metadata: TaskNodeMetadata
+    duration: _duration_pb2.Duration
+    created_at: _timestamp_pb2.Timestamp
     updated_at: _timestamp_pb2.Timestamp
     workflow_node_metadata: WorkflowNodeMetadata
-    def __init__(self, output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., phase: _Optional[_Union[_execution_pb2.NodeExecution.Phase, str]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., workflow_node_metadata: _Optional[_Union[WorkflowNodeMetadata, _Mapping]] = ..., task_node_metadata: _Optional[_Union[TaskNodeMetadata, _Mapping]] = ..., deck_uri: _Optional[str] = ...) -> None: ...
+    task_node_metadata: TaskNodeMetadata
+    deck_uri: str
+    dynamic_job_spec_uri: str
+    def __init__(self, output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., phase: _Optional[_Union[_execution_pb2.NodeExecution.Phase, str]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., workflow_node_metadata: _Optional[_Union[WorkflowNodeMetadata, _Mapping]] = ..., task_node_metadata: _Optional[_Union[TaskNodeMetadata, _Mapping]] = ..., deck_uri: _Optional[str] = ..., dynamic_job_spec_uri: _Optional[str] = ...) -> None: ...
 
-class NodeExecutionForTaskListRequest(_message.Message):
-    __slots__ = ["filters", "limit", "sort_by", "task_execution_id", "token"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
-    TASK_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    filters: str
-    limit: int
-    sort_by: _common_pb2.Sort
-    task_execution_id: _identifier_pb2.TaskExecutionIdentifier
-    token: str
-    def __init__(self, task_execution_id: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
+class WorkflowNodeMetadata(_message.Message):
+    __slots__ = ["executionId"]
+    EXECUTIONID_FIELD_NUMBER: _ClassVar[int]
+    executionId: _identifier_pb2.WorkflowExecutionIdentifier
+    def __init__(self, executionId: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
+
+class TaskNodeMetadata(_message.Message):
+    __slots__ = ["cache_status", "catalog_key", "checkpoint_uri"]
+    CACHE_STATUS_FIELD_NUMBER: _ClassVar[int]
+    CATALOG_KEY_FIELD_NUMBER: _ClassVar[int]
+    CHECKPOINT_URI_FIELD_NUMBER: _ClassVar[int]
+    cache_status: _catalog_pb2.CatalogCacheStatus
+    catalog_key: _catalog_pb2.CatalogMetadata
+    checkpoint_uri: str
+    def __init__(self, cache_status: _Optional[_Union[_catalog_pb2.CatalogCacheStatus, str]] = ..., catalog_key: _Optional[_Union[_catalog_pb2.CatalogMetadata, _Mapping]] = ..., checkpoint_uri: _Optional[str] = ...) -> None: ...
+
+class DynamicWorkflowNodeMetadata(_message.Message):
+    __slots__ = ["id", "compiled_workflow", "dynamic_job_spec_uri"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
+    DYNAMIC_JOB_SPEC_URI_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.Identifier
+    compiled_workflow: _compiler_pb2.CompiledWorkflowClosure
+    dynamic_job_spec_uri: str
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., compiled_workflow: _Optional[_Union[_compiler_pb2.CompiledWorkflowClosure, _Mapping]] = ..., dynamic_job_spec_uri: _Optional[str] = ...) -> None: ...
 
 class NodeExecutionGetDataRequest(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.NodeExecutionIdentifier
     def __init__(self, id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
 class NodeExecutionGetDataResponse(_message.Message):
-    __slots__ = ["dynamic_workflow", "full_inputs", "full_outputs", "inputs", "outputs"]
-    DYNAMIC_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    FULL_INPUTS_FIELD_NUMBER: _ClassVar[int]
-    FULL_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["inputs", "outputs", "full_inputs", "full_outputs", "dynamic_workflow", "flyte_urls"]
     INPUTS_FIELD_NUMBER: _ClassVar[int]
     OUTPUTS_FIELD_NUMBER: _ClassVar[int]
-    dynamic_workflow: DynamicWorkflowNodeMetadata
-    full_inputs: _literals_pb2.LiteralMap
-    full_outputs: _literals_pb2.LiteralMap
+    FULL_INPUTS_FIELD_NUMBER: _ClassVar[int]
+    FULL_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    DYNAMIC_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
+    FLYTE_URLS_FIELD_NUMBER: _ClassVar[int]
     inputs: _common_pb2.UrlBlob
     outputs: _common_pb2.UrlBlob
-    def __init__(self, inputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., outputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., full_inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., full_outputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., dynamic_workflow: _Optional[_Union[DynamicWorkflowNodeMetadata, _Mapping]] = ...) -> None: ...
-
-class NodeExecutionGetRequest(_message.Message):
-    __slots__ = ["id"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.NodeExecutionIdentifier
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ...) -> None: ...
-
-class NodeExecutionList(_message.Message):
-    __slots__ = ["node_executions", "token"]
-    NODE_EXECUTIONS_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    node_executions: _containers.RepeatedCompositeFieldContainer[NodeExecution]
-    token: str
-    def __init__(self, node_executions: _Optional[_Iterable[_Union[NodeExecution, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
-
-class NodeExecutionListRequest(_message.Message):
-    __slots__ = ["filters", "limit", "sort_by", "token", "unique_parent_id", "workflow_execution_id"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    UNIQUE_PARENT_ID_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    filters: str
-    limit: int
-    sort_by: _common_pb2.Sort
-    token: str
-    unique_parent_id: str
-    workflow_execution_id: _identifier_pb2.WorkflowExecutionIdentifier
-    def __init__(self, workflow_execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ..., unique_parent_id: _Optional[str] = ...) -> None: ...
-
-class NodeExecutionMetaData(_message.Message):
-    __slots__ = ["is_dynamic", "is_parent_node", "retry_group", "spec_node_id"]
-    IS_DYNAMIC_FIELD_NUMBER: _ClassVar[int]
-    IS_PARENT_NODE_FIELD_NUMBER: _ClassVar[int]
-    RETRY_GROUP_FIELD_NUMBER: _ClassVar[int]
-    SPEC_NODE_ID_FIELD_NUMBER: _ClassVar[int]
-    is_dynamic: bool
-    is_parent_node: bool
-    retry_group: str
-    spec_node_id: str
-    def __init__(self, retry_group: _Optional[str] = ..., is_parent_node: bool = ..., spec_node_id: _Optional[str] = ..., is_dynamic: bool = ...) -> None: ...
-
-class TaskNodeMetadata(_message.Message):
-    __slots__ = ["cache_status", "catalog_key", "checkpoint_uri"]
-    CACHE_STATUS_FIELD_NUMBER: _ClassVar[int]
-    CATALOG_KEY_FIELD_NUMBER: _ClassVar[int]
-    CHECKPOINT_URI_FIELD_NUMBER: _ClassVar[int]
-    cache_status: _catalog_pb2.CatalogCacheStatus
-    catalog_key: _catalog_pb2.CatalogMetadata
-    checkpoint_uri: str
-    def __init__(self, cache_status: _Optional[_Union[_catalog_pb2.CatalogCacheStatus, str]] = ..., catalog_key: _Optional[_Union[_catalog_pb2.CatalogMetadata, _Mapping]] = ..., checkpoint_uri: _Optional[str] = ...) -> None: ...
-
-class WorkflowNodeMetadata(_message.Message):
-    __slots__ = ["executionId"]
-    EXECUTIONID_FIELD_NUMBER: _ClassVar[int]
-    executionId: _identifier_pb2.WorkflowExecutionIdentifier
-    def __init__(self, executionId: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
+    full_inputs: _literals_pb2.LiteralMap
+    full_outputs: _literals_pb2.LiteralMap
+    dynamic_workflow: DynamicWorkflowNodeMetadata
+    flyte_urls: _common_pb2.FlyteURLs
+    def __init__(self, inputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., outputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., full_inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., full_outputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., dynamic_workflow: _Optional[_Union[DynamicWorkflowNodeMetadata, _Mapping]] = ..., flyte_urls: _Optional[_Union[_common_pb2.FlyteURLs, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/notification_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/notification_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!flyteidl/admin/notification.proto\x12\x0e\x66lyteidl.admin\"\x93\x01\n\x0c\x45mailMessage\x12)\n\x10recipients_email\x18\x01 \x03(\tR\x0frecipientsEmail\x12!\n\x0csender_email\x18\x02 \x01(\tR\x0bsenderEmail\x12!\n\x0csubject_line\x18\x03 \x01(\tR\x0bsubjectLine\x12\x12\n\x04\x62ody\x18\x04 \x01(\tR\x04\x62odyB\xb7\x01\n\x12\x63om.flyteidl.adminB\x11NotificationProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.notification_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.notification_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\021NotificationProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _EMAILMESSAGE._serialized_start=54
-  _EMAILMESSAGE._serialized_end=201
+  _globals['_EMAILMESSAGE']._serialized_start=54
+  _globals['_EMAILMESSAGE']._serialized_end=201
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/notification_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/notification_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class EmailMessage(_message.Message):
-    __slots__ = ["body", "recipients_email", "sender_email", "subject_line"]
-    BODY_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["recipients_email", "sender_email", "subject_line", "body"]
     RECIPIENTS_EMAIL_FIELD_NUMBER: _ClassVar[int]
     SENDER_EMAIL_FIELD_NUMBER: _ClassVar[int]
     SUBJECT_LINE_FIELD_NUMBER: _ClassVar[int]
-    body: str
+    BODY_FIELD_NUMBER: _ClassVar[int]
     recipients_email: _containers.RepeatedScalarFieldContainer[str]
     sender_email: str
     subject_line: str
+    body: str
     def __init__(self, recipients_email: _Optional[_Iterable[str]] = ..., sender_email: _Optional[str] = ..., subject_line: _Optional[str] = ..., body: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_attributes_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_attributes_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 
 
 from flyteidl.admin import matchable_resource_pb2 as flyteidl_dot_admin_dot_matchable__resource__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'flyteidl/admin/project_attributes.proto\x12\x0e\x66lyteidl.admin\x1a\'flyteidl/admin/matchable_resource.proto\"\x82\x01\n\x11ProjectAttributes\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12S\n\x13matching_attributes\x18\x02 \x01(\x0b\x32\".flyteidl.admin.MatchingAttributesR\x12matchingAttributes\"c\n\x1eProjectAttributesUpdateRequest\x12\x41\n\nattributes\x18\x01 \x01(\x0b\x32!.flyteidl.admin.ProjectAttributesR\nattributes\"!\n\x1fProjectAttributesUpdateResponse\"\x7f\n\x1bProjectAttributesGetRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x46\n\rresource_type\x18\x02 \x01(\x0e\x32!.flyteidl.admin.MatchableResourceR\x0cresourceType\"a\n\x1cProjectAttributesGetResponse\x12\x41\n\nattributes\x18\x01 \x01(\x0b\x32!.flyteidl.admin.ProjectAttributesR\nattributes\"\x82\x01\n\x1eProjectAttributesDeleteRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x46\n\rresource_type\x18\x02 \x01(\x0e\x32!.flyteidl.admin.MatchableResourceR\x0cresourceType\"!\n\x1fProjectAttributesDeleteResponseB\xbc\x01\n\x12\x63om.flyteidl.adminB\x16ProjectAttributesProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.project_attributes_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.project_attributes_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\026ProjectAttributesProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _PROJECTATTRIBUTES._serialized_start=101
-  _PROJECTATTRIBUTES._serialized_end=231
-  _PROJECTATTRIBUTESUPDATEREQUEST._serialized_start=233
-  _PROJECTATTRIBUTESUPDATEREQUEST._serialized_end=332
-  _PROJECTATTRIBUTESUPDATERESPONSE._serialized_start=334
-  _PROJECTATTRIBUTESUPDATERESPONSE._serialized_end=367
-  _PROJECTATTRIBUTESGETREQUEST._serialized_start=369
-  _PROJECTATTRIBUTESGETREQUEST._serialized_end=496
-  _PROJECTATTRIBUTESGETRESPONSE._serialized_start=498
-  _PROJECTATTRIBUTESGETRESPONSE._serialized_end=595
-  _PROJECTATTRIBUTESDELETEREQUEST._serialized_start=598
-  _PROJECTATTRIBUTESDELETEREQUEST._serialized_end=728
-  _PROJECTATTRIBUTESDELETERESPONSE._serialized_start=730
-  _PROJECTATTRIBUTESDELETERESPONSE._serialized_end=763
+  _globals['_PROJECTATTRIBUTES']._serialized_start=101
+  _globals['_PROJECTATTRIBUTES']._serialized_end=231
+  _globals['_PROJECTATTRIBUTESUPDATEREQUEST']._serialized_start=233
+  _globals['_PROJECTATTRIBUTESUPDATEREQUEST']._serialized_end=332
+  _globals['_PROJECTATTRIBUTESUPDATERESPONSE']._serialized_start=334
+  _globals['_PROJECTATTRIBUTESUPDATERESPONSE']._serialized_end=367
+  _globals['_PROJECTATTRIBUTESGETREQUEST']._serialized_start=369
+  _globals['_PROJECTATTRIBUTESGETREQUEST']._serialized_end=496
+  _globals['_PROJECTATTRIBUTESGETRESPONSE']._serialized_start=498
+  _globals['_PROJECTATTRIBUTESGETRESPONSE']._serialized_end=595
+  _globals['_PROJECTATTRIBUTESDELETEREQUEST']._serialized_start=598
+  _globals['_PROJECTATTRIBUTESDELETEREQUEST']._serialized_end=728
+  _globals['_PROJECTATTRIBUTESDELETERESPONSE']._serialized_start=730
+  _globals['_PROJECTATTRIBUTESDELETERESPONSE']._serialized_end=763
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_attributes_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_attributes_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ProjectAttributes(_message.Message):
-    __slots__ = ["matching_attributes", "project"]
-    MATCHING_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["project", "matching_attributes"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
-    matching_attributes: _matchable_resource_pb2.MatchingAttributes
+    MATCHING_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     project: str
+    matching_attributes: _matchable_resource_pb2.MatchingAttributes
     def __init__(self, project: _Optional[str] = ..., matching_attributes: _Optional[_Union[_matchable_resource_pb2.MatchingAttributes, _Mapping]] = ...) -> None: ...
 
-class ProjectAttributesDeleteRequest(_message.Message):
-    __slots__ = ["project", "resource_type"]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    project: str
-    resource_type: _matchable_resource_pb2.MatchableResource
-    def __init__(self, project: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
+class ProjectAttributesUpdateRequest(_message.Message):
+    __slots__ = ["attributes"]
+    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    attributes: ProjectAttributes
+    def __init__(self, attributes: _Optional[_Union[ProjectAttributes, _Mapping]] = ...) -> None: ...
 
-class ProjectAttributesDeleteResponse(_message.Message):
+class ProjectAttributesUpdateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class ProjectAttributesGetRequest(_message.Message):
     __slots__ = ["project", "resource_type"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
@@ -35,16 +33,18 @@
 
 class ProjectAttributesGetResponse(_message.Message):
     __slots__ = ["attributes"]
     ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     attributes: ProjectAttributes
     def __init__(self, attributes: _Optional[_Union[ProjectAttributes, _Mapping]] = ...) -> None: ...
 
-class ProjectAttributesUpdateRequest(_message.Message):
-    __slots__ = ["attributes"]
-    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    attributes: ProjectAttributes
-    def __init__(self, attributes: _Optional[_Union[ProjectAttributes, _Mapping]] = ...) -> None: ...
+class ProjectAttributesDeleteRequest(_message.Message):
+    __slots__ = ["project", "resource_type"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    resource_type: _matchable_resource_pb2.MatchableResource
+    def __init__(self, project: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
 
-class ProjectAttributesUpdateResponse(_message.Message):
+class ProjectAttributesDeleteResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 
 
 from flyteidl.admin import matchable_resource_pb2 as flyteidl_dot_admin_dot_matchable__resource__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.flyteidl/admin/project_domain_attributes.proto\x12\x0e\x66lyteidl.admin\x1a\'flyteidl/admin/matchable_resource.proto\"\xa0\x01\n\x17ProjectDomainAttributes\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12S\n\x13matching_attributes\x18\x03 \x01(\x0b\x32\".flyteidl.admin.MatchingAttributesR\x12matchingAttributes\"o\n$ProjectDomainAttributesUpdateRequest\x12G\n\nattributes\x18\x01 \x01(\x0b\x32\'.flyteidl.admin.ProjectDomainAttributesR\nattributes\"\'\n%ProjectDomainAttributesUpdateResponse\"\x9d\x01\n!ProjectDomainAttributesGetRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x46\n\rresource_type\x18\x03 \x01(\x0e\x32!.flyteidl.admin.MatchableResourceR\x0cresourceType\"m\n\"ProjectDomainAttributesGetResponse\x12G\n\nattributes\x18\x01 \x01(\x0b\x32\'.flyteidl.admin.ProjectDomainAttributesR\nattributes\"\xa0\x01\n$ProjectDomainAttributesDeleteRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x46\n\rresource_type\x18\x03 \x01(\x0e\x32!.flyteidl.admin.MatchableResourceR\x0cresourceType\"\'\n%ProjectDomainAttributesDeleteResponseB\xc2\x01\n\x12\x63om.flyteidl.adminB\x1cProjectDomainAttributesProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.project_domain_attributes_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.project_domain_attributes_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\034ProjectDomainAttributesProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _PROJECTDOMAINATTRIBUTES._serialized_start=108
-  _PROJECTDOMAINATTRIBUTES._serialized_end=268
-  _PROJECTDOMAINATTRIBUTESUPDATEREQUEST._serialized_start=270
-  _PROJECTDOMAINATTRIBUTESUPDATEREQUEST._serialized_end=381
-  _PROJECTDOMAINATTRIBUTESUPDATERESPONSE._serialized_start=383
-  _PROJECTDOMAINATTRIBUTESUPDATERESPONSE._serialized_end=422
-  _PROJECTDOMAINATTRIBUTESGETREQUEST._serialized_start=425
-  _PROJECTDOMAINATTRIBUTESGETREQUEST._serialized_end=582
-  _PROJECTDOMAINATTRIBUTESGETRESPONSE._serialized_start=584
-  _PROJECTDOMAINATTRIBUTESGETRESPONSE._serialized_end=693
-  _PROJECTDOMAINATTRIBUTESDELETEREQUEST._serialized_start=696
-  _PROJECTDOMAINATTRIBUTESDELETEREQUEST._serialized_end=856
-  _PROJECTDOMAINATTRIBUTESDELETERESPONSE._serialized_start=858
-  _PROJECTDOMAINATTRIBUTESDELETERESPONSE._serialized_end=897
+  _globals['_PROJECTDOMAINATTRIBUTES']._serialized_start=108
+  _globals['_PROJECTDOMAINATTRIBUTES']._serialized_end=268
+  _globals['_PROJECTDOMAINATTRIBUTESUPDATEREQUEST']._serialized_start=270
+  _globals['_PROJECTDOMAINATTRIBUTESUPDATEREQUEST']._serialized_end=381
+  _globals['_PROJECTDOMAINATTRIBUTESUPDATERESPONSE']._serialized_start=383
+  _globals['_PROJECTDOMAINATTRIBUTESUPDATERESPONSE']._serialized_end=422
+  _globals['_PROJECTDOMAINATTRIBUTESGETREQUEST']._serialized_start=425
+  _globals['_PROJECTDOMAINATTRIBUTESGETREQUEST']._serialized_end=582
+  _globals['_PROJECTDOMAINATTRIBUTESGETRESPONSE']._serialized_start=584
+  _globals['_PROJECTDOMAINATTRIBUTESGETRESPONSE']._serialized_end=693
+  _globals['_PROJECTDOMAINATTRIBUTESDELETEREQUEST']._serialized_start=696
+  _globals['_PROJECTDOMAINATTRIBUTESDELETEREQUEST']._serialized_end=856
+  _globals['_PROJECTDOMAINATTRIBUTESDELETERESPONSE']._serialized_start=858
+  _globals['_PROJECTDOMAINATTRIBUTESDELETERESPONSE']._serialized_end=897
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,55 +2,55 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ProjectDomainAttributes(_message.Message):
-    __slots__ = ["domain", "matching_attributes", "project"]
+    __slots__ = ["project", "domain", "matching_attributes"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
     DOMAIN_FIELD_NUMBER: _ClassVar[int]
     MATCHING_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    project: str
     domain: str
     matching_attributes: _matchable_resource_pb2.MatchingAttributes
-    project: str
     def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., matching_attributes: _Optional[_Union[_matchable_resource_pb2.MatchingAttributes, _Mapping]] = ...) -> None: ...
 
-class ProjectDomainAttributesDeleteRequest(_message.Message):
-    __slots__ = ["domain", "project", "resource_type"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    project: str
-    resource_type: _matchable_resource_pb2.MatchableResource
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
+class ProjectDomainAttributesUpdateRequest(_message.Message):
+    __slots__ = ["attributes"]
+    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    attributes: ProjectDomainAttributes
+    def __init__(self, attributes: _Optional[_Union[ProjectDomainAttributes, _Mapping]] = ...) -> None: ...
 
-class ProjectDomainAttributesDeleteResponse(_message.Message):
+class ProjectDomainAttributesUpdateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class ProjectDomainAttributesGetRequest(_message.Message):
-    __slots__ = ["domain", "project", "resource_type"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["project", "domain", "resource_type"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    domain: str
     project: str
+    domain: str
     resource_type: _matchable_resource_pb2.MatchableResource
     def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
 
 class ProjectDomainAttributesGetResponse(_message.Message):
     __slots__ = ["attributes"]
     ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     attributes: ProjectDomainAttributes
     def __init__(self, attributes: _Optional[_Union[ProjectDomainAttributes, _Mapping]] = ...) -> None: ...
 
-class ProjectDomainAttributesUpdateRequest(_message.Message):
-    __slots__ = ["attributes"]
-    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    attributes: ProjectDomainAttributes
-    def __init__(self, attributes: _Optional[_Union[ProjectDomainAttributes, _Mapping]] = ...) -> None: ...
+class ProjectDomainAttributesDeleteRequest(_message.Message):
+    __slots__ = ["project", "domain", "resource_type"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    resource_type: _matchable_resource_pb2.MatchableResource
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
 
-class ProjectDomainAttributesUpdateResponse(_message.Message):
+class ProjectDomainAttributesDeleteResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 
 
 from flyteidl.admin import common_pb2 as flyteidl_dot_admin_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/admin/project.proto\x12\x0e\x66lyteidl.admin\x1a\x1b\x66lyteidl/admin/common.proto\",\n\x06\x44omain\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"\xad\x02\n\x07Project\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x30\n\x07\x64omains\x18\x03 \x03(\x0b\x32\x16.flyteidl.admin.DomainR\x07\x64omains\x12 \n\x0b\x64\x65scription\x18\x04 \x01(\tR\x0b\x64\x65scription\x12.\n\x06labels\x18\x05 \x01(\x0b\x32\x16.flyteidl.admin.LabelsR\x06labels\x12:\n\x05state\x18\x06 \x01(\x0e\x32$.flyteidl.admin.Project.ProjectStateR\x05state\">\n\x0cProjectState\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08\x41RCHIVED\x10\x01\x12\x14\n\x10SYSTEM_GENERATED\x10\x02\"U\n\x08Projects\x12\x33\n\x08projects\x18\x01 \x03(\x0b\x32\x17.flyteidl.admin.ProjectR\x08projects\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x89\x01\n\x12ProjectListRequest\x12\x14\n\x05limit\x18\x01 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x03 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x04 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\"K\n\x16ProjectRegisterRequest\x12\x31\n\x07project\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.ProjectR\x07project\"\x19\n\x17ProjectRegisterResponse\"\x17\n\x15ProjectUpdateResponseB\xb2\x01\n\x12\x63om.flyteidl.adminB\x0cProjectProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.project_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.project_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\014ProjectProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _DOMAIN._serialized_start=77
-  _DOMAIN._serialized_end=121
-  _PROJECT._serialized_start=124
-  _PROJECT._serialized_end=425
-  _PROJECT_PROJECTSTATE._serialized_start=363
-  _PROJECT_PROJECTSTATE._serialized_end=425
-  _PROJECTS._serialized_start=427
-  _PROJECTS._serialized_end=512
-  _PROJECTLISTREQUEST._serialized_start=515
-  _PROJECTLISTREQUEST._serialized_end=652
-  _PROJECTREGISTERREQUEST._serialized_start=654
-  _PROJECTREGISTERREQUEST._serialized_end=729
-  _PROJECTREGISTERRESPONSE._serialized_start=731
-  _PROJECTREGISTERRESPONSE._serialized_end=756
-  _PROJECTUPDATERESPONSE._serialized_start=758
-  _PROJECTUPDATERESPONSE._serialized_end=781
+  _globals['_DOMAIN']._serialized_start=77
+  _globals['_DOMAIN']._serialized_end=121
+  _globals['_PROJECT']._serialized_start=124
+  _globals['_PROJECT']._serialized_end=425
+  _globals['_PROJECT_PROJECTSTATE']._serialized_start=363
+  _globals['_PROJECT_PROJECTSTATE']._serialized_end=425
+  _globals['_PROJECTS']._serialized_start=427
+  _globals['_PROJECTS']._serialized_end=512
+  _globals['_PROJECTLISTREQUEST']._serialized_start=515
+  _globals['_PROJECTLISTREQUEST']._serialized_end=652
+  _globals['_PROJECTREGISTERREQUEST']._serialized_start=654
+  _globals['_PROJECTREGISTERREQUEST']._serialized_end=729
+  _globals['_PROJECTREGISTERRESPONSE']._serialized_start=731
+  _globals['_PROJECTREGISTERRESPONSE']._serialized_end=756
+  _globals['_PROJECTUPDATERESPONSE']._serialized_start=758
+  _globals['_PROJECTUPDATERESPONSE']._serialized_end=781
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/project_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/project_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,44 +12,55 @@
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
 
 class Project(_message.Message):
-    __slots__ = ["description", "domains", "id", "labels", "name", "state"]
+    __slots__ = ["id", "name", "domains", "description", "labels", "state"]
     class ProjectState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        ACTIVE: _ClassVar[Project.ProjectState]
+        ARCHIVED: _ClassVar[Project.ProjectState]
+        SYSTEM_GENERATED: _ClassVar[Project.ProjectState]
     ACTIVE: Project.ProjectState
     ARCHIVED: Project.ProjectState
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    DOMAINS_FIELD_NUMBER: _ClassVar[int]
+    SYSTEM_GENERATED: Project.ProjectState
     ID_FIELD_NUMBER: _ClassVar[int]
-    LABELS_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    DOMAINS_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    LABELS_FIELD_NUMBER: _ClassVar[int]
     STATE_FIELD_NUMBER: _ClassVar[int]
-    SYSTEM_GENERATED: Project.ProjectState
-    description: str
-    domains: _containers.RepeatedCompositeFieldContainer[Domain]
     id: str
-    labels: _common_pb2.Labels
     name: str
+    domains: _containers.RepeatedCompositeFieldContainer[Domain]
+    description: str
+    labels: _common_pb2.Labels
     state: Project.ProjectState
     def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., domains: _Optional[_Iterable[_Union[Domain, _Mapping]]] = ..., description: _Optional[str] = ..., labels: _Optional[_Union[_common_pb2.Labels, _Mapping]] = ..., state: _Optional[_Union[Project.ProjectState, str]] = ...) -> None: ...
 
+class Projects(_message.Message):
+    __slots__ = ["projects", "token"]
+    PROJECTS_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    projects: _containers.RepeatedCompositeFieldContainer[Project]
+    token: str
+    def __init__(self, projects: _Optional[_Iterable[_Union[Project, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
+
 class ProjectListRequest(_message.Message):
-    __slots__ = ["filters", "limit", "sort_by", "token"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["limit", "token", "filters", "sort_by"]
     LIMIT_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
-    filters: str
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
     limit: int
-    sort_by: _common_pb2.Sort
     token: str
+    filters: str
+    sort_by: _common_pb2.Sort
     def __init__(self, limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
 
 class ProjectRegisterRequest(_message.Message):
     __slots__ = ["project"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     project: Project
     def __init__(self, project: _Optional[_Union[Project, _Mapping]] = ...) -> None: ...
@@ -57,15 +68,7 @@
 class ProjectRegisterResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class ProjectUpdateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
-
-class Projects(_message.Message):
-    __slots__ = ["projects", "token"]
-    PROJECTS_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    projects: _containers.RepeatedCompositeFieldContainer[Project]
-    token: str
-    def __init__(self, projects: _Optional[_Iterable[_Union[Project, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/schedule_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/schedule_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/admin/schedule.proto\x12\x0e\x66lyteidl.admin\"T\n\tFixedRate\x12\x14\n\x05value\x18\x01 \x01(\rR\x05value\x12\x31\n\x04unit\x18\x02 \x01(\x0e\x32\x1d.flyteidl.admin.FixedRateUnitR\x04unit\"B\n\x0c\x43ronSchedule\x12\x1a\n\x08schedule\x18\x01 \x01(\tR\x08schedule\x12\x16\n\x06offset\x18\x02 \x01(\tR\x06offset\"\xfa\x01\n\x08Schedule\x12-\n\x0f\x63ron_expression\x18\x01 \x01(\tB\x02\x18\x01H\x00R\x0e\x63ronExpression\x12/\n\x04rate\x18\x02 \x01(\x0b\x32\x19.flyteidl.admin.FixedRateH\x00R\x04rate\x12\x43\n\rcron_schedule\x18\x04 \x01(\x0b\x32\x1c.flyteidl.admin.CronScheduleH\x00R\x0c\x63ronSchedule\x12\x33\n\x16kickoff_time_input_arg\x18\x03 \x01(\tR\x13kickoffTimeInputArgB\x14\n\x12ScheduleExpression*.\n\rFixedRateUnit\x12\n\n\x06MINUTE\x10\x00\x12\x08\n\x04HOUR\x10\x01\x12\x07\n\x03\x44\x41Y\x10\x02\x42\xb3\x01\n\x12\x63om.flyteidl.adminB\rScheduleProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.schedule_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.schedule_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\rScheduleProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
   _SCHEDULE.fields_by_name['cron_expression']._options = None
   _SCHEDULE.fields_by_name['cron_expression']._serialized_options = b'\030\001'
-  _FIXEDRATEUNIT._serialized_start=456
-  _FIXEDRATEUNIT._serialized_end=502
-  _FIXEDRATE._serialized_start=49
-  _FIXEDRATE._serialized_end=133
-  _CRONSCHEDULE._serialized_start=135
-  _CRONSCHEDULE._serialized_end=201
-  _SCHEDULE._serialized_start=204
-  _SCHEDULE._serialized_end=454
+  _globals['_FIXEDRATEUNIT']._serialized_start=456
+  _globals['_FIXEDRATEUNIT']._serialized_end=502
+  _globals['_FIXEDRATE']._serialized_start=49
+  _globals['_FIXEDRATE']._serialized_end=133
+  _globals['_CRONSCHEDULE']._serialized_start=135
+  _globals['_CRONSCHEDULE']._serialized_end=201
+  _globals['_SCHEDULE']._serialized_start=204
+  _globals['_SCHEDULE']._serialized_end=454
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/schedule_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/schedule_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-DAY: FixedRateUnit
 DESCRIPTOR: _descriptor.FileDescriptor
-HOUR: FixedRateUnit
-MINUTE: FixedRateUnit
 
-class CronSchedule(_message.Message):
-    __slots__ = ["offset", "schedule"]
-    OFFSET_FIELD_NUMBER: _ClassVar[int]
-    SCHEDULE_FIELD_NUMBER: _ClassVar[int]
-    offset: str
-    schedule: str
-    def __init__(self, schedule: _Optional[str] = ..., offset: _Optional[str] = ...) -> None: ...
+class FixedRateUnit(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    MINUTE: _ClassVar[FixedRateUnit]
+    HOUR: _ClassVar[FixedRateUnit]
+    DAY: _ClassVar[FixedRateUnit]
+MINUTE: FixedRateUnit
+HOUR: FixedRateUnit
+DAY: FixedRateUnit
 
 class FixedRate(_message.Message):
-    __slots__ = ["unit", "value"]
-    UNIT_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["value", "unit"]
     VALUE_FIELD_NUMBER: _ClassVar[int]
-    unit: FixedRateUnit
+    UNIT_FIELD_NUMBER: _ClassVar[int]
     value: int
+    unit: FixedRateUnit
     def __init__(self, value: _Optional[int] = ..., unit: _Optional[_Union[FixedRateUnit, str]] = ...) -> None: ...
 
+class CronSchedule(_message.Message):
+    __slots__ = ["schedule", "offset"]
+    SCHEDULE_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_FIELD_NUMBER: _ClassVar[int]
+    schedule: str
+    offset: str
+    def __init__(self, schedule: _Optional[str] = ..., offset: _Optional[str] = ...) -> None: ...
+
 class Schedule(_message.Message):
-    __slots__ = ["cron_expression", "cron_schedule", "kickoff_time_input_arg", "rate"]
+    __slots__ = ["cron_expression", "rate", "cron_schedule", "kickoff_time_input_arg"]
     CRON_EXPRESSION_FIELD_NUMBER: _ClassVar[int]
+    RATE_FIELD_NUMBER: _ClassVar[int]
     CRON_SCHEDULE_FIELD_NUMBER: _ClassVar[int]
     KICKOFF_TIME_INPUT_ARG_FIELD_NUMBER: _ClassVar[int]
-    RATE_FIELD_NUMBER: _ClassVar[int]
     cron_expression: str
+    rate: FixedRate
     cron_schedule: CronSchedule
     kickoff_time_input_arg: str
-    rate: FixedRate
     def __init__(self, cron_expression: _Optional[str] = ..., rate: _Optional[_Union[FixedRate, _Mapping]] = ..., cron_schedule: _Optional[_Union[CronSchedule, _Mapping]] = ..., kickoff_time_input_arg: _Optional[str] = ...) -> None: ...
-
-class FixedRateUnit(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/signal_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/signal_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 from flyteidl.core import types_pb2 as flyteidl_dot_core_dot_types__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/admin/signal.proto\x12\x0e\x66lyteidl.admin\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x19\x66lyteidl/core/types.proto\"{\n\x18SignalGetOrCreateRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.SignalIdentifierR\x02id\x12.\n\x04type\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\x04type\"\xe8\x01\n\x11SignalListRequest\x12^\n\x15workflow_execution_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x13workflowExecutionId\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\"T\n\nSignalList\x12\x30\n\x07signals\x18\x01 \x03(\x0b\x32\x16.flyteidl.admin.SignalR\x07signals\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"q\n\x10SignalSetRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.SignalIdentifierR\x02id\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.flyteidl.core.LiteralR\x05value\"\x13\n\x11SignalSetResponse\"\x97\x01\n\x06Signal\x12/\n\x02id\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.SignalIdentifierR\x02id\x12.\n\x04type\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\x04type\x12,\n\x05value\x18\x03 \x01(\x0b\x32\x16.flyteidl.core.LiteralR\x05valueB\xb1\x01\n\x12\x63om.flyteidl.adminB\x0bSignalProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.signal_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.signal_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\013SignalProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _SIGNALGETORCREATEREQUEST._serialized_start=165
-  _SIGNALGETORCREATEREQUEST._serialized_end=288
-  _SIGNALLISTREQUEST._serialized_start=291
-  _SIGNALLISTREQUEST._serialized_end=523
-  _SIGNALLIST._serialized_start=525
-  _SIGNALLIST._serialized_end=609
-  _SIGNALSETREQUEST._serialized_start=611
-  _SIGNALSETREQUEST._serialized_end=724
-  _SIGNALSETRESPONSE._serialized_start=726
-  _SIGNALSETRESPONSE._serialized_end=745
-  _SIGNAL._serialized_start=748
-  _SIGNAL._serialized_end=899
+  _globals['_SIGNALGETORCREATEREQUEST']._serialized_start=165
+  _globals['_SIGNALGETORCREATEREQUEST']._serialized_end=288
+  _globals['_SIGNALLISTREQUEST']._serialized_start=291
+  _globals['_SIGNALLISTREQUEST']._serialized_end=523
+  _globals['_SIGNALLIST']._serialized_start=525
+  _globals['_SIGNALLIST']._serialized_end=609
+  _globals['_SIGNALSETREQUEST']._serialized_start=611
+  _globals['_SIGNALSETREQUEST']._serialized_end=724
+  _globals['_SIGNALSETRESPONSE']._serialized_start=726
+  _globals['_SIGNALSETRESPONSE']._serialized_end=745
+  _globals['_SIGNAL']._serialized_start=748
+  _globals['_SIGNAL']._serialized_end=899
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/signal_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/signal_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -5,58 +5,58 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Signal(_message.Message):
-    __slots__ = ["id", "type", "value"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.SignalIdentifier
-    type: _types_pb2.LiteralType
-    value: _literals_pb2.Literal
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.SignalIdentifier, _Mapping]] = ..., type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ..., value: _Optional[_Union[_literals_pb2.Literal, _Mapping]] = ...) -> None: ...
-
 class SignalGetOrCreateRequest(_message.Message):
     __slots__ = ["id", "type"]
     ID_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.SignalIdentifier
     type: _types_pb2.LiteralType
     def __init__(self, id: _Optional[_Union[_identifier_pb2.SignalIdentifier, _Mapping]] = ..., type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ...) -> None: ...
 
+class SignalListRequest(_message.Message):
+    __slots__ = ["workflow_execution_id", "limit", "token", "filters", "sort_by"]
+    WORKFLOW_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    workflow_execution_id: _identifier_pb2.WorkflowExecutionIdentifier
+    limit: int
+    token: str
+    filters: str
+    sort_by: _common_pb2.Sort
+    def __init__(self, workflow_execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
+
 class SignalList(_message.Message):
     __slots__ = ["signals", "token"]
     SIGNALS_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     signals: _containers.RepeatedCompositeFieldContainer[Signal]
     token: str
     def __init__(self, signals: _Optional[_Iterable[_Union[Signal, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
 
-class SignalListRequest(_message.Message):
-    __slots__ = ["filters", "limit", "sort_by", "token", "workflow_execution_id"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    filters: str
-    limit: int
-    sort_by: _common_pb2.Sort
-    token: str
-    workflow_execution_id: _identifier_pb2.WorkflowExecutionIdentifier
-    def __init__(self, workflow_execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
-
 class SignalSetRequest(_message.Message):
     __slots__ = ["id", "value"]
     ID_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.SignalIdentifier
     value: _literals_pb2.Literal
     def __init__(self, id: _Optional[_Union[_identifier_pb2.SignalIdentifier, _Mapping]] = ..., value: _Optional[_Union[_literals_pb2.Literal, _Mapping]] = ...) -> None: ...
 
 class SignalSetResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
+
+class Signal(_message.Message):
+    __slots__ = ["id", "type", "value"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.SignalIdentifier
+    type: _types_pb2.LiteralType
+    value: _literals_pb2.Literal
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.SignalIdentifier, _Mapping]] = ..., type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ..., value: _Optional[_Union[_literals_pb2.Literal, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_execution_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_execution_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,38 +17,41 @@
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 from flyteidl.event import event_pb2 as flyteidl_dot_event_dot_event__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#flyteidl/admin/task_execution.proto\x12\x0e\x66lyteidl.admin\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1a\x66lyteidl/event/event.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"Q\n\x17TaskExecutionGetRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\"\xe3\x01\n\x18TaskExecutionListRequest\x12R\n\x11node_execution_id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x0fnodeExecutionId\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\"\xc1\x01\n\rTaskExecution\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\x12\x1b\n\tinput_uri\x18\x02 \x01(\tR\x08inputUri\x12>\n\x07\x63losure\x18\x03 \x01(\x0b\x32$.flyteidl.admin.TaskExecutionClosureR\x07\x63losure\x12\x1b\n\tis_parent\x18\x04 \x01(\x08R\x08isParent\"q\n\x11TaskExecutionList\x12\x46\n\x0ftask_executions\x18\x01 \x03(\x0b\x32\x1d.flyteidl.admin.TaskExecutionR\x0etaskExecutions\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\xea\x05\n\x14TaskExecutionClosure\x12#\n\noutput_uri\x18\x01 \x01(\tB\x02\x18\x01H\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12@\n\x0boutput_data\x18\x0c \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\noutputData\x12\x38\n\x05phase\x18\x03 \x01(\x0e\x32\".flyteidl.core.TaskExecution.PhaseR\x05phase\x12*\n\x04logs\x18\x04 \x03(\x0b\x32\x16.flyteidl.core.TaskLogR\x04logs\x12\x39\n\nstarted_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartedAt\x12\x35\n\x08\x64uration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08\x64uration\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x38\n\x0b\x63ustom_info\x18\t \x01(\x0b\x32\x17.google.protobuf.StructR\ncustomInfo\x12\x16\n\x06reason\x18\n \x01(\tR\x06reason\x12\x1b\n\ttask_type\x18\x0b \x01(\tR\x08taskType\x12\x41\n\x08metadata\x18\x10 \x01(\x0b\x32%.flyteidl.event.TaskExecutionMetadataR\x08metadata\x12#\n\revent_version\x18\x11 \x01(\x05R\x0c\x65ventVersionB\x0f\n\routput_result\"U\n\x1bTaskExecutionGetDataRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\"\x84\x02\n\x1cTaskExecutionGetDataResponse\x12\x33\n\x06inputs\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x06inputs\x12\x35\n\x07outputs\x18\x02 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x07outputs\x12:\n\x0b\x66ull_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\nfullInputs\x12<\n\x0c\x66ull_outputs\x18\x04 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x0b\x66ullOutputsB\xb8\x01\n\x12\x63om.flyteidl.adminB\x12TaskExecutionProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#flyteidl/admin/task_execution.proto\x12\x0e\x66lyteidl.admin\x1a\x1b\x66lyteidl/admin/common.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1a\x66lyteidl/event/event.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"Q\n\x17TaskExecutionGetRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\"\xe3\x01\n\x18TaskExecutionListRequest\x12R\n\x11node_execution_id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x0fnodeExecutionId\x12\x14\n\x05limit\x18\x02 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x03 \x01(\tR\x05token\x12\x18\n\x07\x66ilters\x18\x04 \x01(\tR\x07\x66ilters\x12-\n\x07sort_by\x18\x05 \x01(\x0b\x32\x14.flyteidl.admin.SortR\x06sortBy\"\xc1\x01\n\rTaskExecution\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\x12\x1b\n\tinput_uri\x18\x02 \x01(\tR\x08inputUri\x12>\n\x07\x63losure\x18\x03 \x01(\x0b\x32$.flyteidl.admin.TaskExecutionClosureR\x07\x63losure\x12\x1b\n\tis_parent\x18\x04 \x01(\x08R\x08isParent\"q\n\x11TaskExecutionList\x12\x46\n\x0ftask_executions\x18\x01 \x03(\x0b\x32\x1d.flyteidl.admin.TaskExecutionR\x0etaskExecutions\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x9c\x06\n\x14TaskExecutionClosure\x12#\n\noutput_uri\x18\x01 \x01(\tB\x02\x18\x01H\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12@\n\x0boutput_data\x18\x0c \x01(\x0b\x32\x19.flyteidl.core.LiteralMapB\x02\x18\x01H\x00R\noutputData\x12\x38\n\x05phase\x18\x03 \x01(\x0e\x32\".flyteidl.core.TaskExecution.PhaseR\x05phase\x12*\n\x04logs\x18\x04 \x03(\x0b\x32\x16.flyteidl.core.TaskLogR\x04logs\x12\x39\n\nstarted_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartedAt\x12\x35\n\x08\x64uration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08\x64uration\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nupdated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x38\n\x0b\x63ustom_info\x18\t \x01(\x0b\x32\x17.google.protobuf.StructR\ncustomInfo\x12\x16\n\x06reason\x18\n \x01(\tR\x06reason\x12\x1b\n\ttask_type\x18\x0b \x01(\tR\x08taskType\x12\x41\n\x08metadata\x18\x10 \x01(\x0b\x32%.flyteidl.event.TaskExecutionMetadataR\x08metadata\x12#\n\revent_version\x18\x11 \x01(\x05R\x0c\x65ventVersion\x12\x30\n\x07reasons\x18\x12 \x03(\x0b\x32\x16.flyteidl.admin.ReasonR\x07reasonsB\x0f\n\routput_result\"_\n\x06Reason\x12;\n\x0boccurred_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"U\n\x1bTaskExecutionGetDataRequest\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\"\xbe\x02\n\x1cTaskExecutionGetDataResponse\x12\x33\n\x06inputs\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x06inputs\x12\x35\n\x07outputs\x18\x02 \x01(\x0b\x32\x17.flyteidl.admin.UrlBlobB\x02\x18\x01R\x07outputs\x12:\n\x0b\x66ull_inputs\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\nfullInputs\x12<\n\x0c\x66ull_outputs\x18\x04 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapR\x0b\x66ullOutputs\x12\x38\n\nflyte_urls\x18\x05 \x01(\x0b\x32\x19.flyteidl.admin.FlyteURLsR\tflyteUrlsB\xb8\x01\n\x12\x63om.flyteidl.adminB\x12TaskExecutionProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.task_execution_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.task_execution_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\022TaskExecutionProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
   _TASKEXECUTIONCLOSURE.fields_by_name['output_uri']._options = None
   _TASKEXECUTIONCLOSURE.fields_by_name['output_uri']._serialized_options = b'\030\001'
   _TASKEXECUTIONCLOSURE.fields_by_name['output_data']._options = None
   _TASKEXECUTIONCLOSURE.fields_by_name['output_data']._serialized_options = b'\030\001'
   _TASKEXECUTIONGETDATARESPONSE.fields_by_name['inputs']._options = None
   _TASKEXECUTIONGETDATARESPONSE.fields_by_name['inputs']._serialized_options = b'\030\001'
   _TASKEXECUTIONGETDATARESPONSE.fields_by_name['outputs']._options = None
   _TASKEXECUTIONGETDATARESPONSE.fields_by_name['outputs']._serialized_options = b'\030\001'
-  _TASKEXECUTIONGETREQUEST._serialized_start=300
-  _TASKEXECUTIONGETREQUEST._serialized_end=381
-  _TASKEXECUTIONLISTREQUEST._serialized_start=384
-  _TASKEXECUTIONLISTREQUEST._serialized_end=611
-  _TASKEXECUTION._serialized_start=614
-  _TASKEXECUTION._serialized_end=807
-  _TASKEXECUTIONLIST._serialized_start=809
-  _TASKEXECUTIONLIST._serialized_end=922
-  _TASKEXECUTIONCLOSURE._serialized_start=925
-  _TASKEXECUTIONCLOSURE._serialized_end=1671
-  _TASKEXECUTIONGETDATAREQUEST._serialized_start=1673
-  _TASKEXECUTIONGETDATAREQUEST._serialized_end=1758
-  _TASKEXECUTIONGETDATARESPONSE._serialized_start=1761
-  _TASKEXECUTIONGETDATARESPONSE._serialized_end=2021
+  _globals['_TASKEXECUTIONGETREQUEST']._serialized_start=300
+  _globals['_TASKEXECUTIONGETREQUEST']._serialized_end=381
+  _globals['_TASKEXECUTIONLISTREQUEST']._serialized_start=384
+  _globals['_TASKEXECUTIONLISTREQUEST']._serialized_end=611
+  _globals['_TASKEXECUTION']._serialized_start=614
+  _globals['_TASKEXECUTION']._serialized_end=807
+  _globals['_TASKEXECUTIONLIST']._serialized_start=809
+  _globals['_TASKEXECUTIONLIST']._serialized_end=922
+  _globals['_TASKEXECUTIONCLOSURE']._serialized_start=925
+  _globals['_TASKEXECUTIONCLOSURE']._serialized_end=1721
+  _globals['_REASON']._serialized_start=1723
+  _globals['_REASON']._serialized_end=1818
+  _globals['_TASKEXECUTIONGETDATAREQUEST']._serialized_start=1820
+  _globals['_TASKEXECUTIONGETDATAREQUEST']._serialized_end=1905
+  _globals['_TASKEXECUTIONGETDATARESPONSE']._serialized_start=1908
+  _globals['_TASKEXECUTIONGETDATARESPONSE']._serialized_end=2226
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_execution_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_execution_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -9,96 +9,108 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class TaskExecutionGetRequest(_message.Message):
+    __slots__ = ["id"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.TaskExecutionIdentifier
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ...) -> None: ...
+
+class TaskExecutionListRequest(_message.Message):
+    __slots__ = ["node_execution_id", "limit", "token", "filters", "sort_by"]
+    NODE_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    node_execution_id: _identifier_pb2.NodeExecutionIdentifier
+    limit: int
+    token: str
+    filters: str
+    sort_by: _common_pb2.Sort
+    def __init__(self, node_execution_id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
+
 class TaskExecution(_message.Message):
-    __slots__ = ["closure", "id", "input_uri", "is_parent"]
-    CLOSURE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "input_uri", "closure", "is_parent"]
     ID_FIELD_NUMBER: _ClassVar[int]
     INPUT_URI_FIELD_NUMBER: _ClassVar[int]
+    CLOSURE_FIELD_NUMBER: _ClassVar[int]
     IS_PARENT_FIELD_NUMBER: _ClassVar[int]
-    closure: TaskExecutionClosure
     id: _identifier_pb2.TaskExecutionIdentifier
     input_uri: str
+    closure: TaskExecutionClosure
     is_parent: bool
     def __init__(self, id: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ..., input_uri: _Optional[str] = ..., closure: _Optional[_Union[TaskExecutionClosure, _Mapping]] = ..., is_parent: bool = ...) -> None: ...
 
+class TaskExecutionList(_message.Message):
+    __slots__ = ["task_executions", "token"]
+    TASK_EXECUTIONS_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    task_executions: _containers.RepeatedCompositeFieldContainer[TaskExecution]
+    token: str
+    def __init__(self, task_executions: _Optional[_Iterable[_Union[TaskExecution, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
+
 class TaskExecutionClosure(_message.Message):
-    __slots__ = ["created_at", "custom_info", "duration", "error", "event_version", "logs", "metadata", "output_data", "output_uri", "phase", "reason", "started_at", "task_type", "updated_at"]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    CUSTOM_INFO_FIELD_NUMBER: _ClassVar[int]
-    DURATION_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["output_uri", "error", "output_data", "phase", "logs", "started_at", "duration", "created_at", "updated_at", "custom_info", "reason", "task_type", "metadata", "event_version", "reasons"]
+    OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
-    EVENT_VERSION_FIELD_NUMBER: _ClassVar[int]
-    LOGS_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
     PHASE_FIELD_NUMBER: _ClassVar[int]
-    REASON_FIELD_NUMBER: _ClassVar[int]
+    LOGS_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
-    TASK_TYPE_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
-    created_at: _timestamp_pb2.Timestamp
-    custom_info: _struct_pb2.Struct
-    duration: _duration_pb2.Duration
+    CUSTOM_INFO_FIELD_NUMBER: _ClassVar[int]
+    REASON_FIELD_NUMBER: _ClassVar[int]
+    TASK_TYPE_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    EVENT_VERSION_FIELD_NUMBER: _ClassVar[int]
+    REASONS_FIELD_NUMBER: _ClassVar[int]
+    output_uri: str
     error: _execution_pb2.ExecutionError
-    event_version: int
-    logs: _containers.RepeatedCompositeFieldContainer[_execution_pb2.TaskLog]
-    metadata: _event_pb2.TaskExecutionMetadata
     output_data: _literals_pb2.LiteralMap
-    output_uri: str
     phase: _execution_pb2.TaskExecution.Phase
-    reason: str
+    logs: _containers.RepeatedCompositeFieldContainer[_execution_pb2.TaskLog]
     started_at: _timestamp_pb2.Timestamp
-    task_type: str
+    duration: _duration_pb2.Duration
+    created_at: _timestamp_pb2.Timestamp
     updated_at: _timestamp_pb2.Timestamp
-    def __init__(self, output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., phase: _Optional[_Union[_execution_pb2.TaskExecution.Phase, str]] = ..., logs: _Optional[_Iterable[_Union[_execution_pb2.TaskLog, _Mapping]]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., custom_info: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., reason: _Optional[str] = ..., task_type: _Optional[str] = ..., metadata: _Optional[_Union[_event_pb2.TaskExecutionMetadata, _Mapping]] = ..., event_version: _Optional[int] = ...) -> None: ...
+    custom_info: _struct_pb2.Struct
+    reason: str
+    task_type: str
+    metadata: _event_pb2.TaskExecutionMetadata
+    event_version: int
+    reasons: _containers.RepeatedCompositeFieldContainer[Reason]
+    def __init__(self, output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., phase: _Optional[_Union[_execution_pb2.TaskExecution.Phase, str]] = ..., logs: _Optional[_Iterable[_Union[_execution_pb2.TaskLog, _Mapping]]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., custom_info: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., reason: _Optional[str] = ..., task_type: _Optional[str] = ..., metadata: _Optional[_Union[_event_pb2.TaskExecutionMetadata, _Mapping]] = ..., event_version: _Optional[int] = ..., reasons: _Optional[_Iterable[_Union[Reason, _Mapping]]] = ...) -> None: ...
+
+class Reason(_message.Message):
+    __slots__ = ["occurred_at", "message"]
+    OCCURRED_AT_FIELD_NUMBER: _ClassVar[int]
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    occurred_at: _timestamp_pb2.Timestamp
+    message: str
+    def __init__(self, occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., message: _Optional[str] = ...) -> None: ...
 
 class TaskExecutionGetDataRequest(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.TaskExecutionIdentifier
     def __init__(self, id: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
 class TaskExecutionGetDataResponse(_message.Message):
-    __slots__ = ["full_inputs", "full_outputs", "inputs", "outputs"]
-    FULL_INPUTS_FIELD_NUMBER: _ClassVar[int]
-    FULL_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["inputs", "outputs", "full_inputs", "full_outputs", "flyte_urls"]
     INPUTS_FIELD_NUMBER: _ClassVar[int]
     OUTPUTS_FIELD_NUMBER: _ClassVar[int]
-    full_inputs: _literals_pb2.LiteralMap
-    full_outputs: _literals_pb2.LiteralMap
+    FULL_INPUTS_FIELD_NUMBER: _ClassVar[int]
+    FULL_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
+    FLYTE_URLS_FIELD_NUMBER: _ClassVar[int]
     inputs: _common_pb2.UrlBlob
     outputs: _common_pb2.UrlBlob
-    def __init__(self, inputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., outputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., full_inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., full_outputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ...) -> None: ...
-
-class TaskExecutionGetRequest(_message.Message):
-    __slots__ = ["id"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.TaskExecutionIdentifier
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ...) -> None: ...
-
-class TaskExecutionList(_message.Message):
-    __slots__ = ["task_executions", "token"]
-    TASK_EXECUTIONS_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    task_executions: _containers.RepeatedCompositeFieldContainer[TaskExecution]
-    token: str
-    def __init__(self, task_executions: _Optional[_Iterable[_Union[TaskExecution, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
-
-class TaskExecutionListRequest(_message.Message):
-    __slots__ = ["filters", "limit", "node_execution_id", "sort_by", "token"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    NODE_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    SORT_BY_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    filters: str
-    limit: int
-    node_execution_id: _identifier_pb2.NodeExecutionIdentifier
-    sort_by: _common_pb2.Sort
-    token: str
-    def __init__(self, node_execution_id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., limit: _Optional[int] = ..., token: _Optional[str] = ..., filters: _Optional[str] = ..., sort_by: _Optional[_Union[_common_pb2.Sort, _Mapping]] = ...) -> None: ...
+    full_inputs: _literals_pb2.LiteralMap
+    full_outputs: _literals_pb2.LiteralMap
+    flyte_urls: _common_pb2.FlyteURLs
+    def __init__(self, inputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., outputs: _Optional[_Union[_common_pb2.UrlBlob, _Mapping]] = ..., full_inputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., full_outputs: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., flyte_urls: _Optional[_Union[_common_pb2.FlyteURLs, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 from flyteidl.core import compiler_pb2 as flyteidl_dot_core_dot_compiler__pb2
 from flyteidl.admin import description_entity_pb2 as flyteidl_dot_admin_dot_description__entity__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66lyteidl/admin/task.proto\x12\x0e\x66lyteidl.admin\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x19\x66lyteidl/core/tasks.proto\x1a\x1c\x66lyteidl/core/compiler.proto\x1a\'flyteidl/admin/description_entity.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"l\n\x11TaskCreateRequest\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12,\n\x04spec\x18\x02 \x01(\x0b\x32\x18.flyteidl.admin.TaskSpecR\x04spec\"\x14\n\x12TaskCreateResponse\"\x95\x01\n\x04Task\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12\x35\n\x07\x63losure\x18\x02 \x01(\x0b\x32\x1b.flyteidl.admin.TaskClosureR\x07\x63losure\x12+\n\x11short_description\x18\x03 \x01(\tR\x10shortDescription\"L\n\x08TaskList\x12*\n\x05tasks\x18\x01 \x03(\x0b\x32\x14.flyteidl.admin.TaskR\x05tasks\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x88\x01\n\x08TaskSpec\x12\x37\n\x08template\x18\x01 \x01(\x0b\x32\x1b.flyteidl.core.TaskTemplateR\x08template\x12\x43\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32!.flyteidl.admin.DescriptionEntityR\x0b\x64\x65scription\"\x8a\x01\n\x0bTaskClosure\x12@\n\rcompiled_task\x18\x01 \x01(\x0b\x32\x1b.flyteidl.core.CompiledTaskR\x0c\x63ompiledTask\x12\x39\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAtB\xaf\x01\n\x12\x63om.flyteidl.adminB\tTaskProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.task_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.task_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\tTaskProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _TASKCREATEREQUEST._serialized_start=208
-  _TASKCREATEREQUEST._serialized_end=316
-  _TASKCREATERESPONSE._serialized_start=318
-  _TASKCREATERESPONSE._serialized_end=338
-  _TASK._serialized_start=341
-  _TASK._serialized_end=490
-  _TASKLIST._serialized_start=492
-  _TASKLIST._serialized_end=568
-  _TASKSPEC._serialized_start=571
-  _TASKSPEC._serialized_end=707
-  _TASKCLOSURE._serialized_start=710
-  _TASKCLOSURE._serialized_end=848
+  _globals['_TASKCREATEREQUEST']._serialized_start=208
+  _globals['_TASKCREATEREQUEST']._serialized_end=316
+  _globals['_TASKCREATERESPONSE']._serialized_start=318
+  _globals['_TASKCREATERESPONSE']._serialized_end=338
+  _globals['_TASK']._serialized_start=341
+  _globals['_TASK']._serialized_end=490
+  _globals['_TASKLIST']._serialized_start=492
+  _globals['_TASKLIST']._serialized_end=568
+  _globals['_TASKSPEC']._serialized_start=571
+  _globals['_TASKSPEC']._serialized_end=707
+  _globals['_TASKCLOSURE']._serialized_start=710
+  _globals['_TASKCLOSURE']._serialized_end=848
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/task_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/task_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -6,52 +6,52 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Task(_message.Message):
-    __slots__ = ["closure", "id", "short_description"]
-    CLOSURE_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    SHORT_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    closure: TaskClosure
-    id: _identifier_pb2.Identifier
-    short_description: str
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., closure: _Optional[_Union[TaskClosure, _Mapping]] = ..., short_description: _Optional[str] = ...) -> None: ...
-
-class TaskClosure(_message.Message):
-    __slots__ = ["compiled_task", "created_at"]
-    COMPILED_TASK_FIELD_NUMBER: _ClassVar[int]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    compiled_task: _compiler_pb2.CompiledTask
-    created_at: _timestamp_pb2.Timestamp
-    def __init__(self, compiled_task: _Optional[_Union[_compiler_pb2.CompiledTask, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
-
 class TaskCreateRequest(_message.Message):
     __slots__ = ["id", "spec"]
     ID_FIELD_NUMBER: _ClassVar[int]
     SPEC_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
     spec: TaskSpec
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., spec: _Optional[_Union[TaskSpec, _Mapping]] = ...) -> None: ...
 
 class TaskCreateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
+class Task(_message.Message):
+    __slots__ = ["id", "closure", "short_description"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    CLOSURE_FIELD_NUMBER: _ClassVar[int]
+    SHORT_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.Identifier
+    closure: TaskClosure
+    short_description: str
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., closure: _Optional[_Union[TaskClosure, _Mapping]] = ..., short_description: _Optional[str] = ...) -> None: ...
+
 class TaskList(_message.Message):
     __slots__ = ["tasks", "token"]
     TASKS_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     tasks: _containers.RepeatedCompositeFieldContainer[Task]
     token: str
     def __init__(self, tasks: _Optional[_Iterable[_Union[Task, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
 
 class TaskSpec(_message.Message):
-    __slots__ = ["description", "template"]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["template", "description"]
     TEMPLATE_FIELD_NUMBER: _ClassVar[int]
-    description: _description_entity_pb2.DescriptionEntity
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     template: _tasks_pb2.TaskTemplate
+    description: _description_entity_pb2.DescriptionEntity
     def __init__(self, template: _Optional[_Union[_tasks_pb2.TaskTemplate, _Mapping]] = ..., description: _Optional[_Union[_description_entity_pb2.DescriptionEntity, _Mapping]] = ...) -> None: ...
+
+class TaskClosure(_message.Message):
+    __slots__ = ["compiled_task", "created_at"]
+    COMPILED_TASK_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    compiled_task: _compiler_pb2.CompiledTask
+    created_at: _timestamp_pb2.Timestamp
+    def __init__(self, compiled_task: _Optional[_Union[_compiler_pb2.CompiledTask, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/version_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/version_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/admin/version.proto\x12\x0e\x66lyteidl.admin\"a\n\x12GetVersionResponse\x12K\n\x15\x63ontrol_plane_version\x18\x01 \x01(\x0b\x32\x17.flyteidl.admin.VersionR\x13\x63ontrolPlaneVersion\"W\n\x07Version\x12\x14\n\x05\x42uild\x18\x01 \x01(\tR\x05\x42uild\x12\x18\n\x07Version\x18\x02 \x01(\tR\x07Version\x12\x1c\n\tBuildTime\x18\x03 \x01(\tR\tBuildTime\"\x13\n\x11GetVersionRequestB\xb2\x01\n\x12\x63om.flyteidl.adminB\x0cVersionProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.version_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.version_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\014VersionProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _GETVERSIONRESPONSE._serialized_start=48
-  _GETVERSIONRESPONSE._serialized_end=145
-  _VERSION._serialized_start=147
-  _VERSION._serialized_end=234
-  _GETVERSIONREQUEST._serialized_start=236
-  _GETVERSIONREQUEST._serialized_end=255
+  _globals['_GETVERSIONRESPONSE']._serialized_start=48
+  _globals['_GETVERSIONRESPONSE']._serialized_end=145
+  _globals['_VERSION']._serialized_start=147
+  _globals['_VERSION']._serialized_end=234
+  _globals['_GETVERSIONREQUEST']._serialized_start=236
+  _globals['_GETVERSIONREQUEST']._serialized_end=255
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/version_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/version_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class GetVersionRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
 class GetVersionResponse(_message.Message):
     __slots__ = ["control_plane_version"]
     CONTROL_PLANE_VERSION_FIELD_NUMBER: _ClassVar[int]
     control_plane_version: Version
     def __init__(self, control_plane_version: _Optional[_Union[Version, _Mapping]] = ...) -> None: ...
 
 class Version(_message.Message):
-    __slots__ = ["Build", "BuildTime", "Version"]
-    BUILDTIME_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["Build", "Version", "BuildTime"]
     BUILD_FIELD_NUMBER: _ClassVar[int]
-    Build: str
-    BuildTime: str
     VERSION_FIELD_NUMBER: _ClassVar[int]
+    BUILDTIME_FIELD_NUMBER: _ClassVar[int]
+    Build: str
     Version: str
+    BuildTime: str
     def __init__(self, Build: _Optional[str] = ..., Version: _Optional[str] = ..., BuildTime: _Optional[str] = ...) -> None: ...
+
+class GetVersionRequest(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 
 
 from flyteidl.admin import matchable_resource_pb2 as flyteidl_dot_admin_dot_matchable__resource__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(flyteidl/admin/workflow_attributes.proto\x12\x0e\x66lyteidl.admin\x1a\'flyteidl/admin/matchable_resource.proto\"\xb7\x01\n\x12WorkflowAttributes\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x1a\n\x08workflow\x18\x03 \x01(\tR\x08workflow\x12S\n\x13matching_attributes\x18\x04 \x01(\x0b\x32\".flyteidl.admin.MatchingAttributesR\x12matchingAttributes\"e\n\x1fWorkflowAttributesUpdateRequest\x12\x42\n\nattributes\x18\x01 \x01(\x0b\x32\".flyteidl.admin.WorkflowAttributesR\nattributes\"\"\n WorkflowAttributesUpdateResponse\"\xb4\x01\n\x1cWorkflowAttributesGetRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x1a\n\x08workflow\x18\x03 \x01(\tR\x08workflow\x12\x46\n\rresource_type\x18\x04 \x01(\x0e\x32!.flyteidl.admin.MatchableResourceR\x0cresourceType\"c\n\x1dWorkflowAttributesGetResponse\x12\x42\n\nattributes\x18\x01 \x01(\x0b\x32\".flyteidl.admin.WorkflowAttributesR\nattributes\"\xb7\x01\n\x1fWorkflowAttributesDeleteRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x1a\n\x08workflow\x18\x03 \x01(\tR\x08workflow\x12\x46\n\rresource_type\x18\x04 \x01(\x0e\x32!.flyteidl.admin.MatchableResourceR\x0cresourceType\"\"\n WorkflowAttributesDeleteResponseB\xbd\x01\n\x12\x63om.flyteidl.adminB\x17WorkflowAttributesProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\xa2\x02\x03\x46\x41X\xaa\x02\x0e\x46lyteidl.Admin\xca\x02\x0e\x46lyteidl\\Admin\xe2\x02\x1a\x46lyteidl\\Admin\\GPBMetadata\xea\x02\x0f\x46lyteidl::Adminb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.workflow_attributes_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.admin.workflow_attributes_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.adminB\027WorkflowAttributesProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/admin\242\002\003FAX\252\002\016Flyteidl.Admin\312\002\016Flyteidl\\Admin\342\002\032Flyteidl\\Admin\\GPBMetadata\352\002\017Flyteidl::Admin'
-  _WORKFLOWATTRIBUTES._serialized_start=102
-  _WORKFLOWATTRIBUTES._serialized_end=285
-  _WORKFLOWATTRIBUTESUPDATEREQUEST._serialized_start=287
-  _WORKFLOWATTRIBUTESUPDATEREQUEST._serialized_end=388
-  _WORKFLOWATTRIBUTESUPDATERESPONSE._serialized_start=390
-  _WORKFLOWATTRIBUTESUPDATERESPONSE._serialized_end=424
-  _WORKFLOWATTRIBUTESGETREQUEST._serialized_start=427
-  _WORKFLOWATTRIBUTESGETREQUEST._serialized_end=607
-  _WORKFLOWATTRIBUTESGETRESPONSE._serialized_start=609
-  _WORKFLOWATTRIBUTESGETRESPONSE._serialized_end=708
-  _WORKFLOWATTRIBUTESDELETEREQUEST._serialized_start=711
-  _WORKFLOWATTRIBUTESDELETEREQUEST._serialized_end=894
-  _WORKFLOWATTRIBUTESDELETERESPONSE._serialized_start=896
-  _WORKFLOWATTRIBUTESDELETERESPONSE._serialized_end=930
+  _globals['_WORKFLOWATTRIBUTES']._serialized_start=102
+  _globals['_WORKFLOWATTRIBUTES']._serialized_end=285
+  _globals['_WORKFLOWATTRIBUTESUPDATEREQUEST']._serialized_start=287
+  _globals['_WORKFLOWATTRIBUTESUPDATEREQUEST']._serialized_end=388
+  _globals['_WORKFLOWATTRIBUTESUPDATERESPONSE']._serialized_start=390
+  _globals['_WORKFLOWATTRIBUTESUPDATERESPONSE']._serialized_end=424
+  _globals['_WORKFLOWATTRIBUTESGETREQUEST']._serialized_start=427
+  _globals['_WORKFLOWATTRIBUTESGETREQUEST']._serialized_end=607
+  _globals['_WORKFLOWATTRIBUTESGETRESPONSE']._serialized_start=609
+  _globals['_WORKFLOWATTRIBUTESGETRESPONSE']._serialized_end=708
+  _globals['_WORKFLOWATTRIBUTESDELETEREQUEST']._serialized_start=711
+  _globals['_WORKFLOWATTRIBUTESDELETEREQUEST']._serialized_end=894
+  _globals['_WORKFLOWATTRIBUTESDELETERESPONSE']._serialized_start=896
+  _globals['_WORKFLOWATTRIBUTESDELETERESPONSE']._serialized_end=930
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,61 +2,61 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class WorkflowAttributes(_message.Message):
-    __slots__ = ["domain", "matching_attributes", "project", "workflow"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    MATCHING_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["project", "domain", "workflow", "matching_attributes"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
     WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    matching_attributes: _matchable_resource_pb2.MatchingAttributes
+    MATCHING_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     project: str
+    domain: str
     workflow: str
+    matching_attributes: _matchable_resource_pb2.MatchingAttributes
     def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., workflow: _Optional[str] = ..., matching_attributes: _Optional[_Union[_matchable_resource_pb2.MatchingAttributes, _Mapping]] = ...) -> None: ...
 
-class WorkflowAttributesDeleteRequest(_message.Message):
-    __slots__ = ["domain", "project", "resource_type", "workflow"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    project: str
-    resource_type: _matchable_resource_pb2.MatchableResource
-    workflow: str
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., workflow: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
+class WorkflowAttributesUpdateRequest(_message.Message):
+    __slots__ = ["attributes"]
+    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
+    attributes: WorkflowAttributes
+    def __init__(self, attributes: _Optional[_Union[WorkflowAttributes, _Mapping]] = ...) -> None: ...
 
-class WorkflowAttributesDeleteResponse(_message.Message):
+class WorkflowAttributesUpdateResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class WorkflowAttributesGetRequest(_message.Message):
-    __slots__ = ["domain", "project", "resource_type", "workflow"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["project", "domain", "workflow", "resource_type"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
     WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    domain: str
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
     project: str
-    resource_type: _matchable_resource_pb2.MatchableResource
+    domain: str
     workflow: str
+    resource_type: _matchable_resource_pb2.MatchableResource
     def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., workflow: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
 
 class WorkflowAttributesGetResponse(_message.Message):
     __slots__ = ["attributes"]
     ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     attributes: WorkflowAttributes
     def __init__(self, attributes: _Optional[_Union[WorkflowAttributes, _Mapping]] = ...) -> None: ...
 
-class WorkflowAttributesUpdateRequest(_message.Message):
-    __slots__ = ["attributes"]
-    ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
-    attributes: WorkflowAttributes
-    def __init__(self, attributes: _Optional[_Union[WorkflowAttributes, _Mapping]] = ...) -> None: ...
+class WorkflowAttributesDeleteRequest(_message.Message):
+    __slots__ = ["project", "domain", "workflow", "resource_type"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    WORKFLOW_FIELD_NUMBER: _ClassVar[int]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    workflow: str
+    resource_type: _matchable_resource_pb2.MatchableResource
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., workflow: _Optional[str] = ..., resource_type: _Optional[_Union[_matchable_resource_pb2.MatchableResource, str]] = ...) -> None: ...
 
-class WorkflowAttributesUpdateResponse(_message.Message):
+class WorkflowAttributesDeleteResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/admin/workflow_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/admin/workflow_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -6,74 +6,74 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CreateWorkflowFailureReason(_message.Message):
-    __slots__ = ["exists_different_structure", "exists_identical_structure"]
-    EXISTS_DIFFERENT_STRUCTURE_FIELD_NUMBER: _ClassVar[int]
-    EXISTS_IDENTICAL_STRUCTURE_FIELD_NUMBER: _ClassVar[int]
-    exists_different_structure: WorkflowErrorExistsDifferentStructure
-    exists_identical_structure: WorkflowErrorExistsIdenticalStructure
-    def __init__(self, exists_different_structure: _Optional[_Union[WorkflowErrorExistsDifferentStructure, _Mapping]] = ..., exists_identical_structure: _Optional[_Union[WorkflowErrorExistsIdenticalStructure, _Mapping]] = ...) -> None: ...
+class WorkflowCreateRequest(_message.Message):
+    __slots__ = ["id", "spec"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    SPEC_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.Identifier
+    spec: WorkflowSpec
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., spec: _Optional[_Union[WorkflowSpec, _Mapping]] = ...) -> None: ...
+
+class WorkflowCreateResponse(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
 class Workflow(_message.Message):
-    __slots__ = ["closure", "id", "short_description"]
-    CLOSURE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "closure", "short_description"]
     ID_FIELD_NUMBER: _ClassVar[int]
+    CLOSURE_FIELD_NUMBER: _ClassVar[int]
     SHORT_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    closure: WorkflowClosure
     id: _identifier_pb2.Identifier
+    closure: WorkflowClosure
     short_description: str
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., closure: _Optional[_Union[WorkflowClosure, _Mapping]] = ..., short_description: _Optional[str] = ...) -> None: ...
 
+class WorkflowList(_message.Message):
+    __slots__ = ["workflows", "token"]
+    WORKFLOWS_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    workflows: _containers.RepeatedCompositeFieldContainer[Workflow]
+    token: str
+    def __init__(self, workflows: _Optional[_Iterable[_Union[Workflow, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
+
+class WorkflowSpec(_message.Message):
+    __slots__ = ["template", "sub_workflows", "description"]
+    TEMPLATE_FIELD_NUMBER: _ClassVar[int]
+    SUB_WORKFLOWS_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    template: _workflow_pb2.WorkflowTemplate
+    sub_workflows: _containers.RepeatedCompositeFieldContainer[_workflow_pb2.WorkflowTemplate]
+    description: _description_entity_pb2.DescriptionEntity
+    def __init__(self, template: _Optional[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]] = ..., sub_workflows: _Optional[_Iterable[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]]] = ..., description: _Optional[_Union[_description_entity_pb2.DescriptionEntity, _Mapping]] = ...) -> None: ...
+
 class WorkflowClosure(_message.Message):
     __slots__ = ["compiled_workflow", "created_at"]
     COMPILED_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     compiled_workflow: _compiler_pb2.CompiledWorkflowClosure
     created_at: _timestamp_pb2.Timestamp
     def __init__(self, compiled_workflow: _Optional[_Union[_compiler_pb2.CompiledWorkflowClosure, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class WorkflowCreateRequest(_message.Message):
-    __slots__ = ["id", "spec"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    SPEC_FIELD_NUMBER: _ClassVar[int]
-    id: _identifier_pb2.Identifier
-    spec: WorkflowSpec
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., spec: _Optional[_Union[WorkflowSpec, _Mapping]] = ...) -> None: ...
-
-class WorkflowCreateResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
 class WorkflowErrorExistsDifferentStructure(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ...) -> None: ...
 
 class WorkflowErrorExistsIdenticalStructure(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ...) -> None: ...
 
-class WorkflowList(_message.Message):
-    __slots__ = ["token", "workflows"]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOWS_FIELD_NUMBER: _ClassVar[int]
-    token: str
-    workflows: _containers.RepeatedCompositeFieldContainer[Workflow]
-    def __init__(self, workflows: _Optional[_Iterable[_Union[Workflow, _Mapping]]] = ..., token: _Optional[str] = ...) -> None: ...
-
-class WorkflowSpec(_message.Message):
-    __slots__ = ["description", "sub_workflows", "template"]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    SUB_WORKFLOWS_FIELD_NUMBER: _ClassVar[int]
-    TEMPLATE_FIELD_NUMBER: _ClassVar[int]
-    description: _description_entity_pb2.DescriptionEntity
-    sub_workflows: _containers.RepeatedCompositeFieldContainer[_workflow_pb2.WorkflowTemplate]
-    template: _workflow_pb2.WorkflowTemplate
-    def __init__(self, template: _Optional[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]] = ..., sub_workflows: _Optional[_Iterable[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]]] = ..., description: _Optional[_Union[_description_entity_pb2.DescriptionEntity, _Mapping]] = ...) -> None: ...
+class CreateWorkflowFailureReason(_message.Message):
+    __slots__ = ["exists_different_structure", "exists_identical_structure"]
+    EXISTS_DIFFERENT_STRUCTURE_FIELD_NUMBER: _ClassVar[int]
+    EXISTS_IDENTICAL_STRUCTURE_FIELD_NUMBER: _ClassVar[int]
+    exists_different_structure: WorkflowErrorExistsDifferentStructure
+    exists_identical_structure: WorkflowErrorExistsIdenticalStructure
+    def __init__(self, exists_different_structure: _Optional[_Union[WorkflowErrorExistsDifferentStructure, _Mapping]] = ..., exists_identical_structure: _Optional[_Union[WorkflowErrorExistsIdenticalStructure, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/catalog_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/identifier_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/core/catalog.proto
+# source: flyteidl/core/identifier.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/core/catalog.proto\x12\rflyteidl.core\x1a\x1e\x66lyteidl/core/identifier.proto\"I\n\x12\x43\x61talogArtifactTag\x12\x1f\n\x0b\x61rtifact_id\x18\x01 \x01(\tR\nartifactId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"\x83\x02\n\x0f\x43\x61talogMetadata\x12\x38\n\ndataset_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\tdatasetId\x12\x44\n\x0c\x61rtifact_tag\x18\x02 \x01(\x0b\x32!.flyteidl.core.CatalogArtifactTagR\x0b\x61rtifactTag\x12\\\n\x15source_task_execution\x18\x03 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierH\x00R\x13sourceTaskExecutionB\x12\n\x10source_execution\"\x9e\x01\n\x12\x43\x61talogReservation\"\x87\x01\n\x06Status\x12\x18\n\x14RESERVATION_DISABLED\x10\x00\x12\x18\n\x14RESERVATION_ACQUIRED\x10\x01\x12\x16\n\x12RESERVATION_EXISTS\x10\x02\x12\x18\n\x14RESERVATION_RELEASED\x10\x03\x12\x17\n\x13RESERVATION_FAILURE\x10\x04*\xa0\x01\n\x12\x43\x61talogCacheStatus\x12\x12\n\x0e\x43\x41\x43HE_DISABLED\x10\x00\x12\x0e\n\nCACHE_MISS\x10\x01\x12\r\n\tCACHE_HIT\x10\x02\x12\x13\n\x0f\x43\x41\x43HE_POPULATED\x10\x03\x12\x18\n\x14\x43\x41\x43HE_LOOKUP_FAILURE\x10\x04\x12\x15\n\x11\x43\x41\x43HE_PUT_FAILURE\x10\x05\x12\x11\n\rCACHE_SKIPPED\x10\x06\x42\xac\x01\n\x11\x63om.flyteidl.coreB\x0c\x43\x61talogProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x66lyteidl/core/identifier.proto\x12\rflyteidl.core\"\xae\x01\n\nIdentifier\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x18\n\x07project\x18\x02 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x03 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x18\n\x07version\x18\x05 \x01(\tR\x07version\"c\n\x1bWorkflowExecutionIdentifier\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\"\x81\x01\n\x17NodeExecutionIdentifier\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12M\n\x0c\x65xecution_id\x18\x02 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\"\xc6\x01\n\x17TaskExecutionIdentifier\x12\x32\n\x07task_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x06taskId\x12R\n\x11node_execution_id\x18\x02 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x0fnodeExecutionId\x12#\n\rretry_attempt\x18\x03 \x01(\rR\x0cretryAttempt\"~\n\x10SignalIdentifier\x12\x1b\n\tsignal_id\x18\x01 \x01(\tR\x08signalId\x12M\n\x0c\x65xecution_id\x18\x02 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId*U\n\x0cResourceType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04TASK\x10\x01\x12\x0c\n\x08WORKFLOW\x10\x02\x12\x0f\n\x0bLAUNCH_PLAN\x10\x03\x12\x0b\n\x07\x44\x41TASET\x10\x04\x42\xaf\x01\n\x11\x63om.flyteidl.coreB\x0fIdentifierProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.catalog_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.identifier_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\014CatalogProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _CATALOGCACHESTATUS._serialized_start=577
-  _CATALOGCACHESTATUS._serialized_end=737
-  _CATALOGARTIFACTTAG._serialized_start=78
-  _CATALOGARTIFACTTAG._serialized_end=151
-  _CATALOGMETADATA._serialized_start=154
-  _CATALOGMETADATA._serialized_end=413
-  _CATALOGRESERVATION._serialized_start=416
-  _CATALOGRESERVATION._serialized_end=574
-  _CATALOGRESERVATION_STATUS._serialized_start=439
-  _CATALOGRESERVATION_STATUS._serialized_end=574
+  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\017IdentifierProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
+  _globals['_RESOURCETYPE']._serialized_start=788
+  _globals['_RESOURCETYPE']._serialized_end=873
+  _globals['_IDENTIFIER']._serialized_start=50
+  _globals['_IDENTIFIER']._serialized_end=224
+  _globals['_WORKFLOWEXECUTIONIDENTIFIER']._serialized_start=226
+  _globals['_WORKFLOWEXECUTIONIDENTIFIER']._serialized_end=325
+  _globals['_NODEEXECUTIONIDENTIFIER']._serialized_start=328
+  _globals['_NODEEXECUTIONIDENTIFIER']._serialized_end=457
+  _globals['_TASKEXECUTIONIDENTIFIER']._serialized_start=460
+  _globals['_TASKEXECUTIONIDENTIFIER']._serialized_end=658
+  _globals['_SIGNALIDENTIFIER']._serialized_start=660
+  _globals['_SIGNALIDENTIFIER']._serialized_end=786
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/catalog_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/catalog_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 from flyteidl.core import identifier_pb2 as _identifier_pb2
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class CatalogCacheStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    CACHE_DISABLED: _ClassVar[CatalogCacheStatus]
+    CACHE_MISS: _ClassVar[CatalogCacheStatus]
+    CACHE_HIT: _ClassVar[CatalogCacheStatus]
+    CACHE_POPULATED: _ClassVar[CatalogCacheStatus]
+    CACHE_LOOKUP_FAILURE: _ClassVar[CatalogCacheStatus]
+    CACHE_PUT_FAILURE: _ClassVar[CatalogCacheStatus]
+    CACHE_SKIPPED: _ClassVar[CatalogCacheStatus]
 CACHE_DISABLED: CatalogCacheStatus
-CACHE_HIT: CatalogCacheStatus
-CACHE_LOOKUP_FAILURE: CatalogCacheStatus
 CACHE_MISS: CatalogCacheStatus
+CACHE_HIT: CatalogCacheStatus
 CACHE_POPULATED: CatalogCacheStatus
+CACHE_LOOKUP_FAILURE: CatalogCacheStatus
 CACHE_PUT_FAILURE: CatalogCacheStatus
 CACHE_SKIPPED: CatalogCacheStatus
-DESCRIPTOR: _descriptor.FileDescriptor
 
 class CatalogArtifactTag(_message.Message):
     __slots__ = ["artifact_id", "name"]
     ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     artifact_id: str
     name: str
     def __init__(self, artifact_id: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
 
 class CatalogMetadata(_message.Message):
-    __slots__ = ["artifact_tag", "dataset_id", "source_task_execution"]
-    ARTIFACT_TAG_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["dataset_id", "artifact_tag", "source_task_execution"]
     DATASET_ID_FIELD_NUMBER: _ClassVar[int]
+    ARTIFACT_TAG_FIELD_NUMBER: _ClassVar[int]
     SOURCE_TASK_EXECUTION_FIELD_NUMBER: _ClassVar[int]
-    artifact_tag: CatalogArtifactTag
     dataset_id: _identifier_pb2.Identifier
+    artifact_tag: CatalogArtifactTag
     source_task_execution: _identifier_pb2.TaskExecutionIdentifier
     def __init__(self, dataset_id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., artifact_tag: _Optional[_Union[CatalogArtifactTag, _Mapping]] = ..., source_task_execution: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
 class CatalogReservation(_message.Message):
     __slots__ = []
     class Status(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    RESERVATION_ACQUIRED: CatalogReservation.Status
+        RESERVATION_DISABLED: _ClassVar[CatalogReservation.Status]
+        RESERVATION_ACQUIRED: _ClassVar[CatalogReservation.Status]
+        RESERVATION_EXISTS: _ClassVar[CatalogReservation.Status]
+        RESERVATION_RELEASED: _ClassVar[CatalogReservation.Status]
+        RESERVATION_FAILURE: _ClassVar[CatalogReservation.Status]
     RESERVATION_DISABLED: CatalogReservation.Status
+    RESERVATION_ACQUIRED: CatalogReservation.Status
     RESERVATION_EXISTS: CatalogReservation.Status
-    RESERVATION_FAILURE: CatalogReservation.Status
     RESERVATION_RELEASED: CatalogReservation.Status
+    RESERVATION_FAILURE: CatalogReservation.Status
     def __init__(self) -> None: ...
-
-class CatalogCacheStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/compiler_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/condition_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/core/compiler.proto
+# source: flyteidl/core/condition.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from flyteidl.core import workflow_pb2 as flyteidl_dot_core_dot_workflow__pb2
-from flyteidl.core import tasks_pb2 as flyteidl_dot_core_dot_tasks__pb2
+from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/core/compiler.proto\x12\rflyteidl.core\x1a\x1c\x66lyteidl/core/workflow.proto\x1a\x19\x66lyteidl/core/tasks.proto\"\x87\x03\n\rConnectionSet\x12L\n\ndownstream\x18\x07 \x03(\x0b\x32,.flyteidl.core.ConnectionSet.DownstreamEntryR\ndownstream\x12\x46\n\x08upstream\x18\x08 \x03(\x0b\x32*.flyteidl.core.ConnectionSet.UpstreamEntryR\x08upstream\x1a\x1a\n\x06IdList\x12\x10\n\x03ids\x18\x01 \x03(\tR\x03ids\x1a\x62\n\x0f\x44ownstreamEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.flyteidl.core.ConnectionSet.IdListR\x05value:\x02\x38\x01\x1a`\n\rUpstreamEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.flyteidl.core.ConnectionSet.IdListR\x05value:\x02\x38\x01\"\x8f\x01\n\x10\x43ompiledWorkflow\x12;\n\x08template\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.WorkflowTemplateR\x08template\x12>\n\x0b\x63onnections\x18\x02 \x01(\x0b\x32\x1c.flyteidl.core.ConnectionSetR\x0b\x63onnections\"G\n\x0c\x43ompiledTask\x12\x37\n\x08template\x18\x01 \x01(\x0b\x32\x1b.flyteidl.core.TaskTemplateR\x08template\"\xcd\x01\n\x17\x43ompiledWorkflowClosure\x12\x39\n\x07primary\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.CompiledWorkflowR\x07primary\x12\x44\n\rsub_workflows\x18\x02 \x03(\x0b\x32\x1f.flyteidl.core.CompiledWorkflowR\x0csubWorkflows\x12\x31\n\x05tasks\x18\x03 \x03(\x0b\x32\x1b.flyteidl.core.CompiledTaskR\x05tasksB\xad\x01\n\x11\x63om.flyteidl.coreB\rCompilerProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/core/condition.proto\x12\rflyteidl.core\x1a\x1c\x66lyteidl/core/literals.proto\"\x8f\x02\n\x14\x43omparisonExpression\x12H\n\x08operator\x18\x01 \x01(\x0e\x32,.flyteidl.core.ComparisonExpression.OperatorR\x08operator\x12\x35\n\nleft_value\x18\x02 \x01(\x0b\x32\x16.flyteidl.core.OperandR\tleftValue\x12\x37\n\x0bright_value\x18\x03 \x01(\x0b\x32\x16.flyteidl.core.OperandR\nrightValue\"=\n\x08Operator\x12\x06\n\x02\x45Q\x10\x00\x12\x07\n\x03NEQ\x10\x01\x12\x06\n\x02GT\x10\x02\x12\x07\n\x03GTE\x10\x03\x12\x06\n\x02LT\x10\x04\x12\x07\n\x03LTE\x10\x05\"^\n\x07Operand\x12\x38\n\tprimitive\x18\x01 \x01(\x0b\x32\x18.flyteidl.core.PrimitiveH\x00R\tprimitive\x12\x12\n\x03var\x18\x02 \x01(\tH\x00R\x03varB\x05\n\x03val\"\xac\x01\n\x11\x42ooleanExpression\x12H\n\x0b\x63onjunction\x18\x01 \x01(\x0b\x32$.flyteidl.core.ConjunctionExpressionH\x00R\x0b\x63onjunction\x12\x45\n\ncomparison\x18\x02 \x01(\x0b\x32#.flyteidl.core.ComparisonExpressionH\x00R\ncomparisonB\x06\n\x04\x65xpr\"\xa5\x02\n\x15\x43onjunctionExpression\x12P\n\x08operator\x18\x01 \x01(\x0e\x32\x34.flyteidl.core.ConjunctionExpression.LogicalOperatorR\x08operator\x12I\n\x0fleft_expression\x18\x02 \x01(\x0b\x32 .flyteidl.core.BooleanExpressionR\x0eleftExpression\x12K\n\x10right_expression\x18\x03 \x01(\x0b\x32 .flyteidl.core.BooleanExpressionR\x0frightExpression\"\"\n\x0fLogicalOperator\x12\x07\n\x03\x41ND\x10\x00\x12\x06\n\x02OR\x10\x01\x42\xae\x01\n\x11\x63om.flyteidl.coreB\x0e\x43onditionProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.compiler_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.condition_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\rCompilerProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _CONNECTIONSET_DOWNSTREAMENTRY._options = None
-  _CONNECTIONSET_DOWNSTREAMENTRY._serialized_options = b'8\001'
-  _CONNECTIONSET_UPSTREAMENTRY._options = None
-  _CONNECTIONSET_UPSTREAMENTRY._serialized_options = b'8\001'
-  _CONNECTIONSET._serialized_start=105
-  _CONNECTIONSET._serialized_end=496
-  _CONNECTIONSET_IDLIST._serialized_start=272
-  _CONNECTIONSET_IDLIST._serialized_end=298
-  _CONNECTIONSET_DOWNSTREAMENTRY._serialized_start=300
-  _CONNECTIONSET_DOWNSTREAMENTRY._serialized_end=398
-  _CONNECTIONSET_UPSTREAMENTRY._serialized_start=400
-  _CONNECTIONSET_UPSTREAMENTRY._serialized_end=496
-  _COMPILEDWORKFLOW._serialized_start=499
-  _COMPILEDWORKFLOW._serialized_end=642
-  _COMPILEDTASK._serialized_start=644
-  _COMPILEDTASK._serialized_end=715
-  _COMPILEDWORKFLOWCLOSURE._serialized_start=718
-  _COMPILEDWORKFLOWCLOSURE._serialized_end=923
+  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\016ConditionProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
+  _globals['_COMPARISONEXPRESSION']._serialized_start=79
+  _globals['_COMPARISONEXPRESSION']._serialized_end=350
+  _globals['_COMPARISONEXPRESSION_OPERATOR']._serialized_start=289
+  _globals['_COMPARISONEXPRESSION_OPERATOR']._serialized_end=350
+  _globals['_OPERAND']._serialized_start=352
+  _globals['_OPERAND']._serialized_end=446
+  _globals['_BOOLEANEXPRESSION']._serialized_start=449
+  _globals['_BOOLEANEXPRESSION']._serialized_end=621
+  _globals['_CONJUNCTIONEXPRESSION']._serialized_start=624
+  _globals['_CONJUNCTIONEXPRESSION']._serialized_end=917
+  _globals['_CONJUNCTIONEXPRESSION_LOGICALOPERATOR']._serialized_start=883
+  _globals['_CONJUNCTIONEXPRESSION_LOGICALOPERATOR']._serialized_end=917
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/compiler_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/compiler_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3,57 +3,57 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CompiledTask(_message.Message):
-    __slots__ = ["template"]
-    TEMPLATE_FIELD_NUMBER: _ClassVar[int]
-    template: _tasks_pb2.TaskTemplate
-    def __init__(self, template: _Optional[_Union[_tasks_pb2.TaskTemplate, _Mapping]] = ...) -> None: ...
-
-class CompiledWorkflow(_message.Message):
-    __slots__ = ["connections", "template"]
-    CONNECTIONS_FIELD_NUMBER: _ClassVar[int]
-    TEMPLATE_FIELD_NUMBER: _ClassVar[int]
-    connections: ConnectionSet
-    template: _workflow_pb2.WorkflowTemplate
-    def __init__(self, template: _Optional[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]] = ..., connections: _Optional[_Union[ConnectionSet, _Mapping]] = ...) -> None: ...
-
-class CompiledWorkflowClosure(_message.Message):
-    __slots__ = ["primary", "sub_workflows", "tasks"]
-    PRIMARY_FIELD_NUMBER: _ClassVar[int]
-    SUB_WORKFLOWS_FIELD_NUMBER: _ClassVar[int]
-    TASKS_FIELD_NUMBER: _ClassVar[int]
-    primary: CompiledWorkflow
-    sub_workflows: _containers.RepeatedCompositeFieldContainer[CompiledWorkflow]
-    tasks: _containers.RepeatedCompositeFieldContainer[CompiledTask]
-    def __init__(self, primary: _Optional[_Union[CompiledWorkflow, _Mapping]] = ..., sub_workflows: _Optional[_Iterable[_Union[CompiledWorkflow, _Mapping]]] = ..., tasks: _Optional[_Iterable[_Union[CompiledTask, _Mapping]]] = ...) -> None: ...
-
 class ConnectionSet(_message.Message):
     __slots__ = ["downstream", "upstream"]
+    class IdList(_message.Message):
+        __slots__ = ["ids"]
+        IDS_FIELD_NUMBER: _ClassVar[int]
+        ids: _containers.RepeatedScalarFieldContainer[str]
+        def __init__(self, ids: _Optional[_Iterable[str]] = ...) -> None: ...
     class DownstreamEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: ConnectionSet.IdList
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[ConnectionSet.IdList, _Mapping]] = ...) -> None: ...
-    class IdList(_message.Message):
-        __slots__ = ["ids"]
-        IDS_FIELD_NUMBER: _ClassVar[int]
-        ids: _containers.RepeatedScalarFieldContainer[str]
-        def __init__(self, ids: _Optional[_Iterable[str]] = ...) -> None: ...
     class UpstreamEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: ConnectionSet.IdList
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[ConnectionSet.IdList, _Mapping]] = ...) -> None: ...
     DOWNSTREAM_FIELD_NUMBER: _ClassVar[int]
     UPSTREAM_FIELD_NUMBER: _ClassVar[int]
     downstream: _containers.MessageMap[str, ConnectionSet.IdList]
     upstream: _containers.MessageMap[str, ConnectionSet.IdList]
     def __init__(self, downstream: _Optional[_Mapping[str, ConnectionSet.IdList]] = ..., upstream: _Optional[_Mapping[str, ConnectionSet.IdList]] = ...) -> None: ...
+
+class CompiledWorkflow(_message.Message):
+    __slots__ = ["template", "connections"]
+    TEMPLATE_FIELD_NUMBER: _ClassVar[int]
+    CONNECTIONS_FIELD_NUMBER: _ClassVar[int]
+    template: _workflow_pb2.WorkflowTemplate
+    connections: ConnectionSet
+    def __init__(self, template: _Optional[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]] = ..., connections: _Optional[_Union[ConnectionSet, _Mapping]] = ...) -> None: ...
+
+class CompiledTask(_message.Message):
+    __slots__ = ["template"]
+    TEMPLATE_FIELD_NUMBER: _ClassVar[int]
+    template: _tasks_pb2.TaskTemplate
+    def __init__(self, template: _Optional[_Union[_tasks_pb2.TaskTemplate, _Mapping]] = ...) -> None: ...
+
+class CompiledWorkflowClosure(_message.Message):
+    __slots__ = ["primary", "sub_workflows", "tasks"]
+    PRIMARY_FIELD_NUMBER: _ClassVar[int]
+    SUB_WORKFLOWS_FIELD_NUMBER: _ClassVar[int]
+    TASKS_FIELD_NUMBER: _ClassVar[int]
+    primary: CompiledWorkflow
+    sub_workflows: _containers.RepeatedCompositeFieldContainer[CompiledWorkflow]
+    tasks: _containers.RepeatedCompositeFieldContainer[CompiledTask]
+    def __init__(self, primary: _Optional[_Union[CompiledWorkflow, _Mapping]] = ..., sub_workflows: _Optional[_Iterable[_Union[CompiledWorkflow, _Mapping]]] = ..., tasks: _Optional[_Iterable[_Union[CompiledTask, _Mapping]]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/condition_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/dask_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/core/condition.proto
+# source: flyteidl/plugins/dask.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
+from flyteidl.core import tasks_pb2 as flyteidl_dot_core_dot_tasks__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/core/condition.proto\x12\rflyteidl.core\x1a\x1c\x66lyteidl/core/literals.proto\"\x8f\x02\n\x14\x43omparisonExpression\x12H\n\x08operator\x18\x01 \x01(\x0e\x32,.flyteidl.core.ComparisonExpression.OperatorR\x08operator\x12\x35\n\nleft_value\x18\x02 \x01(\x0b\x32\x16.flyteidl.core.OperandR\tleftValue\x12\x37\n\x0bright_value\x18\x03 \x01(\x0b\x32\x16.flyteidl.core.OperandR\nrightValue\"=\n\x08Operator\x12\x06\n\x02\x45Q\x10\x00\x12\x07\n\x03NEQ\x10\x01\x12\x06\n\x02GT\x10\x02\x12\x07\n\x03GTE\x10\x03\x12\x06\n\x02LT\x10\x04\x12\x07\n\x03LTE\x10\x05\"^\n\x07Operand\x12\x38\n\tprimitive\x18\x01 \x01(\x0b\x32\x18.flyteidl.core.PrimitiveH\x00R\tprimitive\x12\x12\n\x03var\x18\x02 \x01(\tH\x00R\x03varB\x05\n\x03val\"\xac\x01\n\x11\x42ooleanExpression\x12H\n\x0b\x63onjunction\x18\x01 \x01(\x0b\x32$.flyteidl.core.ConjunctionExpressionH\x00R\x0b\x63onjunction\x12\x45\n\ncomparison\x18\x02 \x01(\x0b\x32#.flyteidl.core.ComparisonExpressionH\x00R\ncomparisonB\x06\n\x04\x65xpr\"\xa5\x02\n\x15\x43onjunctionExpression\x12P\n\x08operator\x18\x01 \x01(\x0e\x32\x34.flyteidl.core.ConjunctionExpression.LogicalOperatorR\x08operator\x12I\n\x0fleft_expression\x18\x02 \x01(\x0b\x32 .flyteidl.core.BooleanExpressionR\x0eleftExpression\x12K\n\x10right_expression\x18\x03 \x01(\x0b\x32 .flyteidl.core.BooleanExpressionR\x0frightExpression\"\"\n\x0fLogicalOperator\x12\x07\n\x03\x41ND\x10\x00\x12\x06\n\x02OR\x10\x01\x42\xae\x01\n\x11\x63om.flyteidl.coreB\x0e\x43onditionProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/plugins/dask.proto\x12\x10\x66lyteidl.plugins\x1a\x19\x66lyteidl/core/tasks.proto\"\x85\x01\n\x07\x44\x61skJob\x12=\n\tscheduler\x18\x01 \x01(\x0b\x32\x1f.flyteidl.plugins.DaskSchedulerR\tscheduler\x12;\n\x07workers\x18\x02 \x01(\x0b\x32!.flyteidl.plugins.DaskWorkerGroupR\x07workers\"]\n\rDaskScheduler\x12\x14\n\x05image\x18\x01 \x01(\tR\x05image\x12\x36\n\tresources\x18\x02 \x01(\x0b\x32\x18.flyteidl.core.ResourcesR\tresources\"\x8b\x01\n\x0f\x44\x61skWorkerGroup\x12*\n\x11number_of_workers\x18\x01 \x01(\rR\x0fnumberOfWorkers\x12\x14\n\x05image\x18\x02 \x01(\tR\x05image\x12\x36\n\tresources\x18\x03 \x01(\x0b\x32\x18.flyteidl.core.ResourcesR\tresourcesB\xbb\x01\n\x14\x63om.flyteidl.pluginsB\tDaskProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.condition_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.dask_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\016ConditionProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _COMPARISONEXPRESSION._serialized_start=79
-  _COMPARISONEXPRESSION._serialized_end=350
-  _COMPARISONEXPRESSION_OPERATOR._serialized_start=289
-  _COMPARISONEXPRESSION_OPERATOR._serialized_end=350
-  _OPERAND._serialized_start=352
-  _OPERAND._serialized_end=446
-  _BOOLEANEXPRESSION._serialized_start=449
-  _BOOLEANEXPRESSION._serialized_end=621
-  _CONJUNCTIONEXPRESSION._serialized_start=624
-  _CONJUNCTIONEXPRESSION._serialized_end=917
-  _CONJUNCTIONEXPRESSION_LOGICALOPERATOR._serialized_start=883
-  _CONJUNCTIONEXPRESSION_LOGICALOPERATOR._serialized_end=917
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\tDaskProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
+  _globals['_DASKJOB']._serialized_start=77
+  _globals['_DASKJOB']._serialized_end=210
+  _globals['_DASKSCHEDULER']._serialized_start=212
+  _globals['_DASKSCHEDULER']._serialized_end=305
+  _globals['_DASKWORKERGROUP']._serialized_start=308
+  _globals['_DASKWORKERGROUP']._serialized_end=447
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/condition_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/condition_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,54 +2,62 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class BooleanExpression(_message.Message):
-    __slots__ = ["comparison", "conjunction"]
-    COMPARISON_FIELD_NUMBER: _ClassVar[int]
-    CONJUNCTION_FIELD_NUMBER: _ClassVar[int]
-    comparison: ComparisonExpression
-    conjunction: ConjunctionExpression
-    def __init__(self, conjunction: _Optional[_Union[ConjunctionExpression, _Mapping]] = ..., comparison: _Optional[_Union[ComparisonExpression, _Mapping]] = ...) -> None: ...
-
 class ComparisonExpression(_message.Message):
-    __slots__ = ["left_value", "operator", "right_value"]
+    __slots__ = ["operator", "left_value", "right_value"]
     class Operator(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        EQ: _ClassVar[ComparisonExpression.Operator]
+        NEQ: _ClassVar[ComparisonExpression.Operator]
+        GT: _ClassVar[ComparisonExpression.Operator]
+        GTE: _ClassVar[ComparisonExpression.Operator]
+        LT: _ClassVar[ComparisonExpression.Operator]
+        LTE: _ClassVar[ComparisonExpression.Operator]
     EQ: ComparisonExpression.Operator
+    NEQ: ComparisonExpression.Operator
     GT: ComparisonExpression.Operator
     GTE: ComparisonExpression.Operator
-    LEFT_VALUE_FIELD_NUMBER: _ClassVar[int]
     LT: ComparisonExpression.Operator
     LTE: ComparisonExpression.Operator
-    NEQ: ComparisonExpression.Operator
     OPERATOR_FIELD_NUMBER: _ClassVar[int]
+    LEFT_VALUE_FIELD_NUMBER: _ClassVar[int]
     RIGHT_VALUE_FIELD_NUMBER: _ClassVar[int]
-    left_value: Operand
     operator: ComparisonExpression.Operator
+    left_value: Operand
     right_value: Operand
     def __init__(self, operator: _Optional[_Union[ComparisonExpression.Operator, str]] = ..., left_value: _Optional[_Union[Operand, _Mapping]] = ..., right_value: _Optional[_Union[Operand, _Mapping]] = ...) -> None: ...
 
+class Operand(_message.Message):
+    __slots__ = ["primitive", "var"]
+    PRIMITIVE_FIELD_NUMBER: _ClassVar[int]
+    VAR_FIELD_NUMBER: _ClassVar[int]
+    primitive: _literals_pb2.Primitive
+    var: str
+    def __init__(self, primitive: _Optional[_Union[_literals_pb2.Primitive, _Mapping]] = ..., var: _Optional[str] = ...) -> None: ...
+
+class BooleanExpression(_message.Message):
+    __slots__ = ["conjunction", "comparison"]
+    CONJUNCTION_FIELD_NUMBER: _ClassVar[int]
+    COMPARISON_FIELD_NUMBER: _ClassVar[int]
+    conjunction: ConjunctionExpression
+    comparison: ComparisonExpression
+    def __init__(self, conjunction: _Optional[_Union[ConjunctionExpression, _Mapping]] = ..., comparison: _Optional[_Union[ComparisonExpression, _Mapping]] = ...) -> None: ...
+
 class ConjunctionExpression(_message.Message):
-    __slots__ = ["left_expression", "operator", "right_expression"]
+    __slots__ = ["operator", "left_expression", "right_expression"]
     class LogicalOperator(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        AND: _ClassVar[ConjunctionExpression.LogicalOperator]
+        OR: _ClassVar[ConjunctionExpression.LogicalOperator]
     AND: ConjunctionExpression.LogicalOperator
-    LEFT_EXPRESSION_FIELD_NUMBER: _ClassVar[int]
-    OPERATOR_FIELD_NUMBER: _ClassVar[int]
     OR: ConjunctionExpression.LogicalOperator
+    OPERATOR_FIELD_NUMBER: _ClassVar[int]
+    LEFT_EXPRESSION_FIELD_NUMBER: _ClassVar[int]
     RIGHT_EXPRESSION_FIELD_NUMBER: _ClassVar[int]
-    left_expression: BooleanExpression
     operator: ConjunctionExpression.LogicalOperator
+    left_expression: BooleanExpression
     right_expression: BooleanExpression
     def __init__(self, operator: _Optional[_Union[ConjunctionExpression.LogicalOperator, str]] = ..., left_expression: _Optional[_Union[BooleanExpression, _Mapping]] = ..., right_expression: _Optional[_Union[BooleanExpression, _Mapping]] = ...) -> None: ...
-
-class Operand(_message.Message):
-    __slots__ = ["primitive", "var"]
-    PRIMITIVE_FIELD_NUMBER: _ClassVar[int]
-    VAR_FIELD_NUMBER: _ClassVar[int]
-    primitive: _literals_pb2.Primitive
-    var: str
-    def __init__(self, primitive: _Optional[_Union[_literals_pb2.Primitive, _Mapping]] = ..., var: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/dynamic_job_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/dynamic_job_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 from flyteidl.core import tasks_pb2 as flyteidl_dot_core_dot_tasks__pb2
 from flyteidl.core import workflow_pb2 as flyteidl_dot_core_dot_workflow__pb2
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66lyteidl/core/dynamic_job.proto\x12\rflyteidl.core\x1a\x19\x66lyteidl/core/tasks.proto\x1a\x1c\x66lyteidl/core/workflow.proto\x1a\x1c\x66lyteidl/core/literals.proto\"\x8a\x02\n\x0e\x44ynamicJobSpec\x12)\n\x05nodes\x18\x01 \x03(\x0b\x32\x13.flyteidl.core.NodeR\x05nodes\x12#\n\rmin_successes\x18\x02 \x01(\x03R\x0cminSuccesses\x12\x30\n\x07outputs\x18\x03 \x03(\x0b\x32\x16.flyteidl.core.BindingR\x07outputs\x12\x31\n\x05tasks\x18\x04 \x03(\x0b\x32\x1b.flyteidl.core.TaskTemplateR\x05tasks\x12\x43\n\x0csubworkflows\x18\x05 \x03(\x0b\x32\x1f.flyteidl.core.WorkflowTemplateR\x0csubworkflowsB\xaf\x01\n\x11\x63om.flyteidl.coreB\x0f\x44ynamicJobProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.dynamic_job_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.dynamic_job_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\017DynamicJobProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _DYNAMICJOBSPEC._serialized_start=138
-  _DYNAMICJOBSPEC._serialized_end=404
+  _globals['_DYNAMICJOBSPEC']._serialized_start=138
+  _globals['_DYNAMICJOBSPEC']._serialized_end=404
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/dynamic_job_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/dynamic_job_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DynamicJobSpec(_message.Message):
-    __slots__ = ["min_successes", "nodes", "outputs", "subworkflows", "tasks"]
-    MIN_SUCCESSES_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["nodes", "min_successes", "outputs", "tasks", "subworkflows"]
     NODES_FIELD_NUMBER: _ClassVar[int]
+    MIN_SUCCESSES_FIELD_NUMBER: _ClassVar[int]
     OUTPUTS_FIELD_NUMBER: _ClassVar[int]
-    SUBWORKFLOWS_FIELD_NUMBER: _ClassVar[int]
     TASKS_FIELD_NUMBER: _ClassVar[int]
-    min_successes: int
+    SUBWORKFLOWS_FIELD_NUMBER: _ClassVar[int]
     nodes: _containers.RepeatedCompositeFieldContainer[_workflow_pb2.Node]
+    min_successes: int
     outputs: _containers.RepeatedCompositeFieldContainer[_literals_pb2.Binding]
-    subworkflows: _containers.RepeatedCompositeFieldContainer[_workflow_pb2.WorkflowTemplate]
     tasks: _containers.RepeatedCompositeFieldContainer[_tasks_pb2.TaskTemplate]
+    subworkflows: _containers.RepeatedCompositeFieldContainer[_workflow_pb2.WorkflowTemplate]
     def __init__(self, nodes: _Optional[_Iterable[_Union[_workflow_pb2.Node, _Mapping]]] = ..., min_successes: _Optional[int] = ..., outputs: _Optional[_Iterable[_Union[_literals_pb2.Binding, _Mapping]]] = ..., tasks: _Optional[_Iterable[_Union[_tasks_pb2.TaskTemplate, _Mapping]]] = ..., subworkflows: _Optional[_Iterable[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/errors_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/errors_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 
 
 from flyteidl.core import execution_pb2 as flyteidl_dot_core_dot_execution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66lyteidl/core/errors.proto\x12\rflyteidl.core\x1a\x1d\x66lyteidl/core/execution.proto\"\xe5\x01\n\x0e\x43ontainerError\x12\x12\n\x04\x63ode\x18\x01 \x01(\tR\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x36\n\x04kind\x18\x03 \x01(\x0e\x32\".flyteidl.core.ContainerError.KindR\x04kind\x12?\n\x06origin\x18\x04 \x01(\x0e\x32\'.flyteidl.core.ExecutionError.ErrorKindR\x06origin\",\n\x04Kind\x12\x13\n\x0fNON_RECOVERABLE\x10\x00\x12\x0f\n\x0bRECOVERABLE\x10\x01\"D\n\rErrorDocument\x12\x33\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.flyteidl.core.ContainerErrorR\x05\x65rrorB\xab\x01\n\x11\x63om.flyteidl.coreB\x0b\x45rrorsProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.errors_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.errors_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\013ErrorsProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _CONTAINERERROR._serialized_start=77
-  _CONTAINERERROR._serialized_end=306
-  _CONTAINERERROR_KIND._serialized_start=262
-  _CONTAINERERROR_KIND._serialized_end=306
-  _ERRORDOCUMENT._serialized_start=308
-  _ERRORDOCUMENT._serialized_end=376
+  _globals['_CONTAINERERROR']._serialized_start=77
+  _globals['_CONTAINERERROR']._serialized_end=306
+  _globals['_CONTAINERERROR_KIND']._serialized_start=262
+  _globals['_CONTAINERERROR_KIND']._serialized_end=306
+  _globals['_ERRORDOCUMENT']._serialized_start=308
+  _globals['_ERRORDOCUMENT']._serialized_end=376
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/errors_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/errors_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ContainerError(_message.Message):
-    __slots__ = ["code", "kind", "message", "origin"]
+    __slots__ = ["code", "message", "kind", "origin"]
     class Kind(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        NON_RECOVERABLE: _ClassVar[ContainerError.Kind]
+        RECOVERABLE: _ClassVar[ContainerError.Kind]
+    NON_RECOVERABLE: ContainerError.Kind
+    RECOVERABLE: ContainerError.Kind
     CODE_FIELD_NUMBER: _ClassVar[int]
-    KIND_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    NON_RECOVERABLE: ContainerError.Kind
+    KIND_FIELD_NUMBER: _ClassVar[int]
     ORIGIN_FIELD_NUMBER: _ClassVar[int]
-    RECOVERABLE: ContainerError.Kind
     code: str
-    kind: ContainerError.Kind
     message: str
+    kind: ContainerError.Kind
     origin: _execution_pb2.ExecutionError.ErrorKind
     def __init__(self, code: _Optional[str] = ..., message: _Optional[str] = ..., kind: _Optional[_Union[ContainerError.Kind, str]] = ..., origin: _Optional[_Union[_execution_pb2.ExecutionError.ErrorKind, str]] = ...) -> None: ...
 
 class ErrorDocument(_message.Message):
     __slots__ = ["error"]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     error: ContainerError
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/execution_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/execution_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,40 +12,41 @@
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/core/execution.proto\x12\rflyteidl.core\x1a\x1egoogle/protobuf/duration.proto\"\xa7\x01\n\x11WorkflowExecution\"\x91\x01\n\x05Phase\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06QUEUED\x10\x01\x12\x0b\n\x07RUNNING\x10\x02\x12\x0e\n\nSUCCEEDING\x10\x03\x12\r\n\tSUCCEEDED\x10\x04\x12\x0b\n\x07\x46\x41ILING\x10\x05\x12\n\n\x06\x46\x41ILED\x10\x06\x12\x0b\n\x07\x41\x42ORTED\x10\x07\x12\r\n\tTIMED_OUT\x10\x08\x12\x0c\n\x08\x41\x42ORTING\x10\t\"\xb6\x01\n\rNodeExecution\"\xa4\x01\n\x05Phase\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06QUEUED\x10\x01\x12\x0b\n\x07RUNNING\x10\x02\x12\r\n\tSUCCEEDED\x10\x03\x12\x0b\n\x07\x46\x41ILING\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x41\x42ORTED\x10\x06\x12\x0b\n\x07SKIPPED\x10\x07\x12\r\n\tTIMED_OUT\x10\x08\x12\x13\n\x0f\x44YNAMIC_RUNNING\x10\t\x12\r\n\tRECOVERED\x10\n\"\x96\x01\n\rTaskExecution\"\x84\x01\n\x05Phase\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06QUEUED\x10\x01\x12\x0b\n\x07RUNNING\x10\x02\x12\r\n\tSUCCEEDED\x10\x03\x12\x0b\n\x07\x41\x42ORTED\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x10\n\x0cINITIALIZING\x10\x06\x12\x19\n\x15WAITING_FOR_RESOURCES\x10\x07\"\xc8\x01\n\x0e\x45xecutionError\x12\x12\n\x04\x63ode\x18\x01 \x01(\tR\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x1b\n\terror_uri\x18\x03 \x01(\tR\x08\x65rrorUri\x12;\n\x04kind\x18\x04 \x01(\x0e\x32\'.flyteidl.core.ExecutionError.ErrorKindR\x04kind\".\n\tErrorKind\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04USER\x10\x01\x12\n\n\x06SYSTEM\x10\x02\"\xda\x01\n\x07TaskLog\x12\x10\n\x03uri\x18\x01 \x01(\tR\x03uri\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12K\n\x0emessage_format\x18\x03 \x01(\x0e\x32$.flyteidl.core.TaskLog.MessageFormatR\rmessageFormat\x12+\n\x03ttl\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03ttl\"/\n\rMessageFormat\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x43SV\x10\x01\x12\x08\n\x04JSON\x10\x02\"Z\n\x14QualityOfServiceSpec\x12\x42\n\x0fqueueing_budget\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0equeueingBudget\"\xce\x01\n\x10QualityOfService\x12:\n\x04tier\x18\x01 \x01(\x0e\x32$.flyteidl.core.QualityOfService.TierH\x00R\x04tier\x12\x39\n\x04spec\x18\x02 \x01(\x0b\x32#.flyteidl.core.QualityOfServiceSpecH\x00R\x04spec\"4\n\x04Tier\x12\r\n\tUNDEFINED\x10\x00\x12\x08\n\x04HIGH\x10\x01\x12\n\n\x06MEDIUM\x10\x02\x12\x07\n\x03LOW\x10\x03\x42\r\n\x0b\x64\x65signationB\xae\x01\n\x11\x63om.flyteidl.coreB\x0e\x45xecutionProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.execution_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.execution_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\016ExecutionProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _WORKFLOWEXECUTION._serialized_start=81
-  _WORKFLOWEXECUTION._serialized_end=248
-  _WORKFLOWEXECUTION_PHASE._serialized_start=103
-  _WORKFLOWEXECUTION_PHASE._serialized_end=248
-  _NODEEXECUTION._serialized_start=251
-  _NODEEXECUTION._serialized_end=433
-  _NODEEXECUTION_PHASE._serialized_start=269
-  _NODEEXECUTION_PHASE._serialized_end=433
-  _TASKEXECUTION._serialized_start=436
-  _TASKEXECUTION._serialized_end=586
-  _TASKEXECUTION_PHASE._serialized_start=454
-  _TASKEXECUTION_PHASE._serialized_end=586
-  _EXECUTIONERROR._serialized_start=589
-  _EXECUTIONERROR._serialized_end=789
-  _EXECUTIONERROR_ERRORKIND._serialized_start=743
-  _EXECUTIONERROR_ERRORKIND._serialized_end=789
-  _TASKLOG._serialized_start=792
-  _TASKLOG._serialized_end=1010
-  _TASKLOG_MESSAGEFORMAT._serialized_start=963
-  _TASKLOG_MESSAGEFORMAT._serialized_end=1010
-  _QUALITYOFSERVICESPEC._serialized_start=1012
-  _QUALITYOFSERVICESPEC._serialized_end=1102
-  _QUALITYOFSERVICE._serialized_start=1105
-  _QUALITYOFSERVICE._serialized_end=1311
-  _QUALITYOFSERVICE_TIER._serialized_start=1244
-  _QUALITYOFSERVICE_TIER._serialized_end=1296
+  _globals['_WORKFLOWEXECUTION']._serialized_start=81
+  _globals['_WORKFLOWEXECUTION']._serialized_end=248
+  _globals['_WORKFLOWEXECUTION_PHASE']._serialized_start=103
+  _globals['_WORKFLOWEXECUTION_PHASE']._serialized_end=248
+  _globals['_NODEEXECUTION']._serialized_start=251
+  _globals['_NODEEXECUTION']._serialized_end=433
+  _globals['_NODEEXECUTION_PHASE']._serialized_start=269
+  _globals['_NODEEXECUTION_PHASE']._serialized_end=433
+  _globals['_TASKEXECUTION']._serialized_start=436
+  _globals['_TASKEXECUTION']._serialized_end=586
+  _globals['_TASKEXECUTION_PHASE']._serialized_start=454
+  _globals['_TASKEXECUTION_PHASE']._serialized_end=586
+  _globals['_EXECUTIONERROR']._serialized_start=589
+  _globals['_EXECUTIONERROR']._serialized_end=789
+  _globals['_EXECUTIONERROR_ERRORKIND']._serialized_start=743
+  _globals['_EXECUTIONERROR_ERRORKIND']._serialized_end=789
+  _globals['_TASKLOG']._serialized_start=792
+  _globals['_TASKLOG']._serialized_end=1010
+  _globals['_TASKLOG_MESSAGEFORMAT']._serialized_start=963
+  _globals['_TASKLOG_MESSAGEFORMAT']._serialized_end=1010
+  _globals['_QUALITYOFSERVICESPEC']._serialized_start=1012
+  _globals['_QUALITYOFSERVICESPEC']._serialized_end=1102
+  _globals['_QUALITYOFSERVICE']._serialized_start=1105
+  _globals['_QUALITYOFSERVICE']._serialized_end=1311
+  _globals['_QUALITYOFSERVICE_TIER']._serialized_start=1244
+  _globals['_QUALITYOFSERVICE_TIER']._serialized_end=1296
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/identifier_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/security_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/core/identifier.proto
+# source: flyteidl/core/security.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x66lyteidl/core/identifier.proto\x12\rflyteidl.core\"\xae\x01\n\nIdentifier\x12@\n\rresource_type\x18\x01 \x01(\x0e\x32\x1b.flyteidl.core.ResourceTypeR\x0cresourceType\x12\x18\n\x07project\x18\x02 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x03 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x18\n\x07version\x18\x05 \x01(\tR\x07version\"c\n\x1bWorkflowExecutionIdentifier\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\"\x81\x01\n\x17NodeExecutionIdentifier\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12M\n\x0c\x65xecution_id\x18\x02 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\"\xc6\x01\n\x17TaskExecutionIdentifier\x12\x32\n\x07task_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x06taskId\x12R\n\x11node_execution_id\x18\x02 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x0fnodeExecutionId\x12#\n\rretry_attempt\x18\x03 \x01(\rR\x0cretryAttempt\"~\n\x10SignalIdentifier\x12\x1b\n\tsignal_id\x18\x01 \x01(\tR\x08signalId\x12M\n\x0c\x65xecution_id\x18\x02 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId*U\n\x0cResourceType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04TASK\x10\x01\x12\x0c\n\x08WORKFLOW\x10\x02\x12\x0f\n\x0bLAUNCH_PLAN\x10\x03\x12\x0b\n\x07\x44\x41TASET\x10\x04\x42\xaf\x01\n\x11\x63om.flyteidl.coreB\x0fIdentifierProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/core/security.proto\x12\rflyteidl.core\"\xd0\x01\n\x06Secret\x12\x14\n\x05group\x18\x01 \x01(\tR\x05group\x12#\n\rgroup_version\x18\x02 \x01(\tR\x0cgroupVersion\x12\x10\n\x03key\x18\x03 \x01(\tR\x03key\x12L\n\x11mount_requirement\x18\x04 \x01(\x0e\x32\x1f.flyteidl.core.Secret.MountTypeR\x10mountRequirement\"+\n\tMountType\x12\x07\n\x03\x41NY\x10\x00\x12\x0b\n\x07\x45NV_VAR\x10\x01\x12\x08\n\x04\x46ILE\x10\x02\"g\n\x0cOAuth2Client\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12:\n\rclient_secret\x18\x02 \x01(\x0b\x32\x15.flyteidl.core.SecretR\x0c\x63lientSecret\"\x97\x01\n\x08Identity\x12\x19\n\x08iam_role\x18\x01 \x01(\tR\x07iamRole\x12.\n\x13k8s_service_account\x18\x02 \x01(\tR\x11k8sServiceAccount\x12@\n\roauth2_client\x18\x03 \x01(\x0b\x32\x1b.flyteidl.core.OAuth2ClientR\x0coauth2Client\"\x96\x02\n\x12OAuth2TokenRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12:\n\x04type\x18\x02 \x01(\x0e\x32&.flyteidl.core.OAuth2TokenRequest.TypeR\x04type\x12\x33\n\x06\x63lient\x18\x03 \x01(\x0b\x32\x1b.flyteidl.core.OAuth2ClientR\x06\x63lient\x12\x34\n\x16idp_discovery_endpoint\x18\x04 \x01(\tR\x14idpDiscoveryEndpoint\x12%\n\x0etoken_endpoint\x18\x05 \x01(\tR\rtokenEndpoint\"\x1e\n\x04Type\x12\x16\n\x12\x43LIENT_CREDENTIALS\x10\x00\"\xad\x01\n\x0fSecurityContext\x12.\n\x06run_as\x18\x01 \x01(\x0b\x32\x17.flyteidl.core.IdentityR\x05runAs\x12/\n\x07secrets\x18\x02 \x03(\x0b\x32\x15.flyteidl.core.SecretR\x07secrets\x12\x39\n\x06tokens\x18\x03 \x03(\x0b\x32!.flyteidl.core.OAuth2TokenRequestR\x06tokensB\xad\x01\n\x11\x63om.flyteidl.coreB\rSecurityProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.identifier_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.security_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\017IdentifierProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _RESOURCETYPE._serialized_start=788
-  _RESOURCETYPE._serialized_end=873
-  _IDENTIFIER._serialized_start=50
-  _IDENTIFIER._serialized_end=224
-  _WORKFLOWEXECUTIONIDENTIFIER._serialized_start=226
-  _WORKFLOWEXECUTIONIDENTIFIER._serialized_end=325
-  _NODEEXECUTIONIDENTIFIER._serialized_start=328
-  _NODEEXECUTIONIDENTIFIER._serialized_end=457
-  _TASKEXECUTIONIDENTIFIER._serialized_start=460
-  _TASKEXECUTIONIDENTIFIER._serialized_end=658
-  _SIGNALIDENTIFIER._serialized_start=660
-  _SIGNALIDENTIFIER._serialized_end=786
+  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\rSecurityProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
+  _globals['_SECRET']._serialized_start=48
+  _globals['_SECRET']._serialized_end=256
+  _globals['_SECRET_MOUNTTYPE']._serialized_start=213
+  _globals['_SECRET_MOUNTTYPE']._serialized_end=256
+  _globals['_OAUTH2CLIENT']._serialized_start=258
+  _globals['_OAUTH2CLIENT']._serialized_end=361
+  _globals['_IDENTITY']._serialized_start=364
+  _globals['_IDENTITY']._serialized_end=515
+  _globals['_OAUTH2TOKENREQUEST']._serialized_start=518
+  _globals['_OAUTH2TOKENREQUEST']._serialized_end=796
+  _globals['_OAUTH2TOKENREQUEST_TYPE']._serialized_start=766
+  _globals['_OAUTH2TOKENREQUEST_TYPE']._serialized_end=796
+  _globals['_SECURITYCONTEXT']._serialized_start=799
+  _globals['_SECURITYCONTEXT']._serialized_end=972
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/identifier_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/identifier_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-DATASET: ResourceType
 DESCRIPTOR: _descriptor.FileDescriptor
-LAUNCH_PLAN: ResourceType
-TASK: ResourceType
+
+class ResourceType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    UNSPECIFIED: _ClassVar[ResourceType]
+    TASK: _ClassVar[ResourceType]
+    WORKFLOW: _ClassVar[ResourceType]
+    LAUNCH_PLAN: _ClassVar[ResourceType]
+    DATASET: _ClassVar[ResourceType]
 UNSPECIFIED: ResourceType
+TASK: ResourceType
 WORKFLOW: ResourceType
+LAUNCH_PLAN: ResourceType
+DATASET: ResourceType
 
 class Identifier(_message.Message):
-    __slots__ = ["domain", "name", "project", "resource_type", "version"]
+    __slots__ = ["resource_type", "project", "domain", "name", "version"]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
     DOMAIN_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
+    resource_type: ResourceType
+    project: str
     domain: str
     name: str
-    project: str
-    resource_type: ResourceType
     version: str
     def __init__(self, resource_type: _Optional[_Union[ResourceType, str]] = ..., project: _Optional[str] = ..., domain: _Optional[str] = ..., name: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
 
+class WorkflowExecutionIdentifier(_message.Message):
+    __slots__ = ["project", "domain", "name"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    name: str
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
+
 class NodeExecutionIdentifier(_message.Message):
-    __slots__ = ["execution_id", "node_id"]
-    EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["node_id", "execution_id"]
     NODE_ID_FIELD_NUMBER: _ClassVar[int]
-    execution_id: WorkflowExecutionIdentifier
-    node_id: str
-    def __init__(self, node_id: _Optional[str] = ..., execution_id: _Optional[_Union[WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
-
-class SignalIdentifier(_message.Message):
-    __slots__ = ["execution_id", "signal_id"]
     EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    SIGNAL_ID_FIELD_NUMBER: _ClassVar[int]
+    node_id: str
     execution_id: WorkflowExecutionIdentifier
-    signal_id: str
-    def __init__(self, signal_id: _Optional[str] = ..., execution_id: _Optional[_Union[WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
+    def __init__(self, node_id: _Optional[str] = ..., execution_id: _Optional[_Union[WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
 class TaskExecutionIdentifier(_message.Message):
-    __slots__ = ["node_execution_id", "retry_attempt", "task_id"]
+    __slots__ = ["task_id", "node_execution_id", "retry_attempt"]
+    TASK_ID_FIELD_NUMBER: _ClassVar[int]
     NODE_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
     RETRY_ATTEMPT_FIELD_NUMBER: _ClassVar[int]
-    TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    task_id: Identifier
     node_execution_id: NodeExecutionIdentifier
     retry_attempt: int
-    task_id: Identifier
     def __init__(self, task_id: _Optional[_Union[Identifier, _Mapping]] = ..., node_execution_id: _Optional[_Union[NodeExecutionIdentifier, _Mapping]] = ..., retry_attempt: _Optional[int] = ...) -> None: ...
 
-class WorkflowExecutionIdentifier(_message.Message):
-    __slots__ = ["domain", "name", "project"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    name: str
-    project: str
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
-
-class ResourceType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class SignalIdentifier(_message.Message):
+    __slots__ = ["signal_id", "execution_id"]
+    SIGNAL_ID_FIELD_NUMBER: _ClassVar[int]
+    EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    signal_id: str
+    execution_id: WorkflowExecutionIdentifier
+    def __init__(self, signal_id: _Optional[str] = ..., execution_id: _Optional[_Union[WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/interface_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/interface_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 
 from flyteidl.core import types_pb2 as flyteidl_dot_core_dot_types__pb2
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/core/interface.proto\x12\rflyteidl.core\x1a\x19\x66lyteidl/core/types.proto\x1a\x1c\x66lyteidl/core/literals.proto\"\\\n\x08Variable\x12.\n\x04type\x18\x01 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\x04type\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"\xad\x01\n\x0bVariableMap\x12G\n\tvariables\x18\x01 \x03(\x0b\x32).flyteidl.core.VariableMap.VariablesEntryR\tvariables\x1aU\n\x0eVariablesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x17.flyteidl.core.VariableR\x05value:\x02\x38\x01\"z\n\x0eTypedInterface\x12\x32\n\x06inputs\x18\x01 \x01(\x0b\x32\x1a.flyteidl.core.VariableMapR\x06inputs\x12\x34\n\x07outputs\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.VariableMapR\x07outputs\"\x94\x01\n\tParameter\x12)\n\x03var\x18\x01 \x01(\x0b\x32\x17.flyteidl.core.VariableR\x03var\x12\x32\n\x07\x64\x65\x66\x61ult\x18\x02 \x01(\x0b\x32\x16.flyteidl.core.LiteralH\x00R\x07\x64\x65\x66\x61ult\x12\x1c\n\x08required\x18\x03 \x01(\x08H\x00R\x08requiredB\n\n\x08\x62\x65havior\"\xb4\x01\n\x0cParameterMap\x12K\n\nparameters\x18\x01 \x03(\x0b\x32+.flyteidl.core.ParameterMap.ParametersEntryR\nparameters\x1aW\n\x0fParametersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x18.flyteidl.core.ParameterR\x05value:\x02\x38\x01\x42\xae\x01\n\x11\x63om.flyteidl.coreB\x0eInterfaceProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.interface_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.interface_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\016InterfaceProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
   _VARIABLEMAP_VARIABLESENTRY._options = None
   _VARIABLEMAP_VARIABLESENTRY._serialized_options = b'8\001'
   _PARAMETERMAP_PARAMETERSENTRY._options = None
   _PARAMETERMAP_PARAMETERSENTRY._serialized_options = b'8\001'
-  _VARIABLE._serialized_start=105
-  _VARIABLE._serialized_end=197
-  _VARIABLEMAP._serialized_start=200
-  _VARIABLEMAP._serialized_end=373
-  _VARIABLEMAP_VARIABLESENTRY._serialized_start=288
-  _VARIABLEMAP_VARIABLESENTRY._serialized_end=373
-  _TYPEDINTERFACE._serialized_start=375
-  _TYPEDINTERFACE._serialized_end=497
-  _PARAMETER._serialized_start=500
-  _PARAMETER._serialized_end=648
-  _PARAMETERMAP._serialized_start=651
-  _PARAMETERMAP._serialized_end=831
-  _PARAMETERMAP_PARAMETERSENTRY._serialized_start=744
-  _PARAMETERMAP_PARAMETERSENTRY._serialized_end=831
+  _globals['_VARIABLE']._serialized_start=105
+  _globals['_VARIABLE']._serialized_end=197
+  _globals['_VARIABLEMAP']._serialized_start=200
+  _globals['_VARIABLEMAP']._serialized_end=373
+  _globals['_VARIABLEMAP_VARIABLESENTRY']._serialized_start=288
+  _globals['_VARIABLEMAP_VARIABLESENTRY']._serialized_end=373
+  _globals['_TYPEDINTERFACE']._serialized_start=375
+  _globals['_TYPEDINTERFACE']._serialized_end=497
+  _globals['_PARAMETER']._serialized_start=500
+  _globals['_PARAMETER']._serialized_end=648
+  _globals['_PARAMETERMAP']._serialized_start=651
+  _globals['_PARAMETERMAP']._serialized_end=831
+  _globals['_PARAMETERMAP_PARAMETERSENTRY']._serialized_start=744
+  _globals['_PARAMETERMAP_PARAMETERSENTRY']._serialized_end=831
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/interface_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/interface_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -3,58 +3,58 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Parameter(_message.Message):
-    __slots__ = ["default", "required", "var"]
-    DEFAULT_FIELD_NUMBER: _ClassVar[int]
-    REQUIRED_FIELD_NUMBER: _ClassVar[int]
-    VAR_FIELD_NUMBER: _ClassVar[int]
-    default: _literals_pb2.Literal
-    required: bool
-    var: Variable
-    def __init__(self, var: _Optional[_Union[Variable, _Mapping]] = ..., default: _Optional[_Union[_literals_pb2.Literal, _Mapping]] = ..., required: bool = ...) -> None: ...
+class Variable(_message.Message):
+    __slots__ = ["type", "description"]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    type: _types_pb2.LiteralType
+    description: str
+    def __init__(self, type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ..., description: _Optional[str] = ...) -> None: ...
 
-class ParameterMap(_message.Message):
-    __slots__ = ["parameters"]
-    class ParametersEntry(_message.Message):
+class VariableMap(_message.Message):
+    __slots__ = ["variables"]
+    class VariablesEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
-        value: Parameter
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[Parameter, _Mapping]] = ...) -> None: ...
-    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
-    parameters: _containers.MessageMap[str, Parameter]
-    def __init__(self, parameters: _Optional[_Mapping[str, Parameter]] = ...) -> None: ...
+        value: Variable
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[Variable, _Mapping]] = ...) -> None: ...
+    VARIABLES_FIELD_NUMBER: _ClassVar[int]
+    variables: _containers.MessageMap[str, Variable]
+    def __init__(self, variables: _Optional[_Mapping[str, Variable]] = ...) -> None: ...
 
 class TypedInterface(_message.Message):
     __slots__ = ["inputs", "outputs"]
     INPUTS_FIELD_NUMBER: _ClassVar[int]
     OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     inputs: VariableMap
     outputs: VariableMap
     def __init__(self, inputs: _Optional[_Union[VariableMap, _Mapping]] = ..., outputs: _Optional[_Union[VariableMap, _Mapping]] = ...) -> None: ...
 
-class Variable(_message.Message):
-    __slots__ = ["description", "type"]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    description: str
-    type: _types_pb2.LiteralType
-    def __init__(self, type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ..., description: _Optional[str] = ...) -> None: ...
+class Parameter(_message.Message):
+    __slots__ = ["var", "default", "required"]
+    VAR_FIELD_NUMBER: _ClassVar[int]
+    DEFAULT_FIELD_NUMBER: _ClassVar[int]
+    REQUIRED_FIELD_NUMBER: _ClassVar[int]
+    var: Variable
+    default: _literals_pb2.Literal
+    required: bool
+    def __init__(self, var: _Optional[_Union[Variable, _Mapping]] = ..., default: _Optional[_Union[_literals_pb2.Literal, _Mapping]] = ..., required: bool = ...) -> None: ...
 
-class VariableMap(_message.Message):
-    __slots__ = ["variables"]
-    class VariablesEntry(_message.Message):
+class ParameterMap(_message.Message):
+    __slots__ = ["parameters"]
+    class ParametersEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
-        value: Variable
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[Variable, _Mapping]] = ...) -> None: ...
-    VARIABLES_FIELD_NUMBER: _ClassVar[int]
-    variables: _containers.MessageMap[str, Variable]
-    def __init__(self, variables: _Optional[_Mapping[str, Variable]] = ...) -> None: ...
+        value: Parameter
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[Parameter, _Mapping]] = ...) -> None: ...
+    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
+    parameters: _containers.MessageMap[str, Parameter]
+    def __init__(self, parameters: _Optional[_Mapping[str, Parameter]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/literals_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/types_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,56 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/core/literals.proto
+# source: flyteidl/core/types.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from flyteidl.core import types_pb2 as flyteidl_dot_core_dot_types__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/core/literals.proto\x12\rflyteidl.core\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x19\x66lyteidl/core/types.proto\"\x87\x02\n\tPrimitive\x12\x1a\n\x07integer\x18\x01 \x01(\x03H\x00R\x07integer\x12!\n\x0b\x66loat_value\x18\x02 \x01(\x01H\x00R\nfloatValue\x12#\n\x0cstring_value\x18\x03 \x01(\tH\x00R\x0bstringValue\x12\x1a\n\x07\x62oolean\x18\x04 \x01(\x08H\x00R\x07\x62oolean\x12\x38\n\x08\x64\x61tetime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00R\x08\x64\x61tetime\x12\x37\n\x08\x64uration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationH\x00R\x08\x64urationB\x07\n\x05value\"\x06\n\x04Void\"Q\n\x04\x42lob\x12\x37\n\x08metadata\x18\x01 \x01(\x0b\x32\x1b.flyteidl.core.BlobMetadataR\x08metadata\x12\x10\n\x03uri\x18\x03 \x01(\tR\x03uri\";\n\x0c\x42lobMetadata\x12+\n\x04type\x18\x01 \x01(\x0b\x32\x17.flyteidl.core.BlobTypeR\x04type\"0\n\x06\x42inary\x12\x14\n\x05value\x18\x01 \x01(\x0cR\x05value\x12\x10\n\x03tag\x18\x02 \x01(\tR\x03tag\"I\n\x06Schema\x12\x10\n\x03uri\x18\x01 \x01(\tR\x03uri\x12-\n\x04type\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.SchemaTypeR\x04type\"e\n\x05Union\x12,\n\x05value\x18\x01 \x01(\x0b\x32\x16.flyteidl.core.LiteralR\x05value\x12.\n\x04type\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\x04type\"y\n\x19StructuredDatasetMetadata\x12\\\n\x17structured_dataset_type\x18\x01 \x01(\x0b\x32$.flyteidl.core.StructuredDatasetTypeR\x15structuredDatasetType\"k\n\x11StructuredDataset\x12\x10\n\x03uri\x18\x01 \x01(\tR\x03uri\x12\x44\n\x08metadata\x18\x02 \x01(\x0b\x32(.flyteidl.core.StructuredDatasetMetadataR\x08metadata\"\xf0\x03\n\x06Scalar\x12\x38\n\tprimitive\x18\x01 \x01(\x0b\x32\x18.flyteidl.core.PrimitiveH\x00R\tprimitive\x12)\n\x04\x62lob\x18\x02 \x01(\x0b\x32\x13.flyteidl.core.BlobH\x00R\x04\x62lob\x12/\n\x06\x62inary\x18\x03 \x01(\x0b\x32\x15.flyteidl.core.BinaryH\x00R\x06\x62inary\x12/\n\x06schema\x18\x04 \x01(\x0b\x32\x15.flyteidl.core.SchemaH\x00R\x06schema\x12\x32\n\tnone_type\x18\x05 \x01(\x0b\x32\x13.flyteidl.core.VoidH\x00R\x08noneType\x12,\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x14.flyteidl.core.ErrorH\x00R\x05\x65rror\x12\x33\n\x07generic\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructH\x00R\x07generic\x12Q\n\x12structured_dataset\x18\x08 \x01(\x0b\x32 .flyteidl.core.StructuredDatasetH\x00R\x11structuredDataset\x12,\n\x05union\x18\t \x01(\x0b\x32\x14.flyteidl.core.UnionH\x00R\x05unionB\x07\n\x05value\"\xca\x01\n\x07Literal\x12/\n\x06scalar\x18\x01 \x01(\x0b\x32\x15.flyteidl.core.ScalarH\x00R\x06scalar\x12\x42\n\ncollection\x18\x02 \x01(\x0b\x32 .flyteidl.core.LiteralCollectionH\x00R\ncollection\x12-\n\x03map\x18\x03 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\x03map\x12\x12\n\x04hash\x18\x04 \x01(\tR\x04hashB\x07\n\x05value\"G\n\x11LiteralCollection\x12\x32\n\x08literals\x18\x01 \x03(\x0b\x32\x16.flyteidl.core.LiteralR\x08literals\"\xa6\x01\n\nLiteralMap\x12\x43\n\x08literals\x18\x01 \x03(\x0b\x32\'.flyteidl.core.LiteralMap.LiteralsEntryR\x08literals\x1aS\n\rLiteralsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.flyteidl.core.LiteralR\x05value:\x02\x38\x01\"O\n\x15\x42indingDataCollection\x12\x36\n\x08\x62indings\x18\x01 \x03(\x0b\x32\x1a.flyteidl.core.BindingDataR\x08\x62indings\"\xb2\x01\n\x0e\x42indingDataMap\x12G\n\x08\x62indings\x18\x01 \x03(\x0b\x32+.flyteidl.core.BindingDataMap.BindingsEntryR\x08\x62indings\x1aW\n\rBindingsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.BindingDataR\x05value:\x02\x38\x01\"G\n\tUnionInfo\x12:\n\ntargetType\x18\x01 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\ntargetType\"\xae\x02\n\x0b\x42indingData\x12/\n\x06scalar\x18\x01 \x01(\x0b\x32\x15.flyteidl.core.ScalarH\x00R\x06scalar\x12\x46\n\ncollection\x18\x02 \x01(\x0b\x32$.flyteidl.core.BindingDataCollectionH\x00R\ncollection\x12:\n\x07promise\x18\x03 \x01(\x0b\x32\x1e.flyteidl.core.OutputReferenceH\x00R\x07promise\x12\x31\n\x03map\x18\x04 \x01(\x0b\x32\x1d.flyteidl.core.BindingDataMapH\x00R\x03map\x12.\n\x05union\x18\x05 \x01(\x0b\x32\x18.flyteidl.core.UnionInfoR\x05unionB\x07\n\x05value\"Q\n\x07\x42inding\x12\x10\n\x03var\x18\x01 \x01(\tR\x03var\x12\x34\n\x07\x62inding\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.BindingDataR\x07\x62inding\"6\n\x0cKeyValuePair\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\")\n\rRetryStrategy\x12\x18\n\x07retries\x18\x05 \x01(\rR\x07retriesB\xad\x01\n\x11\x63om.flyteidl.coreB\rLiteralsProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66lyteidl/core/types.proto\x12\rflyteidl.core\x1a\x1cgoogle/protobuf/struct.proto\"\xa1\x02\n\nSchemaType\x12@\n\x07\x63olumns\x18\x03 \x03(\x0b\x32&.flyteidl.core.SchemaType.SchemaColumnR\x07\x63olumns\x1a\xd0\x01\n\x0cSchemaColumn\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12K\n\x04type\x18\x02 \x01(\x0e\x32\x37.flyteidl.core.SchemaType.SchemaColumn.SchemaColumnTypeR\x04type\"_\n\x10SchemaColumnType\x12\x0b\n\x07INTEGER\x10\x00\x12\t\n\x05\x46LOAT\x10\x01\x12\n\n\x06STRING\x10\x02\x12\x0b\n\x07\x42OOLEAN\x10\x03\x12\x0c\n\x08\x44\x41TETIME\x10\x04\x12\x0c\n\x08\x44URATION\x10\x05\"\xc7\x02\n\x15StructuredDatasetType\x12L\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x32.flyteidl.core.StructuredDatasetType.DatasetColumnR\x07\x63olumns\x12\x16\n\x06\x66ormat\x18\x02 \x01(\tR\x06\x66ormat\x12\x30\n\x14\x65xternal_schema_type\x18\x03 \x01(\tR\x12\x65xternalSchemaType\x12\x32\n\x15\x65xternal_schema_bytes\x18\x04 \x01(\x0cR\x13\x65xternalSchemaBytes\x1a\x62\n\rDatasetColumn\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12=\n\x0cliteral_type\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\x0bliteralType\"\xa7\x01\n\x08\x42lobType\x12\x16\n\x06\x66ormat\x18\x01 \x01(\tR\x06\x66ormat\x12R\n\x0e\x64imensionality\x18\x02 \x01(\x0e\x32*.flyteidl.core.BlobType.BlobDimensionalityR\x0e\x64imensionality\"/\n\x12\x42lobDimensionality\x12\n\n\x06SINGLE\x10\x00\x12\r\n\tMULTIPART\x10\x01\"\"\n\x08\x45numType\x12\x16\n\x06values\x18\x01 \x03(\tR\x06values\"C\n\tUnionType\x12\x36\n\x08variants\x18\x01 \x03(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\x08variants\"!\n\rTypeStructure\x12\x10\n\x03tag\x18\x01 \x01(\tR\x03tag\"K\n\x0eTypeAnnotation\x12\x39\n\x0b\x61nnotations\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x0b\x61nnotations\"\xbc\x05\n\x0bLiteralType\x12\x33\n\x06simple\x18\x01 \x01(\x0e\x32\x19.flyteidl.core.SimpleTypeH\x00R\x06simple\x12\x33\n\x06schema\x18\x02 \x01(\x0b\x32\x19.flyteidl.core.SchemaTypeH\x00R\x06schema\x12\x45\n\x0f\x63ollection_type\x18\x03 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeH\x00R\x0e\x63ollectionType\x12\x42\n\x0emap_value_type\x18\x04 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeH\x00R\x0cmapValueType\x12-\n\x04\x62lob\x18\x05 \x01(\x0b\x32\x17.flyteidl.core.BlobTypeH\x00R\x04\x62lob\x12\x36\n\tenum_type\x18\x07 \x01(\x0b\x32\x17.flyteidl.core.EnumTypeH\x00R\x08\x65numType\x12^\n\x17structured_dataset_type\x18\x08 \x01(\x0b\x32$.flyteidl.core.StructuredDatasetTypeH\x00R\x15structuredDatasetType\x12\x39\n\nunion_type\x18\n \x01(\x0b\x32\x18.flyteidl.core.UnionTypeH\x00R\tunionType\x12\x33\n\x08metadata\x18\x06 \x01(\x0b\x32\x17.google.protobuf.StructR\x08metadata\x12=\n\nannotation\x18\t \x01(\x0b\x32\x1d.flyteidl.core.TypeAnnotationR\nannotation\x12:\n\tstructure\x18\x0b \x01(\x0b\x32\x1c.flyteidl.core.TypeStructureR\tstructureB\x06\n\x04type\"<\n\x0fOutputReference\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x10\n\x03var\x18\x02 \x01(\tR\x03var\"G\n\x05\x45rror\x12$\n\x0e\x66\x61iled_node_id\x18\x01 \x01(\tR\x0c\x66\x61iledNodeId\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message*\x86\x01\n\nSimpleType\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07INTEGER\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\n\n\x06STRING\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05\x12\x0c\n\x08\x44URATION\x10\x06\x12\n\n\x06\x42INARY\x10\x07\x12\t\n\x05\x45RROR\x10\x08\x12\n\n\x06STRUCT\x10\tB\xaa\x01\n\x11\x63om.flyteidl.coreB\nTypesProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.literals_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.types_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\rLiteralsProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _LITERALMAP_LITERALSENTRY._options = None
-  _LITERALMAP_LITERALSENTRY._serialized_options = b'8\001'
-  _BINDINGDATAMAP_BINDINGSENTRY._options = None
-  _BINDINGDATAMAP_BINDINGSENTRY._serialized_options = b'8\001'
-  _PRIMITIVE._serialized_start=170
-  _PRIMITIVE._serialized_end=433
-  _VOID._serialized_start=435
-  _VOID._serialized_end=441
-  _BLOB._serialized_start=443
-  _BLOB._serialized_end=524
-  _BLOBMETADATA._serialized_start=526
-  _BLOBMETADATA._serialized_end=585
-  _BINARY._serialized_start=587
-  _BINARY._serialized_end=635
-  _SCHEMA._serialized_start=637
-  _SCHEMA._serialized_end=710
-  _UNION._serialized_start=712
-  _UNION._serialized_end=813
-  _STRUCTUREDDATASETMETADATA._serialized_start=815
-  _STRUCTUREDDATASETMETADATA._serialized_end=936
-  _STRUCTUREDDATASET._serialized_start=938
-  _STRUCTUREDDATASET._serialized_end=1045
-  _SCALAR._serialized_start=1048
-  _SCALAR._serialized_end=1544
-  _LITERAL._serialized_start=1547
-  _LITERAL._serialized_end=1749
-  _LITERALCOLLECTION._serialized_start=1751
-  _LITERALCOLLECTION._serialized_end=1822
-  _LITERALMAP._serialized_start=1825
-  _LITERALMAP._serialized_end=1991
-  _LITERALMAP_LITERALSENTRY._serialized_start=1908
-  _LITERALMAP_LITERALSENTRY._serialized_end=1991
-  _BINDINGDATACOLLECTION._serialized_start=1993
-  _BINDINGDATACOLLECTION._serialized_end=2072
-  _BINDINGDATAMAP._serialized_start=2075
-  _BINDINGDATAMAP._serialized_end=2253
-  _BINDINGDATAMAP_BINDINGSENTRY._serialized_start=2166
-  _BINDINGDATAMAP_BINDINGSENTRY._serialized_end=2253
-  _UNIONINFO._serialized_start=2255
-  _UNIONINFO._serialized_end=2326
-  _BINDINGDATA._serialized_start=2329
-  _BINDINGDATA._serialized_end=2631
-  _BINDING._serialized_start=2633
-  _BINDING._serialized_end=2714
-  _KEYVALUEPAIR._serialized_start=2716
-  _KEYVALUEPAIR._serialized_end=2770
-  _RETRYSTRATEGY._serialized_start=2772
-  _RETRYSTRATEGY._serialized_end=2813
+  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\nTypesProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
+  _globals['_SIMPLETYPE']._serialized_start=1922
+  _globals['_SIMPLETYPE']._serialized_end=2056
+  _globals['_SCHEMATYPE']._serialized_start=75
+  _globals['_SCHEMATYPE']._serialized_end=364
+  _globals['_SCHEMATYPE_SCHEMACOLUMN']._serialized_start=156
+  _globals['_SCHEMATYPE_SCHEMACOLUMN']._serialized_end=364
+  _globals['_SCHEMATYPE_SCHEMACOLUMN_SCHEMACOLUMNTYPE']._serialized_start=269
+  _globals['_SCHEMATYPE_SCHEMACOLUMN_SCHEMACOLUMNTYPE']._serialized_end=364
+  _globals['_STRUCTUREDDATASETTYPE']._serialized_start=367
+  _globals['_STRUCTUREDDATASETTYPE']._serialized_end=694
+  _globals['_STRUCTUREDDATASETTYPE_DATASETCOLUMN']._serialized_start=596
+  _globals['_STRUCTUREDDATASETTYPE_DATASETCOLUMN']._serialized_end=694
+  _globals['_BLOBTYPE']._serialized_start=697
+  _globals['_BLOBTYPE']._serialized_end=864
+  _globals['_BLOBTYPE_BLOBDIMENSIONALITY']._serialized_start=817
+  _globals['_BLOBTYPE_BLOBDIMENSIONALITY']._serialized_end=864
+  _globals['_ENUMTYPE']._serialized_start=866
+  _globals['_ENUMTYPE']._serialized_end=900
+  _globals['_UNIONTYPE']._serialized_start=902
+  _globals['_UNIONTYPE']._serialized_end=969
+  _globals['_TYPESTRUCTURE']._serialized_start=971
+  _globals['_TYPESTRUCTURE']._serialized_end=1004
+  _globals['_TYPEANNOTATION']._serialized_start=1006
+  _globals['_TYPEANNOTATION']._serialized_end=1081
+  _globals['_LITERALTYPE']._serialized_start=1084
+  _globals['_LITERALTYPE']._serialized_end=1784
+  _globals['_OUTPUTREFERENCE']._serialized_start=1786
+  _globals['_OUTPUTREFERENCE']._serialized_end=1846
+  _globals['_ERROR']._serialized_start=1848
+  _globals['_ERROR']._serialized_end=1919
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/literals_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/literals_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,62 +5,33 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Binary(_message.Message):
-    __slots__ = ["tag", "value"]
-    TAG_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    tag: str
-    value: bytes
-    def __init__(self, value: _Optional[bytes] = ..., tag: _Optional[str] = ...) -> None: ...
-
-class Binding(_message.Message):
-    __slots__ = ["binding", "var"]
-    BINDING_FIELD_NUMBER: _ClassVar[int]
-    VAR_FIELD_NUMBER: _ClassVar[int]
-    binding: BindingData
-    var: str
-    def __init__(self, var: _Optional[str] = ..., binding: _Optional[_Union[BindingData, _Mapping]] = ...) -> None: ...
-
-class BindingData(_message.Message):
-    __slots__ = ["collection", "map", "promise", "scalar", "union"]
-    COLLECTION_FIELD_NUMBER: _ClassVar[int]
-    MAP_FIELD_NUMBER: _ClassVar[int]
-    PROMISE_FIELD_NUMBER: _ClassVar[int]
-    SCALAR_FIELD_NUMBER: _ClassVar[int]
-    UNION_FIELD_NUMBER: _ClassVar[int]
-    collection: BindingDataCollection
-    map: BindingDataMap
-    promise: _types_pb2.OutputReference
-    scalar: Scalar
-    union: UnionInfo
-    def __init__(self, scalar: _Optional[_Union[Scalar, _Mapping]] = ..., collection: _Optional[_Union[BindingDataCollection, _Mapping]] = ..., promise: _Optional[_Union[_types_pb2.OutputReference, _Mapping]] = ..., map: _Optional[_Union[BindingDataMap, _Mapping]] = ..., union: _Optional[_Union[UnionInfo, _Mapping]] = ...) -> None: ...
-
-class BindingDataCollection(_message.Message):
-    __slots__ = ["bindings"]
-    BINDINGS_FIELD_NUMBER: _ClassVar[int]
-    bindings: _containers.RepeatedCompositeFieldContainer[BindingData]
-    def __init__(self, bindings: _Optional[_Iterable[_Union[BindingData, _Mapping]]] = ...) -> None: ...
+class Primitive(_message.Message):
+    __slots__ = ["integer", "float_value", "string_value", "boolean", "datetime", "duration"]
+    INTEGER_FIELD_NUMBER: _ClassVar[int]
+    FLOAT_VALUE_FIELD_NUMBER: _ClassVar[int]
+    STRING_VALUE_FIELD_NUMBER: _ClassVar[int]
+    BOOLEAN_FIELD_NUMBER: _ClassVar[int]
+    DATETIME_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
+    integer: int
+    float_value: float
+    string_value: str
+    boolean: bool
+    datetime: _timestamp_pb2.Timestamp
+    duration: _duration_pb2.Duration
+    def __init__(self, integer: _Optional[int] = ..., float_value: _Optional[float] = ..., string_value: _Optional[str] = ..., boolean: bool = ..., datetime: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
 
-class BindingDataMap(_message.Message):
-    __slots__ = ["bindings"]
-    class BindingsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: BindingData
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[BindingData, _Mapping]] = ...) -> None: ...
-    BINDINGS_FIELD_NUMBER: _ClassVar[int]
-    bindings: _containers.MessageMap[str, BindingData]
-    def __init__(self, bindings: _Optional[_Mapping[str, BindingData]] = ...) -> None: ...
+class Void(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
 class Blob(_message.Message):
     __slots__ = ["metadata", "uri"]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     URI_FIELD_NUMBER: _ClassVar[int]
     metadata: BlobMetadata
     uri: str
@@ -68,32 +39,84 @@
 
 class BlobMetadata(_message.Message):
     __slots__ = ["type"]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     type: _types_pb2.BlobType
     def __init__(self, type: _Optional[_Union[_types_pb2.BlobType, _Mapping]] = ...) -> None: ...
 
-class KeyValuePair(_message.Message):
-    __slots__ = ["key", "value"]
-    KEY_FIELD_NUMBER: _ClassVar[int]
+class Binary(_message.Message):
+    __slots__ = ["value", "tag"]
     VALUE_FIELD_NUMBER: _ClassVar[int]
-    key: str
-    value: str
-    def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    TAG_FIELD_NUMBER: _ClassVar[int]
+    value: bytes
+    tag: str
+    def __init__(self, value: _Optional[bytes] = ..., tag: _Optional[str] = ...) -> None: ...
+
+class Schema(_message.Message):
+    __slots__ = ["uri", "type"]
+    URI_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    uri: str
+    type: _types_pb2.SchemaType
+    def __init__(self, uri: _Optional[str] = ..., type: _Optional[_Union[_types_pb2.SchemaType, _Mapping]] = ...) -> None: ...
+
+class Union(_message.Message):
+    __slots__ = ["value", "type"]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    value: Literal
+    type: _types_pb2.LiteralType
+    def __init__(self, value: _Optional[_Union[Literal, _Mapping]] = ..., type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ...) -> None: ...
+
+class StructuredDatasetMetadata(_message.Message):
+    __slots__ = ["structured_dataset_type"]
+    STRUCTURED_DATASET_TYPE_FIELD_NUMBER: _ClassVar[int]
+    structured_dataset_type: _types_pb2.StructuredDatasetType
+    def __init__(self, structured_dataset_type: _Optional[_Union[_types_pb2.StructuredDatasetType, _Mapping]] = ...) -> None: ...
+
+class StructuredDataset(_message.Message):
+    __slots__ = ["uri", "metadata"]
+    URI_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    uri: str
+    metadata: StructuredDatasetMetadata
+    def __init__(self, uri: _Optional[str] = ..., metadata: _Optional[_Union[StructuredDatasetMetadata, _Mapping]] = ...) -> None: ...
+
+class Scalar(_message.Message):
+    __slots__ = ["primitive", "blob", "binary", "schema", "none_type", "error", "generic", "structured_dataset", "union"]
+    PRIMITIVE_FIELD_NUMBER: _ClassVar[int]
+    BLOB_FIELD_NUMBER: _ClassVar[int]
+    BINARY_FIELD_NUMBER: _ClassVar[int]
+    SCHEMA_FIELD_NUMBER: _ClassVar[int]
+    NONE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    GENERIC_FIELD_NUMBER: _ClassVar[int]
+    STRUCTURED_DATASET_FIELD_NUMBER: _ClassVar[int]
+    UNION_FIELD_NUMBER: _ClassVar[int]
+    primitive: Primitive
+    blob: Blob
+    binary: Binary
+    schema: Schema
+    none_type: Void
+    error: _types_pb2.Error
+    generic: _struct_pb2.Struct
+    structured_dataset: StructuredDataset
+    union: Union
+    def __init__(self, primitive: _Optional[_Union[Primitive, _Mapping]] = ..., blob: _Optional[_Union[Blob, _Mapping]] = ..., binary: _Optional[_Union[Binary, _Mapping]] = ..., schema: _Optional[_Union[Schema, _Mapping]] = ..., none_type: _Optional[_Union[Void, _Mapping]] = ..., error: _Optional[_Union[_types_pb2.Error, _Mapping]] = ..., generic: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., structured_dataset: _Optional[_Union[StructuredDataset, _Mapping]] = ..., union: _Optional[_Union[Union, _Mapping]] = ...) -> None: ...
 
 class Literal(_message.Message):
-    __slots__ = ["collection", "hash", "map", "scalar"]
+    __slots__ = ["scalar", "collection", "map", "hash"]
+    SCALAR_FIELD_NUMBER: _ClassVar[int]
     COLLECTION_FIELD_NUMBER: _ClassVar[int]
-    HASH_FIELD_NUMBER: _ClassVar[int]
     MAP_FIELD_NUMBER: _ClassVar[int]
-    SCALAR_FIELD_NUMBER: _ClassVar[int]
+    HASH_FIELD_NUMBER: _ClassVar[int]
+    scalar: Scalar
     collection: LiteralCollection
-    hash: str
     map: LiteralMap
-    scalar: Scalar
+    hash: str
     def __init__(self, scalar: _Optional[_Union[Scalar, _Mapping]] = ..., collection: _Optional[_Union[LiteralCollection, _Mapping]] = ..., map: _Optional[_Union[LiteralMap, _Mapping]] = ..., hash: _Optional[str] = ...) -> None: ...
 
 class LiteralCollection(_message.Message):
     __slots__ = ["literals"]
     LITERALS_FIELD_NUMBER: _ClassVar[int]
     literals: _containers.RepeatedCompositeFieldContainer[Literal]
     def __init__(self, literals: _Optional[_Iterable[_Union[Literal, _Mapping]]] = ...) -> None: ...
@@ -107,90 +130,67 @@
         key: str
         value: Literal
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[Literal, _Mapping]] = ...) -> None: ...
     LITERALS_FIELD_NUMBER: _ClassVar[int]
     literals: _containers.MessageMap[str, Literal]
     def __init__(self, literals: _Optional[_Mapping[str, Literal]] = ...) -> None: ...
 
-class Primitive(_message.Message):
-    __slots__ = ["boolean", "datetime", "duration", "float_value", "integer", "string_value"]
-    BOOLEAN_FIELD_NUMBER: _ClassVar[int]
-    DATETIME_FIELD_NUMBER: _ClassVar[int]
-    DURATION_FIELD_NUMBER: _ClassVar[int]
-    FLOAT_VALUE_FIELD_NUMBER: _ClassVar[int]
-    INTEGER_FIELD_NUMBER: _ClassVar[int]
-    STRING_VALUE_FIELD_NUMBER: _ClassVar[int]
-    boolean: bool
-    datetime: _timestamp_pb2.Timestamp
-    duration: _duration_pb2.Duration
-    float_value: float
-    integer: int
-    string_value: str
-    def __init__(self, integer: _Optional[int] = ..., float_value: _Optional[float] = ..., string_value: _Optional[str] = ..., boolean: bool = ..., datetime: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
-
-class RetryStrategy(_message.Message):
-    __slots__ = ["retries"]
-    RETRIES_FIELD_NUMBER: _ClassVar[int]
-    retries: int
-    def __init__(self, retries: _Optional[int] = ...) -> None: ...
-
-class Scalar(_message.Message):
-    __slots__ = ["binary", "blob", "error", "generic", "none_type", "primitive", "schema", "structured_dataset", "union"]
-    BINARY_FIELD_NUMBER: _ClassVar[int]
-    BLOB_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    GENERIC_FIELD_NUMBER: _ClassVar[int]
-    NONE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    PRIMITIVE_FIELD_NUMBER: _ClassVar[int]
-    SCHEMA_FIELD_NUMBER: _ClassVar[int]
-    STRUCTURED_DATASET_FIELD_NUMBER: _ClassVar[int]
-    UNION_FIELD_NUMBER: _ClassVar[int]
-    binary: Binary
-    blob: Blob
-    error: _types_pb2.Error
-    generic: _struct_pb2.Struct
-    none_type: Void
-    primitive: Primitive
-    schema: Schema
-    structured_dataset: StructuredDataset
-    union: Union
-    def __init__(self, primitive: _Optional[_Union[Primitive, _Mapping]] = ..., blob: _Optional[_Union[Blob, _Mapping]] = ..., binary: _Optional[_Union[Binary, _Mapping]] = ..., schema: _Optional[_Union[Schema, _Mapping]] = ..., none_type: _Optional[_Union[Void, _Mapping]] = ..., error: _Optional[_Union[_types_pb2.Error, _Mapping]] = ..., generic: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., structured_dataset: _Optional[_Union[StructuredDataset, _Mapping]] = ..., union: _Optional[_Union[Union, _Mapping]] = ...) -> None: ...
-
-class Schema(_message.Message):
-    __slots__ = ["type", "uri"]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    URI_FIELD_NUMBER: _ClassVar[int]
-    type: _types_pb2.SchemaType
-    uri: str
-    def __init__(self, uri: _Optional[str] = ..., type: _Optional[_Union[_types_pb2.SchemaType, _Mapping]] = ...) -> None: ...
-
-class StructuredDataset(_message.Message):
-    __slots__ = ["metadata", "uri"]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    URI_FIELD_NUMBER: _ClassVar[int]
-    metadata: StructuredDatasetMetadata
-    uri: str
-    def __init__(self, uri: _Optional[str] = ..., metadata: _Optional[_Union[StructuredDatasetMetadata, _Mapping]] = ...) -> None: ...
-
-class StructuredDatasetMetadata(_message.Message):
-    __slots__ = ["structured_dataset_type"]
-    STRUCTURED_DATASET_TYPE_FIELD_NUMBER: _ClassVar[int]
-    structured_dataset_type: _types_pb2.StructuredDatasetType
-    def __init__(self, structured_dataset_type: _Optional[_Union[_types_pb2.StructuredDatasetType, _Mapping]] = ...) -> None: ...
+class BindingDataCollection(_message.Message):
+    __slots__ = ["bindings"]
+    BINDINGS_FIELD_NUMBER: _ClassVar[int]
+    bindings: _containers.RepeatedCompositeFieldContainer[BindingData]
+    def __init__(self, bindings: _Optional[_Iterable[_Union[BindingData, _Mapping]]] = ...) -> None: ...
 
-class Union(_message.Message):
-    __slots__ = ["type", "value"]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    type: _types_pb2.LiteralType
-    value: Literal
-    def __init__(self, value: _Optional[_Union[Literal, _Mapping]] = ..., type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ...) -> None: ...
+class BindingDataMap(_message.Message):
+    __slots__ = ["bindings"]
+    class BindingsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: BindingData
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[BindingData, _Mapping]] = ...) -> None: ...
+    BINDINGS_FIELD_NUMBER: _ClassVar[int]
+    bindings: _containers.MessageMap[str, BindingData]
+    def __init__(self, bindings: _Optional[_Mapping[str, BindingData]] = ...) -> None: ...
 
 class UnionInfo(_message.Message):
     __slots__ = ["targetType"]
     TARGETTYPE_FIELD_NUMBER: _ClassVar[int]
     targetType: _types_pb2.LiteralType
     def __init__(self, targetType: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ...) -> None: ...
 
-class Void(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+class BindingData(_message.Message):
+    __slots__ = ["scalar", "collection", "promise", "map", "union"]
+    SCALAR_FIELD_NUMBER: _ClassVar[int]
+    COLLECTION_FIELD_NUMBER: _ClassVar[int]
+    PROMISE_FIELD_NUMBER: _ClassVar[int]
+    MAP_FIELD_NUMBER: _ClassVar[int]
+    UNION_FIELD_NUMBER: _ClassVar[int]
+    scalar: Scalar
+    collection: BindingDataCollection
+    promise: _types_pb2.OutputReference
+    map: BindingDataMap
+    union: UnionInfo
+    def __init__(self, scalar: _Optional[_Union[Scalar, _Mapping]] = ..., collection: _Optional[_Union[BindingDataCollection, _Mapping]] = ..., promise: _Optional[_Union[_types_pb2.OutputReference, _Mapping]] = ..., map: _Optional[_Union[BindingDataMap, _Mapping]] = ..., union: _Optional[_Union[UnionInfo, _Mapping]] = ...) -> None: ...
+
+class Binding(_message.Message):
+    __slots__ = ["var", "binding"]
+    VAR_FIELD_NUMBER: _ClassVar[int]
+    BINDING_FIELD_NUMBER: _ClassVar[int]
+    var: str
+    binding: BindingData
+    def __init__(self, var: _Optional[str] = ..., binding: _Optional[_Union[BindingData, _Mapping]] = ...) -> None: ...
+
+class KeyValuePair(_message.Message):
+    __slots__ = ["key", "value"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    key: str
+    value: str
+    def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+
+class RetryStrategy(_message.Message):
+    __slots__ = ["retries"]
+    RETRIES_FIELD_NUMBER: _ClassVar[int]
+    retries: int
+    def __init__(self, retries: _Optional[int] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/security_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/signal_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/core/security.proto
+# source: flyteidl/service/signal.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from flyteidl.admin import signal_pb2 as flyteidl_dot_admin_dot_signal__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/core/security.proto\x12\rflyteidl.core\"\xd0\x01\n\x06Secret\x12\x14\n\x05group\x18\x01 \x01(\tR\x05group\x12#\n\rgroup_version\x18\x02 \x01(\tR\x0cgroupVersion\x12\x10\n\x03key\x18\x03 \x01(\tR\x03key\x12L\n\x11mount_requirement\x18\x04 \x01(\x0e\x32\x1f.flyteidl.core.Secret.MountTypeR\x10mountRequirement\"+\n\tMountType\x12\x07\n\x03\x41NY\x10\x00\x12\x0b\n\x07\x45NV_VAR\x10\x01\x12\x08\n\x04\x46ILE\x10\x02\"g\n\x0cOAuth2Client\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12:\n\rclient_secret\x18\x02 \x01(\x0b\x32\x15.flyteidl.core.SecretR\x0c\x63lientSecret\"\x97\x01\n\x08Identity\x12\x19\n\x08iam_role\x18\x01 \x01(\tR\x07iamRole\x12.\n\x13k8s_service_account\x18\x02 \x01(\tR\x11k8sServiceAccount\x12@\n\roauth2_client\x18\x03 \x01(\x0b\x32\x1b.flyteidl.core.OAuth2ClientR\x0coauth2Client\"\x96\x02\n\x12OAuth2TokenRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12:\n\x04type\x18\x02 \x01(\x0e\x32&.flyteidl.core.OAuth2TokenRequest.TypeR\x04type\x12\x33\n\x06\x63lient\x18\x03 \x01(\x0b\x32\x1b.flyteidl.core.OAuth2ClientR\x06\x63lient\x12\x34\n\x16idp_discovery_endpoint\x18\x04 \x01(\tR\x14idpDiscoveryEndpoint\x12%\n\x0etoken_endpoint\x18\x05 \x01(\tR\rtokenEndpoint\"\x1e\n\x04Type\x12\x16\n\x12\x43LIENT_CREDENTIALS\x10\x00\"\xad\x01\n\x0fSecurityContext\x12.\n\x06run_as\x18\x01 \x01(\x0b\x32\x17.flyteidl.core.IdentityR\x05runAs\x12/\n\x07secrets\x18\x02 \x03(\x0b\x32\x15.flyteidl.core.SecretR\x07secrets\x12\x39\n\x06tokens\x18\x03 \x03(\x0b\x32!.flyteidl.core.OAuth2TokenRequestR\x06tokensB\xad\x01\n\x11\x63om.flyteidl.coreB\rSecurityProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/service/signal.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1b\x66lyteidl/admin/signal.proto2\x9a\x03\n\rSignalService\x12W\n\x11GetOrCreateSignal\x12(.flyteidl.admin.SignalGetOrCreateRequest\x1a\x16.flyteidl.admin.Signal\"\x00\x12\xc1\x01\n\x0bListSignals\x12!.flyteidl.admin.SignalListRequest\x1a\x1a.flyteidl.admin.SignalList\"s\x82\xd3\xe4\x93\x02m\x12k/api/v1/signals/{workflow_execution_id.project}/{workflow_execution_id.domain}/{workflow_execution_id.name}\x12l\n\tSetSignal\x12 .flyteidl.admin.SignalSetRequest\x1a!.flyteidl.admin.SignalSetResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/api/v1/signalsB\xbd\x01\n\x14\x63om.flyteidl.serviceB\x0bSignalProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.security_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.signal_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\rSecurityProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _SECRET._serialized_start=48
-  _SECRET._serialized_end=256
-  _SECRET_MOUNTTYPE._serialized_start=213
-  _SECRET_MOUNTTYPE._serialized_end=256
-  _OAUTH2CLIENT._serialized_start=258
-  _OAUTH2CLIENT._serialized_end=361
-  _IDENTITY._serialized_start=364
-  _IDENTITY._serialized_end=515
-  _OAUTH2TOKENREQUEST._serialized_start=518
-  _OAUTH2TOKENREQUEST._serialized_end=796
-  _OAUTH2TOKENREQUEST_TYPE._serialized_start=766
-  _OAUTH2TOKENREQUEST_TYPE._serialized_end=796
-  _SECURITYCONTEXT._serialized_start=799
-  _SECURITYCONTEXT._serialized_end=972
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.serviceB\013SignalProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\242\002\003FSX\252\002\020Flyteidl.Service\312\002\020Flyteidl\\Service\342\002\034Flyteidl\\Service\\GPBMetadata\352\002\021Flyteidl::Service'
+  _SIGNALSERVICE.methods_by_name['ListSignals']._options = None
+  _SIGNALSERVICE.methods_by_name['ListSignals']._serialized_options = b'\202\323\344\223\002m\022k/api/v1/signals/{workflow_execution_id.project}/{workflow_execution_id.domain}/{workflow_execution_id.name}'
+  _SIGNALSERVICE.methods_by_name['SetSignal']._options = None
+  _SIGNALSERVICE.methods_by_name['SetSignal']._serialized_options = b'\202\323\344\223\002\024:\001*\"\017/api/v1/signals'
+  _globals['_SIGNALSERVICE']._serialized_start=111
+  _globals['_SIGNALSERVICE']._serialized_end=521
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/security_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/security_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,66 +2,70 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class Secret(_message.Message):
+    __slots__ = ["group", "group_version", "key", "mount_requirement"]
+    class MountType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        ANY: _ClassVar[Secret.MountType]
+        ENV_VAR: _ClassVar[Secret.MountType]
+        FILE: _ClassVar[Secret.MountType]
+    ANY: Secret.MountType
+    ENV_VAR: Secret.MountType
+    FILE: Secret.MountType
+    GROUP_FIELD_NUMBER: _ClassVar[int]
+    GROUP_VERSION_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    MOUNT_REQUIREMENT_FIELD_NUMBER: _ClassVar[int]
+    group: str
+    group_version: str
+    key: str
+    mount_requirement: Secret.MountType
+    def __init__(self, group: _Optional[str] = ..., group_version: _Optional[str] = ..., key: _Optional[str] = ..., mount_requirement: _Optional[_Union[Secret.MountType, str]] = ...) -> None: ...
+
+class OAuth2Client(_message.Message):
+    __slots__ = ["client_id", "client_secret"]
+    CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
+    CLIENT_SECRET_FIELD_NUMBER: _ClassVar[int]
+    client_id: str
+    client_secret: Secret
+    def __init__(self, client_id: _Optional[str] = ..., client_secret: _Optional[_Union[Secret, _Mapping]] = ...) -> None: ...
+
 class Identity(_message.Message):
     __slots__ = ["iam_role", "k8s_service_account", "oauth2_client"]
     IAM_ROLE_FIELD_NUMBER: _ClassVar[int]
     K8S_SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
     OAUTH2_CLIENT_FIELD_NUMBER: _ClassVar[int]
     iam_role: str
     k8s_service_account: str
     oauth2_client: OAuth2Client
     def __init__(self, iam_role: _Optional[str] = ..., k8s_service_account: _Optional[str] = ..., oauth2_client: _Optional[_Union[OAuth2Client, _Mapping]] = ...) -> None: ...
 
-class OAuth2Client(_message.Message):
-    __slots__ = ["client_id", "client_secret"]
-    CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
-    CLIENT_SECRET_FIELD_NUMBER: _ClassVar[int]
-    client_id: str
-    client_secret: Secret
-    def __init__(self, client_id: _Optional[str] = ..., client_secret: _Optional[_Union[Secret, _Mapping]] = ...) -> None: ...
-
 class OAuth2TokenRequest(_message.Message):
-    __slots__ = ["client", "idp_discovery_endpoint", "name", "token_endpoint", "type"]
+    __slots__ = ["name", "type", "client", "idp_discovery_endpoint", "token_endpoint"]
     class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        CLIENT_CREDENTIALS: _ClassVar[OAuth2TokenRequest.Type]
     CLIENT_CREDENTIALS: OAuth2TokenRequest.Type
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
     CLIENT_FIELD_NUMBER: _ClassVar[int]
     IDP_DISCOVERY_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    type: OAuth2TokenRequest.Type
     client: OAuth2Client
     idp_discovery_endpoint: str
-    name: str
     token_endpoint: str
-    type: OAuth2TokenRequest.Type
     def __init__(self, name: _Optional[str] = ..., type: _Optional[_Union[OAuth2TokenRequest.Type, str]] = ..., client: _Optional[_Union[OAuth2Client, _Mapping]] = ..., idp_discovery_endpoint: _Optional[str] = ..., token_endpoint: _Optional[str] = ...) -> None: ...
 
-class Secret(_message.Message):
-    __slots__ = ["group", "group_version", "key", "mount_requirement"]
-    class MountType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    ANY: Secret.MountType
-    ENV_VAR: Secret.MountType
-    FILE: Secret.MountType
-    GROUP_FIELD_NUMBER: _ClassVar[int]
-    GROUP_VERSION_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    MOUNT_REQUIREMENT_FIELD_NUMBER: _ClassVar[int]
-    group: str
-    group_version: str
-    key: str
-    mount_requirement: Secret.MountType
-    def __init__(self, group: _Optional[str] = ..., group_version: _Optional[str] = ..., key: _Optional[str] = ..., mount_requirement: _Optional[_Union[Secret.MountType, str]] = ...) -> None: ...
-
 class SecurityContext(_message.Message):
     __slots__ = ["run_as", "secrets", "tokens"]
     RUN_AS_FIELD_NUMBER: _ClassVar[int]
     SECRETS_FIELD_NUMBER: _ClassVar[int]
     TOKENS_FIELD_NUMBER: _ClassVar[int]
     run_as: Identity
     secrets: _containers.RepeatedCompositeFieldContainer[Secret]
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/tasks_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/tasks_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,72 +15,73 @@
 from flyteidl.core import interface_pb2 as flyteidl_dot_core_dot_interface__pb2
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 from flyteidl.core import security_pb2 as flyteidl_dot_core_dot_security__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66lyteidl/core/tasks.proto\x12\rflyteidl.core\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1d\x66lyteidl/core/interface.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1c\x66lyteidl/core/security.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xd0\x02\n\tResources\x12\x42\n\x08requests\x18\x01 \x03(\x0b\x32&.flyteidl.core.Resources.ResourceEntryR\x08requests\x12>\n\x06limits\x18\x02 \x03(\x0b\x32&.flyteidl.core.Resources.ResourceEntryR\x06limits\x1a`\n\rResourceEntry\x12\x39\n\x04name\x18\x01 \x01(\x0e\x32%.flyteidl.core.Resources.ResourceNameR\x04name\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"]\n\x0cResourceName\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x12\n\n\x06MEMORY\x10\x03\x12\x0b\n\x07STORAGE\x10\x04\x12\x15\n\x11\x45PHEMERAL_STORAGE\x10\x05\"\xac\x01\n\x0fRuntimeMetadata\x12>\n\x04type\x18\x01 \x01(\x0e\x32*.flyteidl.core.RuntimeMetadata.RuntimeTypeR\x04type\x12\x18\n\x07version\x18\x02 \x01(\tR\x07version\x12\x16\n\x06\x66lavor\x18\x03 \x01(\tR\x06\x66lavor\"\'\n\x0bRuntimeType\x12\t\n\x05OTHER\x10\x00\x12\r\n\tFLYTE_SDK\x10\x01\"\xc9\x04\n\x0cTaskMetadata\x12\"\n\x0c\x64iscoverable\x18\x01 \x01(\x08R\x0c\x64iscoverable\x12\x38\n\x07runtime\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.RuntimeMetadataR\x07runtime\x12\x33\n\x07timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x07timeout\x12\x36\n\x07retries\x18\x05 \x01(\x0b\x32\x1c.flyteidl.core.RetryStrategyR\x07retries\x12+\n\x11\x64iscovery_version\x18\x06 \x01(\tR\x10\x64iscoveryVersion\x12\x38\n\x18\x64\x65precated_error_message\x18\x07 \x01(\tR\x16\x64\x65precatedErrorMessage\x12&\n\rinterruptible\x18\x08 \x01(\x08H\x00R\rinterruptible\x12-\n\x12\x63\x61\x63he_serializable\x18\t \x01(\x08R\x11\x63\x61\x63heSerializable\x12%\n\x0egenerates_deck\x18\n \x01(\x08R\rgeneratesDeck\x12\x39\n\x04tags\x18\x0b \x03(\x0b\x32%.flyteidl.core.TaskMetadata.TagsEntryR\x04tags\x1a\x37\n\tTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x15\n\x13interruptible_value\"\x85\x05\n\x0cTaskTemplate\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x37\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.flyteidl.core.TaskMetadataR\x08metadata\x12;\n\tinterface\x18\x04 \x01(\x0b\x32\x1d.flyteidl.core.TypedInterfaceR\tinterface\x12/\n\x06\x63ustom\x18\x05 \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x63ustom\x12\x38\n\tcontainer\x18\x06 \x01(\x0b\x32\x18.flyteidl.core.ContainerH\x00R\tcontainer\x12\x30\n\x07k8s_pod\x18\x11 \x01(\x0b\x32\x15.flyteidl.core.K8sPodH\x00R\x06k8sPod\x12&\n\x03sql\x18\x12 \x01(\x0b\x32\x12.flyteidl.core.SqlH\x00R\x03sql\x12*\n\x11task_type_version\x18\x07 \x01(\x05R\x0ftaskTypeVersion\x12I\n\x10security_context\x18\x08 \x01(\x0b\x32\x1e.flyteidl.core.SecurityContextR\x0fsecurityContext\x12?\n\x06\x63onfig\x18\x10 \x03(\x0b\x32\'.flyteidl.core.TaskTemplate.ConfigEntryR\x06\x63onfig\x1a\x39\n\x0b\x43onfigEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x08\n\x06target\"6\n\rContainerPort\x12%\n\x0e\x63ontainer_port\x18\x01 \x01(\rR\rcontainerPort\"\xfc\x03\n\tContainer\x12\x14\n\x05image\x18\x01 \x01(\tR\x05image\x12\x18\n\x07\x63ommand\x18\x02 \x03(\tR\x07\x63ommand\x12\x12\n\x04\x61rgs\x18\x03 \x03(\tR\x04\x61rgs\x12\x36\n\tresources\x18\x04 \x01(\x0b\x32\x18.flyteidl.core.ResourcesR\tresources\x12-\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1b.flyteidl.core.KeyValuePairR\x03\x65nv\x12\x37\n\x06\x63onfig\x18\x06 \x03(\x0b\x32\x1b.flyteidl.core.KeyValuePairB\x02\x18\x01R\x06\x63onfig\x12\x32\n\x05ports\x18\x07 \x03(\x0b\x32\x1c.flyteidl.core.ContainerPortR\x05ports\x12\x41\n\x0b\x64\x61ta_config\x18\t \x01(\x0b\x32 .flyteidl.core.DataLoadingConfigR\ndataConfig\x12I\n\x0c\x61rchitecture\x18\n \x01(\x0e\x32%.flyteidl.core.Container.ArchitectureR\x0c\x61rchitecture\"I\n\x0c\x41rchitecture\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x41MD64\x10\x01\x12\t\n\x05\x41RM64\x10\x02\x12\n\n\x06\x41RM_V6\x10\x03\x12\n\n\x06\x41RM_V7\x10\x04\"\xb5\x02\n\nIOStrategy\x12K\n\rdownload_mode\x18\x01 \x01(\x0e\x32&.flyteidl.core.IOStrategy.DownloadModeR\x0c\x64ownloadMode\x12\x45\n\x0bupload_mode\x18\x02 \x01(\x0e\x32$.flyteidl.core.IOStrategy.UploadModeR\nuploadMode\"L\n\x0c\x44ownloadMode\x12\x12\n\x0e\x44OWNLOAD_EAGER\x10\x00\x12\x13\n\x0f\x44OWNLOAD_STREAM\x10\x01\x12\x13\n\x0f\x44O_NOT_DOWNLOAD\x10\x02\"E\n\nUploadMode\x12\x12\n\x0eUPLOAD_ON_EXIT\x10\x00\x12\x10\n\x0cUPLOAD_EAGER\x10\x01\x12\x11\n\rDO_NOT_UPLOAD\x10\x02\"\xa7\x02\n\x11\x44\x61taLoadingConfig\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\ninput_path\x18\x02 \x01(\tR\tinputPath\x12\x1f\n\x0boutput_path\x18\x03 \x01(\tR\noutputPath\x12I\n\x06\x66ormat\x18\x04 \x01(\x0e\x32\x31.flyteidl.core.DataLoadingConfig.LiteralMapFormatR\x06\x66ormat\x12:\n\x0bio_strategy\x18\x05 \x01(\x0b\x32\x19.flyteidl.core.IOStrategyR\nioStrategy\"1\n\x10LiteralMapFormat\x12\x08\n\x04JSON\x10\x00\x12\x08\n\x04YAML\x10\x01\x12\t\n\x05PROTO\x10\x02\"z\n\x06K8sPod\x12<\n\x08metadata\x18\x01 \x01(\x0b\x32 .flyteidl.core.K8sObjectMetadataR\x08metadata\x12\x32\n\x08pod_spec\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructR\x07podSpec\"\xa9\x02\n\x11K8sObjectMetadata\x12\x44\n\x06labels\x18\x01 \x03(\x0b\x32,.flyteidl.core.K8sObjectMetadata.LabelsEntryR\x06labels\x12S\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x31.flyteidl.core.K8sObjectMetadata.AnnotationsEntryR\x0b\x61nnotations\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a>\n\x10\x41nnotationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\x92\x01\n\x03Sql\x12\x1c\n\tstatement\x18\x01 \x01(\tR\tstatement\x12\x34\n\x07\x64ialect\x18\x02 \x01(\x0e\x32\x1a.flyteidl.core.Sql.DialectR\x07\x64ialect\"7\n\x07\x44ialect\x12\r\n\tUNDEFINED\x10\x00\x12\x08\n\x04\x41NSI\x10\x01\x12\x08\n\x04HIVE\x10\x02\x12\t\n\x05OTHER\x10\x03\x42\xaa\x01\n\x11\x63om.flyteidl.coreB\nTasksProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66lyteidl/core/tasks.proto\x12\rflyteidl.core\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1d\x66lyteidl/core/interface.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1c\x66lyteidl/core/security.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xd0\x02\n\tResources\x12\x42\n\x08requests\x18\x01 \x03(\x0b\x32&.flyteidl.core.Resources.ResourceEntryR\x08requests\x12>\n\x06limits\x18\x02 \x03(\x0b\x32&.flyteidl.core.Resources.ResourceEntryR\x06limits\x1a`\n\rResourceEntry\x12\x39\n\x04name\x18\x01 \x01(\x0e\x32%.flyteidl.core.Resources.ResourceNameR\x04name\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"]\n\x0cResourceName\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x12\n\n\x06MEMORY\x10\x03\x12\x0b\n\x07STORAGE\x10\x04\x12\x15\n\x11\x45PHEMERAL_STORAGE\x10\x05\"\xac\x01\n\x0fRuntimeMetadata\x12>\n\x04type\x18\x01 \x01(\x0e\x32*.flyteidl.core.RuntimeMetadata.RuntimeTypeR\x04type\x12\x18\n\x07version\x18\x02 \x01(\tR\x07version\x12\x16\n\x06\x66lavor\x18\x03 \x01(\tR\x06\x66lavor\"\'\n\x0bRuntimeType\x12\t\n\x05OTHER\x10\x00\x12\r\n\tFLYTE_SDK\x10\x01\"\xf5\x04\n\x0cTaskMetadata\x12\"\n\x0c\x64iscoverable\x18\x01 \x01(\x08R\x0c\x64iscoverable\x12\x38\n\x07runtime\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.RuntimeMetadataR\x07runtime\x12\x33\n\x07timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x07timeout\x12\x36\n\x07retries\x18\x05 \x01(\x0b\x32\x1c.flyteidl.core.RetryStrategyR\x07retries\x12+\n\x11\x64iscovery_version\x18\x06 \x01(\tR\x10\x64iscoveryVersion\x12\x38\n\x18\x64\x65precated_error_message\x18\x07 \x01(\tR\x16\x64\x65precatedErrorMessage\x12&\n\rinterruptible\x18\x08 \x01(\x08H\x00R\rinterruptible\x12-\n\x12\x63\x61\x63he_serializable\x18\t \x01(\x08R\x11\x63\x61\x63heSerializable\x12%\n\x0egenerates_deck\x18\n \x01(\x08R\rgeneratesDeck\x12\x39\n\x04tags\x18\x0b \x03(\x0b\x32%.flyteidl.core.TaskMetadata.TagsEntryR\x04tags\x12*\n\x11pod_template_name\x18\x0c \x01(\tR\x0fpodTemplateName\x1a\x37\n\tTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x15\n\x13interruptible_value\"\x85\x05\n\x0cTaskTemplate\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x37\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.flyteidl.core.TaskMetadataR\x08metadata\x12;\n\tinterface\x18\x04 \x01(\x0b\x32\x1d.flyteidl.core.TypedInterfaceR\tinterface\x12/\n\x06\x63ustom\x18\x05 \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x63ustom\x12\x38\n\tcontainer\x18\x06 \x01(\x0b\x32\x18.flyteidl.core.ContainerH\x00R\tcontainer\x12\x30\n\x07k8s_pod\x18\x11 \x01(\x0b\x32\x15.flyteidl.core.K8sPodH\x00R\x06k8sPod\x12&\n\x03sql\x18\x12 \x01(\x0b\x32\x12.flyteidl.core.SqlH\x00R\x03sql\x12*\n\x11task_type_version\x18\x07 \x01(\x05R\x0ftaskTypeVersion\x12I\n\x10security_context\x18\x08 \x01(\x0b\x32\x1e.flyteidl.core.SecurityContextR\x0fsecurityContext\x12?\n\x06\x63onfig\x18\x10 \x03(\x0b\x32\'.flyteidl.core.TaskTemplate.ConfigEntryR\x06\x63onfig\x1a\x39\n\x0b\x43onfigEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x08\n\x06target\"6\n\rContainerPort\x12%\n\x0e\x63ontainer_port\x18\x01 \x01(\rR\rcontainerPort\"\xfc\x03\n\tContainer\x12\x14\n\x05image\x18\x01 \x01(\tR\x05image\x12\x18\n\x07\x63ommand\x18\x02 \x03(\tR\x07\x63ommand\x12\x12\n\x04\x61rgs\x18\x03 \x03(\tR\x04\x61rgs\x12\x36\n\tresources\x18\x04 \x01(\x0b\x32\x18.flyteidl.core.ResourcesR\tresources\x12-\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1b.flyteidl.core.KeyValuePairR\x03\x65nv\x12\x37\n\x06\x63onfig\x18\x06 \x03(\x0b\x32\x1b.flyteidl.core.KeyValuePairB\x02\x18\x01R\x06\x63onfig\x12\x32\n\x05ports\x18\x07 \x03(\x0b\x32\x1c.flyteidl.core.ContainerPortR\x05ports\x12\x41\n\x0b\x64\x61ta_config\x18\t \x01(\x0b\x32 .flyteidl.core.DataLoadingConfigR\ndataConfig\x12I\n\x0c\x61rchitecture\x18\n \x01(\x0e\x32%.flyteidl.core.Container.ArchitectureR\x0c\x61rchitecture\"I\n\x0c\x41rchitecture\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x41MD64\x10\x01\x12\t\n\x05\x41RM64\x10\x02\x12\n\n\x06\x41RM_V6\x10\x03\x12\n\n\x06\x41RM_V7\x10\x04\"\xb5\x02\n\nIOStrategy\x12K\n\rdownload_mode\x18\x01 \x01(\x0e\x32&.flyteidl.core.IOStrategy.DownloadModeR\x0c\x64ownloadMode\x12\x45\n\x0bupload_mode\x18\x02 \x01(\x0e\x32$.flyteidl.core.IOStrategy.UploadModeR\nuploadMode\"L\n\x0c\x44ownloadMode\x12\x12\n\x0e\x44OWNLOAD_EAGER\x10\x00\x12\x13\n\x0f\x44OWNLOAD_STREAM\x10\x01\x12\x13\n\x0f\x44O_NOT_DOWNLOAD\x10\x02\"E\n\nUploadMode\x12\x12\n\x0eUPLOAD_ON_EXIT\x10\x00\x12\x10\n\x0cUPLOAD_EAGER\x10\x01\x12\x11\n\rDO_NOT_UPLOAD\x10\x02\"\xa7\x02\n\x11\x44\x61taLoadingConfig\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\ninput_path\x18\x02 \x01(\tR\tinputPath\x12\x1f\n\x0boutput_path\x18\x03 \x01(\tR\noutputPath\x12I\n\x06\x66ormat\x18\x04 \x01(\x0e\x32\x31.flyteidl.core.DataLoadingConfig.LiteralMapFormatR\x06\x66ormat\x12:\n\x0bio_strategy\x18\x05 \x01(\x0b\x32\x19.flyteidl.core.IOStrategyR\nioStrategy\"1\n\x10LiteralMapFormat\x12\x08\n\x04JSON\x10\x00\x12\x08\n\x04YAML\x10\x01\x12\t\n\x05PROTO\x10\x02\"\xbd\x01\n\x06K8sPod\x12<\n\x08metadata\x18\x01 \x01(\x0b\x32 .flyteidl.core.K8sObjectMetadataR\x08metadata\x12\x32\n\x08pod_spec\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructR\x07podSpec\x12\x41\n\x0b\x64\x61ta_config\x18\x03 \x01(\x0b\x32 .flyteidl.core.DataLoadingConfigR\ndataConfig\"\xa9\x02\n\x11K8sObjectMetadata\x12\x44\n\x06labels\x18\x01 \x03(\x0b\x32,.flyteidl.core.K8sObjectMetadata.LabelsEntryR\x06labels\x12S\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x31.flyteidl.core.K8sObjectMetadata.AnnotationsEntryR\x0b\x61nnotations\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a>\n\x10\x41nnotationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\x92\x01\n\x03Sql\x12\x1c\n\tstatement\x18\x01 \x01(\tR\tstatement\x12\x34\n\x07\x64ialect\x18\x02 \x01(\x0e\x32\x1a.flyteidl.core.Sql.DialectR\x07\x64ialect\"7\n\x07\x44ialect\x12\r\n\tUNDEFINED\x10\x00\x12\x08\n\x04\x41NSI\x10\x01\x12\x08\n\x04HIVE\x10\x02\x12\t\n\x05OTHER\x10\x03\x42\xaa\x01\n\x11\x63om.flyteidl.coreB\nTasksProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.tasks_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.tasks_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\nTasksProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
   _TASKMETADATA_TAGSENTRY._options = None
   _TASKMETADATA_TAGSENTRY._serialized_options = b'8\001'
   _TASKTEMPLATE_CONFIGENTRY._options = None
   _TASKTEMPLATE_CONFIGENTRY._serialized_options = b'8\001'
   _CONTAINER.fields_by_name['config']._options = None
   _CONTAINER.fields_by_name['config']._serialized_options = b'\030\001'
   _K8SOBJECTMETADATA_LABELSENTRY._options = None
   _K8SOBJECTMETADATA_LABELSENTRY._serialized_options = b'8\001'
   _K8SOBJECTMETADATA_ANNOTATIONSENTRY._options = None
   _K8SOBJECTMETADATA_ANNOTATIONSENTRY._serialized_options = b'8\001'
-  _RESOURCES._serialized_start=230
-  _RESOURCES._serialized_end=566
-  _RESOURCES_RESOURCEENTRY._serialized_start=375
-  _RESOURCES_RESOURCEENTRY._serialized_end=471
-  _RESOURCES_RESOURCENAME._serialized_start=473
-  _RESOURCES_RESOURCENAME._serialized_end=566
-  _RUNTIMEMETADATA._serialized_start=569
-  _RUNTIMEMETADATA._serialized_end=741
-  _RUNTIMEMETADATA_RUNTIMETYPE._serialized_start=702
-  _RUNTIMEMETADATA_RUNTIMETYPE._serialized_end=741
-  _TASKMETADATA._serialized_start=744
-  _TASKMETADATA._serialized_end=1329
-  _TASKMETADATA_TAGSENTRY._serialized_start=1251
-  _TASKMETADATA_TAGSENTRY._serialized_end=1306
-  _TASKTEMPLATE._serialized_start=1332
-  _TASKTEMPLATE._serialized_end=1977
-  _TASKTEMPLATE_CONFIGENTRY._serialized_start=1910
-  _TASKTEMPLATE_CONFIGENTRY._serialized_end=1967
-  _CONTAINERPORT._serialized_start=1979
-  _CONTAINERPORT._serialized_end=2033
-  _CONTAINER._serialized_start=2036
-  _CONTAINER._serialized_end=2544
-  _CONTAINER_ARCHITECTURE._serialized_start=2471
-  _CONTAINER_ARCHITECTURE._serialized_end=2544
-  _IOSTRATEGY._serialized_start=2547
-  _IOSTRATEGY._serialized_end=2856
-  _IOSTRATEGY_DOWNLOADMODE._serialized_start=2709
-  _IOSTRATEGY_DOWNLOADMODE._serialized_end=2785
-  _IOSTRATEGY_UPLOADMODE._serialized_start=2787
-  _IOSTRATEGY_UPLOADMODE._serialized_end=2856
-  _DATALOADINGCONFIG._serialized_start=2859
-  _DATALOADINGCONFIG._serialized_end=3154
-  _DATALOADINGCONFIG_LITERALMAPFORMAT._serialized_start=3105
-  _DATALOADINGCONFIG_LITERALMAPFORMAT._serialized_end=3154
-  _K8SPOD._serialized_start=3156
-  _K8SPOD._serialized_end=3278
-  _K8SOBJECTMETADATA._serialized_start=3281
-  _K8SOBJECTMETADATA._serialized_end=3578
-  _K8SOBJECTMETADATA_LABELSENTRY._serialized_start=3457
-  _K8SOBJECTMETADATA_LABELSENTRY._serialized_end=3514
-  _K8SOBJECTMETADATA_ANNOTATIONSENTRY._serialized_start=3516
-  _K8SOBJECTMETADATA_ANNOTATIONSENTRY._serialized_end=3578
-  _SQL._serialized_start=3581
-  _SQL._serialized_end=3727
-  _SQL_DIALECT._serialized_start=3672
-  _SQL_DIALECT._serialized_end=3727
+  _globals['_RESOURCES']._serialized_start=230
+  _globals['_RESOURCES']._serialized_end=566
+  _globals['_RESOURCES_RESOURCEENTRY']._serialized_start=375
+  _globals['_RESOURCES_RESOURCEENTRY']._serialized_end=471
+  _globals['_RESOURCES_RESOURCENAME']._serialized_start=473
+  _globals['_RESOURCES_RESOURCENAME']._serialized_end=566
+  _globals['_RUNTIMEMETADATA']._serialized_start=569
+  _globals['_RUNTIMEMETADATA']._serialized_end=741
+  _globals['_RUNTIMEMETADATA_RUNTIMETYPE']._serialized_start=702
+  _globals['_RUNTIMEMETADATA_RUNTIMETYPE']._serialized_end=741
+  _globals['_TASKMETADATA']._serialized_start=744
+  _globals['_TASKMETADATA']._serialized_end=1373
+  _globals['_TASKMETADATA_TAGSENTRY']._serialized_start=1295
+  _globals['_TASKMETADATA_TAGSENTRY']._serialized_end=1350
+  _globals['_TASKTEMPLATE']._serialized_start=1376
+  _globals['_TASKTEMPLATE']._serialized_end=2021
+  _globals['_TASKTEMPLATE_CONFIGENTRY']._serialized_start=1954
+  _globals['_TASKTEMPLATE_CONFIGENTRY']._serialized_end=2011
+  _globals['_CONTAINERPORT']._serialized_start=2023
+  _globals['_CONTAINERPORT']._serialized_end=2077
+  _globals['_CONTAINER']._serialized_start=2080
+  _globals['_CONTAINER']._serialized_end=2588
+  _globals['_CONTAINER_ARCHITECTURE']._serialized_start=2515
+  _globals['_CONTAINER_ARCHITECTURE']._serialized_end=2588
+  _globals['_IOSTRATEGY']._serialized_start=2591
+  _globals['_IOSTRATEGY']._serialized_end=2900
+  _globals['_IOSTRATEGY_DOWNLOADMODE']._serialized_start=2753
+  _globals['_IOSTRATEGY_DOWNLOADMODE']._serialized_end=2829
+  _globals['_IOSTRATEGY_UPLOADMODE']._serialized_start=2831
+  _globals['_IOSTRATEGY_UPLOADMODE']._serialized_end=2900
+  _globals['_DATALOADINGCONFIG']._serialized_start=2903
+  _globals['_DATALOADINGCONFIG']._serialized_end=3198
+  _globals['_DATALOADINGCONFIG_LITERALMAPFORMAT']._serialized_start=3149
+  _globals['_DATALOADINGCONFIG_LITERALMAPFORMAT']._serialized_end=3198
+  _globals['_K8SPOD']._serialized_start=3201
+  _globals['_K8SPOD']._serialized_end=3390
+  _globals['_K8SOBJECTMETADATA']._serialized_start=3393
+  _globals['_K8SOBJECTMETADATA']._serialized_end=3690
+  _globals['_K8SOBJECTMETADATA_LABELSENTRY']._serialized_start=3569
+  _globals['_K8SOBJECTMETADATA_LABELSENTRY']._serialized_end=3626
+  _globals['_K8SOBJECTMETADATA_ANNOTATIONSENTRY']._serialized_start=3628
+  _globals['_K8SOBJECTMETADATA_ANNOTATIONSENTRY']._serialized_end=3690
+  _globals['_SQL']._serialized_start=3693
+  _globals['_SQL']._serialized_end=3839
+  _globals['_SQL_DIALECT']._serialized_start=3784
+  _globals['_SQL_DIALECT']._serialized_end=3839
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/tasks_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/tasks_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -8,223 +8,253 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Container(_message.Message):
-    __slots__ = ["architecture", "args", "command", "config", "data_config", "env", "image", "ports", "resources"]
-    class Architecture(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    AMD64: Container.Architecture
-    ARCHITECTURE_FIELD_NUMBER: _ClassVar[int]
-    ARGS_FIELD_NUMBER: _ClassVar[int]
-    ARM64: Container.Architecture
-    ARM_V6: Container.Architecture
-    ARM_V7: Container.Architecture
-    COMMAND_FIELD_NUMBER: _ClassVar[int]
-    CONFIG_FIELD_NUMBER: _ClassVar[int]
-    DATA_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    ENV_FIELD_NUMBER: _ClassVar[int]
-    IMAGE_FIELD_NUMBER: _ClassVar[int]
-    PORTS_FIELD_NUMBER: _ClassVar[int]
-    RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: Container.Architecture
-    architecture: Container.Architecture
-    args: _containers.RepeatedScalarFieldContainer[str]
-    command: _containers.RepeatedScalarFieldContainer[str]
-    config: _containers.RepeatedCompositeFieldContainer[_literals_pb2.KeyValuePair]
-    data_config: DataLoadingConfig
-    env: _containers.RepeatedCompositeFieldContainer[_literals_pb2.KeyValuePair]
-    image: str
-    ports: _containers.RepeatedCompositeFieldContainer[ContainerPort]
-    resources: Resources
-    def __init__(self, image: _Optional[str] = ..., command: _Optional[_Iterable[str]] = ..., args: _Optional[_Iterable[str]] = ..., resources: _Optional[_Union[Resources, _Mapping]] = ..., env: _Optional[_Iterable[_Union[_literals_pb2.KeyValuePair, _Mapping]]] = ..., config: _Optional[_Iterable[_Union[_literals_pb2.KeyValuePair, _Mapping]]] = ..., ports: _Optional[_Iterable[_Union[ContainerPort, _Mapping]]] = ..., data_config: _Optional[_Union[DataLoadingConfig, _Mapping]] = ..., architecture: _Optional[_Union[Container.Architecture, str]] = ...) -> None: ...
-
-class ContainerPort(_message.Message):
-    __slots__ = ["container_port"]
-    CONTAINER_PORT_FIELD_NUMBER: _ClassVar[int]
-    container_port: int
-    def __init__(self, container_port: _Optional[int] = ...) -> None: ...
-
-class DataLoadingConfig(_message.Message):
-    __slots__ = ["enabled", "format", "input_path", "io_strategy", "output_path"]
-    class LiteralMapFormat(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    ENABLED_FIELD_NUMBER: _ClassVar[int]
-    FORMAT_FIELD_NUMBER: _ClassVar[int]
-    INPUT_PATH_FIELD_NUMBER: _ClassVar[int]
-    IO_STRATEGY_FIELD_NUMBER: _ClassVar[int]
-    JSON: DataLoadingConfig.LiteralMapFormat
-    OUTPUT_PATH_FIELD_NUMBER: _ClassVar[int]
-    PROTO: DataLoadingConfig.LiteralMapFormat
-    YAML: DataLoadingConfig.LiteralMapFormat
-    enabled: bool
-    format: DataLoadingConfig.LiteralMapFormat
-    input_path: str
-    io_strategy: IOStrategy
-    output_path: str
-    def __init__(self, enabled: bool = ..., input_path: _Optional[str] = ..., output_path: _Optional[str] = ..., format: _Optional[_Union[DataLoadingConfig.LiteralMapFormat, str]] = ..., io_strategy: _Optional[_Union[IOStrategy, _Mapping]] = ...) -> None: ...
-
-class IOStrategy(_message.Message):
-    __slots__ = ["download_mode", "upload_mode"]
-    class DownloadMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class UploadMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    DOWNLOAD_EAGER: IOStrategy.DownloadMode
-    DOWNLOAD_MODE_FIELD_NUMBER: _ClassVar[int]
-    DOWNLOAD_STREAM: IOStrategy.DownloadMode
-    DO_NOT_DOWNLOAD: IOStrategy.DownloadMode
-    DO_NOT_UPLOAD: IOStrategy.UploadMode
-    UPLOAD_EAGER: IOStrategy.UploadMode
-    UPLOAD_MODE_FIELD_NUMBER: _ClassVar[int]
-    UPLOAD_ON_EXIT: IOStrategy.UploadMode
-    download_mode: IOStrategy.DownloadMode
-    upload_mode: IOStrategy.UploadMode
-    def __init__(self, download_mode: _Optional[_Union[IOStrategy.DownloadMode, str]] = ..., upload_mode: _Optional[_Union[IOStrategy.UploadMode, str]] = ...) -> None: ...
-
-class K8sObjectMetadata(_message.Message):
-    __slots__ = ["annotations", "labels"]
-    class AnnotationsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    class LabelsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
-    LABELS_FIELD_NUMBER: _ClassVar[int]
-    annotations: _containers.ScalarMap[str, str]
-    labels: _containers.ScalarMap[str, str]
-    def __init__(self, labels: _Optional[_Mapping[str, str]] = ..., annotations: _Optional[_Mapping[str, str]] = ...) -> None: ...
-
-class K8sPod(_message.Message):
-    __slots__ = ["metadata", "pod_spec"]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    POD_SPEC_FIELD_NUMBER: _ClassVar[int]
-    metadata: K8sObjectMetadata
-    pod_spec: _struct_pb2.Struct
-    def __init__(self, metadata: _Optional[_Union[K8sObjectMetadata, _Mapping]] = ..., pod_spec: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...) -> None: ...
-
 class Resources(_message.Message):
-    __slots__ = ["limits", "requests"]
+    __slots__ = ["requests", "limits"]
     class ResourceName(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        UNKNOWN: _ClassVar[Resources.ResourceName]
+        CPU: _ClassVar[Resources.ResourceName]
+        GPU: _ClassVar[Resources.ResourceName]
+        MEMORY: _ClassVar[Resources.ResourceName]
+        STORAGE: _ClassVar[Resources.ResourceName]
+        EPHEMERAL_STORAGE: _ClassVar[Resources.ResourceName]
+    UNKNOWN: Resources.ResourceName
+    CPU: Resources.ResourceName
+    GPU: Resources.ResourceName
+    MEMORY: Resources.ResourceName
+    STORAGE: Resources.ResourceName
+    EPHEMERAL_STORAGE: Resources.ResourceName
     class ResourceEntry(_message.Message):
         __slots__ = ["name", "value"]
         NAME_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         name: Resources.ResourceName
         value: str
         def __init__(self, name: _Optional[_Union[Resources.ResourceName, str]] = ..., value: _Optional[str] = ...) -> None: ...
-    CPU: Resources.ResourceName
-    EPHEMERAL_STORAGE: Resources.ResourceName
-    GPU: Resources.ResourceName
-    LIMITS_FIELD_NUMBER: _ClassVar[int]
-    MEMORY: Resources.ResourceName
     REQUESTS_FIELD_NUMBER: _ClassVar[int]
-    STORAGE: Resources.ResourceName
-    UNKNOWN: Resources.ResourceName
-    limits: _containers.RepeatedCompositeFieldContainer[Resources.ResourceEntry]
+    LIMITS_FIELD_NUMBER: _ClassVar[int]
     requests: _containers.RepeatedCompositeFieldContainer[Resources.ResourceEntry]
+    limits: _containers.RepeatedCompositeFieldContainer[Resources.ResourceEntry]
     def __init__(self, requests: _Optional[_Iterable[_Union[Resources.ResourceEntry, _Mapping]]] = ..., limits: _Optional[_Iterable[_Union[Resources.ResourceEntry, _Mapping]]] = ...) -> None: ...
 
 class RuntimeMetadata(_message.Message):
-    __slots__ = ["flavor", "type", "version"]
+    __slots__ = ["type", "version", "flavor"]
     class RuntimeType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    FLAVOR_FIELD_NUMBER: _ClassVar[int]
-    FLYTE_SDK: RuntimeMetadata.RuntimeType
+        OTHER: _ClassVar[RuntimeMetadata.RuntimeType]
+        FLYTE_SDK: _ClassVar[RuntimeMetadata.RuntimeType]
     OTHER: RuntimeMetadata.RuntimeType
+    FLYTE_SDK: RuntimeMetadata.RuntimeType
     TYPE_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
-    flavor: str
+    FLAVOR_FIELD_NUMBER: _ClassVar[int]
     type: RuntimeMetadata.RuntimeType
     version: str
+    flavor: str
     def __init__(self, type: _Optional[_Union[RuntimeMetadata.RuntimeType, str]] = ..., version: _Optional[str] = ..., flavor: _Optional[str] = ...) -> None: ...
 
-class Sql(_message.Message):
-    __slots__ = ["dialect", "statement"]
-    class Dialect(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    ANSI: Sql.Dialect
-    DIALECT_FIELD_NUMBER: _ClassVar[int]
-    HIVE: Sql.Dialect
-    OTHER: Sql.Dialect
-    STATEMENT_FIELD_NUMBER: _ClassVar[int]
-    UNDEFINED: Sql.Dialect
-    dialect: Sql.Dialect
-    statement: str
-    def __init__(self, statement: _Optional[str] = ..., dialect: _Optional[_Union[Sql.Dialect, str]] = ...) -> None: ...
-
 class TaskMetadata(_message.Message):
-    __slots__ = ["cache_serializable", "deprecated_error_message", "discoverable", "discovery_version", "generates_deck", "interruptible", "retries", "runtime", "tags", "timeout"]
+    __slots__ = ["discoverable", "runtime", "timeout", "retries", "discovery_version", "deprecated_error_message", "interruptible", "cache_serializable", "generates_deck", "tags", "pod_template_name"]
     class TagsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    CACHE_SERIALIZABLE_FIELD_NUMBER: _ClassVar[int]
-    DEPRECATED_ERROR_MESSAGE_FIELD_NUMBER: _ClassVar[int]
     DISCOVERABLE_FIELD_NUMBER: _ClassVar[int]
+    RUNTIME_FIELD_NUMBER: _ClassVar[int]
+    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
+    RETRIES_FIELD_NUMBER: _ClassVar[int]
     DISCOVERY_VERSION_FIELD_NUMBER: _ClassVar[int]
-    GENERATES_DECK_FIELD_NUMBER: _ClassVar[int]
+    DEPRECATED_ERROR_MESSAGE_FIELD_NUMBER: _ClassVar[int]
     INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
-    RETRIES_FIELD_NUMBER: _ClassVar[int]
-    RUNTIME_FIELD_NUMBER: _ClassVar[int]
+    CACHE_SERIALIZABLE_FIELD_NUMBER: _ClassVar[int]
+    GENERATES_DECK_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
-    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
-    cache_serializable: bool
-    deprecated_error_message: str
+    POD_TEMPLATE_NAME_FIELD_NUMBER: _ClassVar[int]
     discoverable: bool
+    runtime: RuntimeMetadata
+    timeout: _duration_pb2.Duration
+    retries: _literals_pb2.RetryStrategy
     discovery_version: str
-    generates_deck: bool
+    deprecated_error_message: str
     interruptible: bool
-    retries: _literals_pb2.RetryStrategy
-    runtime: RuntimeMetadata
+    cache_serializable: bool
+    generates_deck: bool
     tags: _containers.ScalarMap[str, str]
-    timeout: _duration_pb2.Duration
-    def __init__(self, discoverable: bool = ..., runtime: _Optional[_Union[RuntimeMetadata, _Mapping]] = ..., timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., retries: _Optional[_Union[_literals_pb2.RetryStrategy, _Mapping]] = ..., discovery_version: _Optional[str] = ..., deprecated_error_message: _Optional[str] = ..., interruptible: bool = ..., cache_serializable: bool = ..., generates_deck: bool = ..., tags: _Optional[_Mapping[str, str]] = ...) -> None: ...
+    pod_template_name: str
+    def __init__(self, discoverable: bool = ..., runtime: _Optional[_Union[RuntimeMetadata, _Mapping]] = ..., timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., retries: _Optional[_Union[_literals_pb2.RetryStrategy, _Mapping]] = ..., discovery_version: _Optional[str] = ..., deprecated_error_message: _Optional[str] = ..., interruptible: bool = ..., cache_serializable: bool = ..., generates_deck: bool = ..., tags: _Optional[_Mapping[str, str]] = ..., pod_template_name: _Optional[str] = ...) -> None: ...
 
 class TaskTemplate(_message.Message):
-    __slots__ = ["config", "container", "custom", "id", "interface", "k8s_pod", "metadata", "security_context", "sql", "task_type_version", "type"]
+    __slots__ = ["id", "type", "metadata", "interface", "custom", "container", "k8s_pod", "sql", "task_type_version", "security_context", "config"]
     class ConfigEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    CONFIG_FIELD_NUMBER: _ClassVar[int]
-    CONTAINER_FIELD_NUMBER: _ClassVar[int]
-    CUSTOM_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
     INTERFACE_FIELD_NUMBER: _ClassVar[int]
+    CUSTOM_FIELD_NUMBER: _ClassVar[int]
+    CONTAINER_FIELD_NUMBER: _ClassVar[int]
     K8S_POD_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
     SQL_FIELD_NUMBER: _ClassVar[int]
     TASK_TYPE_VERSION_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    config: _containers.ScalarMap[str, str]
-    container: Container
-    custom: _struct_pb2.Struct
+    SECURITY_CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    CONFIG_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
+    type: str
+    metadata: TaskMetadata
     interface: _interface_pb2.TypedInterface
+    custom: _struct_pb2.Struct
+    container: Container
     k8s_pod: K8sPod
-    metadata: TaskMetadata
-    security_context: _security_pb2.SecurityContext
     sql: Sql
     task_type_version: int
-    type: str
+    security_context: _security_pb2.SecurityContext
+    config: _containers.ScalarMap[str, str]
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., type: _Optional[str] = ..., metadata: _Optional[_Union[TaskMetadata, _Mapping]] = ..., interface: _Optional[_Union[_interface_pb2.TypedInterface, _Mapping]] = ..., custom: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., container: _Optional[_Union[Container, _Mapping]] = ..., k8s_pod: _Optional[_Union[K8sPod, _Mapping]] = ..., sql: _Optional[_Union[Sql, _Mapping]] = ..., task_type_version: _Optional[int] = ..., security_context: _Optional[_Union[_security_pb2.SecurityContext, _Mapping]] = ..., config: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class ContainerPort(_message.Message):
+    __slots__ = ["container_port"]
+    CONTAINER_PORT_FIELD_NUMBER: _ClassVar[int]
+    container_port: int
+    def __init__(self, container_port: _Optional[int] = ...) -> None: ...
+
+class Container(_message.Message):
+    __slots__ = ["image", "command", "args", "resources", "env", "config", "ports", "data_config", "architecture"]
+    class Architecture(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        UNKNOWN: _ClassVar[Container.Architecture]
+        AMD64: _ClassVar[Container.Architecture]
+        ARM64: _ClassVar[Container.Architecture]
+        ARM_V6: _ClassVar[Container.Architecture]
+        ARM_V7: _ClassVar[Container.Architecture]
+    UNKNOWN: Container.Architecture
+    AMD64: Container.Architecture
+    ARM64: Container.Architecture
+    ARM_V6: Container.Architecture
+    ARM_V7: Container.Architecture
+    IMAGE_FIELD_NUMBER: _ClassVar[int]
+    COMMAND_FIELD_NUMBER: _ClassVar[int]
+    ARGS_FIELD_NUMBER: _ClassVar[int]
+    RESOURCES_FIELD_NUMBER: _ClassVar[int]
+    ENV_FIELD_NUMBER: _ClassVar[int]
+    CONFIG_FIELD_NUMBER: _ClassVar[int]
+    PORTS_FIELD_NUMBER: _ClassVar[int]
+    DATA_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    ARCHITECTURE_FIELD_NUMBER: _ClassVar[int]
+    image: str
+    command: _containers.RepeatedScalarFieldContainer[str]
+    args: _containers.RepeatedScalarFieldContainer[str]
+    resources: Resources
+    env: _containers.RepeatedCompositeFieldContainer[_literals_pb2.KeyValuePair]
+    config: _containers.RepeatedCompositeFieldContainer[_literals_pb2.KeyValuePair]
+    ports: _containers.RepeatedCompositeFieldContainer[ContainerPort]
+    data_config: DataLoadingConfig
+    architecture: Container.Architecture
+    def __init__(self, image: _Optional[str] = ..., command: _Optional[_Iterable[str]] = ..., args: _Optional[_Iterable[str]] = ..., resources: _Optional[_Union[Resources, _Mapping]] = ..., env: _Optional[_Iterable[_Union[_literals_pb2.KeyValuePair, _Mapping]]] = ..., config: _Optional[_Iterable[_Union[_literals_pb2.KeyValuePair, _Mapping]]] = ..., ports: _Optional[_Iterable[_Union[ContainerPort, _Mapping]]] = ..., data_config: _Optional[_Union[DataLoadingConfig, _Mapping]] = ..., architecture: _Optional[_Union[Container.Architecture, str]] = ...) -> None: ...
+
+class IOStrategy(_message.Message):
+    __slots__ = ["download_mode", "upload_mode"]
+    class DownloadMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        DOWNLOAD_EAGER: _ClassVar[IOStrategy.DownloadMode]
+        DOWNLOAD_STREAM: _ClassVar[IOStrategy.DownloadMode]
+        DO_NOT_DOWNLOAD: _ClassVar[IOStrategy.DownloadMode]
+    DOWNLOAD_EAGER: IOStrategy.DownloadMode
+    DOWNLOAD_STREAM: IOStrategy.DownloadMode
+    DO_NOT_DOWNLOAD: IOStrategy.DownloadMode
+    class UploadMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        UPLOAD_ON_EXIT: _ClassVar[IOStrategy.UploadMode]
+        UPLOAD_EAGER: _ClassVar[IOStrategy.UploadMode]
+        DO_NOT_UPLOAD: _ClassVar[IOStrategy.UploadMode]
+    UPLOAD_ON_EXIT: IOStrategy.UploadMode
+    UPLOAD_EAGER: IOStrategy.UploadMode
+    DO_NOT_UPLOAD: IOStrategy.UploadMode
+    DOWNLOAD_MODE_FIELD_NUMBER: _ClassVar[int]
+    UPLOAD_MODE_FIELD_NUMBER: _ClassVar[int]
+    download_mode: IOStrategy.DownloadMode
+    upload_mode: IOStrategy.UploadMode
+    def __init__(self, download_mode: _Optional[_Union[IOStrategy.DownloadMode, str]] = ..., upload_mode: _Optional[_Union[IOStrategy.UploadMode, str]] = ...) -> None: ...
+
+class DataLoadingConfig(_message.Message):
+    __slots__ = ["enabled", "input_path", "output_path", "format", "io_strategy"]
+    class LiteralMapFormat(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        JSON: _ClassVar[DataLoadingConfig.LiteralMapFormat]
+        YAML: _ClassVar[DataLoadingConfig.LiteralMapFormat]
+        PROTO: _ClassVar[DataLoadingConfig.LiteralMapFormat]
+    JSON: DataLoadingConfig.LiteralMapFormat
+    YAML: DataLoadingConfig.LiteralMapFormat
+    PROTO: DataLoadingConfig.LiteralMapFormat
+    ENABLED_FIELD_NUMBER: _ClassVar[int]
+    INPUT_PATH_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_PATH_FIELD_NUMBER: _ClassVar[int]
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
+    IO_STRATEGY_FIELD_NUMBER: _ClassVar[int]
+    enabled: bool
+    input_path: str
+    output_path: str
+    format: DataLoadingConfig.LiteralMapFormat
+    io_strategy: IOStrategy
+    def __init__(self, enabled: bool = ..., input_path: _Optional[str] = ..., output_path: _Optional[str] = ..., format: _Optional[_Union[DataLoadingConfig.LiteralMapFormat, str]] = ..., io_strategy: _Optional[_Union[IOStrategy, _Mapping]] = ...) -> None: ...
+
+class K8sPod(_message.Message):
+    __slots__ = ["metadata", "pod_spec", "data_config"]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    POD_SPEC_FIELD_NUMBER: _ClassVar[int]
+    DATA_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    metadata: K8sObjectMetadata
+    pod_spec: _struct_pb2.Struct
+    data_config: DataLoadingConfig
+    def __init__(self, metadata: _Optional[_Union[K8sObjectMetadata, _Mapping]] = ..., pod_spec: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., data_config: _Optional[_Union[DataLoadingConfig, _Mapping]] = ...) -> None: ...
+
+class K8sObjectMetadata(_message.Message):
+    __slots__ = ["labels", "annotations"]
+    class LabelsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    class AnnotationsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
+    labels: _containers.ScalarMap[str, str]
+    annotations: _containers.ScalarMap[str, str]
+    def __init__(self, labels: _Optional[_Mapping[str, str]] = ..., annotations: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class Sql(_message.Message):
+    __slots__ = ["statement", "dialect"]
+    class Dialect(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        UNDEFINED: _ClassVar[Sql.Dialect]
+        ANSI: _ClassVar[Sql.Dialect]
+        HIVE: _ClassVar[Sql.Dialect]
+        OTHER: _ClassVar[Sql.Dialect]
+    UNDEFINED: Sql.Dialect
+    ANSI: Sql.Dialect
+    HIVE: Sql.Dialect
+    OTHER: Sql.Dialect
+    STATEMENT_FIELD_NUMBER: _ClassVar[int]
+    DIALECT_FIELD_NUMBER: _ClassVar[int]
+    statement: str
+    dialect: Sql.Dialect
+    def __init__(self, statement: _Optional[str] = ..., dialect: _Optional[_Union[Sql.Dialect, str]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/types_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/types_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,139 +1,157 @@
 from google.protobuf import struct_pb2 as _struct_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-BINARY: SimpleType
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class SimpleType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    NONE: _ClassVar[SimpleType]
+    INTEGER: _ClassVar[SimpleType]
+    FLOAT: _ClassVar[SimpleType]
+    STRING: _ClassVar[SimpleType]
+    BOOLEAN: _ClassVar[SimpleType]
+    DATETIME: _ClassVar[SimpleType]
+    DURATION: _ClassVar[SimpleType]
+    BINARY: _ClassVar[SimpleType]
+    ERROR: _ClassVar[SimpleType]
+    STRUCT: _ClassVar[SimpleType]
+NONE: SimpleType
+INTEGER: SimpleType
+FLOAT: SimpleType
+STRING: SimpleType
 BOOLEAN: SimpleType
 DATETIME: SimpleType
-DESCRIPTOR: _descriptor.FileDescriptor
 DURATION: SimpleType
+BINARY: SimpleType
 ERROR: SimpleType
-FLOAT: SimpleType
-INTEGER: SimpleType
-NONE: SimpleType
-STRING: SimpleType
 STRUCT: SimpleType
 
-class BlobType(_message.Message):
-    __slots__ = ["dimensionality", "format"]
-    class BlobDimensionality(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    DIMENSIONALITY_FIELD_NUMBER: _ClassVar[int]
-    FORMAT_FIELD_NUMBER: _ClassVar[int]
-    MULTIPART: BlobType.BlobDimensionality
-    SINGLE: BlobType.BlobDimensionality
-    dimensionality: BlobType.BlobDimensionality
-    format: str
-    def __init__(self, format: _Optional[str] = ..., dimensionality: _Optional[_Union[BlobType.BlobDimensionality, str]] = ...) -> None: ...
-
-class EnumType(_message.Message):
-    __slots__ = ["values"]
-    VALUES_FIELD_NUMBER: _ClassVar[int]
-    values: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class Error(_message.Message):
-    __slots__ = ["failed_node_id", "message"]
-    FAILED_NODE_ID_FIELD_NUMBER: _ClassVar[int]
-    MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    failed_node_id: str
-    message: str
-    def __init__(self, failed_node_id: _Optional[str] = ..., message: _Optional[str] = ...) -> None: ...
-
-class LiteralType(_message.Message):
-    __slots__ = ["annotation", "blob", "collection_type", "enum_type", "map_value_type", "metadata", "schema", "simple", "structure", "structured_dataset_type", "union_type"]
-    ANNOTATION_FIELD_NUMBER: _ClassVar[int]
-    BLOB_FIELD_NUMBER: _ClassVar[int]
-    COLLECTION_TYPE_FIELD_NUMBER: _ClassVar[int]
-    ENUM_TYPE_FIELD_NUMBER: _ClassVar[int]
-    MAP_VALUE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    SCHEMA_FIELD_NUMBER: _ClassVar[int]
-    SIMPLE_FIELD_NUMBER: _ClassVar[int]
-    STRUCTURED_DATASET_TYPE_FIELD_NUMBER: _ClassVar[int]
-    STRUCTURE_FIELD_NUMBER: _ClassVar[int]
-    UNION_TYPE_FIELD_NUMBER: _ClassVar[int]
-    annotation: TypeAnnotation
-    blob: BlobType
-    collection_type: LiteralType
-    enum_type: EnumType
-    map_value_type: LiteralType
-    metadata: _struct_pb2.Struct
-    schema: SchemaType
-    simple: SimpleType
-    structure: TypeStructure
-    structured_dataset_type: StructuredDatasetType
-    union_type: UnionType
-    def __init__(self, simple: _Optional[_Union[SimpleType, str]] = ..., schema: _Optional[_Union[SchemaType, _Mapping]] = ..., collection_type: _Optional[_Union[LiteralType, _Mapping]] = ..., map_value_type: _Optional[_Union[LiteralType, _Mapping]] = ..., blob: _Optional[_Union[BlobType, _Mapping]] = ..., enum_type: _Optional[_Union[EnumType, _Mapping]] = ..., structured_dataset_type: _Optional[_Union[StructuredDatasetType, _Mapping]] = ..., union_type: _Optional[_Union[UnionType, _Mapping]] = ..., metadata: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., annotation: _Optional[_Union[TypeAnnotation, _Mapping]] = ..., structure: _Optional[_Union[TypeStructure, _Mapping]] = ...) -> None: ...
-
-class OutputReference(_message.Message):
-    __slots__ = ["node_id", "var"]
-    NODE_ID_FIELD_NUMBER: _ClassVar[int]
-    VAR_FIELD_NUMBER: _ClassVar[int]
-    node_id: str
-    var: str
-    def __init__(self, node_id: _Optional[str] = ..., var: _Optional[str] = ...) -> None: ...
-
 class SchemaType(_message.Message):
     __slots__ = ["columns"]
     class SchemaColumn(_message.Message):
         __slots__ = ["name", "type"]
         class SchemaColumnType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
             __slots__ = []
+            INTEGER: _ClassVar[SchemaType.SchemaColumn.SchemaColumnType]
+            FLOAT: _ClassVar[SchemaType.SchemaColumn.SchemaColumnType]
+            STRING: _ClassVar[SchemaType.SchemaColumn.SchemaColumnType]
+            BOOLEAN: _ClassVar[SchemaType.SchemaColumn.SchemaColumnType]
+            DATETIME: _ClassVar[SchemaType.SchemaColumn.SchemaColumnType]
+            DURATION: _ClassVar[SchemaType.SchemaColumn.SchemaColumnType]
+        INTEGER: SchemaType.SchemaColumn.SchemaColumnType
+        FLOAT: SchemaType.SchemaColumn.SchemaColumnType
+        STRING: SchemaType.SchemaColumn.SchemaColumnType
         BOOLEAN: SchemaType.SchemaColumn.SchemaColumnType
         DATETIME: SchemaType.SchemaColumn.SchemaColumnType
         DURATION: SchemaType.SchemaColumn.SchemaColumnType
-        FLOAT: SchemaType.SchemaColumn.SchemaColumnType
-        INTEGER: SchemaType.SchemaColumn.SchemaColumnType
         NAME_FIELD_NUMBER: _ClassVar[int]
-        STRING: SchemaType.SchemaColumn.SchemaColumnType
         TYPE_FIELD_NUMBER: _ClassVar[int]
         name: str
         type: SchemaType.SchemaColumn.SchemaColumnType
         def __init__(self, name: _Optional[str] = ..., type: _Optional[_Union[SchemaType.SchemaColumn.SchemaColumnType, str]] = ...) -> None: ...
     COLUMNS_FIELD_NUMBER: _ClassVar[int]
     columns: _containers.RepeatedCompositeFieldContainer[SchemaType.SchemaColumn]
     def __init__(self, columns: _Optional[_Iterable[_Union[SchemaType.SchemaColumn, _Mapping]]] = ...) -> None: ...
 
 class StructuredDatasetType(_message.Message):
-    __slots__ = ["columns", "external_schema_bytes", "external_schema_type", "format"]
+    __slots__ = ["columns", "format", "external_schema_type", "external_schema_bytes"]
     class DatasetColumn(_message.Message):
-        __slots__ = ["literal_type", "name"]
-        LITERAL_TYPE_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["name", "literal_type"]
         NAME_FIELD_NUMBER: _ClassVar[int]
-        literal_type: LiteralType
+        LITERAL_TYPE_FIELD_NUMBER: _ClassVar[int]
         name: str
+        literal_type: LiteralType
         def __init__(self, name: _Optional[str] = ..., literal_type: _Optional[_Union[LiteralType, _Mapping]] = ...) -> None: ...
     COLUMNS_FIELD_NUMBER: _ClassVar[int]
-    EXTERNAL_SCHEMA_BYTES_FIELD_NUMBER: _ClassVar[int]
-    EXTERNAL_SCHEMA_TYPE_FIELD_NUMBER: _ClassVar[int]
     FORMAT_FIELD_NUMBER: _ClassVar[int]
+    EXTERNAL_SCHEMA_TYPE_FIELD_NUMBER: _ClassVar[int]
+    EXTERNAL_SCHEMA_BYTES_FIELD_NUMBER: _ClassVar[int]
     columns: _containers.RepeatedCompositeFieldContainer[StructuredDatasetType.DatasetColumn]
-    external_schema_bytes: bytes
-    external_schema_type: str
     format: str
+    external_schema_type: str
+    external_schema_bytes: bytes
     def __init__(self, columns: _Optional[_Iterable[_Union[StructuredDatasetType.DatasetColumn, _Mapping]]] = ..., format: _Optional[str] = ..., external_schema_type: _Optional[str] = ..., external_schema_bytes: _Optional[bytes] = ...) -> None: ...
 
-class TypeAnnotation(_message.Message):
-    __slots__ = ["annotations"]
-    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
-    annotations: _struct_pb2.Struct
-    def __init__(self, annotations: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...) -> None: ...
+class BlobType(_message.Message):
+    __slots__ = ["format", "dimensionality"]
+    class BlobDimensionality(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        SINGLE: _ClassVar[BlobType.BlobDimensionality]
+        MULTIPART: _ClassVar[BlobType.BlobDimensionality]
+    SINGLE: BlobType.BlobDimensionality
+    MULTIPART: BlobType.BlobDimensionality
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
+    DIMENSIONALITY_FIELD_NUMBER: _ClassVar[int]
+    format: str
+    dimensionality: BlobType.BlobDimensionality
+    def __init__(self, format: _Optional[str] = ..., dimensionality: _Optional[_Union[BlobType.BlobDimensionality, str]] = ...) -> None: ...
 
-class TypeStructure(_message.Message):
-    __slots__ = ["tag"]
-    TAG_FIELD_NUMBER: _ClassVar[int]
-    tag: str
-    def __init__(self, tag: _Optional[str] = ...) -> None: ...
+class EnumType(_message.Message):
+    __slots__ = ["values"]
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class UnionType(_message.Message):
     __slots__ = ["variants"]
     VARIANTS_FIELD_NUMBER: _ClassVar[int]
     variants: _containers.RepeatedCompositeFieldContainer[LiteralType]
     def __init__(self, variants: _Optional[_Iterable[_Union[LiteralType, _Mapping]]] = ...) -> None: ...
 
-class SimpleType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class TypeStructure(_message.Message):
+    __slots__ = ["tag"]
+    TAG_FIELD_NUMBER: _ClassVar[int]
+    tag: str
+    def __init__(self, tag: _Optional[str] = ...) -> None: ...
+
+class TypeAnnotation(_message.Message):
+    __slots__ = ["annotations"]
+    ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
+    annotations: _struct_pb2.Struct
+    def __init__(self, annotations: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...) -> None: ...
+
+class LiteralType(_message.Message):
+    __slots__ = ["simple", "schema", "collection_type", "map_value_type", "blob", "enum_type", "structured_dataset_type", "union_type", "metadata", "annotation", "structure"]
+    SIMPLE_FIELD_NUMBER: _ClassVar[int]
+    SCHEMA_FIELD_NUMBER: _ClassVar[int]
+    COLLECTION_TYPE_FIELD_NUMBER: _ClassVar[int]
+    MAP_VALUE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    BLOB_FIELD_NUMBER: _ClassVar[int]
+    ENUM_TYPE_FIELD_NUMBER: _ClassVar[int]
+    STRUCTURED_DATASET_TYPE_FIELD_NUMBER: _ClassVar[int]
+    UNION_TYPE_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    ANNOTATION_FIELD_NUMBER: _ClassVar[int]
+    STRUCTURE_FIELD_NUMBER: _ClassVar[int]
+    simple: SimpleType
+    schema: SchemaType
+    collection_type: LiteralType
+    map_value_type: LiteralType
+    blob: BlobType
+    enum_type: EnumType
+    structured_dataset_type: StructuredDatasetType
+    union_type: UnionType
+    metadata: _struct_pb2.Struct
+    annotation: TypeAnnotation
+    structure: TypeStructure
+    def __init__(self, simple: _Optional[_Union[SimpleType, str]] = ..., schema: _Optional[_Union[SchemaType, _Mapping]] = ..., collection_type: _Optional[_Union[LiteralType, _Mapping]] = ..., map_value_type: _Optional[_Union[LiteralType, _Mapping]] = ..., blob: _Optional[_Union[BlobType, _Mapping]] = ..., enum_type: _Optional[_Union[EnumType, _Mapping]] = ..., structured_dataset_type: _Optional[_Union[StructuredDatasetType, _Mapping]] = ..., union_type: _Optional[_Union[UnionType, _Mapping]] = ..., metadata: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., annotation: _Optional[_Union[TypeAnnotation, _Mapping]] = ..., structure: _Optional[_Union[TypeStructure, _Mapping]] = ...) -> None: ...
+
+class OutputReference(_message.Message):
+    __slots__ = ["node_id", "var"]
+    NODE_ID_FIELD_NUMBER: _ClassVar[int]
+    VAR_FIELD_NUMBER: _ClassVar[int]
+    node_id: str
+    var: str
+    def __init__(self, node_id: _Optional[str] = ..., var: _Optional[str] = ...) -> None: ...
+
+class Error(_message.Message):
+    __slots__ = ["failed_node_id", "message"]
+    FAILED_NODE_ID_FIELD_NUMBER: _ClassVar[int]
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    failed_node_id: str
+    message: str
+    def __init__(self, failed_node_id: _Optional[str] = ..., message: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_closure_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_closure_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 from flyteidl.core import workflow_pb2 as flyteidl_dot_core_dot_workflow__pb2
 from flyteidl.core import tasks_pb2 as flyteidl_dot_core_dot_tasks__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$flyteidl/core/workflow_closure.proto\x12\rflyteidl.core\x1a\x1c\x66lyteidl/core/workflow.proto\x1a\x19\x66lyteidl/core/tasks.proto\"\x81\x01\n\x0fWorkflowClosure\x12;\n\x08workflow\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.WorkflowTemplateR\x08workflow\x12\x31\n\x05tasks\x18\x02 \x03(\x0b\x32\x1b.flyteidl.core.TaskTemplateR\x05tasksB\xb4\x01\n\x11\x63om.flyteidl.coreB\x14WorkflowClosureProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.workflow_closure_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.workflow_closure_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\024WorkflowClosureProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
-  _WORKFLOWCLOSURE._serialized_start=113
-  _WORKFLOWCLOSURE._serialized_end=242
+  _globals['_WORKFLOWCLOSURE']._serialized_start=113
+  _globals['_WORKFLOWCLOSURE']._serialized_end=242
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_closure_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_closure_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class WorkflowClosure(_message.Message):
-    __slots__ = ["tasks", "workflow"]
-    TASKS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["workflow", "tasks"]
     WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    tasks: _containers.RepeatedCompositeFieldContainer[_tasks_pb2.TaskTemplate]
+    TASKS_FIELD_NUMBER: _ClassVar[int]
     workflow: _workflow_pb2.WorkflowTemplate
+    tasks: _containers.RepeatedCompositeFieldContainer[_tasks_pb2.TaskTemplate]
     def __init__(self, workflow: _Optional[_Union[_workflow_pb2.WorkflowTemplate, _Mapping]] = ..., tasks: _Optional[_Iterable[_Union[_tasks_pb2.TaskTemplate, _Mapping]]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,52 +20,53 @@
 from flyteidl.core import types_pb2 as flyteidl_dot_core_dot_types__pb2
 from flyteidl.core import security_pb2 as flyteidl_dot_core_dot_security__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/core/workflow.proto\x12\rflyteidl.core\x1a\x1d\x66lyteidl/core/condition.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1d\x66lyteidl/core/interface.proto\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x19\x66lyteidl/core/tasks.proto\x1a\x19\x66lyteidl/core/types.proto\x1a\x1c\x66lyteidl/core/security.proto\x1a\x1egoogle/protobuf/duration.proto\"{\n\x07IfBlock\x12>\n\tcondition\x18\x01 \x01(\x0b\x32 .flyteidl.core.BooleanExpressionR\tcondition\x12\x30\n\tthen_node\x18\x02 \x01(\x0b\x32\x13.flyteidl.core.NodeR\x08thenNode\"\xd4\x01\n\x0bIfElseBlock\x12*\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\x16.flyteidl.core.IfBlockR\x04\x63\x61se\x12,\n\x05other\x18\x02 \x03(\x0b\x32\x16.flyteidl.core.IfBlockR\x05other\x12\x32\n\telse_node\x18\x03 \x01(\x0b\x32\x13.flyteidl.core.NodeH\x00R\x08\x65lseNode\x12,\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x14.flyteidl.core.ErrorH\x00R\x05\x65rrorB\t\n\x07\x64\x65\x66\x61ult\"A\n\nBranchNode\x12\x33\n\x07if_else\x18\x01 \x01(\x0b\x32\x1a.flyteidl.core.IfElseBlockR\x06ifElse\"\x97\x01\n\x08TaskNode\x12>\n\x0creference_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierH\x00R\x0breferenceId\x12>\n\toverrides\x18\x02 \x01(\x0b\x32 .flyteidl.core.TaskNodeOverridesR\toverridesB\x0b\n\treference\"\xa6\x01\n\x0cWorkflowNode\x12\x42\n\x0elaunchplan_ref\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierH\x00R\rlaunchplanRef\x12\x45\n\x10sub_workflow_ref\x18\x02 \x01(\x0b\x32\x19.flyteidl.core.IdentifierH\x00R\x0esubWorkflowRefB\x0b\n\treference\"/\n\x10\x41pproveCondition\x12\x1b\n\tsignal_id\x18\x01 \x01(\tR\x08signalId\"\x90\x01\n\x0fSignalCondition\x12\x1b\n\tsignal_id\x18\x01 \x01(\tR\x08signalId\x12.\n\x04type\x18\x02 \x01(\x0b\x32\x1a.flyteidl.core.LiteralTypeR\x04type\x12\x30\n\x14output_variable_name\x18\x03 \x01(\tR\x12outputVariableName\"G\n\x0eSleepCondition\x12\x35\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08\x64uration\"\xc5\x01\n\x08GateNode\x12;\n\x07\x61pprove\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.ApproveConditionH\x00R\x07\x61pprove\x12\x38\n\x06signal\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.SignalConditionH\x00R\x06signal\x12\x35\n\x05sleep\x18\x03 \x01(\x0b\x32\x1d.flyteidl.core.SleepConditionH\x00R\x05sleepB\x0b\n\tcondition\"\xce\x01\n\x0cNodeMetadata\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x33\n\x07timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x07timeout\x12\x36\n\x07retries\x18\x05 \x01(\x0b\x32\x1c.flyteidl.core.RetryStrategyR\x07retries\x12&\n\rinterruptible\x18\x06 \x01(\x08H\x00R\rinterruptibleB\x15\n\x13interruptible_value\"/\n\x05\x41lias\x12\x10\n\x03var\x18\x01 \x01(\tR\x03var\x12\x14\n\x05\x61lias\x18\x02 \x01(\tR\x05\x61lias\"\xe4\x03\n\x04Node\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x37\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.flyteidl.core.NodeMetadataR\x08metadata\x12.\n\x06inputs\x18\x03 \x03(\x0b\x32\x16.flyteidl.core.BindingR\x06inputs\x12*\n\x11upstream_node_ids\x18\x04 \x03(\tR\x0fupstreamNodeIds\x12;\n\x0eoutput_aliases\x18\x05 \x03(\x0b\x32\x14.flyteidl.core.AliasR\routputAliases\x12\x36\n\ttask_node\x18\x06 \x01(\x0b\x32\x17.flyteidl.core.TaskNodeH\x00R\x08taskNode\x12\x42\n\rworkflow_node\x18\x07 \x01(\x0b\x32\x1b.flyteidl.core.WorkflowNodeH\x00R\x0cworkflowNode\x12<\n\x0b\x62ranch_node\x18\x08 \x01(\x0b\x32\x19.flyteidl.core.BranchNodeH\x00R\nbranchNode\x12\x36\n\tgate_node\x18\t \x01(\x0b\x32\x17.flyteidl.core.GateNodeH\x00R\x08gateNodeB\x08\n\x06target\"\xfc\x02\n\x10WorkflowMetadata\x12M\n\x12quality_of_service\x18\x01 \x01(\x0b\x32\x1f.flyteidl.core.QualityOfServiceR\x10qualityOfService\x12N\n\non_failure\x18\x02 \x01(\x0e\x32/.flyteidl.core.WorkflowMetadata.OnFailurePolicyR\tonFailure\x12=\n\x04tags\x18\x03 \x03(\x0b\x32).flyteidl.core.WorkflowMetadata.TagsEntryR\x04tags\x1a\x37\n\tTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"Q\n\x0fOnFailurePolicy\x12\x14\n\x10\x46\x41IL_IMMEDIATELY\x10\x00\x12(\n$FAIL_AFTER_EXECUTABLE_NODES_COMPLETE\x10\x01\"@\n\x18WorkflowMetadataDefaults\x12$\n\rinterruptible\x18\x01 \x01(\x08R\rinterruptible\"\xa2\x03\n\x10WorkflowTemplate\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12;\n\x08metadata\x18\x02 \x01(\x0b\x32\x1f.flyteidl.core.WorkflowMetadataR\x08metadata\x12;\n\tinterface\x18\x03 \x01(\x0b\x32\x1d.flyteidl.core.TypedInterfaceR\tinterface\x12)\n\x05nodes\x18\x04 \x03(\x0b\x32\x13.flyteidl.core.NodeR\x05nodes\x12\x30\n\x07outputs\x18\x05 \x03(\x0b\x32\x16.flyteidl.core.BindingR\x07outputs\x12\x36\n\x0c\x66\x61ilure_node\x18\x06 \x01(\x0b\x32\x13.flyteidl.core.NodeR\x0b\x66\x61ilureNode\x12T\n\x11metadata_defaults\x18\x07 \x01(\x0b\x32\'.flyteidl.core.WorkflowMetadataDefaultsR\x10metadataDefaults\"K\n\x11TaskNodeOverrides\x12\x36\n\tresources\x18\x01 \x01(\x0b\x32\x18.flyteidl.core.ResourcesR\tresourcesB\xad\x01\n\x11\x63om.flyteidl.coreB\rWorkflowProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.workflow_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.workflow_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\rWorkflowProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
   _WORKFLOWMETADATA_TAGSENTRY._options = None
   _WORKFLOWMETADATA_TAGSENTRY._serialized_options = b'8\001'
-  _IFBLOCK._serialized_start=318
-  _IFBLOCK._serialized_end=441
-  _IFELSEBLOCK._serialized_start=444
-  _IFELSEBLOCK._serialized_end=656
-  _BRANCHNODE._serialized_start=658
-  _BRANCHNODE._serialized_end=723
-  _TASKNODE._serialized_start=726
-  _TASKNODE._serialized_end=877
-  _WORKFLOWNODE._serialized_start=880
-  _WORKFLOWNODE._serialized_end=1046
-  _APPROVECONDITION._serialized_start=1048
-  _APPROVECONDITION._serialized_end=1095
-  _SIGNALCONDITION._serialized_start=1098
-  _SIGNALCONDITION._serialized_end=1242
-  _SLEEPCONDITION._serialized_start=1244
-  _SLEEPCONDITION._serialized_end=1315
-  _GATENODE._serialized_start=1318
-  _GATENODE._serialized_end=1515
-  _NODEMETADATA._serialized_start=1518
-  _NODEMETADATA._serialized_end=1724
-  _ALIAS._serialized_start=1726
-  _ALIAS._serialized_end=1773
-  _NODE._serialized_start=1776
-  _NODE._serialized_end=2260
-  _WORKFLOWMETADATA._serialized_start=2263
-  _WORKFLOWMETADATA._serialized_end=2643
-  _WORKFLOWMETADATA_TAGSENTRY._serialized_start=2505
-  _WORKFLOWMETADATA_TAGSENTRY._serialized_end=2560
-  _WORKFLOWMETADATA_ONFAILUREPOLICY._serialized_start=2562
-  _WORKFLOWMETADATA_ONFAILUREPOLICY._serialized_end=2643
-  _WORKFLOWMETADATADEFAULTS._serialized_start=2645
-  _WORKFLOWMETADATADEFAULTS._serialized_end=2709
-  _WORKFLOWTEMPLATE._serialized_start=2712
-  _WORKFLOWTEMPLATE._serialized_end=3130
-  _TASKNODEOVERRIDES._serialized_start=3132
-  _TASKNODEOVERRIDES._serialized_end=3207
+  _globals['_IFBLOCK']._serialized_start=318
+  _globals['_IFBLOCK']._serialized_end=441
+  _globals['_IFELSEBLOCK']._serialized_start=444
+  _globals['_IFELSEBLOCK']._serialized_end=656
+  _globals['_BRANCHNODE']._serialized_start=658
+  _globals['_BRANCHNODE']._serialized_end=723
+  _globals['_TASKNODE']._serialized_start=726
+  _globals['_TASKNODE']._serialized_end=877
+  _globals['_WORKFLOWNODE']._serialized_start=880
+  _globals['_WORKFLOWNODE']._serialized_end=1046
+  _globals['_APPROVECONDITION']._serialized_start=1048
+  _globals['_APPROVECONDITION']._serialized_end=1095
+  _globals['_SIGNALCONDITION']._serialized_start=1098
+  _globals['_SIGNALCONDITION']._serialized_end=1242
+  _globals['_SLEEPCONDITION']._serialized_start=1244
+  _globals['_SLEEPCONDITION']._serialized_end=1315
+  _globals['_GATENODE']._serialized_start=1318
+  _globals['_GATENODE']._serialized_end=1515
+  _globals['_NODEMETADATA']._serialized_start=1518
+  _globals['_NODEMETADATA']._serialized_end=1724
+  _globals['_ALIAS']._serialized_start=1726
+  _globals['_ALIAS']._serialized_end=1773
+  _globals['_NODE']._serialized_start=1776
+  _globals['_NODE']._serialized_end=2260
+  _globals['_WORKFLOWMETADATA']._serialized_start=2263
+  _globals['_WORKFLOWMETADATA']._serialized_end=2643
+  _globals['_WORKFLOWMETADATA_TAGSENTRY']._serialized_start=2505
+  _globals['_WORKFLOWMETADATA_TAGSENTRY']._serialized_end=2560
+  _globals['_WORKFLOWMETADATA_ONFAILUREPOLICY']._serialized_start=2562
+  _globals['_WORKFLOWMETADATA_ONFAILUREPOLICY']._serialized_end=2643
+  _globals['_WORKFLOWMETADATADEFAULTS']._serialized_start=2645
+  _globals['_WORKFLOWMETADATADEFAULTS']._serialized_end=2709
+  _globals['_WORKFLOWTEMPLATE']._serialized_start=2712
+  _globals['_WORKFLOWTEMPLATE']._serialized_end=3130
+  _globals['_TASKNODEOVERRIDES']._serialized_start=3132
+  _globals['_TASKNODEOVERRIDES']._serialized_end=3207
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/core/workflow_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/workflow_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,173 +11,175 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Alias(_message.Message):
-    __slots__ = ["alias", "var"]
-    ALIAS_FIELD_NUMBER: _ClassVar[int]
-    VAR_FIELD_NUMBER: _ClassVar[int]
-    alias: str
-    var: str
-    def __init__(self, var: _Optional[str] = ..., alias: _Optional[str] = ...) -> None: ...
-
-class ApproveCondition(_message.Message):
-    __slots__ = ["signal_id"]
-    SIGNAL_ID_FIELD_NUMBER: _ClassVar[int]
-    signal_id: str
-    def __init__(self, signal_id: _Optional[str] = ...) -> None: ...
-
-class BranchNode(_message.Message):
-    __slots__ = ["if_else"]
-    IF_ELSE_FIELD_NUMBER: _ClassVar[int]
-    if_else: IfElseBlock
-    def __init__(self, if_else: _Optional[_Union[IfElseBlock, _Mapping]] = ...) -> None: ...
-
-class GateNode(_message.Message):
-    __slots__ = ["approve", "signal", "sleep"]
-    APPROVE_FIELD_NUMBER: _ClassVar[int]
-    SIGNAL_FIELD_NUMBER: _ClassVar[int]
-    SLEEP_FIELD_NUMBER: _ClassVar[int]
-    approve: ApproveCondition
-    signal: SignalCondition
-    sleep: SleepCondition
-    def __init__(self, approve: _Optional[_Union[ApproveCondition, _Mapping]] = ..., signal: _Optional[_Union[SignalCondition, _Mapping]] = ..., sleep: _Optional[_Union[SleepCondition, _Mapping]] = ...) -> None: ...
-
 class IfBlock(_message.Message):
     __slots__ = ["condition", "then_node"]
     CONDITION_FIELD_NUMBER: _ClassVar[int]
     THEN_NODE_FIELD_NUMBER: _ClassVar[int]
     condition: _condition_pb2.BooleanExpression
     then_node: Node
     def __init__(self, condition: _Optional[_Union[_condition_pb2.BooleanExpression, _Mapping]] = ..., then_node: _Optional[_Union[Node, _Mapping]] = ...) -> None: ...
 
 class IfElseBlock(_message.Message):
-    __slots__ = ["case", "else_node", "error", "other"]
+    __slots__ = ["case", "other", "else_node", "error"]
     CASE_FIELD_NUMBER: _ClassVar[int]
+    OTHER_FIELD_NUMBER: _ClassVar[int]
     ELSE_NODE_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
-    OTHER_FIELD_NUMBER: _ClassVar[int]
     case: IfBlock
+    other: _containers.RepeatedCompositeFieldContainer[IfBlock]
     else_node: Node
     error: _types_pb2.Error
-    other: _containers.RepeatedCompositeFieldContainer[IfBlock]
     def __init__(self, case: _Optional[_Union[IfBlock, _Mapping]] = ..., other: _Optional[_Iterable[_Union[IfBlock, _Mapping]]] = ..., else_node: _Optional[_Union[Node, _Mapping]] = ..., error: _Optional[_Union[_types_pb2.Error, _Mapping]] = ...) -> None: ...
 
-class Node(_message.Message):
-    __slots__ = ["branch_node", "gate_node", "id", "inputs", "metadata", "output_aliases", "task_node", "upstream_node_ids", "workflow_node"]
-    BRANCH_NODE_FIELD_NUMBER: _ClassVar[int]
-    GATE_NODE_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    INPUTS_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_ALIASES_FIELD_NUMBER: _ClassVar[int]
-    TASK_NODE_FIELD_NUMBER: _ClassVar[int]
-    UPSTREAM_NODE_IDS_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_NODE_FIELD_NUMBER: _ClassVar[int]
-    branch_node: BranchNode
-    gate_node: GateNode
-    id: str
-    inputs: _containers.RepeatedCompositeFieldContainer[_literals_pb2.Binding]
-    metadata: NodeMetadata
-    output_aliases: _containers.RepeatedCompositeFieldContainer[Alias]
-    task_node: TaskNode
-    upstream_node_ids: _containers.RepeatedScalarFieldContainer[str]
-    workflow_node: WorkflowNode
-    def __init__(self, id: _Optional[str] = ..., metadata: _Optional[_Union[NodeMetadata, _Mapping]] = ..., inputs: _Optional[_Iterable[_Union[_literals_pb2.Binding, _Mapping]]] = ..., upstream_node_ids: _Optional[_Iterable[str]] = ..., output_aliases: _Optional[_Iterable[_Union[Alias, _Mapping]]] = ..., task_node: _Optional[_Union[TaskNode, _Mapping]] = ..., workflow_node: _Optional[_Union[WorkflowNode, _Mapping]] = ..., branch_node: _Optional[_Union[BranchNode, _Mapping]] = ..., gate_node: _Optional[_Union[GateNode, _Mapping]] = ...) -> None: ...
+class BranchNode(_message.Message):
+    __slots__ = ["if_else"]
+    IF_ELSE_FIELD_NUMBER: _ClassVar[int]
+    if_else: IfElseBlock
+    def __init__(self, if_else: _Optional[_Union[IfElseBlock, _Mapping]] = ...) -> None: ...
 
-class NodeMetadata(_message.Message):
-    __slots__ = ["interruptible", "name", "retries", "timeout"]
-    INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    RETRIES_FIELD_NUMBER: _ClassVar[int]
-    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
-    interruptible: bool
-    name: str
-    retries: _literals_pb2.RetryStrategy
-    timeout: _duration_pb2.Duration
-    def __init__(self, name: _Optional[str] = ..., timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., retries: _Optional[_Union[_literals_pb2.RetryStrategy, _Mapping]] = ..., interruptible: bool = ...) -> None: ...
+class TaskNode(_message.Message):
+    __slots__ = ["reference_id", "overrides"]
+    REFERENCE_ID_FIELD_NUMBER: _ClassVar[int]
+    OVERRIDES_FIELD_NUMBER: _ClassVar[int]
+    reference_id: _identifier_pb2.Identifier
+    overrides: TaskNodeOverrides
+    def __init__(self, reference_id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., overrides: _Optional[_Union[TaskNodeOverrides, _Mapping]] = ...) -> None: ...
+
+class WorkflowNode(_message.Message):
+    __slots__ = ["launchplan_ref", "sub_workflow_ref"]
+    LAUNCHPLAN_REF_FIELD_NUMBER: _ClassVar[int]
+    SUB_WORKFLOW_REF_FIELD_NUMBER: _ClassVar[int]
+    launchplan_ref: _identifier_pb2.Identifier
+    sub_workflow_ref: _identifier_pb2.Identifier
+    def __init__(self, launchplan_ref: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., sub_workflow_ref: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ...) -> None: ...
+
+class ApproveCondition(_message.Message):
+    __slots__ = ["signal_id"]
+    SIGNAL_ID_FIELD_NUMBER: _ClassVar[int]
+    signal_id: str
+    def __init__(self, signal_id: _Optional[str] = ...) -> None: ...
 
 class SignalCondition(_message.Message):
-    __slots__ = ["output_variable_name", "signal_id", "type"]
-    OUTPUT_VARIABLE_NAME_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["signal_id", "type", "output_variable_name"]
     SIGNAL_ID_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
-    output_variable_name: str
+    OUTPUT_VARIABLE_NAME_FIELD_NUMBER: _ClassVar[int]
     signal_id: str
     type: _types_pb2.LiteralType
+    output_variable_name: str
     def __init__(self, signal_id: _Optional[str] = ..., type: _Optional[_Union[_types_pb2.LiteralType, _Mapping]] = ..., output_variable_name: _Optional[str] = ...) -> None: ...
 
 class SleepCondition(_message.Message):
     __slots__ = ["duration"]
     DURATION_FIELD_NUMBER: _ClassVar[int]
     duration: _duration_pb2.Duration
     def __init__(self, duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
 
-class TaskNode(_message.Message):
-    __slots__ = ["overrides", "reference_id"]
-    OVERRIDES_FIELD_NUMBER: _ClassVar[int]
-    REFERENCE_ID_FIELD_NUMBER: _ClassVar[int]
-    overrides: TaskNodeOverrides
-    reference_id: _identifier_pb2.Identifier
-    def __init__(self, reference_id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., overrides: _Optional[_Union[TaskNodeOverrides, _Mapping]] = ...) -> None: ...
+class GateNode(_message.Message):
+    __slots__ = ["approve", "signal", "sleep"]
+    APPROVE_FIELD_NUMBER: _ClassVar[int]
+    SIGNAL_FIELD_NUMBER: _ClassVar[int]
+    SLEEP_FIELD_NUMBER: _ClassVar[int]
+    approve: ApproveCondition
+    signal: SignalCondition
+    sleep: SleepCondition
+    def __init__(self, approve: _Optional[_Union[ApproveCondition, _Mapping]] = ..., signal: _Optional[_Union[SignalCondition, _Mapping]] = ..., sleep: _Optional[_Union[SleepCondition, _Mapping]] = ...) -> None: ...
 
-class TaskNodeOverrides(_message.Message):
-    __slots__ = ["resources"]
-    RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    resources: _tasks_pb2.Resources
-    def __init__(self, resources: _Optional[_Union[_tasks_pb2.Resources, _Mapping]] = ...) -> None: ...
+class NodeMetadata(_message.Message):
+    __slots__ = ["name", "timeout", "retries", "interruptible"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
+    RETRIES_FIELD_NUMBER: _ClassVar[int]
+    INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    timeout: _duration_pb2.Duration
+    retries: _literals_pb2.RetryStrategy
+    interruptible: bool
+    def __init__(self, name: _Optional[str] = ..., timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., retries: _Optional[_Union[_literals_pb2.RetryStrategy, _Mapping]] = ..., interruptible: bool = ...) -> None: ...
+
+class Alias(_message.Message):
+    __slots__ = ["var", "alias"]
+    VAR_FIELD_NUMBER: _ClassVar[int]
+    ALIAS_FIELD_NUMBER: _ClassVar[int]
+    var: str
+    alias: str
+    def __init__(self, var: _Optional[str] = ..., alias: _Optional[str] = ...) -> None: ...
+
+class Node(_message.Message):
+    __slots__ = ["id", "metadata", "inputs", "upstream_node_ids", "output_aliases", "task_node", "workflow_node", "branch_node", "gate_node"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
+    UPSTREAM_NODE_IDS_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_ALIASES_FIELD_NUMBER: _ClassVar[int]
+    TASK_NODE_FIELD_NUMBER: _ClassVar[int]
+    WORKFLOW_NODE_FIELD_NUMBER: _ClassVar[int]
+    BRANCH_NODE_FIELD_NUMBER: _ClassVar[int]
+    GATE_NODE_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    metadata: NodeMetadata
+    inputs: _containers.RepeatedCompositeFieldContainer[_literals_pb2.Binding]
+    upstream_node_ids: _containers.RepeatedScalarFieldContainer[str]
+    output_aliases: _containers.RepeatedCompositeFieldContainer[Alias]
+    task_node: TaskNode
+    workflow_node: WorkflowNode
+    branch_node: BranchNode
+    gate_node: GateNode
+    def __init__(self, id: _Optional[str] = ..., metadata: _Optional[_Union[NodeMetadata, _Mapping]] = ..., inputs: _Optional[_Iterable[_Union[_literals_pb2.Binding, _Mapping]]] = ..., upstream_node_ids: _Optional[_Iterable[str]] = ..., output_aliases: _Optional[_Iterable[_Union[Alias, _Mapping]]] = ..., task_node: _Optional[_Union[TaskNode, _Mapping]] = ..., workflow_node: _Optional[_Union[WorkflowNode, _Mapping]] = ..., branch_node: _Optional[_Union[BranchNode, _Mapping]] = ..., gate_node: _Optional[_Union[GateNode, _Mapping]] = ...) -> None: ...
 
 class WorkflowMetadata(_message.Message):
-    __slots__ = ["on_failure", "quality_of_service", "tags"]
+    __slots__ = ["quality_of_service", "on_failure", "tags"]
     class OnFailurePolicy(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        FAIL_IMMEDIATELY: _ClassVar[WorkflowMetadata.OnFailurePolicy]
+        FAIL_AFTER_EXECUTABLE_NODES_COMPLETE: _ClassVar[WorkflowMetadata.OnFailurePolicy]
+    FAIL_IMMEDIATELY: WorkflowMetadata.OnFailurePolicy
+    FAIL_AFTER_EXECUTABLE_NODES_COMPLETE: WorkflowMetadata.OnFailurePolicy
     class TagsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    FAIL_AFTER_EXECUTABLE_NODES_COMPLETE: WorkflowMetadata.OnFailurePolicy
-    FAIL_IMMEDIATELY: WorkflowMetadata.OnFailurePolicy
-    ON_FAILURE_FIELD_NUMBER: _ClassVar[int]
     QUALITY_OF_SERVICE_FIELD_NUMBER: _ClassVar[int]
+    ON_FAILURE_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
-    on_failure: WorkflowMetadata.OnFailurePolicy
     quality_of_service: _execution_pb2.QualityOfService
+    on_failure: WorkflowMetadata.OnFailurePolicy
     tags: _containers.ScalarMap[str, str]
     def __init__(self, quality_of_service: _Optional[_Union[_execution_pb2.QualityOfService, _Mapping]] = ..., on_failure: _Optional[_Union[WorkflowMetadata.OnFailurePolicy, str]] = ..., tags: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class WorkflowMetadataDefaults(_message.Message):
     __slots__ = ["interruptible"]
     INTERRUPTIBLE_FIELD_NUMBER: _ClassVar[int]
     interruptible: bool
     def __init__(self, interruptible: bool = ...) -> None: ...
 
-class WorkflowNode(_message.Message):
-    __slots__ = ["launchplan_ref", "sub_workflow_ref"]
-    LAUNCHPLAN_REF_FIELD_NUMBER: _ClassVar[int]
-    SUB_WORKFLOW_REF_FIELD_NUMBER: _ClassVar[int]
-    launchplan_ref: _identifier_pb2.Identifier
-    sub_workflow_ref: _identifier_pb2.Identifier
-    def __init__(self, launchplan_ref: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., sub_workflow_ref: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ...) -> None: ...
-
 class WorkflowTemplate(_message.Message):
-    __slots__ = ["failure_node", "id", "interface", "metadata", "metadata_defaults", "nodes", "outputs"]
-    FAILURE_NODE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "metadata", "interface", "nodes", "outputs", "failure_node", "metadata_defaults"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    INTERFACE_FIELD_NUMBER: _ClassVar[int]
-    METADATA_DEFAULTS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
+    INTERFACE_FIELD_NUMBER: _ClassVar[int]
     NODES_FIELD_NUMBER: _ClassVar[int]
     OUTPUTS_FIELD_NUMBER: _ClassVar[int]
-    failure_node: Node
+    FAILURE_NODE_FIELD_NUMBER: _ClassVar[int]
+    METADATA_DEFAULTS_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.Identifier
-    interface: _interface_pb2.TypedInterface
     metadata: WorkflowMetadata
-    metadata_defaults: WorkflowMetadataDefaults
+    interface: _interface_pb2.TypedInterface
     nodes: _containers.RepeatedCompositeFieldContainer[Node]
     outputs: _containers.RepeatedCompositeFieldContainer[_literals_pb2.Binding]
+    failure_node: Node
+    metadata_defaults: WorkflowMetadataDefaults
     def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., metadata: _Optional[_Union[WorkflowMetadata, _Mapping]] = ..., interface: _Optional[_Union[_interface_pb2.TypedInterface, _Mapping]] = ..., nodes: _Optional[_Iterable[_Union[Node, _Mapping]]] = ..., outputs: _Optional[_Iterable[_Union[_literals_pb2.Binding, _Mapping]]] = ..., failure_node: _Optional[_Union[Node, _Mapping]] = ..., metadata_defaults: _Optional[_Union[WorkflowMetadataDefaults, _Mapping]] = ...) -> None: ...
+
+class TaskNodeOverrides(_message.Message):
+    __slots__ = ["resources"]
+    RESOURCES_FIELD_NUMBER: _ClassVar[int]
+    resources: _tasks_pb2.Resources
+    def __init__(self, resources: _Optional[_Union[_tasks_pb2.Resources, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,100 +14,101 @@
 from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&flyteidl/datacatalog/datacatalog.proto\x12\x0b\x64\x61tacatalog\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"F\n\x14\x43reateDatasetRequest\x12.\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x14.datacatalog.DatasetR\x07\x64\x61taset\"\x17\n\x15\x43reateDatasetResponse\"E\n\x11GetDatasetRequest\x12\x30\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\x07\x64\x61taset\"D\n\x12GetDatasetResponse\x12.\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x14.datacatalog.DatasetR\x07\x64\x61taset\"\x96\x01\n\x12GetArtifactRequest\x12\x30\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\x07\x64\x61taset\x12!\n\x0b\x61rtifact_id\x18\x02 \x01(\tH\x00R\nartifactId\x12\x1b\n\x08tag_name\x18\x03 \x01(\tH\x00R\x07tagNameB\x0e\n\x0cquery_handle\"H\n\x13GetArtifactResponse\x12\x31\n\x08\x61rtifact\x18\x01 \x01(\x0b\x32\x15.datacatalog.ArtifactR\x08\x61rtifact\"J\n\x15\x43reateArtifactRequest\x12\x31\n\x08\x61rtifact\x18\x01 \x01(\x0b\x32\x15.datacatalog.ArtifactR\x08\x61rtifact\"\x18\n\x16\x43reateArtifactResponse\"3\n\rAddTagRequest\x12\"\n\x03tag\x18\x01 \x01(\x0b\x32\x10.datacatalog.TagR\x03tag\"\x10\n\x0e\x41\x64\x64TagResponse\"\xbf\x01\n\x14ListArtifactsRequest\x12\x30\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\x07\x64\x61taset\x12\x35\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x1d.datacatalog.FilterExpressionR\x06\x66ilter\x12>\n\npagination\x18\x03 \x01(\x0b\x32\x1e.datacatalog.PaginationOptionsR\npagination\"k\n\x15ListArtifactsResponse\x12\x33\n\tartifacts\x18\x01 \x03(\x0b\x32\x15.datacatalog.ArtifactR\tartifacts\x12\x1d\n\nnext_token\x18\x02 \x01(\tR\tnextToken\"\x8c\x01\n\x13ListDatasetsRequest\x12\x35\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1d.datacatalog.FilterExpressionR\x06\x66ilter\x12>\n\npagination\x18\x02 \x01(\x0b\x32\x1e.datacatalog.PaginationOptionsR\npagination\"g\n\x14ListDatasetsResponse\x12\x30\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\x14.datacatalog.DatasetR\x08\x64\x61tasets\x12\x1d\n\nnext_token\x18\x02 \x01(\tR\tnextToken\"\xc8\x01\n\x15UpdateArtifactRequest\x12\x30\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\x07\x64\x61taset\x12!\n\x0b\x61rtifact_id\x18\x02 \x01(\tH\x00R\nartifactId\x12\x1b\n\x08tag_name\x18\x03 \x01(\tH\x00R\x07tagName\x12-\n\x04\x64\x61ta\x18\x04 \x03(\x0b\x32\x19.datacatalog.ArtifactDataR\x04\x64\x61taB\x0e\n\x0cquery_handle\"9\n\x16UpdateArtifactResponse\x12\x1f\n\x0b\x61rtifact_id\x18\x01 \x01(\tR\nartifactId\"a\n\rReservationID\x12\x35\n\ndataset_id\x18\x01 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\tdatasetId\x12\x19\n\x08tag_name\x18\x02 \x01(\tR\x07tagName\"\xc7\x01\n\x1dGetOrExtendReservationRequest\x12\x41\n\x0ereservation_id\x18\x01 \x01(\x0b\x32\x1a.datacatalog.ReservationIDR\rreservationId\x12\x19\n\x08owner_id\x18\x02 \x01(\tR\x07ownerId\x12H\n\x12heartbeat_interval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11heartbeatInterval\"\xa3\x02\n\x0bReservation\x12\x41\n\x0ereservation_id\x18\x01 \x01(\x0b\x32\x1a.datacatalog.ReservationIDR\rreservationId\x12\x19\n\x08owner_id\x18\x02 \x01(\tR\x07ownerId\x12H\n\x12heartbeat_interval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11heartbeatInterval\x12\x39\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12\x31\n\x08metadata\x18\x06 \x01(\x0b\x32\x15.datacatalog.MetadataR\x08metadata\"\\\n\x1eGetOrExtendReservationResponse\x12:\n\x0breservation\x18\x01 \x01(\x0b\x32\x18.datacatalog.ReservationR\x0breservation\"y\n\x19ReleaseReservationRequest\x12\x41\n\x0ereservation_id\x18\x01 \x01(\x0b\x32\x1a.datacatalog.ReservationIDR\rreservationId\x12\x19\n\x08owner_id\x18\x02 \x01(\tR\x07ownerId\"\x1c\n\x1aReleaseReservationResponse\"\x8a\x01\n\x07\x44\x61taset\x12&\n\x02id\x18\x01 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\x02id\x12\x31\n\x08metadata\x18\x02 \x01(\x0b\x32\x15.datacatalog.MetadataR\x08metadata\x12$\n\rpartitionKeys\x18\x03 \x03(\tR\rpartitionKeys\"3\n\tPartition\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"\x7f\n\tDatasetID\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x16\n\x06\x64omain\x18\x03 \x01(\tR\x06\x64omain\x12\x18\n\x07version\x18\x04 \x01(\tR\x07version\x12\x12\n\x04UUID\x18\x05 \x01(\tR\x04UUID\"\xc7\x02\n\x08\x41rtifact\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x30\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\x07\x64\x61taset\x12-\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32\x19.datacatalog.ArtifactDataR\x04\x64\x61ta\x12\x31\n\x08metadata\x18\x04 \x01(\x0b\x32\x15.datacatalog.MetadataR\x08metadata\x12\x36\n\npartitions\x18\x05 \x03(\x0b\x32\x16.datacatalog.PartitionR\npartitions\x12$\n\x04tags\x18\x06 \x03(\x0b\x32\x10.datacatalog.TagR\x04tags\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"P\n\x0c\x41rtifactData\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.flyteidl.core.LiteralR\x05value\"l\n\x03Tag\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1f\n\x0b\x61rtifact_id\x18\x02 \x01(\tR\nartifactId\x12\x30\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32\x16.datacatalog.DatasetIDR\x07\x64\x61taset\"\x81\x01\n\x08Metadata\x12:\n\x07key_map\x18\x01 \x03(\x0b\x32!.datacatalog.Metadata.KeyMapEntryR\x06keyMap\x1a\x39\n\x0bKeyMapEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"O\n\x10\x46ilterExpression\x12;\n\x07\x66ilters\x18\x01 \x03(\x0b\x32!.datacatalog.SinglePropertyFilterR\x07\x66ilters\"\xce\x03\n\x14SinglePropertyFilter\x12?\n\ntag_filter\x18\x01 \x01(\x0b\x32\x1e.datacatalog.TagPropertyFilterH\x00R\ttagFilter\x12Q\n\x10partition_filter\x18\x02 \x01(\x0b\x32$.datacatalog.PartitionPropertyFilterH\x00R\x0fpartitionFilter\x12N\n\x0f\x61rtifact_filter\x18\x03 \x01(\x0b\x32#.datacatalog.ArtifactPropertyFilterH\x00R\x0e\x61rtifactFilter\x12K\n\x0e\x64\x61taset_filter\x18\x04 \x01(\x0b\x32\".datacatalog.DatasetPropertyFilterH\x00R\rdatasetFilter\x12P\n\x08operator\x18\n \x01(\x0e\x32\x34.datacatalog.SinglePropertyFilter.ComparisonOperatorR\x08operator\" \n\x12\x43omparisonOperator\x12\n\n\x06\x45QUALS\x10\x00\x42\x11\n\x0fproperty_filter\"G\n\x16\x41rtifactPropertyFilter\x12!\n\x0b\x61rtifact_id\x18\x01 \x01(\tH\x00R\nartifactIdB\n\n\x08property\"<\n\x11TagPropertyFilter\x12\x1b\n\x08tag_name\x18\x01 \x01(\tH\x00R\x07tagNameB\n\n\x08property\"[\n\x17PartitionPropertyFilter\x12\x34\n\x07key_val\x18\x01 \x01(\x0b\x32\x19.datacatalog.KeyValuePairH\x00R\x06keyValB\n\n\x08property\"6\n\x0cKeyValuePair\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"\x8b\x01\n\x15\x44\x61tasetPropertyFilter\x12\x1a\n\x07project\x18\x01 \x01(\tH\x00R\x07project\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x18\n\x06\x64omain\x18\x03 \x01(\tH\x00R\x06\x64omain\x12\x1a\n\x07version\x18\x04 \x01(\tH\x00R\x07versionB\n\n\x08property\"\x93\x02\n\x11PaginationOptions\x12\x14\n\x05limit\x18\x01 \x01(\rR\x05limit\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\x12@\n\x07sortKey\x18\x03 \x01(\x0e\x32&.datacatalog.PaginationOptions.SortKeyR\x07sortKey\x12\x46\n\tsortOrder\x18\x04 \x01(\x0e\x32(.datacatalog.PaginationOptions.SortOrderR\tsortOrder\"*\n\tSortOrder\x12\x0e\n\nDESCENDING\x10\x00\x12\r\n\tASCENDING\x10\x01\"\x1c\n\x07SortKey\x12\x11\n\rCREATION_TIME\x10\x00\x32\x86\x07\n\x0b\x44\x61taCatalog\x12V\n\rCreateDataset\x12!.datacatalog.CreateDatasetRequest\x1a\".datacatalog.CreateDatasetResponse\x12M\n\nGetDataset\x12\x1e.datacatalog.GetDatasetRequest\x1a\x1f.datacatalog.GetDatasetResponse\x12Y\n\x0e\x43reateArtifact\x12\".datacatalog.CreateArtifactRequest\x1a#.datacatalog.CreateArtifactResponse\x12P\n\x0bGetArtifact\x12\x1f.datacatalog.GetArtifactRequest\x1a .datacatalog.GetArtifactResponse\x12\x41\n\x06\x41\x64\x64Tag\x12\x1a.datacatalog.AddTagRequest\x1a\x1b.datacatalog.AddTagResponse\x12V\n\rListArtifacts\x12!.datacatalog.ListArtifactsRequest\x1a\".datacatalog.ListArtifactsResponse\x12S\n\x0cListDatasets\x12 .datacatalog.ListDatasetsRequest\x1a!.datacatalog.ListDatasetsResponse\x12Y\n\x0eUpdateArtifact\x12\".datacatalog.UpdateArtifactRequest\x1a#.datacatalog.UpdateArtifactResponse\x12q\n\x16GetOrExtendReservation\x12*.datacatalog.GetOrExtendReservationRequest\x1a+.datacatalog.GetOrExtendReservationResponse\x12\x65\n\x12ReleaseReservation\x12&.datacatalog.ReleaseReservationRequest\x1a\'.datacatalog.ReleaseReservationResponseB\xac\x01\n\x0f\x63om.datacatalogB\x10\x44\x61tacatalogProtoP\x01Z;github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/datacatalog\xa2\x02\x03\x44XX\xaa\x02\x0b\x44\x61tacatalog\xca\x02\x0b\x44\x61tacatalog\xe2\x02\x17\x44\x61tacatalog\\GPBMetadata\xea\x02\x0b\x44\x61tacatalogb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.datacatalog.datacatalog_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.datacatalog.datacatalog_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.datacatalogB\020DatacatalogProtoP\001Z;github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/datacatalog\242\002\003DXX\252\002\013Datacatalog\312\002\013Datacatalog\342\002\027Datacatalog\\GPBMetadata\352\002\013Datacatalog'
   _METADATA_KEYMAPENTRY._options = None
   _METADATA_KEYMAPENTRY._serialized_options = b'8\001'
-  _CREATEDATASETREQUEST._serialized_start=150
-  _CREATEDATASETREQUEST._serialized_end=220
-  _CREATEDATASETRESPONSE._serialized_start=222
-  _CREATEDATASETRESPONSE._serialized_end=245
-  _GETDATASETREQUEST._serialized_start=247
-  _GETDATASETREQUEST._serialized_end=316
-  _GETDATASETRESPONSE._serialized_start=318
-  _GETDATASETRESPONSE._serialized_end=386
-  _GETARTIFACTREQUEST._serialized_start=389
-  _GETARTIFACTREQUEST._serialized_end=539
-  _GETARTIFACTRESPONSE._serialized_start=541
-  _GETARTIFACTRESPONSE._serialized_end=613
-  _CREATEARTIFACTREQUEST._serialized_start=615
-  _CREATEARTIFACTREQUEST._serialized_end=689
-  _CREATEARTIFACTRESPONSE._serialized_start=691
-  _CREATEARTIFACTRESPONSE._serialized_end=715
-  _ADDTAGREQUEST._serialized_start=717
-  _ADDTAGREQUEST._serialized_end=768
-  _ADDTAGRESPONSE._serialized_start=770
-  _ADDTAGRESPONSE._serialized_end=786
-  _LISTARTIFACTSREQUEST._serialized_start=789
-  _LISTARTIFACTSREQUEST._serialized_end=980
-  _LISTARTIFACTSRESPONSE._serialized_start=982
-  _LISTARTIFACTSRESPONSE._serialized_end=1089
-  _LISTDATASETSREQUEST._serialized_start=1092
-  _LISTDATASETSREQUEST._serialized_end=1232
-  _LISTDATASETSRESPONSE._serialized_start=1234
-  _LISTDATASETSRESPONSE._serialized_end=1337
-  _UPDATEARTIFACTREQUEST._serialized_start=1340
-  _UPDATEARTIFACTREQUEST._serialized_end=1540
-  _UPDATEARTIFACTRESPONSE._serialized_start=1542
-  _UPDATEARTIFACTRESPONSE._serialized_end=1599
-  _RESERVATIONID._serialized_start=1601
-  _RESERVATIONID._serialized_end=1698
-  _GETOREXTENDRESERVATIONREQUEST._serialized_start=1701
-  _GETOREXTENDRESERVATIONREQUEST._serialized_end=1900
-  _RESERVATION._serialized_start=1903
-  _RESERVATION._serialized_end=2194
-  _GETOREXTENDRESERVATIONRESPONSE._serialized_start=2196
-  _GETOREXTENDRESERVATIONRESPONSE._serialized_end=2288
-  _RELEASERESERVATIONREQUEST._serialized_start=2290
-  _RELEASERESERVATIONREQUEST._serialized_end=2411
-  _RELEASERESERVATIONRESPONSE._serialized_start=2413
-  _RELEASERESERVATIONRESPONSE._serialized_end=2441
-  _DATASET._serialized_start=2444
-  _DATASET._serialized_end=2582
-  _PARTITION._serialized_start=2584
-  _PARTITION._serialized_end=2635
-  _DATASETID._serialized_start=2637
-  _DATASETID._serialized_end=2764
-  _ARTIFACT._serialized_start=2767
-  _ARTIFACT._serialized_end=3094
-  _ARTIFACTDATA._serialized_start=3096
-  _ARTIFACTDATA._serialized_end=3176
-  _TAG._serialized_start=3178
-  _TAG._serialized_end=3286
-  _METADATA._serialized_start=3289
-  _METADATA._serialized_end=3418
-  _METADATA_KEYMAPENTRY._serialized_start=3361
-  _METADATA_KEYMAPENTRY._serialized_end=3418
-  _FILTEREXPRESSION._serialized_start=3420
-  _FILTEREXPRESSION._serialized_end=3499
-  _SINGLEPROPERTYFILTER._serialized_start=3502
-  _SINGLEPROPERTYFILTER._serialized_end=3964
-  _SINGLEPROPERTYFILTER_COMPARISONOPERATOR._serialized_start=3913
-  _SINGLEPROPERTYFILTER_COMPARISONOPERATOR._serialized_end=3945
-  _ARTIFACTPROPERTYFILTER._serialized_start=3966
-  _ARTIFACTPROPERTYFILTER._serialized_end=4037
-  _TAGPROPERTYFILTER._serialized_start=4039
-  _TAGPROPERTYFILTER._serialized_end=4099
-  _PARTITIONPROPERTYFILTER._serialized_start=4101
-  _PARTITIONPROPERTYFILTER._serialized_end=4192
-  _KEYVALUEPAIR._serialized_start=4194
-  _KEYVALUEPAIR._serialized_end=4248
-  _DATASETPROPERTYFILTER._serialized_start=4251
-  _DATASETPROPERTYFILTER._serialized_end=4390
-  _PAGINATIONOPTIONS._serialized_start=4393
-  _PAGINATIONOPTIONS._serialized_end=4668
-  _PAGINATIONOPTIONS_SORTORDER._serialized_start=4596
-  _PAGINATIONOPTIONS_SORTORDER._serialized_end=4638
-  _PAGINATIONOPTIONS_SORTKEY._serialized_start=4640
-  _PAGINATIONOPTIONS_SORTKEY._serialized_end=4668
-  _DATACATALOG._serialized_start=4671
-  _DATACATALOG._serialized_end=5573
+  _globals['_CREATEDATASETREQUEST']._serialized_start=150
+  _globals['_CREATEDATASETREQUEST']._serialized_end=220
+  _globals['_CREATEDATASETRESPONSE']._serialized_start=222
+  _globals['_CREATEDATASETRESPONSE']._serialized_end=245
+  _globals['_GETDATASETREQUEST']._serialized_start=247
+  _globals['_GETDATASETREQUEST']._serialized_end=316
+  _globals['_GETDATASETRESPONSE']._serialized_start=318
+  _globals['_GETDATASETRESPONSE']._serialized_end=386
+  _globals['_GETARTIFACTREQUEST']._serialized_start=389
+  _globals['_GETARTIFACTREQUEST']._serialized_end=539
+  _globals['_GETARTIFACTRESPONSE']._serialized_start=541
+  _globals['_GETARTIFACTRESPONSE']._serialized_end=613
+  _globals['_CREATEARTIFACTREQUEST']._serialized_start=615
+  _globals['_CREATEARTIFACTREQUEST']._serialized_end=689
+  _globals['_CREATEARTIFACTRESPONSE']._serialized_start=691
+  _globals['_CREATEARTIFACTRESPONSE']._serialized_end=715
+  _globals['_ADDTAGREQUEST']._serialized_start=717
+  _globals['_ADDTAGREQUEST']._serialized_end=768
+  _globals['_ADDTAGRESPONSE']._serialized_start=770
+  _globals['_ADDTAGRESPONSE']._serialized_end=786
+  _globals['_LISTARTIFACTSREQUEST']._serialized_start=789
+  _globals['_LISTARTIFACTSREQUEST']._serialized_end=980
+  _globals['_LISTARTIFACTSRESPONSE']._serialized_start=982
+  _globals['_LISTARTIFACTSRESPONSE']._serialized_end=1089
+  _globals['_LISTDATASETSREQUEST']._serialized_start=1092
+  _globals['_LISTDATASETSREQUEST']._serialized_end=1232
+  _globals['_LISTDATASETSRESPONSE']._serialized_start=1234
+  _globals['_LISTDATASETSRESPONSE']._serialized_end=1337
+  _globals['_UPDATEARTIFACTREQUEST']._serialized_start=1340
+  _globals['_UPDATEARTIFACTREQUEST']._serialized_end=1540
+  _globals['_UPDATEARTIFACTRESPONSE']._serialized_start=1542
+  _globals['_UPDATEARTIFACTRESPONSE']._serialized_end=1599
+  _globals['_RESERVATIONID']._serialized_start=1601
+  _globals['_RESERVATIONID']._serialized_end=1698
+  _globals['_GETOREXTENDRESERVATIONREQUEST']._serialized_start=1701
+  _globals['_GETOREXTENDRESERVATIONREQUEST']._serialized_end=1900
+  _globals['_RESERVATION']._serialized_start=1903
+  _globals['_RESERVATION']._serialized_end=2194
+  _globals['_GETOREXTENDRESERVATIONRESPONSE']._serialized_start=2196
+  _globals['_GETOREXTENDRESERVATIONRESPONSE']._serialized_end=2288
+  _globals['_RELEASERESERVATIONREQUEST']._serialized_start=2290
+  _globals['_RELEASERESERVATIONREQUEST']._serialized_end=2411
+  _globals['_RELEASERESERVATIONRESPONSE']._serialized_start=2413
+  _globals['_RELEASERESERVATIONRESPONSE']._serialized_end=2441
+  _globals['_DATASET']._serialized_start=2444
+  _globals['_DATASET']._serialized_end=2582
+  _globals['_PARTITION']._serialized_start=2584
+  _globals['_PARTITION']._serialized_end=2635
+  _globals['_DATASETID']._serialized_start=2637
+  _globals['_DATASETID']._serialized_end=2764
+  _globals['_ARTIFACT']._serialized_start=2767
+  _globals['_ARTIFACT']._serialized_end=3094
+  _globals['_ARTIFACTDATA']._serialized_start=3096
+  _globals['_ARTIFACTDATA']._serialized_end=3176
+  _globals['_TAG']._serialized_start=3178
+  _globals['_TAG']._serialized_end=3286
+  _globals['_METADATA']._serialized_start=3289
+  _globals['_METADATA']._serialized_end=3418
+  _globals['_METADATA_KEYMAPENTRY']._serialized_start=3361
+  _globals['_METADATA_KEYMAPENTRY']._serialized_end=3418
+  _globals['_FILTEREXPRESSION']._serialized_start=3420
+  _globals['_FILTEREXPRESSION']._serialized_end=3499
+  _globals['_SINGLEPROPERTYFILTER']._serialized_start=3502
+  _globals['_SINGLEPROPERTYFILTER']._serialized_end=3964
+  _globals['_SINGLEPROPERTYFILTER_COMPARISONOPERATOR']._serialized_start=3913
+  _globals['_SINGLEPROPERTYFILTER_COMPARISONOPERATOR']._serialized_end=3945
+  _globals['_ARTIFACTPROPERTYFILTER']._serialized_start=3966
+  _globals['_ARTIFACTPROPERTYFILTER']._serialized_end=4037
+  _globals['_TAGPROPERTYFILTER']._serialized_start=4039
+  _globals['_TAGPROPERTYFILTER']._serialized_end=4099
+  _globals['_PARTITIONPROPERTYFILTER']._serialized_start=4101
+  _globals['_PARTITIONPROPERTYFILTER']._serialized_end=4192
+  _globals['_KEYVALUEPAIR']._serialized_start=4194
+  _globals['_KEYVALUEPAIR']._serialized_end=4248
+  _globals['_DATASETPROPERTYFILTER']._serialized_start=4251
+  _globals['_DATASETPROPERTYFILTER']._serialized_end=4390
+  _globals['_PAGINATIONOPTIONS']._serialized_start=4393
+  _globals['_PAGINATIONOPTIONS']._serialized_end=4668
+  _globals['_PAGINATIONOPTIONS_SORTORDER']._serialized_start=4596
+  _globals['_PAGINATIONOPTIONS_SORTORDER']._serialized_end=4638
+  _globals['_PAGINATIONOPTIONS_SORTKEY']._serialized_start=4640
+  _globals['_PAGINATIONOPTIONS_SORTKEY']._serialized_end=4668
+  _globals['_DATACATALOG']._serialized_start=4671
+  _globals['_DATACATALOG']._serialized_end=5573
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -5,169 +5,71 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class AddTagRequest(_message.Message):
-    __slots__ = ["tag"]
-    TAG_FIELD_NUMBER: _ClassVar[int]
-    tag: Tag
-    def __init__(self, tag: _Optional[_Union[Tag, _Mapping]] = ...) -> None: ...
-
-class AddTagResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class Artifact(_message.Message):
-    __slots__ = ["created_at", "data", "dataset", "id", "metadata", "partitions", "tags"]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    DATASET_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    PARTITIONS_FIELD_NUMBER: _ClassVar[int]
-    TAGS_FIELD_NUMBER: _ClassVar[int]
-    created_at: _timestamp_pb2.Timestamp
-    data: _containers.RepeatedCompositeFieldContainer[ArtifactData]
-    dataset: DatasetID
-    id: str
-    metadata: Metadata
-    partitions: _containers.RepeatedCompositeFieldContainer[Partition]
-    tags: _containers.RepeatedCompositeFieldContainer[Tag]
-    def __init__(self, id: _Optional[str] = ..., dataset: _Optional[_Union[DatasetID, _Mapping]] = ..., data: _Optional[_Iterable[_Union[ArtifactData, _Mapping]]] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ..., partitions: _Optional[_Iterable[_Union[Partition, _Mapping]]] = ..., tags: _Optional[_Iterable[_Union[Tag, _Mapping]]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
-
-class ArtifactData(_message.Message):
-    __slots__ = ["name", "value"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    value: _literals_pb2.Literal
-    def __init__(self, name: _Optional[str] = ..., value: _Optional[_Union[_literals_pb2.Literal, _Mapping]] = ...) -> None: ...
-
-class ArtifactPropertyFilter(_message.Message):
-    __slots__ = ["artifact_id"]
-    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
-    artifact_id: str
-    def __init__(self, artifact_id: _Optional[str] = ...) -> None: ...
-
-class CreateArtifactRequest(_message.Message):
-    __slots__ = ["artifact"]
-    ARTIFACT_FIELD_NUMBER: _ClassVar[int]
-    artifact: Artifact
-    def __init__(self, artifact: _Optional[_Union[Artifact, _Mapping]] = ...) -> None: ...
-
-class CreateArtifactResponse(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
 class CreateDatasetRequest(_message.Message):
     __slots__ = ["dataset"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     dataset: Dataset
     def __init__(self, dataset: _Optional[_Union[Dataset, _Mapping]] = ...) -> None: ...
 
 class CreateDatasetResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class Dataset(_message.Message):
-    __slots__ = ["id", "metadata", "partitionKeys"]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
-    PARTITIONKEYS_FIELD_NUMBER: _ClassVar[int]
-    id: DatasetID
-    metadata: Metadata
-    partitionKeys: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, id: _Optional[_Union[DatasetID, _Mapping]] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ..., partitionKeys: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class DatasetID(_message.Message):
-    __slots__ = ["UUID", "domain", "name", "project", "version"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    UUID: str
-    UUID_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    name: str
-    project: str
-    version: str
-    def __init__(self, project: _Optional[str] = ..., name: _Optional[str] = ..., domain: _Optional[str] = ..., version: _Optional[str] = ..., UUID: _Optional[str] = ...) -> None: ...
-
-class DatasetPropertyFilter(_message.Message):
-    __slots__ = ["domain", "name", "project", "version"]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    domain: str
-    name: str
-    project: str
-    version: str
-    def __init__(self, project: _Optional[str] = ..., name: _Optional[str] = ..., domain: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
+class GetDatasetRequest(_message.Message):
+    __slots__ = ["dataset"]
+    DATASET_FIELD_NUMBER: _ClassVar[int]
+    dataset: DatasetID
+    def __init__(self, dataset: _Optional[_Union[DatasetID, _Mapping]] = ...) -> None: ...
 
-class FilterExpression(_message.Message):
-    __slots__ = ["filters"]
-    FILTERS_FIELD_NUMBER: _ClassVar[int]
-    filters: _containers.RepeatedCompositeFieldContainer[SinglePropertyFilter]
-    def __init__(self, filters: _Optional[_Iterable[_Union[SinglePropertyFilter, _Mapping]]] = ...) -> None: ...
+class GetDatasetResponse(_message.Message):
+    __slots__ = ["dataset"]
+    DATASET_FIELD_NUMBER: _ClassVar[int]
+    dataset: Dataset
+    def __init__(self, dataset: _Optional[_Union[Dataset, _Mapping]] = ...) -> None: ...
 
 class GetArtifactRequest(_message.Message):
-    __slots__ = ["artifact_id", "dataset", "tag_name"]
-    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["dataset", "artifact_id", "tag_name"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
+    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
     TAG_NAME_FIELD_NUMBER: _ClassVar[int]
-    artifact_id: str
     dataset: DatasetID
+    artifact_id: str
     tag_name: str
     def __init__(self, dataset: _Optional[_Union[DatasetID, _Mapping]] = ..., artifact_id: _Optional[str] = ..., tag_name: _Optional[str] = ...) -> None: ...
 
 class GetArtifactResponse(_message.Message):
     __slots__ = ["artifact"]
     ARTIFACT_FIELD_NUMBER: _ClassVar[int]
     artifact: Artifact
     def __init__(self, artifact: _Optional[_Union[Artifact, _Mapping]] = ...) -> None: ...
 
-class GetDatasetRequest(_message.Message):
-    __slots__ = ["dataset"]
-    DATASET_FIELD_NUMBER: _ClassVar[int]
-    dataset: DatasetID
-    def __init__(self, dataset: _Optional[_Union[DatasetID, _Mapping]] = ...) -> None: ...
-
-class GetDatasetResponse(_message.Message):
-    __slots__ = ["dataset"]
-    DATASET_FIELD_NUMBER: _ClassVar[int]
-    dataset: Dataset
-    def __init__(self, dataset: _Optional[_Union[Dataset, _Mapping]] = ...) -> None: ...
+class CreateArtifactRequest(_message.Message):
+    __slots__ = ["artifact"]
+    ARTIFACT_FIELD_NUMBER: _ClassVar[int]
+    artifact: Artifact
+    def __init__(self, artifact: _Optional[_Union[Artifact, _Mapping]] = ...) -> None: ...
 
-class GetOrExtendReservationRequest(_message.Message):
-    __slots__ = ["heartbeat_interval", "owner_id", "reservation_id"]
-    HEARTBEAT_INTERVAL_FIELD_NUMBER: _ClassVar[int]
-    OWNER_ID_FIELD_NUMBER: _ClassVar[int]
-    RESERVATION_ID_FIELD_NUMBER: _ClassVar[int]
-    heartbeat_interval: _duration_pb2.Duration
-    owner_id: str
-    reservation_id: ReservationID
-    def __init__(self, reservation_id: _Optional[_Union[ReservationID, _Mapping]] = ..., owner_id: _Optional[str] = ..., heartbeat_interval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
+class CreateArtifactResponse(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
-class GetOrExtendReservationResponse(_message.Message):
-    __slots__ = ["reservation"]
-    RESERVATION_FIELD_NUMBER: _ClassVar[int]
-    reservation: Reservation
-    def __init__(self, reservation: _Optional[_Union[Reservation, _Mapping]] = ...) -> None: ...
+class AddTagRequest(_message.Message):
+    __slots__ = ["tag"]
+    TAG_FIELD_NUMBER: _ClassVar[int]
+    tag: Tag
+    def __init__(self, tag: _Optional[_Union[Tag, _Mapping]] = ...) -> None: ...
 
-class KeyValuePair(_message.Message):
-    __slots__ = ["key", "value"]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    key: str
-    value: str
-    def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+class AddTagResponse(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
 
 class ListArtifactsRequest(_message.Message):
     __slots__ = ["dataset", "filter", "pagination"]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATION_FIELD_NUMBER: _ClassVar[int]
     dataset: DatasetID
@@ -195,137 +97,239 @@
     __slots__ = ["datasets", "next_token"]
     DATASETS_FIELD_NUMBER: _ClassVar[int]
     NEXT_TOKEN_FIELD_NUMBER: _ClassVar[int]
     datasets: _containers.RepeatedCompositeFieldContainer[Dataset]
     next_token: str
     def __init__(self, datasets: _Optional[_Iterable[_Union[Dataset, _Mapping]]] = ..., next_token: _Optional[str] = ...) -> None: ...
 
-class Metadata(_message.Message):
-    __slots__ = ["key_map"]
-    class KeyMapEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: str
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    KEY_MAP_FIELD_NUMBER: _ClassVar[int]
-    key_map: _containers.ScalarMap[str, str]
-    def __init__(self, key_map: _Optional[_Mapping[str, str]] = ...) -> None: ...
-
-class PaginationOptions(_message.Message):
-    __slots__ = ["limit", "sortKey", "sortOrder", "token"]
-    class SortKey(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class SortOrder(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    ASCENDING: PaginationOptions.SortOrder
-    CREATION_TIME: PaginationOptions.SortKey
-    DESCENDING: PaginationOptions.SortOrder
-    LIMIT_FIELD_NUMBER: _ClassVar[int]
-    SORTKEY_FIELD_NUMBER: _ClassVar[int]
-    SORTORDER_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_FIELD_NUMBER: _ClassVar[int]
-    limit: int
-    sortKey: PaginationOptions.SortKey
-    sortOrder: PaginationOptions.SortOrder
-    token: str
-    def __init__(self, limit: _Optional[int] = ..., token: _Optional[str] = ..., sortKey: _Optional[_Union[PaginationOptions.SortKey, str]] = ..., sortOrder: _Optional[_Union[PaginationOptions.SortOrder, str]] = ...) -> None: ...
+class UpdateArtifactRequest(_message.Message):
+    __slots__ = ["dataset", "artifact_id", "tag_name", "data"]
+    DATASET_FIELD_NUMBER: _ClassVar[int]
+    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
+    TAG_NAME_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    dataset: DatasetID
+    artifact_id: str
+    tag_name: str
+    data: _containers.RepeatedCompositeFieldContainer[ArtifactData]
+    def __init__(self, dataset: _Optional[_Union[DatasetID, _Mapping]] = ..., artifact_id: _Optional[str] = ..., tag_name: _Optional[str] = ..., data: _Optional[_Iterable[_Union[ArtifactData, _Mapping]]] = ...) -> None: ...
 
-class Partition(_message.Message):
-    __slots__ = ["key", "value"]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    VALUE_FIELD_NUMBER: _ClassVar[int]
-    key: str
-    value: str
-    def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+class UpdateArtifactResponse(_message.Message):
+    __slots__ = ["artifact_id"]
+    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
+    artifact_id: str
+    def __init__(self, artifact_id: _Optional[str] = ...) -> None: ...
 
-class PartitionPropertyFilter(_message.Message):
-    __slots__ = ["key_val"]
-    KEY_VAL_FIELD_NUMBER: _ClassVar[int]
-    key_val: KeyValuePair
-    def __init__(self, key_val: _Optional[_Union[KeyValuePair, _Mapping]] = ...) -> None: ...
+class ReservationID(_message.Message):
+    __slots__ = ["dataset_id", "tag_name"]
+    DATASET_ID_FIELD_NUMBER: _ClassVar[int]
+    TAG_NAME_FIELD_NUMBER: _ClassVar[int]
+    dataset_id: DatasetID
+    tag_name: str
+    def __init__(self, dataset_id: _Optional[_Union[DatasetID, _Mapping]] = ..., tag_name: _Optional[str] = ...) -> None: ...
 
-class ReleaseReservationRequest(_message.Message):
-    __slots__ = ["owner_id", "reservation_id"]
+class GetOrExtendReservationRequest(_message.Message):
+    __slots__ = ["reservation_id", "owner_id", "heartbeat_interval"]
+    RESERVATION_ID_FIELD_NUMBER: _ClassVar[int]
     OWNER_ID_FIELD_NUMBER: _ClassVar[int]
+    HEARTBEAT_INTERVAL_FIELD_NUMBER: _ClassVar[int]
+    reservation_id: ReservationID
+    owner_id: str
+    heartbeat_interval: _duration_pb2.Duration
+    def __init__(self, reservation_id: _Optional[_Union[ReservationID, _Mapping]] = ..., owner_id: _Optional[str] = ..., heartbeat_interval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
+
+class Reservation(_message.Message):
+    __slots__ = ["reservation_id", "owner_id", "heartbeat_interval", "expires_at", "metadata"]
     RESERVATION_ID_FIELD_NUMBER: _ClassVar[int]
+    OWNER_ID_FIELD_NUMBER: _ClassVar[int]
+    HEARTBEAT_INTERVAL_FIELD_NUMBER: _ClassVar[int]
+    EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    reservation_id: ReservationID
     owner_id: str
+    heartbeat_interval: _duration_pb2.Duration
+    expires_at: _timestamp_pb2.Timestamp
+    metadata: Metadata
+    def __init__(self, reservation_id: _Optional[_Union[ReservationID, _Mapping]] = ..., owner_id: _Optional[str] = ..., heartbeat_interval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ...) -> None: ...
+
+class GetOrExtendReservationResponse(_message.Message):
+    __slots__ = ["reservation"]
+    RESERVATION_FIELD_NUMBER: _ClassVar[int]
+    reservation: Reservation
+    def __init__(self, reservation: _Optional[_Union[Reservation, _Mapping]] = ...) -> None: ...
+
+class ReleaseReservationRequest(_message.Message):
+    __slots__ = ["reservation_id", "owner_id"]
+    RESERVATION_ID_FIELD_NUMBER: _ClassVar[int]
+    OWNER_ID_FIELD_NUMBER: _ClassVar[int]
     reservation_id: ReservationID
+    owner_id: str
     def __init__(self, reservation_id: _Optional[_Union[ReservationID, _Mapping]] = ..., owner_id: _Optional[str] = ...) -> None: ...
 
 class ReleaseReservationResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
-class Reservation(_message.Message):
-    __slots__ = ["expires_at", "heartbeat_interval", "metadata", "owner_id", "reservation_id"]
-    EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
-    HEARTBEAT_INTERVAL_FIELD_NUMBER: _ClassVar[int]
+class Dataset(_message.Message):
+    __slots__ = ["id", "metadata", "partitionKeys"]
+    ID_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
-    OWNER_ID_FIELD_NUMBER: _ClassVar[int]
-    RESERVATION_ID_FIELD_NUMBER: _ClassVar[int]
-    expires_at: _timestamp_pb2.Timestamp
-    heartbeat_interval: _duration_pb2.Duration
+    PARTITIONKEYS_FIELD_NUMBER: _ClassVar[int]
+    id: DatasetID
     metadata: Metadata
-    owner_id: str
-    reservation_id: ReservationID
-    def __init__(self, reservation_id: _Optional[_Union[ReservationID, _Mapping]] = ..., owner_id: _Optional[str] = ..., heartbeat_interval: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ...) -> None: ...
+    partitionKeys: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, id: _Optional[_Union[DatasetID, _Mapping]] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ..., partitionKeys: _Optional[_Iterable[str]] = ...) -> None: ...
 
-class ReservationID(_message.Message):
-    __slots__ = ["dataset_id", "tag_name"]
-    DATASET_ID_FIELD_NUMBER: _ClassVar[int]
-    TAG_NAME_FIELD_NUMBER: _ClassVar[int]
-    dataset_id: DatasetID
-    tag_name: str
-    def __init__(self, dataset_id: _Optional[_Union[DatasetID, _Mapping]] = ..., tag_name: _Optional[str] = ...) -> None: ...
+class Partition(_message.Message):
+    __slots__ = ["key", "value"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    key: str
+    value: str
+    def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+
+class DatasetID(_message.Message):
+    __slots__ = ["project", "name", "domain", "version", "UUID"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    UUID_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    name: str
+    domain: str
+    version: str
+    UUID: str
+    def __init__(self, project: _Optional[str] = ..., name: _Optional[str] = ..., domain: _Optional[str] = ..., version: _Optional[str] = ..., UUID: _Optional[str] = ...) -> None: ...
+
+class Artifact(_message.Message):
+    __slots__ = ["id", "dataset", "data", "metadata", "partitions", "tags", "created_at"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    DATASET_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    PARTITIONS_FIELD_NUMBER: _ClassVar[int]
+    TAGS_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    dataset: DatasetID
+    data: _containers.RepeatedCompositeFieldContainer[ArtifactData]
+    metadata: Metadata
+    partitions: _containers.RepeatedCompositeFieldContainer[Partition]
+    tags: _containers.RepeatedCompositeFieldContainer[Tag]
+    created_at: _timestamp_pb2.Timestamp
+    def __init__(self, id: _Optional[str] = ..., dataset: _Optional[_Union[DatasetID, _Mapping]] = ..., data: _Optional[_Iterable[_Union[ArtifactData, _Mapping]]] = ..., metadata: _Optional[_Union[Metadata, _Mapping]] = ..., partitions: _Optional[_Iterable[_Union[Partition, _Mapping]]] = ..., tags: _Optional[_Iterable[_Union[Tag, _Mapping]]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+
+class ArtifactData(_message.Message):
+    __slots__ = ["name", "value"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    value: _literals_pb2.Literal
+    def __init__(self, name: _Optional[str] = ..., value: _Optional[_Union[_literals_pb2.Literal, _Mapping]] = ...) -> None: ...
+
+class Tag(_message.Message):
+    __slots__ = ["name", "artifact_id", "dataset"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
+    DATASET_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    artifact_id: str
+    dataset: DatasetID
+    def __init__(self, name: _Optional[str] = ..., artifact_id: _Optional[str] = ..., dataset: _Optional[_Union[DatasetID, _Mapping]] = ...) -> None: ...
+
+class Metadata(_message.Message):
+    __slots__ = ["key_map"]
+    class KeyMapEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    KEY_MAP_FIELD_NUMBER: _ClassVar[int]
+    key_map: _containers.ScalarMap[str, str]
+    def __init__(self, key_map: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class FilterExpression(_message.Message):
+    __slots__ = ["filters"]
+    FILTERS_FIELD_NUMBER: _ClassVar[int]
+    filters: _containers.RepeatedCompositeFieldContainer[SinglePropertyFilter]
+    def __init__(self, filters: _Optional[_Iterable[_Union[SinglePropertyFilter, _Mapping]]] = ...) -> None: ...
 
 class SinglePropertyFilter(_message.Message):
-    __slots__ = ["artifact_filter", "dataset_filter", "operator", "partition_filter", "tag_filter"]
+    __slots__ = ["tag_filter", "partition_filter", "artifact_filter", "dataset_filter", "operator"]
     class ComparisonOperator(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        EQUALS: _ClassVar[SinglePropertyFilter.ComparisonOperator]
+    EQUALS: SinglePropertyFilter.ComparisonOperator
+    TAG_FILTER_FIELD_NUMBER: _ClassVar[int]
+    PARTITION_FILTER_FIELD_NUMBER: _ClassVar[int]
     ARTIFACT_FILTER_FIELD_NUMBER: _ClassVar[int]
     DATASET_FILTER_FIELD_NUMBER: _ClassVar[int]
-    EQUALS: SinglePropertyFilter.ComparisonOperator
     OPERATOR_FIELD_NUMBER: _ClassVar[int]
-    PARTITION_FILTER_FIELD_NUMBER: _ClassVar[int]
-    TAG_FILTER_FIELD_NUMBER: _ClassVar[int]
+    tag_filter: TagPropertyFilter
+    partition_filter: PartitionPropertyFilter
     artifact_filter: ArtifactPropertyFilter
     dataset_filter: DatasetPropertyFilter
     operator: SinglePropertyFilter.ComparisonOperator
-    partition_filter: PartitionPropertyFilter
-    tag_filter: TagPropertyFilter
     def __init__(self, tag_filter: _Optional[_Union[TagPropertyFilter, _Mapping]] = ..., partition_filter: _Optional[_Union[PartitionPropertyFilter, _Mapping]] = ..., artifact_filter: _Optional[_Union[ArtifactPropertyFilter, _Mapping]] = ..., dataset_filter: _Optional[_Union[DatasetPropertyFilter, _Mapping]] = ..., operator: _Optional[_Union[SinglePropertyFilter.ComparisonOperator, str]] = ...) -> None: ...
 
-class Tag(_message.Message):
-    __slots__ = ["artifact_id", "dataset", "name"]
+class ArtifactPropertyFilter(_message.Message):
+    __slots__ = ["artifact_id"]
     ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
-    DATASET_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
     artifact_id: str
-    dataset: DatasetID
-    name: str
-    def __init__(self, name: _Optional[str] = ..., artifact_id: _Optional[str] = ..., dataset: _Optional[_Union[DatasetID, _Mapping]] = ...) -> None: ...
+    def __init__(self, artifact_id: _Optional[str] = ...) -> None: ...
 
 class TagPropertyFilter(_message.Message):
     __slots__ = ["tag_name"]
     TAG_NAME_FIELD_NUMBER: _ClassVar[int]
     tag_name: str
     def __init__(self, tag_name: _Optional[str] = ...) -> None: ...
 
-class UpdateArtifactRequest(_message.Message):
-    __slots__ = ["artifact_id", "data", "dataset", "tag_name"]
-    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
-    DATASET_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    TAG_NAME_FIELD_NUMBER: _ClassVar[int]
-    artifact_id: str
-    data: _containers.RepeatedCompositeFieldContainer[ArtifactData]
-    dataset: DatasetID
-    tag_name: str
-    def __init__(self, dataset: _Optional[_Union[DatasetID, _Mapping]] = ..., artifact_id: _Optional[str] = ..., tag_name: _Optional[str] = ..., data: _Optional[_Iterable[_Union[ArtifactData, _Mapping]]] = ...) -> None: ...
+class PartitionPropertyFilter(_message.Message):
+    __slots__ = ["key_val"]
+    KEY_VAL_FIELD_NUMBER: _ClassVar[int]
+    key_val: KeyValuePair
+    def __init__(self, key_val: _Optional[_Union[KeyValuePair, _Mapping]] = ...) -> None: ...
 
-class UpdateArtifactResponse(_message.Message):
-    __slots__ = ["artifact_id"]
-    ARTIFACT_ID_FIELD_NUMBER: _ClassVar[int]
-    artifact_id: str
-    def __init__(self, artifact_id: _Optional[str] = ...) -> None: ...
+class KeyValuePair(_message.Message):
+    __slots__ = ["key", "value"]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    key: str
+    value: str
+    def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+
+class DatasetPropertyFilter(_message.Message):
+    __slots__ = ["project", "name", "domain", "version"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    name: str
+    domain: str
+    version: str
+    def __init__(self, project: _Optional[str] = ..., name: _Optional[str] = ..., domain: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
+
+class PaginationOptions(_message.Message):
+    __slots__ = ["limit", "token", "sortKey", "sortOrder"]
+    class SortOrder(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        DESCENDING: _ClassVar[PaginationOptions.SortOrder]
+        ASCENDING: _ClassVar[PaginationOptions.SortOrder]
+    DESCENDING: PaginationOptions.SortOrder
+    ASCENDING: PaginationOptions.SortOrder
+    class SortKey(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        CREATION_TIME: _ClassVar[PaginationOptions.SortKey]
+    CREATION_TIME: PaginationOptions.SortKey
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    SORTKEY_FIELD_NUMBER: _ClassVar[int]
+    SORTORDER_FIELD_NUMBER: _ClassVar[int]
+    limit: int
+    token: str
+    sortKey: PaginationOptions.SortKey
+    sortOrder: PaginationOptions.SortOrder
+    def __init__(self, limit: _Optional[int] = ..., token: _Optional[str] = ..., sortKey: _Optional[_Union[PaginationOptions.SortKey, str]] = ..., sortOrder: _Optional[_Union[PaginationOptions.SortOrder, str]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/event/event_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/event/event_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,40 +16,41 @@
 from flyteidl.core import execution_pb2 as flyteidl_dot_core_dot_execution__pb2
 from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 from flyteidl.core import catalog_pb2 as flyteidl_dot_core_dot_catalog__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66lyteidl/event/event.proto\x12\x0e\x66lyteidl.event\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1c\x66lyteidl/core/compiler.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1b\x66lyteidl/core/catalog.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xaa\x03\n\x16WorkflowExecutionEvent\x12M\n\x0c\x65xecution_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\x12\x1f\n\x0bproducer_id\x18\x02 \x01(\tR\nproducerId\x12<\n\x05phase\x18\x03 \x01(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x05phase\x12;\n\x0boccurred_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1f\n\noutput_uri\x18\x05 \x01(\tH\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12<\n\x0boutput_data\x18\x07 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\noutputDataB\x0f\n\routput_result\"\x85\x08\n\x12NodeExecutionEvent\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\x12\x1f\n\x0bproducer_id\x18\x02 \x01(\tR\nproducerId\x12\x38\n\x05phase\x18\x03 \x01(\x0e\x32\".flyteidl.core.NodeExecution.PhaseR\x05phase\x12;\n\x0boccurred_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1b\n\tinput_uri\x18\x05 \x01(\tR\x08inputUri\x12\x1f\n\noutput_uri\x18\x06 \x01(\tH\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\x07 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12<\n\x0boutput_data\x18\x0f \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\noutputData\x12\\\n\x16workflow_node_metadata\x18\x08 \x01(\x0b\x32$.flyteidl.event.WorkflowNodeMetadataH\x01R\x14workflowNodeMetadata\x12P\n\x12task_node_metadata\x18\x0e \x01(\x0b\x32 .flyteidl.event.TaskNodeMetadataH\x01R\x10taskNodeMetadata\x12]\n\x14parent_task_metadata\x18\t \x01(\x0b\x32+.flyteidl.event.ParentTaskExecutionMetadataR\x12parentTaskMetadata\x12]\n\x14parent_node_metadata\x18\n \x01(\x0b\x32+.flyteidl.event.ParentNodeExecutionMetadataR\x12parentNodeMetadata\x12\x1f\n\x0bretry_group\x18\x0b \x01(\tR\nretryGroup\x12 \n\x0cspec_node_id\x18\x0c \x01(\tR\nspecNodeId\x12\x1b\n\tnode_name\x18\r \x01(\tR\x08nodeName\x12#\n\revent_version\x18\x10 \x01(\x05R\x0c\x65ventVersion\x12\x1b\n\tis_parent\x18\x11 \x01(\x08R\x08isParent\x12\x1d\n\nis_dynamic\x18\x12 \x01(\x08R\tisDynamic\x12\x19\n\x08\x64\x65\x63k_uri\x18\x13 \x01(\tR\x07\x64\x65\x63kUriB\x0f\n\routput_resultB\x11\n\x0ftarget_metadata\"e\n\x14WorkflowNodeMetadata\x12M\n\x0c\x65xecution_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\"\xf1\x02\n\x10TaskNodeMetadata\x12\x44\n\x0c\x63\x61\x63he_status\x18\x01 \x01(\x0e\x32!.flyteidl.core.CatalogCacheStatusR\x0b\x63\x61\x63heStatus\x12?\n\x0b\x63\x61talog_key\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.CatalogMetadataR\ncatalogKey\x12W\n\x12reservation_status\x18\x03 \x01(\x0e\x32(.flyteidl.core.CatalogReservation.StatusR\x11reservationStatus\x12%\n\x0e\x63heckpoint_uri\x18\x04 \x01(\tR\rcheckpointUri\x12V\n\x10\x64ynamic_workflow\x18\x10 \x01(\x0b\x32+.flyteidl.event.DynamicWorkflowNodeMetadataR\x0f\x64ynamicWorkflow\"\x9d\x01\n\x1b\x44ynamicWorkflowNodeMetadata\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12S\n\x11\x63ompiled_workflow\x18\x02 \x01(\x0b\x32&.flyteidl.core.CompiledWorkflowClosureR\x10\x63ompiledWorkflow\"U\n\x1bParentTaskExecutionMetadata\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\"6\n\x1bParentNodeExecutionMetadata\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\"\xd2\x06\n\x12TaskExecutionEvent\x12\x32\n\x07task_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x06taskId\x12_\n\x18parent_node_execution_id\x18\x02 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x15parentNodeExecutionId\x12#\n\rretry_attempt\x18\x03 \x01(\rR\x0cretryAttempt\x12\x38\n\x05phase\x18\x04 \x01(\x0e\x32\".flyteidl.core.TaskExecution.PhaseR\x05phase\x12\x1f\n\x0bproducer_id\x18\x05 \x01(\tR\nproducerId\x12*\n\x04logs\x18\x06 \x03(\x0b\x32\x16.flyteidl.core.TaskLogR\x04logs\x12;\n\x0boccurred_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1b\n\tinput_uri\x18\x08 \x01(\tR\x08inputUri\x12\x1f\n\noutput_uri\x18\t \x01(\tH\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\n \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12<\n\x0boutput_data\x18\x11 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\noutputData\x12\x38\n\x0b\x63ustom_info\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructR\ncustomInfo\x12#\n\rphase_version\x18\x0c \x01(\rR\x0cphaseVersion\x12\x16\n\x06reason\x18\r \x01(\tR\x06reason\x12\x1b\n\ttask_type\x18\x0e \x01(\tR\x08taskType\x12\x41\n\x08metadata\x18\x10 \x01(\x0b\x32%.flyteidl.event.TaskExecutionMetadataR\x08metadata\x12#\n\revent_version\x18\x12 \x01(\x05R\x0c\x65ventVersionB\x0f\n\routput_result\"\x9e\x02\n\x14\x45xternalResourceInfo\x12\x1f\n\x0b\x65xternal_id\x18\x01 \x01(\tR\nexternalId\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12#\n\rretry_attempt\x18\x03 \x01(\rR\x0cretryAttempt\x12\x38\n\x05phase\x18\x04 \x01(\x0e\x32\".flyteidl.core.TaskExecution.PhaseR\x05phase\x12\x44\n\x0c\x63\x61\x63he_status\x18\x05 \x01(\x0e\x32!.flyteidl.core.CatalogCacheStatusR\x0b\x63\x61\x63heStatus\x12*\n\x04logs\x18\x06 \x03(\x0b\x32\x16.flyteidl.core.TaskLogR\x04logs\"[\n\x10ResourcePoolInfo\x12)\n\x10\x61llocation_token\x18\x01 \x01(\tR\x0f\x61llocationToken\x12\x1c\n\tnamespace\x18\x02 \x01(\tR\tnamespace\"\x9d\x03\n\x15TaskExecutionMetadata\x12%\n\x0egenerated_name\x18\x01 \x01(\tR\rgeneratedName\x12S\n\x12\x65xternal_resources\x18\x02 \x03(\x0b\x32$.flyteidl.event.ExternalResourceInfoR\x11\x65xternalResources\x12N\n\x12resource_pool_info\x18\x03 \x03(\x0b\x32 .flyteidl.event.ResourcePoolInfoR\x10resourcePoolInfo\x12+\n\x11plugin_identifier\x18\x04 \x01(\tR\x10pluginIdentifier\x12Z\n\x0einstance_class\x18\x10 \x01(\x0e\x32\x33.flyteidl.event.TaskExecutionMetadata.InstanceClassR\rinstanceClass\"/\n\rInstanceClass\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x11\n\rINTERRUPTIBLE\x10\x01\x42\xb0\x01\n\x12\x63om.flyteidl.eventB\nEventProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/event\xa2\x02\x03\x46\x45X\xaa\x02\x0e\x46lyteidl.Event\xca\x02\x0e\x46lyteidl\\Event\xe2\x02\x1a\x46lyteidl\\Event\\GPBMetadata\xea\x02\x0f\x46lyteidl::Eventb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66lyteidl/event/event.proto\x12\x0e\x66lyteidl.event\x1a\x1c\x66lyteidl/core/literals.proto\x1a\x1c\x66lyteidl/core/compiler.proto\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1b\x66lyteidl/core/catalog.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xaa\x03\n\x16WorkflowExecutionEvent\x12M\n\x0c\x65xecution_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\x12\x1f\n\x0bproducer_id\x18\x02 \x01(\tR\nproducerId\x12<\n\x05phase\x18\x03 \x01(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x05phase\x12;\n\x0boccurred_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1f\n\noutput_uri\x18\x05 \x01(\tH\x00R\toutputUri\x12\x35\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x00R\x05\x65rror\x12<\n\x0boutput_data\x18\x07 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\noutputDataB\x0f\n\routput_result\"\x8f\t\n\x12NodeExecutionEvent\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x02id\x12\x1f\n\x0bproducer_id\x18\x02 \x01(\tR\nproducerId\x12\x38\n\x05phase\x18\x03 \x01(\x0e\x32\".flyteidl.core.NodeExecution.PhaseR\x05phase\x12;\n\x0boccurred_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1d\n\tinput_uri\x18\x05 \x01(\tH\x00R\x08inputUri\x12:\n\ninput_data\x18\x14 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\tinputData\x12\x1f\n\noutput_uri\x18\x06 \x01(\tH\x01R\toutputUri\x12\x35\n\x05\x65rror\x18\x07 \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x01R\x05\x65rror\x12<\n\x0boutput_data\x18\x0f \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x01R\noutputData\x12\\\n\x16workflow_node_metadata\x18\x08 \x01(\x0b\x32$.flyteidl.event.WorkflowNodeMetadataH\x02R\x14workflowNodeMetadata\x12P\n\x12task_node_metadata\x18\x0e \x01(\x0b\x32 .flyteidl.event.TaskNodeMetadataH\x02R\x10taskNodeMetadata\x12]\n\x14parent_task_metadata\x18\t \x01(\x0b\x32+.flyteidl.event.ParentTaskExecutionMetadataR\x12parentTaskMetadata\x12]\n\x14parent_node_metadata\x18\n \x01(\x0b\x32+.flyteidl.event.ParentNodeExecutionMetadataR\x12parentNodeMetadata\x12\x1f\n\x0bretry_group\x18\x0b \x01(\tR\nretryGroup\x12 \n\x0cspec_node_id\x18\x0c \x01(\tR\nspecNodeId\x12\x1b\n\tnode_name\x18\r \x01(\tR\x08nodeName\x12#\n\revent_version\x18\x10 \x01(\x05R\x0c\x65ventVersion\x12\x1b\n\tis_parent\x18\x11 \x01(\x08R\x08isParent\x12\x1d\n\nis_dynamic\x18\x12 \x01(\x08R\tisDynamic\x12\x19\n\x08\x64\x65\x63k_uri\x18\x13 \x01(\tR\x07\x64\x65\x63kUri\x12;\n\x0breported_at\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\nreportedAtB\r\n\x0binput_valueB\x0f\n\routput_resultB\x11\n\x0ftarget_metadata\"e\n\x14WorkflowNodeMetadata\x12M\n\x0c\x65xecution_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x0b\x65xecutionId\"\xf1\x02\n\x10TaskNodeMetadata\x12\x44\n\x0c\x63\x61\x63he_status\x18\x01 \x01(\x0e\x32!.flyteidl.core.CatalogCacheStatusR\x0b\x63\x61\x63heStatus\x12?\n\x0b\x63\x61talog_key\x18\x02 \x01(\x0b\x32\x1e.flyteidl.core.CatalogMetadataR\ncatalogKey\x12W\n\x12reservation_status\x18\x03 \x01(\x0e\x32(.flyteidl.core.CatalogReservation.StatusR\x11reservationStatus\x12%\n\x0e\x63heckpoint_uri\x18\x04 \x01(\tR\rcheckpointUri\x12V\n\x10\x64ynamic_workflow\x18\x10 \x01(\x0b\x32+.flyteidl.event.DynamicWorkflowNodeMetadataR\x0f\x64ynamicWorkflow\"\xce\x01\n\x1b\x44ynamicWorkflowNodeMetadata\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x02id\x12S\n\x11\x63ompiled_workflow\x18\x02 \x01(\x0b\x32&.flyteidl.core.CompiledWorkflowClosureR\x10\x63ompiledWorkflow\x12/\n\x14\x64ynamic_job_spec_uri\x18\x03 \x01(\tR\x11\x64ynamicJobSpecUri\"U\n\x1bParentTaskExecutionMetadata\x12\x36\n\x02id\x18\x01 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierR\x02id\"6\n\x1bParentNodeExecutionMetadata\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\"\xdc\x07\n\x12TaskExecutionEvent\x12\x32\n\x07task_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\x06taskId\x12_\n\x18parent_node_execution_id\x18\x02 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierR\x15parentNodeExecutionId\x12#\n\rretry_attempt\x18\x03 \x01(\rR\x0cretryAttempt\x12\x38\n\x05phase\x18\x04 \x01(\x0e\x32\".flyteidl.core.TaskExecution.PhaseR\x05phase\x12\x1f\n\x0bproducer_id\x18\x05 \x01(\tR\nproducerId\x12*\n\x04logs\x18\x06 \x03(\x0b\x32\x16.flyteidl.core.TaskLogR\x04logs\x12;\n\x0boccurred_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x1d\n\tinput_uri\x18\x08 \x01(\tH\x00R\x08inputUri\x12:\n\ninput_data\x18\x13 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\tinputData\x12\x1f\n\noutput_uri\x18\t \x01(\tH\x01R\toutputUri\x12\x35\n\x05\x65rror\x18\n \x01(\x0b\x32\x1d.flyteidl.core.ExecutionErrorH\x01R\x05\x65rror\x12<\n\x0boutput_data\x18\x11 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x01R\noutputData\x12\x38\n\x0b\x63ustom_info\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructR\ncustomInfo\x12#\n\rphase_version\x18\x0c \x01(\rR\x0cphaseVersion\x12\x16\n\x06reason\x18\r \x01(\tR\x06reason\x12\x1b\n\ttask_type\x18\x0e \x01(\tR\x08taskType\x12\x41\n\x08metadata\x18\x10 \x01(\x0b\x32%.flyteidl.event.TaskExecutionMetadataR\x08metadata\x12#\n\revent_version\x18\x12 \x01(\x05R\x0c\x65ventVersion\x12;\n\x0breported_at\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\nreportedAtB\r\n\x0binput_valueB\x0f\n\routput_result\"\x9e\x02\n\x14\x45xternalResourceInfo\x12\x1f\n\x0b\x65xternal_id\x18\x01 \x01(\tR\nexternalId\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12#\n\rretry_attempt\x18\x03 \x01(\rR\x0cretryAttempt\x12\x38\n\x05phase\x18\x04 \x01(\x0e\x32\".flyteidl.core.TaskExecution.PhaseR\x05phase\x12\x44\n\x0c\x63\x61\x63he_status\x18\x05 \x01(\x0e\x32!.flyteidl.core.CatalogCacheStatusR\x0b\x63\x61\x63heStatus\x12*\n\x04logs\x18\x06 \x03(\x0b\x32\x16.flyteidl.core.TaskLogR\x04logs\"[\n\x10ResourcePoolInfo\x12)\n\x10\x61llocation_token\x18\x01 \x01(\tR\x0f\x61llocationToken\x12\x1c\n\tnamespace\x18\x02 \x01(\tR\tnamespace\"\x9d\x03\n\x15TaskExecutionMetadata\x12%\n\x0egenerated_name\x18\x01 \x01(\tR\rgeneratedName\x12S\n\x12\x65xternal_resources\x18\x02 \x03(\x0b\x32$.flyteidl.event.ExternalResourceInfoR\x11\x65xternalResources\x12N\n\x12resource_pool_info\x18\x03 \x03(\x0b\x32 .flyteidl.event.ResourcePoolInfoR\x10resourcePoolInfo\x12+\n\x11plugin_identifier\x18\x04 \x01(\tR\x10pluginIdentifier\x12Z\n\x0einstance_class\x18\x10 \x01(\x0e\x32\x33.flyteidl.event.TaskExecutionMetadata.InstanceClassR\rinstanceClass\"/\n\rInstanceClass\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x11\n\rINTERRUPTIBLE\x10\x01\x42\xb0\x01\n\x12\x63om.flyteidl.eventB\nEventProtoP\x01Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/event\xa2\x02\x03\x46\x45X\xaa\x02\x0e\x46lyteidl.Event\xca\x02\x0e\x46lyteidl\\Event\xe2\x02\x1a\x46lyteidl\\Event\\GPBMetadata\xea\x02\x0f\x46lyteidl::Eventb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.event.event_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.event.event_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.flyteidl.eventB\nEventProtoP\001Z5github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/event\242\002\003FEX\252\002\016Flyteidl.Event\312\002\016Flyteidl\\Event\342\002\032Flyteidl\\Event\\GPBMetadata\352\002\017Flyteidl::Event'
-  _WORKFLOWEXECUTIONEVENT._serialized_start=262
-  _WORKFLOWEXECUTIONEVENT._serialized_end=688
-  _NODEEXECUTIONEVENT._serialized_start=691
-  _NODEEXECUTIONEVENT._serialized_end=1720
-  _WORKFLOWNODEMETADATA._serialized_start=1722
-  _WORKFLOWNODEMETADATA._serialized_end=1823
-  _TASKNODEMETADATA._serialized_start=1826
-  _TASKNODEMETADATA._serialized_end=2195
-  _DYNAMICWORKFLOWNODEMETADATA._serialized_start=2198
-  _DYNAMICWORKFLOWNODEMETADATA._serialized_end=2355
-  _PARENTTASKEXECUTIONMETADATA._serialized_start=2357
-  _PARENTTASKEXECUTIONMETADATA._serialized_end=2442
-  _PARENTNODEEXECUTIONMETADATA._serialized_start=2444
-  _PARENTNODEEXECUTIONMETADATA._serialized_end=2498
-  _TASKEXECUTIONEVENT._serialized_start=2501
-  _TASKEXECUTIONEVENT._serialized_end=3351
-  _EXTERNALRESOURCEINFO._serialized_start=3354
-  _EXTERNALRESOURCEINFO._serialized_end=3640
-  _RESOURCEPOOLINFO._serialized_start=3642
-  _RESOURCEPOOLINFO._serialized_end=3733
-  _TASKEXECUTIONMETADATA._serialized_start=3736
-  _TASKEXECUTIONMETADATA._serialized_end=4149
-  _TASKEXECUTIONMETADATA_INSTANCECLASS._serialized_start=4102
-  _TASKEXECUTIONMETADATA_INSTANCECLASS._serialized_end=4149
+  _globals['_WORKFLOWEXECUTIONEVENT']._serialized_start=262
+  _globals['_WORKFLOWEXECUTIONEVENT']._serialized_end=688
+  _globals['_NODEEXECUTIONEVENT']._serialized_start=691
+  _globals['_NODEEXECUTIONEVENT']._serialized_end=1858
+  _globals['_WORKFLOWNODEMETADATA']._serialized_start=1860
+  _globals['_WORKFLOWNODEMETADATA']._serialized_end=1961
+  _globals['_TASKNODEMETADATA']._serialized_start=1964
+  _globals['_TASKNODEMETADATA']._serialized_end=2333
+  _globals['_DYNAMICWORKFLOWNODEMETADATA']._serialized_start=2336
+  _globals['_DYNAMICWORKFLOWNODEMETADATA']._serialized_end=2542
+  _globals['_PARENTTASKEXECUTIONMETADATA']._serialized_start=2544
+  _globals['_PARENTTASKEXECUTIONMETADATA']._serialized_end=2629
+  _globals['_PARENTNODEEXECUTIONMETADATA']._serialized_start=2631
+  _globals['_PARENTNODEEXECUTIONMETADATA']._serialized_end=2685
+  _globals['_TASKEXECUTIONEVENT']._serialized_start=2688
+  _globals['_TASKEXECUTIONEVENT']._serialized_end=3676
+  _globals['_EXTERNALRESOURCEINFO']._serialized_start=3679
+  _globals['_EXTERNALRESOURCEINFO']._serialized_end=3965
+  _globals['_RESOURCEPOOLINFO']._serialized_start=3967
+  _globals['_RESOURCEPOOLINFO']._serialized_end=4058
+  _globals['_TASKEXECUTIONMETADATA']._serialized_start=4061
+  _globals['_TASKEXECUTIONMETADATA']._serialized_end=4474
+  _globals['_TASKEXECUTIONMETADATA_INSTANCECLASS']._serialized_start=4427
+  _globals['_TASKEXECUTIONMETADATA_INSTANCECLASS']._serialized_end=4474
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/event/event_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/event/event_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,186 +9,198 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DynamicWorkflowNodeMetadata(_message.Message):
-    __slots__ = ["compiled_workflow", "id"]
-    COMPILED_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    compiled_workflow: _compiler_pb2.CompiledWorkflowClosure
-    id: _identifier_pb2.Identifier
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., compiled_workflow: _Optional[_Union[_compiler_pb2.CompiledWorkflowClosure, _Mapping]] = ...) -> None: ...
-
-class ExternalResourceInfo(_message.Message):
-    __slots__ = ["cache_status", "external_id", "index", "logs", "phase", "retry_attempt"]
-    CACHE_STATUS_FIELD_NUMBER: _ClassVar[int]
-    EXTERNAL_ID_FIELD_NUMBER: _ClassVar[int]
-    INDEX_FIELD_NUMBER: _ClassVar[int]
-    LOGS_FIELD_NUMBER: _ClassVar[int]
+class WorkflowExecutionEvent(_message.Message):
+    __slots__ = ["execution_id", "producer_id", "phase", "occurred_at", "output_uri", "error", "output_data"]
+    EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    PRODUCER_ID_FIELD_NUMBER: _ClassVar[int]
     PHASE_FIELD_NUMBER: _ClassVar[int]
-    RETRY_ATTEMPT_FIELD_NUMBER: _ClassVar[int]
-    cache_status: _catalog_pb2.CatalogCacheStatus
-    external_id: str
-    index: int
-    logs: _containers.RepeatedCompositeFieldContainer[_execution_pb2.TaskLog]
-    phase: _execution_pb2.TaskExecution.Phase
-    retry_attempt: int
-    def __init__(self, external_id: _Optional[str] = ..., index: _Optional[int] = ..., retry_attempt: _Optional[int] = ..., phase: _Optional[_Union[_execution_pb2.TaskExecution.Phase, str]] = ..., cache_status: _Optional[_Union[_catalog_pb2.CatalogCacheStatus, str]] = ..., logs: _Optional[_Iterable[_Union[_execution_pb2.TaskLog, _Mapping]]] = ...) -> None: ...
+    OCCURRED_AT_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
+    execution_id: _identifier_pb2.WorkflowExecutionIdentifier
+    producer_id: str
+    phase: _execution_pb2.WorkflowExecution.Phase
+    occurred_at: _timestamp_pb2.Timestamp
+    output_uri: str
+    error: _execution_pb2.ExecutionError
+    output_data: _literals_pb2.LiteralMap
+    def __init__(self, execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., producer_id: _Optional[str] = ..., phase: _Optional[_Union[_execution_pb2.WorkflowExecution.Phase, str]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ...) -> None: ...
 
 class NodeExecutionEvent(_message.Message):
-    __slots__ = ["deck_uri", "error", "event_version", "id", "input_uri", "is_dynamic", "is_parent", "node_name", "occurred_at", "output_data", "output_uri", "parent_node_metadata", "parent_task_metadata", "phase", "producer_id", "retry_group", "spec_node_id", "task_node_metadata", "workflow_node_metadata"]
-    DECK_URI_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    EVENT_VERSION_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["id", "producer_id", "phase", "occurred_at", "input_uri", "input_data", "output_uri", "error", "output_data", "workflow_node_metadata", "task_node_metadata", "parent_task_metadata", "parent_node_metadata", "retry_group", "spec_node_id", "node_name", "event_version", "is_parent", "is_dynamic", "deck_uri", "reported_at"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    INPUT_URI_FIELD_NUMBER: _ClassVar[int]
-    IS_DYNAMIC_FIELD_NUMBER: _ClassVar[int]
-    IS_PARENT_FIELD_NUMBER: _ClassVar[int]
-    NODE_NAME_FIELD_NUMBER: _ClassVar[int]
+    PRODUCER_ID_FIELD_NUMBER: _ClassVar[int]
+    PHASE_FIELD_NUMBER: _ClassVar[int]
     OCCURRED_AT_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
+    INPUT_URI_FIELD_NUMBER: _ClassVar[int]
+    INPUT_DATA_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
-    PARENT_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
+    WORKFLOW_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
+    TASK_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
     PARENT_TASK_METADATA_FIELD_NUMBER: _ClassVar[int]
-    PHASE_FIELD_NUMBER: _ClassVar[int]
-    PRODUCER_ID_FIELD_NUMBER: _ClassVar[int]
+    PARENT_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
     RETRY_GROUP_FIELD_NUMBER: _ClassVar[int]
     SPEC_NODE_ID_FIELD_NUMBER: _ClassVar[int]
-    TASK_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
-    WORKFLOW_NODE_METADATA_FIELD_NUMBER: _ClassVar[int]
-    deck_uri: str
-    error: _execution_pb2.ExecutionError
-    event_version: int
+    NODE_NAME_FIELD_NUMBER: _ClassVar[int]
+    EVENT_VERSION_FIELD_NUMBER: _ClassVar[int]
+    IS_PARENT_FIELD_NUMBER: _ClassVar[int]
+    IS_DYNAMIC_FIELD_NUMBER: _ClassVar[int]
+    DECK_URI_FIELD_NUMBER: _ClassVar[int]
+    REPORTED_AT_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.NodeExecutionIdentifier
-    input_uri: str
-    is_dynamic: bool
-    is_parent: bool
-    node_name: str
+    producer_id: str
+    phase: _execution_pb2.NodeExecution.Phase
     occurred_at: _timestamp_pb2.Timestamp
-    output_data: _literals_pb2.LiteralMap
+    input_uri: str
+    input_data: _literals_pb2.LiteralMap
     output_uri: str
-    parent_node_metadata: ParentNodeExecutionMetadata
+    error: _execution_pb2.ExecutionError
+    output_data: _literals_pb2.LiteralMap
+    workflow_node_metadata: WorkflowNodeMetadata
+    task_node_metadata: TaskNodeMetadata
     parent_task_metadata: ParentTaskExecutionMetadata
-    phase: _execution_pb2.NodeExecution.Phase
-    producer_id: str
+    parent_node_metadata: ParentNodeExecutionMetadata
     retry_group: str
     spec_node_id: str
-    task_node_metadata: TaskNodeMetadata
-    workflow_node_metadata: WorkflowNodeMetadata
-    def __init__(self, id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., producer_id: _Optional[str] = ..., phase: _Optional[_Union[_execution_pb2.NodeExecution.Phase, str]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., input_uri: _Optional[str] = ..., output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., workflow_node_metadata: _Optional[_Union[WorkflowNodeMetadata, _Mapping]] = ..., task_node_metadata: _Optional[_Union[TaskNodeMetadata, _Mapping]] = ..., parent_task_metadata: _Optional[_Union[ParentTaskExecutionMetadata, _Mapping]] = ..., parent_node_metadata: _Optional[_Union[ParentNodeExecutionMetadata, _Mapping]] = ..., retry_group: _Optional[str] = ..., spec_node_id: _Optional[str] = ..., node_name: _Optional[str] = ..., event_version: _Optional[int] = ..., is_parent: bool = ..., is_dynamic: bool = ..., deck_uri: _Optional[str] = ...) -> None: ...
+    node_name: str
+    event_version: int
+    is_parent: bool
+    is_dynamic: bool
+    deck_uri: str
+    reported_at: _timestamp_pb2.Timestamp
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., producer_id: _Optional[str] = ..., phase: _Optional[_Union[_execution_pb2.NodeExecution.Phase, str]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., input_uri: _Optional[str] = ..., input_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., workflow_node_metadata: _Optional[_Union[WorkflowNodeMetadata, _Mapping]] = ..., task_node_metadata: _Optional[_Union[TaskNodeMetadata, _Mapping]] = ..., parent_task_metadata: _Optional[_Union[ParentTaskExecutionMetadata, _Mapping]] = ..., parent_node_metadata: _Optional[_Union[ParentNodeExecutionMetadata, _Mapping]] = ..., retry_group: _Optional[str] = ..., spec_node_id: _Optional[str] = ..., node_name: _Optional[str] = ..., event_version: _Optional[int] = ..., is_parent: bool = ..., is_dynamic: bool = ..., deck_uri: _Optional[str] = ..., reported_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class ParentNodeExecutionMetadata(_message.Message):
-    __slots__ = ["node_id"]
-    NODE_ID_FIELD_NUMBER: _ClassVar[int]
-    node_id: str
-    def __init__(self, node_id: _Optional[str] = ...) -> None: ...
+class WorkflowNodeMetadata(_message.Message):
+    __slots__ = ["execution_id"]
+    EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    execution_id: _identifier_pb2.WorkflowExecutionIdentifier
+    def __init__(self, execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
+
+class TaskNodeMetadata(_message.Message):
+    __slots__ = ["cache_status", "catalog_key", "reservation_status", "checkpoint_uri", "dynamic_workflow"]
+    CACHE_STATUS_FIELD_NUMBER: _ClassVar[int]
+    CATALOG_KEY_FIELD_NUMBER: _ClassVar[int]
+    RESERVATION_STATUS_FIELD_NUMBER: _ClassVar[int]
+    CHECKPOINT_URI_FIELD_NUMBER: _ClassVar[int]
+    DYNAMIC_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
+    cache_status: _catalog_pb2.CatalogCacheStatus
+    catalog_key: _catalog_pb2.CatalogMetadata
+    reservation_status: _catalog_pb2.CatalogReservation.Status
+    checkpoint_uri: str
+    dynamic_workflow: DynamicWorkflowNodeMetadata
+    def __init__(self, cache_status: _Optional[_Union[_catalog_pb2.CatalogCacheStatus, str]] = ..., catalog_key: _Optional[_Union[_catalog_pb2.CatalogMetadata, _Mapping]] = ..., reservation_status: _Optional[_Union[_catalog_pb2.CatalogReservation.Status, str]] = ..., checkpoint_uri: _Optional[str] = ..., dynamic_workflow: _Optional[_Union[DynamicWorkflowNodeMetadata, _Mapping]] = ...) -> None: ...
+
+class DynamicWorkflowNodeMetadata(_message.Message):
+    __slots__ = ["id", "compiled_workflow", "dynamic_job_spec_uri"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    COMPILED_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
+    DYNAMIC_JOB_SPEC_URI_FIELD_NUMBER: _ClassVar[int]
+    id: _identifier_pb2.Identifier
+    compiled_workflow: _compiler_pb2.CompiledWorkflowClosure
+    dynamic_job_spec_uri: str
+    def __init__(self, id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., compiled_workflow: _Optional[_Union[_compiler_pb2.CompiledWorkflowClosure, _Mapping]] = ..., dynamic_job_spec_uri: _Optional[str] = ...) -> None: ...
 
 class ParentTaskExecutionMetadata(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: _identifier_pb2.TaskExecutionIdentifier
     def __init__(self, id: _Optional[_Union[_identifier_pb2.TaskExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
-class ResourcePoolInfo(_message.Message):
-    __slots__ = ["allocation_token", "namespace"]
-    ALLOCATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
-    allocation_token: str
-    namespace: str
-    def __init__(self, allocation_token: _Optional[str] = ..., namespace: _Optional[str] = ...) -> None: ...
+class ParentNodeExecutionMetadata(_message.Message):
+    __slots__ = ["node_id"]
+    NODE_ID_FIELD_NUMBER: _ClassVar[int]
+    node_id: str
+    def __init__(self, node_id: _Optional[str] = ...) -> None: ...
 
 class TaskExecutionEvent(_message.Message):
-    __slots__ = ["custom_info", "error", "event_version", "input_uri", "logs", "metadata", "occurred_at", "output_data", "output_uri", "parent_node_execution_id", "phase", "phase_version", "producer_id", "reason", "retry_attempt", "task_id", "task_type"]
-    CUSTOM_INFO_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    EVENT_VERSION_FIELD_NUMBER: _ClassVar[int]
-    INPUT_URI_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["task_id", "parent_node_execution_id", "retry_attempt", "phase", "producer_id", "logs", "occurred_at", "input_uri", "input_data", "output_uri", "error", "output_data", "custom_info", "phase_version", "reason", "task_type", "metadata", "event_version", "reported_at"]
+    TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    PARENT_NODE_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    RETRY_ATTEMPT_FIELD_NUMBER: _ClassVar[int]
+    PHASE_FIELD_NUMBER: _ClassVar[int]
+    PRODUCER_ID_FIELD_NUMBER: _ClassVar[int]
     LOGS_FIELD_NUMBER: _ClassVar[int]
-    METADATA_FIELD_NUMBER: _ClassVar[int]
     OCCURRED_AT_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
+    INPUT_URI_FIELD_NUMBER: _ClassVar[int]
+    INPUT_DATA_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
-    PARENT_NODE_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    PHASE_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
+    CUSTOM_INFO_FIELD_NUMBER: _ClassVar[int]
     PHASE_VERSION_FIELD_NUMBER: _ClassVar[int]
-    PRODUCER_ID_FIELD_NUMBER: _ClassVar[int]
     REASON_FIELD_NUMBER: _ClassVar[int]
-    RETRY_ATTEMPT_FIELD_NUMBER: _ClassVar[int]
-    TASK_ID_FIELD_NUMBER: _ClassVar[int]
     TASK_TYPE_FIELD_NUMBER: _ClassVar[int]
-    custom_info: _struct_pb2.Struct
-    error: _execution_pb2.ExecutionError
-    event_version: int
-    input_uri: str
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    EVENT_VERSION_FIELD_NUMBER: _ClassVar[int]
+    REPORTED_AT_FIELD_NUMBER: _ClassVar[int]
+    task_id: _identifier_pb2.Identifier
+    parent_node_execution_id: _identifier_pb2.NodeExecutionIdentifier
+    retry_attempt: int
+    phase: _execution_pb2.TaskExecution.Phase
+    producer_id: str
     logs: _containers.RepeatedCompositeFieldContainer[_execution_pb2.TaskLog]
-    metadata: TaskExecutionMetadata
     occurred_at: _timestamp_pb2.Timestamp
-    output_data: _literals_pb2.LiteralMap
+    input_uri: str
+    input_data: _literals_pb2.LiteralMap
     output_uri: str
-    parent_node_execution_id: _identifier_pb2.NodeExecutionIdentifier
-    phase: _execution_pb2.TaskExecution.Phase
+    error: _execution_pb2.ExecutionError
+    output_data: _literals_pb2.LiteralMap
+    custom_info: _struct_pb2.Struct
     phase_version: int
-    producer_id: str
     reason: str
-    retry_attempt: int
-    task_id: _identifier_pb2.Identifier
     task_type: str
-    def __init__(self, task_id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., parent_node_execution_id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., retry_attempt: _Optional[int] = ..., phase: _Optional[_Union[_execution_pb2.TaskExecution.Phase, str]] = ..., producer_id: _Optional[str] = ..., logs: _Optional[_Iterable[_Union[_execution_pb2.TaskLog, _Mapping]]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., input_uri: _Optional[str] = ..., output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., custom_info: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., phase_version: _Optional[int] = ..., reason: _Optional[str] = ..., task_type: _Optional[str] = ..., metadata: _Optional[_Union[TaskExecutionMetadata, _Mapping]] = ..., event_version: _Optional[int] = ...) -> None: ...
+    metadata: TaskExecutionMetadata
+    event_version: int
+    reported_at: _timestamp_pb2.Timestamp
+    def __init__(self, task_id: _Optional[_Union[_identifier_pb2.Identifier, _Mapping]] = ..., parent_node_execution_id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ..., retry_attempt: _Optional[int] = ..., phase: _Optional[_Union[_execution_pb2.TaskExecution.Phase, str]] = ..., producer_id: _Optional[str] = ..., logs: _Optional[_Iterable[_Union[_execution_pb2.TaskLog, _Mapping]]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., input_uri: _Optional[str] = ..., input_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., custom_info: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., phase_version: _Optional[int] = ..., reason: _Optional[str] = ..., task_type: _Optional[str] = ..., metadata: _Optional[_Union[TaskExecutionMetadata, _Mapping]] = ..., event_version: _Optional[int] = ..., reported_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+
+class ExternalResourceInfo(_message.Message):
+    __slots__ = ["external_id", "index", "retry_attempt", "phase", "cache_status", "logs"]
+    EXTERNAL_ID_FIELD_NUMBER: _ClassVar[int]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    RETRY_ATTEMPT_FIELD_NUMBER: _ClassVar[int]
+    PHASE_FIELD_NUMBER: _ClassVar[int]
+    CACHE_STATUS_FIELD_NUMBER: _ClassVar[int]
+    LOGS_FIELD_NUMBER: _ClassVar[int]
+    external_id: str
+    index: int
+    retry_attempt: int
+    phase: _execution_pb2.TaskExecution.Phase
+    cache_status: _catalog_pb2.CatalogCacheStatus
+    logs: _containers.RepeatedCompositeFieldContainer[_execution_pb2.TaskLog]
+    def __init__(self, external_id: _Optional[str] = ..., index: _Optional[int] = ..., retry_attempt: _Optional[int] = ..., phase: _Optional[_Union[_execution_pb2.TaskExecution.Phase, str]] = ..., cache_status: _Optional[_Union[_catalog_pb2.CatalogCacheStatus, str]] = ..., logs: _Optional[_Iterable[_Union[_execution_pb2.TaskLog, _Mapping]]] = ...) -> None: ...
+
+class ResourcePoolInfo(_message.Message):
+    __slots__ = ["allocation_token", "namespace"]
+    ALLOCATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    allocation_token: str
+    namespace: str
+    def __init__(self, allocation_token: _Optional[str] = ..., namespace: _Optional[str] = ...) -> None: ...
 
 class TaskExecutionMetadata(_message.Message):
-    __slots__ = ["external_resources", "generated_name", "instance_class", "plugin_identifier", "resource_pool_info"]
+    __slots__ = ["generated_name", "external_resources", "resource_pool_info", "plugin_identifier", "instance_class"]
     class InstanceClass(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        DEFAULT: _ClassVar[TaskExecutionMetadata.InstanceClass]
+        INTERRUPTIBLE: _ClassVar[TaskExecutionMetadata.InstanceClass]
     DEFAULT: TaskExecutionMetadata.InstanceClass
-    EXTERNAL_RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    GENERATED_NAME_FIELD_NUMBER: _ClassVar[int]
-    INSTANCE_CLASS_FIELD_NUMBER: _ClassVar[int]
     INTERRUPTIBLE: TaskExecutionMetadata.InstanceClass
-    PLUGIN_IDENTIFIER_FIELD_NUMBER: _ClassVar[int]
+    GENERATED_NAME_FIELD_NUMBER: _ClassVar[int]
+    EXTERNAL_RESOURCES_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_POOL_INFO_FIELD_NUMBER: _ClassVar[int]
-    external_resources: _containers.RepeatedCompositeFieldContainer[ExternalResourceInfo]
+    PLUGIN_IDENTIFIER_FIELD_NUMBER: _ClassVar[int]
+    INSTANCE_CLASS_FIELD_NUMBER: _ClassVar[int]
     generated_name: str
-    instance_class: TaskExecutionMetadata.InstanceClass
-    plugin_identifier: str
+    external_resources: _containers.RepeatedCompositeFieldContainer[ExternalResourceInfo]
     resource_pool_info: _containers.RepeatedCompositeFieldContainer[ResourcePoolInfo]
+    plugin_identifier: str
+    instance_class: TaskExecutionMetadata.InstanceClass
     def __init__(self, generated_name: _Optional[str] = ..., external_resources: _Optional[_Iterable[_Union[ExternalResourceInfo, _Mapping]]] = ..., resource_pool_info: _Optional[_Iterable[_Union[ResourcePoolInfo, _Mapping]]] = ..., plugin_identifier: _Optional[str] = ..., instance_class: _Optional[_Union[TaskExecutionMetadata.InstanceClass, str]] = ...) -> None: ...
-
-class TaskNodeMetadata(_message.Message):
-    __slots__ = ["cache_status", "catalog_key", "checkpoint_uri", "dynamic_workflow", "reservation_status"]
-    CACHE_STATUS_FIELD_NUMBER: _ClassVar[int]
-    CATALOG_KEY_FIELD_NUMBER: _ClassVar[int]
-    CHECKPOINT_URI_FIELD_NUMBER: _ClassVar[int]
-    DYNAMIC_WORKFLOW_FIELD_NUMBER: _ClassVar[int]
-    RESERVATION_STATUS_FIELD_NUMBER: _ClassVar[int]
-    cache_status: _catalog_pb2.CatalogCacheStatus
-    catalog_key: _catalog_pb2.CatalogMetadata
-    checkpoint_uri: str
-    dynamic_workflow: DynamicWorkflowNodeMetadata
-    reservation_status: _catalog_pb2.CatalogReservation.Status
-    def __init__(self, cache_status: _Optional[_Union[_catalog_pb2.CatalogCacheStatus, str]] = ..., catalog_key: _Optional[_Union[_catalog_pb2.CatalogMetadata, _Mapping]] = ..., reservation_status: _Optional[_Union[_catalog_pb2.CatalogReservation.Status, str]] = ..., checkpoint_uri: _Optional[str] = ..., dynamic_workflow: _Optional[_Union[DynamicWorkflowNodeMetadata, _Mapping]] = ...) -> None: ...
-
-class WorkflowExecutionEvent(_message.Message):
-    __slots__ = ["error", "execution_id", "occurred_at", "output_data", "output_uri", "phase", "producer_id"]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    OCCURRED_AT_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_DATA_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_URI_FIELD_NUMBER: _ClassVar[int]
-    PHASE_FIELD_NUMBER: _ClassVar[int]
-    PRODUCER_ID_FIELD_NUMBER: _ClassVar[int]
-    error: _execution_pb2.ExecutionError
-    execution_id: _identifier_pb2.WorkflowExecutionIdentifier
-    occurred_at: _timestamp_pb2.Timestamp
-    output_data: _literals_pb2.LiteralMap
-    output_uri: str
-    phase: _execution_pb2.WorkflowExecution.Phase
-    producer_id: str
-    def __init__(self, execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., producer_id: _Optional[str] = ..., phase: _Optional[_Union[_execution_pb2.WorkflowExecution.Phase, str]] = ..., occurred_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., output_uri: _Optional[str] = ..., error: _Optional[_Union[_execution_pb2.ExecutionError, _Mapping]] = ..., output_data: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ...) -> None: ...
-
-class WorkflowNodeMetadata(_message.Message):
-    __slots__ = ["execution_id"]
-    EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    execution_id: _identifier_pb2.WorkflowExecutionIdentifier
-    def __init__(self, execution_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/array_job_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/array_job_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n flyteidl/plugins/array_job.proto\x12\x10\x66lyteidl.plugins\"\xa9\x01\n\x08\x41rrayJob\x12 \n\x0bparallelism\x18\x01 \x01(\x03R\x0bparallelism\x12\x12\n\x04size\x18\x02 \x01(\x03R\x04size\x12%\n\rmin_successes\x18\x03 \x01(\x03H\x00R\x0cminSuccesses\x12,\n\x11min_success_ratio\x18\x04 \x01(\x02H\x00R\x0fminSuccessRatioB\x12\n\x10success_criteriaB\xbf\x01\n\x14\x63om.flyteidl.pluginsB\rArrayJobProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.array_job_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.array_job_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\rArrayJobProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
-  _ARRAYJOB._serialized_start=55
-  _ARRAYJOB._serialized_end=224
+  _globals['_ARRAYJOB']._serialized_start=55
+  _globals['_ARRAYJOB']._serialized_end=224
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/array_job_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/array_job_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ArrayJob(_message.Message):
-    __slots__ = ["min_success_ratio", "min_successes", "parallelism", "size"]
-    MIN_SUCCESSES_FIELD_NUMBER: _ClassVar[int]
-    MIN_SUCCESS_RATIO_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["parallelism", "size", "min_successes", "min_success_ratio"]
     PARALLELISM_FIELD_NUMBER: _ClassVar[int]
     SIZE_FIELD_NUMBER: _ClassVar[int]
-    min_success_ratio: float
-    min_successes: int
+    MIN_SUCCESSES_FIELD_NUMBER: _ClassVar[int]
+    MIN_SUCCESS_RATIO_FIELD_NUMBER: _ClassVar[int]
     parallelism: int
     size: int
+    min_successes: int
+    min_success_ratio: float
     def __init__(self, parallelism: _Optional[int] = ..., size: _Optional[int] = ..., min_successes: _Optional[int] = ..., min_success_ratio: _Optional[float] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/dask_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/mpi_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/plugins/dask.proto
+# source: flyteidl/plugins/mpi.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from flyteidl.core import tasks_pb2 as flyteidl_dot_core_dot_tasks__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/plugins/dask.proto\x12\x10\x66lyteidl.plugins\x1a\x19\x66lyteidl/core/tasks.proto\"\x85\x01\n\x07\x44\x61skJob\x12=\n\tscheduler\x18\x01 \x01(\x0b\x32\x1f.flyteidl.plugins.DaskSchedulerR\tscheduler\x12;\n\x07workers\x18\x02 \x01(\x0b\x32!.flyteidl.plugins.DaskWorkerGroupR\x07workers\"]\n\rDaskScheduler\x12\x14\n\x05image\x18\x01 \x01(\tR\x05image\x12\x36\n\tresources\x18\x02 \x01(\x0b\x32\x18.flyteidl.core.ResourcesR\tresources\"\x8b\x01\n\x0f\x44\x61skWorkerGroup\x12*\n\x11number_of_workers\x18\x01 \x01(\rR\x0fnumberOfWorkers\x12\x14\n\x05image\x18\x02 \x01(\tR\x05image\x12\x36\n\tresources\x18\x03 \x01(\x0b\x32\x18.flyteidl.core.ResourcesR\tresourcesB\xbb\x01\n\x14\x63om.flyteidl.pluginsB\tDaskProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66lyteidl/plugins/mpi.proto\x12\x10\x66lyteidl.plugins\"\x87\x01\n\x1a\x44istributedMPITrainingTask\x12\x1f\n\x0bnum_workers\x18\x01 \x01(\x05R\nnumWorkers\x12\x32\n\x15num_launcher_replicas\x18\x02 \x01(\x05R\x13numLauncherReplicas\x12\x14\n\x05slots\x18\x03 \x01(\x05R\x05slotsB\xba\x01\n\x14\x63om.flyteidl.pluginsB\x08MpiProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.dask_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.mpi_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\tDaskProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
-  _DASKJOB._serialized_start=77
-  _DASKJOB._serialized_end=210
-  _DASKSCHEDULER._serialized_start=212
-  _DASKSCHEDULER._serialized_end=305
-  _DASKWORKERGROUP._serialized_start=308
-  _DASKWORKERGROUP._serialized_end=447
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\010MpiProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
+  _globals['_DISTRIBUTEDMPITRAININGTASK']._serialized_start=49
+  _globals['_DISTRIBUTEDMPITRAININGTASK']._serialized_end=184
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/dask_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/dask_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     IMAGE_FIELD_NUMBER: _ClassVar[int]
     RESOURCES_FIELD_NUMBER: _ClassVar[int]
     image: str
     resources: _tasks_pb2.Resources
     def __init__(self, image: _Optional[str] = ..., resources: _Optional[_Union[_tasks_pb2.Resources, _Mapping]] = ...) -> None: ...
 
 class DaskWorkerGroup(_message.Message):
-    __slots__ = ["image", "number_of_workers", "resources"]
-    IMAGE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["number_of_workers", "image", "resources"]
     NUMBER_OF_WORKERS_FIELD_NUMBER: _ClassVar[int]
+    IMAGE_FIELD_NUMBER: _ClassVar[int]
     RESOURCES_FIELD_NUMBER: _ClassVar[int]
-    image: str
     number_of_workers: int
+    image: str
     resources: _tasks_pb2.Resources
     def __init__(self, number_of_workers: _Optional[int] = ..., image: _Optional[str] = ..., resources: _Optional[_Union[_tasks_pb2.Resources, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/mpi_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/tensorflow_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/plugins/mpi.proto
+# source: flyteidl/plugins/tensorflow.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66lyteidl/plugins/mpi.proto\x12\x10\x66lyteidl.plugins\"\x87\x01\n\x1a\x44istributedMPITrainingTask\x12\x1f\n\x0bnum_workers\x18\x01 \x01(\x05R\nnumWorkers\x12\x32\n\x15num_launcher_replicas\x18\x02 \x01(\x05R\x13numLauncherReplicas\x12\x14\n\x05slots\x18\x03 \x01(\x05R\x05slotsB\xba\x01\n\x14\x63om.flyteidl.pluginsB\x08MpiProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!flyteidl/plugins/tensorflow.proto\x12\x10\x66lyteidl.plugins\"\x85\x01\n!DistributedTensorflowTrainingTask\x12\x18\n\x07workers\x18\x01 \x01(\x05R\x07workers\x12\x1f\n\x0bps_replicas\x18\x02 \x01(\x05R\npsReplicas\x12%\n\x0e\x63hief_replicas\x18\x03 \x01(\x05R\rchiefReplicasB\xc1\x01\n\x14\x63om.flyteidl.pluginsB\x0fTensorflowProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.mpi_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.tensorflow_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\010MpiProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
-  _DISTRIBUTEDMPITRAININGTASK._serialized_start=49
-  _DISTRIBUTEDMPITRAININGTASK._serialized_end=184
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\017TensorflowProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
+  _globals['_DISTRIBUTEDTENSORFLOWTRAININGTASK']._serialized_start=56
+  _globals['_DISTRIBUTEDTENSORFLOWTRAININGTASK']._serialized_end=189
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/mpi_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/mpi_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DistributedMPITrainingTask(_message.Message):
-    __slots__ = ["num_launcher_replicas", "num_workers", "slots"]
-    NUM_LAUNCHER_REPLICAS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["num_workers", "num_launcher_replicas", "slots"]
     NUM_WORKERS_FIELD_NUMBER: _ClassVar[int]
+    NUM_LAUNCHER_REPLICAS_FIELD_NUMBER: _ClassVar[int]
     SLOTS_FIELD_NUMBER: _ClassVar[int]
-    num_launcher_replicas: int
     num_workers: int
+    num_launcher_replicas: int
     slots: int
     def __init__(self, num_workers: _Optional[int] = ..., num_launcher_replicas: _Optional[int] = ..., slots: _Optional[int] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/presto_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/presto_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/plugins/presto.proto\x12\x10\x66lyteidl.plugins\"\x82\x01\n\x0bPrestoQuery\x12#\n\rrouting_group\x18\x01 \x01(\tR\x0croutingGroup\x12\x18\n\x07\x63\x61talog\x18\x02 \x01(\tR\x07\x63\x61talog\x12\x16\n\x06schema\x18\x03 \x01(\tR\x06schema\x12\x1c\n\tstatement\x18\x04 \x01(\tR\tstatementB\xbd\x01\n\x14\x63om.flyteidl.pluginsB\x0bPrestoProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.presto_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.presto_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\013PrestoProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
-  _PRESTOQUERY._serialized_start=52
-  _PRESTOQUERY._serialized_end=182
+  _globals['_PRESTOQUERY']._serialized_start=52
+  _globals['_PRESTOQUERY']._serialized_end=182
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/presto_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/presto_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PrestoQuery(_message.Message):
-    __slots__ = ["catalog", "routing_group", "schema", "statement"]
-    CATALOG_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["routing_group", "catalog", "schema", "statement"]
     ROUTING_GROUP_FIELD_NUMBER: _ClassVar[int]
+    CATALOG_FIELD_NUMBER: _ClassVar[int]
     SCHEMA_FIELD_NUMBER: _ClassVar[int]
     STATEMENT_FIELD_NUMBER: _ClassVar[int]
-    catalog: str
     routing_group: str
+    catalog: str
     schema: str
     statement: str
     def __init__(self, routing_group: _Optional[str] = ..., catalog: _Optional[str] = ..., schema: _Optional[str] = ..., statement: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/pytorch_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/waitable_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/plugins/pytorch.proto
+# source: flyteidl/plugins/waitable.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from flyteidl.core import execution_pb2 as flyteidl_dot_core_dot_execution__pb2
+from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x66lyteidl/plugins/pytorch.proto\x12\x10\x66lyteidl.plugins\":\n\x1e\x44istributedPyTorchTrainingTask\x12\x18\n\x07workers\x18\x01 \x01(\x05R\x07workersB\xbe\x01\n\x14\x63om.flyteidl.pluginsB\x0cPytorchProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66lyteidl/plugins/waitable.proto\x12\x10\x66lyteidl.plugins\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\"\xb3\x01\n\x08Waitable\x12H\n\nwf_exec_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x08wfExecId\x12<\n\x05phase\x18\x02 \x01(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x05phase\x12\x1f\n\x0bworkflow_id\x18\x03 \x01(\tR\nworkflowIdB\xbf\x01\n\x14\x63om.flyteidl.pluginsB\rWaitableProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.pytorch_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.waitable_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\014PytorchProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
-  _DISTRIBUTEDPYTORCHTRAININGTASK._serialized_start=52
-  _DISTRIBUTEDPYTORCHTRAININGTASK._serialized_end=110
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\rWaitableProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
+  _globals['_WAITABLE']._serialized_start=117
+  _globals['_WAITABLE']._serialized_end=296
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/qubole_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/qubole_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/plugins/qubole.proto\x12\x10\x66lyteidl.plugins\"b\n\tHiveQuery\x12\x14\n\x05query\x18\x01 \x01(\tR\x05query\x12\x1f\n\x0btimeout_sec\x18\x02 \x01(\rR\ntimeoutSec\x12\x1e\n\nretryCount\x18\x03 \x01(\rR\nretryCount\"L\n\x13HiveQueryCollection\x12\x35\n\x07queries\x18\x02 \x03(\x0b\x32\x1b.flyteidl.plugins.HiveQueryR\x07queries\"\xd1\x01\n\rQuboleHiveJob\x12#\n\rcluster_label\x18\x01 \x01(\tR\x0c\x63lusterLabel\x12T\n\x10query_collection\x18\x02 \x01(\x0b\x32%.flyteidl.plugins.HiveQueryCollectionB\x02\x18\x01R\x0fqueryCollection\x12\x12\n\x04tags\x18\x03 \x03(\tR\x04tags\x12\x31\n\x05query\x18\x04 \x01(\x0b\x32\x1b.flyteidl.plugins.HiveQueryR\x05queryB\xbd\x01\n\x14\x63om.flyteidl.pluginsB\x0bQuboleProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.qubole_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.qubole_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\013QuboleProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
   _QUBOLEHIVEJOB.fields_by_name['query_collection']._options = None
   _QUBOLEHIVEJOB.fields_by_name['query_collection']._serialized_options = b'\030\001'
-  _HIVEQUERY._serialized_start=51
-  _HIVEQUERY._serialized_end=149
-  _HIVEQUERYCOLLECTION._serialized_start=151
-  _HIVEQUERYCOLLECTION._serialized_end=227
-  _QUBOLEHIVEJOB._serialized_start=230
-  _QUBOLEHIVEJOB._serialized_end=439
+  _globals['_HIVEQUERY']._serialized_start=51
+  _globals['_HIVEQUERY']._serialized_end=149
+  _globals['_HIVEQUERYCOLLECTION']._serialized_start=151
+  _globals['_HIVEQUERYCOLLECTION']._serialized_end=227
+  _globals['_QUBOLEHIVEJOB']._serialized_start=230
+  _globals['_QUBOLEHIVEJOB']._serialized_end=439
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/qubole_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/qubole_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class HiveQuery(_message.Message):
-    __slots__ = ["query", "retryCount", "timeout_sec"]
+    __slots__ = ["query", "timeout_sec", "retryCount"]
     QUERY_FIELD_NUMBER: _ClassVar[int]
-    RETRYCOUNT_FIELD_NUMBER: _ClassVar[int]
     TIMEOUT_SEC_FIELD_NUMBER: _ClassVar[int]
+    RETRYCOUNT_FIELD_NUMBER: _ClassVar[int]
     query: str
-    retryCount: int
     timeout_sec: int
+    retryCount: int
     def __init__(self, query: _Optional[str] = ..., timeout_sec: _Optional[int] = ..., retryCount: _Optional[int] = ...) -> None: ...
 
 class HiveQueryCollection(_message.Message):
     __slots__ = ["queries"]
     QUERIES_FIELD_NUMBER: _ClassVar[int]
     queries: _containers.RepeatedCompositeFieldContainer[HiveQuery]
     def __init__(self, queries: _Optional[_Iterable[_Union[HiveQuery, _Mapping]]] = ...) -> None: ...
 
 class QuboleHiveJob(_message.Message):
-    __slots__ = ["cluster_label", "query", "query_collection", "tags"]
+    __slots__ = ["cluster_label", "query_collection", "tags", "query"]
     CLUSTER_LABEL_FIELD_NUMBER: _ClassVar[int]
     QUERY_COLLECTION_FIELD_NUMBER: _ClassVar[int]
-    QUERY_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
+    QUERY_FIELD_NUMBER: _ClassVar[int]
     cluster_label: str
-    query: HiveQuery
     query_collection: HiveQueryCollection
     tags: _containers.RepeatedScalarFieldContainer[str]
+    query: HiveQuery
     def __init__(self, cluster_label: _Optional[str] = ..., query_collection: _Optional[_Union[HiveQueryCollection, _Mapping]] = ..., tags: _Optional[_Iterable[str]] = ..., query: _Optional[_Union[HiveQuery, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/ray_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/spark_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/plugins/ray.proto
+# source: flyteidl/plugins/spark.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66lyteidl/plugins/ray.proto\x12\x10\x66lyteidl.plugins\"h\n\x06RayJob\x12=\n\x0bray_cluster\x18\x01 \x01(\x0b\x32\x1c.flyteidl.plugins.RayClusterR\nrayCluster\x12\x1f\n\x0bruntime_env\x18\x02 \x01(\tR\nruntimeEnv\"\xa4\x01\n\nRayCluster\x12G\n\x0fhead_group_spec\x18\x01 \x01(\x0b\x32\x1f.flyteidl.plugins.HeadGroupSpecR\rheadGroupSpec\x12M\n\x11worker_group_spec\x18\x02 \x03(\x0b\x32!.flyteidl.plugins.WorkerGroupSpecR\x0fworkerGroupSpec\"\xb1\x01\n\rHeadGroupSpec\x12]\n\x10ray_start_params\x18\x01 \x03(\x0b\x32\x33.flyteidl.plugins.HeadGroupSpec.RayStartParamsEntryR\x0erayStartParams\x1a\x41\n\x13RayStartParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xb6\x02\n\x0fWorkerGroupSpec\x12\x1d\n\ngroup_name\x18\x01 \x01(\tR\tgroupName\x12\x1a\n\x08replicas\x18\x02 \x01(\x05R\x08replicas\x12!\n\x0cmin_replicas\x18\x03 \x01(\x05R\x0bminReplicas\x12!\n\x0cmax_replicas\x18\x04 \x01(\x05R\x0bmaxReplicas\x12_\n\x10ray_start_params\x18\x05 \x03(\x0b\x32\x35.flyteidl.plugins.WorkerGroupSpec.RayStartParamsEntryR\x0erayStartParams\x1a\x41\n\x13RayStartParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\xba\x01\n\x14\x63om.flyteidl.pluginsB\x08RayProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/plugins/spark.proto\x12\x10\x66lyteidl.plugins\x1a\x1cgoogle/protobuf/struct.proto\"B\n\x10SparkApplication\".\n\x04Type\x12\n\n\x06PYTHON\x10\x00\x12\x08\n\x04JAVA\x10\x01\x12\t\n\x05SCALA\x10\x02\x12\x05\n\x01R\x10\x03\"\xfe\x04\n\x08SparkJob\x12Q\n\x0f\x61pplicationType\x18\x01 \x01(\x0e\x32\'.flyteidl.plugins.SparkApplication.TypeR\x0f\x61pplicationType\x12\x30\n\x13mainApplicationFile\x18\x02 \x01(\tR\x13mainApplicationFile\x12\x1c\n\tmainClass\x18\x03 \x01(\tR\tmainClass\x12G\n\tsparkConf\x18\x04 \x03(\x0b\x32).flyteidl.plugins.SparkJob.SparkConfEntryR\tsparkConf\x12J\n\nhadoopConf\x18\x05 \x03(\x0b\x32*.flyteidl.plugins.SparkJob.HadoopConfEntryR\nhadoopConf\x12\"\n\x0c\x65xecutorPath\x18\x06 \x01(\tR\x0c\x65xecutorPath\x12?\n\x0e\x64\x61tabricksConf\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructR\x0e\x64\x61tabricksConf\x12(\n\x0f\x64\x61tabricksToken\x18\x08 \x01(\tR\x0f\x64\x61tabricksToken\x12.\n\x12\x64\x61tabricksInstance\x18\t \x01(\tR\x12\x64\x61tabricksInstance\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a=\n\x0fHadoopConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\xbc\x01\n\x14\x63om.flyteidl.pluginsB\nSparkProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.ray_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.spark_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\010RayProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
-  _HEADGROUPSPEC_RAYSTARTPARAMSENTRY._options = None
-  _HEADGROUPSPEC_RAYSTARTPARAMSENTRY._serialized_options = b'8\001'
-  _WORKERGROUPSPEC_RAYSTARTPARAMSENTRY._options = None
-  _WORKERGROUPSPEC_RAYSTARTPARAMSENTRY._serialized_options = b'8\001'
-  _RAYJOB._serialized_start=48
-  _RAYJOB._serialized_end=152
-  _RAYCLUSTER._serialized_start=155
-  _RAYCLUSTER._serialized_end=319
-  _HEADGROUPSPEC._serialized_start=322
-  _HEADGROUPSPEC._serialized_end=499
-  _HEADGROUPSPEC_RAYSTARTPARAMSENTRY._serialized_start=434
-  _HEADGROUPSPEC_RAYSTARTPARAMSENTRY._serialized_end=499
-  _WORKERGROUPSPEC._serialized_start=502
-  _WORKERGROUPSPEC._serialized_end=812
-  _WORKERGROUPSPEC_RAYSTARTPARAMSENTRY._serialized_start=434
-  _WORKERGROUPSPEC_RAYSTARTPARAMSENTRY._serialized_end=499
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\nSparkProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
+  _SPARKJOB_SPARKCONFENTRY._options = None
+  _SPARKJOB_SPARKCONFENTRY._serialized_options = b'8\001'
+  _SPARKJOB_HADOOPCONFENTRY._options = None
+  _SPARKJOB_HADOOPCONFENTRY._serialized_options = b'8\001'
+  _globals['_SPARKAPPLICATION']._serialized_start=80
+  _globals['_SPARKAPPLICATION']._serialized_end=146
+  _globals['_SPARKAPPLICATION_TYPE']._serialized_start=100
+  _globals['_SPARKAPPLICATION_TYPE']._serialized_end=146
+  _globals['_SPARKJOB']._serialized_start=149
+  _globals['_SPARKJOB']._serialized_end=787
+  _globals['_SPARKJOB_SPARKCONFENTRY']._serialized_start=664
+  _globals['_SPARKJOB_SPARKCONFENTRY']._serialized_end=724
+  _globals['_SPARKJOB_HADOOPCONFENTRY']._serialized_start=726
+  _globals['_SPARKJOB_HADOOPCONFENTRY']._serialized_end=787
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/ray_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/ray_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class RayJob(_message.Message):
+    __slots__ = ["ray_cluster", "runtime_env"]
+    RAY_CLUSTER_FIELD_NUMBER: _ClassVar[int]
+    RUNTIME_ENV_FIELD_NUMBER: _ClassVar[int]
+    ray_cluster: RayCluster
+    runtime_env: str
+    def __init__(self, ray_cluster: _Optional[_Union[RayCluster, _Mapping]] = ..., runtime_env: _Optional[str] = ...) -> None: ...
+
+class RayCluster(_message.Message):
+    __slots__ = ["head_group_spec", "worker_group_spec"]
+    HEAD_GROUP_SPEC_FIELD_NUMBER: _ClassVar[int]
+    WORKER_GROUP_SPEC_FIELD_NUMBER: _ClassVar[int]
+    head_group_spec: HeadGroupSpec
+    worker_group_spec: _containers.RepeatedCompositeFieldContainer[WorkerGroupSpec]
+    def __init__(self, head_group_spec: _Optional[_Union[HeadGroupSpec, _Mapping]] = ..., worker_group_spec: _Optional[_Iterable[_Union[WorkerGroupSpec, _Mapping]]] = ...) -> None: ...
+
 class HeadGroupSpec(_message.Message):
     __slots__ = ["ray_start_params"]
     class RayStartParamsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     RAY_START_PARAMS_FIELD_NUMBER: _ClassVar[int]
     ray_start_params: _containers.ScalarMap[str, str]
     def __init__(self, ray_start_params: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
-class RayCluster(_message.Message):
-    __slots__ = ["head_group_spec", "worker_group_spec"]
-    HEAD_GROUP_SPEC_FIELD_NUMBER: _ClassVar[int]
-    WORKER_GROUP_SPEC_FIELD_NUMBER: _ClassVar[int]
-    head_group_spec: HeadGroupSpec
-    worker_group_spec: _containers.RepeatedCompositeFieldContainer[WorkerGroupSpec]
-    def __init__(self, head_group_spec: _Optional[_Union[HeadGroupSpec, _Mapping]] = ..., worker_group_spec: _Optional[_Iterable[_Union[WorkerGroupSpec, _Mapping]]] = ...) -> None: ...
-
-class RayJob(_message.Message):
-    __slots__ = ["ray_cluster", "runtime_env"]
-    RAY_CLUSTER_FIELD_NUMBER: _ClassVar[int]
-    RUNTIME_ENV_FIELD_NUMBER: _ClassVar[int]
-    ray_cluster: RayCluster
-    runtime_env: str
-    def __init__(self, ray_cluster: _Optional[_Union[RayCluster, _Mapping]] = ..., runtime_env: _Optional[str] = ...) -> None: ...
-
 class WorkerGroupSpec(_message.Message):
-    __slots__ = ["group_name", "max_replicas", "min_replicas", "ray_start_params", "replicas"]
+    __slots__ = ["group_name", "replicas", "min_replicas", "max_replicas", "ray_start_params"]
     class RayStartParamsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     GROUP_NAME_FIELD_NUMBER: _ClassVar[int]
-    MAX_REPLICAS_FIELD_NUMBER: _ClassVar[int]
+    REPLICAS_FIELD_NUMBER: _ClassVar[int]
     MIN_REPLICAS_FIELD_NUMBER: _ClassVar[int]
+    MAX_REPLICAS_FIELD_NUMBER: _ClassVar[int]
     RAY_START_PARAMS_FIELD_NUMBER: _ClassVar[int]
-    REPLICAS_FIELD_NUMBER: _ClassVar[int]
     group_name: str
-    max_replicas: int
+    replicas: int
     min_replicas: int
+    max_replicas: int
     ray_start_params: _containers.ScalarMap[str, str]
-    replicas: int
     def __init__(self, group_name: _Optional[str] = ..., replicas: _Optional[int] = ..., min_replicas: _Optional[int] = ..., max_replicas: _Optional[int] = ..., ray_start_params: _Optional[_Mapping[str, str]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 
 from flyteidl.plugins.sagemaker import parameter_ranges_pb2 as flyteidl_dot_plugins_dot_sagemaker_dot_parameter__ranges__pb2
 from flyteidl.plugins.sagemaker import training_job_pb2 as flyteidl_dot_plugins_dot_sagemaker_dot_training__job__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n:flyteidl/plugins/sagemaker/hyperparameter_tuning_job.proto\x12\x1a\x66lyteidl.plugins.sagemaker\x1a\x31\x66lyteidl/plugins/sagemaker/parameter_ranges.proto\x1a-flyteidl/plugins/sagemaker/training_job.proto\"\xe0\x01\n\x17HyperparameterTuningJob\x12J\n\x0ctraining_job\x18\x01 \x01(\x0b\x32\'.flyteidl.plugins.sagemaker.TrainingJobR\x0btrainingJob\x12<\n\x1bmax_number_of_training_jobs\x18\x02 \x01(\x03R\x17maxNumberOfTrainingJobs\x12;\n\x1amax_parallel_training_jobs\x18\x03 \x01(\x03R\x17maxParallelTrainingJobs\"H\n!HyperparameterTuningObjectiveType\"#\n\x05Value\x12\x0c\n\x08MINIMIZE\x10\x00\x12\x0c\n\x08MAXIMIZE\x10\x01\"\xac\x01\n\x1dHyperparameterTuningObjective\x12j\n\x0eobjective_type\x18\x01 \x01(\x0e\x32\x43.flyteidl.plugins.sagemaker.HyperparameterTuningObjectiveType.ValueR\robjectiveType\x12\x1f\n\x0bmetric_name\x18\x02 \x01(\tR\nmetricName\"A\n\x1cHyperparameterTuningStrategy\"!\n\x05Value\x12\x0c\n\x08\x42\x41YESIAN\x10\x00\x12\n\n\x06RANDOM\x10\x01\":\n\x1cTrainingJobEarlyStoppingType\"\x1a\n\x05Value\x12\x07\n\x03OFF\x10\x00\x12\x08\n\x04\x41UTO\x10\x01\"\xd9\x03\n\x1dHyperparameterTuningJobConfig\x12`\n\x15hyperparameter_ranges\x18\x01 \x01(\x0b\x32+.flyteidl.plugins.sagemaker.ParameterRangesR\x14hyperparameterRanges\x12g\n\x0ftuning_strategy\x18\x02 \x01(\x0e\x32>.flyteidl.plugins.sagemaker.HyperparameterTuningStrategy.ValueR\x0etuningStrategy\x12\x64\n\x10tuning_objective\x18\x03 \x01(\x0b\x32\x39.flyteidl.plugins.sagemaker.HyperparameterTuningObjectiveR\x0ftuningObjective\x12\x86\x01\n training_job_early_stopping_type\x18\x04 \x01(\x0e\x32>.flyteidl.plugins.sagemaker.TrainingJobEarlyStoppingType.ValueR\x1ctrainingJobEarlyStoppingTypeB\x81\x02\n\x1e\x63om.flyteidl.plugins.sagemakerB\x1cHyperparameterTuningJobProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PS\xaa\x02\x1a\x46lyteidl.Plugins.Sagemaker\xca\x02\x1a\x46lyteidl\\Plugins\\Sagemaker\xe2\x02&Flyteidl\\Plugins\\Sagemaker\\GPBMetadata\xea\x02\x1c\x46lyteidl::Plugins::Sagemakerb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.sagemaker.hyperparameter_tuning_job_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.sagemaker.hyperparameter_tuning_job_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.flyteidl.plugins.sagemakerB\034HyperparameterTuningJobProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPS\252\002\032Flyteidl.Plugins.Sagemaker\312\002\032Flyteidl\\Plugins\\Sagemaker\342\002&Flyteidl\\Plugins\\Sagemaker\\GPBMetadata\352\002\034Flyteidl::Plugins::Sagemaker'
-  _HYPERPARAMETERTUNINGJOB._serialized_start=189
-  _HYPERPARAMETERTUNINGJOB._serialized_end=413
-  _HYPERPARAMETERTUNINGOBJECTIVETYPE._serialized_start=415
-  _HYPERPARAMETERTUNINGOBJECTIVETYPE._serialized_end=487
-  _HYPERPARAMETERTUNINGOBJECTIVETYPE_VALUE._serialized_start=452
-  _HYPERPARAMETERTUNINGOBJECTIVETYPE_VALUE._serialized_end=487
-  _HYPERPARAMETERTUNINGOBJECTIVE._serialized_start=490
-  _HYPERPARAMETERTUNINGOBJECTIVE._serialized_end=662
-  _HYPERPARAMETERTUNINGSTRATEGY._serialized_start=664
-  _HYPERPARAMETERTUNINGSTRATEGY._serialized_end=729
-  _HYPERPARAMETERTUNINGSTRATEGY_VALUE._serialized_start=696
-  _HYPERPARAMETERTUNINGSTRATEGY_VALUE._serialized_end=729
-  _TRAININGJOBEARLYSTOPPINGTYPE._serialized_start=731
-  _TRAININGJOBEARLYSTOPPINGTYPE._serialized_end=789
-  _TRAININGJOBEARLYSTOPPINGTYPE_VALUE._serialized_start=763
-  _TRAININGJOBEARLYSTOPPINGTYPE_VALUE._serialized_end=789
-  _HYPERPARAMETERTUNINGJOBCONFIG._serialized_start=792
-  _HYPERPARAMETERTUNINGJOBCONFIG._serialized_end=1265
+  _globals['_HYPERPARAMETERTUNINGJOB']._serialized_start=189
+  _globals['_HYPERPARAMETERTUNINGJOB']._serialized_end=413
+  _globals['_HYPERPARAMETERTUNINGOBJECTIVETYPE']._serialized_start=415
+  _globals['_HYPERPARAMETERTUNINGOBJECTIVETYPE']._serialized_end=487
+  _globals['_HYPERPARAMETERTUNINGOBJECTIVETYPE_VALUE']._serialized_start=452
+  _globals['_HYPERPARAMETERTUNINGOBJECTIVETYPE_VALUE']._serialized_end=487
+  _globals['_HYPERPARAMETERTUNINGOBJECTIVE']._serialized_start=490
+  _globals['_HYPERPARAMETERTUNINGOBJECTIVE']._serialized_end=662
+  _globals['_HYPERPARAMETERTUNINGSTRATEGY']._serialized_start=664
+  _globals['_HYPERPARAMETERTUNINGSTRATEGY']._serialized_end=729
+  _globals['_HYPERPARAMETERTUNINGSTRATEGY_VALUE']._serialized_start=696
+  _globals['_HYPERPARAMETERTUNINGSTRATEGY_VALUE']._serialized_end=729
+  _globals['_TRAININGJOBEARLYSTOPPINGTYPE']._serialized_start=731
+  _globals['_TRAININGJOBEARLYSTOPPINGTYPE']._serialized_end=789
+  _globals['_TRAININGJOBEARLYSTOPPINGTYPE_VALUE']._serialized_start=763
+  _globals['_TRAININGJOBEARLYSTOPPINGTYPE_VALUE']._serialized_end=789
+  _globals['_HYPERPARAMETERTUNINGJOBCONFIG']._serialized_start=792
+  _globals['_HYPERPARAMETERTUNINGJOBCONFIG']._serialized_end=1265
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,59 +4,65 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class HyperparameterTuningJob(_message.Message):
-    __slots__ = ["max_number_of_training_jobs", "max_parallel_training_jobs", "training_job"]
+    __slots__ = ["training_job", "max_number_of_training_jobs", "max_parallel_training_jobs"]
+    TRAINING_JOB_FIELD_NUMBER: _ClassVar[int]
     MAX_NUMBER_OF_TRAINING_JOBS_FIELD_NUMBER: _ClassVar[int]
     MAX_PARALLEL_TRAINING_JOBS_FIELD_NUMBER: _ClassVar[int]
-    TRAINING_JOB_FIELD_NUMBER: _ClassVar[int]
+    training_job: _training_job_pb2.TrainingJob
     max_number_of_training_jobs: int
     max_parallel_training_jobs: int
-    training_job: _training_job_pb2.TrainingJob
     def __init__(self, training_job: _Optional[_Union[_training_job_pb2.TrainingJob, _Mapping]] = ..., max_number_of_training_jobs: _Optional[int] = ..., max_parallel_training_jobs: _Optional[int] = ...) -> None: ...
 
-class HyperparameterTuningJobConfig(_message.Message):
-    __slots__ = ["hyperparameter_ranges", "training_job_early_stopping_type", "tuning_objective", "tuning_strategy"]
-    HYPERPARAMETER_RANGES_FIELD_NUMBER: _ClassVar[int]
-    TRAINING_JOB_EARLY_STOPPING_TYPE_FIELD_NUMBER: _ClassVar[int]
-    TUNING_OBJECTIVE_FIELD_NUMBER: _ClassVar[int]
-    TUNING_STRATEGY_FIELD_NUMBER: _ClassVar[int]
-    hyperparameter_ranges: _parameter_ranges_pb2.ParameterRanges
-    training_job_early_stopping_type: TrainingJobEarlyStoppingType.Value
-    tuning_objective: HyperparameterTuningObjective
-    tuning_strategy: HyperparameterTuningStrategy.Value
-    def __init__(self, hyperparameter_ranges: _Optional[_Union[_parameter_ranges_pb2.ParameterRanges, _Mapping]] = ..., tuning_strategy: _Optional[_Union[HyperparameterTuningStrategy.Value, str]] = ..., tuning_objective: _Optional[_Union[HyperparameterTuningObjective, _Mapping]] = ..., training_job_early_stopping_type: _Optional[_Union[TrainingJobEarlyStoppingType.Value, str]] = ...) -> None: ...
-
-class HyperparameterTuningObjective(_message.Message):
-    __slots__ = ["metric_name", "objective_type"]
-    METRIC_NAME_FIELD_NUMBER: _ClassVar[int]
-    OBJECTIVE_TYPE_FIELD_NUMBER: _ClassVar[int]
-    metric_name: str
-    objective_type: HyperparameterTuningObjectiveType.Value
-    def __init__(self, objective_type: _Optional[_Union[HyperparameterTuningObjectiveType.Value, str]] = ..., metric_name: _Optional[str] = ...) -> None: ...
-
 class HyperparameterTuningObjectiveType(_message.Message):
     __slots__ = []
     class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    MAXIMIZE: HyperparameterTuningObjectiveType.Value
+        MINIMIZE: _ClassVar[HyperparameterTuningObjectiveType.Value]
+        MAXIMIZE: _ClassVar[HyperparameterTuningObjectiveType.Value]
     MINIMIZE: HyperparameterTuningObjectiveType.Value
+    MAXIMIZE: HyperparameterTuningObjectiveType.Value
     def __init__(self) -> None: ...
 
+class HyperparameterTuningObjective(_message.Message):
+    __slots__ = ["objective_type", "metric_name"]
+    OBJECTIVE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    METRIC_NAME_FIELD_NUMBER: _ClassVar[int]
+    objective_type: HyperparameterTuningObjectiveType.Value
+    metric_name: str
+    def __init__(self, objective_type: _Optional[_Union[HyperparameterTuningObjectiveType.Value, str]] = ..., metric_name: _Optional[str] = ...) -> None: ...
+
 class HyperparameterTuningStrategy(_message.Message):
     __slots__ = []
     class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        BAYESIAN: _ClassVar[HyperparameterTuningStrategy.Value]
+        RANDOM: _ClassVar[HyperparameterTuningStrategy.Value]
     BAYESIAN: HyperparameterTuningStrategy.Value
     RANDOM: HyperparameterTuningStrategy.Value
     def __init__(self) -> None: ...
 
 class TrainingJobEarlyStoppingType(_message.Message):
     __slots__ = []
     class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    AUTO: TrainingJobEarlyStoppingType.Value
+        OFF: _ClassVar[TrainingJobEarlyStoppingType.Value]
+        AUTO: _ClassVar[TrainingJobEarlyStoppingType.Value]
     OFF: TrainingJobEarlyStoppingType.Value
+    AUTO: TrainingJobEarlyStoppingType.Value
     def __init__(self) -> None: ...
+
+class HyperparameterTuningJobConfig(_message.Message):
+    __slots__ = ["hyperparameter_ranges", "tuning_strategy", "tuning_objective", "training_job_early_stopping_type"]
+    HYPERPARAMETER_RANGES_FIELD_NUMBER: _ClassVar[int]
+    TUNING_STRATEGY_FIELD_NUMBER: _ClassVar[int]
+    TUNING_OBJECTIVE_FIELD_NUMBER: _ClassVar[int]
+    TRAINING_JOB_EARLY_STOPPING_TYPE_FIELD_NUMBER: _ClassVar[int]
+    hyperparameter_ranges: _parameter_ranges_pb2.ParameterRanges
+    tuning_strategy: HyperparameterTuningStrategy.Value
+    tuning_objective: HyperparameterTuningObjective
+    training_job_early_stopping_type: TrainingJobEarlyStoppingType.Value
+    def __init__(self, hyperparameter_ranges: _Optional[_Union[_parameter_ranges_pb2.ParameterRanges, _Mapping]] = ..., tuning_strategy: _Optional[_Union[HyperparameterTuningStrategy.Value, str]] = ..., tuning_objective: _Optional[_Union[HyperparameterTuningObjective, _Mapping]] = ..., training_job_early_stopping_type: _Optional[_Union[TrainingJobEarlyStoppingType.Value, str]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n1flyteidl/plugins/sagemaker/parameter_ranges.proto\x12\x1a\x66lyteidl.plugins.sagemaker\"c\n\x19HyperparameterScalingType\"F\n\x05Value\x12\x08\n\x04\x41UTO\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\x0f\n\x0bLOGARITHMIC\x10\x02\x12\x16\n\x12REVERSELOGARITHMIC\x10\x03\"\xb4\x01\n\x18\x43ontinuousParameterRange\x12\x1b\n\tmax_value\x18\x01 \x01(\x01R\x08maxValue\x12\x1b\n\tmin_value\x18\x02 \x01(\x01R\x08minValue\x12^\n\x0cscaling_type\x18\x03 \x01(\x0e\x32;.flyteidl.plugins.sagemaker.HyperparameterScalingType.ValueR\x0bscalingType\"\xb1\x01\n\x15IntegerParameterRange\x12\x1b\n\tmax_value\x18\x01 \x01(\x03R\x08maxValue\x12\x1b\n\tmin_value\x18\x02 \x01(\x03R\x08minValue\x12^\n\x0cscaling_type\x18\x03 \x01(\x0e\x32;.flyteidl.plugins.sagemaker.HyperparameterScalingType.ValueR\x0bscalingType\"3\n\x19\x43\x61tegoricalParameterRange\x12\x16\n\x06values\x18\x01 \x03(\tR\x06values\"\x89\x03\n\x13ParameterRangeOneOf\x12t\n\x1a\x63ontinuous_parameter_range\x18\x01 \x01(\x0b\x32\x34.flyteidl.plugins.sagemaker.ContinuousParameterRangeH\x00R\x18\x63ontinuousParameterRange\x12k\n\x17integer_parameter_range\x18\x02 \x01(\x0b\x32\x31.flyteidl.plugins.sagemaker.IntegerParameterRangeH\x00R\x15integerParameterRange\x12w\n\x1b\x63\x61tegorical_parameter_range\x18\x03 \x01(\x0b\x32\x35.flyteidl.plugins.sagemaker.CategoricalParameterRangeH\x00R\x19\x63\x61tegoricalParameterRangeB\x16\n\x14parameter_range_type\"\xfc\x01\n\x0fParameterRanges\x12r\n\x13parameter_range_map\x18\x01 \x03(\x0b\x32\x42.flyteidl.plugins.sagemaker.ParameterRanges.ParameterRangeMapEntryR\x11parameterRangeMap\x1au\n\x16ParameterRangeMapEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x45\n\x05value\x18\x02 \x01(\x0b\x32/.flyteidl.plugins.sagemaker.ParameterRangeOneOfR\x05value:\x02\x38\x01\x42\xf9\x01\n\x1e\x63om.flyteidl.plugins.sagemakerB\x14ParameterRangesProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PS\xaa\x02\x1a\x46lyteidl.Plugins.Sagemaker\xca\x02\x1a\x46lyteidl\\Plugins\\Sagemaker\xe2\x02&Flyteidl\\Plugins\\Sagemaker\\GPBMetadata\xea\x02\x1c\x46lyteidl::Plugins::Sagemakerb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.sagemaker.parameter_ranges_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.sagemaker.parameter_ranges_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.flyteidl.plugins.sagemakerB\024ParameterRangesProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPS\252\002\032Flyteidl.Plugins.Sagemaker\312\002\032Flyteidl\\Plugins\\Sagemaker\342\002&Flyteidl\\Plugins\\Sagemaker\\GPBMetadata\352\002\034Flyteidl::Plugins::Sagemaker'
   _PARAMETERRANGES_PARAMETERRANGEMAPENTRY._options = None
   _PARAMETERRANGES_PARAMETERRANGEMAPENTRY._serialized_options = b'8\001'
-  _HYPERPARAMETERSCALINGTYPE._serialized_start=81
-  _HYPERPARAMETERSCALINGTYPE._serialized_end=180
-  _HYPERPARAMETERSCALINGTYPE_VALUE._serialized_start=110
-  _HYPERPARAMETERSCALINGTYPE_VALUE._serialized_end=180
-  _CONTINUOUSPARAMETERRANGE._serialized_start=183
-  _CONTINUOUSPARAMETERRANGE._serialized_end=363
-  _INTEGERPARAMETERRANGE._serialized_start=366
-  _INTEGERPARAMETERRANGE._serialized_end=543
-  _CATEGORICALPARAMETERRANGE._serialized_start=545
-  _CATEGORICALPARAMETERRANGE._serialized_end=596
-  _PARAMETERRANGEONEOF._serialized_start=599
-  _PARAMETERRANGEONEOF._serialized_end=992
-  _PARAMETERRANGES._serialized_start=995
-  _PARAMETERRANGES._serialized_end=1247
-  _PARAMETERRANGES_PARAMETERRANGEMAPENTRY._serialized_start=1130
-  _PARAMETERRANGES_PARAMETERRANGEMAPENTRY._serialized_end=1247
+  _globals['_HYPERPARAMETERSCALINGTYPE']._serialized_start=81
+  _globals['_HYPERPARAMETERSCALINGTYPE']._serialized_end=180
+  _globals['_HYPERPARAMETERSCALINGTYPE_VALUE']._serialized_start=110
+  _globals['_HYPERPARAMETERSCALINGTYPE_VALUE']._serialized_end=180
+  _globals['_CONTINUOUSPARAMETERRANGE']._serialized_start=183
+  _globals['_CONTINUOUSPARAMETERRANGE']._serialized_end=363
+  _globals['_INTEGERPARAMETERRANGE']._serialized_start=366
+  _globals['_INTEGERPARAMETERRANGE']._serialized_end=543
+  _globals['_CATEGORICALPARAMETERRANGE']._serialized_start=545
+  _globals['_CATEGORICALPARAMETERRANGE']._serialized_end=596
+  _globals['_PARAMETERRANGEONEOF']._serialized_start=599
+  _globals['_PARAMETERRANGEONEOF']._serialized_end=992
+  _globals['_PARAMETERRANGES']._serialized_start=995
+  _globals['_PARAMETERRANGES']._serialized_end=1247
+  _globals['_PARAMETERRANGES_PARAMETERRANGEMAPENTRY']._serialized_start=1130
+  _globals['_PARAMETERRANGES_PARAMETERRANGEMAPENTRY']._serialized_end=1247
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,58 +2,62 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CategoricalParameterRange(_message.Message):
-    __slots__ = ["values"]
-    VALUES_FIELD_NUMBER: _ClassVar[int]
-    values: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
+class HyperparameterScalingType(_message.Message):
+    __slots__ = []
+    class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        AUTO: _ClassVar[HyperparameterScalingType.Value]
+        LINEAR: _ClassVar[HyperparameterScalingType.Value]
+        LOGARITHMIC: _ClassVar[HyperparameterScalingType.Value]
+        REVERSELOGARITHMIC: _ClassVar[HyperparameterScalingType.Value]
+    AUTO: HyperparameterScalingType.Value
+    LINEAR: HyperparameterScalingType.Value
+    LOGARITHMIC: HyperparameterScalingType.Value
+    REVERSELOGARITHMIC: HyperparameterScalingType.Value
+    def __init__(self) -> None: ...
 
 class ContinuousParameterRange(_message.Message):
     __slots__ = ["max_value", "min_value", "scaling_type"]
     MAX_VALUE_FIELD_NUMBER: _ClassVar[int]
     MIN_VALUE_FIELD_NUMBER: _ClassVar[int]
     SCALING_TYPE_FIELD_NUMBER: _ClassVar[int]
     max_value: float
     min_value: float
     scaling_type: HyperparameterScalingType.Value
     def __init__(self, max_value: _Optional[float] = ..., min_value: _Optional[float] = ..., scaling_type: _Optional[_Union[HyperparameterScalingType.Value, str]] = ...) -> None: ...
 
-class HyperparameterScalingType(_message.Message):
-    __slots__ = []
-    class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    AUTO: HyperparameterScalingType.Value
-    LINEAR: HyperparameterScalingType.Value
-    LOGARITHMIC: HyperparameterScalingType.Value
-    REVERSELOGARITHMIC: HyperparameterScalingType.Value
-    def __init__(self) -> None: ...
-
 class IntegerParameterRange(_message.Message):
     __slots__ = ["max_value", "min_value", "scaling_type"]
     MAX_VALUE_FIELD_NUMBER: _ClassVar[int]
     MIN_VALUE_FIELD_NUMBER: _ClassVar[int]
     SCALING_TYPE_FIELD_NUMBER: _ClassVar[int]
     max_value: int
     min_value: int
     scaling_type: HyperparameterScalingType.Value
     def __init__(self, max_value: _Optional[int] = ..., min_value: _Optional[int] = ..., scaling_type: _Optional[_Union[HyperparameterScalingType.Value, str]] = ...) -> None: ...
 
+class CategoricalParameterRange(_message.Message):
+    __slots__ = ["values"]
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class ParameterRangeOneOf(_message.Message):
-    __slots__ = ["categorical_parameter_range", "continuous_parameter_range", "integer_parameter_range"]
-    CATEGORICAL_PARAMETER_RANGE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["continuous_parameter_range", "integer_parameter_range", "categorical_parameter_range"]
     CONTINUOUS_PARAMETER_RANGE_FIELD_NUMBER: _ClassVar[int]
     INTEGER_PARAMETER_RANGE_FIELD_NUMBER: _ClassVar[int]
-    categorical_parameter_range: CategoricalParameterRange
+    CATEGORICAL_PARAMETER_RANGE_FIELD_NUMBER: _ClassVar[int]
     continuous_parameter_range: ContinuousParameterRange
     integer_parameter_range: IntegerParameterRange
+    categorical_parameter_range: CategoricalParameterRange
     def __init__(self, continuous_parameter_range: _Optional[_Union[ContinuousParameterRange, _Mapping]] = ..., integer_parameter_range: _Optional[_Union[IntegerParameterRange, _Mapping]] = ..., categorical_parameter_range: _Optional[_Union[CategoricalParameterRange, _Mapping]] = ...) -> None: ...
 
 class ParameterRanges(_message.Message):
     __slots__ = ["parameter_range_map"]
     class ParameterRangeMapEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,38 +12,39 @@
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-flyteidl/plugins/sagemaker/training_job.proto\x12\x1a\x66lyteidl.plugins.sagemaker\x1a\x1egoogle/protobuf/duration.proto\"(\n\tInputMode\"\x1b\n\x05Value\x12\x08\n\x04\x46ILE\x10\x00\x12\x08\n\x04PIPE\x10\x01\"1\n\rAlgorithmName\" \n\x05Value\x12\n\n\x06\x43USTOM\x10\x00\x12\x0b\n\x07XGBOOST\x10\x01\")\n\x10InputContentType\"\x15\n\x05Value\x12\x0c\n\x08TEXT_CSV\x10\x00\"<\n\x10MetricDefinition\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05regex\x18\x02 \x01(\tR\x05regex\"\xa8\x03\n\x16\x41lgorithmSpecification\x12J\n\ninput_mode\x18\x01 \x01(\x0e\x32+.flyteidl.plugins.sagemaker.InputMode.ValueR\tinputMode\x12V\n\x0e\x61lgorithm_name\x18\x02 \x01(\x0e\x32/.flyteidl.plugins.sagemaker.AlgorithmName.ValueR\ralgorithmName\x12+\n\x11\x61lgorithm_version\x18\x03 \x01(\tR\x10\x61lgorithmVersion\x12[\n\x12metric_definitions\x18\x04 \x03(\x0b\x32,.flyteidl.plugins.sagemaker.MetricDefinitionR\x11metricDefinitions\x12`\n\x12input_content_type\x18\x05 \x01(\x0e\x32\x32.flyteidl.plugins.sagemaker.InputContentType.ValueR\x10inputContentType\"8\n\x13\x44istributedProtocol\"!\n\x05Value\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03MPI\x10\x01\"\xfc\x01\n\x19TrainingJobResourceConfig\x12%\n\x0einstance_count\x18\x01 \x01(\x03R\rinstanceCount\x12#\n\rinstance_type\x18\x02 \x01(\tR\x0cinstanceType\x12)\n\x11volume_size_in_gb\x18\x03 \x01(\x03R\x0evolumeSizeInGb\x12h\n\x14\x64istributed_protocol\x18\x04 \x01(\x0e\x32\x35.flyteidl.plugins.sagemaker.DistributedProtocol.ValueR\x13\x64istributedProtocol\"\xf2\x01\n\x0bTrainingJob\x12k\n\x17\x61lgorithm_specification\x18\x01 \x01(\x0b\x32\x32.flyteidl.plugins.sagemaker.AlgorithmSpecificationR\x16\x61lgorithmSpecification\x12v\n\x1ctraining_job_resource_config\x18\x02 \x01(\x0b\x32\x35.flyteidl.plugins.sagemaker.TrainingJobResourceConfigR\x19trainingJobResourceConfigB\xf5\x01\n\x1e\x63om.flyteidl.plugins.sagemakerB\x10TrainingJobProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PS\xaa\x02\x1a\x46lyteidl.Plugins.Sagemaker\xca\x02\x1a\x46lyteidl\\Plugins\\Sagemaker\xe2\x02&Flyteidl\\Plugins\\Sagemaker\\GPBMetadata\xea\x02\x1c\x46lyteidl::Plugins::Sagemakerb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.sagemaker.training_job_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.sagemaker.training_job_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.flyteidl.plugins.sagemakerB\020TrainingJobProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPS\252\002\032Flyteidl.Plugins.Sagemaker\312\002\032Flyteidl\\Plugins\\Sagemaker\342\002&Flyteidl\\Plugins\\Sagemaker\\GPBMetadata\352\002\034Flyteidl::Plugins::Sagemaker'
-  _INPUTMODE._serialized_start=109
-  _INPUTMODE._serialized_end=149
-  _INPUTMODE_VALUE._serialized_start=122
-  _INPUTMODE_VALUE._serialized_end=149
-  _ALGORITHMNAME._serialized_start=151
-  _ALGORITHMNAME._serialized_end=200
-  _ALGORITHMNAME_VALUE._serialized_start=168
-  _ALGORITHMNAME_VALUE._serialized_end=200
-  _INPUTCONTENTTYPE._serialized_start=202
-  _INPUTCONTENTTYPE._serialized_end=243
-  _INPUTCONTENTTYPE_VALUE._serialized_start=222
-  _INPUTCONTENTTYPE_VALUE._serialized_end=243
-  _METRICDEFINITION._serialized_start=245
-  _METRICDEFINITION._serialized_end=305
-  _ALGORITHMSPECIFICATION._serialized_start=308
-  _ALGORITHMSPECIFICATION._serialized_end=732
-  _DISTRIBUTEDPROTOCOL._serialized_start=734
-  _DISTRIBUTEDPROTOCOL._serialized_end=790
-  _DISTRIBUTEDPROTOCOL_VALUE._serialized_start=757
-  _DISTRIBUTEDPROTOCOL_VALUE._serialized_end=790
-  _TRAININGJOBRESOURCECONFIG._serialized_start=793
-  _TRAININGJOBRESOURCECONFIG._serialized_end=1045
-  _TRAININGJOB._serialized_start=1048
-  _TRAININGJOB._serialized_end=1290
+  _globals['_INPUTMODE']._serialized_start=109
+  _globals['_INPUTMODE']._serialized_end=149
+  _globals['_INPUTMODE_VALUE']._serialized_start=122
+  _globals['_INPUTMODE_VALUE']._serialized_end=149
+  _globals['_ALGORITHMNAME']._serialized_start=151
+  _globals['_ALGORITHMNAME']._serialized_end=200
+  _globals['_ALGORITHMNAME_VALUE']._serialized_start=168
+  _globals['_ALGORITHMNAME_VALUE']._serialized_end=200
+  _globals['_INPUTCONTENTTYPE']._serialized_start=202
+  _globals['_INPUTCONTENTTYPE']._serialized_end=243
+  _globals['_INPUTCONTENTTYPE_VALUE']._serialized_start=222
+  _globals['_INPUTCONTENTTYPE_VALUE']._serialized_end=243
+  _globals['_METRICDEFINITION']._serialized_start=245
+  _globals['_METRICDEFINITION']._serialized_end=305
+  _globals['_ALGORITHMSPECIFICATION']._serialized_start=308
+  _globals['_ALGORITHMSPECIFICATION']._serialized_end=732
+  _globals['_DISTRIBUTEDPROTOCOL']._serialized_start=734
+  _globals['_DISTRIBUTEDPROTOCOL']._serialized_end=790
+  _globals['_DISTRIBUTEDPROTOCOL_VALUE']._serialized_start=757
+  _globals['_DISTRIBUTEDPROTOCOL_VALUE']._serialized_end=790
+  _globals['_TRAININGJOBRESOURCECONFIG']._serialized_start=793
+  _globals['_TRAININGJOBRESOURCECONFIG']._serialized_end=1045
+  _globals['_TRAININGJOB']._serialized_start=1048
+  _globals['_TRAININGJOB']._serialized_end=1290
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,79 +3,86 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class AlgorithmName(_message.Message):
+class InputMode(_message.Message):
     __slots__ = []
     class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    CUSTOM: AlgorithmName.Value
-    XGBOOST: AlgorithmName.Value
+        FILE: _ClassVar[InputMode.Value]
+        PIPE: _ClassVar[InputMode.Value]
+    FILE: InputMode.Value
+    PIPE: InputMode.Value
     def __init__(self) -> None: ...
 
-class AlgorithmSpecification(_message.Message):
-    __slots__ = ["algorithm_name", "algorithm_version", "input_content_type", "input_mode", "metric_definitions"]
-    ALGORITHM_NAME_FIELD_NUMBER: _ClassVar[int]
-    ALGORITHM_VERSION_FIELD_NUMBER: _ClassVar[int]
-    INPUT_CONTENT_TYPE_FIELD_NUMBER: _ClassVar[int]
-    INPUT_MODE_FIELD_NUMBER: _ClassVar[int]
-    METRIC_DEFINITIONS_FIELD_NUMBER: _ClassVar[int]
-    algorithm_name: AlgorithmName.Value
-    algorithm_version: str
-    input_content_type: InputContentType.Value
-    input_mode: InputMode.Value
-    metric_definitions: _containers.RepeatedCompositeFieldContainer[MetricDefinition]
-    def __init__(self, input_mode: _Optional[_Union[InputMode.Value, str]] = ..., algorithm_name: _Optional[_Union[AlgorithmName.Value, str]] = ..., algorithm_version: _Optional[str] = ..., metric_definitions: _Optional[_Iterable[_Union[MetricDefinition, _Mapping]]] = ..., input_content_type: _Optional[_Union[InputContentType.Value, str]] = ...) -> None: ...
-
-class DistributedProtocol(_message.Message):
+class AlgorithmName(_message.Message):
     __slots__ = []
     class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    MPI: DistributedProtocol.Value
-    UNSPECIFIED: DistributedProtocol.Value
+        CUSTOM: _ClassVar[AlgorithmName.Value]
+        XGBOOST: _ClassVar[AlgorithmName.Value]
+    CUSTOM: AlgorithmName.Value
+    XGBOOST: AlgorithmName.Value
     def __init__(self) -> None: ...
 
 class InputContentType(_message.Message):
     __slots__ = []
     class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
+        TEXT_CSV: _ClassVar[InputContentType.Value]
     TEXT_CSV: InputContentType.Value
     def __init__(self) -> None: ...
 
-class InputMode(_message.Message):
-    __slots__ = []
-    class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    FILE: InputMode.Value
-    PIPE: InputMode.Value
-    def __init__(self) -> None: ...
-
 class MetricDefinition(_message.Message):
     __slots__ = ["name", "regex"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     REGEX_FIELD_NUMBER: _ClassVar[int]
     name: str
     regex: str
     def __init__(self, name: _Optional[str] = ..., regex: _Optional[str] = ...) -> None: ...
 
-class TrainingJob(_message.Message):
-    __slots__ = ["algorithm_specification", "training_job_resource_config"]
-    ALGORITHM_SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
-    TRAINING_JOB_RESOURCE_CONFIG_FIELD_NUMBER: _ClassVar[int]
-    algorithm_specification: AlgorithmSpecification
-    training_job_resource_config: TrainingJobResourceConfig
-    def __init__(self, algorithm_specification: _Optional[_Union[AlgorithmSpecification, _Mapping]] = ..., training_job_resource_config: _Optional[_Union[TrainingJobResourceConfig, _Mapping]] = ...) -> None: ...
+class AlgorithmSpecification(_message.Message):
+    __slots__ = ["input_mode", "algorithm_name", "algorithm_version", "metric_definitions", "input_content_type"]
+    INPUT_MODE_FIELD_NUMBER: _ClassVar[int]
+    ALGORITHM_NAME_FIELD_NUMBER: _ClassVar[int]
+    ALGORITHM_VERSION_FIELD_NUMBER: _ClassVar[int]
+    METRIC_DEFINITIONS_FIELD_NUMBER: _ClassVar[int]
+    INPUT_CONTENT_TYPE_FIELD_NUMBER: _ClassVar[int]
+    input_mode: InputMode.Value
+    algorithm_name: AlgorithmName.Value
+    algorithm_version: str
+    metric_definitions: _containers.RepeatedCompositeFieldContainer[MetricDefinition]
+    input_content_type: InputContentType.Value
+    def __init__(self, input_mode: _Optional[_Union[InputMode.Value, str]] = ..., algorithm_name: _Optional[_Union[AlgorithmName.Value, str]] = ..., algorithm_version: _Optional[str] = ..., metric_definitions: _Optional[_Iterable[_Union[MetricDefinition, _Mapping]]] = ..., input_content_type: _Optional[_Union[InputContentType.Value, str]] = ...) -> None: ...
+
+class DistributedProtocol(_message.Message):
+    __slots__ = []
+    class Value(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+        UNSPECIFIED: _ClassVar[DistributedProtocol.Value]
+        MPI: _ClassVar[DistributedProtocol.Value]
+    UNSPECIFIED: DistributedProtocol.Value
+    MPI: DistributedProtocol.Value
+    def __init__(self) -> None: ...
 
 class TrainingJobResourceConfig(_message.Message):
-    __slots__ = ["distributed_protocol", "instance_count", "instance_type", "volume_size_in_gb"]
-    DISTRIBUTED_PROTOCOL_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["instance_count", "instance_type", "volume_size_in_gb", "distributed_protocol"]
     INSTANCE_COUNT_FIELD_NUMBER: _ClassVar[int]
     INSTANCE_TYPE_FIELD_NUMBER: _ClassVar[int]
     VOLUME_SIZE_IN_GB_FIELD_NUMBER: _ClassVar[int]
-    distributed_protocol: DistributedProtocol.Value
+    DISTRIBUTED_PROTOCOL_FIELD_NUMBER: _ClassVar[int]
     instance_count: int
     instance_type: str
     volume_size_in_gb: int
+    distributed_protocol: DistributedProtocol.Value
     def __init__(self, instance_count: _Optional[int] = ..., instance_type: _Optional[str] = ..., volume_size_in_gb: _Optional[int] = ..., distributed_protocol: _Optional[_Union[DistributedProtocol.Value, str]] = ...) -> None: ...
+
+class TrainingJob(_message.Message):
+    __slots__ = ["algorithm_specification", "training_job_resource_config"]
+    ALGORITHM_SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
+    TRAINING_JOB_RESOURCE_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    algorithm_specification: AlgorithmSpecification
+    training_job_resource_config: TrainingJobResourceConfig
+    def __init__(self, algorithm_specification: _Optional[_Union[AlgorithmSpecification, _Mapping]] = ..., training_job_resource_config: _Optional[_Union[TrainingJobResourceConfig, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/spark_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/spark_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,52 @@
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class SparkApplication(_message.Message):
     __slots__ = []
     class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    JAVA: SparkApplication.Type
+        PYTHON: _ClassVar[SparkApplication.Type]
+        JAVA: _ClassVar[SparkApplication.Type]
+        SCALA: _ClassVar[SparkApplication.Type]
+        R: _ClassVar[SparkApplication.Type]
     PYTHON: SparkApplication.Type
-    R: SparkApplication.Type
+    JAVA: SparkApplication.Type
     SCALA: SparkApplication.Type
+    R: SparkApplication.Type
     def __init__(self) -> None: ...
 
 class SparkJob(_message.Message):
-    __slots__ = ["applicationType", "databricksConf", "databricksInstance", "databricksToken", "executorPath", "hadoopConf", "mainApplicationFile", "mainClass", "sparkConf"]
-    class HadoopConfEntry(_message.Message):
+    __slots__ = ["applicationType", "mainApplicationFile", "mainClass", "sparkConf", "hadoopConf", "executorPath", "databricksConf", "databricksToken", "databricksInstance"]
+    class SparkConfEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    class SparkConfEntry(_message.Message):
+    class HadoopConfEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     APPLICATIONTYPE_FIELD_NUMBER: _ClassVar[int]
-    DATABRICKSCONF_FIELD_NUMBER: _ClassVar[int]
-    DATABRICKSINSTANCE_FIELD_NUMBER: _ClassVar[int]
-    DATABRICKSTOKEN_FIELD_NUMBER: _ClassVar[int]
-    EXECUTORPATH_FIELD_NUMBER: _ClassVar[int]
-    HADOOPCONF_FIELD_NUMBER: _ClassVar[int]
     MAINAPPLICATIONFILE_FIELD_NUMBER: _ClassVar[int]
     MAINCLASS_FIELD_NUMBER: _ClassVar[int]
     SPARKCONF_FIELD_NUMBER: _ClassVar[int]
+    HADOOPCONF_FIELD_NUMBER: _ClassVar[int]
+    EXECUTORPATH_FIELD_NUMBER: _ClassVar[int]
+    DATABRICKSCONF_FIELD_NUMBER: _ClassVar[int]
+    DATABRICKSTOKEN_FIELD_NUMBER: _ClassVar[int]
+    DATABRICKSINSTANCE_FIELD_NUMBER: _ClassVar[int]
     applicationType: SparkApplication.Type
-    databricksConf: _struct_pb2.Struct
-    databricksInstance: str
-    databricksToken: str
-    executorPath: str
-    hadoopConf: _containers.ScalarMap[str, str]
     mainApplicationFile: str
     mainClass: str
     sparkConf: _containers.ScalarMap[str, str]
+    hadoopConf: _containers.ScalarMap[str, str]
+    executorPath: str
+    databricksConf: _struct_pb2.Struct
+    databricksToken: str
+    databricksInstance: str
     def __init__(self, applicationType: _Optional[_Union[SparkApplication.Type, str]] = ..., mainApplicationFile: _Optional[str] = ..., mainClass: _Optional[str] = ..., sparkConf: _Optional[_Mapping[str, str]] = ..., hadoopConf: _Optional[_Mapping[str, str]] = ..., executorPath: _Optional[str] = ..., databricksConf: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., databricksToken: _Optional[str] = ..., databricksInstance: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/tensorflow_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/tensorflow_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DistributedTensorflowTrainingTask(_message.Message):
-    __slots__ = ["chief_replicas", "ps_replicas", "workers"]
-    CHIEF_REPLICAS_FIELD_NUMBER: _ClassVar[int]
-    PS_REPLICAS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["workers", "ps_replicas", "chief_replicas"]
     WORKERS_FIELD_NUMBER: _ClassVar[int]
-    chief_replicas: int
-    ps_replicas: int
+    PS_REPLICAS_FIELD_NUMBER: _ClassVar[int]
+    CHIEF_REPLICAS_FIELD_NUMBER: _ClassVar[int]
     workers: int
+    ps_replicas: int
+    chief_replicas: int
     def __init__(self, workers: _Optional[int] = ..., ps_replicas: _Optional[int] = ..., chief_replicas: _Optional[int] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/waitable_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/pytorch_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/plugins/waitable.proto
+# source: flyteidl/plugins/pytorch.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from flyteidl.core import execution_pb2 as flyteidl_dot_core_dot_execution__pb2
-from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66lyteidl/plugins/waitable.proto\x12\x10\x66lyteidl.plugins\x1a\x1d\x66lyteidl/core/execution.proto\x1a\x1e\x66lyteidl/core/identifier.proto\"\xb3\x01\n\x08Waitable\x12H\n\nwf_exec_id\x18\x01 \x01(\x0b\x32*.flyteidl.core.WorkflowExecutionIdentifierR\x08wfExecId\x12<\n\x05phase\x18\x02 \x01(\x0e\x32&.flyteidl.core.WorkflowExecution.PhaseR\x05phase\x12\x1f\n\x0bworkflow_id\x18\x03 \x01(\tR\nworkflowIdB\xbf\x01\n\x14\x63om.flyteidl.pluginsB\rWaitableProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x66lyteidl/plugins/pytorch.proto\x12\x10\x66lyteidl.plugins\"\xc1\x01\n\rElasticConfig\x12!\n\x0crdzv_backend\x18\x01 \x01(\tR\x0brdzvBackend\x12!\n\x0cmin_replicas\x18\x02 \x01(\x05R\x0bminReplicas\x12!\n\x0cmax_replicas\x18\x03 \x01(\x05R\x0bmaxReplicas\x12$\n\x0enproc_per_node\x18\x04 \x01(\x05R\x0cnprocPerNode\x12!\n\x0cmax_restarts\x18\x05 \x01(\x05R\x0bmaxRestarts\"\x82\x01\n\x1e\x44istributedPyTorchTrainingTask\x12\x18\n\x07workers\x18\x01 \x01(\x05R\x07workers\x12\x46\n\x0e\x65lastic_config\x18\x02 \x01(\x0b\x32\x1f.flyteidl.plugins.ElasticConfigR\relasticConfigB\xbe\x01\n\x14\x63om.flyteidl.pluginsB\x0cPytorchProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\xa2\x02\x03\x46PX\xaa\x02\x10\x46lyteidl.Plugins\xca\x02\x10\x46lyteidl\\Plugins\xe2\x02\x1c\x46lyteidl\\Plugins\\GPBMetadata\xea\x02\x11\x46lyteidl::Pluginsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.waitable_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.plugins.pytorch_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\rWaitableProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
-  _WAITABLE._serialized_start=117
-  _WAITABLE._serialized_end=296
+  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.pluginsB\014PytorchProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/plugins\242\002\003FPX\252\002\020Flyteidl.Plugins\312\002\020Flyteidl\\Plugins\342\002\034Flyteidl\\Plugins\\GPBMetadata\352\002\021Flyteidl::Plugins'
+  _globals['_ELASTICCONFIG']._serialized_start=53
+  _globals['_ELASTICCONFIG']._serialized_end=246
+  _globals['_DISTRIBUTEDPYTORCHTRAININGTASK']._serialized_start=249
+  _globals['_DISTRIBUTEDPYTORCHTRAININGTASK']._serialized_end=379
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/plugins/waitable_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/plugins/waitable_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Waitable(_message.Message):
-    __slots__ = ["phase", "wf_exec_id", "workflow_id"]
-    PHASE_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["wf_exec_id", "phase", "workflow_id"]
     WF_EXEC_ID_FIELD_NUMBER: _ClassVar[int]
+    PHASE_FIELD_NUMBER: _ClassVar[int]
     WORKFLOW_ID_FIELD_NUMBER: _ClassVar[int]
-    phase: _execution_pb2.WorkflowExecution.Phase
     wf_exec_id: _identifier_pb2.WorkflowExecutionIdentifier
+    phase: _execution_pb2.WorkflowExecution.Phase
     workflow_id: str
     def __init__(self, wf_exec_id: _Optional[_Union[_identifier_pb2.WorkflowExecutionIdentifier, _Mapping]] = ..., phase: _Optional[_Union[_execution_pb2.WorkflowExecution.Phase, str]] = ..., workflow_id: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/admin_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/admin_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 from flyteidl.admin import execution_pb2 as flyteidl_dot_admin_dot_execution__pb2
 from flyteidl.admin import matchable_resource_pb2 as flyteidl_dot_admin_dot_matchable__resource__pb2
 from flyteidl.admin import node_execution_pb2 as flyteidl_dot_admin_dot_node__execution__pb2
 from flyteidl.admin import task_execution_pb2 as flyteidl_dot_admin_dot_task__execution__pb2
 from flyteidl.admin import version_pb2 as flyteidl_dot_admin_dot_version__pb2
 from flyteidl.admin import common_pb2 as flyteidl_dot_admin_dot_common__pb2
 from flyteidl.admin import description_entity_pb2 as flyteidl_dot_admin_dot_description__entity__pb2
-from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/service/admin.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1c\x66lyteidl/admin/project.proto\x1a.flyteidl/admin/project_domain_attributes.proto\x1a\'flyteidl/admin/project_attributes.proto\x1a\x19\x66lyteidl/admin/task.proto\x1a\x1d\x66lyteidl/admin/workflow.proto\x1a(flyteidl/admin/workflow_attributes.proto\x1a flyteidl/admin/launch_plan.proto\x1a\x1a\x66lyteidl/admin/event.proto\x1a\x1e\x66lyteidl/admin/execution.proto\x1a\'flyteidl/admin/matchable_resource.proto\x1a#flyteidl/admin/node_execution.proto\x1a#flyteidl/admin/task_execution.proto\x1a\x1c\x66lyteidl/admin/version.proto\x1a\x1b\x66lyteidl/admin/common.proto\x1a\'flyteidl/admin/description_entity.proto\x1a\x1e\x66lyteidl/core/identifier.proto2\xbcL\n\x0c\x41\x64minService\x12m\n\nCreateTask\x12!.flyteidl.admin.TaskCreateRequest\x1a\".flyteidl.admin.TaskCreateResponse\"\x18\x82\xd3\xe4\x93\x02\x12:\x01*\"\r/api/v1/tasks\x12\x88\x01\n\x07GetTask\x12 .flyteidl.admin.ObjectGetRequest\x1a\x14.flyteidl.admin.Task\"E\x82\xd3\xe4\x93\x02?\x12=/api/v1/tasks/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x97\x01\n\x0bListTaskIds\x12\x30.flyteidl.admin.NamedEntityIdentifierListRequest\x1a).flyteidl.admin.NamedEntityIdentifierList\"+\x82\xd3\xe4\x93\x02%\x12#/api/v1/task_ids/{project}/{domain}\x12\xae\x01\n\tListTasks\x12#.flyteidl.admin.ResourceListRequest\x1a\x18.flyteidl.admin.TaskList\"b\x82\xd3\xe4\x93\x02\\Z(\x12&/api/v1/tasks/{id.project}/{id.domain}\x12\x30/api/v1/tasks/{id.project}/{id.domain}/{id.name}\x12}\n\x0e\x43reateWorkflow\x12%.flyteidl.admin.WorkflowCreateRequest\x1a&.flyteidl.admin.WorkflowCreateResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/api/v1/workflows\x12\x94\x01\n\x0bGetWorkflow\x12 .flyteidl.admin.ObjectGetRequest\x1a\x18.flyteidl.admin.Workflow\"I\x82\xd3\xe4\x93\x02\x43\x12\x41/api/v1/workflows/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x9f\x01\n\x0fListWorkflowIds\x12\x30.flyteidl.admin.NamedEntityIdentifierListRequest\x1a).flyteidl.admin.NamedEntityIdentifierList\"/\x82\xd3\xe4\x93\x02)\x12\'/api/v1/workflow_ids/{project}/{domain}\x12\xbe\x01\n\rListWorkflows\x12#.flyteidl.admin.ResourceListRequest\x1a\x1c.flyteidl.admin.WorkflowList\"j\x82\xd3\xe4\x93\x02\x64Z,\x12*/api/v1/workflows/{id.project}/{id.domain}\x12\x34/api/v1/workflows/{id.project}/{id.domain}/{id.name}\x12\x86\x01\n\x10\x43reateLaunchPlan\x12\'.flyteidl.admin.LaunchPlanCreateRequest\x1a(.flyteidl.admin.LaunchPlanCreateResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/api/v1/launch_plans\x12\x9b\x01\n\rGetLaunchPlan\x12 .flyteidl.admin.ObjectGetRequest\x1a\x1a.flyteidl.admin.LaunchPlan\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/api/v1/launch_plans/{id.project}/{id.domain}/{id.name}/{id.version}\x12\xa2\x01\n\x13GetActiveLaunchPlan\x12\'.flyteidl.admin.ActiveLaunchPlanRequest\x1a\x1a.flyteidl.admin.LaunchPlan\"F\x82\xd3\xe4\x93\x02@\x12>/api/v1/active_launch_plans/{id.project}/{id.domain}/{id.name}\x12\x9c\x01\n\x15ListActiveLaunchPlans\x12+.flyteidl.admin.ActiveLaunchPlanListRequest\x1a\x1e.flyteidl.admin.LaunchPlanList\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/active_launch_plans/{project}/{domain}\x12\xa4\x01\n\x11ListLaunchPlanIds\x12\x30.flyteidl.admin.NamedEntityIdentifierListRequest\x1a).flyteidl.admin.NamedEntityIdentifierList\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/launch_plan_ids/{project}/{domain}\x12\xc8\x01\n\x0fListLaunchPlans\x12#.flyteidl.admin.ResourceListRequest\x1a\x1e.flyteidl.admin.LaunchPlanList\"p\x82\xd3\xe4\x93\x02jZ/\x12-/api/v1/launch_plans/{id.project}/{id.domain}\x12\x37/api/v1/launch_plans/{id.project}/{id.domain}/{id.name}\x12\xb6\x01\n\x10UpdateLaunchPlan\x12\'.flyteidl.admin.LaunchPlanUpdateRequest\x1a(.flyteidl.admin.LaunchPlanUpdateResponse\"O\x82\xd3\xe4\x93\x02I:\x01*\x1a\x44/api/v1/launch_plans/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x81\x01\n\x0f\x43reateExecution\x12&.flyteidl.admin.ExecutionCreateRequest\x1a\'.flyteidl.admin.ExecutionCreateResponse\"\x1d\x82\xd3\xe4\x93\x02\x17:\x01*\"\x12/api/v1/executions\x12\x8e\x01\n\x11RelaunchExecution\x12(.flyteidl.admin.ExecutionRelaunchRequest\x1a\'.flyteidl.admin.ExecutionCreateResponse\"&\x82\xd3\xe4\x93\x02 :\x01*\"\x1b/api/v1/executions/relaunch\x12\x8b\x01\n\x10RecoverExecution\x12\'.flyteidl.admin.ExecutionRecoverRequest\x1a\'.flyteidl.admin.ExecutionCreateResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/api/v1/executions/recover\x12\x95\x01\n\x0cGetExecution\x12+.flyteidl.admin.WorkflowExecutionGetRequest\x1a\x19.flyteidl.admin.Execution\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/executions/{id.project}/{id.domain}/{id.name}\x12\xa4\x01\n\x0fUpdateExecution\x12&.flyteidl.admin.ExecutionUpdateRequest\x1a\'.flyteidl.admin.ExecutionUpdateResponse\"@\x82\xd3\xe4\x93\x02::\x01*\x1a\x35/api/v1/executions/{id.project}/{id.domain}/{id.name}\x12\xb9\x01\n\x10GetExecutionData\x12/.flyteidl.admin.WorkflowExecutionGetDataRequest\x1a\x30.flyteidl.admin.WorkflowExecutionGetDataResponse\"B\x82\xd3\xe4\x93\x02<\x12:/api/v1/data/executions/{id.project}/{id.domain}/{id.name}\x12\x89\x01\n\x0eListExecutions\x12#.flyteidl.admin.ResourceListRequest\x1a\x1d.flyteidl.admin.ExecutionList\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/executions/{id.project}/{id.domain}\x12\xad\x01\n\x12TerminateExecution\x12).flyteidl.admin.ExecutionTerminateRequest\x1a*.flyteidl.admin.ExecutionTerminateResponse\"@\x82\xd3\xe4\x93\x02::\x01**5/api/v1/executions/{id.project}/{id.domain}/{id.name}\x12\xd2\x01\n\x10GetNodeExecution\x12\'.flyteidl.admin.NodeExecutionGetRequest\x1a\x1d.flyteidl.admin.NodeExecution\"v\x82\xd3\xe4\x93\x02p\x12n/api/v1/node_executions/{id.execution_id.project}/{id.execution_id.domain}/{id.execution_id.name}/{id.node_id}\x12\xde\x01\n\x12ListNodeExecutions\x12(.flyteidl.admin.NodeExecutionListRequest\x1a!.flyteidl.admin.NodeExecutionList\"{\x82\xd3\xe4\x93\x02u\x12s/api/v1/node_executions/{workflow_execution_id.project}/{workflow_execution_id.domain}/{workflow_execution_id.name}\x12\xa5\x04\n\x19ListNodeExecutionsForTask\x12/.flyteidl.admin.NodeExecutionForTaskListRequest\x1a!.flyteidl.admin.NodeExecutionList\"\xb3\x03\x82\xd3\xe4\x93\x02\xac\x03\x12\xa9\x03/api/v1/children/task_executions/{task_execution_id.node_execution_id.execution_id.project}/{task_execution_id.node_execution_id.execution_id.domain}/{task_execution_id.node_execution_id.execution_id.name}/{task_execution_id.node_execution_id.node_id}/{task_execution_id.task_id.project}/{task_execution_id.task_id.domain}/{task_execution_id.task_id.name}/{task_execution_id.task_id.version}/{task_execution_id.retry_attempt}\x12\xee\x01\n\x14GetNodeExecutionData\x12+.flyteidl.admin.NodeExecutionGetDataRequest\x1a,.flyteidl.admin.NodeExecutionGetDataResponse\"{\x82\xd3\xe4\x93\x02u\x12s/api/v1/data/node_executions/{id.execution_id.project}/{id.execution_id.domain}/{id.execution_id.name}/{id.node_id}\x12\x7f\n\x0fRegisterProject\x12&.flyteidl.admin.ProjectRegisterRequest\x1a\'.flyteidl.admin.ProjectRegisterResponse\"\x1b\x82\xd3\xe4\x93\x02\x15:\x01*\"\x10/api/v1/projects\x12q\n\rUpdateProject\x12\x17.flyteidl.admin.Project\x1a%.flyteidl.admin.ProjectUpdateResponse\" \x82\xd3\xe4\x93\x02\x1a:\x01*\x1a\x15/api/v1/projects/{id}\x12\x66\n\x0cListProjects\x12\".flyteidl.admin.ProjectListRequest\x1a\x18.flyteidl.admin.Projects\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/api/v1/projects\x12\x99\x01\n\x13\x43reateWorkflowEvent\x12-.flyteidl.admin.WorkflowExecutionEventRequest\x1a..flyteidl.admin.WorkflowExecutionEventResponse\"#\x82\xd3\xe4\x93\x02\x1d:\x01*\"\x18/api/v1/events/workflows\x12\x89\x01\n\x0f\x43reateNodeEvent\x12).flyteidl.admin.NodeExecutionEventRequest\x1a*.flyteidl.admin.NodeExecutionEventResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/api/v1/events/nodes\x12\x89\x01\n\x0f\x43reateTaskEvent\x12).flyteidl.admin.TaskExecutionEventRequest\x1a*.flyteidl.admin.TaskExecutionEventResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/api/v1/events/tasks\x12\x80\x03\n\x10GetTaskExecution\x12\'.flyteidl.admin.TaskExecutionGetRequest\x1a\x1d.flyteidl.admin.TaskExecution\"\xa3\x02\x82\xd3\xe4\x93\x02\x9c\x02\x12\x99\x02/api/v1/task_executions/{id.node_execution_id.execution_id.project}/{id.node_execution_id.execution_id.domain}/{id.node_execution_id.execution_id.name}/{id.node_execution_id.node_id}/{id.task_id.project}/{id.task_id.domain}/{id.task_id.name}/{id.task_id.version}/{id.retry_attempt}\x12\x98\x02\n\x12ListTaskExecutions\x12(.flyteidl.admin.TaskExecutionListRequest\x1a!.flyteidl.admin.TaskExecutionList\"\xb4\x01\x82\xd3\xe4\x93\x02\xad\x01\x12\xaa\x01/api/v1/task_executions/{node_execution_id.execution_id.project}/{node_execution_id.execution_id.domain}/{node_execution_id.execution_id.name}/{node_execution_id.node_id}\x12\x9c\x03\n\x14GetTaskExecutionData\x12+.flyteidl.admin.TaskExecutionGetDataRequest\x1a,.flyteidl.admin.TaskExecutionGetDataResponse\"\xa8\x02\x82\xd3\xe4\x93\x02\xa1\x02\x12\x9e\x02/api/v1/data/task_executions/{id.node_execution_id.execution_id.project}/{id.node_execution_id.execution_id.domain}/{id.node_execution_id.execution_id.name}/{id.node_execution_id.node_id}/{id.task_id.project}/{id.task_id.domain}/{id.task_id.name}/{id.task_id.version}/{id.retry_attempt}\x12\xe3\x01\n\x1dUpdateProjectDomainAttributes\x12\x34.flyteidl.admin.ProjectDomainAttributesUpdateRequest\x1a\x35.flyteidl.admin.ProjectDomainAttributesUpdateResponse\"U\x82\xd3\xe4\x93\x02O:\x01*\x1aJ/api/v1/project_domain_attributes/{attributes.project}/{attributes.domain}\x12\xc1\x01\n\x1aGetProjectDomainAttributes\x12\x31.flyteidl.admin.ProjectDomainAttributesGetRequest\x1a\x32.flyteidl.admin.ProjectDomainAttributesGetResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/api/v1/project_domain_attributes/{project}/{domain}\x12\xcd\x01\n\x1d\x44\x65leteProjectDomainAttributes\x12\x34.flyteidl.admin.ProjectDomainAttributesDeleteRequest\x1a\x35.flyteidl.admin.ProjectDomainAttributesDeleteResponse\"?\x82\xd3\xe4\x93\x02\x39:\x01**4/api/v1/project_domain_attributes/{project}/{domain}\x12\xb6\x01\n\x17UpdateProjectAttributes\x12..flyteidl.admin.ProjectAttributesUpdateRequest\x1a/.flyteidl.admin.ProjectAttributesUpdateResponse\":\x82\xd3\xe4\x93\x02\x34:\x01*\x1a//api/v1/project_attributes/{attributes.project}\x12\x9f\x01\n\x14GetProjectAttributes\x12+.flyteidl.admin.ProjectAttributesGetRequest\x1a,.flyteidl.admin.ProjectAttributesGetResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/project_attributes/{project}\x12\xab\x01\n\x17\x44\x65leteProjectAttributes\x12..flyteidl.admin.ProjectAttributesDeleteRequest\x1a/.flyteidl.admin.ProjectAttributesDeleteResponse\"/\x82\xd3\xe4\x93\x02):\x01**$/api/v1/project_attributes/{project}\x12\xe4\x01\n\x18UpdateWorkflowAttributes\x12/.flyteidl.admin.WorkflowAttributesUpdateRequest\x1a\x30.flyteidl.admin.WorkflowAttributesUpdateResponse\"e\x82\xd3\xe4\x93\x02_:\x01*\x1aZ/api/v1/workflow_attributes/{attributes.project}/{attributes.domain}/{attributes.workflow}\x12\xb7\x01\n\x15GetWorkflowAttributes\x12,.flyteidl.admin.WorkflowAttributesGetRequest\x1a-.flyteidl.admin.WorkflowAttributesGetResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/api/v1/workflow_attributes/{project}/{domain}/{workflow}\x12\xc3\x01\n\x18\x44\x65leteWorkflowAttributes\x12/.flyteidl.admin.WorkflowAttributesDeleteRequest\x1a\x30.flyteidl.admin.WorkflowAttributesDeleteResponse\"D\x82\xd3\xe4\x93\x02>:\x01**9/api/v1/workflow_attributes/{project}/{domain}/{workflow}\x12\xa0\x01\n\x17ListMatchableAttributes\x12..flyteidl.admin.ListMatchableAttributesRequest\x1a/.flyteidl.admin.ListMatchableAttributesResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/matchable_attributes\x12\x9f\x01\n\x11ListNamedEntities\x12&.flyteidl.admin.NamedEntityListRequest\x1a\x1f.flyteidl.admin.NamedEntityList\"A\x82\xd3\xe4\x93\x02;\x12\x39/api/v1/named_entities/{resource_type}/{project}/{domain}\x12\xa7\x01\n\x0eGetNamedEntity\x12%.flyteidl.admin.NamedEntityGetRequest\x1a\x1b.flyteidl.admin.NamedEntity\"Q\x82\xd3\xe4\x93\x02K\x12I/api/v1/named_entities/{resource_type}/{id.project}/{id.domain}/{id.name}\x12\xbe\x01\n\x11UpdateNamedEntity\x12(.flyteidl.admin.NamedEntityUpdateRequest\x1a).flyteidl.admin.NamedEntityUpdateResponse\"T\x82\xd3\xe4\x93\x02N:\x01*\x1aI/api/v1/named_entities/{resource_type}/{id.project}/{id.domain}/{id.name}\x12l\n\nGetVersion\x12!.flyteidl.admin.GetVersionRequest\x1a\".flyteidl.admin.GetVersionResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/version\x12\xc4\x01\n\x14GetDescriptionEntity\x12 .flyteidl.admin.ObjectGetRequest\x1a!.flyteidl.admin.DescriptionEntity\"g\x82\xd3\xe4\x93\x02\x61\x12_/api/v1/description_entities/{id.resource_type}/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x92\x02\n\x17ListDescriptionEntities\x12,.flyteidl.admin.DescriptionEntityListRequest\x1a%.flyteidl.admin.DescriptionEntityList\"\xa1\x01\x82\xd3\xe4\x93\x02\x9a\x01ZG\x12\x45/api/v1/description_entities/{resource_type}/{id.project}/{id.domain}\x12O/api/v1/description_entities/{resource_type}/{id.project}/{id.domain}/{id.name}B\xbc\x01\n\x14\x63om.flyteidl.serviceB\nAdminProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66lyteidl/service/admin.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1c\x66lyteidl/admin/project.proto\x1a.flyteidl/admin/project_domain_attributes.proto\x1a\'flyteidl/admin/project_attributes.proto\x1a\x19\x66lyteidl/admin/task.proto\x1a\x1d\x66lyteidl/admin/workflow.proto\x1a(flyteidl/admin/workflow_attributes.proto\x1a flyteidl/admin/launch_plan.proto\x1a\x1a\x66lyteidl/admin/event.proto\x1a\x1e\x66lyteidl/admin/execution.proto\x1a\'flyteidl/admin/matchable_resource.proto\x1a#flyteidl/admin/node_execution.proto\x1a#flyteidl/admin/task_execution.proto\x1a\x1c\x66lyteidl/admin/version.proto\x1a\x1b\x66lyteidl/admin/common.proto\x1a\'flyteidl/admin/description_entity.proto2\x84N\n\x0c\x41\x64minService\x12m\n\nCreateTask\x12!.flyteidl.admin.TaskCreateRequest\x1a\".flyteidl.admin.TaskCreateResponse\"\x18\x82\xd3\xe4\x93\x02\x12:\x01*\"\r/api/v1/tasks\x12\x88\x01\n\x07GetTask\x12 .flyteidl.admin.ObjectGetRequest\x1a\x14.flyteidl.admin.Task\"E\x82\xd3\xe4\x93\x02?\x12=/api/v1/tasks/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x97\x01\n\x0bListTaskIds\x12\x30.flyteidl.admin.NamedEntityIdentifierListRequest\x1a).flyteidl.admin.NamedEntityIdentifierList\"+\x82\xd3\xe4\x93\x02%\x12#/api/v1/task_ids/{project}/{domain}\x12\xae\x01\n\tListTasks\x12#.flyteidl.admin.ResourceListRequest\x1a\x18.flyteidl.admin.TaskList\"b\x82\xd3\xe4\x93\x02\\Z(\x12&/api/v1/tasks/{id.project}/{id.domain}\x12\x30/api/v1/tasks/{id.project}/{id.domain}/{id.name}\x12}\n\x0e\x43reateWorkflow\x12%.flyteidl.admin.WorkflowCreateRequest\x1a&.flyteidl.admin.WorkflowCreateResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/api/v1/workflows\x12\x94\x01\n\x0bGetWorkflow\x12 .flyteidl.admin.ObjectGetRequest\x1a\x18.flyteidl.admin.Workflow\"I\x82\xd3\xe4\x93\x02\x43\x12\x41/api/v1/workflows/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x9f\x01\n\x0fListWorkflowIds\x12\x30.flyteidl.admin.NamedEntityIdentifierListRequest\x1a).flyteidl.admin.NamedEntityIdentifierList\"/\x82\xd3\xe4\x93\x02)\x12\'/api/v1/workflow_ids/{project}/{domain}\x12\xbe\x01\n\rListWorkflows\x12#.flyteidl.admin.ResourceListRequest\x1a\x1c.flyteidl.admin.WorkflowList\"j\x82\xd3\xe4\x93\x02\x64Z,\x12*/api/v1/workflows/{id.project}/{id.domain}\x12\x34/api/v1/workflows/{id.project}/{id.domain}/{id.name}\x12\x86\x01\n\x10\x43reateLaunchPlan\x12\'.flyteidl.admin.LaunchPlanCreateRequest\x1a(.flyteidl.admin.LaunchPlanCreateResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/api/v1/launch_plans\x12\x9b\x01\n\rGetLaunchPlan\x12 .flyteidl.admin.ObjectGetRequest\x1a\x1a.flyteidl.admin.LaunchPlan\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/api/v1/launch_plans/{id.project}/{id.domain}/{id.name}/{id.version}\x12\xa2\x01\n\x13GetActiveLaunchPlan\x12\'.flyteidl.admin.ActiveLaunchPlanRequest\x1a\x1a.flyteidl.admin.LaunchPlan\"F\x82\xd3\xe4\x93\x02@\x12>/api/v1/active_launch_plans/{id.project}/{id.domain}/{id.name}\x12\x9c\x01\n\x15ListActiveLaunchPlans\x12+.flyteidl.admin.ActiveLaunchPlanListRequest\x1a\x1e.flyteidl.admin.LaunchPlanList\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/active_launch_plans/{project}/{domain}\x12\xa4\x01\n\x11ListLaunchPlanIds\x12\x30.flyteidl.admin.NamedEntityIdentifierListRequest\x1a).flyteidl.admin.NamedEntityIdentifierList\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/launch_plan_ids/{project}/{domain}\x12\xc8\x01\n\x0fListLaunchPlans\x12#.flyteidl.admin.ResourceListRequest\x1a\x1e.flyteidl.admin.LaunchPlanList\"p\x82\xd3\xe4\x93\x02jZ/\x12-/api/v1/launch_plans/{id.project}/{id.domain}\x12\x37/api/v1/launch_plans/{id.project}/{id.domain}/{id.name}\x12\xb6\x01\n\x10UpdateLaunchPlan\x12\'.flyteidl.admin.LaunchPlanUpdateRequest\x1a(.flyteidl.admin.LaunchPlanUpdateResponse\"O\x82\xd3\xe4\x93\x02I:\x01*\x1a\x44/api/v1/launch_plans/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x81\x01\n\x0f\x43reateExecution\x12&.flyteidl.admin.ExecutionCreateRequest\x1a\'.flyteidl.admin.ExecutionCreateResponse\"\x1d\x82\xd3\xe4\x93\x02\x17:\x01*\"\x12/api/v1/executions\x12\x8e\x01\n\x11RelaunchExecution\x12(.flyteidl.admin.ExecutionRelaunchRequest\x1a\'.flyteidl.admin.ExecutionCreateResponse\"&\x82\xd3\xe4\x93\x02 :\x01*\"\x1b/api/v1/executions/relaunch\x12\x8b\x01\n\x10RecoverExecution\x12\'.flyteidl.admin.ExecutionRecoverRequest\x1a\'.flyteidl.admin.ExecutionCreateResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/api/v1/executions/recover\x12\x95\x01\n\x0cGetExecution\x12+.flyteidl.admin.WorkflowExecutionGetRequest\x1a\x19.flyteidl.admin.Execution\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/executions/{id.project}/{id.domain}/{id.name}\x12\xa4\x01\n\x0fUpdateExecution\x12&.flyteidl.admin.ExecutionUpdateRequest\x1a\'.flyteidl.admin.ExecutionUpdateResponse\"@\x82\xd3\xe4\x93\x02::\x01*\x1a\x35/api/v1/executions/{id.project}/{id.domain}/{id.name}\x12\xb9\x01\n\x10GetExecutionData\x12/.flyteidl.admin.WorkflowExecutionGetDataRequest\x1a\x30.flyteidl.admin.WorkflowExecutionGetDataResponse\"B\x82\xd3\xe4\x93\x02<\x12:/api/v1/data/executions/{id.project}/{id.domain}/{id.name}\x12\x89\x01\n\x0eListExecutions\x12#.flyteidl.admin.ResourceListRequest\x1a\x1d.flyteidl.admin.ExecutionList\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/executions/{id.project}/{id.domain}\x12\xad\x01\n\x12TerminateExecution\x12).flyteidl.admin.ExecutionTerminateRequest\x1a*.flyteidl.admin.ExecutionTerminateResponse\"@\x82\xd3\xe4\x93\x02::\x01**5/api/v1/executions/{id.project}/{id.domain}/{id.name}\x12\xd2\x01\n\x10GetNodeExecution\x12\'.flyteidl.admin.NodeExecutionGetRequest\x1a\x1d.flyteidl.admin.NodeExecution\"v\x82\xd3\xe4\x93\x02p\x12n/api/v1/node_executions/{id.execution_id.project}/{id.execution_id.domain}/{id.execution_id.name}/{id.node_id}\x12\xde\x01\n\x12ListNodeExecutions\x12(.flyteidl.admin.NodeExecutionListRequest\x1a!.flyteidl.admin.NodeExecutionList\"{\x82\xd3\xe4\x93\x02u\x12s/api/v1/node_executions/{workflow_execution_id.project}/{workflow_execution_id.domain}/{workflow_execution_id.name}\x12\xa5\x04\n\x19ListNodeExecutionsForTask\x12/.flyteidl.admin.NodeExecutionForTaskListRequest\x1a!.flyteidl.admin.NodeExecutionList\"\xb3\x03\x82\xd3\xe4\x93\x02\xac\x03\x12\xa9\x03/api/v1/children/task_executions/{task_execution_id.node_execution_id.execution_id.project}/{task_execution_id.node_execution_id.execution_id.domain}/{task_execution_id.node_execution_id.execution_id.name}/{task_execution_id.node_execution_id.node_id}/{task_execution_id.task_id.project}/{task_execution_id.task_id.domain}/{task_execution_id.task_id.name}/{task_execution_id.task_id.version}/{task_execution_id.retry_attempt}\x12\xee\x01\n\x14GetNodeExecutionData\x12+.flyteidl.admin.NodeExecutionGetDataRequest\x1a,.flyteidl.admin.NodeExecutionGetDataResponse\"{\x82\xd3\xe4\x93\x02u\x12s/api/v1/data/node_executions/{id.execution_id.project}/{id.execution_id.domain}/{id.execution_id.name}/{id.node_id}\x12\x7f\n\x0fRegisterProject\x12&.flyteidl.admin.ProjectRegisterRequest\x1a\'.flyteidl.admin.ProjectRegisterResponse\"\x1b\x82\xd3\xe4\x93\x02\x15:\x01*\"\x10/api/v1/projects\x12q\n\rUpdateProject\x12\x17.flyteidl.admin.Project\x1a%.flyteidl.admin.ProjectUpdateResponse\" \x82\xd3\xe4\x93\x02\x1a:\x01*\x1a\x15/api/v1/projects/{id}\x12\x66\n\x0cListProjects\x12\".flyteidl.admin.ProjectListRequest\x1a\x18.flyteidl.admin.Projects\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/api/v1/projects\x12\x99\x01\n\x13\x43reateWorkflowEvent\x12-.flyteidl.admin.WorkflowExecutionEventRequest\x1a..flyteidl.admin.WorkflowExecutionEventResponse\"#\x82\xd3\xe4\x93\x02\x1d:\x01*\"\x18/api/v1/events/workflows\x12\x89\x01\n\x0f\x43reateNodeEvent\x12).flyteidl.admin.NodeExecutionEventRequest\x1a*.flyteidl.admin.NodeExecutionEventResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/api/v1/events/nodes\x12\x89\x01\n\x0f\x43reateTaskEvent\x12).flyteidl.admin.TaskExecutionEventRequest\x1a*.flyteidl.admin.TaskExecutionEventResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/api/v1/events/tasks\x12\x80\x03\n\x10GetTaskExecution\x12\'.flyteidl.admin.TaskExecutionGetRequest\x1a\x1d.flyteidl.admin.TaskExecution\"\xa3\x02\x82\xd3\xe4\x93\x02\x9c\x02\x12\x99\x02/api/v1/task_executions/{id.node_execution_id.execution_id.project}/{id.node_execution_id.execution_id.domain}/{id.node_execution_id.execution_id.name}/{id.node_execution_id.node_id}/{id.task_id.project}/{id.task_id.domain}/{id.task_id.name}/{id.task_id.version}/{id.retry_attempt}\x12\x98\x02\n\x12ListTaskExecutions\x12(.flyteidl.admin.TaskExecutionListRequest\x1a!.flyteidl.admin.TaskExecutionList\"\xb4\x01\x82\xd3\xe4\x93\x02\xad\x01\x12\xaa\x01/api/v1/task_executions/{node_execution_id.execution_id.project}/{node_execution_id.execution_id.domain}/{node_execution_id.execution_id.name}/{node_execution_id.node_id}\x12\x9c\x03\n\x14GetTaskExecutionData\x12+.flyteidl.admin.TaskExecutionGetDataRequest\x1a,.flyteidl.admin.TaskExecutionGetDataResponse\"\xa8\x02\x82\xd3\xe4\x93\x02\xa1\x02\x12\x9e\x02/api/v1/data/task_executions/{id.node_execution_id.execution_id.project}/{id.node_execution_id.execution_id.domain}/{id.node_execution_id.execution_id.name}/{id.node_execution_id.node_id}/{id.task_id.project}/{id.task_id.domain}/{id.task_id.name}/{id.task_id.version}/{id.retry_attempt}\x12\xe3\x01\n\x1dUpdateProjectDomainAttributes\x12\x34.flyteidl.admin.ProjectDomainAttributesUpdateRequest\x1a\x35.flyteidl.admin.ProjectDomainAttributesUpdateResponse\"U\x82\xd3\xe4\x93\x02O:\x01*\x1aJ/api/v1/project_domain_attributes/{attributes.project}/{attributes.domain}\x12\xc1\x01\n\x1aGetProjectDomainAttributes\x12\x31.flyteidl.admin.ProjectDomainAttributesGetRequest\x1a\x32.flyteidl.admin.ProjectDomainAttributesGetResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/api/v1/project_domain_attributes/{project}/{domain}\x12\xcd\x01\n\x1d\x44\x65leteProjectDomainAttributes\x12\x34.flyteidl.admin.ProjectDomainAttributesDeleteRequest\x1a\x35.flyteidl.admin.ProjectDomainAttributesDeleteResponse\"?\x82\xd3\xe4\x93\x02\x39:\x01**4/api/v1/project_domain_attributes/{project}/{domain}\x12\xb6\x01\n\x17UpdateProjectAttributes\x12..flyteidl.admin.ProjectAttributesUpdateRequest\x1a/.flyteidl.admin.ProjectAttributesUpdateResponse\":\x82\xd3\xe4\x93\x02\x34:\x01*\x1a//api/v1/project_attributes/{attributes.project}\x12\x9f\x01\n\x14GetProjectAttributes\x12+.flyteidl.admin.ProjectAttributesGetRequest\x1a,.flyteidl.admin.ProjectAttributesGetResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/project_attributes/{project}\x12\xab\x01\n\x17\x44\x65leteProjectAttributes\x12..flyteidl.admin.ProjectAttributesDeleteRequest\x1a/.flyteidl.admin.ProjectAttributesDeleteResponse\"/\x82\xd3\xe4\x93\x02):\x01**$/api/v1/project_attributes/{project}\x12\xe4\x01\n\x18UpdateWorkflowAttributes\x12/.flyteidl.admin.WorkflowAttributesUpdateRequest\x1a\x30.flyteidl.admin.WorkflowAttributesUpdateResponse\"e\x82\xd3\xe4\x93\x02_:\x01*\x1aZ/api/v1/workflow_attributes/{attributes.project}/{attributes.domain}/{attributes.workflow}\x12\xb7\x01\n\x15GetWorkflowAttributes\x12,.flyteidl.admin.WorkflowAttributesGetRequest\x1a-.flyteidl.admin.WorkflowAttributesGetResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/api/v1/workflow_attributes/{project}/{domain}/{workflow}\x12\xc3\x01\n\x18\x44\x65leteWorkflowAttributes\x12/.flyteidl.admin.WorkflowAttributesDeleteRequest\x1a\x30.flyteidl.admin.WorkflowAttributesDeleteResponse\"D\x82\xd3\xe4\x93\x02>:\x01**9/api/v1/workflow_attributes/{project}/{domain}/{workflow}\x12\xa0\x01\n\x17ListMatchableAttributes\x12..flyteidl.admin.ListMatchableAttributesRequest\x1a/.flyteidl.admin.ListMatchableAttributesResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/matchable_attributes\x12\x9f\x01\n\x11ListNamedEntities\x12&.flyteidl.admin.NamedEntityListRequest\x1a\x1f.flyteidl.admin.NamedEntityList\"A\x82\xd3\xe4\x93\x02;\x12\x39/api/v1/named_entities/{resource_type}/{project}/{domain}\x12\xa7\x01\n\x0eGetNamedEntity\x12%.flyteidl.admin.NamedEntityGetRequest\x1a\x1b.flyteidl.admin.NamedEntity\"Q\x82\xd3\xe4\x93\x02K\x12I/api/v1/named_entities/{resource_type}/{id.project}/{id.domain}/{id.name}\x12\xbe\x01\n\x11UpdateNamedEntity\x12(.flyteidl.admin.NamedEntityUpdateRequest\x1a).flyteidl.admin.NamedEntityUpdateResponse\"T\x82\xd3\xe4\x93\x02N:\x01*\x1aI/api/v1/named_entities/{resource_type}/{id.project}/{id.domain}/{id.name}\x12l\n\nGetVersion\x12!.flyteidl.admin.GetVersionRequest\x1a\".flyteidl.admin.GetVersionResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/version\x12\xc4\x01\n\x14GetDescriptionEntity\x12 .flyteidl.admin.ObjectGetRequest\x1a!.flyteidl.admin.DescriptionEntity\"g\x82\xd3\xe4\x93\x02\x61\x12_/api/v1/description_entities/{id.resource_type}/{id.project}/{id.domain}/{id.name}/{id.version}\x12\x92\x02\n\x17ListDescriptionEntities\x12,.flyteidl.admin.DescriptionEntityListRequest\x1a%.flyteidl.admin.DescriptionEntityList\"\xa1\x01\x82\xd3\xe4\x93\x02\x9a\x01ZG\x12\x45/api/v1/description_entities/{resource_type}/{id.project}/{id.domain}\x12O/api/v1/description_entities/{resource_type}/{id.project}/{id.domain}/{id.name}\x12\xc5\x01\n\x13GetExecutionMetrics\x12\x32.flyteidl.admin.WorkflowExecutionGetMetricsRequest\x1a\x33.flyteidl.admin.WorkflowExecutionGetMetricsResponse\"E\x82\xd3\xe4\x93\x02?\x12=/api/v1/metrics/executions/{id.project}/{id.domain}/{id.name}B\xbc\x01\n\x14\x63om.flyteidl.serviceB\nAdminProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.admin_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.admin_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.serviceB\nAdminProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\242\002\003FSX\252\002\020Flyteidl.Service\312\002\020Flyteidl\\Service\342\002\034Flyteidl\\Service\\GPBMetadata\352\002\021Flyteidl::Service'
   _ADMINSERVICE.methods_by_name['CreateTask']._options = None
   _ADMINSERVICE.methods_by_name['CreateTask']._serialized_options = b'\202\323\344\223\002\022:\001*\"\r/api/v1/tasks'
   _ADMINSERVICE.methods_by_name['GetTask']._options = None
@@ -138,10 +138,12 @@
   _ADMINSERVICE.methods_by_name['UpdateNamedEntity']._serialized_options = b'\202\323\344\223\002N:\001*\032I/api/v1/named_entities/{resource_type}/{id.project}/{id.domain}/{id.name}'
   _ADMINSERVICE.methods_by_name['GetVersion']._options = None
   _ADMINSERVICE.methods_by_name['GetVersion']._serialized_options = b'\202\323\344\223\002\021\022\017/api/v1/version'
   _ADMINSERVICE.methods_by_name['GetDescriptionEntity']._options = None
   _ADMINSERVICE.methods_by_name['GetDescriptionEntity']._serialized_options = b'\202\323\344\223\002a\022_/api/v1/description_entities/{id.resource_type}/{id.project}/{id.domain}/{id.name}/{id.version}'
   _ADMINSERVICE.methods_by_name['ListDescriptionEntities']._options = None
   _ADMINSERVICE.methods_by_name['ListDescriptionEntities']._serialized_options = b'\202\323\344\223\002\232\001ZG\022E/api/v1/description_entities/{resource_type}/{id.project}/{id.domain}\022O/api/v1/description_entities/{resource_type}/{id.project}/{id.domain}/{id.name}'
-  _ADMINSERVICE._serialized_start=641
-  _ADMINSERVICE._serialized_end=10429
+  _ADMINSERVICE.methods_by_name['GetExecutionMetrics']._options = None
+  _ADMINSERVICE.methods_by_name['GetExecutionMetrics']._serialized_options = b'\202\323\344\223\002?\022=/api/v1/metrics/executions/{id.project}/{id.domain}/{id.name}'
+  _globals['_ADMINSERVICE']._serialized_start=609
+  _globals['_ADMINSERVICE']._serialized_end=10597
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/admin_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/admin_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,12 +10,11 @@
 from flyteidl.admin import execution_pb2 as _execution_pb2
 from flyteidl.admin import matchable_resource_pb2 as _matchable_resource_pb2
 from flyteidl.admin import node_execution_pb2 as _node_execution_pb2
 from flyteidl.admin import task_execution_pb2 as _task_execution_pb2
 from flyteidl.admin import version_pb2 as _version_pb2
 from flyteidl.admin import common_pb2 as _common_pb2
 from flyteidl.admin import description_entity_pb2 as _description_entity_pb2
-from flyteidl.core import identifier_pb2 as _identifier_pb2
 from google.protobuf import descriptor as _descriptor
 from typing import ClassVar as _ClassVar
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/admin_pb2_grpc.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/admin_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,14 +286,19 @@
                 response_deserializer=flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntity.FromString,
                 )
         self.ListDescriptionEntities = channel.unary_unary(
                 '/flyteidl.service.AdminService/ListDescriptionEntities',
                 request_serializer=flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntityListRequest.SerializeToString,
                 response_deserializer=flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntityList.FromString,
                 )
+        self.GetExecutionMetrics = channel.unary_unary(
+                '/flyteidl.service.AdminService/GetExecutionMetrics',
+                request_serializer=flyteidl_dot_admin_dot_execution__pb2.WorkflowExecutionGetMetricsRequest.SerializeToString,
+                response_deserializer=flyteidl_dot_admin_dot_execution__pb2.WorkflowExecutionGetMetricsResponse.FromString,
+                )
 
 
 class AdminServiceServicer(object):
     """The following defines an RPC service that is also served over HTTP via grpc-gateway.
     Standard response codes for both are defined here: https://github.com/grpc-ecosystem/grpc-gateway/blob/master/runtime/errors.go
     """
 
@@ -662,14 +667,21 @@
     def ListDescriptionEntities(self, request, context):
         """Fetch a list of :ref:`ref_flyteidl.admin.DescriptionEntity` definitions.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetExecutionMetrics(self, request, context):
+        """Fetches runtime metrics for a :ref:`ref_flyteidl.admin.Execution`.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_AdminServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateTask': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateTask,
                     request_deserializer=flyteidl_dot_admin_dot_task__pb2.TaskCreateRequest.FromString,
                     response_serializer=flyteidl_dot_admin_dot_task__pb2.TaskCreateResponse.SerializeToString,
@@ -925,14 +937,19 @@
                     response_serializer=flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntity.SerializeToString,
             ),
             'ListDescriptionEntities': grpc.unary_unary_rpc_method_handler(
                     servicer.ListDescriptionEntities,
                     request_deserializer=flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntityListRequest.FromString,
                     response_serializer=flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntityList.SerializeToString,
             ),
+            'GetExecutionMetrics': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetExecutionMetrics,
+                    request_deserializer=flyteidl_dot_admin_dot_execution__pb2.WorkflowExecutionGetMetricsRequest.FromString,
+                    response_serializer=flyteidl_dot_admin_dot_execution__pb2.WorkflowExecutionGetMetricsResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'flyteidl.service.AdminService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -1820,7 +1837,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/flyteidl.service.AdminService/ListDescriptionEntities',
             flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntityListRequest.SerializeToString,
             flyteidl_dot_admin_dot_description__entity__pb2.DescriptionEntityList.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetExecutionMetrics(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/flyteidl.service.AdminService/GetExecutionMetrics',
+            flyteidl_dot_admin_dot_execution__pb2.WorkflowExecutionGetMetricsRequest.SerializeToString,
+            flyteidl_dot_admin_dot_execution__pb2.WorkflowExecutionGetMetricsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/auth_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/auth_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/service/auth.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\"\x17\n\x15OAuth2MetadataRequest\"\xa1\x04\n\x16OAuth2MetadataResponse\x12\x16\n\x06issuer\x18\x01 \x01(\tR\x06issuer\x12\x35\n\x16\x61uthorization_endpoint\x18\x02 \x01(\tR\x15\x61uthorizationEndpoint\x12%\n\x0etoken_endpoint\x18\x03 \x01(\tR\rtokenEndpoint\x12\x38\n\x18response_types_supported\x18\x04 \x03(\tR\x16responseTypesSupported\x12)\n\x10scopes_supported\x18\x05 \x03(\tR\x0fscopesSupported\x12P\n%token_endpoint_auth_methods_supported\x18\x06 \x03(\tR!tokenEndpointAuthMethodsSupported\x12\x19\n\x08jwks_uri\x18\x07 \x01(\tR\x07jwksUri\x12G\n code_challenge_methods_supported\x18\x08 \x03(\tR\x1d\x63odeChallengeMethodsSupported\x12\x32\n\x15grant_types_supported\x18\t \x03(\tR\x13grantTypesSupported\x12\x42\n\x1d\x64\x65vice_authorization_endpoint\x18\n \x01(\tR\x1b\x64\x65viceAuthorizationEndpoint\"\x1f\n\x1dPublicClientAuthConfigRequest\"\x86\x02\n\x1ePublicClientAuthConfigResponse\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12!\n\x0credirect_uri\x18\x02 \x01(\tR\x0bredirectUri\x12\x16\n\x06scopes\x18\x03 \x03(\tR\x06scopes\x12<\n\x1a\x61uthorization_metadata_key\x18\x04 \x01(\tR\x18\x61uthorizationMetadataKey\x12\x32\n\x15service_http_endpoint\x18\x05 \x01(\tR\x13serviceHttpEndpoint\x12\x1a\n\x08\x61udience\x18\x06 \x01(\tR\x08\x61udience2\xcd\x02\n\x13\x41uthMetadataService\x12\x97\x01\n\x11GetOAuth2Metadata\x12\'.flyteidl.service.OAuth2MetadataRequest\x1a(.flyteidl.service.OAuth2MetadataResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/.well-known/oauth-authorization-server\x12\x9b\x01\n\x15GetPublicClientConfig\x12/.flyteidl.service.PublicClientAuthConfigRequest\x1a\x30.flyteidl.service.PublicClientAuthConfigResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/config/v1/flyte_clientB\xbb\x01\n\x14\x63om.flyteidl.serviceB\tAuthProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.auth_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.auth_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.serviceB\tAuthProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\242\002\003FSX\252\002\020Flyteidl.Service\312\002\020Flyteidl\\Service\342\002\034Flyteidl\\Service\\GPBMetadata\352\002\021Flyteidl::Service'
   _AUTHMETADATASERVICE.methods_by_name['GetOAuth2Metadata']._options = None
   _AUTHMETADATASERVICE.methods_by_name['GetOAuth2Metadata']._serialized_options = b'\202\323\344\223\002)\022\'/.well-known/oauth-authorization-server'
   _AUTHMETADATASERVICE.methods_by_name['GetPublicClientConfig']._options = None
   _AUTHMETADATASERVICE.methods_by_name['GetPublicClientConfig']._serialized_options = b'\202\323\344\223\002\031\022\027/config/v1/flyte_client'
-  _OAUTH2METADATAREQUEST._serialized_start=79
-  _OAUTH2METADATAREQUEST._serialized_end=102
-  _OAUTH2METADATARESPONSE._serialized_start=105
-  _OAUTH2METADATARESPONSE._serialized_end=650
-  _PUBLICCLIENTAUTHCONFIGREQUEST._serialized_start=652
-  _PUBLICCLIENTAUTHCONFIGREQUEST._serialized_end=683
-  _PUBLICCLIENTAUTHCONFIGRESPONSE._serialized_start=686
-  _PUBLICCLIENTAUTHCONFIGRESPONSE._serialized_end=948
-  _AUTHMETADATASERVICE._serialized_start=951
-  _AUTHMETADATASERVICE._serialized_end=1284
+  _globals['_OAUTH2METADATAREQUEST']._serialized_start=79
+  _globals['_OAUTH2METADATAREQUEST']._serialized_end=102
+  _globals['_OAUTH2METADATARESPONSE']._serialized_start=105
+  _globals['_OAUTH2METADATARESPONSE']._serialized_end=650
+  _globals['_PUBLICCLIENTAUTHCONFIGREQUEST']._serialized_start=652
+  _globals['_PUBLICCLIENTAUTHCONFIGREQUEST']._serialized_end=683
+  _globals['_PUBLICCLIENTAUTHCONFIGRESPONSE']._serialized_start=686
+  _globals['_PUBLICCLIENTAUTHCONFIGRESPONSE']._serialized_end=948
+  _globals['_AUTHMETADATASERVICE']._serialized_start=951
+  _globals['_AUTHMETADATASERVICE']._serialized_end=1284
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/auth_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/auth_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -7,49 +7,49 @@
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class OAuth2MetadataRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class OAuth2MetadataResponse(_message.Message):
-    __slots__ = ["authorization_endpoint", "code_challenge_methods_supported", "device_authorization_endpoint", "grant_types_supported", "issuer", "jwks_uri", "response_types_supported", "scopes_supported", "token_endpoint", "token_endpoint_auth_methods_supported"]
-    AUTHORIZATION_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
-    CODE_CHALLENGE_METHODS_SUPPORTED_FIELD_NUMBER: _ClassVar[int]
-    DEVICE_AUTHORIZATION_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
-    GRANT_TYPES_SUPPORTED_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["issuer", "authorization_endpoint", "token_endpoint", "response_types_supported", "scopes_supported", "token_endpoint_auth_methods_supported", "jwks_uri", "code_challenge_methods_supported", "grant_types_supported", "device_authorization_endpoint"]
     ISSUER_FIELD_NUMBER: _ClassVar[int]
-    JWKS_URI_FIELD_NUMBER: _ClassVar[int]
+    AUTHORIZATION_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
+    TOKEN_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_TYPES_SUPPORTED_FIELD_NUMBER: _ClassVar[int]
     SCOPES_SUPPORTED_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ENDPOINT_AUTH_METHODS_SUPPORTED_FIELD_NUMBER: _ClassVar[int]
-    TOKEN_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
-    authorization_endpoint: str
-    code_challenge_methods_supported: _containers.RepeatedScalarFieldContainer[str]
-    device_authorization_endpoint: str
-    grant_types_supported: _containers.RepeatedScalarFieldContainer[str]
+    JWKS_URI_FIELD_NUMBER: _ClassVar[int]
+    CODE_CHALLENGE_METHODS_SUPPORTED_FIELD_NUMBER: _ClassVar[int]
+    GRANT_TYPES_SUPPORTED_FIELD_NUMBER: _ClassVar[int]
+    DEVICE_AUTHORIZATION_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     issuer: str
-    jwks_uri: str
+    authorization_endpoint: str
+    token_endpoint: str
     response_types_supported: _containers.RepeatedScalarFieldContainer[str]
     scopes_supported: _containers.RepeatedScalarFieldContainer[str]
-    token_endpoint: str
     token_endpoint_auth_methods_supported: _containers.RepeatedScalarFieldContainer[str]
+    jwks_uri: str
+    code_challenge_methods_supported: _containers.RepeatedScalarFieldContainer[str]
+    grant_types_supported: _containers.RepeatedScalarFieldContainer[str]
+    device_authorization_endpoint: str
     def __init__(self, issuer: _Optional[str] = ..., authorization_endpoint: _Optional[str] = ..., token_endpoint: _Optional[str] = ..., response_types_supported: _Optional[_Iterable[str]] = ..., scopes_supported: _Optional[_Iterable[str]] = ..., token_endpoint_auth_methods_supported: _Optional[_Iterable[str]] = ..., jwks_uri: _Optional[str] = ..., code_challenge_methods_supported: _Optional[_Iterable[str]] = ..., grant_types_supported: _Optional[_Iterable[str]] = ..., device_authorization_endpoint: _Optional[str] = ...) -> None: ...
 
 class PublicClientAuthConfigRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class PublicClientAuthConfigResponse(_message.Message):
-    __slots__ = ["audience", "authorization_metadata_key", "client_id", "redirect_uri", "scopes", "service_http_endpoint"]
-    AUDIENCE_FIELD_NUMBER: _ClassVar[int]
-    AUTHORIZATION_METADATA_KEY_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["client_id", "redirect_uri", "scopes", "authorization_metadata_key", "service_http_endpoint", "audience"]
     CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
     REDIRECT_URI_FIELD_NUMBER: _ClassVar[int]
     SCOPES_FIELD_NUMBER: _ClassVar[int]
+    AUTHORIZATION_METADATA_KEY_FIELD_NUMBER: _ClassVar[int]
     SERVICE_HTTP_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
-    audience: str
-    authorization_metadata_key: str
+    AUDIENCE_FIELD_NUMBER: _ClassVar[int]
     client_id: str
     redirect_uri: str
     scopes: _containers.RepeatedScalarFieldContainer[str]
+    authorization_metadata_key: str
     service_http_endpoint: str
+    audience: str
     def __init__(self, client_id: _Optional[str] = ..., redirect_uri: _Optional[str] = ..., scopes: _Optional[_Iterable[str]] = ..., authorization_metadata_key: _Optional[str] = ..., service_http_endpoint: _Optional[str] = ..., audience: _Optional[str] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/auth_pb2_grpc.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/dataproxy_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/dataproxy_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,44 +11,58 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
+from flyteidl.core import literals_pb2 as flyteidl_dot_core_dot_literals__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n flyteidl/service/dataproxy.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1e\x66lyteidl/core/identifier.proto\"\x97\x01\n\x1c\x43reateUploadLocationResponse\x12\x1d\n\nsigned_url\x18\x01 \x01(\tR\tsignedUrl\x12\x1d\n\nnative_url\x18\x02 \x01(\tR\tnativeUrl\x12\x39\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\"\xc6\x01\n\x1b\x43reateUploadLocationRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x1a\n\x08\x66ilename\x18\x03 \x01(\tR\x08\x66ilename\x12\x38\n\nexpires_in\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\texpiresIn\x12\x1f\n\x0b\x63ontent_md5\x18\x05 \x01(\x0cR\ncontentMd5\"|\n\x1d\x43reateDownloadLocationRequest\x12\x1d\n\nnative_url\x18\x01 \x01(\tR\tnativeUrl\x12\x38\n\nexpires_in\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\texpiresIn:\x02\x18\x01\"~\n\x1e\x43reateDownloadLocationResponse\x12\x1d\n\nsigned_url\x18\x01 \x01(\tR\tsignedUrl\x12\x39\n\nexpires_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt:\x02\x18\x01\"\xfa\x01\n\x19\x43reateDownloadLinkRequest\x12\x43\n\rartifact_type\x18\x01 \x01(\x0e\x32\x1e.flyteidl.service.ArtifactTypeR\x0c\x61rtifactType\x12\x38\n\nexpires_in\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\texpiresIn\x12T\n\x11node_execution_id\x18\x03 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierH\x00R\x0fnodeExecutionIdB\x08\n\x06source\"v\n\x1a\x43reateDownloadLinkResponse\x12\x1d\n\nsigned_url\x18\x01 \x03(\tR\tsignedUrl\x12\x39\n\nexpires_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt*C\n\x0c\x41rtifactType\x12\x1b\n\x17\x41RTIFACT_TYPE_UNDEFINED\x10\x00\x12\x16\n\x12\x41RTIFACT_TYPE_DECK\x10\x01\x32\xfc\x03\n\x10\x44\x61taProxyService\x12\xa0\x01\n\x14\x43reateUploadLocation\x12-.flyteidl.service.CreateUploadLocationRequest\x1a..flyteidl.service.CreateUploadLocationResponse\")\x82\xd3\xe4\x93\x02#:\x01*\"\x1e/api/v1/dataproxy/artifact_urn\x12\xa6\x01\n\x16\x43reateDownloadLocation\x12/.flyteidl.service.CreateDownloadLocationRequest\x1a\x30.flyteidl.service.CreateDownloadLocationResponse\")\x88\x02\x01\x82\xd3\xe4\x93\x02 \x12\x1e/api/v1/dataproxy/artifact_urn\x12\x9b\x01\n\x12\x43reateDownloadLink\x12+.flyteidl.service.CreateDownloadLinkRequest\x1a,.flyteidl.service.CreateDownloadLinkResponse\"*\x82\xd3\xe4\x93\x02$:\x01*\"\x1f/api/v1/dataproxy/artifact_linkB\xc0\x01\n\x14\x63om.flyteidl.serviceB\x0e\x44\x61taproxyProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n flyteidl/service/dataproxy.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1e\x66lyteidl/core/identifier.proto\x1a\x1c\x66lyteidl/core/literals.proto\"\x97\x01\n\x1c\x43reateUploadLocationResponse\x12\x1d\n\nsigned_url\x18\x01 \x01(\tR\tsignedUrl\x12\x1d\n\nnative_url\x18\x02 \x01(\tR\tnativeUrl\x12\x39\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\"\xc6\x01\n\x1b\x43reateUploadLocationRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x16\n\x06\x64omain\x18\x02 \x01(\tR\x06\x64omain\x12\x1a\n\x08\x66ilename\x18\x03 \x01(\tR\x08\x66ilename\x12\x38\n\nexpires_in\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\texpiresIn\x12\x1f\n\x0b\x63ontent_md5\x18\x05 \x01(\x0cR\ncontentMd5\"|\n\x1d\x43reateDownloadLocationRequest\x12\x1d\n\nnative_url\x18\x01 \x01(\tR\tnativeUrl\x12\x38\n\nexpires_in\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\texpiresIn:\x02\x18\x01\"~\n\x1e\x43reateDownloadLocationResponse\x12\x1d\n\nsigned_url\x18\x01 \x01(\tR\tsignedUrl\x12\x39\n\nexpires_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt:\x02\x18\x01\"\xfa\x01\n\x19\x43reateDownloadLinkRequest\x12\x43\n\rartifact_type\x18\x01 \x01(\x0e\x32\x1e.flyteidl.service.ArtifactTypeR\x0c\x61rtifactType\x12\x38\n\nexpires_in\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\texpiresIn\x12T\n\x11node_execution_id\x18\x03 \x01(\x0b\x32&.flyteidl.core.NodeExecutionIdentifierH\x00R\x0fnodeExecutionIdB\x08\n\x06source\"\xc7\x01\n\x1a\x43reateDownloadLinkResponse\x12!\n\nsigned_url\x18\x01 \x03(\tB\x02\x18\x01R\tsignedUrl\x12=\n\nexpires_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01R\texpiresAt\x12G\n\x0fpre_signed_urls\x18\x03 \x01(\x0b\x32\x1f.flyteidl.service.PreSignedURLsR\rpreSignedUrls\"i\n\rPreSignedURLs\x12\x1d\n\nsigned_url\x18\x01 \x03(\tR\tsignedUrl\x12\x39\n\nexpires_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\"-\n\x0eGetDataRequest\x12\x1b\n\tflyte_url\x18\x01 \x01(\tR\x08\x66lyteUrl\"\xa2\x01\n\x0fGetDataResponse\x12<\n\x0bliteral_map\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.LiteralMapH\x00R\nliteralMap\x12I\n\x0fpre_signed_urls\x18\x02 \x01(\x0b\x32\x1f.flyteidl.service.PreSignedURLsH\x00R\rpreSignedUrlsB\x06\n\x04\x64\x61ta*C\n\x0c\x41rtifactType\x12\x1b\n\x17\x41RTIFACT_TYPE_UNDEFINED\x10\x00\x12\x16\n\x12\x41RTIFACT_TYPE_DECK\x10\x01\x32\xe2\x04\n\x10\x44\x61taProxyService\x12\xa0\x01\n\x14\x43reateUploadLocation\x12-.flyteidl.service.CreateUploadLocationRequest\x1a..flyteidl.service.CreateUploadLocationResponse\")\x82\xd3\xe4\x93\x02#:\x01*\"\x1e/api/v1/dataproxy/artifact_urn\x12\xa6\x01\n\x16\x43reateDownloadLocation\x12/.flyteidl.service.CreateDownloadLocationRequest\x1a\x30.flyteidl.service.CreateDownloadLocationResponse\")\x88\x02\x01\x82\xd3\xe4\x93\x02 \x12\x1e/api/v1/dataproxy/artifact_urn\x12\x9b\x01\n\x12\x43reateDownloadLink\x12+.flyteidl.service.CreateDownloadLinkRequest\x1a,.flyteidl.service.CreateDownloadLinkResponse\"*\x82\xd3\xe4\x93\x02$:\x01*\"\x1f/api/v1/dataproxy/artifact_link\x12\x64\n\x07GetData\x12 .flyteidl.service.GetDataRequest\x1a!.flyteidl.service.GetDataResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/api/v1/dataB\xc0\x01\n\x14\x63om.flyteidl.serviceB\x0e\x44\x61taproxyProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.dataproxy_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.dataproxy_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.serviceB\016DataproxyProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\242\002\003FSX\252\002\020Flyteidl.Service\312\002\020Flyteidl\\Service\342\002\034Flyteidl\\Service\\GPBMetadata\352\002\021Flyteidl::Service'
   _CREATEDOWNLOADLOCATIONREQUEST._options = None
   _CREATEDOWNLOADLOCATIONREQUEST._serialized_options = b'\030\001'
   _CREATEDOWNLOADLOCATIONRESPONSE._options = None
   _CREATEDOWNLOADLOCATIONRESPONSE._serialized_options = b'\030\001'
+  _CREATEDOWNLOADLINKRESPONSE.fields_by_name['signed_url']._options = None
+  _CREATEDOWNLOADLINKRESPONSE.fields_by_name['signed_url']._serialized_options = b'\030\001'
+  _CREATEDOWNLOADLINKRESPONSE.fields_by_name['expires_at']._options = None
+  _CREATEDOWNLOADLINKRESPONSE.fields_by_name['expires_at']._serialized_options = b'\030\001'
   _DATAPROXYSERVICE.methods_by_name['CreateUploadLocation']._options = None
   _DATAPROXYSERVICE.methods_by_name['CreateUploadLocation']._serialized_options = b'\202\323\344\223\002#:\001*\"\036/api/v1/dataproxy/artifact_urn'
   _DATAPROXYSERVICE.methods_by_name['CreateDownloadLocation']._options = None
   _DATAPROXYSERVICE.methods_by_name['CreateDownloadLocation']._serialized_options = b'\210\002\001\202\323\344\223\002 \022\036/api/v1/dataproxy/artifact_urn'
   _DATAPROXYSERVICE.methods_by_name['CreateDownloadLink']._options = None
   _DATAPROXYSERVICE.methods_by_name['CreateDownloadLink']._serialized_options = b'\202\323\344\223\002$:\001*\"\037/api/v1/dataproxy/artifact_link'
-  _ARTIFACTTYPE._serialized_start=1163
-  _ARTIFACTTYPE._serialized_end=1230
-  _CREATEUPLOADLOCATIONRESPONSE._serialized_start=182
-  _CREATEUPLOADLOCATIONRESPONSE._serialized_end=333
-  _CREATEUPLOADLOCATIONREQUEST._serialized_start=336
-  _CREATEUPLOADLOCATIONREQUEST._serialized_end=534
-  _CREATEDOWNLOADLOCATIONREQUEST._serialized_start=536
-  _CREATEDOWNLOADLOCATIONREQUEST._serialized_end=660
-  _CREATEDOWNLOADLOCATIONRESPONSE._serialized_start=662
-  _CREATEDOWNLOADLOCATIONRESPONSE._serialized_end=788
-  _CREATEDOWNLOADLINKREQUEST._serialized_start=791
-  _CREATEDOWNLOADLINKREQUEST._serialized_end=1041
-  _CREATEDOWNLOADLINKRESPONSE._serialized_start=1043
-  _CREATEDOWNLOADLINKRESPONSE._serialized_end=1161
-  _DATAPROXYSERVICE._serialized_start=1233
-  _DATAPROXYSERVICE._serialized_end=1741
+  _DATAPROXYSERVICE.methods_by_name['GetData']._options = None
+  _DATAPROXYSERVICE.methods_by_name['GetData']._serialized_options = b'\202\323\344\223\002\016\022\014/api/v1/data'
+  _globals['_ARTIFACTTYPE']._serialized_start=1594
+  _globals['_ARTIFACTTYPE']._serialized_end=1661
+  _globals['_CREATEUPLOADLOCATIONRESPONSE']._serialized_start=212
+  _globals['_CREATEUPLOADLOCATIONRESPONSE']._serialized_end=363
+  _globals['_CREATEUPLOADLOCATIONREQUEST']._serialized_start=366
+  _globals['_CREATEUPLOADLOCATIONREQUEST']._serialized_end=564
+  _globals['_CREATEDOWNLOADLOCATIONREQUEST']._serialized_start=566
+  _globals['_CREATEDOWNLOADLOCATIONREQUEST']._serialized_end=690
+  _globals['_CREATEDOWNLOADLOCATIONRESPONSE']._serialized_start=692
+  _globals['_CREATEDOWNLOADLOCATIONRESPONSE']._serialized_end=818
+  _globals['_CREATEDOWNLOADLINKREQUEST']._serialized_start=821
+  _globals['_CREATEDOWNLOADLINKREQUEST']._serialized_end=1071
+  _globals['_CREATEDOWNLOADLINKRESPONSE']._serialized_start=1074
+  _globals['_CREATEDOWNLOADLINKRESPONSE']._serialized_end=1273
+  _globals['_PRESIGNEDURLS']._serialized_start=1275
+  _globals['_PRESIGNEDURLS']._serialized_end=1380
+  _globals['_GETDATAREQUEST']._serialized_start=1382
+  _globals['_GETDATAREQUEST']._serialized_end=1427
+  _globals['_GETDATARESPONSE']._serialized_start=1430
+  _globals['_GETDATARESPONSE']._serialized_end=1592
+  _globals['_DATAPROXYSERVICE']._serialized_start=1664
+  _globals['_DATAPROXYSERVICE']._serialized_end=2274
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/dataproxy_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/dataproxy_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,101 @@
 from google.api import annotations_pb2 as _annotations_pb2
 from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from flyteidl.core import identifier_pb2 as _identifier_pb2
+from flyteidl.core import literals_pb2 as _literals_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
-ARTIFACT_TYPE_DECK: ArtifactType
-ARTIFACT_TYPE_UNDEFINED: ArtifactType
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CreateDownloadLinkRequest(_message.Message):
-    __slots__ = ["artifact_type", "expires_in", "node_execution_id"]
-    ARTIFACT_TYPE_FIELD_NUMBER: _ClassVar[int]
-    EXPIRES_IN_FIELD_NUMBER: _ClassVar[int]
-    NODE_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
-    artifact_type: ArtifactType
-    expires_in: _duration_pb2.Duration
-    node_execution_id: _identifier_pb2.NodeExecutionIdentifier
-    def __init__(self, artifact_type: _Optional[_Union[ArtifactType, str]] = ..., expires_in: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., node_execution_id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ...) -> None: ...
+class ArtifactType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    ARTIFACT_TYPE_UNDEFINED: _ClassVar[ArtifactType]
+    ARTIFACT_TYPE_DECK: _ClassVar[ArtifactType]
+ARTIFACT_TYPE_UNDEFINED: ArtifactType
+ARTIFACT_TYPE_DECK: ArtifactType
 
-class CreateDownloadLinkResponse(_message.Message):
-    __slots__ = ["expires_at", "signed_url"]
-    EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
+class CreateUploadLocationResponse(_message.Message):
+    __slots__ = ["signed_url", "native_url", "expires_at"]
     SIGNED_URL_FIELD_NUMBER: _ClassVar[int]
+    NATIVE_URL_FIELD_NUMBER: _ClassVar[int]
+    EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
+    signed_url: str
+    native_url: str
     expires_at: _timestamp_pb2.Timestamp
-    signed_url: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, signed_url: _Optional[_Iterable[str]] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+    def __init__(self, signed_url: _Optional[str] = ..., native_url: _Optional[str] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class CreateDownloadLocationRequest(_message.Message):
-    __slots__ = ["expires_in", "native_url"]
+class CreateUploadLocationRequest(_message.Message):
+    __slots__ = ["project", "domain", "filename", "expires_in", "content_md5"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+    FILENAME_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_IN_FIELD_NUMBER: _ClassVar[int]
-    NATIVE_URL_FIELD_NUMBER: _ClassVar[int]
+    CONTENT_MD5_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    domain: str
+    filename: str
     expires_in: _duration_pb2.Duration
+    content_md5: bytes
+    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., filename: _Optional[str] = ..., expires_in: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., content_md5: _Optional[bytes] = ...) -> None: ...
+
+class CreateDownloadLocationRequest(_message.Message):
+    __slots__ = ["native_url", "expires_in"]
+    NATIVE_URL_FIELD_NUMBER: _ClassVar[int]
+    EXPIRES_IN_FIELD_NUMBER: _ClassVar[int]
     native_url: str
+    expires_in: _duration_pb2.Duration
     def __init__(self, native_url: _Optional[str] = ..., expires_in: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
 
 class CreateDownloadLocationResponse(_message.Message):
-    __slots__ = ["expires_at", "signed_url"]
-    EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["signed_url", "expires_at"]
     SIGNED_URL_FIELD_NUMBER: _ClassVar[int]
-    expires_at: _timestamp_pb2.Timestamp
+    EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
     signed_url: str
+    expires_at: _timestamp_pb2.Timestamp
     def __init__(self, signed_url: _Optional[str] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class CreateUploadLocationRequest(_message.Message):
-    __slots__ = ["content_md5", "domain", "expires_in", "filename", "project"]
-    CONTENT_MD5_FIELD_NUMBER: _ClassVar[int]
-    DOMAIN_FIELD_NUMBER: _ClassVar[int]
+class CreateDownloadLinkRequest(_message.Message):
+    __slots__ = ["artifact_type", "expires_in", "node_execution_id"]
+    ARTIFACT_TYPE_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_IN_FIELD_NUMBER: _ClassVar[int]
-    FILENAME_FIELD_NUMBER: _ClassVar[int]
-    PROJECT_FIELD_NUMBER: _ClassVar[int]
-    content_md5: bytes
-    domain: str
+    NODE_EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    artifact_type: ArtifactType
     expires_in: _duration_pb2.Duration
-    filename: str
-    project: str
-    def __init__(self, project: _Optional[str] = ..., domain: _Optional[str] = ..., filename: _Optional[str] = ..., expires_in: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., content_md5: _Optional[bytes] = ...) -> None: ...
+    node_execution_id: _identifier_pb2.NodeExecutionIdentifier
+    def __init__(self, artifact_type: _Optional[_Union[ArtifactType, str]] = ..., expires_in: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., node_execution_id: _Optional[_Union[_identifier_pb2.NodeExecutionIdentifier, _Mapping]] = ...) -> None: ...
 
-class CreateUploadLocationResponse(_message.Message):
-    __slots__ = ["expires_at", "native_url", "signed_url"]
+class CreateDownloadLinkResponse(_message.Message):
+    __slots__ = ["signed_url", "expires_at", "pre_signed_urls"]
+    SIGNED_URL_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
-    NATIVE_URL_FIELD_NUMBER: _ClassVar[int]
+    PRE_SIGNED_URLS_FIELD_NUMBER: _ClassVar[int]
+    signed_url: _containers.RepeatedScalarFieldContainer[str]
+    expires_at: _timestamp_pb2.Timestamp
+    pre_signed_urls: PreSignedURLs
+    def __init__(self, signed_url: _Optional[_Iterable[str]] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., pre_signed_urls: _Optional[_Union[PreSignedURLs, _Mapping]] = ...) -> None: ...
+
+class PreSignedURLs(_message.Message):
+    __slots__ = ["signed_url", "expires_at"]
     SIGNED_URL_FIELD_NUMBER: _ClassVar[int]
+    EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
+    signed_url: _containers.RepeatedScalarFieldContainer[str]
     expires_at: _timestamp_pb2.Timestamp
-    native_url: str
-    signed_url: str
-    def __init__(self, signed_url: _Optional[str] = ..., native_url: _Optional[str] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+    def __init__(self, signed_url: _Optional[_Iterable[str]] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class ArtifactType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+class GetDataRequest(_message.Message):
+    __slots__ = ["flyte_url"]
+    FLYTE_URL_FIELD_NUMBER: _ClassVar[int]
+    flyte_url: str
+    def __init__(self, flyte_url: _Optional[str] = ...) -> None: ...
+
+class GetDataResponse(_message.Message):
+    __slots__ = ["literal_map", "pre_signed_urls"]
+    LITERAL_MAP_FIELD_NUMBER: _ClassVar[int]
+    PRE_SIGNED_URLS_FIELD_NUMBER: _ClassVar[int]
+    literal_map: _literals_pb2.LiteralMap
+    pre_signed_urls: PreSignedURLs
+    def __init__(self, literal_map: _Optional[_Union[_literals_pb2.LiteralMap, _Mapping]] = ..., pre_signed_urls: _Optional[_Union[PreSignedURLs, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/identity_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/identity_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66lyteidl/service/identity.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\"\x11\n\x0fUserInfoRequest\"\xdf\x01\n\x10UserInfoResponse\x12\x18\n\x07subject\x18\x01 \x01(\tR\x07subject\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12-\n\x12preferred_username\x18\x03 \x01(\tR\x11preferredUsername\x12\x1d\n\ngiven_name\x18\x04 \x01(\tR\tgivenName\x12\x1f\n\x0b\x66\x61mily_name\x18\x05 \x01(\tR\nfamilyName\x12\x14\n\x05\x65mail\x18\x06 \x01(\tR\x05\x65mail\x12\x18\n\x07picture\x18\x07 \x01(\tR\x07picture2q\n\x0fIdentityService\x12^\n\x08UserInfo\x12!.flyteidl.service.UserInfoRequest\x1a\".flyteidl.service.UserInfoResponse\"\x0b\x82\xd3\xe4\x93\x02\x05\x12\x03/meB\xbf\x01\n\x14\x63om.flyteidl.serviceB\rIdentityProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66lyteidl/service/identity.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x11\n\x0fUserInfoRequest\"\xa5\x02\n\x10UserInfoResponse\x12\x18\n\x07subject\x18\x01 \x01(\tR\x07subject\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12-\n\x12preferred_username\x18\x03 \x01(\tR\x11preferredUsername\x12\x1d\n\ngiven_name\x18\x04 \x01(\tR\tgivenName\x12\x1f\n\x0b\x66\x61mily_name\x18\x05 \x01(\tR\nfamilyName\x12\x14\n\x05\x65mail\x18\x06 \x01(\tR\x05\x65mail\x12\x18\n\x07picture\x18\x07 \x01(\tR\x07picture\x12\x44\n\x11\x61\x64\x64itional_claims\x18\x08 \x01(\x0b\x32\x17.google.protobuf.StructR\x10\x61\x64\x64itionalClaims2q\n\x0fIdentityService\x12^\n\x08UserInfo\x12!.flyteidl.service.UserInfoRequest\x1a\".flyteidl.service.UserInfoResponse\"\x0b\x82\xd3\xe4\x93\x02\x05\x12\x03/meB\xbf\x01\n\x14\x63om.flyteidl.serviceB\rIdentityProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.identity_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.identity_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.serviceB\rIdentityProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\242\002\003FSX\252\002\020Flyteidl.Service\312\002\020Flyteidl\\Service\342\002\034Flyteidl\\Service\\GPBMetadata\352\002\021Flyteidl::Service'
   _IDENTITYSERVICE.methods_by_name['UserInfo']._options = None
   _IDENTITYSERVICE.methods_by_name['UserInfo']._serialized_options = b'\202\323\344\223\002\005\022\003/me'
-  _USERINFOREQUEST._serialized_start=83
-  _USERINFOREQUEST._serialized_end=100
-  _USERINFORESPONSE._serialized_start=103
-  _USERINFORESPONSE._serialized_end=326
-  _IDENTITYSERVICE._serialized_start=328
-  _IDENTITYSERVICE._serialized_end=441
+  _globals['_USERINFOREQUEST']._serialized_start=113
+  _globals['_USERINFOREQUEST']._serialized_end=130
+  _globals['_USERINFORESPONSE']._serialized_start=133
+  _globals['_USERINFORESPONSE']._serialized_end=426
+  _globals['_IDENTITYSERVICE']._serialized_start=428
+  _globals['_IDENTITYSERVICE']._serialized_end=541
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/identity_pb2.pyi` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/identity_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from google.api import annotations_pb2 as _annotations_pb2
+from google.protobuf import struct_pb2 as _struct_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class UserInfoRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class UserInfoResponse(_message.Message):
-    __slots__ = ["email", "family_name", "given_name", "name", "picture", "preferred_username", "subject"]
-    EMAIL_FIELD_NUMBER: _ClassVar[int]
-    FAMILY_NAME_FIELD_NUMBER: _ClassVar[int]
-    GIVEN_NAME_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["subject", "name", "preferred_username", "given_name", "family_name", "email", "picture", "additional_claims"]
+    SUBJECT_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    PICTURE_FIELD_NUMBER: _ClassVar[int]
     PREFERRED_USERNAME_FIELD_NUMBER: _ClassVar[int]
-    SUBJECT_FIELD_NUMBER: _ClassVar[int]
-    email: str
-    family_name: str
-    given_name: str
+    GIVEN_NAME_FIELD_NUMBER: _ClassVar[int]
+    FAMILY_NAME_FIELD_NUMBER: _ClassVar[int]
+    EMAIL_FIELD_NUMBER: _ClassVar[int]
+    PICTURE_FIELD_NUMBER: _ClassVar[int]
+    ADDITIONAL_CLAIMS_FIELD_NUMBER: _ClassVar[int]
+    subject: str
     name: str
-    picture: str
     preferred_username: str
-    subject: str
-    def __init__(self, subject: _Optional[str] = ..., name: _Optional[str] = ..., preferred_username: _Optional[str] = ..., given_name: _Optional[str] = ..., family_name: _Optional[str] = ..., email: _Optional[str] = ..., picture: _Optional[str] = ...) -> None: ...
+    given_name: str
+    family_name: str
+    email: str
+    picture: str
+    additional_claims: _struct_pb2.Struct
+    def __init__(self, subject: _Optional[str] = ..., name: _Optional[str] = ..., preferred_username: _Optional[str] = ..., given_name: _Optional[str] = ..., family_name: _Optional[str] = ..., email: _Optional[str] = ..., picture: _Optional[str] = ..., additional_claims: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...) -> None: ...
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/identity_pb2_grpc.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/identity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/signal_pb2.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/core/catalog_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flyteidl/service/signal.proto
+# source: flyteidl/core/catalog.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from flyteidl.admin import signal_pb2 as flyteidl_dot_admin_dot_signal__pb2
+from flyteidl.core import identifier_pb2 as flyteidl_dot_core_dot_identifier__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66lyteidl/service/signal.proto\x12\x10\x66lyteidl.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1b\x66lyteidl/admin/signal.proto2\x9a\x03\n\rSignalService\x12W\n\x11GetOrCreateSignal\x12(.flyteidl.admin.SignalGetOrCreateRequest\x1a\x16.flyteidl.admin.Signal\"\x00\x12\xc1\x01\n\x0bListSignals\x12!.flyteidl.admin.SignalListRequest\x1a\x1a.flyteidl.admin.SignalList\"s\x82\xd3\xe4\x93\x02m\x12k/api/v1/signals/{workflow_execution_id.project}/{workflow_execution_id.domain}/{workflow_execution_id.name}\x12l\n\tSetSignal\x12 .flyteidl.admin.SignalSetRequest\x1a!.flyteidl.admin.SignalSetResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/api/v1/signalsB\xbd\x01\n\x14\x63om.flyteidl.serviceB\x0bSignalProtoP\x01Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\xa2\x02\x03\x46SX\xaa\x02\x10\x46lyteidl.Service\xca\x02\x10\x46lyteidl\\Service\xe2\x02\x1c\x46lyteidl\\Service\\GPBMetadata\xea\x02\x11\x46lyteidl::Serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66lyteidl/core/catalog.proto\x12\rflyteidl.core\x1a\x1e\x66lyteidl/core/identifier.proto\"I\n\x12\x43\x61talogArtifactTag\x12\x1f\n\x0b\x61rtifact_id\x18\x01 \x01(\tR\nartifactId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"\x83\x02\n\x0f\x43\x61talogMetadata\x12\x38\n\ndataset_id\x18\x01 \x01(\x0b\x32\x19.flyteidl.core.IdentifierR\tdatasetId\x12\x44\n\x0c\x61rtifact_tag\x18\x02 \x01(\x0b\x32!.flyteidl.core.CatalogArtifactTagR\x0b\x61rtifactTag\x12\\\n\x15source_task_execution\x18\x03 \x01(\x0b\x32&.flyteidl.core.TaskExecutionIdentifierH\x00R\x13sourceTaskExecutionB\x12\n\x10source_execution\"\x9e\x01\n\x12\x43\x61talogReservation\"\x87\x01\n\x06Status\x12\x18\n\x14RESERVATION_DISABLED\x10\x00\x12\x18\n\x14RESERVATION_ACQUIRED\x10\x01\x12\x16\n\x12RESERVATION_EXISTS\x10\x02\x12\x18\n\x14RESERVATION_RELEASED\x10\x03\x12\x17\n\x13RESERVATION_FAILURE\x10\x04*\xa0\x01\n\x12\x43\x61talogCacheStatus\x12\x12\n\x0e\x43\x41\x43HE_DISABLED\x10\x00\x12\x0e\n\nCACHE_MISS\x10\x01\x12\r\n\tCACHE_HIT\x10\x02\x12\x13\n\x0f\x43\x41\x43HE_POPULATED\x10\x03\x12\x18\n\x14\x43\x41\x43HE_LOOKUP_FAILURE\x10\x04\x12\x15\n\x11\x43\x41\x43HE_PUT_FAILURE\x10\x05\x12\x11\n\rCACHE_SKIPPED\x10\x06\x42\xac\x01\n\x11\x63om.flyteidl.coreB\x0c\x43\x61talogProtoP\x01Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\xa2\x02\x03\x46\x43X\xaa\x02\rFlyteidl.Core\xca\x02\rFlyteidl\\Core\xe2\x02\x19\x46lyteidl\\Core\\GPBMetadata\xea\x02\x0e\x46lyteidl::Coreb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.service.signal_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flyteidl.core.catalog_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\024com.flyteidl.serviceB\013SignalProtoP\001Z7github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/service\242\002\003FSX\252\002\020Flyteidl.Service\312\002\020Flyteidl\\Service\342\002\034Flyteidl\\Service\\GPBMetadata\352\002\021Flyteidl::Service'
-  _SIGNALSERVICE.methods_by_name['ListSignals']._options = None
-  _SIGNALSERVICE.methods_by_name['ListSignals']._serialized_options = b'\202\323\344\223\002m\022k/api/v1/signals/{workflow_execution_id.project}/{workflow_execution_id.domain}/{workflow_execution_id.name}'
-  _SIGNALSERVICE.methods_by_name['SetSignal']._options = None
-  _SIGNALSERVICE.methods_by_name['SetSignal']._serialized_options = b'\202\323\344\223\002\024:\001*\"\017/api/v1/signals'
-  _SIGNALSERVICE._serialized_start=111
-  _SIGNALSERVICE._serialized_end=521
+  DESCRIPTOR._serialized_options = b'\n\021com.flyteidl.coreB\014CatalogProtoP\001Z4github.com/flyteorg/flyteidl/gen/pb-go/flyteidl/core\242\002\003FCX\252\002\rFlyteidl.Core\312\002\rFlyteidl\\Core\342\002\031Flyteidl\\Core\\GPBMetadata\352\002\016Flyteidl::Core'
+  _globals['_CATALOGCACHESTATUS']._serialized_start=577
+  _globals['_CATALOGCACHESTATUS']._serialized_end=737
+  _globals['_CATALOGARTIFACTTAG']._serialized_start=78
+  _globals['_CATALOGARTIFACTTAG']._serialized_end=151
+  _globals['_CATALOGMETADATA']._serialized_start=154
+  _globals['_CATALOGMETADATA']._serialized_end=413
+  _globals['_CATALOGRESERVATION']._serialized_start=416
+  _globals['_CATALOGRESERVATION']._serialized_end=574
+  _globals['_CATALOGRESERVATION_STATUS']._serialized_start=439
+  _globals['_CATALOGRESERVATION_STATUS']._serialized_end=574
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl/service/signal_pb2_grpc.py` & `flyteidl-1.5.0/gen/pb_python/flyteidl/service/signal_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/gen/pb_python/flyteidl.egg-info/SOURCES.txt` & `flyteidl-1.5.0/gen/pb_python/flyteidl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 gen/pb_python/flyteidl/core/identifier_pb2_grpc.py
 gen/pb_python/flyteidl/core/interface_pb2.py
 gen/pb_python/flyteidl/core/interface_pb2.pyi
 gen/pb_python/flyteidl/core/interface_pb2_grpc.py
 gen/pb_python/flyteidl/core/literals_pb2.py
 gen/pb_python/flyteidl/core/literals_pb2.pyi
 gen/pb_python/flyteidl/core/literals_pb2_grpc.py
+gen/pb_python/flyteidl/core/metrics_pb2.py
+gen/pb_python/flyteidl/core/metrics_pb2.pyi
+gen/pb_python/flyteidl/core/metrics_pb2_grpc.py
 gen/pb_python/flyteidl/core/security_pb2.py
 gen/pb_python/flyteidl/core/security_pb2.pyi
 gen/pb_python/flyteidl/core/security_pb2_grpc.py
 gen/pb_python/flyteidl/core/tasks_pb2.py
 gen/pb_python/flyteidl/core/tasks_pb2.pyi
 gen/pb_python/flyteidl/core/tasks_pb2_grpc.py
 gen/pb_python/flyteidl/core/types_pb2.py
@@ -165,14 +168,17 @@
 gen/pb_python/flyteidl/service/admin_pb2_grpc.py
 gen/pb_python/flyteidl/service/auth_pb2.py
 gen/pb_python/flyteidl/service/auth_pb2.pyi
 gen/pb_python/flyteidl/service/auth_pb2_grpc.py
 gen/pb_python/flyteidl/service/dataproxy_pb2.py
 gen/pb_python/flyteidl/service/dataproxy_pb2.pyi
 gen/pb_python/flyteidl/service/dataproxy_pb2_grpc.py
+gen/pb_python/flyteidl/service/external_plugin_service_pb2.py
+gen/pb_python/flyteidl/service/external_plugin_service_pb2.pyi
+gen/pb_python/flyteidl/service/external_plugin_service_pb2_grpc.py
 gen/pb_python/flyteidl/service/identity_pb2.py
 gen/pb_python/flyteidl/service/identity_pb2.pyi
 gen/pb_python/flyteidl/service/identity_pb2_grpc.py
 gen/pb_python/flyteidl/service/signal_pb2.py
 gen/pb_python/flyteidl/service/signal_pb2.pyi
 gen/pb_python/flyteidl/service/signal_pb2_grpc.py
 gen/pb_python/validate/__init__.py
```

### Comparing `flyteidl-1.4.2/gen/pb_python/validate/validate_pb2.py` & `flyteidl-1.5.0/gen/pb_python/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/setup.cfg` & `flyteidl-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flyteidl-1.4.2/setup.py` & `flyteidl-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = "1.4.2"
+__version__ = "1.5.0"
 
 setup(
     name='flyteidl',
     version=__version__,
     description='IDL for Flyte Platform',
     url='https://www.github.com/flyteorg/flyteidl',
     maintainer='FlyteOrg',
```

