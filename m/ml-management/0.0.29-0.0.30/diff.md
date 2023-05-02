# Comparing `tmp/ml-management-0.0.29.tar.gz` & `tmp/ml-management-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.29.tar", last modified: Thu Apr 13 06:27:53 2023, max compression
+gzip compressed data, was "ml-management-0.0.30.tar", last modified: Tue May  2 17:28:10 2023, max compression
```

## Comparing `ml-management-0.0.29.tar` & `ml-management-0.0.30.tar`

### file list

```diff
@@ -1,47 +1,61 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/
--rw-rw-r--   0 user      (1001) user      (1001)       18 2023-02-14 12:40:10.000000 ml-management-0.0.29/MANIFEST.in
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.665418 ml-management-0.0.29/ML_management/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.665418 ml-management-0.0.29/ML_management/dataset/
--rw-rw-r--   0 user      (1001) user      (1001)     1298 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/Dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)      190 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      330 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/datamodel.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.665418 ml-management-0.0.29/ML_management/dataset/dummy_dataset/
--rw-rw-r--   0 user      (1001) user      (1001)      560 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/dummy_dataset/DummyDataset.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/dummy_dataset/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/dataset/s3_dataset/
--rw-rw-r--   0 user      (1001) user      (1001)    10399 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/dataset/s3_dataset/S3Dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/dataset/s3_dataset/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/mlmanagement/
--rw-rw-r--   0 user      (1001) user      (1001)      581 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3392 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 user      (1001) user      (1001)     5054 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 user      (1001) user      (1001)    11679 2023-04-04 08:31:43.000000 ml-management-0.0.29/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 user      (1001) user      (1001)     7792 2023-04-04 08:32:07.000000 ml-management-0.0.29/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 user      (1001) user      (1001)     2986 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/mlmanagement/server_mlmanager_exceptions.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/models/
--rw-rw-r--   0 user      (1001) user      (1001)      930 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/RetrainableModel.py
--rw-rw-r--   0 user      (1001) user      (1001)      824 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/TrainableModel.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      238 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/action_type.py
--rw-rw-r--   0 user      (1001) user      (1001)      360 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/models/function_name_to_tag.py
--rw-rw-r--   0 user      (1001) user      (1001)     2430 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/models/model_pattern.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/registry/
--rw-rw-r--   0 user      (1001) user      (1001)     7552 2023-04-04 08:31:43.000000 ml-management-0.0.29/ML_management/registry/RegistryManager.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/registry/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     2483 2023-04-04 08:28:47.000000 ml-management-0.0.29/ML_management/registry/exceptions.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ML_management/tests/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/tests/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3361 2023-02-14 12:40:10.000000 ml-management-0.0.29/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 user      (1001) user      (1001)     9508 2023-04-04 08:31:43.000000 ml-management-0.0.29/ML_management/tests/test_s3_dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)      367 2023-04-13 06:27:53.669418 ml-management-0.0.29/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       56 2023-02-14 12:40:10.000000 ml-management-0.0.29/README.md
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-04-13 06:25:51.000000 ml-management-0.0.29/VERSION
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-13 06:27:53.669418 ml-management-0.0.29/ml_management.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      367 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)     1290 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)      111 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       14 2023-04-13 06:27:53.000000 ml-management-0.0.29/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-04-13 06:27:53.669418 ml-management-0.0.29/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     1062 2023-02-14 12:40:10.000000 ml-management-0.0.29/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/
+-rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-04-17 13:42:26.000000 ml-management-0.0.30/MANIFEST.in
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.30/ML_management/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/dataset/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      191 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      330 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/dataset/datamodel.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1298 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/dataset.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/dataset/dummy_dataset/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/dataset/dummy_dataset/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      560 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/dummy_dataset/dummy_dataset.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/dataset/s3_dataset/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/dataset/s3_dataset/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    10399 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/s3_dataset/s3dataset.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/executor_template/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4592 2023-04-28 13:10:54.000000 ml-management-0.0.30/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      401 2023-04-28 11:28:11.000000 ml-management-0.0.30/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/mlmanagement/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      581 2023-04-26 06:58:05.000000 ml-management-0.0.30/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    11676 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     9478 2023-05-02 08:26:15.000000 ml-management-0.0.30/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      163 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-02 11:36:10.000000 ml-management-0.0.30/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      261 2023-04-28 08:12:41.000000 ml-management-0.0.30/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/models/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.30/ML_management/models/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/models/patterns/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4365 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/registry/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.30/ML_management/registry/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-04-28 08:49:51.000000 ml-management-0.0.30/ML_management/registry/exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/tests/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/tests/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     9508 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/tests/test_s3_dataset.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-02 17:28:10.288478 ml-management-0.0.30/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)       56 2022-11-02 13:55:55.000000 ml-management-0.0.30/README.md
+-rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-05-02 17:22:45.000000 ml-management-0.0.30/VERSION
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ml_management.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1938 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)      142 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-02 17:28:10.288478 ml-management-0.0.30/setup.cfg
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1030 2023-04-28 06:57:33.000000 ml-management-0.0.30/setup.py
```

### Comparing `ml-management-0.0.29/ML_management/dataset/Dataset.py` & `ml-management-0.0.30/ML_management/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.29/ML_management/dataset/dummy_dataset/DummyDataset.py` & `ml-management-0.0.30/ML_management/dataset/dummy_dataset/dummy_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Dummy dataset inherited from the base abstract class."""
 from ML_management.dataset.datamodel import DatasetFlavour
-from ML_management.dataset.Dataset import Dataset
+from ML_management.dataset.dataset import Dataset
 
 
 class DummyDataset(Dataset):
     """Implementation of DummyLoader Dataset."""
 
     def get_json_schema(self):
         """Return empty json schema."""
```

### Comparing `ml-management-0.0.29/ML_management/dataset/s3_dataset/S3Dataset.py` & `ml-management-0.0.30/ML_management/dataset/s3_dataset/s3dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import posixpath
 from typing import List, Optional, Union
 
 from boto3 import client
 from botocore.exceptions import ClientError
 from ML_management.dataset.datamodel import DatasetFlavour
-from ML_management.dataset.Dataset import Dataset
+from ML_management.dataset.dataset import Dataset
 
 
 class S3FolderNotFound(Exception):
     """Define Version Not Found Exception."""
 
     def __init__(self, path: str, bucket: str):
         self.path = path
```

### Comparing `ml-management-0.0.29/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.30/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.29/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.30/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.29/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.30/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.29/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.30/ML_management/mlmanagement/mlmanagement.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 import io
 import os
 import tempfile
 import zipfile
 from typing import Any, Dict, List, Optional, Union
 
 import pandas
-from ML_management.mlmanagement import mlmanager
-from ML_management.mlmanagement.mlmanager import active_run_stack, is_server, request_for_function
+from ML_management.executor_template.upload_model_mode import UploadModelMode
+from ML_management.mlmanagement import utils
+from ML_management.mlmanagement.mlmanager import request_for_function
+from ML_management.mlmanagement.utils import active_run_stack, is_server
 from mlflow.entities import Experiment, Run, RunStatus, ViewType
 from mlflow.entities.model_registry import ModelVersion, RegisteredModel
 from mlflow.models import ModelInputExample, ModelSignature
 from mlflow.pyfunc import PyFuncModel
 from mlflow.store.entities import PagedList
 from mlflow.tracking._model_registry import DEFAULT_AWAIT_MAX_SLEEP_SECONDS
 from mlflow.tracking.fluent import _RUN_ID_ENV_VAR, SEARCH_MAX_RESULTS_PANDAS
@@ -50,15 +52,15 @@
     Set the given experiment as the active experiment.
 
     The experiment must either be specified by name via
     experiment_name or by ID via experiment_id. The experiment name and ID cannot both be specified.
     Set global variable active_experiment_name to that experiment_name.
     """
     request_for_function(inspect.currentframe())
