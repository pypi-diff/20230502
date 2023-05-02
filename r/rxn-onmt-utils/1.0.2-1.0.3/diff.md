# Comparing `tmp/rxn-onmt-utils-1.0.2.tar.gz` & `tmp/rxn-onmt-utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-onmt-utils-1.0.2.tar", last modified: Thu Apr 13 15:36:39 2023, max compression
+gzip compressed data, was "rxn-onmt-utils-1.0.3.tar", last modified: Tue May  2 08:03:35 2023, max compression
```

## Comparing `rxn-onmt-utils-1.0.2.tar` & `rxn-onmt-utils-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.470267 rxn-onmt-utils-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.466266 rxn-onmt-utils-1.0.2/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.470267 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/internal_translation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.470267 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/strip_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/train_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:35.026493 rxn-onmt-utils-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-02 08:03:35.030493 rxn-onmt-utils-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-02 08:03:35.030493 rxn-onmt-utils-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:35.022493 rxn-onmt-utils-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:35.018493 rxn-onmt-utils-1.0.3/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:35.026493 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/internal_translation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/model_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/model_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:35.026493 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/scripts/strip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/scripts/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/train_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-02 08:03:23.000000 rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:03:35.026493 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-02 08:03:35.000000 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-02 08:03:35.000000 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:03:35.000000 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 08:03:35.000000 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:03:34.000000 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 08:03:35.000000 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 08:03:35.000000 rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/top_level.txt
```

### Comparing `rxn-onmt-utils-1.0.2/LICENSE` & `rxn-onmt-utils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/PKG-INFO` & `rxn-onmt-utils-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-onmt-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utilities related to the use of OpenNMT
 Home-page: https://github.com/rxn4chemistry/rxn-onmt-utils
 Author: IBM RXN team
 License: MIT
 Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-onmt-utils/
 Project-URL: Repository, https://github.com/rxn4chemistry/rxn-onmt-utils
 Classifier: Operating System :: OS Independent
```

### Comparing `rxn-onmt-utils-1.0.2/README.md` & `rxn-onmt-utils-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/setup.cfg` & `rxn-onmt-utils-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/internal_translation_utils.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/internal_translation_utils.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_introspection.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/model_introspection.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_resize.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/model_resize.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/translate.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/scripts/translate.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/train_command.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/train_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     Arg("decay_method", "noam", RxnCommand.TF),
     Arg("decoder_type", "transformer", RxnCommand.T),
     Arg("dropout", None, RxnCommand.TCF),
     Arg("encoder_type", "transformer", RxnCommand.T),
     Arg("global_attention", "general", RxnCommand.T),
     Arg("global_attention_function", "softmax", RxnCommand.T),
     Arg("heads", None, RxnCommand.T),
-    Arg("keep_checkpoint", "20", RxnCommand.TCF),
+    Arg("keep_checkpoint", "-1", RxnCommand.TCF),
     Arg("label_smoothing", "0.0", RxnCommand.TCF),
     Arg("layers", None, RxnCommand.T),
     Arg("learning_rate", None, RxnCommand.TF),
     Arg("max_generator_batches", "32", RxnCommand.TCF),
     Arg("max_grad_norm", "0", RxnCommand.TF),
     Arg("normalization", "tokens", RxnCommand.TCF),
     Arg("optim", "adam", RxnCommand.TF),
@@ -194,23 +194,25 @@
         seed: int,
         train_steps: int,
         transformer_ff: int,
         warmup_steps: int,
         word_vec_size: int,
         no_gpu: bool,
         data_weights: Tuple[int, ...],
+        keep_checkpoint: int = -1,
     ) -> "OnmtTrainCommand":
         return cls(
             command_type=RxnCommand.T,
             no_gpu=no_gpu,
             data_weights=data_weights,
             batch_size=batch_size,
             data=data,
             dropout=dropout,
             heads=heads,
+            keep_checkpoint=keep_checkpoint,
             layers=layers,
             learning_rate=learning_rate,
             rnn_size=rnn_size,
             save_model=save_model,
             seed=seed,
             train_steps=train_steps,
             transformer_ff=transformer_ff,
@@ -226,22 +228,24 @@
         dropout: float,
         save_model: PathLike,
         seed: int,
         train_from: PathLike,
         train_steps: int,
         no_gpu: bool,
         data_weights: Tuple[int, ...],
+        keep_checkpoint: int = -1,
     ) -> "OnmtTrainCommand":
         return cls(
             command_type=RxnCommand.C,
             no_gpu=no_gpu,
             data_weights=data_weights,
             batch_size=batch_size,
             data=data,
             dropout=dropout,
+            keep_checkpoint=keep_checkpoint,
             reset_optim="none",
             save_model=save_model,
             seed=seed,
             train_from=train_from,
             train_steps=train_steps,
         )
 
@@ -257,14 +261,15 @@
         train_from: PathLike,
         train_steps: int,
         warmup_steps: int,
         no_gpu: bool,
         data_weights: Tuple[int, ...],
         report_every: int,
         save_checkpoint_steps: int,
+        keep_checkpoint: int = -1,
         rnn_size: Optional[int] = None,
     ) -> "OnmtTrainCommand":
         if rnn_size is None:
             # In principle, the rnn_size should not be needed for finetuning. However,
             # when resetting the decay algorithm for the learning rate, this value
             # is necessary - and does not get it from the model checkpoint (OpenNMT bug).
             rnn_size = get_model_rnn_size(train_from)
@@ -273,14 +278,15 @@
         return cls(
             command_type=RxnCommand.F,
             no_gpu=no_gpu,
             data_weights=data_weights,
             batch_size=batch_size,
             data=data,
             dropout=dropout,
+            keep_checkpoint=keep_checkpoint,
             learning_rate=learning_rate,
             reset_optim="all",
             rnn_size=rnn_size,
             save_model=save_model,
             seed=seed,
             train_from=train_from,
             train_steps=train_steps,
```

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translate.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/translate.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translator.py` & `rxn-onmt-utils-1.0.3/src/rxn/onmt_utils/translator.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/PKG-INFO` & `rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-onmt-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utilities related to the use of OpenNMT
 Home-page: https://github.com/rxn4chemistry/rxn-onmt-utils
 Author: IBM RXN team
 License: MIT
 Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-onmt-utils/
 Project-URL: Repository, https://github.com/rxn4chemistry/rxn-onmt-utils
 Classifier: Operating System :: OS Independent
```

### Comparing `rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/SOURCES.txt` & `rxn-onmt-utils-1.0.3/src/rxn_onmt_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

