# Comparing `tmp/adelecv-0.0.1.tar.gz` & `tmp/adelecv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adelecv-0.0.1.tar", max compression
+gzip compressed data, was "adelecv-0.0.2.tar", max compression
```

## Comparing `adelecv-0.0.1.tar` & `adelecv-0.0.2.tar`

### file list

```diff
@@ -1,56 +1,59 @@
--rw-r--r--   0        0        0     1062 2023-03-09 08:02:42.976673 adelecv-0.0.1/LICENSE
--rw-r--r--   0        0        0     4442 2023-03-09 08:02:42.976673 adelecv-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/__init__.py
--rw-r--r--   0        0        0       61 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/config/__init__.py
--rw-r--r--   0        0        0     1359 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/config/default.py
--rw-r--r--   0        0        0        0 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/data/__init__.py
--rw-r--r--   0        0        0      456 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/data/segmentations/__init__.py
--rw-r--r--   0        0        0     6583 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/data/segmentations/dataset.py
--rw-r--r--   0        0        0     1655 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/data/segmentations/torch_dataset.py
--rw-r--r--   0        0        0     3257 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/data/segmentations/types.py
--rw-r--r--   0        0        0      166 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/logs/__init__.py
--rw-r--r--   0        0        0      859 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/logs/handlers.py
--rw-r--r--   0        0        0      997 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/logs/utils.py
--rw-r--r--   0        0        0        0 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/__init__.py
--rw-r--r--   0        0        0       65 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/base/__init__.py
--rw-r--r--   0        0        0     3723 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/base/base_model.py
--rw-r--r--   0        0        0      410 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/segmentations/__init__.py
--rw-r--r--   0        0        0     2442 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/segmentations/functional.py
--rw-r--r--   0        0        0     6706 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/segmentations/segmentation_model.py
--rw-r--r--   0        0        0     1342 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/segmentations/utils.py
--rw-r--r--   0        0        0       89 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/tensorboard_logger/__init__.py
--rw-r--r--   0        0        0     1599 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/models/tensorboard_logger/tensorboard_logger.py
--rw-r--r--   0        0        0       69 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/modification_models/__init__.py
--rw-r--r--   0        0        0     1341 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/modification_models/export.py
--rw-r--r--   0        0        0      219 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/optimize/segmentations/__init__.py
--rw-r--r--   0        0        0      535 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/optimize/segmentations/functional.py
--rw-r--r--   0        0        0     5892 2023-03-09 08:02:42.976673 adelecv-0.0.1/adelecv/api/optimize/segmentations/hp_optimizer.py
--rw-r--r--   0        0        0     3992 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/api/optimize/segmentations/hyper_params.py
--rw-r--r--   0        0        0        0 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/__init__.py
--rw-r--r--   0        0        0      717 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/app.py
--rw-r--r--   0        0        0     1523 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/assets/script.js
--rw-r--r--   0        0        0     1987 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/assets/style.css
--rw-r--r--   0        0        0      453 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/callbacks/__init__.py
--rw-r--r--   0        0        0      521 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/callbacks/console.py
--rw-r--r--   0        0        0     2138 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/callbacks/dataset.py
--rw-r--r--   0        0        0     1008 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/callbacks/notifications.py
--rw-r--r--   0        0        0     1227 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/callbacks/table_models.py
--rw-r--r--   0        0        0     1979 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/callbacks/train.py
--rw-r--r--   0        0        0      300 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/components/__init__.py
--rw-r--r--   0        0        0      339 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/components/console.py
--rw-r--r--   0        0        0     3579 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/components/dataset.py
--rw-r--r--   0        0        0     2886 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/components/homepage.py
--rw-r--r--   0        0        0      437 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/components/navbar.py
--rw-r--r--   0        0        0     2039 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/components/table_models.py
--rw-r--r--   0        0        0     5035 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/components/train.py
--rw-r--r--   0        0        0     2000 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/index.py
--rw-r--r--   0        0        0      130 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/task/__init__.py
--rw-r--r--   0        0        0     2269 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/task/base.py
--rw-r--r--   0        0        0     1871 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/task/segmentation_task.py
--rw-r--r--   0        0        0      272 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/utils/__init__.py
--rw-r--r--   0        0        0      722 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/utils/console.py
--rw-r--r--   0        0        0     1723 2023-03-09 08:02:42.980674 adelecv-0.0.1/adelecv/ui/dashboard/utils/notifications.py
--rw-r--r--   0        0        0     1342 2023-03-09 08:02:42.980674 adelecv-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5702 1970-01-01 00:00:00.000000 adelecv-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-02 18:10:12.413374 adelecv-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4397 2023-05-02 18:10:12.413374 adelecv-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/config/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/config/default.py
+-rw-r--r--   0        0        0        0 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/data/__init__.py
+-rw-r--r--   0        0        0      456 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/data/segmentations/__init__.py
+-rw-r--r--   0        0        0     6583 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/data/segmentations/dataset.py
+-rw-r--r--   0        0        0     1655 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/data/segmentations/torch_dataset.py
+-rw-r--r--   0        0        0     3257 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/data/segmentations/types.py
+-rw-r--r--   0        0        0      166 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/logs/__init__.py
+-rw-r--r--   0        0        0      859 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/logs/handlers.py
+-rw-r--r--   0        0        0      997 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/logs/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 18:10:12.413374 adelecv-0.0.2/adelecv/api/models/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/base/__init__.py
+-rw-r--r--   0        0        0     3729 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/base/base_model.py
+-rw-r--r--   0        0        0      410 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/segmentations/__init__.py
+-rw-r--r--   0        0        0     2442 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/segmentations/functional.py
+-rw-r--r--   0        0        0     6706 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/segmentations/segmentation_model.py
+-rw-r--r--   0        0        0     1342 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/segmentations/utils.py
+-rw-r--r--   0        0        0       89 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/tensorboard_logger/__init__.py
+-rw-r--r--   0        0        0     1599 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/models/tensorboard_logger/tensorboard_logger.py
+-rw-r--r--   0        0        0      127 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/modification_models/__init__.py
+-rw-r--r--   0        0        0     3259 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/modification_models/convert.py
+-rw-r--r--   0        0        0     1410 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/modification_models/conveter.py
+-rw-r--r--   0        0        0     1341 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/modification_models/export.py
+-rw-r--r--   0        0        0        0 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/optimize/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/optimize/segmentations/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/optimize/segmentations/functional.py
+-rw-r--r--   0        0        0     5892 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/optimize/segmentations/hp_optimizer.py
+-rw-r--r--   0        0        0     3992 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/api/optimize/segmentations/hyper_params.py
+-rw-r--r--   0        0        0        0 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/__init__.py
+-rw-r--r--   0        0        0      717 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/app.py
+-rw-r--r--   0        0        0     1523 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/assets/script.js
+-rw-r--r--   0        0        0     1987 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/assets/style.css
+-rw-r--r--   0        0        0      453 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/callbacks/__init__.py
+-rw-r--r--   0        0        0      521 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/callbacks/console.py
+-rw-r--r--   0        0        0     2138 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/callbacks/dataset.py
+-rw-r--r--   0        0        0     1008 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/callbacks/notifications.py
+-rw-r--r--   0        0        0     1492 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/callbacks/table_models.py
+-rw-r--r--   0        0        0     1979 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/callbacks/train.py
+-rw-r--r--   0        0        0      300 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/components/__init__.py
+-rw-r--r--   0        0        0      339 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/components/console.py
+-rw-r--r--   0        0        0     3579 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/components/dataset.py
+-rw-r--r--   0        0        0     2886 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/components/homepage.py
+-rw-r--r--   0        0        0      437 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/components/navbar.py
+-rw-r--r--   0        0        0     2472 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/components/table_models.py
+-rw-r--r--   0        0        0     5035 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/components/train.py
+-rw-r--r--   0        0        0     1937 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/index.py
+-rw-r--r--   0        0        0      130 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/task/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/task/base.py
+-rw-r--r--   0        0        0     1905 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/task/segmentation_task.py
+-rw-r--r--   0        0        0      272 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/utils/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/utils/console.py
+-rw-r--r--   0        0        0     1723 2023-05-02 18:10:12.417374 adelecv-0.0.2/adelecv/ui/dashboard/utils/notifications.py
+-rw-r--r--   0        0        0     1342 2023-05-02 18:10:12.417374 adelecv-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5657 1970-01-01 00:00:00.000000 adelecv-0.0.2/PKG-INFO
```

### Comparing `adelecv-0.0.1/LICENSE` & `adelecv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/README.md` & `adelecv-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 <div align="center">
 
 <img src="https://github.com/AsakoKabe/AdeleCV/blob/main/docs/logo.png?raw=true" alt="drawing" width="200"/>
 
