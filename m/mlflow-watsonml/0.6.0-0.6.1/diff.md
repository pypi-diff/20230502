# Comparing `tmp/mlflow-watsonml-0.6.0.tar.gz` & `tmp/mlflow-watsonml-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-watsonml-0.6.0.tar", last modified: Thu Apr 27 19:58:12 2023, max compression
+gzip compressed data, was "mlflow-watsonml-0.6.1.tar", last modified: Tue May  2 19:31:19 2023, max compression
```

## Comparing `mlflow-watsonml-0.6.0.tar` & `mlflow-watsonml-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:58:12.337595 mlflow-watsonml-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-27 19:58:12.337595 mlflow-watsonml-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-27 19:58:02.000000 mlflow-watsonml-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:58:12.333595 mlflow-watsonml-0.6.0/mlflow_watsonml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:58:02.000000 mlflow-watsonml-0.6.0/mlflow_watsonml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-27 19:58:02.000000 mlflow-watsonml-0.6.0/mlflow_watsonml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-27 19:58:02.000000 mlflow-watsonml-0.6.0/mlflow_watsonml/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-27 19:58:02.000000 mlflow-watsonml-0.6.0/mlflow_watsonml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-27 19:58:02.000000 mlflow-watsonml-0.6.0/mlflow_watsonml/wml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:58:12.333595 mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-27 19:58:12.000000 mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 19:58:12.000000 mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:58:12.000000 mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 19:58:12.000000 mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 19:58:12.000000 mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 19:58:12.000000 mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:58:12.337595 mlflow-watsonml-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 19:58:02.000000 mlflow-watsonml-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/mlflow_watsonml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/wml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/setup.py
```

### Comparing `mlflow-watsonml-0.6.0/PKG-INFO` & `mlflow-watsonml-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.0
+Version: 0.6.1
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.6.0/README.md` & `mlflow-watsonml-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.0/mlflow_watsonml/config.py` & `mlflow-watsonml-0.6.1/mlflow_watsonml/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.0/mlflow_watsonml/deploy.py` & `mlflow-watsonml-0.6.1/mlflow_watsonml/deploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,21 +99,27 @@
         client = self._wml_client
 
         if endpoint is not None:
             try:
                 client = set_deployment_space(
                     client=client, deployment_space_name=endpoint
                 )
-                LOGGER.info(f"Set deployment space to {endpoint}")
             except Exception as e:
                 raise MlflowException(e)
 
             return client
 
         elif self.endpoint is not None:
+            try:
+                client = set_deployment_space(
+                    client=client, deployment_space_name=self.endpoint
+                )
+            except Exception as e:
+                raise MlflowException(e)
+
             return client
 
         else:
             raise MlflowException(
                 f"Deployment space name not set. Please set it using `endpoint` parameter"
             )
 
@@ -162,25 +168,18 @@
                 f"Deplyment {name} already exists. Use `update_deployment()` or use a different name",
                 error_code=INVALID_PARAMETER_VALUE,
             )
 
         model_object = mlflow.sklearn.load_model(model_uri=model_uri)
 
         software_spec_type = config.get("software_spec_type", DEFAULT_SOFTWARE_SPEC)
