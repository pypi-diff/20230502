# Comparing `tmp/preemo_worker_sdk-0.5.1.tar.gz` & `tmp/preemo_worker_sdk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preemo_worker_sdk-0.5.1.tar", max compression
+gzip compressed data, was "preemo_worker_sdk-0.5.2.tar", max compression
```

## Comparing `preemo_worker_sdk-0.5.1.tar` & `preemo_worker_sdk-0.5.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.5.1/LICENSE
--rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.5.1/README.md
--rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.5.1/preemo/__init__.py
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057207 preemo_worker_sdk-0.5.1/preemo/gen/__init__.py
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057418 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/__init__.py
--rw-r--r--   0        0        0     4333 2023-04-25 19:46:41.903033 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py
--rw-r--r--   0        0        0     7285 2023-04-25 19:46:42.071630 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi
--rw-r--r--   0        0        0     3035 2023-04-25 19:46:41.903159 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_create_artifact_pb2.py
--rw-r--r--   0        0        0     6629 2023-04-25 19:46:42.078426 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
--rw-r--r--   0        0        0     2642 2023-04-25 19:46:41.903266 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_execute_function_pb2.py
--rw-r--r--   0        0        0     4134 2023-04-25 19:46:42.084193 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_execute_function_pb2.pyi
--rw-r--r--   0        0        0     2837 2023-04-25 19:46:41.903373 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
--rw-r--r--   0        0        0     5106 2023-04-25 19:46:42.090178 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
--rw-r--r--   0        0        0     4502 2023-04-25 19:46:41.903470 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py
--rw-r--r--   0        0        0     7767 2023-04-25 19:46:42.099799 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-04-25 19:46:41.903560 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_pb2.py
--rw-r--r--   0        0        0     5686 2023-04-25 19:46:42.109202 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
--rw-r--r--   0        0        0     4409 2023-04-25 19:46:41.903662 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py
--rw-r--r--   0        0        0     7699 2023-04-25 19:46:42.117663 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi
--rw-r--r--   0        0        0     1382 2023-04-25 19:46:41.903764 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/check_function_pb2.py
--rw-r--r--   0        0        0     1811 2023-04-25 19:46:42.125765 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/check_function_pb2.pyi
--rw-r--r--   0        0        0     1665 2023-04-25 19:46:41.903852 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/execute_function_pb2.py
--rw-r--r--   0        0        0     3019 2023-04-25 19:46:42.133597 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/execute_function_pb2.pyi
--rw-r--r--   0        0        0     1128 2023-04-25 19:46:41.903952 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/header_pb2.py
--rw-r--r--   0        0        0     1515 2023-04-25 19:46:42.148610 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/header_pb2.pyi
--rw-r--r--   0        0        0     1403 2023-04-25 19:46:41.904045 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/register_function_pb2.py
--rw-r--r--   0        0        0     1721 2023-04-25 19:46:42.158689 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/register_function_pb2.pyi
--rw-r--r--   0        0        0     1130 2023-05-01 17:44:07.185317 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/sdk_server_ready_pb2.py
--rw-r--r--   0        0        0      816 2023-05-01 17:44:07.185506 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
--rw-r--r--   0        0        0     1085 2023-04-25 19:46:41.904240 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/terminate_pb2.py
--rw-r--r--   0        0        0      786 2023-04-25 19:46:42.174637 preemo_worker_sdk-0.5.1/preemo/gen/endpoints/terminate_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057965 preemo_worker_sdk-0.5.1/preemo/gen/models/__init__.py
--rw-r--r--   0        0        0     1104 2023-04-25 19:46:41.904364 preemo_worker_sdk-0.5.1/preemo/gen/models/artifact_type_pb2.py
--rw-r--r--   0        0        0     1129 2023-04-25 19:46:42.181218 preemo_worker_sdk-0.5.1/preemo/gen/models/artifact_type_pb2.pyi
--rw-r--r--   0        0        0     1135 2023-04-25 19:46:41.904467 preemo_worker_sdk-0.5.1/preemo/gen/models/registered_function_pb2.py
--rw-r--r--   0        0        0     1624 2023-04-25 19:46:42.189956 preemo_worker_sdk-0.5.1/preemo/gen/models/registered_function_pb2.pyi
--rw-r--r--   0        0        0     1174 2023-04-25 19:46:41.904568 preemo_worker_sdk-0.5.1/preemo/gen/models/value_pb2.py
--rw-r--r--   0        0        0     1396 2023-04-25 19:46:42.196623 preemo_worker_sdk-0.5.1/preemo/gen/models/value_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.058182 preemo_worker_sdk-0.5.1/preemo/gen/services/__init__.py
--rw-r--r--   0        0        0     4369 2023-04-25 19:46:42.046773 preemo_worker_sdk-0.5.1/preemo/gen/services/sdk_pb2_grpc.py
--rw-r--r--   0        0        0     1302 2023-04-25 19:46:42.206915 preemo_worker_sdk-0.5.1/preemo/gen/services/sdk_pb2_grpc.pyi
--rw-r--r--   0        0        0    21861 2023-04-25 19:46:42.047102 preemo_worker_sdk-0.5.1/preemo/gen/services/worker_pb2_grpc.py
--rw-r--r--   0        0        0     6536 2023-04-25 19:46:42.216498 preemo_worker_sdk-0.5.1/preemo/gen/services/worker_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.5.1/preemo/py.typed
--rw-r--r--   0        0        0     2500 2023-05-01 17:44:07.185692 preemo_worker_sdk-0.5.1/preemo/worker/__init__.py
--rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.5.1/preemo/worker/__init__.pyi
--rw-r--r--   0        0        0    13253 2023-05-01 17:44:07.186213 preemo_worker_sdk-0.5.1/preemo/worker/_artifact_manager.py
--rw-r--r--   0        0        0     1959 2023-05-01 17:44:07.186566 preemo_worker_sdk-0.5.1/preemo/worker/_env_manager.py
--rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.5.1/preemo/worker/_function_registry.py
--rw-r--r--   0        0        0    11315 2023-04-21 16:59:41.872373 preemo_worker_sdk-0.5.1/preemo/worker/_messaging_client.py
--rw-r--r--   0        0        0     1394 2023-05-01 17:44:07.186878 preemo_worker_sdk-0.5.1/preemo/worker/_sdk_server.py
--rw-r--r--   0        0        0     3581 2023-04-21 16:59:41.872685 preemo_worker_sdk-0.5.1/preemo/worker/_sdk_service.py
--rw-r--r--   0        0        0     1286 2023-04-25 19:43:44.759473 preemo_worker_sdk-0.5.1/preemo/worker/_types.py
--rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.5.1/preemo/worker/_validation.py
--rw-r--r--   0        0        0     7044 2023-04-21 16:59:41.872944 preemo_worker_sdk-0.5.1/preemo/worker/_worker_client.py
--rw-r--r--   0        0        0     1852 2023-05-01 17:44:07.187350 preemo_worker_sdk-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.5.2/README.md
+-rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.5.2/preemo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057207 preemo_worker_sdk-0.5.2/preemo/gen/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057418 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/__init__.py
+-rw-r--r--   0        0        0     4333 2023-04-25 19:46:41.903033 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py
+-rw-r--r--   0        0        0     7285 2023-04-25 19:46:42.071630 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi
+-rw-r--r--   0        0        0     3035 2023-04-25 19:46:41.903159 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.py
+-rw-r--r--   0        0        0     6629 2023-04-25 19:46:42.078426 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
+-rw-r--r--   0        0        0     2642 2023-04-25 19:46:41.903266 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.py
+-rw-r--r--   0        0        0     4134 2023-04-25 19:46:42.084193 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.pyi
+-rw-r--r--   0        0        0     2837 2023-04-25 19:46:41.903373 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
+-rw-r--r--   0        0        0     5106 2023-04-25 19:46:42.090178 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4502 2023-04-25 19:46:41.903470 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py
+-rw-r--r--   0        0        0     7767 2023-04-25 19:46:42.099799 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-04-25 19:46:41.903560 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.py
+-rw-r--r--   0        0        0     5686 2023-04-25 19:46:42.109202 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4409 2023-04-25 19:46:41.903662 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py
+-rw-r--r--   0        0        0     7699 2023-04-25 19:46:42.117663 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi
+-rw-r--r--   0        0        0     1382 2023-04-25 19:46:41.903764 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.py
+-rw-r--r--   0        0        0     1811 2023-04-25 19:46:42.125765 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.pyi
+-rw-r--r--   0        0        0     1665 2023-04-25 19:46:41.903852 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.py
+-rw-r--r--   0        0        0     3019 2023-04-25 19:46:42.133597 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.pyi
+-rw-r--r--   0        0        0     1128 2023-04-25 19:46:41.903952 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.py
+-rw-r--r--   0        0        0     1515 2023-04-25 19:46:42.148610 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.pyi
+-rw-r--r--   0        0        0     1403 2023-04-25 19:46:41.904045 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/register_function_pb2.py
+-rw-r--r--   0        0        0     1721 2023-04-25 19:46:42.158689 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/register_function_pb2.pyi
+-rw-r--r--   0        0        0     1130 2023-05-01 17:44:07.185317 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.py
+-rw-r--r--   0        0        0      816 2023-05-01 17:44:07.185506 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
+-rw-r--r--   0        0        0     1085 2023-04-25 19:46:41.904240 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.py
+-rw-r--r--   0        0        0      786 2023-04-25 19:46:42.174637 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057965 preemo_worker_sdk-0.5.2/preemo/gen/models/__init__.py
+-rw-r--r--   0        0        0     1104 2023-04-25 19:46:41.904364 preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.py
+-rw-r--r--   0        0        0     1129 2023-04-25 19:46:42.181218 preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.pyi
+-rw-r--r--   0        0        0     1135 2023-04-25 19:46:41.904467 preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.py
+-rw-r--r--   0        0        0     1624 2023-04-25 19:46:42.189956 preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.pyi
+-rw-r--r--   0        0        0     1174 2023-04-25 19:46:41.904568 preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.py
+-rw-r--r--   0        0        0     1396 2023-04-25 19:46:42.196623 preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-25 19:46:42.058182 preemo_worker_sdk-0.5.2/preemo/gen/services/__init__.py
+-rw-r--r--   0        0        0     4369 2023-04-25 19:46:42.046773 preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.py
+-rw-r--r--   0        0        0     1302 2023-04-25 19:46:42.206915 preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.pyi
+-rw-r--r--   0        0        0    21861 2023-04-25 19:46:42.047102 preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.py
+-rw-r--r--   0        0        0     6536 2023-04-25 19:46:42.216498 preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.5.2/preemo/py.typed
+-rw-r--r--   0        0        0     2500 2023-05-01 17:44:07.185692 preemo_worker_sdk-0.5.2/preemo/worker/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.5.2/preemo/worker/__init__.pyi
+-rw-r--r--   0        0        0    13624 2023-05-02 18:39:31.234171 preemo_worker_sdk-0.5.2/preemo/worker/_artifact_manager.py
+-rw-r--r--   0        0        0     1959 2023-05-01 17:44:07.186566 preemo_worker_sdk-0.5.2/preemo/worker/_env_manager.py
+-rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.5.2/preemo/worker/_function_registry.py
+-rw-r--r--   0        0        0    11315 2023-04-21 16:59:41.872373 preemo_worker_sdk-0.5.2/preemo/worker/_messaging_client.py
+-rw-r--r--   0        0        0     1394 2023-05-01 17:44:07.186878 preemo_worker_sdk-0.5.2/preemo/worker/_sdk_server.py
+-rw-r--r--   0        0        0     3581 2023-04-21 16:59:41.872685 preemo_worker_sdk-0.5.2/preemo/worker/_sdk_service.py
+-rw-r--r--   0        0        0     1286 2023-04-25 19:43:44.759473 preemo_worker_sdk-0.5.2/preemo/worker/_types.py
+-rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.5.2/preemo/worker/_validation.py
+-rw-r--r--   0        0        0     7044 2023-04-21 16:59:41.872944 preemo_worker_sdk-0.5.2/preemo/worker/_worker_client.py
+-rw-r--r--   0        0        0     1852 2023-05-02 21:07:16.127981 preemo_worker_sdk-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.5.2/PKG-INFO
```

### Comparing `preemo_worker_sdk-0.5.1/LICENSE` & `preemo_worker_sdk-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/README.md` & `preemo_worker_sdk-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_create_artifact_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_create_artifact_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_execute_function_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_execute_function_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/check_function_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/check_function_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/execute_function_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/execute_function_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/header_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/header_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/register_function_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/register_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/register_function_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/register_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/sdk_server_ready_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/sdk_server_ready_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/terminate_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/endpoints/terminate_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/models/artifact_type_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/models/artifact_type_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/models/registered_function_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/models/registered_function_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/models/value_pb2.py` & `preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/models/value_pb2.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/services/sdk_pb2_grpc.py` & `preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/services/sdk_pb2_grpc.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/services/worker_pb2_grpc.py` & `preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/gen/services/worker_pb2_grpc.pyi` & `preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/__init__.py` & `preemo_worker_sdk-0.5.2/preemo/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/__init__.pyi` & `preemo_worker_sdk-0.5.2/preemo/worker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_artifact_manager.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_artifact_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import concurrent.futures
 import enum
