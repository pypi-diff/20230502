# Comparing `tmp/aib_logging-0.9.tar.gz` & `tmp/aib_logging-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-0.9.tar", last modified: Wed Apr 26 07:09:11 2023, max compression
+gzip compressed data, was "aib_logging-1.0.0.tar", last modified: Tue May  2 09:29:02 2023, max compression
```

## Comparing `aib_logging-0.9.tar` & `aib_logging-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.756364 aib_logging-0.9/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-0.9/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-26 07:09:11.756364 aib_logging-0.9/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-0.9/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      621 2023-04-26 07:08:30.000000 aib_logging-0.9/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-04-26 07:09:11.756364 aib_logging-0.9/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.751363 aib_logging-0.9/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.754364 aib_logging-0.9/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-0.9/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14074 2023-04-26 07:08:23.000000 aib_logging-0.9/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.756364 aib_logging-0.9/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.563649 aib_logging-1.0.0/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.0/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-02 09:29:02.563649 aib_logging-1.0.0/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.0/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      623 2023-05-02 09:28:54.000000 aib_logging-1.0.0/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-02 09:29:02.564648 aib_logging-1.0.0/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.558648 aib_logging-1.0.0/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.560648 aib_logging-1.0.0/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.0/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    13057 2023-05-02 08:42:56.000000 aib_logging-1.0.0/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.563649 aib_logging-1.0.0/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-0.9/LICENSE.txt` & `aib_logging-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-0.9/PKG-INFO` & `aib_logging-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib_logging
-Version: 0.9
+Version: 1.0.0
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aib_logging-0.9/pyproject.toml` & `aib_logging-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "0.9"
+version = "1.0.0"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aib_logging-0.9/src/aib_logging/logger.py` & `aib_logging-1.0.0/src/aib_logging/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,40 @@
         """
         import logging
         import google.cloud.logging
         self.project=project
         self.pipeline_name=pipeline_name
         client = google.cloud.logging.Client(project=project)
         self.logger = client.logger(name=logger_name)
+
+    def log(
+        self,
+        msg:str,
+        status:str='Running',
+        severity:Severities=Severities.INFO,
+    ):
+        import inspect
+        payload={
+            "pipeline_run_name":self.pipeline_name,
+            "project":self.project,
+            "component_name": inspect.stack()[1].function,
+            "Status":status,
+            "message":msg,
+        }
+        self.logger.log_struct(payload, severity=severity.value)
+
     
     def score_log(
         self,
         msg:str,
         category:Categories=Categories.MODEL,
         action:Actions=Actions.MODEL_SCORE,
         severity:Severities=Severities.INFO,
         model_name:str="AIB_Test",
+        model_version:str="default",
         data_subset:str='training',
         model_type:str='regression',
         accuracy_score:float=0.00,
         confusion_metric:dict={'TP':0,'TN':0,'FP':0,'FN':0},
         precision:float=0.00,
         recall:float=0.00,
         f1_score:float=0.00,
@@ -93,14 +111,15 @@
         example:
         from aib_logging.logger import aib_logger
         logger = aib_logger("my-gcp-project-name",pipeline_name="pipeline_job_name")
     
         logger.score_log(
             "This is test for model score",
             model_name="sklearn_model",
+            model_version="champion",
             data_subset="training",
             model_type="classification",
             accuracy_score=78.5275893,
             )
 
         Args:
             msg:str,
@@ -108,14 +127,16 @@
                 default is model,
             action: Actions perform for logs 
                 default is model_score,
             severity: Severities for logs,
                 default is INFO
             model_name(str): Name of model 
                 default is 'AIB_Test',
+            model_version(str): model version
+                default is 'default'
             data_subset(str): type of your data set/sample (training,validation,test)
                 default is training
             model_type(str): type of model (regression,classification,clustering)
                 default is regression
             model score metrics get selected on basis of model type. 
                 model_type = 'regression
                     accuracy_score:float=0.00,
@@ -160,21 +181,22 @@
             payload={
                 "pipeline_run_name":self.pipeline_name,
                 "component_name": inspect.stack()[1].function,
                 "project":self.project,
                 "category":category.value,
                 "action":action.value,
                 "model_name":model_name,
+                "model_version":model_version,
                 "data_subset":data_subset,
                 "model_type":model_type,
                 "accuracy_score":accuracy_score,
                 "confusion_metric":confusion_metric,
                 "precision":precision,
                 "recall":recall,
-                "f1-score":f1_score,
+                "f1_score":f1_score,
                 "roc_auc_score":roc_auc_score,
                 "precision_recall_auc":precision_recall_auc,
                 "log_loss":log_loss,
                 "zero_one_loss_normal":zero_one_loss_normal,
                 "zero_one_loss_fraction":zero_one_loss_fraction,
                 "balanced_accuracy_score_normal":balanced_accuracy_score_normal,
                 "balanced_accuracy_score_adjusted":balanced_accuracy_score_adjusted,
@@ -194,14 +216,15 @@
             payload={
                 "pipeline_run_name":self.pipeline_name,
                 "component_name": inspect.stack()[1].function,
                 "project":self.project,
                 "category":category.value,
                 "action":action.value,
                 "model_name":model_name,
+                "model_version":model_version,
                 "data_subset":data_subset,
                 "model_type":model_type,
                 "r2_score":r2_score,
                 "mean_absolute_error":mean_absolute_error,
                 "mean_squared_error":mean_squared_error,
                 "mean_squared_log_error":mean_squared_log_error,
                 "median_absolute_error":median_absolute_error,
@@ -218,14 +241,15 @@
             payload={
                 "pipeline_run_name":self.pipeline_name,
                 "component_name": inspect.stack()[1].function,
                 "project":self.project,
                 "category":category.value,
                 "action":action.value,
                 "model_name":model_name,
+                "model_version":model_version,
                 "data_subset":data_subset,
                 "model_type":model_type,
                 "accuracy_score":accuracy_score,
                 "confusion_metric":confusion_metric,
                 "adjusted_rand_score":adjusted_rand_score,
                 "extra_labels":extra_labels,
                 "message":msg,
@@ -304,74 +328,17 @@
             "category":category.value,
             "action":action.value,
             "min":min_val,
             "max":max_val,
             "count":count_val,
             "mean":mean_val,
             "std":std_val,
-            "25%":percentile_25,
-            "50%":percentile_50,
-            "75%":percentile_75,
-            "extra_labels":extra_labels,
-            "message":msg,
-            "object":object
-        }
-        for key, value in kwargs.items():
-                payload[key]=value
-        # Send the Log request
-        self.logger.log_struct(payload, severity=severity.value)
-    
-    def model_log(
-        self,
-        msg:str,
-        category:Categories=Categories.MODEL,
-        severity:Severities=Severities.INFO,
-        model_name:str='AIB-test-model',
-        action:str='Create',
-        version:str='default',
-        extra_labels:list=[],
-        object:dict={},
-        **kwargs
-        ):
-        """
-        Method to add model information into logs
-
-        example:
-        from aib_logging.logger import aib_logger
-        logger = aib_logger("my-gcp-project-name",pipeline_name="pipeline_job_name")
-    
-        logger.model_log(
-            "This is test for model info",
-            model_name='AIB-test-model',
-            action='update',
-            version='champion',
-            )
-
-        Args:
-            msg:str,
-            category: Categories of log type 
-                default is model,
-            action(str): Actions perform for logs 
-                default is 'create',
-            severity: Severities for logs,
-                default is INFO,
-            model_name(str): Name of model
-                default is 'AIB-test-model'
-            version(str): Model version
-                default is 'default'
-        """
-        import inspect
-        payload={
-            "pipeline_run_name":self.pipeline_name,
-            "component_name": inspect.stack()[1].function,
-            "project":self.project,
-            "category":category.value,
-            "action":action,
-            "model_name":model_name,
-            "version":version,
+            "percentile_25":percentile_25,
+            "percentile_50":percentile_50,
+            "percentile_75":percentile_75,
             "extra_labels":extra_labels,
             "message":msg,
             "object":object
         }
         for key, value in kwargs.items():
                 payload[key]=value
         # Send the Log request
```

### Comparing `aib_logging-0.9/src/aib_logging.egg-info/PKG-INFO` & `aib_logging-1.0.0/src/aib_logging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib-logging
-Version: 0.9
+Version: 1.0.0
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

