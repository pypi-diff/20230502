# Comparing `tmp/rxn-onmt-models-1.0.0.tar.gz` & `tmp/rxn-onmt-models-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-onmt-models-1.0.0.tar", last modified: Fri Feb 24 09:21:11 2023, max compression
+gzip compressed data, was "rxn-onmt-models-1.0.1.tar", last modified: Tue May  2 08:16:13 2023, max compression
```

## Comparing `rxn-onmt-models-1.0.0.tar` & `rxn-onmt-models-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:11.634455 rxn-onmt-models-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-02-24 09:21:11.634455 rxn-onmt-models-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-02-24 09:21:11.634455 rxn-onmt-models-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:11.630455 rxn-onmt-models-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:11.630455 rxn-onmt-models-1.0.0/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:11.630455 rxn-onmt-models-1.0.0/src/rxn/onmt_models/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/prediction_collapser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:11.634455 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_continue_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_finetune.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_plan_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/training_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/src/rxn/onmt_models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:11.634455 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-02-24 09:21:11.000000 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-24 09:21:11.000000 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:21:11.000000 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-24 09:21:11.000000 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:21:11.000000 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-24 09:21:11.000000 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-24 09:21:11.000000 rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:21:11.634455 rxn-onmt-models-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/tests/test_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/tests/test_prediction_collapser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/tests/test_prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-02-24 09:21:02.000000 rxn-onmt-models-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:13.603381 rxn-onmt-models-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-02 08:16:13.603381 rxn-onmt-models-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 08:16:13.607381 rxn-onmt-models-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:13.599380 rxn-onmt-models-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:13.599380 rxn-onmt-models-1.0.1/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:13.603381 rxn-onmt-models-1.0.1/src/rxn/onmt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/prediction_collapser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:13.603381 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_continue_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_plan_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/training_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/src/rxn/onmt_models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:13.603381 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-02 08:16:13.000000 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-02 08:16:13.000000 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:16:13.000000 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 08:16:13.000000 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:16:13.000000 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 08:16:13.000000 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 08:16:13.000000 rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:16:13.603381 rxn-onmt-models-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/tests/test_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/tests/test_prediction_collapser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/tests/test_prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-02 08:16:03.000000 rxn-onmt-models-1.0.1/tests/test_utils.py
```

### Comparing `rxn-onmt-models-1.0.0/LICENSE` & `rxn-onmt-models-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/PKG-INFO` & `rxn-onmt-models-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: rxn-onmt-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Training of OpenNMT-based RXN models
 Home-page: https://github.com/rxn4chemistry/rxn-onmt-models
 Author: IBM RXN team
 License: MIT
 Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-onmt-models/
 Project-URL: Repository, https://github.com/rxn4chemistry/rxn-onmt-models
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: rdkit
 License-File: LICENSE
 
 # RXN package for OpenNMT-based models
```

### Comparing `rxn-onmt-models-1.0.0/README.md` & `rxn-onmt-models-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/setup.cfg` & `rxn-onmt-models-1.0.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 project_urls = 
 	Documentation = https://rxn4chemistry.github.io/rxn-onmt-models/
 	Repository = https://github.com/rxn4chemistry/rxn-onmt-models
 classifiers = 
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
 python_requires = >= 3.6
 zip_safe = False
 include_package_data = True
 install_requires = 
 	attrs>=21.2.0
 	click>=8.0
 	rxn-chem-utils>=1.1.4
-	rxn-onmt-utils>=1.0.0
+	rxn-onmt-utils>=1.0.3
 	rxn-reaction-preprocessing>=2.0.2
 	rxn-utils>=1.1.9
 
 [options.packages.find]
 where = src
 
 [options.package_data]