-        software_spec_uid = client.software_specifications.get_uid_by_name(
+        software_spec_uid = client.software_specifications.get_id_by_name(
             software_spec_type
         )
 
-        custom_packages: Optional[List[Dict]] = config.get("custom_packages", None)
-
-        if custom_packages is not None:
-            software_spec_uid = add_custom_packages(
-                client, software_spec_uid, custom_packages
-            )
-
         model_description = config.get("model_description", "no explanation")
         model_type = config.get("model_type", DEFAULT_MODEL_TYPE)
 
         model_details = store_model(
             client=client,
             model_object=model_object,
             software_spec_uid=software_spec_uid,
```

### Comparing `mlflow-watsonml-0.6.0/mlflow_watsonml/utils.py` & `mlflow-watsonml-0.6.1/mlflow_watsonml/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -248,7 +248,32 @@
 
 def get_endpoint(client: APIClient, endpoint: str):
     deployment_space_id = get_space_id_from_space_name(
         client=client, space_name=endpoint
     )
     endpoint_details = client.spaces.get_details(space_id=deployment_space_id)
     return endpoint_details
+
+
+def list_software_specs(client: APIClient) -> List[Dict]:
+    sw_specs = client.software_specifications.get_details()["resources"]
+    return sw_specs
+
+
+def get_software_spec(client: APIClient, sw_spec: str) -> Dict:
+    sw_specs = list_software_specs(client=client)
+
+    try:
+        return next(item for item in sw_specs if item["metadata"]["name"] == sw_spec)[
+            "metadata"
+        ]["id"]
+    except StopIteration as _:
+        raise MlflowException(
+            message=f"Software Specifiction - {sw_spec} not found",
+            error_code=ENDPOINT_NOT_FOUND,
+        )
+
+
+def software_spec_exists(client: APIClient, sw_spec: str) -> bool:
+    sw_specs = list_software_specs(client=client)
+
+    return any(item for item in sw_specs if item["metadata"]["name"] == sw_spec)
```

### Comparing `mlflow-watsonml-0.6.0/mlflow_watsonml/wml.py` & `mlflow-watsonml-0.6.1/mlflow_watsonml/wml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 from typing import Any, Dict
 
 from ibm_watson_machine_learning.client import APIClient
 from mlflow.exceptions import MlflowException
 
 from mlflow_watsonml.utils import *
 
+LOGGER = logging.getLogger(__name__)
+
 
 def store_model(
     client: APIClient,
     model_object: Any,
     software_spec_uid: str,
     name: str,
     model_description: str,
@@ -48,14 +51,16 @@
             model=model_object,
             meta_props=model_props,
             training_data=None,
             training_target=None,
             feature_names=None,
             label_column_names=None,
         )
+        LOGGER.info(model_details)
+        LOGGER.info(f"Stored model {name} in the repository.")
 
     except Exception as e:
         raise MlflowException(e)
 
     return model_details
 
 
@@ -98,14 +103,17 @@
         deployment_details = client.deployments.create(
             artifact_uid=model_id,
             meta_props=deployment_props,
         )
 
         deployment_details["name"] = deployment_details["entity"]["name"]
 
+        LOGGER.info(deployment_details)
+        LOGGER.info(f"Created {'batch' if batch else 'online'} deployment {name}")
+
     except Exception as e:
         raise MlflowException(e)
 
     return deployment_details
 
 
 def delete_deployment(client: APIClient, name: str):
@@ -119,14 +127,16 @@
         name of the deployment to delete
     """
     try:
         deployment_id = get_deployment_id_from_deployment_name(
             client=client, deployment_name=name
         )
         client.deployments.delete(deployment_uid=deployment_id)
+
+        LOGGER.info(f"Deleted deployment {name} with id {deployment_id}.")
     except Exception as e:
         raise MlflowException(e)
 
 
 def delete_model(client: APIClient, name: str):
     """Delete a model from WML repository
 
@@ -137,14 +147,16 @@
     name : str
         name of the deployment to delete
     """
     try:
         model_id = get_model_id_from_model_name(client=client, model_name=name)
         client.repository.delete(artifact_uid=model_id)
 
+        LOGGER.info(f"Deleted model {name} with id {model_id} from the repository.")
+
     except Exception as e:
         raise MlflowException(e)
 
 
 def update_model(client: APIClient):
     raise NotImplementedError()
 
@@ -153,53 +165,62 @@
     try:
         space_uid = get_space_id_from_space_name(
             client=client,
             space_name=deployment_space_name,
         )
         client.set.default_space(space_uid=space_uid)
 
+        LOGGER.info(f"Set deployment space to {deployment_space_name}")
+
     except Exception as e:
         raise MlflowException(
             f"Failed to set deployment space {deployment_space_name}", f"{e}"
         )
 
     return client
 
 
-def add_custom_packages(
-    client: APIClient, software_spec_uid: str, custom_packages: List[Dict]
-) -> str:
-    base_sw_spec_uid = software_spec_uid
+def create_custom_software_spec(
+    client: APIClient,
+    name: str,
+    base_sofware_spec: str,
+    custom_packages: List[Dict[str, str]],
+):
+    if software_spec_exists(client=client, sw_spec=name):
+        raise MlflowException(
+            f"""Software spec {name} already exists. 
+            Please delete the software spec or create one with another name."""
+        )
+
+    base_software_spec_id = client.software_specifications.get_id_by_name(
+        base_sofware_spec
+    )
 
     meta_prop_sw_spec = {
-        client.software_specifications.ConfigurationMetaNames.NAME: "custom_sw_spec",
-        client.software_specifications.ConfigurationMetaNames.DESCRIPTION: "Custom Software specification",
+        client.software_specifications.ConfigurationMetaNames.NAME: name,
         client.software_specifications.ConfigurationMetaNames.BASE_SOFTWARE_SPECIFICATION: {
-            "guid": base_sw_spec_uid
+            "guid": base_software_spec_id
         },
     }
 
     sw_spec_details = client.software_specifications.store(meta_props=meta_prop_sw_spec)
-    software_spec_uid = client.software_specifications.get_uid(sw_spec_details)
+    software_spec_id = client.software_specifications.get_uid(sw_spec_details)
 
     for custom_package in custom_packages:
         meta_prop_pkg_extn = {
-            client.package_extensions.ConfigurationMetaNames.NAME: custom_package.get(
-                "name", "some package name"
-            ),
-            client.package_extensions.ConfigurationMetaNames.DESCRIPTION: custom_package.get(
-                "description", "some package description"
-            ),
+            client.package_extensions.ConfigurationMetaNames.NAME: custom_package[
+                "name"
+            ],
             client.package_extensions.ConfigurationMetaNames.TYPE: "pip_zip",
         }
 
         pkg_extn_details = client.package_extensions.store(
-            meta_props=meta_prop_pkg_extn, file_path=custom_package.get("file")
+            meta_props=meta_prop_pkg_extn, file_path=custom_package["file"]
         )
 
-        pkg_extn_uid = client.package_extensions.get_uid(pkg_extn_details)
+        pkg_extn_id = client.package_extensions.get_id(pkg_extn_details)
 
         client.software_specifications.add_package_extension(
-            software_spec_uid, pkg_extn_uid
+            software_spec_id, pkg_extn_id
         )
 
-    return software_spec_uid
+    return software_spec_id
```

### Comparing `mlflow-watsonml-0.6.0/mlflow_watsonml.egg-info/PKG-INFO` & `mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.0
+Version: 0.6.1
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.6.0/setup.py` & `mlflow-watsonml-0.6.1/setup.py`

 * *Files identical despite different names*

