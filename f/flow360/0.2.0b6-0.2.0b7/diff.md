# Comparing `tmp/flow360-0.2.0b6.tar.gz` & `tmp/flow360-0.2.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b6.tar", max compression
+gzip compressed data, was "flow360-0.2.0b7.tar", max compression
```

## Comparing `flow360-0.2.0b6.tar` & `flow360-0.2.0b7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0    26526 2023-05-02 11:27:26.610545 flow360-0.2.0b6/LICENSE
--rw-r--r--   0        0        0     1493 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cli/__init__.py
--rw-r--r--   0        0        0     2526 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     3029 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1191 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     9044 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      220 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/__init__.py
--rw-r--r--   0        0        0    25949 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/constants.py
--rw-r--r--   0        0        0    26919 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0    21249 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     8093 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0      220 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     5798 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/meshing/params.py
--rw-r--r--   0        0        0     9472 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/resource_base.py
--rw-r--r--   0        0        0    10086 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2349 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/types.py
--rw-r--r--   0        0        0     1688 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/utils.py
--rw-r--r--   0        0        0     3255 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/validator.py
--rw-r--r--   0        0        0    22202 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2595 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/environment.py
--rw-r--r--   0        0        0      942 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/error_messages.py
--rw-r--r--   0        0        0      237 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5406 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-05-02 11:27:26.618546 flow360-0.2.0b6/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0      427 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1564 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/exceptions.py
--rw-r--r--   0        0        0     5841 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/solver_version.py
--rw-r--r--   0        0        0     3465 2023-05-02 11:27:26.630547 flow360-0.2.0b6/flow360/user_config.py
--rw-r--r--   0        0        0       38 2023-05-02 11:27:26.630547 flow360-0.2.0b6/flow360/version.py
--rw-r--r--   0        0        0     1465 2023-05-02 11:27:47.960682 flow360-0.2.0b6/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b6/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-05-02 13:34:05.158936 flow360-0.2.0b7/LICENSE
+-rw-r--r--   0        0        0     1493 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2526 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     3029 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1191 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     9089 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      220 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/__init__.py
+-rw-r--r--   0        0        0    26630 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/constants.py
+-rw-r--r--   0        0        0    26919 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0    21249 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     8093 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0      220 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     5798 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0     9561 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    10086 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2349 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/types.py
+-rw-r--r--   0        0        0     1688 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/utils.py
+-rw-r--r--   0        0        0     3255 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/validator.py
+-rw-r--r--   0        0        0    22242 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2595 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/environment.py
+-rw-r--r--   0        0        0      942 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/error_messages.py
+-rw-r--r--   0        0        0      237 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5406 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-05-02 13:34:05.170937 flow360-0.2.0b7/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-05-02 13:34:05.174937 flow360-0.2.0b7/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0      427 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1564 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/exceptions.py
+-rw-r--r--   0        0        0     5841 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/solver_version.py
+-rw-r--r--   0        0        0     3465 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/user_config.py
+-rw-r--r--   0        0        0       38 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/version.py
+-rw-r--r--   0        0        0     1465 2023-05-02 13:34:33.006559 flow360-0.2.0b7/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b7/PKG-INFO
```

### Comparing `flow360-0.2.0b6/LICENSE` & `flow360-0.2.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/__init__.py` & `flow360-0.2.0b7/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/cli/app.py` & `flow360-0.2.0b7/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/cloud/http_util.py` & `flow360-0.2.0b7/flow360/cloud/http_util.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/cloud/rest_api.py` & `flow360-0.2.0b7/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/cloud/s3_utils.py` & `flow360-0.2.0b7/flow360/cloud/s3_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,15 @@
         self,
         resource_id: str,
         remote_file_name: str,
         to_file: str,
         keep_folder: bool = True,
         overwrite: bool = True,
         progress_callback=None,