```

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/augmentation.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/augmentation.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/prediction_collapser.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/prediction_collapser.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/prediction_utils.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_augment.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_augment.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_continue_training.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_continue_training.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 @click.option(
     "--data_weights",
     type=int,
     multiple=True,
     help="Weights of the different data sets for training. Only needed in a multi-task setting.",
 )
 @click.option(
+    "--keep_checkpoint",
+    type=int,
+    default=defaults.KEEP_CHECKPOINT,
+    help='How many checkpoints to keep ("-1" means "keep all").',
+)
+@click.option(
     "--model_output_dir", type=str, required=True, help="Where to save the models"
 )
 @click.option("--no_gpu", is_flag=True, help="Run the training on CPU (slow!)")
 @click.option(
     "--preprocess_dir",
     type=str,
     required=True,
@@ -50,14 +56,15 @@
     "--train_num_steps",
     default=100000,
     help="Number of steps, including steps from the initial training run.",
 )
 def main(
     batch_size: int,
     data_weights: Tuple[int, ...],
+    keep_checkpoint: int,
     model_output_dir: str,
     no_gpu: bool,
     preprocess_dir: str,
     train_from: Optional[str],
     train_num_steps: int,
 ) -> None:
     """Continue training for an OpenNMT model.
@@ -92,14 +99,15 @@
     config_file = model_files.next_config_file()
     dropout = get_model_dropout(train_from)
     seed = get_model_seed(train_from)
 
     train_cmd = OnmtTrainCommand.continue_training(
         batch_size=batch_size,
         data=onmt_preprocessed_files.preprocess_prefix,
+        keep_checkpoint=keep_checkpoint,
         dropout=dropout,
         save_model=model_files.model_prefix,
         seed=seed,
         train_from=train_from,
         train_steps=train_num_steps,
         no_gpu=no_gpu,
         data_weights=data_weights,
```

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_finetune.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_finetune.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 @click.option(
     "--data_weights",
     type=int,
     multiple=True,
     help="Weights of the different data sets for training. Only needed in a multi-task setting.",
 )
 @click.option("--dropout", default=defaults.DROPOUT)