+**Auto DEap LEarning Computer Vision**
+
 **Python library and dashboard for hyperparameter search and model training for computer vision tasks
 based on [PyTorch](https://pytorch.org/), [Optuna](https://optuna.org/),
     [FiftyOne](https://docs.voxel51.com/), [Dash](https://dash.plotly.com/),
     [Segmentation Model Pytorch](https://github.com/qubvel/segmentation_models.pytorch).**  
 
 [![Generic badge](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=for-the-badge)](https://github.com/AsakoKabe/AdeleCV/blob/main/LICENSE)
 [![Read the Docs](https://img.shields.io/readthedocs/smp?style=for-the-badge&logo=readthedocs&logoColor=white)](https://adelecv.readthedocs.io/en/latest/) 
 [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/AsakoKabe/AdeleCV/code-style.yaml?branch=main&style=for-the-badge)](https://github.com/AsakoKabe/AdeleCV/actions/workflows/code-style.yaml)
 
-[//]: # ([![PyPI]&#40;https://img.shields.io/pypi/v/segmentation-models-pytorch?color=blue&style=for-the-badge&logo=pypi&logoColor=white&#41;]&#40;https://pypi.org/project/segmentation-models-pytorch/&#41; )
-[//]: # ([![PyPI - Downloads]&#40;https://img.shields.io/pypi/dm/segmentation-models-pytorch?style=for-the-badge&color=blue&#41;]&#40;https://pepy.tech/project/segmentation-models-pytorch&#41; )
-[//]: # (<br>)
+[![PyPI](https://img.shields.io/pypi/v/adelecv?color=blue&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/adelecv/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/adelecv?style=for-the-badge&color=blue)](https://pepy.tech/project/adelecv) 
+<br>
 </div>
 
 The main features of this library are:
 
  - Fiftyone dataset integration with prediction visualization
  - Uploading your dataset in one of the popular formats, currently supported - 2
  - Adding your own python class for convert dataset
  - Displaying training statistics in tensorboard
  - Support for all samples from optuna
  - Segmentation use smp: 9 model architectures, popular losses and metrics, see [doc smp](https://github.com/qubvel/segmentation_models.pytorch)
- - Convert weights to another format, currently supported - 0
+ - Convert weights to another format, currently supported - 1 (onnx)
  
 ### [📚 Project Documentation 📚](https://adelecv.readthedocs.io/en/latest/)
 
 Visit [Read The Docs Project Page](https://adelecv.readthedocs.io/en/latest/) or read following README to know more about Auto Deap Learning Computer Vision (AdeleCV for short) library
 
 ### 📋 Table of content
  1. [Examples](#examples)
@@ -70,15 +72,15 @@
 TMP_PATH='./tmp'
 DASHBOARD_PORT=8080
 FIFTYONE_PORT=5151
 TENSORBOARD_PORT=6006
 NOTIFICATION_LEVEL=DEBUG
 ```
 
-2. Run.
+2. Run (about 30 seconds (I'm working on acceleration)).
 ```bash
 adelecv_dashboard --envfile .env
 ```
 
 3. Help
 ```bash
 adelecv_dashboard --help
@@ -97,15 +99,15 @@
 - logs: python logging 
 
 The Dash library was used for dashboard. It is based on components and callbacks on these component elements.
 
 ### 📝 Citing
 ```
 @misc{Mamatin:2023,
-  Author = {Denis Mamtin},
+  Author = {Denis Mamatin},
   Title = {AdeleCV},
   Year = {2023},
   Publisher = {GitHub},
   Journal = {GitHub repository},
   Howpublished = {\url{https://github.com/AsakoKabe/AdeleCV}}
 }
 ```
```

### Comparing `adelecv-0.0.1/adelecv/api/config/default.py` & `adelecv-0.0.2/adelecv/api/config/default.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/data/segmentations/dataset.py` & `adelecv-0.0.2/adelecv/api/data/segmentations/dataset.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/data/segmentations/torch_dataset.py` & `adelecv-0.0.2/adelecv/api/data/segmentations/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/data/segmentations/types.py` & `adelecv-0.0.2/adelecv/api/data/segmentations/types.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/logs/handlers.py` & `adelecv-0.0.2/adelecv/api/logs/handlers.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/logs/utils.py` & `adelecv-0.0.2/adelecv/api/logs/utils.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/models/base/base_model.py` & `adelecv-0.0.2/adelecv/api/models/base/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self._stats_model = None
 
     def save_weights(self) -> None:
         path = self._weights_path
         if not os.path.exists(path):
             os.mkdir(path)
         save_path = path / f'{self._id}.pt'
-        torch.save(self._torch_model, save_path)
+        torch.save(self._torch_model.cpu(), save_path)
         get_logger().debug(
             "Save weights model: %s, path: %s", str(self), save_path.as_posix()
         )
 
     @property
     def stats_model(self) -> pd.DataFrame:
         return self._stats_model
```

### Comparing `adelecv-0.0.1/adelecv/api/models/segmentations/functional.py` & `adelecv-0.0.2/adelecv/api/models/segmentations/functional.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/models/segmentations/segmentation_model.py` & `adelecv-0.0.2/adelecv/api/models/segmentations/segmentation_model.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/models/segmentations/utils.py` & `adelecv-0.0.2/adelecv/api/models/segmentations/utils.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/models/tensorboard_logger/tensorboard_logger.py` & `adelecv-0.0.2/adelecv/api/models/tensorboard_logger/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/modification_models/export.py` & `adelecv-0.0.2/adelecv/api/modification_models/export.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/optimize/segmentations/functional.py` & `adelecv-0.0.2/adelecv/api/optimize/segmentations/functional.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/optimize/segmentations/hp_optimizer.py` & `adelecv-0.0.2/adelecv/api/optimize/segmentations/hp_optimizer.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/api/optimize/segmentations/hyper_params.py` & `adelecv-0.0.2/adelecv/api/optimize/segmentations/hyper_params.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/app.py` & `adelecv-0.0.2/adelecv/ui/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/assets/script.js` & `adelecv-0.0.2/adelecv/ui/dashboard/assets/script.js`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/assets/style.css` & `adelecv-0.0.2/adelecv/ui/dashboard/assets/style.css`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/callbacks/console.py` & `adelecv-0.0.2/adelecv/ui/dashboard/callbacks/console.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/callbacks/dataset.py` & `adelecv-0.0.2/adelecv/ui/dashboard/callbacks/dataset.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/callbacks/notifications.py` & `adelecv-0.0.2/adelecv/ui/dashboard/callbacks/notifications.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/callbacks/table_models.py` & `adelecv-0.0.2/adelecv/ui/dashboard/callbacks/table_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dash import Input, Output, State, dcc
 from dash.exceptions import PreventUpdate
 
 from adelecv.api.config import Settings
-from adelecv.api.modification_models.export import ExportWeights
-from adelecv.ui.dashboard.app import app
+from adelecv.api.modification_models import ExportWeights, ConvertWeights
+from adelecv.ui.dashboard.app import app, _task
 
 
 @app.callback(
     Output("download-weights", "data"),
     Input("export-weights", "n_clicks"),
     State('stats-models-table', "derived_virtual_data"),
     State('stats-models-table', "derived_virtual_selected_rows"),
@@ -20,19 +20,24 @@
     id_selected = {rows[i]['_id'] for i in derived_virtual_selected_rows}
     zip_path = ExportWeights(Settings.WEIGHTS_PATH).create_zip(id_selected)
 
     return dcc.send_file(zip_path.as_posix())
 
 
 @app.callback(
-    Input("convert-weights", "n_clicks"),
+    Output("download-converted-onnx", "data"),
+    Input("convert-weights-format-onnx", "n_clicks"),
     State('stats-models-table', "derived_virtual_data"),
     State('stats-models-table', "derived_virtual_selected_rows"),
     prevent_initial_call=True
 )
 def convert_weights(n_clicks, rows, derived_virtual_selected_rows):
     if not n_clicks:
         raise PreventUpdate()
 
-    print('convert weights', derived_virtual_selected_rows)
-    print(rows)
-    # return ''
+    id_selected = {rows[i]['_id'] for i in derived_virtual_selected_rows}
+    img_shape = _task.img_shape[0], _task.img_shape[0], 3
+    zip_path = ConvertWeights(
+        img_shape, Settings.WEIGHTS_PATH
+    ).run(id_selected, 'onnx')
+
+    return dcc.send_file(zip_path.as_posix())
```

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/callbacks/train.py` & `adelecv-0.0.2/adelecv/ui/dashboard/callbacks/train.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/components/dataset.py` & `adelecv-0.0.2/adelecv/ui/dashboard/components/dataset.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/components/homepage.py` & `adelecv-0.0.2/adelecv/ui/dashboard/components/homepage.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/components/table_models.py` & `adelecv-0.0.2/adelecv/ui/dashboard/components/table_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,21 +16,31 @@
             dbc.DropdownMenu(
                 label="Menu",
                 id='table-menu',
                 children=[
                     dbc.DropdownMenuItem(
                         "Export weights", id='export-weights'
                         ),
-                    dbc.DropdownMenuItem(
-                        "Convert weights", id='convert-weights'
-                        ),
+                    dbc.DropdownMenu(
+                        label="Convert weights",
+                        id='convert-weights',
+                        children=[
+                            dbc.DropdownMenuItem(
+                                "ONNX", id='convert-weights-format-onnx'
+                            ),
+                        ],
+                        color="secondary",
+                        direction="end",
+                        style={"margin-bottom": "1%"}
+                    ),
                 ],
                 style={"margin-bottom": "1%"}
             ),
             dcc.Download(id="download-weights"),
+            dcc.Download(id="download-converted-onnx"),
             html.Div(
                 [
                     dash_table.DataTable(
                         id='stats-models-table',
                         columns=cols,
                         data=df.to_dict('records'),
                         # editable=True,
```

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/components/train.py` & `adelecv-0.0.2/adelecv/ui/dashboard/components/train.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/index.py` & `adelecv-0.0.2/adelecv/ui/dashboard/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,12 @@
     enable_logs(
         LogConsoleHandler(),
         Settings.LOGGER_NAME,
         logging.Formatter(
             '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
         )
     )
-    app.run(
-        port=Settings.DASHBOARD_PORT,
-        debug=False
-    )
+    app.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/task/base.py` & `adelecv-0.0.2/adelecv/ui/dashboard/task/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         self._weights_dir = None
         self.models: list[SegmentationModel] = []
         self._stats_models = pd.DataFrame()
         self._hp_optimizer = None
         self._dataset = None
         self._tb = None
         self._session_dataset = None
+        self._img_shape = None
 
     def launch(self, env_path: Path | None):
         if env_path is not None:
             _load_settings_from_env(Path(env_path))
 
         self._weights_dir = Settings.WEIGHTS_PATH
         self._session_dataset = fo.launch_app(
@@ -67,7 +68,15 @@
 
     def _run_optimize(self) -> None:
         self._hp_optimizer.optimize()
 
     @property
     def stats_models(self) -> pd.DataFrame:
         return self._stats_models
+
+    @property
+    def img_shape(self) -> list[int, int]:
+        return self._img_shape
+
+    @img_shape.setter
+    def img_shape(self, new_val: list[int, int]):
+        self._img_shape = new_val
```

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/task/segmentation_task.py` & `adelecv-0.0.2/adelecv/ui/dashboard/task/segmentation_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,7 +52,8 @@
             dataset_path,
             dataset_type,
             img_size,
             split,
             batch_size
         )
         self._create_dataset_session()
+        self.img_shape = img_size
```

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/utils/console.py` & `adelecv-0.0.2/adelecv/ui/dashboard/utils/console.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/adelecv/ui/dashboard/utils/notifications.py` & `adelecv-0.0.2/adelecv/ui/dashboard/utils/notifications.py`

 * *Files identical despite different names*

### Comparing `adelecv-0.0.1/pyproject.toml` & `adelecv-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adelecv"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Denis Mamatin <mamatin-denis@yandex.ru>"]
 description = ""
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `adelecv-0.0.1/PKG-INFO` & `adelecv-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adelecv
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Denis Mamatin
 Author-email: mamatin-denis@yandex.ru
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -30,37 +30,39 @@
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://github.com/AsakoKabe/AdeleCV/blob/main/docs/logo.png?raw=true" alt="drawing" width="200"/>
 
+**Auto DEap LEarning Computer Vision**
+
 **Python library and dashboard for hyperparameter search and model training for computer vision tasks
 based on [PyTorch](https://pytorch.org/), [Optuna](https://optuna.org/),
     [FiftyOne](https://docs.voxel51.com/), [Dash](https://dash.plotly.com/),
     [Segmentation Model Pytorch](https://github.com/qubvel/segmentation_models.pytorch).**  
 
 [![Generic badge](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=for-the-badge)](https://github.com/AsakoKabe/AdeleCV/blob/main/LICENSE)
 [![Read the Docs](https://img.shields.io/readthedocs/smp?style=for-the-badge&logo=readthedocs&logoColor=white)](https://adelecv.readthedocs.io/en/latest/) 
 [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/AsakoKabe/AdeleCV/code-style.yaml?branch=main&style=for-the-badge)](https://github.com/AsakoKabe/AdeleCV/actions/workflows/code-style.yaml)
 
-[//]: # ([![PyPI]&#40;https://img.shields.io/pypi/v/segmentation-models-pytorch?color=blue&style=for-the-badge&logo=pypi&logoColor=white&#41;]&#40;https://pypi.org/project/segmentation-models-pytorch/&#41; )
-[//]: # ([![PyPI - Downloads]&#40;https://img.shields.io/pypi/dm/segmentation-models-pytorch?style=for-the-badge&color=blue&#41;]&#40;https://pepy.tech/project/segmentation-models-pytorch&#41; )
-[//]: # (<br>)
+[![PyPI](https://img.shields.io/pypi/v/adelecv?color=blue&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/adelecv/) 
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/adelecv?style=for-the-badge&color=blue)](https://pepy.tech/project/adelecv) 
+<br>
 </div>
 
 The main features of this library are:
 
  - Fiftyone dataset integration with prediction visualization
  - Uploading your dataset in one of the popular formats, currently supported - 2
  - Adding your own python class for convert dataset
  - Displaying training statistics in tensorboard
  - Support for all samples from optuna
  - Segmentation use smp: 9 model architectures, popular losses and metrics, see [doc smp](https://github.com/qubvel/segmentation_models.pytorch)
- - Convert weights to another format, currently supported - 0
+ - Convert weights to another format, currently supported - 1 (onnx)
  
 ### [📚 Project Documentation 📚](https://adelecv.readthedocs.io/en/latest/)
 
 Visit [Read The Docs Project Page](https://adelecv.readthedocs.io/en/latest/) or read following README to know more about Auto Deap Learning Computer Vision (AdeleCV for short) library
 
 ### 📋 Table of content
  1. [Examples](#examples)
@@ -102,15 +104,15 @@
 TMP_PATH='./tmp'
 DASHBOARD_PORT=8080
 FIFTYONE_PORT=5151
 TENSORBOARD_PORT=6006
 NOTIFICATION_LEVEL=DEBUG
 ```
 
-2. Run.
+2. Run (about 30 seconds (I'm working on acceleration)).
 ```bash
 adelecv_dashboard --envfile .env
 ```
 
 3. Help
 ```bash
 adelecv_dashboard --help
@@ -129,15 +131,15 @@
 - logs: python logging 
 
 The Dash library was used for dashboard. It is based on components and callbacks on these component elements.
 
 ### 📝 Citing
 ```
 @misc{Mamatin:2023,
-  Author = {Denis Mamtin},
+  Author = {Denis Mamatin},
   Title = {AdeleCV},
   Year = {2023},
   Publisher = {GitHub},
   Journal = {GitHub repository},
   Howpublished = {\url{https://github.com/AsakoKabe/AdeleCV}}
 }
 ```
```

