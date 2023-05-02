# Comparing `tmp/general_text_classifier-0.1.23-py3-none-any.whl.zip` & `tmp/general_text_classifier-0.1.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12489 bytes, number of entries: 6
--rw-r--r--  2.0 unx    52704 b- defN 23-May-02 08:06 general_text_classifier/__init__.py
--rw-------  2.0 unx     1062 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1188 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 23-May-02 08:08 general_text_classifier-0.1.23.dist-info/RECORD
-6 files, 55638 bytes uncompressed, 11445 bytes compressed:  79.4%
+Zip file size: 12541 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    52989 b- defN 23-May-02 09:04 general_text_classifier/__init__.py
+-rw-------  2.0 unx     1062 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1188 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-May-02 09:05 general_text_classifier-0.1.24.dist-info/RECORD
+6 files, 55923 bytes uncompressed, 11497 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: general_text_classifier/__init__.py
 Comment: 
 
-Filename: general_text_classifier-0.1.23.dist-info/LICENSE.txt
+Filename: general_text_classifier-0.1.24.dist-info/LICENSE.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.23.dist-info/METADATA
+Filename: general_text_classifier-0.1.24.dist-info/METADATA
 Comment: 
 
-Filename: general_text_classifier-0.1.23.dist-info/WHEEL
+Filename: general_text_classifier-0.1.24.dist-info/WHEEL
 Comment: 
 
-Filename: general_text_classifier-0.1.23.dist-info/top_level.txt
+Filename: general_text_classifier-0.1.24.dist-info/top_level.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.23.dist-info/RECORD
+Filename: general_text_classifier-0.1.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## general_text_classifier/__init__.py

```diff
@@ -442,15 +442,15 @@
 
             elif self.classification_type == "multi":
                 self.classification_model_obj = MultiLabelClassificationModel
                 self.classification_args_obj = MultiLabelClassificationArgs
 
             self.model_args = {
                 "use_early_stopping": False,
-                "do_lower_case": True if self.data_lang != "tr" else False,
+                "do_lower_case": self.do_lowercase if self.data_lang != "tr" else False,
                 "early_stopping_consider_epochs": False,
                 "early_stopping_delta": 0.0001,
                 "early_stopping_metric": "eval_loss",
                 "early_stopping_metric_minimize": True,
                 "early_stopping_patience": 5,
                 "eval_batch_size": 16,
                 "train_batch_size": 16,
@@ -1171,14 +1171,16 @@
             )
 
         # save model metadata & label encoder
         self.model_metadata = {
             "model_type": self.model_type,
             "task_type": self.classification_type,
             "do_eval": eval_df is not None,
+            "do_lowercase": self.do_lowercase,
+            "data_lang": self.data_lang
         }
 
         joblib.dump(self.label_encoder, self.label_encoder_dir)
         joblib.dump(self.model_metadata, self.model_metadata_dir)
 
         # save original model
         model_save_path = (
@@ -1322,14 +1324,18 @@
 
         # test data is valid, moving to prediction routine...
         self.print_log_messages(11)
         self.result_save_path = result_save_path
         self.do_train = False
         self.test_data = test_data
         self.test_data["text"] = self.test_data["text"].astype(str)
+
+        if self.model_metadata["do_lowercase"] and self.model_metadata["data_lang"] == "tr":
+            self.test_data["text"] = self.test_data["text"].apply(self.lowercase_turkish)
+
         self.predictions, self.raw_outputs = self.model.predict(
             self.test_data["text"].tolist()
         )
 
         if self.model_metadata["task_type"] == "single":
             confidence_scores = softmax(self.raw_outputs, axis=1)
             self.test_data["predictions_encoded"] = self.predictions
```

## Comparing `general_text_classifier-0.1.23.dist-info/LICENSE.txt` & `general_text_classifier-0.1.24.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `general_text_classifier-0.1.23.dist-info/METADATA` & `general_text_classifier-0.1.24.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-text-classifier
-Version: 0.1.23
+Version: 0.1.24
 Summary: General Text Classification Library
 Home-page: UNKNOWN
 Author: Trendyol NLP Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `general_text_classifier-0.1.23.dist-info/RECORD` & `general_text_classifier-0.1.24.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-general_text_classifier/__init__.py,sha256=MDKiCW4j45a9S1OOeap7WzrHveJYh3fOifM_yE8v5pI,52704
-general_text_classifier-0.1.23.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
-general_text_classifier-0.1.23.dist-info/METADATA,sha256=RC6iZCb_5nn4-LsXKz1Y7ji-1IdlAKFOxQqn9FBmLak,1188
-general_text_classifier-0.1.23.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-general_text_classifier-0.1.23.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
-general_text_classifier-0.1.23.dist-info/RECORD,,
+general_text_classifier/__init__.py,sha256=ttV2r05WWlicIYGKPYXBERC0NorWdCfjOcgRuoALSQA,52989
+general_text_classifier-0.1.24.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
+general_text_classifier-0.1.24.dist-info/METADATA,sha256=HQVl3Kc_Jg2Ff8JJC435g-k2iNqADEjvrzj0FgXFFyw,1188
+general_text_classifier-0.1.24.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+general_text_classifier-0.1.24.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
+general_text_classifier-0.1.24.dist-info/RECORD,,
```

