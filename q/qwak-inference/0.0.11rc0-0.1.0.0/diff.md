# Comparing `tmp/qwak_inference-0.0.11rc0.tar.gz` & `tmp/qwak_inference-0.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.0.11rc0.tar", max compression
+gzip compressed data, was "qwak_inference-0.1.0.0.tar", max compression
```

## Comparing `qwak_inference-0.0.11rc0.tar` & `qwak_inference-0.1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10480 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/LICENSE
--rw-r--r--   0        0        0      267 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/README.md
--rw-r--r--   0        0        0     1897 2023-04-27 06:35:10.372577 qwak_inference-0.0.11rc0/pyproject.toml
--rw-r--r--   0        0        0      548 2023-04-27 06:35:10.372577 qwak_inference-0.0.11rc0/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    19154 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0      739 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      688 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     4795 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     1076 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2052 1970-01-01 00:00:00.000000 qwak_inference-0.0.11rc0/setup.py
--rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 qwak_inference-0.0.11rc0/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-05-02 08:29:04.232945 qwak_inference-0.1.0.0/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-02 08:29:04.232945 qwak_inference-0.1.0.0/README.md
+-rw-r--r--   0        0        0     1894 2023-05-02 08:29:56.885084 qwak_inference-0.1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      545 2023-05-02 08:29:56.885084 qwak_inference-0.1.0.0/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 08:29:04.232945 qwak_inference-0.1.0.0/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    19390 2023-05-02 08:29:04.232945 qwak_inference-0.1.0.0/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-05-02 08:29:04.232945 qwak_inference-0.1.0.0/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0      739 2023-05-02 08:29:04.232945 qwak_inference-0.1.0.0/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     4795 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     1076 2023-05-02 08:29:04.236945 qwak_inference-0.1.0.0/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 qwak_inference-0.1.0.0/setup.py
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 qwak_inference-0.1.0.0/PKG-INFO
```

### Comparing `qwak_inference-0.0.11rc0/LICENSE` & `qwak_inference-0.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/pyproject.toml` & `qwak_inference-0.1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.0.11.rc0"
+version = "0.1.0.0"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/__init__.py` & `qwak_inference-0.1.0.0/qwak_inference/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     # not support them due to the pandas, numpy, joblib, etc. dependencies
     pass
 
 from qwak_inference.realtime_client import RealTimeClient
 
 __all__ = ["BatchInferenceClient", "FeedbackClient", "RealTimeClient"]
 