+import gzip
 import math
+import os
 from typing import Dict, List, Protocol, runtime_checkable
 
 import requests
 from pydantic import StrictInt
 
 from preemo.gen.endpoints.batch_allocate_artifact_part_pb2 import (
     AllocateArtifactPartConfig,
@@ -83,37 +85,45 @@
         *,
         messaging_client: IMessagingClient,
     ) -> None:
         self._messaging_client = messaging_client
 
     def _write_content(self, *, content: memoryview, url: str) -> None:
         if EnvManager.is_development:
-            import os
-
             # treat url as file path
             os.makedirs(os.path.dirname(url), exist_ok=True)
             with open(url, "wb") as fout:
                 fout.write(content)
         else:
-            # TODO(adrian@preemo.io, 04/11/2023): might be post
             response = requests.put(
-                url=url, data=content, headers={"Content-Encoding": "gzip"}
+                url=url,
+                data=gzip.compress(content),
+                headers={
+                    "Content-Encoding": "gzip",
+                    "Content-Type": "application/octet-stream",
+                },
             )
 
             # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
             if not response.ok:
                 raise Exception(f"unexpected response while uploading: {response}")
 
     def _read_content(self, *, url: str) -> bytes:
         if EnvManager.is_development:
             # treat url as file path
             with open(url, "rb") as fin:
                 return fin.read()
         else:
