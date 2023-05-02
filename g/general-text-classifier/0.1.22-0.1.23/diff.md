# Comparing `tmp/general_text_classifier-0.1.22-py3-none-any.whl.zip` & `tmp/general_text_classifier-0.1.23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11704 bytes, number of entries: 6
--rw-r--r--  2.0 unx    50950 b- defN 22-Dec-05 11:25 general_text_classifier/__init__.py
--rw-------  2.0 unx     1062 b- defN 22-Dec-05 11:25 general_text_classifier-0.1.22.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1188 b- defN 22-Dec-05 11:25 general_text_classifier-0.1.22.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-05 11:25 general_text_classifier-0.1.22.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 22-Dec-05 11:25 general_text_classifier-0.1.22.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 22-Dec-05 11:25 general_text_classifier-0.1.22.dist-info/RECORD
-6 files, 53884 bytes uncompressed, 10660 bytes compressed:  80.2%
+Zip file size: 12489 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    52704 b- defN 23-May-02 08:06 general_text_classifier/__init__.py
+-rw-------  2.0 unx     1062 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1188 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/RECORD
+6 files, 55638 bytes uncompressed, 11445 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: general_text_classifier/__init__.py
 Comment: 
 
-Filename: general_text_classifier-0.1.22.dist-info/LICENSE.txt
+Filename: general_text_classifier-0.1.23.dist-info/LICENSE.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.22.dist-info/METADATA
+Filename: general_text_classifier-0.1.23.dist-info/METADATA
 Comment: 
 
-Filename: general_text_classifier-0.1.22.dist-info/WHEEL
+Filename: general_text_classifier-0.1.23.dist-info/WHEEL
 Comment: 
 
-Filename: general_text_classifier-0.1.22.dist-info/top_level.txt
+Filename: general_text_classifier-0.1.23.dist-info/top_level.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.22.dist-info/RECORD
+Filename: general_text_classifier-0.1.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## general_text_classifier/__init__.py