+        log_error=True,
     ):
         """
         Download a file from s3.
         :param resource_id:
         :param remote_file_name: file name with path in s3
         :param to_file: local file name or local folder name.
         :param keep_folder: If true, the downloaded file will be put
@@ -245,16 +246,18 @@
         if os.path.exists(to_file) and not overwrite:
             log.info(f"Skipping {remote_file_name}, file exists.")
             return
         token = self._get_s3_sts_token(resource_id, remote_file_name)
         client = token.get_client()
         try:
             meta_data = client.head_object(Bucket=token.get_bucket(), Key=token.get_s3_key())
-        except CloudFileNotFoundError as err:
-            raise CloudFileError(f"{remote_file_name} not found. id={resource_id}") from err
+        except CloudFileNotFoundError:
+            if log_error:
+                log.error(f"{remote_file_name} not found. id={resource_id}")
+            raise
 
         if progress_callback:
             progress_callback.total = meta_data.get("ContentLength", 0)
             client.download_file(
                 Bucket=token.get_bucket(),
                 Filename=to_file,
                 Key=token.get_s3_key(),
```

### Comparing `flow360-0.2.0b6/flow360/component/case.py` & `flow360-0.2.0b7/flow360/component/case.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,23 @@
     """
     CaseMeta data component
     """
 
     id: str = pd.Field(alias="caseId")
     case_mesh_id: str = pd.Field(alias="caseMeshId")
     parent_id: Union[str, None] = pd.Field(alias="parentId")
+    status: Flow360Status = pd.Field()
+
+    # pylint: disable=no-self-argument
+    @pd.validator("status")
+    def set_status_type(cls, value: Flow360Status):
+        """set_status_type when case uploaded"""
+        if value is Flow360Status.UPLOADED:
+            return Flow360Status.CASE_UPLOADED
+        return value
 
     def to_case(self) -> Case:
         """
         returns Case object from case meta info
         """
         return Case(self.id)
 
@@ -836,32 +845,43 @@
 
         for do_download, filename in download_map:
             if do_download or all:
                 self.download_file(filename, overwrite=overwrite)
 
         if bet_forces or all:
             try:
-                self.download_file(CaseDownloadable.BET_FORCES, overwrite=overwrite)
+                self.download_file(
+                    CaseDownloadable.BET_FORCES, overwrite=overwrite, log_error=False
+                )
             except CloudFileNotFoundError as err:
                 if not self._case.has_bet_disks():
                     if bet_forces:
                         log.warning("Case does not have any BET disks.")
                 else:
-                    log.error("A problem occured when trying to download bet disk forces.")
+                    log.error(
+                        f"A problem occured when trying to download bet disk forces: {CaseDownloadable.BET_FORCES}"
+                    )
                     raise err
 
         if actuator_disk_output or all:
             try:
-                self.download_file(CaseDownloadable.ACTUATOR_DISK_OUTPUT, overwrite=overwrite)
+                self.download_file(
+                    CaseDownloadable.ACTUATOR_DISK_OUTPUT, overwrite=overwrite, log_error=False
+                )
             except CloudFileNotFoundError as err:
                 if not self._case.has_actuator_disks():
                     if actuator_disk_output:
                         log.warning("Case does not have any actuator disks.")
                 else:
-                    log.error("A problem occured when trying to download actuator disk results")
+                    log.error(
+                        (
+                            "A problem occured when trying to download actuator disk results:"
+                            f"{CaseDownloadable.ACTUATOR_DISK_OUTPUT}"
+                        )
+                    )
                     raise err
 
 
 class CaseList(Flow360ResourceListBase):
     """
     Case List component
     """
```

### Comparing `flow360-0.2.0b6/flow360/component/flow360_params/flow360_params.py` & `flow360-0.2.0b7/flow360/component/flow360_params/flow360_params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/flow360_params/params_base.py` & `flow360-0.2.0b7/flow360/component/flow360_params/params_base.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/flow360_params/solvers.py` & `flow360-0.2.0b7/flow360/component/flow360_params/solvers.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/meshing/params.py` & `flow360-0.2.0b7/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/resource_base.py` & `flow360-0.2.0b7/flow360/component/resource_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Flow360Status component
     """
 
     COMPLETED = "completed"
     ERROR = "error"
     DIVERGED = "diverged"
     UPLOADED = "uploaded"
