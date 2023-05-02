# Comparing `tmp/eir-dl-0.1.8a0.tar.gz` & `tmp/eir-dl-0.1.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eir-dl-0.1.8a0.tar", max compression
+gzip compressed data, was "eir-dl-0.1.9a0.tar", max compression
```

## Comparing `eir-dl-0.1.8a0.tar` & `eir-dl-0.1.9a0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    34523 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/LICENSE
--rw-r--r--   0        0        0       28 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/__init__.py
--rw-r--r--   0        0        0     1843 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/build_module.py
--rw-r--r--   0        0        0    14993 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/configuration.py
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/data_load/__init__.py
--rw-r--r--   0        0        0     4860 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/data_load/common_ops.py
--rw-r--r--   0        0        0    10231 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/data_load/data_augmentation.py
--rw-r--r--   0        0        0     3892 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/data_load/data_loading_funcs.py
--rw-r--r--   0        0        0      538 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/data_load/data_utils.py
--rw-r--r--   0        0        0    18555 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/data_load/datasets.py
--rw-r--r--   0        0        0    32112 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/data_load/label_setup.py
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/interpretation/__init__.py
--rw-r--r--   0        0        0    13432 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/interpretation/interpret_omics.py
--rw-r--r--   0        0        0    13455 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/interpretation/interpret_tabular.py
--rw-r--r--   0        0        0    17125 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/interpretation/interpretation.py
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/models/.gitkeep
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/models/__init__.py
--rw-r--r--   0        0        0     4091 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/models/fusion.py
--rw-r--r--   0        0        0     6431 2021-06-21 16:09:24.833917 eir-dl-0.1.8a0/eir/models/fusion_mgmoe.py
--rw-r--r--   0        0        0    14613 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/layers.py
--rw-r--r--   0        0        0    13097 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/model_training_utils.py
--rw-r--r--   0        0        0     5321 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/models_base.py
--rw-r--r--   0        0        0     2882 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/models_linear.py
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/omics/__init__.py
--rw-r--r--   0        0        0     8536 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/omics/models_cnn.py
--rw-r--r--   0        0        0     1072 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/omics/models_mlp.py
--rw-r--r--   0        0        0     8449 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/omics/models_split_mlp.py
--rw-r--r--   0        0        0     2947 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/omics/omics_models.py
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/tabular/__init__.py
--rw-r--r--   0        0        0     8397 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/models/tabular/tabular.py
--rw-r--r--   0        0        0    26883 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/predict.py
--rw-r--r--   0        0        0    34406 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train.py
--rw-r--r--   0        0        0      487 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train_utils/__init__.py
--rw-r--r--   0        0        0     8483 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train_utils/evaluation.py
--rw-r--r--   0        0        0    14109 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train_utils/lr_scheduling.py
--rw-r--r--   0        0        0    17149 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train_utils/metrics.py
--rw-r--r--   0        0        0     3774 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train_utils/optimizers.py
--rw-r--r--   0        0        0    23039 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train_utils/train_handlers.py
--rw-r--r--   0        0        0     4101 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/train_utils/utils.py
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/visualization/.gitkeep
--rw-r--r--   0        0        0        0 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/visualization/__init__.py
--rw-r--r--   0        0        0     9080 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/visualization/interpretation_visualization.py
--rw-r--r--   0        0        0    17349 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/eir/visualization/visualization_funcs.py
--rw-r--r--   0        0        0     1285 2021-06-21 16:09:24.837917 eir-dl-0.1.8a0/pyproject.toml
--rw-r--r--   0        0        0     1494 2021-06-21 16:29:07.281208 eir-dl-0.1.8a0/setup.py
--rw-r--r--   0        0        0     1230 2021-06-21 16:29:07.281544 eir-dl-0.1.8a0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/LICENSE
+-rw-r--r--   0        0        0       28 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/__init__.py
+-rw-r--r--   0        0        0     1843 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/build_module.py
+-rw-r--r--   0        0        0    14993 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/configuration.py
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/data_load/__init__.py
+-rw-r--r--   0        0        0     4860 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/data_load/common_ops.py
+-rw-r--r--   0        0        0    10231 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/data_load/data_augmentation.py
+-rw-r--r--   0        0        0     3892 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/data_load/data_loading_funcs.py
+-rw-r--r--   0        0        0      538 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/data_load/data_utils.py
+-rw-r--r--   0        0        0    18555 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/data_load/datasets.py
+-rw-r--r--   0        0        0    32112 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/data_load/label_setup.py
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/interpretation/__init__.py
+-rw-r--r--   0        0        0    13432 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/interpretation/interpret_omics.py
+-rw-r--r--   0        0        0    13455 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/interpretation/interpret_tabular.py
+-rw-r--r--   0        0        0    17125 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/interpretation/interpretation.py
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/.gitkeep
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/__init__.py
+-rw-r--r--   0        0        0     4091 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/fusion.py
+-rw-r--r--   0        0        0     6431 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/fusion_mgmoe.py
+-rw-r--r--   0        0        0    14613 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/layers.py
+-rw-r--r--   0        0        0    13097 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/model_training_utils.py
+-rw-r--r--   0        0        0     5321 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/models_base.py
+-rw-r--r--   0        0        0     2882 2021-06-22 13:08:09.862299 eir-dl-0.1.9a0/eir/models/models_linear.py
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/models/omics/__init__.py
+-rw-r--r--   0        0        0     8536 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/models/omics/models_cnn.py
+-rw-r--r--   0        0        0     1072 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/models/omics/models_mlp.py
+-rw-r--r--   0        0        0     8449 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/models/omics/models_split_mlp.py
+-rw-r--r--   0        0        0     2947 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/models/omics/omics_models.py
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/models/tabular/__init__.py
+-rw-r--r--   0        0        0     8397 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/models/tabular/tabular.py
+-rw-r--r--   0        0        0    26883 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/predict.py
+-rw-r--r--   0        0        0    34406 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train.py
+-rw-r--r--   0        0        0      487 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train_utils/__init__.py
+-rw-r--r--   0        0        0     8483 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train_utils/evaluation.py
+-rw-r--r--   0        0        0    14109 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train_utils/lr_scheduling.py
+-rw-r--r--   0        0        0    17149 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train_utils/metrics.py
+-rw-r--r--   0        0        0     3774 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train_utils/optimizers.py
+-rw-r--r--   0        0        0    23039 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train_utils/train_handlers.py
+-rw-r--r--   0        0        0     4101 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/train_utils/utils.py
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/visualization/.gitkeep
+-rw-r--r--   0        0        0        0 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/visualization/__init__.py
+-rw-r--r--   0        0        0     9080 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/visualization/interpretation_visualization.py
+-rw-r--r--   0        0        0    17349 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/eir/visualization/visualization_funcs.py
+-rw-r--r--   0        0        0     1294 2021-06-22 13:08:09.866299 eir-dl-0.1.9a0/pyproject.toml
+-rw-r--r--   0        0        0     1495 2021-06-22 13:08:19.279168 eir-dl-0.1.9a0/setup.py
+-rw-r--r--   0        0        0     1231 2021-06-22 13:08:19.279674 eir-dl-0.1.9a0/PKG-INFO
```

### Comparing `eir-dl-0.1.8a0/LICENSE` & `eir-dl-0.1.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/build_module.py` & `eir-dl-0.1.9a0/eir/build_module.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/configuration.py` & `eir-dl-0.1.9a0/eir/configuration.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/data_load/common_ops.py` & `eir-dl-0.1.9a0/eir/data_load/common_ops.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/data_load/data_augmentation.py` & `eir-dl-0.1.9a0/eir/data_load/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/data_load/data_loading_funcs.py` & `eir-dl-0.1.9a0/eir/data_load/data_loading_funcs.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/data_load/data_utils.py` & `eir-dl-0.1.9a0/eir/data_load/data_utils.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/data_load/datasets.py` & `eir-dl-0.1.9a0/eir/data_load/datasets.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/data_load/label_setup.py` & `eir-dl-0.1.9a0/eir/data_load/label_setup.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/interpretation/interpret_omics.py` & `eir-dl-0.1.9a0/eir/interpretation/interpret_omics.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/interpretation/interpret_tabular.py` & `eir-dl-0.1.9a0/eir/interpretation/interpret_tabular.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/interpretation/interpretation.py` & `eir-dl-0.1.9a0/eir/interpretation/interpretation.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/fusion.py` & `eir-dl-0.1.9a0/eir/models/fusion.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/fusion_mgmoe.py` & `eir-dl-0.1.9a0/eir/models/fusion_mgmoe.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/layers.py` & `eir-dl-0.1.9a0/eir/models/layers.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/model_training_utils.py` & `eir-dl-0.1.9a0/eir/models/model_training_utils.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/models_base.py` & `eir-dl-0.1.9a0/eir/models/models_base.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/models_linear.py` & `eir-dl-0.1.9a0/eir/models/models_linear.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/omics/models_cnn.py` & `eir-dl-0.1.9a0/eir/models/omics/models_cnn.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/omics/models_mlp.py` & `eir-dl-0.1.9a0/eir/models/omics/models_mlp.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/omics/models_split_mlp.py` & `eir-dl-0.1.9a0/eir/models/omics/models_split_mlp.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/omics/omics_models.py` & `eir-dl-0.1.9a0/eir/models/omics/omics_models.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/models/tabular/tabular.py` & `eir-dl-0.1.9a0/eir/models/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/predict.py` & `eir-dl-0.1.9a0/eir/predict.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/train.py` & `eir-dl-0.1.9a0/eir/train.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/train_utils/evaluation.py` & `eir-dl-0.1.9a0/eir/train_utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/train_utils/lr_scheduling.py` & `eir-dl-0.1.9a0/eir/train_utils/lr_scheduling.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/train_utils/metrics.py` & `eir-dl-0.1.9a0/eir/train_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/train_utils/optimizers.py` & `eir-dl-0.1.9a0/eir/train_utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/train_utils/train_handlers.py` & `eir-dl-0.1.9a0/eir/train_utils/train_handlers.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/train_utils/utils.py` & `eir-dl-0.1.9a0/eir/train_utils/utils.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/visualization/interpretation_visualization.py` & `eir-dl-0.1.9a0/eir/visualization/interpretation_visualization.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/eir/visualization/visualization_funcs.py` & `eir-dl-0.1.9a0/eir/visualization/visualization_funcs.py`

 * *Files identical despite different names*

### Comparing `eir-dl-0.1.8a0/pyproject.toml` & `eir-dl-0.1.9a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "eir-dl"
-version = "0.1.8-alpha"
+version = "0.1.9-alpha"
 description = ""
 license = "AGPLv3"
 authors = ["Arnor Sigurdsson"]
 packages = [
     { include="eir", from="." },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">= 3.8,< 3.10"
 pandas = "^1.2.0"
 numpy = "^1.19.2"
 torch = "1.9.0"
 torchvision = "0.10.0"
 py = "^1.9.0"
 matplotlib = "^3.3.2"
 pytorch-ignite = "^0.4.2"
```

### Comparing `eir-dl-0.1.8a0/setup.py` & `eir-dl-0.1.9a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,25 @@
 
 entry_points = \
 {'console_scripts': ['eirpredict = eir.predict:main',
                      'eirtrain = eir.train:main']}
 
 setup_kwargs = {
     'name': 'eir-dl',
-    'version': '0.1.8a0',
+    'version': '0.1.9a0',
     'description': '',
     'long_description': None,
     'author': 'Arnor Sigurdsson',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `eir-dl-0.1.8a0/PKG-INFO` & `eir-dl-0.1.9a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: eir-dl
-Version: 0.1.8a0
+Version: 0.1.9a0
 Summary: 
 License: AGPLv3
 Author: Arnor Sigurdsson
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: ConfigArgParse (>=1.2.3,<2.0.0)
 Requires-Dist: adabelief-pytorch (>=0.2.0,<0.3.0)
 Requires-Dist: aislib (==0.1.5a0)
```