```diff
@@ -1,72 +1,100 @@
-import warnings
 from google.cloud import bigquery, storage
 from google.oauth2 import service_account
 from iterstrat.ml_stratifiers import MultilabelStratifiedShuffleSplit
 from pathlib import Path
 from scipy.special import softmax
 from shutil import make_archive, unpack_archive
-from simpletransformers.classification import ClassificationModel, ClassificationArgs, MultiLabelClassificationModel, MultiLabelClassificationArgs
-from sklearn.metrics import classification_report, f1_score, precision_score, recall_score, accuracy_score
+from simpletransformers.classification import (
+    ClassificationModel,
+    ClassificationArgs,
+    MultiLabelClassificationModel,
+    MultiLabelClassificationArgs,
+)
+from sklearn.metrics import (
+    classification_report,
+    f1_score,
+    precision_score,
+    recall_score,
+    accuracy_score,
+)
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder, MultiLabelBinarizer
 from typing import List, Optional
 import glob
 import joblib
 import json
 import numpy as np
 import os
 import pandas as pd
 import shutil
 import copy
+
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 import logging
+
 logging.basicConfig(level=logging.INFO)
 transformers_logger = logging.getLogger("transformers")
 transformers_logger.setLevel(logging.WARNING)
 
+
 def f1_multiclass(labels, preds):
-    return f1_score(labels, preds, average='macro')
+    return (
+        f1_score(labels, preds, average="macro")
+        if len(np.unique(labels)) > 2
+        else f1_score(labels, preds, average="binary")
+    )
+
+
+def precision_multiclass(labels, preds):
+    return (
+        precision_score(labels, preds, average="macro")
+        if len(np.unique(labels)) > 2
+        else precision_score(labels, preds, average="binary")
+    )
 
-def prec_multiclass(labels, preds):
-    return precision_score(labels, preds, average='macro')
 
 def recall_multiclass(labels, preds):
-    return recall_score(labels, preds, average='macro')
+    return (
+        recall_score(labels, preds, average="macro")
+        if len(np.unique(labels)) > 2
+        else recall_score(labels, preds, average="binary")
+    )
 
 
 def create_model_card(
-    model_card_path = "model_card.md",
-    model_title = "Model Title",
-    model_summary = "",
-    team = "",
-    contact_persons = "",
-    project_name = "",
-    project_sheet_url = "",
-    model_date = "",
-    model_version = "",
-    model_type = "",
-    model_target_values = "",
-    useful_links = "",
-    primary_intended_uses = "",
-    primary_intended_users = "",
-    known_biases = "",
-    caveats_recommendations = "",
-    minimal_starter_code = "",
-    used_metrics = "",
-    train_data_path = "",
-    simulation_data_path = "",
-    features = "",
-    data_modifications = "",
-    train_data_summary = "",
-    sim_data_summary = "",
-    does_the_model_use_any_sensitive_data = "",
-    risk_mitigation_strategies = "",
-    model_usage_risks = "",
-    possible_fraught_use_cases = ""):
+    model_card_path="model_card.md",
+    model_title="Model Title",
+    model_summary="",
+    team="",
+    contact_persons="",
+    project_name="",
+    project_sheet_url="",
+    model_date="",
+    model_version="",
+    model_type="",
+    model_target_values="",
+    useful_links="",
+    primary_intended_uses="",
+    primary_intended_users="",
+    known_biases="",
+    caveats_recommendations="",
+    minimal_starter_code="",
+    used_metrics="",
+    train_data_path="",
+    simulation_data_path="",
+    features="",
+    data_modifications="",
+    train_data_summary="",
+    sim_data_summary="",
+    does_the_model_use_any_sensitive_data="",
+    risk_mitigation_strategies="",
+    model_usage_risks="",
+    possible_fraught_use_cases="",
+):
     """Create and save a markdown model card.
 
     Parameters
     ----------
     model_card_path : str, optional
         Path to save the model card, by default "model_card.md"
     model_title : str, optional
@@ -208,422 +236,497 @@
 - **What risks may be present in model usage?** {model_usage_risks}
 - **Are there any known model use cases that are especially fraught?** {possible_fraught_use_cases}
 
 """
 
     with open(model_card_path, "w") as f:
         f.write(model_card)
-    
+
     print(f"--- Model card is saved to {model_card_path} ---")
 
+
 def display_markdown(markdown_path: str):
     """Render and display a markdown file given the markdown path.
 
     Parameters
     ----------
     markdown_path : str
         Path to the markdown file.
     """
     from IPython.display import display, Markdown
+
     with open(markdown_path, "r") as f:
         md = f.read()
+        
     display(Markdown(md))
 
-        
+
 class TextClassifier:
-    def __init__(self,
-                 do_train : bool,
-                 model_dir : str,
-                 classification_type : Optional[str] = "single",
-                 model_type : Optional[str] = "bert",
-                 model_version : Optional[str] = "ty_bert",
-                 gpus_to_use : Optional[List[str]] = [],
-                 exp_args : dict = {},
-                 split_val_data : Optional[bool] = True,
-                 split_size : float = 0.2,
-                 save_onnx_model : Optional[bool] = False,
-                 random_state : Optional[int] = 2022,
-                 gcloud_project_id : Optional[str] = None,
-                 gcloud_bucket_name : Optional[str] = None,
-                 gcloud_blob_name : Optional[str] = None,
-                 gcloud_credentials_path : Optional[str] = None,
-                 nlp_project_id : Optional[str] = None,
-                 nlp_bucket_name : Optional[str] = None,
-                 nlp_blob_name : Optional[str] = None,
-                 nlp_credentials_path : Optional[str] = None) -> None:
-        
+    def __init__(
+        self,
+        do_train: bool,
+        model_dir: str,
+        classification_type: Optional[str] = "single",
+        model_type: Optional[str] = "roberta",
+        model_version: Optional[str] = "ty_roberta",
+        gpus_to_use: Optional[List[str]] = [],
+        exp_args: Optional[dict] = {},
+        do_lowercase: Optional[bool] = True,
+        data_lang: Optional[str] = "tr",
+        split_val_data: Optional[bool] = True,
+        split_size: Optional[float] = 0.2,
+        save_onnx_model: Optional[bool] = False,
+        random_state: Optional[int] = 2022,
+        train_only_final_layer: Optional[bool] = False,
+        freeze_layers_dict: Optional[List] = None,
+        gcloud_project_id: Optional[str] = None,
+        gcloud_bucket_name: Optional[str] = None,
+        gcloud_blob_name: Optional[str] = None,
+        gcloud_credentials_path: Optional[str] = None,
+        nlp_project_id: Optional[str] = None,
+        nlp_bucket_name: Optional[str] = None,
+        nlp_blob_name: Optional[str] = None,
+        nlp_credentials_path: Optional[str] = None,
+    ) -> None:
+
         """General text classification pipeline.
-        Train and Evaluation data needs to be in a Pandas Dataframe containing at least two columns, a 'text' and a 'labels' column. 
+        Train and Evaluation data needs to be in a Pandas Dataframe containing at least two columns, a 'text' and a 'labels' column.
         The `labels` column must be string and seperated by comma values, if multilabel classification will be conducted.
-                
+
 
         Parameters
         ----------
         do_train : bool
             Whether to train a model or take inference.
-        
+
         model_dir : str
             Server model directory to be used during training or inference.
-        
-        classification_type : str
+
+        classification_type : str, optional
             Type of classification task. Only 'single' or 'multi' is allowed.
-        
-        model_type : str
+
+        model_type : str, optional
             Model type to be used by Simple Transformers
-            Please consider using 'bert' for Turkish data and 'distilbert' for multilingual data.
-        
-        model_version : str
+            Please consider using 'bert' or 'roberta' for Turkish data and 'distilbert' for multilingual data.
+
+        model_version : str, optional
             Model version to be used by Simple Transformers.
-            Please consider using 'dbmdz/bert-base-turkish-cased' or 'ty_bert' for Turkish data
+            Please consider using 'dbmdz/bert-base-turkish-cased', 'ty_bert', 'ty_roberta' for Turkish data
             and 'sentence-transformers/distiluse-base-multilingual-cased-v2' for multilingual data.
-            
-        gpus_to_use : list of str
+
+        gpus_to_use : list of str, optional
             Available GPU list for training & inference.
-        
-        exp_args: dict
+
+        exp_args: dict, optional
             Simple Transformers model arguments which can be used during training.
+
+        do_lowercase: bool, optional
+            Whether to convert text to lowercase or not.
         
-        split_val_data : bool
+        data_lang: str, optional
+            Language of the data to be trained on.
+
+        split_val_data : bool, optional
             Whether to split training data into training & validation data for model training or not.
-        
-        split_size : bool
+
+        split_size : bool, optional
             Data split size into training & validation sets. Valid if split_val_data == True.
-        
+
         save_onnx_model : bool, optional
             Whether to upload only the ONNX model to GCS or not.
-        
+
         random_state : int, optional
             Random seed for reproducibility
-        
-        gcloud_project_id : str
+
+        train_only_last_layer: bool, optional
+            Whether to train / finetune only the final layer (classification head) or full training (full training may result with overfitting, training only the last layer is recommended).
+
+        freeze_layers_dict: list, optional
+            Model layer config list to be freezed (not trained). Required when train_only_last_layer == True.
+
+        gcloud_project_id : str, optional
             Name of the Google Cloud project.
-        
-        gcloud_bucket_name : str
+
+        gcloud_bucket_name : str, optional
             Name of the GCS bucket.
-        
-        gcloud_blob_name : str
-            Path to GCS bucket for model saving.  
-            
-        gcloud_credentials_path : str
-            Name of the Google Cloud credentials for the project. must be given if model_version == 'ty_bert'.
-        
-        nlp_project_id : str
-            Name of the Google Cloud project for NLP project. must be given if model_version == 'ty_bert'.
-        
-        nlp_bucket_name : str
-            Name of the Google Cloud bucket name for NLP project. must be given if model_version == 'ty_bert'.
-        
-        nlp_blob_name : str
-            Name of the Google Cloud blob name for NLP project. must be given if model_version == 'ty_bert'.
-        
-        nlp_credentials_path : str
-            Name of the Google Cloud credentials for NLP project. must be given if model_version == 'ty_bert'.
-        
-        
+
+        gcloud_blob_name : str, optional
+            Path to GCS bucket for model saving.
+
+        gcloud_credentials_path : str, optional
+            Name of the Google Cloud credentials for the project. must be given if model_version is 'ty_bert' or 'ty_roberta'.
+
+        nlp_project_id : str, optional
+            Name of the Google Cloud project for NLP project. must be given if model_version is 'ty_bert' or 'ty_roberta'.
+
+        nlp_bucket_name : str, optional
+            Name of the Google Cloud bucket name for NLP project. must be given if model_version is 'ty_bert' or 'ty_roberta'.
+
+        nlp_blob_name : str, optional
+            Name of the Google Cloud blob name for NLP project. must be given if model_version is 'ty_bert' or 'ty_roberta'.
+
+        nlp_credentials_path : str, optional
+            Name of the Google Cloud credentials for NLP project. must be given if model_version is 'ty_bert' or 'ty_roberta'.
+
+
         Returns
         -------
         None
 
         """
+        
         # session is starting...
         self.print_log_messages(0)
-        
+
         self.gpus_to_use = gpus_to_use
         self.do_train = do_train
         self.model_dir = model_dir
-        
+        self.do_lowercase = do_lowercase
+        self.train_only_final_layer = train_only_final_layer
+        self.freeze_layers_dict = freeze_layers_dict
+        self.data_lang = data_lang
+
+        if self.train_only_final_layer:
+            assert (
+                self.freeze_layers_dict is not None
+            ), "Please provide freeze_layers_dict to train only the final layer for the current model. You can use https://simpletransformers.ai/docs/tips-and-tricks/#custom-parameter-groups for customization."
+
         # setup GPUs if available
         if len(self.gpus_to_use):
-            os.environ["CUDA_VISIBLE_DEVICES"]=",".join(self.gpus_to_use)
-        
+            os.environ["CUDA_VISIBLE_DEVICES"] = ",".join(self.gpus_to_use)
+
         # GCS params
         self.gcloud_project_id = gcloud_project_id
         self.gcloud_bucket_name = gcloud_bucket_name
         self.gcloud_blob_name = gcloud_blob_name
         self.gcloud_project_id = gcloud_project_id
         self.gcloud_credentials_path = gcloud_credentials_path
-        
+
         if self.gcloud_project_id is not None:
             # setup credentials for big query & GCS
-            assert os.path.exists(self.gcloud_credentials_path), self.print_error_messages(0)
-        
+            assert os.path.exists(
+                self.gcloud_credentials_path
+            ), self.print_error_messages(0)
+
             # make GCS connection
             with open(self.gcloud_credentials_path) as json_file:
                 connection_info_gcs = json.load(json_file)
 
-            credentials = service_account.Credentials.from_service_account_info(connection_info_gcs)
-            self.bigq_client = bigquery.Client(credentials=credentials, 
-                                               project=self.gcloud_project_id)
+            credentials = service_account.Credentials.from_service_account_info(
+                connection_info_gcs
+            )
+            self.bigq_client = bigquery.Client(
+                credentials=credentials, project=self.gcloud_project_id
+            )
 
-            self.storage_client = storage.Client(credentials=credentials, 
-                                                 project=self.gcloud_project_id)
+            self.storage_client = storage.Client(
+                credentials=credentials, project=self.gcloud_project_id
+            )
 
             # setup credentials
             self.print_log_messages(1)
-        
-        
+
         if self.do_train:
             # create model arguments
-            assert classification_type in ["single", "multi"], self.print_error_messages(1)
+            assert classification_type in [
+                "single",
+                "multi",
+            ], self.print_error_messages(1)
             self.classification_type = classification_type
             self.split_val_data = split_val_data
             self.split_size = split_size
             self.random_state = random_state
-        
+
             if self.classification_type == "single":
                 self.classification_model_obj = ClassificationModel
                 self.classification_args_obj = ClassificationArgs
 
             elif self.classification_type == "multi":
                 self.classification_model_obj = MultiLabelClassificationModel
                 self.classification_args_obj = MultiLabelClassificationArgs
-                
+
             self.model_args = {
                 "use_early_stopping": False,
-                "do_lower_case": True,
+                "do_lower_case": True if self.data_lang != "tr" else False,
                 "early_stopping_consider_epochs": False,
                 "early_stopping_delta": 0.0001,
                 "early_stopping_metric": "eval_loss",
-                "early_stopping_metric_minimize":  True,
+                "early_stopping_metric_minimize": True,
                 "early_stopping_patience": 5,
-                "eval_batch_size": 64,
-                "train_batch_size": 32,
+                "eval_batch_size": 16,
+                "train_batch_size": 16,
                 "n_gpu": len(self.gpus_to_use),
                 "evaluate_during_training": True,
                 "evaluate_during_training_silent": False,
                 "save_model_every_epoch": False,
                 "fp16": True,
                 "num_train_epochs": 3,
                 "reprocess_input_data": True,
-                "output_dir":  os.path.join(self.model_dir, "outputs/"),
+                "output_dir": os.path.join(self.model_dir, "outputs/"),
                 "best_model_dir": os.path.join(self.model_dir, "best_model/"),
                 "cache_dir": os.path.join(self.model_dir, "cache_dir/"),
                 "overwrite_output_dir": True,
                 "use_multiprocessing": False,
                 "use_multiprocessing_for_evaluation": False,
-                "manual_seed": self.random_state
+                "manual_seed": self.random_state,
             }
 
             self.model_args = {**self.model_args, **exp_args}
             self.model_type = model_type
             self.model_version = model_version
             self.save_onnx_model = save_onnx_model
             self.split_size = split_size
-            
-            
+
             # create BigQ directories
-            if self.model_version == 'ty_bert':               
+            if self.model_version in ["ty_bert", "ty_roberta"]:
                 assert nlp_credentials_path is not None, self.print_error_messages(2)
-                assert os.path.exists(nlp_credentials_path), self.print_error_messages(3)
+                assert os.path.exists(nlp_credentials_path), self.print_error_messages(
+                    3
+                )
                 assert nlp_project_id is not None, self.print_error_messages(14)
                 assert nlp_bucket_name is not None, self.print_error_messages(15)
                 assert nlp_blob_name is not None, self.print_error_messages(16)
-                
+
                 # setup credentials for internal ty-bert model
                 with open(nlp_credentials_path) as json_file:
                     connection_info_nlp = json.load(json_file)
-                
-                credentials = service_account.Credentials.from_service_account_info(connection_info_nlp)
-                storage_client = storage.Client(credentials=credentials, 
-                                                project=nlp_project_id)
-                
-                
+
+                credentials = service_account.Credentials.from_service_account_info(
+                    connection_info_nlp
+                )
+                storage_client = storage.Client(
+                    credentials=credentials, project=nlp_project_id
+                )
+
+                self.model_version_raw = self.model_version
+
                 # download the ty-bert model
-                self.model_version = os.path.join(self.model_dir, "ty_bert")
-                
-                self.download_from_gcs(storage_client,
-                                       os.path.join(self.model_dir, "ty_bert", "best_model.tar.gz"),
-                                       nlp_bucket_name,
-                                       nlp_blob_name)
-                
-                unpack_archive(os.path.join(self.model_dir, "ty_bert", "best_model.tar.gz"),
-                               extract_dir = self.model_version,
-                               format='gztar')
-                
-                
+                self.model_version = os.path.join(self.model_dir, self.model_version_raw)
+
+                self.download_from_gcs(
+                    storage_client,
+                    os.path.join(self.model_dir, self.model_version_raw, "best_model.tar.gz"),
+                    nlp_bucket_name,
+                    nlp_blob_name,
+                )
+
+                unpack_archive(
+                    os.path.join(self.model_dir, self.model_version_raw, "best_model.tar.gz"),
+                    extract_dir=self.model_version,
+                    format="gztar",
+                )
+
             # arrange directory parameters
             self.model_dir_splitted = os.path.split(self.model_dir)
-            
-            self.label_encoder_dir = os.path.join(self.model_dir_splitted[0],
-                                                  self.model_dir_splitted[-1],
-                                                  "best_model" if self.split_val_data else "outputs",
-                                                  "label_encoder.joblib")
-                
-                
-            self.model_metadata_dir = os.path.join(self.model_dir_splitted[0],
-                                                   self.model_dir_splitted[-1],
-                                                   "best_model" if self.split_val_data else "outputs",
-                                                   "model_metadata.joblib")
-            
+
+            self.label_encoder_dir = os.path.join(
+                self.model_dir_splitted[0],
+                self.model_dir_splitted[-1],
+                "best_model" if self.split_val_data else "outputs",
+                "label_encoder.joblib",
+            )
+
+            self.model_metadata_dir = os.path.join(
+                self.model_dir_splitted[0],
+                self.model_dir_splitted[-1],
+                "best_model" if self.split_val_data else "outputs",
+                "model_metadata.joblib",
+            )
+
             if gcloud_blob_name is not None:
-                self.model_bigq_dir = os.path.join(gcloud_blob_name,
-                                                   "best_model.tar.gz" if self.split_val_data else "outputs.tar.gz")
-            
-            
+                self.model_bigq_dir = os.path.join(
+                    gcloud_blob_name,
+                    "best_model.tar.gz" if self.split_val_data else "outputs.tar.gz",
+                )
+
             if save_onnx_model:
-                self.onnx_model_dir = os.path.join(self.model_dir_splitted[0],
-                                                   self.model_dir_splitted[-1],
-                                                   "onnx_model")
-
-                self.label_encoder_onnx_dir = os.path.join(self.model_dir_splitted[0],
-                                                           self.model_dir_splitted[-1],
-                                                           "onnx_model",
-                                                           "label_encoder.joblib")
-
-                self.model_metadata_onnx_dir = os.path.join(self.model_dir_splitted[0],
-                                                            self.model_dir_splitted[-1],
-                                                            "onnx_model",
-                                                            "model_metadata.joblib")
-                
+                self.onnx_model_dir = os.path.join(
+                    self.model_dir_splitted[0],
+                    self.model_dir_splitted[-1],
+                    "onnx_model",
+                )
+
+                self.label_encoder_onnx_dir = os.path.join(
+                    self.model_dir_splitted[0],
+                    self.model_dir_splitted[-1],
+                    "onnx_model",
+                    "label_encoder.joblib",
+                )
+
+                self.model_metadata_onnx_dir = os.path.join(
+                    self.model_dir_splitted[0],
+                    self.model_dir_splitted[-1],
+                    "onnx_model",
+                    "model_metadata.joblib",
+                )
+
                 if gcloud_blob_name is not None:
-                    self.onnx_model_bigq_dir = os.path.join(gcloud_blob_name,
-                                                            "onnx_model.tar.gz")
-                
+                    self.onnx_model_bigq_dir = os.path.join(
+                        gcloud_blob_name, "onnx_model.tar.gz"
+                    )
+
             self.print_log_messages(2)
-            
+
         else:
-            if gcloud_bucket_name is not None:            
+            if gcloud_bucket_name is not None:
                 # download model from GCS
-                self.download_from_gcs(self.storage_client,
-                                       os.path.join(self.model_dir, os.path.split(self.gcloud_blob_name)[-1]),
-                                       self.gcloud_bucket_name,
-                                       self.gcloud_blob_name)
-            
-            extract_path = os.path.join(self.model_dir, 
-                                        os.path.split(self.gcloud_blob_name)[-1]) if self.gcloud_blob_name is not None else self.model_dir
-            
-            
+                self.download_from_gcs(
+                    self.storage_client,
+                    os.path.join(
+                        self.model_dir, os.path.split(self.gcloud_blob_name)[-1]
+                    ),
+                    self.gcloud_bucket_name,
+                    self.gcloud_blob_name,
+                )
+
+            extract_path = (
+                os.path.join(self.model_dir, os.path.split(self.gcloud_blob_name)[-1])
+                if self.gcloud_blob_name is not None
+                else self.model_dir
+            )
+
             # extract model files
-            if not os.path.isdir(extract_path):            
-                unpack_archive(extract_path,
-                               extract_dir = self.model_dir,
-                               format='gztar')
-            
+            if not os.path.isdir(extract_path):
+                unpack_archive(extract_path, extract_dir=self.model_dir, format="gztar")
+
             # read model files
-            self.model_metadata = joblib.load(os.path.join(self.model_dir,
-                                                          "model_metadata.joblib"))
+            self.model_metadata = joblib.load(
+                os.path.join(self.model_dir, "model_metadata.joblib")
+            )
+
+            self.label_encoder = joblib.load(
+                os.path.join(self.model_dir, "label_encoder.joblib")
+            )
 
-            self.label_encoder = joblib.load(os.path.join(self.model_dir,
-                                                          "label_encoder.joblib"))
-            
             self.classification_type = self.model_metadata["task_type"]
 
-            if self.classification_type == 'single':
-                self.model = ClassificationModel(self.model_metadata["model_type"],
-                                                 self.model_dir,
-                                                 use_cuda = True if len(self.gpus_to_use) else False)
+            if self.classification_type == "single":
+                self.model = ClassificationModel(
+                    self.model_metadata["model_type"],
+                    self.model_dir,
+                    use_cuda=True if len(self.gpus_to_use) else False,
+                )
             else:
-                self.model = MultiLabelClassificationModel(self.model_metadata["model_type"],
-                                                           self.model_dir,
-                                                           use_cuda = True if len(self.gpus_to_use) else False)
+                self.model = MultiLabelClassificationModel(
+                    self.model_metadata["model_type"],
+                    self.model_dir,
+                    use_cuda=True if len(self.gpus_to_use) else False,
+                )
 
             self.print_log_messages(10)
-    
-    
-    
+
     @staticmethod
-    def upload_to_gcs(storage_client, local_path: str, dest_bucket_name: str, dest_blob_name: str):
+    def upload_to_gcs(
+        storage_client, local_path: str, dest_bucket_name: str, dest_blob_name: str
+    ):
         """Helper for uploading files to GCS.
 
         Parameters
         ----------
         storage_client : storage.Client
             GCS client object
-        
+
         local_path : str
             Path for files in the server
-        
+
         dest_bucket_name : str
             GCS bucket name
-        
+
         dest_blob_name : str
             GCS file path
-         
-        
+
+
         Returns
         -------
         None
 
         """
         bucket = storage_client.get_bucket(dest_bucket_name)
         if os.path.isfile(local_path):
             blob = bucket.blob(dest_blob_name)
             blob.upload_from_filename(local_path)
         else:
-            rel_paths = [p for p in glob.glob(local_path + '/**', recursive=True)]
+            rel_paths = [p for p in glob.glob(local_path + "/**", recursive=True)]
             for local_file in rel_paths:
-                remote_path = os.path.join(dest_blob_name,local_file.replace(local_path+"/", ""))
+                remote_path = os.path.join(
+                    dest_blob_name, local_file.replace(local_path + "/", "")
+                )
                 if os.path.isfile(local_file):
                     blob = bucket.blob(remote_path)
                     blob.upload_from_filename(local_file)
 
-
     @staticmethod
-    def download_from_gcs(storage_client, dest_path: str, bucket_name: str, blob_name: str, overwrite=True):
+    def download_from_gcs(
+        storage_client, dest_path: str, bucket_name: str, blob_name: str, overwrite=True
+    ):
         """Helper for downloading files from GCS.
 
         Parameters
         ----------
         storage_client : storage.Client
             GCS client object
-        
+
         dest_path : str
             Path for downloading files to the server
-        
+
         bucket_name : str
             GCS bucket name
-        
+
         blob_name : str
             GCS file path
-        
+
         overwrite : bool
             Whether to overwrite files in the path or not.
-        
-        
+
+
         Returns
         -------
         None
 
         """
         bucket = storage_client.get_bucket(bucket_name)
         if not os.path.exists(dest_path) or overwrite:
             blobs = bucket.list_blobs(prefix=blob_name)  # Get list of files
             for blob in blobs:
                 if blob.name.endswith("/"):
                     continue
-                file_split = [s for s in blob.name.replace(blob_name, "").split("/") if len(s) > 0]
+                file_split = [
+                    s for s in blob.name.replace(blob_name, "").split("/") if len(s) > 0
+                ]
                 if len(file_split) > 0:
-                    directory =  "/".join([dest_path, "/".join(file_split)])
+                    directory = "/".join([dest_path, "/".join(file_split)])
                 else:
                     directory = dest_path
                 if len(file_split) > 0:
-                    Path(directory[:-len(file_split[-1])]).mkdir(parents=True, exist_ok=True)
+                    Path(directory[: -len(file_split[-1])]).mkdir(
+                        parents=True, exist_ok=True
+                    )
                 else:
                     Path(directory).parent.absolute().mkdir(parents=True, exist_ok=True)
                 blob.download_to_filename(directory)
         else:
-            print("The destination path already exists. If you want to overwrite, give overwrite parameter as True.")
+            print(
+                "The destination path already exists. If you want to overwrite, give overwrite parameter as True."
+            )
 
-    
-    
     @staticmethod
-    def print_log_messages(log_code : int):
+    def print_log_messages(log_code: int):
         """Helper for printing log messages.
 
         Parameters
         ----------
         log_code : int
             Log message code.
-        
+
         Returns
         -------
         None
 
         """
-        
+
         log_message_dict = {
             0: "--- Session is started. ---",
             1: "--- Connected to GCP. ---",
             2: "--- Model parameters are ready for training. ---",
             3: "--- Splitting data into train / val sets for training... ---",
             4: "--- Encoding labels... ---",
             6: "--- Model training is started. ---",
@@ -634,549 +737,682 @@
             11: "--- Model prediction is started. ---",
             12: "--- Ground truth labels are found in the data, printing classification report... ---\n",
             13: "--- Overwriting prediction results to the given table... ---",
             14: "--- Prediction results are saved to the result_save_path. ---",
             15: "--- Model prediction is completed. You can get the results with TextClassifier(...).test_data. ---",
             16: "--- You can also get the classification report result object with TextClassifier(...).cls_report. ---",
         }
-        
+
         print(log_message_dict[log_code])
-    
-    
+
     @staticmethod
-    def print_error_messages(error_code : int):
+    def print_error_messages(error_code: int):
         """Helper for printing error messages.
 
         Parameters
         ----------
         error_code : int
             Error message code.
-        
+
         Returns
         -------
         None
 
         """
-        
+
         error_message_dict = {
-                0: "Credentials path does not exist, check the path.",
-                1: "Given classification_type is not supported. Only 'single' or 'multi' is allowed.",
-                2: "nlp_credentials_path must be given if model_version == 'ty_bert'",
-                3: "nlp_credentials_path does not exist, check the path.",
-                4: "Bigquery train data table is empty, check the table.",
-                5: "'text' column does not exist in the train table. Check the columns.",
-                6: "'labels' column does not exist in the train table. Check the columns.",
-                7: "Null rows exist in the 'text' column, check the data in train table.",
-                8: "Null rows exist in the 'labels' column, check the data in train table.",
-                9: "Either test_table_name or test_data must be given.",
-                10: "test_table_name must be str, check the parameter.",
-                11: "test_data must be pd.DataFrame, check the parameter.",
-                12: "Either train_table_name or train_data must be given.",
-                13: "BigQuery credentials path does not exist, check the path.",
-                14: "nlp_project_id must be given if model_version == 'ty_bert'",
-                15: "nlp_bucket_name must be given if model_version == 'ty_bert'",
-                16: "nlp_blob_name must be given if model_version == 'ty_bert'",
-                17: "gcloud_project_id must be given during class initialization if you want to use a BigQuery table during model training.",
-                18: "gcloud_bucket_name must be given during class initialization if you want to use a BigQuery table during model training.",
-                19: "gcloud_blob_name must be given during class initialization if you want to use a BigQuery table during model training.",
-                20: "gcloud_credentials_path must be given during class initialization if you want to use a BigQuery table during model training.",
-                21: "Bigquery validation data table is empty, check the table.",
-                22: "'text' column does not exist in the validation table. Check the columns.",
-                23: "'labels' column does not exist in the validation table. Check the columns.",
-                24: "Null rows exist in the 'text' column, check the data in validation table.",
-                25: "Null rows exist in the 'labels' column, check the data in validation table.",
+            0: "Credentials path does not exist, check the path.",
+            1: "Given classification_type is not supported. Only 'single' or 'multi' is allowed.",
+            2: "nlp_credentials_path must be given if model_version is 'ty_bert' or 'ty_roberta'",
+            3: "nlp_credentials_path does not exist, check the path.",
+            4: "Bigquery train data table is empty, check the table.",
+            5: "'text' column does not exist in the train table. Check the columns.",
+            6: "'labels' column does not exist in the train table. Check the columns.",
+            7: "Null rows exist in the 'text' column, check the data in train table.",
+            8: "Null rows exist in the 'labels' column, check the data in train table.",
+            9: "Either test_table_name or test_data must be given.",
+            10: "test_table_name must be str, check the parameter.",
+            11: "test_data must be pd.DataFrame, check the parameter.",
+            12: "Either train_table_name or train_data must be given.",
+            13: "BigQuery credentials path does not exist, check the path.",
+            14: "nlp_project_id must be given if model_version is 'ty_bert' or 'ty_roberta'",
+            15: "nlp_bucket_name must be given if model_version is 'ty_bert' or 'ty_roberta'",
+            16: "nlp_blob_name must be given if model_version is 'ty_bert' or 'ty_roberta'",
+            17: "gcloud_project_id must be given during class initialization if you want to use a BigQuery table during model training.",
+            18: "gcloud_bucket_name must be given during class initialization if you want to use a BigQuery table during model training.",
+            19: "gcloud_blob_name must be given during class initialization if you want to use a BigQuery table during model training.",
+            20: "gcloud_credentials_path must be given during class initialization if you want to use a BigQuery table during model training.",
+            21: "Bigquery validation data table is empty, check the table.",
+            22: "'text' column does not exist in the validation table. Check the columns.",
+            23: "'labels' column does not exist in the validation table. Check the columns.",
+            24: "Null rows exist in the 'text' column, check the data in validation table.",
+            25: "Null rows exist in the 'labels' column, check the data in validation table.",
         }
 
         return error_message_dict[error_code]
-        
-        
+
+    @staticmethod
+    def lowercase_turkish(text: str) -> str:
+        """Helper for lowercasing Turkish text.
+
+        Parameters
+        ----------
+        text : str
+            Any text
+
+        Returns
+        -------
+        str
+            Lowercased text
+
+        """
+
+        return text.translate(str.maketrans("ĞIİÖÜŞÇ", "ğıiöüşç")).lower()
+
     def encode_labels(self, train_data=None, val_data=None):
         """Helper for encoding text labels.
 
         Parameters
         ----------
         train_data : pd.DataFrame
             Training data which labels are to be encoded.
-        
+
         val_data : pd.DataFrame
             Validation data which labels are to be encoded.
-        
+
         Returns
         -------
         None
 
         """
-        
+
         if self.do_train:
             train_data["labels_original"] = train_data["labels"].tolist()
-            
+
             if val_data is not None:
                 val_data["labels_original"] = val_data["labels"].tolist()
-                
+
             if self.classification_type == "single":
                 label_encoder = LabelEncoder()
-            
+
             else:
                 label_encoder = MultiLabelBinarizer()
-                train_data["labels"] = train_data["labels"].apply(lambda x: [elem.strip() for elem in x.split(",")])
-                
+                train_data["labels"] = train_data["labels"].apply(
+                    lambda x: [elem.strip() for elem in x.split(",")]
+                )
+
                 if val_data is not None:
-                    val_data["labels"] = val_data["labels"].apply(lambda x: [elem.strip() for elem in x.split(",")])
-            
-            train_data["labels"] = label_encoder.fit_transform(train_data["labels"].tolist()).tolist()
-            
+                    val_data["labels"] = val_data["labels"].apply(
+                        lambda x: [elem.strip() for elem in x.split(",")]
+                    )
+
+            train_data["labels"] = label_encoder.fit_transform(
+                train_data["labels"].tolist()
+            ).tolist()
+
             if val_data is not None:
-                val_data["labels"] = label_encoder.transform(val_data["labels"].tolist()).tolist()
-                    
+                val_data["labels"] = label_encoder.transform(
+                    val_data["labels"].tolist()
+                ).tolist()
+
             return [train_data, val_data, label_encoder]
-            
+
         else:
             val_data["labels_original"] = val_data["labels"].tolist()
-            
+
             if self.classification_type == "multi":
-                val_data["labels"] = val_data["labels"].apply(lambda x: [elem.strip() for elem in x.split(",")])
-            
-            val_data["labels"] = self.label_encoder.transform(val_data["labels"].tolist()).tolist()
+                val_data["labels"] = val_data["labels"].apply(
+                    lambda x: [elem.strip() for elem in x.split(",")]
+                )
+
+            val_data["labels"] = self.label_encoder.transform(
+                val_data["labels"].tolist()
+            ).tolist()
             return val_data
-            
 
     def prepare_training_data(self) -> None:
         """Helper for creating training data.
 
         Parameters
         ----------
         None
-        
+
         Returns
         -------
         None
 
         """
-        
+
         # training data is valid, moving to model fitting procedure...
         self.train_data["text"] = self.train_data["text"].astype(str)
-        
+
+        if self.do_lowercase and self.data_lang == "tr":
+            self.train_data["text"] = self.train_data["text"].apply(
+                self.lowercase_turkish
+            )
+
         if self.val_data is not None:
             self.val_data["text"] = self.val_data["text"].astype(str)
             self.split_val_data = False
-        
+
+            if self.do_lowercase and self.data_lang == "tr":
+                self.val_data["text"] = self.val_data["text"].apply(
+                    self.lowercase_turkish
+                )
+
         if self.split_val_data:
             self.print_log_messages(3)
-            
-            if self.classification_type == "single": 
+
+            if self.classification_type == "single":
                 try:
-                    x_train, x_val, y_train, y_val = train_test_split(self.train_data["text"],
-                                                                      self.train_data["labels"],
-                                                                      test_size=self.split_size,
-                                                                      random_state=self.random_state,
-                                                                      stratify=self.train_data["labels"])
+                    x_train, x_val, y_train, y_val = train_test_split(
+                        self.train_data["text"],
+                        self.train_data["labels"],
+                        test_size=self.split_size,
+                        random_state=self.random_state,
+                        stratify=self.train_data["labels"],
+                    )
                 except:
-                    x_train, x_val, y_train, y_val = train_test_split(self.train_data["text"],
-                                                                      self.train_data["labels"],
-                                                                      test_size=self.split_size,
-                                                                      random_state=self.random_state)
-                
-                self.model_train_data = pd.DataFrame({
-                      "text": x_train.values,
-                      "labels": y_train.values
-                })
-
-                self.model_val_data = pd.DataFrame({
-                      "text": x_val.values,
-                      "labels": y_val.values
-                })
-                
+                    x_train, x_val, y_train, y_val = train_test_split(
+                        self.train_data["text"],
+                        self.train_data["labels"],
+                        test_size=self.split_size,
+                        random_state=self.random_state,
+                    )
+
+                self.model_train_data = pd.DataFrame(
+                    {"text": x_train.values, "labels": y_train.values}
+                )
+
+                self.model_val_data = pd.DataFrame(
+                    {"text": x_val.values, "labels": y_val.values}
+                )
+
                 self.print_log_messages(4)
-                self.model_train_data, self.model_val_data, self.label_encoder = self.encode_labels(self.model_train_data, 
-                                                                                                    self.model_val_data)
+                (
+                    self.model_train_data,
+                    self.model_val_data,
+                    self.label_encoder,
+                ) = self.encode_labels(self.model_train_data, self.model_val_data)
 
             else:
                 # Train and Evaluation data needs to be in a Pandas Dataframe containing at least two columns, a 'text' and a 'labels' column. The `labels` column should contain multi-hot encoded lists.
                 self.print_log_messages(4)
-                self.train_data, self.val_data, self.label_encoder = self.encode_labels(self.train_data)
-                
+                self.train_data, self.val_data, self.label_encoder = self.encode_labels(
+                    self.train_data
+                )
+
                 try:
-                    msss = MultilabelStratifiedShuffleSplit(n_splits=3,
-                                                            test_size=self.split_size,
-                                                            random_state=self.random_state)
+                    msss = MultilabelStratifiedShuffleSplit(
+                        n_splits=3,
+                        test_size=self.split_size,
+                        random_state=self.random_state,
+                    )
 
                     X = self.train_data["text"].values
                     y = np.vstack(self.train_data["labels"].values[:])
                     msss.get_n_splits(X, y)
 
                     x_train_dfs = []
                     x_test_dfs = []
 
                     for train_index, test_index in msss.split(X, y):
                         X_train, X_test = X[train_index], X[test_index]
                         y_train, y_test = y[train_index], y[test_index]
 
-                        x_train_dfs.append(pd.DataFrame({
-                            "text": X_train.tolist(),
-                            "labels": y_train.tolist()
-                        }))
-
-                        x_test_dfs.append(pd.DataFrame({
-                            "text": X_test.tolist(),
-                            "labels": y_test.tolist()
-                        }))
+                        x_train_dfs.append(
+                            pd.DataFrame(
+                                {"text": X_train.tolist(), "labels": y_train.tolist()}
+                            )
+                        )
+
+                        x_test_dfs.append(
+                            pd.DataFrame(
+                                {"text": X_test.tolist(), "labels": y_test.tolist()}
+                            )
+                        )
 
                     self.model_train_data = pd.concat(x_train_dfs, ignore_index=True)
                     self.model_val_data = pd.concat(x_test_dfs, ignore_index=True)
-                    
+
                 except:
-                    x_train, x_val, y_train, y_val = train_test_split(self.train_data["text"],
-                                                                      self.train_data["labels"],
-                                                                      test_size=self.split_size,
-                                                                      random_state=self.random_state)
-                    
-                    self.model_train_data = pd.DataFrame({
-                          "text": x_train.values,
-                          "labels": y_train.values
-                    })
-
-                    self.model_val_data = pd.DataFrame({
-                          "text": x_val.values,
-                          "labels": y_val.values
-                    })
-            
+                    x_train, x_val, y_train, y_val = train_test_split(
+                        self.train_data["text"],
+                        self.train_data["labels"],
+                        test_size=self.split_size,
+                        random_state=self.random_state,
+                    )
+
+                    self.model_train_data = pd.DataFrame(
+                        {"text": x_train.values, "labels": y_train.values}
+                    )
+
+                    self.model_val_data = pd.DataFrame(
+                        {"text": x_val.values, "labels": y_val.values}
+                    )
+
         else:
-            self.model_train_data, self.model_val_data, self.label_encoder = self.encode_labels(self.train_data, 
-                                                                                                self.val_data)
-        
-    def fit(self, 
-            train_table_name : Optional[str] = None,
-            train_data : Optional[pd.DataFrame] = None,
-            val_table_name : Optional[str] = None,
-            val_data : Optional[pd.DataFrame] = None,
-            print_model_card : Optional[bool] = True,
-            **kwargs) -> None:
+            (
+                self.model_train_data,
+                self.model_val_data,
+                self.label_encoder,
+            ) = self.encode_labels(self.train_data, self.val_data)
+
+    def fit(
+        self,
+        train_table_name: Optional[str] = None,
+        train_data: Optional[pd.DataFrame] = None,
+        val_table_name: Optional[str] = None,
+        val_data: Optional[pd.DataFrame] = None,
+        print_model_card: Optional[bool] = True,
+        **kwargs,
+    ) -> None:
         """Function to fit the model. If the model is multilabel, data must be a dataframe with two columns:
         | text    | labels                      |
          ---------  ----------------------------
         | <text>  | <label_1>, <label_2>, ...   |
 
         Parameters
         ----------
         train_table_name : str, optional
             Name of the BigQ table for training data
-        
+
         train_data : pd.DataFrame, optional
             Training dataframe object
-            
+
         val_table_name : str, optional
             Name of the BigQ table for validation data
-        
+
         val_data : pd.DataFrame, optional
             Validation dataframe object
-        
-        
+
+
         Returns
         -------
         None
 
         """
         # prepare training data
-        assert train_table_name is not None or train_data is not None, self.print_error_messages(12)
-        
+        assert (
+            train_table_name is not None or train_data is not None
+        ), self.print_error_messages(12)
+
         # training essential checks
         if train_table_name is not None:
             assert self.gcloud_project_id is not None, self.print_error_messages(17)
             assert self.gcloud_bucket_name is not None, self.print_error_messages(18)
             assert self.gcloud_blob_name is not None, self.print_error_messages(19)
-            assert self.gcloud_credentials_path is not None, self.print_error_messages(20)
+            assert self.gcloud_credentials_path is not None, self.print_error_messages(
+                20
+            )
 
             self.train_table_name = train_table_name
 
-            QUERY=f"""
+            QUERY = f"""
                    SELECT * FROM {self.train_table_name} LIMIT 1
                    """
             train_data = self.bigq_client.query(QUERY).to_dataframe()
             assert len(train_data), self.print_error_messages(4)
             assert "text" in train_data.columns.tolist(), self.print_error_messages(5)
             assert "labels" in train_data.columns.tolist(), self.print_error_messages(6)
-            
-            QUERY=f"""
+
+            QUERY = f"""
                    SELECT * FROM {self.train_table_name}
                    """
             train_data = self.bigq_client.query(QUERY).to_dataframe()
             assert train_data["text"].isnull().sum() == 0, self.print_error_messages(7)
-            assert train_data["labels"].isnull().sum() == 0, self.print_error_messages(8)
-            
+            assert train_data["labels"].isnull().sum() == 0, self.print_error_messages(
+                8
+            )
+
             # validation essential checks
             if val_table_name is not None:
                 self.val_table_name = val_table_name
-                
-                QUERY=f"""
+
+                QUERY = f"""
                        SELECT * FROM {self.val_table_name} LIMIT 1
                        """
                 val_data = self.bigq_client.query(QUERY).to_dataframe()
                 assert len(val_data), self.print_error_messages(21)
-                assert "text" in val_data.columns.tolist(), self.print_error_messages(22)
-                assert "labels" in val_data.columns.tolist(), self.print_error_messages(23)
+                assert "text" in val_data.columns.tolist(), self.print_error_messages(
+                    22
+                )
+                assert "labels" in val_data.columns.tolist(), self.print_error_messages(
+                    23
+                )
 
-                QUERY=f"""
+                QUERY = f"""
                    SELECT * FROM {self.val_table_name}
                    """
                 val_data = self.bigq_client.query(QUERY).to_dataframe()
-                assert val_data["text"].isnull().sum() == 0, self.print_error_messages(24)
-                assert val_data["labels"].isnull().sum() == 0, self.print_error_messages(25)
-        
-        
+                assert val_data["text"].isnull().sum() == 0, self.print_error_messages(
+                    24
+                )
+                assert (
+                    val_data["labels"].isnull().sum() == 0
+                ), self.print_error_messages(25)
+
         if train_data is not None:
             assert len(train_data), self.print_error_messages(4)
             assert "text" in train_data.columns.tolist(), self.print_error_messages(5)
             assert "labels" in train_data.columns.tolist(), self.print_error_messages(6)
             assert train_data["text"].isnull().sum() == 0, self.print_error_messages(7)
-            assert train_data["labels"].isnull().sum() == 0, self.print_error_messages(8)
-        
+            assert train_data["labels"].isnull().sum() == 0, self.print_error_messages(
+                8
+            )
+
         if val_data is not None:
             assert len(val_data), self.print_error_messages(21)
             assert "text" in val_data.columns.tolist(), self.print_error_messages(22)
             assert "labels" in val_data.columns.tolist(), self.print_error_messages(23)
             assert val_data["text"].isnull().sum() == 0, self.print_error_messages(24)
             assert val_data["labels"].isnull().sum() == 0, self.print_error_messages(25)
-        
+
         self.train_data = train_data
         self.val_data = val_data
         self.prepare_training_data()
         self.print_log_messages(6)
-        
+
+        # Following Andrew Ng's advice on selecting mini-batch size
+        # https://cs230.stanford.edu/files/C2M2.pdf
+        if len(self.model_train_data) <= 2000 and "train_batch_size" not in self.model_args:
+            self.model_args["train_batch_size"] = 1
+
         self.model_args["evaluate_during_training"] = self.model_val_data is not None
-        eval_df = self.model_val_data[["text", "labels"]] if self.model_val_data is not None else None
+        eval_df = (
+            self.model_val_data[["text", "labels"]]
+            if self.model_val_data is not None
+            else None
+        )
 
-        
         # build model
-        if self.classification_type == 'single':
+        if self.classification_type == "single":
             self.model_args = ClassificationArgs(**self.model_args)
 
+            # only final layer (classification layer) finetuning may prevent overfitting
+            if self.train_only_final_layer:
+                self.model_args.custom_parameter_groups = self.freeze_layers_dict
+
             self.model = ClassificationModel(
                 self.model_type,
                 self.model_version,
-                use_cuda = True if len(self.gpus_to_use) else False,
-                args=self.model_args, 
-                num_labels=len(list(self.label_encoder.classes_))
+                use_cuda=True if len(self.gpus_to_use) else False,
+                args=self.model_args,
+                num_labels=len(list(self.label_encoder.classes_)),
             )
 
             # train model
 
-            _, self.training_details = self.model.train_model(self.model_train_data[["text", "labels"]], 
-                                                                eval_df=eval_df,
-                                                                f1=f1_multiclass,
-                                                                acc=accuracy_score,
-                                                                prec=prec_multiclass,
-                                                                recall=recall_multiclass)
-        
+            _, self.training_details = self.model.train_model(
+                self.model_train_data[["text", "labels"]],
+                eval_df=eval_df,
+                f1=f1_multiclass,
+                acc=accuracy_score,
+                prec=precision_multiclass,
+                recall=recall_multiclass,
+            )
+
         else:
             self.model_args = MultiLabelClassificationArgs(**self.model_args)
 
+            # only final layer (classification layer) finetuning may prevent overfitting
+            if self.train_only_final_layer:
+                self.model_args.custom_parameter_groups = self.freeze_layers_dict
+
             self.model = MultiLabelClassificationModel(
                 self.model_type,
                 self.model_version,
-                use_cuda = True if len(self.gpus_to_use) else False,
-                args=self.model_args, 
-                num_labels=len(list(self.label_encoder.classes_))
+                use_cuda=True if len(self.gpus_to_use) else False,
+                args=self.model_args,
+                num_labels=len(list(self.label_encoder.classes_)),
+            )
+
+            _, self.training_details = self.model.train_model(
+                self.model_train_data[["text", "labels"]], eval_df=eval_df
             )
 
-            _, self.training_details = self.model.train_model(self.model_train_data[["text", "labels"]], 
-                                                                eval_df=eval_df)
-        
-        
         # save model metadata & label encoder
         self.model_metadata = {
-            "model_type": self.model_type, 
+            "model_type": self.model_type,
             "task_type": self.classification_type,
-            "do_eval": eval_df is not None
+            "do_eval": eval_df is not None,
         }
-        
+
         joblib.dump(self.label_encoder, self.label_encoder_dir)
         joblib.dump(self.model_metadata, self.model_metadata_dir)
-        
+
         # save original model
-        model_save_path = os.path.join(self.model_dir, "best_model") if self.model_metadata["do_eval"] else os.path.join(self.model_dir, "outputs")
-        kwargs["model_card_path"] = os.path.join(model_save_path, "model_card.md") if "model_card_path" not in kwargs else kwargs["model_card_path"]        
-        
+        model_save_path = (
+            os.path.join(self.model_dir, "best_model")
+            if self.model_metadata["do_eval"]
+            else os.path.join(self.model_dir, "outputs")
+        )
+        kwargs["model_card_path"] = (
+            os.path.join(model_save_path, "model_card.md")
+            if "model_card_path" not in kwargs
+            else kwargs["model_card_path"]
+        )
+
         if self.model_metadata["do_eval"]:
-            shutil.copyfile(os.path.join(self.model_dir, "outputs", 'training_progress_scores.csv'),
-                            os.path.join(self.model_dir, "best_model", 'training_progress_scores.csv'))
-        
+            shutil.copyfile(
+                os.path.join(self.model_dir, "outputs", "training_progress_scores.csv"),
+                os.path.join(
+                    self.model_dir, "best_model", "training_progress_scores.csv"
+                ),
+            )
+
         if print_model_card:
             create_model_card(**kwargs)
-            
+
             try:
-                self.upload_to_gcs(self.storage_client,
-                                   kwargs["model_card_path"],
-                                   self.gcloud_bucket_name,
-                                   os.path.join(os.path.split(self.model_bigq_dir)[0],
-                                                os.path.split(kwargs["model_card_path"])[-1]))
+                self.upload_to_gcs(
+                    self.storage_client,
+                    kwargs["model_card_path"],
+                    self.gcloud_bucket_name,
+                    os.path.join(
+                        os.path.split(self.model_bigq_dir)[0],
+                        os.path.split(kwargs["model_card_path"])[-1],
+                    ),
+                )
             except:
                 pass
 
-        make_archive(model_save_path,
-                     'gztar',
-                     root_dir=model_save_path) 
-        
-        
+        make_archive(model_save_path, "gztar", root_dir=model_save_path)
+
         if self.gcloud_bucket_name is not None:
             self.print_log_messages(7)
-                    
-            self.upload_to_gcs(self.storage_client,
-                               model_save_path + ".tar.gz",
-                               self.gcloud_bucket_name,
-                               self.model_bigq_dir)
-            
-                
+
+            self.upload_to_gcs(
+                self.storage_client,
+                model_save_path + ".tar.gz",
+                self.gcloud_bucket_name,
+                self.model_bigq_dir,
+            )
+
         # save onnx model
         if self.save_onnx_model:
             if os.path.exists(self.onnx_model_dir):
                 self.print_log_messages(8)
                 shutil.rmtree(self.onnx_model_dir)
-                
+
             copy.deepcopy(self.model).convert_to_onnx(self.onnx_model_dir)
-            
-            make_archive(self.onnx_model_dir,
-                         'gztar',
-                         root_dir=self.onnx_model_dir)
+
+            make_archive(self.onnx_model_dir, "gztar", root_dir=self.onnx_model_dir)
 
             if self.gcloud_bucket_name is not None:
-                self.upload_to_gcs(self.storage_client,
-                                   self.onnx_model_dir + ".tar.gz",
-                                   self.gcloud_bucket_name,
-                                   self.onnx_model_bigq_dir)
-                
+                self.upload_to_gcs(
+                    self.storage_client,
+                    self.onnx_model_dir + ".tar.gz",
+                    self.gcloud_bucket_name,
+                    self.onnx_model_bigq_dir,
+                )
 
         self.print_log_messages(9)
-        
-        
-            
-    def predict(self, 
-                test_table_name : Optional[str] = None,
-                test_data : Optional[pd.DataFrame] = None,
-                result_save_path : Optional[str] = None) -> str:
-        """Function to get predictions from the model. 
+
+    def predict(
+        self,
+        test_table_name: Optional[str] = None,
+        test_data: Optional[pd.DataFrame] = None,
+        result_save_path: Optional[str] = None,
+    ) -> str:
+        """Function to get predictions from the model.
         If the model is multilabel, data must be a dataframe with two columns:
         | text    | labels                      |
          ---------  ----------------------------
         | <text>  | <label_1>, <label_2>, ...   |
 
         Parameters
         ----------
         test_table_name : str
             Name of the BigQ table for test data
-        
+
         test_data : pd.DataFrame
             Test dataframe for prediction.
-        
+
         result_save_path : str
             .csv path for saving results after prediction
 
         Returns
         -------
         None
 
         """
-        assert test_data is not None or test_table_name is not None, self.print_error_messages(9)
-        
+        assert (
+            test_data is not None or test_table_name is not None
+        ), self.print_error_messages(9)
+
         if test_table_name is not None:
             assert self.gcloud_project_id is not None, self.print_error_messages(17)
             assert self.gcloud_bucket_name is not None, self.print_error_messages(18)
             assert self.gcloud_blob_name is not None, self.print_error_messages(19)
-            assert self.gcloud_credentials_path is not None, self.print_error_messages(20)
-            
+            assert self.gcloud_credentials_path is not None, self.print_error_messages(
+                20
+            )
+
             self.test_table_name = test_table_name
-            
-            QUERY=f"""
+
+            QUERY = f"""
                SELECT * FROM {self.test_table_name} LIMIT 1
                """
             test_data = self.bigq_client.query(QUERY).to_dataframe()
             assert len(test_data), self.print_error_messages(4)
             assert "text" in test_data.columns.tolist(), self.print_error_messages(5)
 
-            QUERY=f"""
+            QUERY = f"""
                    SELECT * FROM {self.test_table_name}
                    """
 
             test_data = self.bigq_client.query(QUERY).to_dataframe()
             assert test_data["text"].isnull().sum() == 0, self.print_error_messages(7)
 
             if "labels" in test_data.columns.tolist():
-                assert test_data["labels"].isnull().sum() == 0, self.print_error_messages(8)
-        
-        
+                assert (
+                    test_data["labels"].isnull().sum() == 0
+                ), self.print_error_messages(8)
+
         if test_data is not None:
             assert isinstance(test_data, pd.DataFrame), self.print_error_messages(11)
             assert len(test_data), self.print_error_messages(4)
             assert "text" in test_data.columns.tolist(), self.print_error_messages(5)
             assert test_data["text"].isnull().sum() == 0, self.print_error_messages(7)
 
             if "labels" in test_data.columns.tolist():
-                assert test_data["labels"].isnull().sum() == 0, self.print_error_messages(8)
-        
+                assert (
+                    test_data["labels"].isnull().sum() == 0
+                ), self.print_error_messages(8)
 
         # test data is valid, moving to prediction routine...
         self.print_log_messages(11)
         self.result_save_path = result_save_path
         self.do_train = False
         self.test_data = test_data
         self.test_data["text"] = self.test_data["text"].astype(str)
-        self.predictions, self.raw_outputs = self.model.predict(self.test_data["text"].tolist())
+        self.predictions, self.raw_outputs = self.model.predict(
+            self.test_data["text"].tolist()
+        )
 
         if self.model_metadata["task_type"] == "single":
             confidence_scores = softmax(self.raw_outputs, axis=1)
             self.test_data["predictions_encoded"] = self.predictions
-            self.test_data["predictions"] = self.label_encoder.inverse_transform(np.array(self.predictions))
-            self.test_data["predictions_confidence_scores"] = confidence_scores.max(axis=1)
-            
+            self.test_data["predictions"] = self.label_encoder.inverse_transform(
+                np.array(self.predictions)
+            )
+            self.test_data["predictions_confidence_scores"] = confidence_scores.max(
+                axis=1
+            )
+
             confidence_score_df = pd.DataFrame(
-                confidence_scores,
-                columns=self.label_encoder.classes_.tolist()
+                confidence_scores, columns=self.label_encoder.classes_.tolist()
             )
         else:
             predictions_raw = []
             confidence_scores = []
-            
+
             for i in range(len(self.raw_outputs)):
-                predictions_raw.append(', '.join(self.label_encoder.inverse_transform(np.array(self.predictions[i]).reshape(1,-1))[0]))
-                confidence_scores.append(self.raw_outputs[i][np.nonzero(self.predictions[i])[0]])
-            
+                predictions_raw.append(
+                    ", ".join(
+                        self.label_encoder.inverse_transform(
+                            np.array(self.predictions[i]).reshape(1, -1)
+                        )[0]
+                    )
+                )
+                confidence_scores.append(
+                    self.raw_outputs[i][np.nonzero(self.predictions[i])[0]]
+                )
+
             self.test_data["predictions_encoded"] = self.predictions
             self.test_data["predictions"] = predictions_raw
             self.test_data["predictions_confidence_scores"] = confidence_scores
-            
+
             confidence_score_df = pd.DataFrame(
-                self.raw_outputs,
-                columns=self.label_encoder.classes_.tolist()
+                self.raw_outputs, columns=self.label_encoder.classes_.tolist()
             )
-        
-        self.test_data = pd.concat([self.test_data,
-                                    confidence_score_df], axis=1)
-            
-        
+
+        self.test_data = pd.concat([self.test_data, confidence_score_df], axis=1)
+
         if "labels" in self.test_data.columns.tolist():
             self.print_log_messages(12)
-            
+
             self.test_data = self.encode_labels(val_data=self.test_data)
-            print(classification_report(self.test_data["labels"].tolist(),
-                                        self.test_data["predictions_encoded"].tolist(),
-                                        digits=3,
-                                        target_names=[str(elem) for elem in self.label_encoder.classes_.tolist()]))
-            
-            self.cls_report = classification_report(self.test_data["labels"].tolist(),
-                                                    self.test_data["predictions_encoded"].tolist(),
-                                                    target_names=[str(elem) for elem in self.label_encoder.classes_.tolist()],
-                                                    digits=3,
-                                                    output_dict=True)
+            print(
+                classification_report(
+                    self.test_data["labels"].tolist(),
+                    self.test_data["predictions_encoded"].tolist(),
+                    digits=3,
+                    target_names=[
+                        str(elem) for elem in self.label_encoder.classes_.tolist()
+                    ],
+                )
+            )
+
+            self.cls_report = classification_report(
+                self.test_data["labels"].tolist(),
+                self.test_data["predictions_encoded"].tolist(),
+                target_names=[
+                    str(elem) for elem in self.label_encoder.classes_.tolist()
+                ],
+                digits=3,
+                output_dict=True,
+            )
 
             self.cls_report = pd.DataFrame(self.cls_report).T
-            self.cls_report_path = os.path.join(self.model_dir, "best_model", "cls_report.csv") if self.model_metadata["do_eval"] else os.path.join(self.model_dir, "outputs", "cls_report.csv")
+            self.cls_report_path = (
+                os.path.join(self.model_dir, "best_model", "cls_report.csv")
+                if self.model_metadata["do_eval"]
+                else os.path.join(self.model_dir, "outputs", "cls_report.csv")
+            )
             self.cls_report.to_csv(self.cls_report_path)
-            
+
             self.print_log_messages(16)
-            
-            reindex_cols = ["text", "labels_original"] + [elem for elem in self.test_data.columns.tolist() if elem not in ["text", "labels_original"]]
+
+            reindex_cols = ["text", "labels_original"] + [
+                elem
+                for elem in self.test_data.columns.tolist()
+                if elem not in ["text", "labels_original"]
+            ]
             self.test_data = self.test_data[reindex_cols]
-        
+
         if result_save_path is not None:
             self.test_data.to_csv(result_save_path, index=False)
             self.print_log_messages(14)
-        
-        self.print_log_messages(15)
+
+        self.print_log_messages(15)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `general_text_classifier-0.1.22.dist-info/LICENSE.txt` & `general_text_classifier-0.1.23.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `general_text_classifier-0.1.22.dist-info/METADATA` & `general_text_classifier-0.1.23.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-text-classifier
-Version: 0.1.22
+Version: 0.1.23
 Summary: General Text Classification Library
 Home-page: UNKNOWN
 Author: Trendyol NLP Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,16 +13,16 @@
 Requires-Dist: wandb (>=0.13.3)
 Requires-Dist: google-cloud-bigquery (>=3.3.2)
 Requires-Dist: google-cloud-bigquery[pandas]
 Requires-Dist: google-cloud-storage (>=2.5.0)
 Requires-Dist: google-cloud-core (>=2.3.2)
 Requires-Dist: google-resumable-media (>=2.3.3)
 Requires-Dist: iterative-stratification (>=0.1.7)
-Requires-Dist: torch (>=1.7.1)
 Requires-Dist: transformers (>=4.6.1)
+Requires-Dist: torch (>=1.7.1)
 Requires-Dist: regex (>=2022.6.2)
 Requires-Dist: scikit-learn (>=0.24.2)
 Requires-Dist: streamlit (>=0.82.0)
 Requires-Dist: datasets (>=2.3.2)
 Requires-Dist: tensorboardX (>=2.2)
 Requires-Dist: tokenizers (>=0.10.3)
 Requires-Dist: seqeval (>=1.2.2)
```

## Comparing `general_text_classifier-0.1.22.dist-info/RECORD` & `general_text_classifier-0.1.23.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-general_text_classifier/__init__.py,sha256=qekxyS5tytjE8jwEIDQ7HTtTHc9kEwDrjqKltUEShO8,50950
-general_text_classifier-0.1.22.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
-general_text_classifier-0.1.22.dist-info/METADATA,sha256=15evUVsOkAkTnfdu5lqOIq_IhcS0RIreRLbQ4avloRQ,1188
-general_text_classifier-0.1.22.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-general_text_classifier-0.1.22.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
-general_text_classifier-0.1.22.dist-info/RECORD,,
+general_text_classifier/__init__.py,sha256=MDKiCW4j45a9S1OOeap7WzrHveJYh3fOifM_yE8v5pI,52704
+general_text_classifier-0.1.23.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
+general_text_classifier-0.1.23.dist-info/METADATA,sha256=RC6iZCb_5nn4-LsXKz1Y7ji-1IdlAKFOxQqn9FBmLak,1188
+general_text_classifier-0.1.23.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+general_text_classifier-0.1.23.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
+general_text_classifier-0.1.23.dist-info/RECORD,,
```