-__version__ = "0.0.11.rc0"
+__version__ = "0.1.0.0"
```

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.1.0.0/qwak_inference/batch_client/batch_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             )
         self.model_id = model_id
         self.bucket = bucket
         self.access_key_secret = access_key_secret
         self.secret_access_key_secret = secret_access_key_secret
         self.s3_client = self.get_s3_client()
         self.batch_job_manager_client = BatchJobManagerClient()
-        self.execution_id = None
+
         logging.basicConfig(level=log_level)
 
     def get_s3_client(self):
         if self.access_key_secret:
             secret_service_client = SecretServiceClient()
             aws_access_key_id = secret_service_client.get_secret(self.access_key_secret)
             aws_secret_access_key = secret_service_client.get_secret(
@@ -170,15 +170,15 @@
         cpus: float = None,
         memory: int = None,
         gpus: int = 0,
         gpu_type: str = None,
         iam_role_arn: str = None,
         build_id: str = None,
         parameters: dict = None,
-        serialization_format="FEATHER",
+        serialization_format="PARQUET",
     ) -> pd.DataFrame:
         """Perform batch inference on given data.
 
         Args:
             df: Dataframe to perform batch inference on.
             batch_size: Inference batch size.
             job_timeout: The entire execution job timeout.
@@ -192,16 +192,14 @@
             build_id: Build ID which will be used for performing the batch request.
             parameters:
             serialization_format: The format the files are saved in (Parquet, Feather, CSV)
 
         Returns:
             Dataframe inference result.
         """
-        self.batch_size = batch_size
-        self.df = df
 
         if serialization_format.upper() not in SERIALIZATION_HANDLER_MAP:
             raise ValueError(
                 f"Invalid serialization format {serialization_format}."
                 f" Supported types are: {list(SERIALIZATION_HANDLER_MAP.keys())}"
             )
 
@@ -235,46 +233,56 @@
             gpu_amount=gpus,
         )
         execution_config = ExecutionConfig(
             execution=execution_spec,
             resources=resources_config,
             advanced_options=advanced_options_config,
         )
+
         execution_result: StartExecutionResult = (
             self.batch_job_manager_client.start_execution(execution_config)
         )
         if not execution_result.success:
             error_message = (
                 f"{Color.RED}An error occurred while starting execution: "
                 f"{execution_result.failure_message} {execution_result.execution_id}{Color.END}"
             )
             logging.error(error_message)
             raise QwakException(error_message)
-        self.execution_id = execution_result.execution_id
-        logging.info(f"{Color.GREEN}Started execution {self.execution_id}{Color.END}")
 
-        job_status = self.get_job_status(self.execution_id)
+        execution_id = execution_result.execution_id
 
-        if job_status == "Successful":
-            if self.s3_client:
-                return_df = self.__get_df_client_creds(
-                    destination_folder, serde_handler
-                )
+        try:
+            logging.info(f"{Color.GREEN}Started execution {execution_id}{Color.END}")
+
+            job_status = self.get_job_status(execution_id)
+
+            if job_status == "Successful":
+                if self.s3_client:
+                    return_df = self.__get_df_client_creds(
+                        destination_folder, execution_id, serde_handler
+                    )
+                else:
+                    return_df = self.__get_df_default_auth(execution_id, serde_handler)
+                return return_df
             else:
-                return_df = self.__get_df_default_auth(serde_handler)
-            return return_df
-        else:
-            error_message = f"{Color.RED}Execution failed!{Color.END}"
-            logging.error(error_message)
-            raise QwakException(error_message)
+                error_message = f"{Color.RED}Execution failed!{Color.END}"
+                logging.error(error_message)
+                raise QwakException(error_message)
+        except KeyboardInterrupt:
+            interrupted_msg = "Keyboard interrupted - canceling execution job"
+            logging.warning(interrupted_msg)
+            self.batch_job_manager_client.cancel_execution(execution_id)
+
+            raise QwakException(interrupted_msg)
 
     def __default_auth_execute(
         self, df: pd.DataFrame, batch_size: int, serde_handler: SerializationFormat
     ):
-        num_of_batches = math.ceil(len(self.df.index) / batch_size)
+        num_of_batches = math.ceil(len(df.index) / batch_size)
         if num_of_batches > self.MAX_PRE_SIGNED_BATCHES:
             raise QwakException(
                 f"Number of batches is larger than {self.MAX_PRE_SIGNED_BATCHES} ({num_of_batches}). "
                 f"Please decrease the number of batches. You can do this by increasing the `batch_size` parameter "
                 f"in the execution."
             )
         pre_signed_results: GetBatchJobPreSignedUploadUrlResult = (
@@ -339,31 +347,29 @@
                 destination_folder=destination_folder,
                 access_token_name=self.access_key_secret,
                 access_secret_name=self.secret_access_key_secret,
             ),
             destination_folder,
         )
 
-    def cancel(self):
+    def cancel(self, execution_id):
         """
 
         Returns:
 
         """
         status_response = self.batch_job_manager_client.cancel_execution(
-            execution_id=self.execution_id
+            execution_id=execution_id
         )
         if not status_response.success:
             logging.error(
                 f"{Color.RED}Failed to cancel job {status_response.failure_message}{Color.END}"
             )
         else:
-            logging.info(
-                f"{Color.GREEN}Execution {self.execution_id} canceled{Color.END}"
-            )
+            logging.info(f"{Color.GREEN}Execution {execution_id} canceled{Color.END}")
 
     def get_job_status(self, execution_id):
         """
 
         Args:
             execution_id:
 
@@ -438,17 +444,15 @@
                 Bucket=self.bucket,
                 Key=f"qwak/{self.model_id}/{job_id}/input/split_{i}.{serde_handler.get_file_type()}",
             )
 
         def upload_chunked_df_default_auth(i: int, df_chunk: pd.DataFrame):
             tries = 0
             while tries < self.MAX_UPLOAD_TRIES:
-                logging.info(
-                    f"Trying to upload chunk {i} to {pre_signed_urls[i]} attempt#{tries}"
-                )
+                logging.info(f"Trying to upload chunk {i}, attempt #{tries}")
                 result = requests.put(
                     pre_signed_urls[i],
                     data=serde_handler.get_bytes(df_chunk),
                     headers={"Content-Type": "application/binary"},
                     timeout=300,
                 )
                 if result.status_code == 200:
@@ -477,35 +481,39 @@
         )
         Parallel(n_jobs=-1, prefer="threads")(
             delayed(upload_func)(i, x) for i, x in enumerate(batch(df, batch_size))
         )
 
         return f"qwak/{self.model_id}/{job_id}/input"
 
-    def __get_df_client_creds(self, prefix: str, serde_handler: SerializationFormat):
+    def __get_df_client_creds(
+        self, prefix: str, execution_id: str, serde_handler: SerializationFormat
+    ):
         objects = self.s3_client.list_objects(
             Bucket=self.bucket,
-            Prefix=f"{prefix}/{self.execution_id}/results",
+            Prefix=f"{prefix}/{execution_id}/results",
         )
         dfs = []
         for object in objects["Contents"]:
             response = self.s3_client.get_object(
                 Bucket=self.bucket, Key=f"{object['Key']}"
             )
             dfs.append(
                 serde_handler.read_df(
                     BytesIO(b"".join(response.get("Body").readlines()))
                 )
             )
         return pd.concat(dfs, axis=0, ignore_index=True)
 
-    def __get_df_default_auth(self, serde_handler: SerializationFormat) -> pd.DataFrame:
+    def __get_df_default_auth(
+        self, execution_id: str, serde_handler: SerializationFormat
+    ) -> pd.DataFrame:
         pre_signed_download_urls = (
             self.batch_job_manager_client.get_pre_signed_download_urls_details(
-                self.execution_id
+                execution_id
             ).urls
         )
         dfs = []
         for url in pre_signed_download_urls:
             tries = 0
             while tries < self.MAX_DOWNLOAD_TRIES:
                 response = requests.get(url, timeout=300)
@@ -517,8 +525,9 @@
                     logging.warning(
                         f"Failed downloading results file [{response.status_code}]: {response.reason}"
                     )
             else:
                 raise QwakException(
                     f"An error occurred while downloading the data: {response.reason}"
                 )
-        return pd.concat(dfs, axis=0, ignore_index=True)
+
+        return pd.concat(dfs, axis=0).sort_index()
```

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.1.0.0/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/batch_client/s3.py` & `qwak_inference-0.1.0.0/qwak_inference/batch_client/s3.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/configuration/account.py` & `qwak_inference-0.1.0.0/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/configuration/auth.py` & `qwak_inference-0.1.0.0/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/configuration/session.py` & `qwak_inference-0.1.0.0/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/constants.py` & `qwak_inference-0.1.0.0/qwak_inference/constants.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/exceptions.py` & `qwak_inference-0.1.0.0/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/feedback_client.py` & `qwak_inference-0.1.0.0/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/realtime_client/client.py` & `qwak_inference-0.1.0.0/qwak_inference/realtime_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.1.0.0/qwak_inference/realtime_client/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.11rc0/setup.py` & `qwak_inference-0.1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'feedback:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                         'pandas<1.4'],
  'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.0.11rc0',
+    'version': '0.1.0.0',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_inference-0.0.11rc0/PKG-INFO` & `qwak_inference-0.1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.0.11rc0
+Version: 0.1.0.0
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