-            response = requests.get(url=url, headers={"Accept-Encoding": "gzip"})
+            response = requests.get(
+                url=url,
+                headers={
+                    "Accept-Encoding": "gzip",
+                    "Content-Type": "application/octet-stream",
+                },
+            )
 
             # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
             if not response.ok:
                 raise Exception(f"unexpected response while downloading: {response}")
 
             return response.content
 
@@ -230,14 +240,18 @@
 
             if len(not_done) != 0:
                 raise Exception("expected incomplete future set to be empty")
 
             if len(done) != len(futures):
                 raise Exception("expected all futures to have completed")
 
+            for future in done:
+                # this will raise any exceptions raised in the thread
+                future.result()
+
         self._messaging_client.batch_finalize_artifact(
             BatchFinalizeArtifactRequest(
                 configs_by_artifact_id={
                     artifact.id.value: FinalizeArtifactConfig(
                         total_size=len(content),
                         part_count=ArtifactManager._calculate_part_count(
                             content_length=len(content),
```

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_env_manager.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_env_manager.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_function_registry.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_function_registry.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_messaging_client.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_messaging_client.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_sdk_server.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_sdk_server.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_sdk_service.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_sdk_service.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_types.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_types.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_validation.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_validation.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/preemo/worker/_worker_client.py` & `preemo_worker_sdk-0.5.2/preemo/worker/_worker_client.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.1/pyproject.toml` & `preemo_worker_sdk-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "preemo_worker_sdk"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 license = "MIT"
 authors = [
   "Forrest Moret <forrest@preemo.io>",
   "Adrian Miguel <adrian@preemo.io>",
 ]
 readme = "README.md"
```

### Comparing `preemo_worker_sdk-0.5.1/PKG-INFO` & `preemo_worker_sdk-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preemo-worker-sdk
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Home-page: https://www.preemo.io/
 License: MIT
 Author: Forrest Moret
 Author-email: forrest@preemo.io
 Requires-Python: >=3.8.13,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