-    mlmanager.active_experiment_name = experiment_name
+    utils.active_experiment_name = experiment_name
 
 
 def get_experiment_by_name(name: str) -> Optional[Experiment]:
     """Retrieve an experiment by experiment name from the backend store."""
     return request_for_function(inspect.currentframe())
 
 
@@ -100,24 +102,17 @@
             ).format(active_run_stack[0].info.run_id)
         )
     _active_run = request_for_function(inspect.currentframe())
     active_run_stack.append(_active_run)
     return _active_run
 
 
-def _add_eval_run(
-    run_id,
-):
-    """Add eval run to model version's metainfo on server. For internal use only."""
-    return request_for_function(inspect.currentframe())
-
-
 def log_model(
     artifact_path,
-    action_type,  # "train"/"finetune"/"upload"
+    upload_model_mode: Optional[UploadModelMode] = None,
     loader_module=None,
     data_path=None,
     code_path=None,
     conda_env=None,
     python_model=None,
     artifacts=None,
     registered_model_name="default_name",  # TODO maybe raise if no name?
@@ -215,24 +210,28 @@
 finished_run_status = RunStatus.to_string(RunStatus.FINISHED)
 
 
 def end_run(status: str = finished_run_status) -> None:
     """End an active MLflow run (if there is one)."""
     if is_server:
         mlflow.end_run()
-        active_run_stack.pop()  # why is this not checking len(active_run_stack) > 0:
-    if len(active_run_stack) > 0:
+        if len(active_run_stack) > 0:
+            active_run_stack.pop()
+    elif len(active_run_stack) > 0:
         # Clear out the global existing run environment variable as well.
         env.unset_variable(_RUN_ID_ENV_VAR)
         run = active_run_stack[-1]
         MlflowClient().set_terminated(run.info.run_id, status)
         active_run_stack.pop()
 
 
-atexit.register(end_run)
+if is_server:
+    atexit.unregister(mlflow.end_run)
+else:
+    atexit.register(end_run)
 
 
 class MlflowClient(object):
     """Initialize an MLflow Client."""
 
     def __init__(self, registry_uri: Optional[str] = None):
         self.extra_attrs = ["tracking"]
```

### Comparing `ml-management-0.0.29/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.30/ML_management/mlmanagement/mlmanager.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,45 +3,33 @@
 import json
 import os
 import shutil
 from tempfile import TemporaryDirectory
 
 import cloudpickle
 import requests
+from ML_management.mlmanagement import utils
 from ML_management.mlmanagement.jsonschema_inference import infer_jsonschema
-from ML_management.models.function_name_to_tag import FunctionNameToTag
+from ML_management.mlmanagement.model_type import ModelType
+from ML_management.mlmanagement.server_mlmanager_exceptions import InvalidExperimentName, ModelTypeIsNotFound
+from ML_management.mlmanagement.utils import EXPERIMENT_NAME_FOR_EXECUTOR, active_run_stack, is_server, server_ml_api
 from mlflow.exceptions import MlflowException, RestException
 from requests_toolbelt import MultipartEncoder
 
 import mlflow
 
-need_active_run_functions = [
-    "_add_eval_run",
-    "start_run",
-    "log_model",
-    "log_metric",
-    "set_tag",
-    "autolog",
-]
-
-need_active_experiment_functions = ["set_experiment", "search_runs", "start_run"]
-
-server_ml_api = os.environ.get("server_url", "http://localhost:8000") + "/mlflow"
-is_server = os.environ.get("is_server", False)
-
-active_run_stack = []
-active_experiment_name = None
-
 
 def create_kwargs(frame, is_it_class_function=False):
     """Get name and kwargs of function by its frame."""
     function_name = inspect.getframeinfo(frame)[2]  # get name of function
     _, _, _, kwargs = inspect.getargvalues(frame)  # get kwargs of function
     if is_it_class_function:
         del kwargs["self"]  # delete unneeded self arg
+        if not is_server and "dst_path" in kwargs:
+            del kwargs["dst_path"]  # delete unneeded dst_path for send to server
     return (
         function_name,
         kwargs,
     )  # return name of mlflow function and kwargs for that function
 
 
 def request_log_model(function_name, kwargs, extra_attrs):
@@ -54,81 +42,106 @@
     2) Do mlflow.save_model() locally
     3) Pack it to zip file
     4) Send it to server to log model there.
     """
     delete_args_for_save_model_func = [
         "artifact_path",
         "registered_model_name",
-        "await_registration_for",  # now, extra arguments
-        "action_type",
+        "await_registration_for",
+        # now, extra arguments
+        "upload_model_mode",
         "source_model_name",
         "source_model_version",
     ]  # not need for save_model
     delete_args_for_log_func = [
         "python_model",
         "artifacts",
+        "conda_env",
+        "pip_requirements",
+        "extra_pip_requirements",
     ]  # not need for log model on server
     kwargs_for_save_model = kwargs.copy()
     for delete_arg in delete_args_for_save_model_func:
         del kwargs_for_save_model[delete_arg]
 
     python_model = kwargs_for_save_model["python_model"]
-    # now we need to infer schemas for methods. We cannot check types of models,
-    # because it leads to recursive imports.
-    # TODO But if we only check method names, then user can inherit incorrectly
-    # and still succeed! Should we make it more strict? How?!
-    for func_name_to_infer in FunctionNameToTag:
-        func_from_model = getattr(python_model, func_name_to_infer.name, None)
-        if callable(func_from_model):
-            function_schema = infer_jsonschema(func_from_model)
-            kwargs[func_name_to_infer.value] = json.dumps(function_schema)
+
+    # import some modules here because of circular import
+    from ML_management.executor_template.executor_pattern import JobExecutorPattern
+    from ML_management.executor_template.executor_pattern_to_methods_map import executor_pattern_to_methods
+    from ML_management.models.model_type_to_methods_map import model_pattern_to_methods
+    from ML_management.models.patterns.model_pattern import Model
 
     with TemporaryDirectory() as temp_dir:
         model_folder = "model"
         path_for_model_folder = os.path.join(temp_dir, model_folder)
         zip_file_folder = "zip_file"
         path_for_zip_file = os.path.join(temp_dir, zip_file_folder)
-        if kwargs["python_model"] is not None:
+        if python_model is not None:
+            if isinstance(python_model, Model):
+                kwargs["model_type"] = ModelType.MODEL
+                model_to_methods = model_pattern_to_methods
+                if utils.active_experiment_name == EXPERIMENT_NAME_FOR_EXECUTOR:
+                    raise InvalidExperimentName(ModelType.MODEL.value, EXPERIMENT_NAME_FOR_EXECUTOR)
+            elif isinstance(python_model, JobExecutorPattern):
+                kwargs["model_type"] = ModelType.EXECUTOR
+                model_to_methods = executor_pattern_to_methods
+                if utils.active_experiment_name != EXPERIMENT_NAME_FOR_EXECUTOR:
+                    raise InvalidExperimentName(ModelType.EXECUTOR.value, utils.active_experiment_name)
+                # collect all needed model's methods
+                kwargs["model_method_names"] = python_model.desired_model_methods
+                kwargs["executor_upload_model_mode"] = python_model.executor_upload_model_mode
+
+            else:
+                raise ModelTypeIsNotFound()
+
+            # now we need to infer schemas for methods.
+            methods_schema = {}
+            for (model_type, methods_name_to_schema_map) in model_to_methods.items():
+                if isinstance(python_model, model_type):
+                    for method_name_to_schema in methods_name_to_schema_map:
+                        model_method = getattr(python_model, method_name_to_schema.name, None)
+                        model_method_schema = infer_jsonschema(model_method)
+                        methods_schema[method_name_to_schema.value] = model_method_schema
+            kwargs["model_methods_schema"] = json.dumps(methods_schema)
+
             mlflow.pyfunc.save_model(path=path_for_model_folder, **kwargs_for_save_model)
 
             for delete_arg in delete_args_for_log_func:
                 del kwargs[delete_arg]
             kwargs["loader_module"] = mlflow.pyfunc.model.__name__
             model_filename = shutil.make_archive(path_for_zip_file, "zip", path_for_model_folder)
 
         elif kwargs["loader_module"] is not None:
+            # now one could log only ModelType.MODEL type by 'loader_module' parameter.
+            kwargs["model_type"] = ModelType.MODEL
+            if utils.active_experiment_name == EXPERIMENT_NAME_FOR_EXECUTOR:
+                raise InvalidExperimentName(ModelType.MODEL.value, EXPERIMENT_NAME_FOR_EXECUTOR)
+            # 'model_methods_schema' not defined
+            kwargs["model_methods_schema"] = json.dumps({})
+
             if not os.path.isdir(kwargs["data_path"]):
                 raise Exception("Directory {0} doesn't exist".format(kwargs["data_path"]))
             model_filename = shutil.make_archive(path_for_zip_file, "zip", kwargs["data_path"])
         else:
             raise Exception("Either python_model or loader_module parameter must be specified")
 
         with open(model_filename, "rb") as file:
             return request(function_name, kwargs, extra_attrs, file)
 
 
 def request(function_name, kwargs, extra_attrs, model_file, for_class=None):
     """Create mlflow_request and send it to server."""
-    need_active_run = False
-    if function_name in need_active_run_functions:
-        need_active_run = True
-
-    need_active_experiment = False
-    if function_name in need_active_experiment_functions:
-        need_active_experiment = True
-
     mlflow_request = {
         "function_name": function_name,
         "kwargs": kwargs,
         "for_class": for_class,
         "extra_attrs": extra_attrs,
-        "experiment_name": active_experiment_name,
+        "experiment_name": utils.active_experiment_name,
         "active_run_ids": list(map(lambda run: run.info.run_id, active_run_stack)),
-        "need_active_run": need_active_run,
-        "need_active_experiment": need_active_experiment,
     }
     files = {
         "mlflow_request": json.dumps(mlflow_request),
         "model_zip": ("filename", model_file, "multipart/form-data"),
     }
 
     multipart = MultipartEncoder(fields=files)
@@ -151,18 +164,20 @@
     elif function_name == "load_model":
         return mlflow.pyfunc.load_model(**kwargs)
     elif function_name == "save_model":
         return mlflow.pyfunc.save_model(**kwargs)
     else:
         response = request(function_name, kwargs, extra_attrs, None, for_class)
 
+    response_content = response.content
+
     try:
-        decoded_result = cloudpickle.loads(response.content)
+        decoded_result = cloudpickle.loads(response_content)
     except Exception:
-        raise Exception(response.content.decode())
+        raise Exception(response_content.decode())
 
     # raise error if mlflow is supposed to raise error
     if isinstance(decoded_result, MlflowException):
         is_rest = decoded_result.json_kwargs.pop("isRest", False)
         if is_rest:
             created_json = {
                 "error_code": decoded_result.error_code,
```

### Comparing `ml-management-0.0.29/ML_management/registry/RegistryManager.py` & `ml-management-0.0.30/ML_management/registry/registry_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             if err.error_code == "RESOURCE_DOES_NOT_EXIST":
                 raise ModelNotRegistered(name)
             else:
                 raise err
         return registered_model
 
     def get_latest_version(self, name: str) -> ModelVersion:
-        """Get latest version of a model "name"."""
+        """Get the latest version of a model "name"."""
         latest_version = None
         registered_model = self.check_model_registered(name)
 
         # if there is only one default stage, there should be only one latest version
         # otherwise something is wrong on backend
         # version is not supposed to have no versions
         latest_version = registered_model.latest_versions[0]
```

### Comparing `ml-management-0.0.29/ML_management/registry/exceptions.py` & `ml-management-0.0.30/ML_management/registry/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,23 @@
         """Define reduce method to make exception picklable."""
         return (MetricNotLogged, (self.model_name, self.metric))
 
 
 class ModelNotRegistered(Exception):
     """Define Model Not Registered exception."""
 
-    def __init__(self, model_name: str):
+    def __init__(self, model_name: str, model_type: str = "model"):
         self.model_name = model_name
-        self.message = f'Model "{self.model_name}" is not registered'
+        self.model_type = model_type
+        self.message = f'{model_type} "{model_name}" is not registered'
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
-        return (ModelNotRegistered, (self.model_name))
+        return (ModelNotRegistered, (self.model_name, self.model_type))
 
 
 class NoMetricProvided(Exception):
     """Define No Metric Provided exception."""
 
     def __init__(self, criteria: str):
         self.criteria = criteria
```

### Comparing `ml-management-0.0.29/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.30/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.29/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.30/ML_management/tests/test_s3_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import shutil
 import unittest
 from unittest.mock import Mock, patch
 
 import boto3
-import ML_management.dataset.s3_dataset.S3Dataset
+import ML_management.dataset.s3_dataset.s3dataset
 from botocore.exceptions import ClientError
-from ML_management.dataset.s3_dataset.S3Dataset import S3BucketNotFound, S3FolderNotFound, S3ObjectNotFound
+from ML_management.dataset.s3_dataset.s3dataset import S3BucketNotFound, S3FolderNotFound, S3ObjectNotFound
 
 
 def mock_client_download_successful(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
     def mock_download_file(Bucket, Key, Filename, ExtraArgs=None, Callback=None, Config=None):
         files_content_map = {
@@ -111,20 +111,20 @@
     test-data:
         sample_data/1.txt ("one\n"),
         sample_data/2.txt ("two\n"),
         sample_data/sample_folder/3.txt ("three\n")
     """
 
     @patch(
-        "ML_management.dataset.s3_dataset.S3Dataset.client",
+        "ML_management.dataset.s3_dataset.s3dataset.client",
         new=mock_client_download_successful,
     )
     def test_download_files(self):