+    CASE_UPLOADED = "case_uploaded"
     UPLOADING = "uploading"
     RUNNING = "running"
     PREPROCESSING = "preprocessing"
     GENERATING = "generating"
     PROCESSED = "processed"
     STOPPED = "stopped"
     DELETED = "deleted"
@@ -62,15 +63,15 @@
     Flow360 base Model
     """
 
     name: str = pd.Field()
     user_id: str = pd.Field(alias="userId")
     id: str = pd.Field()
     solver_version: Union[str, None] = pd.Field(alias="solverVersion")
-    status: Flow360Status
+    status: Flow360Status = pd.Field()
     tags: Optional[List[str]]
     created_at: Optional[str] = pd.Field(alias="createdAt")
     updated_at: Optional[datetime] = pd.Field(alias="updatedAt")
     updated_by: Optional[str] = pd.Field(alias="updatedBy")
     deleted: bool
 
     # pylint: disable=no-self-argument
@@ -272,25 +273,27 @@
     def download_file(
         self,
         file_name,
         to_file=".",
         keep_folder: bool = True,
         overwrite: bool = True,
         progress_callback=None,
+        **kwargs,
     ):
         """
         general download functionality
         """
         return self.s3_transfer_method.download_file(
             self.id,
             file_name,
             to_file,
             keep_folder,
             overwrite=overwrite,
             progress_callback=progress_callback,
+            **kwargs,
         )
 
     @on_cloud_resource_only
     def upload_file(self, remote_file_name: str, file_name: str, progress_callback=None):
         """
         general upload functionality
         """
```

### Comparing `flow360-0.2.0b6/flow360/component/surface_mesh.py` & `flow360-0.2.0b7/flow360/component/surface_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/types.py` & `flow360-0.2.0b7/flow360/component/types.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/utils.py` & `flow360-0.2.0b7/flow360/component/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/validator.py` & `flow360-0.2.0b7/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/component/volume_mesh.py` & `flow360-0.2.0b7/flow360/component/volume_mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,14 +545,15 @@
     def download_file(
         self,
         file_name: Union[str, VolumeMeshDownloadable],
         to_file=".",
         keep_folder: bool = True,
         overwrite: bool = True,
         progress_callback=None,
+        **kwargs,
     ):
         """
         Download file from surface mesh
         :param file_name:
         :param to_file:
         :param keep_folder:
         :return:
@@ -561,14 +562,15 @@
             file_name = file_name.value
         return super().download_file(
             file_name,
             to_file,
             keep_folder=keep_folder,
             overwrite=overwrite,
             progress_callback=progress_callback,
+            **kwargs,
         )
 
     def download(self, to_file=".", keep_folder: bool = True, overwrite: bool = True):
         """
         Download volume mesh file
         :param to_file:
         :param keep_folder:
```

### Comparing `flow360-0.2.0b6/flow360/environment.py` & `flow360-0.2.0b7/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/error_messages.py` & `flow360-0.2.0b7/flow360/error_messages.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b7/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b7/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b7/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b7/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/base_test_case.py` & `flow360-0.2.0b7/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b7/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b7/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b7/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b7/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b7/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b7/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b7/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b7/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/exceptions.py` & `flow360-0.2.0b7/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/log.py` & `flow360-0.2.0b7/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/solver_version.py` & `flow360-0.2.0b7/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/flow360/user_config.py` & `flow360-0.2.0b7/flow360/user_config.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b6/pyproject.toml` & `flow360-0.2.0b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b6"
+version = "v0.2.0b7"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
```

### Comparing `flow360-0.2.0b6/PKG-INFO` & `flow360-0.2.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b6
+Version: 0.2.0b7
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