+@click.option(
+    "--keep_checkpoint",
+    type=int,
+    default=defaults.KEEP_CHECKPOINT,
+    help='How many checkpoints to keep ("-1" means "keep all").',
+)
 @click.option("--learning_rate", type=float, default=0.06)
 @click.option(
     "--model_output_dir", type=str, required=True, help="Where to save the models"
 )
 @click.option("--no_gpu", is_flag=True, help="Run the training on CPU (slow!)")
 @click.option(
     "--preprocess_dir",
@@ -48,14 +54,15 @@
 @click.option("--warmup_steps", default=defaults.WARMUP_STEPS)
 @click.option("--report_every", default=1000)
 @click.option("--save_checkpoint_steps", default=5000)
 def main(
     batch_size: int,
     data_weights: Tuple[int, ...],
     dropout: float,
+    keep_checkpoint: int,
     learning_rate: float,
     model_output_dir: str,
     no_gpu: bool,
     preprocess_dir: str,
     seed: int,
     train_from: str,
     train_num_steps: int,
@@ -99,14 +106,15 @@
 
     config_file = model_files.next_config_file()
 
     train_cmd = OnmtTrainCommand.finetune(
         batch_size=batch_size,
         data=onmt_preprocessed_files.preprocess_prefix,
         dropout=dropout,
+        keep_checkpoint=keep_checkpoint,
         learning_rate=learning_rate,
         rnn_size=rnn_size,
         save_model=model_files.model_prefix,
         seed=seed,
         train_from=train_from,
         train_steps=train_num_steps,
         warmup_steps=warmup_steps,
```

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_preprocess.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_preprocess.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_onmt_train.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_onmt_train.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     "--data_weights",
     type=int,
     multiple=True,
     help="Weights of the different data sets for training. Only needed in a multi-task setting.",
 )
 @click.option("--dropout", default=defaults.DROPOUT)
 @click.option("--heads", default=defaults.HEADS)
+@click.option(
+    "--keep_checkpoint",
+    type=int,
+    default=defaults.KEEP_CHECKPOINT,
+    help='How many checkpoints to keep ("-1" means "keep all").',
+)
 @click.option("--layers", default=defaults.LAYERS)
 @click.option("--learning_rate", type=float, default=defaults.LEARNING_RATE)
 @click.option(
     "--model_output_dir", type=str, required=True, help="Where to save the models"
 )
 @click.option("--no_gpu", is_flag=True, help="Run the training on CPU (slow!)")
 @click.option(
@@ -44,14 +50,15 @@
 @click.option("--warmup_steps", default=defaults.WARMUP_STEPS)
 @click.option("--word_vec_size", default=defaults.WORD_VEC_SIZE)
 def main(
     batch_size: int,
     data_weights: Tuple[int, ...],
     dropout: float,
     heads: int,
+    keep_checkpoint: int,
     layers: int,
     learning_rate: float,
     model_output_dir: str,
     no_gpu: bool,
     preprocess_dir: str,
     rnn_size: int,
     seed: int,
@@ -82,14 +89,15 @@
     config_file = model_files.next_config_file()
 
     train_cmd = OnmtTrainCommand.train(
         batch_size=batch_size,
         data=onmt_preprocessed_files.preprocess_prefix,
         dropout=dropout,
         heads=heads,
+        keep_checkpoint=keep_checkpoint,
         layers=layers,
         learning_rate=learning_rate,
         rnn_size=rnn_size,
         save_model=model_files.model_prefix,
         seed=seed,
         train_steps=train_num_steps,
         transformer_ff=transformer_ff,
```

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_plan_training.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_plan_training.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_prepare_data.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_prepare_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from rxn.onmt_utils import __version__ as onmt_utils_version
 from rxn.reaction_preprocessing.config import (
     CommonConfig,
     Config,
     DataConfig,
     FragmentBond,
     InitialDataFormat,
+    PreprocessConfig,
     RxnImportConfig,
     SplitConfig,
     StandardizeConfig,
 )
 from rxn.reaction_preprocessing.main import preprocess_data
 from rxn.utilities.logging import setup_console_and_file_logger
 
@@ -39,25 +40,35 @@
 @click.option(
     "--output_dir",
     type=str,
     required=True,
     help="Directory where to save the generated files",
 )
 @click.option(
+    "--min_reactants",
+    type=int,
+    default=2,
+    help=(
+        "Minimum number of precursors / reactants. "
+        "Reactions with fewer precursors than that will be discarded."
+    ),
+)
+@click.option(
     "--split_seed", default=defaults.SEED, help="Random seed for splitting step"
 )
 @click.option(
     "--fragment_bond",
     type=click.Choice(["DOT", "TILDE"], case_sensitive=False),
     default="DOT",
 )
 def main(
     input_data: str,
     import_from: str,
     output_dir: str,
+    min_reactants: int,
     split_seed: int,
     fragment_bond: str,
 ) -> None:
     """Preprocess the data to generate a dataset for training transformer models.
 
     The script will automatically generate the following files in output_dir:
         data.imported.csv
@@ -103,14 +114,15 @@
             name=RxnPreprocessingFiles.FILENAME_ROOT,
         ),
         common=CommonConfig(fragment_bond=FragmentBond[fragment_bond]),
         rxn_import=import_config,
         standardize=StandardizeConfig(
             annotation_file_paths=[], discard_unannotated_metals=False
         ),
+        preprocess=PreprocessConfig(min_reactants=min_reactants),
         split=SplitConfig(hash_seed=split_seed),
     )
 
     try:
         logger.info("Running the data preprocessing")
         preprocess_data(cfg)
     except Exception as e:
```

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/scripts/rxn_translate.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/scripts/rxn_translate.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/training_files.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/training_files.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/translation.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/translation.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn/onmt_models/utils.py` & `rxn-onmt-models-1.0.1/src/rxn/onmt_models/utils.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/PKG-INFO` & `rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: rxn-onmt-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Training of OpenNMT-based RXN models
 Home-page: https://github.com/rxn4chemistry/rxn-onmt-models
 Author: IBM RXN team
 License: MIT
 Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-onmt-models/
 Project-URL: Repository, https://github.com/rxn4chemistry/rxn-onmt-models
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: rdkit
 License-File: LICENSE
 
 # RXN package for OpenNMT-based models
```

### Comparing `rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/SOURCES.txt` & `rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/src/rxn_onmt_models.egg-info/entry_points.txt` & `rxn-onmt-models-1.0.1/src/rxn_onmt_models.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/tests/test_augmentation.py` & `rxn-onmt-models-1.0.1/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/tests/test_prediction_collapser.py` & `rxn-onmt-models-1.0.1/tests/test_prediction_collapser.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/tests/test_prediction_utils.py` & `rxn-onmt-models-1.0.1/tests/test_prediction_utils.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-models-1.0.0/tests/test_utils.py` & `rxn-onmt-models-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