-        s3_dataset = ML_management.dataset.s3_dataset.S3Dataset.S3Dataset()
-        assert mock_client_download_successful is ML_management.dataset.s3_dataset.S3Dataset.client
+        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
+        assert mock_client_download_successful is ML_management.dataset.s3_dataset.s3dataset.client
         endpoint_url = "some_mock_url"
 
         local_path = s3_dataset.set_data(
             local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
             bucket="test-data",
             remote_paths=[
                 "sample_data/1.txt",
@@ -145,20 +145,20 @@
         with open(os.path.join(local_path, "sample_data/sample_folder/3.txt"), "r") as f:
             text_one = f.read()
             self.assertEqual(text_one, "three\n")
 
         shutil.rmtree(os.path.join(local_path, "sample_data/"))
 
     @patch(
-        "ML_management.dataset.s3_dataset.S3Dataset.client",
+        "ML_management.dataset.s3_dataset.s3dataset.client",
         new=mock_client_download_folder_successful,
     )
     def test_download_folder(self):
-        s3_dataset = ML_management.dataset.s3_dataset.S3Dataset.S3Dataset()
-        assert mock_client_download_folder_successful is ML_management.dataset.s3_dataset.S3Dataset.client
+        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
+        assert mock_client_download_folder_successful is ML_management.dataset.s3_dataset.s3dataset.client
         endpoint_url = "some_mock_url"
 
         local_path = s3_dataset.set_data(
             local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
             bucket="test-data",
             remote_paths=["sample_data/"],
             endpoint_url=endpoint_url,
@@ -175,77 +175,77 @@
         with open(os.path.join(local_path, "sample_data/sample_folder/3.txt"), "r") as f:
             text_one = f.read()
             self.assertEqual(text_one, "three\n")
 
         shutil.rmtree(os.path.join(local_path, "sample_data/"))
 
     @patch(
-        "ML_management.dataset.s3_dataset.S3Dataset.client",
+        "ML_management.dataset.s3_dataset.s3dataset.client",
         new=mock_client_bad_object,
     )
     def test_download_bad_object(self):
-        s3_dataset = ML_management.dataset.s3_dataset.S3Dataset.S3Dataset()
-        assert mock_client_bad_object is ML_management.dataset.s3_dataset.S3Dataset.client
+        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
+        assert mock_client_bad_object is ML_management.dataset.s3_dataset.s3dataset.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3ObjectNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="test-data",
                 remote_paths=["sample_data/nosuchfile.txt"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
             )
 
     @patch(
-        "ML_management.dataset.s3_dataset.S3Dataset.client",
+        "ML_management.dataset.s3_dataset.s3dataset.client",
         new=mock_client_bad_folder,
     )
     def test_download_bad_folder(self):
-        s3_dataset = ML_management.dataset.s3_dataset.S3Dataset.S3Dataset()
-        assert mock_client_bad_folder is ML_management.dataset.s3_dataset.S3Dataset.client
+        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
+        assert mock_client_bad_folder is ML_management.dataset.s3_dataset.s3dataset.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3FolderNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="test-data",
                 remote_paths=["sample_data/nosuchfolder/"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
             )
 
     @patch(
-        "ML_management.dataset.s3_dataset.S3Dataset.client",
+        "ML_management.dataset.s3_dataset.s3dataset.client",
         new=mock_client_bad_bucket_folder,
     )
     def test_download_bad_bucket_folder(self):
-        s3_dataset = ML_management.dataset.s3_dataset.S3Dataset.S3Dataset()
-        assert mock_client_bad_bucket_folder is ML_management.dataset.s3_dataset.S3Dataset.client
+        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
+        assert mock_client_bad_bucket_folder is ML_management.dataset.s3_dataset.s3dataset.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3BucketNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="nosuchbucket",
                 remote_paths=["sample_data/"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
             )
 
     @patch(
-        "ML_management.dataset.s3_dataset.S3Dataset.client",
+        "ML_management.dataset.s3_dataset.s3dataset.client",
         new=mock_client_bad_bucket_object,
     )
     def test_download_bad_bucket_object(self):
-        s3_dataset = ML_management.dataset.s3_dataset.S3Dataset.S3Dataset()
-        assert mock_client_bad_bucket_object is ML_management.dataset.s3_dataset.S3Dataset.client
+        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
+        assert mock_client_bad_bucket_object is ML_management.dataset.s3_dataset.s3dataset.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3BucketNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="nosuchbucket",
                 remote_paths=["sample_data/1.txt"],
```

### Comparing `ml-management-0.0.29/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.30/ml_management.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 MANIFEST.in
 README.md
 VERSION
 setup.py
 ML_management/__init__.py
-ML_management/dataset/Dataset.py
 ML_management/dataset/__init__.py
 ML_management/dataset/datamodel.py
-ML_management/dataset/dummy_dataset/DummyDataset.py
+ML_management/dataset/dataset.py
 ML_management/dataset/dummy_dataset/__init__.py
-ML_management/dataset/s3_dataset/S3Dataset.py
+ML_management/dataset/dummy_dataset/dummy_dataset.py
 ML_management/dataset/s3_dataset/__init__.py
+ML_management/dataset/s3_dataset/s3dataset.py
+ML_management/executor_template/__init__.py
+ML_management/executor_template/executor_pattern.py
+ML_management/executor_template/executor_pattern_to_methods_map.py
+ML_management/executor_template/upload_model_mode.py
+ML_management/executor_template/default_executors/__init__.py
+ML_management/executor_template/default_executors/finetune_executor.py
+ML_management/executor_template/default_executors/test_executor.py
+ML_management/executor_template/default_executors/train_executor.py
 ML_management/mlmanagement/__init__.py
 ML_management/mlmanagement/jsonschema_exceptions.py
 ML_management/mlmanagement/jsonschema_inference.py
 ML_management/mlmanagement/mlmanagement.py
 ML_management/mlmanagement/mlmanager.py
+ML_management/mlmanagement/model_type.py
 ML_management/mlmanagement/server_mlmanager_exceptions.py
-ML_management/models/RetrainableModel.py
-ML_management/models/TrainableModel.py
+ML_management/mlmanagement/utils.py
 ML_management/models/__init__.py
-ML_management/models/action_type.py
-ML_management/models/function_name_to_tag.py
-ML_management/models/model_pattern.py
-ML_management/registry/RegistryManager.py
+ML_management/models/model_type_to_methods_map.py
+ML_management/models/patterns/__init__.py
+ML_management/models/patterns/model_pattern.py
+ML_management/models/patterns/retrainable_model.py
+ML_management/models/patterns/torch_model.py
+ML_management/models/patterns/trainable_model.py
 ML_management/registry/__init__.py
 ML_management/registry/exceptions.py
+ML_management/registry/registry_manager.py
 ML_management/tests/__init__.py
 ML_management/tests/test_jsonschema_inference.py
 ML_management/tests/test_s3_dataset.py
 ml_management.egg-info/PKG-INFO
 ml_management.egg-info/SOURCES.txt
 ml_management.egg-info/dependency_links.txt
 ml_management.egg-info/requires.txt
```

### Comparing `ml-management-0.0.29/setup.py` & `ml-management-0.0.30/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     author="ISPRAS MODIS",
     author_email="modis@ispras.ru",
     maintainer="Maxim Ryndin",
     packages=find_packages(include=["ML_management", "ML_management.*"]),
     include_package_data=True,
     # jsonschema 2.6.0 is the last one to support python 3.6
     install_requires=[
-        "mlflow==1.21.0",  # TODO requires alembic, kinda sus
-        "numpy<=1.23.5",  # TODO figure out minimum np version
+        "mlflow==1.21.0",
+        "pandas>=0.20.1,<=1.5.2",
+        "numpy>=1.8.1,<=1.23.5",
         "jsonschema==2.6.0",
         "requests_toolbelt>=0.9.1,<=0.10.1",
         "boto3==1.21.21",
         "protobuf<4.0.0",
     ],
     data_files=[("", ["VERSION"])],
     python_requires=">=3.6",
```

