# Comparing `tmp/flow360-0.2.0b5.tar.gz` & `tmp/flow360-0.2.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b5.tar", max compression
+gzip compressed data, was "flow360-0.2.0b6.tar", max compression
```

## Comparing `flow360-0.2.0b5.tar` & `flow360-0.2.0b6.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0    26526 2023-04-25 14:33:37.416890 flow360-0.2.0b5/LICENSE
--rw-r--r--   0        0        0     1493 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cli/__init__.py
--rw-r--r--   0        0        0     2526 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     3029 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1466 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     8847 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      220 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/__init__.py
--rw-r--r--   0        0        0    24217 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/constants.py
--rw-r--r--   0        0        0    26899 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0    21248 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     8093 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0      220 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     5798 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/meshing/params.py
--rw-r--r--   0        0        0     8584 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/resource_base.py
--rw-r--r--   0        0        0    10172 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2349 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/types.py
--rw-r--r--   0        0        0     1019 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/utils.py
--rw-r--r--   0        0        0     3255 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/validator.py
--rw-r--r--   0        0        0    21646 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2595 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/environment.py
--rw-r--r--   0        0        0      237 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5406 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-04-25 14:33:37.424890 flow360-0.2.0b5/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-04-25 14:33:37.428890 flow360-0.2.0b5/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0      427 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1354 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/exceptions.py
--rw-r--r--   0        0        0     5809 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/solver_version.py
--rw-r--r--   0        0        0     2908 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/user_config.py
--rw-r--r--   0        0        0       38 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/version.py
--rw-r--r--   0        0        0     1465 2023-04-25 14:33:54.097131 flow360-0.2.0b5/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b5/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-05-02 11:27:26.610545 flow360-0.2.0b6/LICENSE
+-rw-r--r--   0        0        0     1493 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2526 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     3029 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1191 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     9044 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      220 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/__init__.py
+-rw-r--r--   0        0        0    25949 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/constants.py
+-rw-r--r--   0        0        0    26919 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0    21249 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     8093 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0      220 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     5798 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0     9472 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    10086 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2349 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/types.py
+-rw-r--r--   0        0        0     1688 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/utils.py
+-rw-r--r--   0        0        0     3255 2023-05-02 11:27:26.610545 flow360-0.2.0b6/flow360/component/validator.py
+-rw-r--r--   0        0        0    22202 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2595 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/environment.py
+-rw-r--r--   0        0        0      942 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/error_messages.py
+-rw-r--r--   0        0        0      237 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5406 2023-05-02 11:27:26.614546 flow360-0.2.0b6/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-05-02 11:27:26.618546 flow360-0.2.0b6/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0      427 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1564 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/exceptions.py
+-rw-r--r--   0        0        0     5841 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-05-02 11:27:26.626546 flow360-0.2.0b6/flow360/solver_version.py
+-rw-r--r--   0        0        0     3465 2023-05-02 11:27:26.630547 flow360-0.2.0b6/flow360/user_config.py
+-rw-r--r--   0        0        0       38 2023-05-02 11:27:26.630547 flow360-0.2.0b6/flow360/version.py
+-rw-r--r--   0        0        0     1465 2023-05-02 11:27:47.960682 flow360-0.2.0b6/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b6/PKG-INFO
```

### Comparing `flow360-0.2.0b5/LICENSE` & `flow360-0.2.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/__init__.py` & `flow360-0.2.0b6/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/cli/app.py` & `flow360-0.2.0b6/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/cloud/http_util.py` & `flow360-0.2.0b6/flow360/cloud/http_util.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/cloud/rest_api.py` & `flow360-0.2.0b6/flow360/cloud/rest_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,24 +20,14 @@
         url = f"{self._endpoint}"
         if self._id is not None:
             url += f"/{self._id}"
         if method is not None:
             url += f"/{method}"
         return url
 
-    # pylint: disable=redefined-builtin
-    def init_id(self, id):
-        """
-        Init id, run only once
-        """
-        if self._id is None:
-            self._id = id
-        else:
-            raise RuntimeError('"id" already set, change of "id" is not allowed.')
-
     def get(self, path=None, method=None, json=None, params=None):
         """
         Resource get
         """
         return http.get(path or self._url(method), json=json, params=params)
 
     def post(self, json, path=None, method=None):
```

### Comparing `flow360-0.2.0b5/flow360/cloud/s3_utils.py` & `flow360-0.2.0b6/flow360/cloud/s3_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Progress,
     TextColumn,
     TimeRemainingColumn,
     TransferSpeedColumn,
 )
 
 from ..environment import Env
+from ..exceptions import CloudFileError
 from ..log import log
 from .http_util import http
 
 
 class ProgressCallbackInterface(ABC):
     """
     Progress callback abstract class
@@ -242,15 +243,19 @@
         """
         to_file = create_base_folder(resource_id, remote_file_name, to_file, keep_folder)
         if os.path.exists(to_file) and not overwrite:
             log.info(f"Skipping {remote_file_name}, file exists.")
             return
         token = self._get_s3_sts_token(resource_id, remote_file_name)
         client = token.get_client()
-        meta_data = client.head_object(Bucket=token.get_bucket(), Key=token.get_s3_key())
+        try:
+            meta_data = client.head_object(Bucket=token.get_bucket(), Key=token.get_s3_key())
+        except CloudFileNotFoundError as err:
+            raise CloudFileError(f"{remote_file_name} not found. id={resource_id}") from err
+
         if progress_callback:
             progress_callback.total = meta_data.get("ContentLength", 0)
             client.download_file(
                 Bucket=token.get_bucket(),
                 Filename=to_file,
                 Key=token.get_s3_key(),
                 Callback=progress_callback,
```

### Comparing `flow360-0.2.0b5/flow360/component/case.py` & `flow360-0.2.0b6/flow360/component/case.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """
 Case component
 """
 from __future__ import annotations
 
 import json
 from enum import Enum
-from typing import Iterator, List
+from typing import Iterator, List, Union
 
 import pydantic as pd
 from pylab import show, subplots
 
+from .. import error_messages
 from ..cloud.rest_api import RestApi
 from ..cloud.s3_utils import CloudFileNotFoundError, S3TransferType
+from ..exceptions import RuntimeError as FlRuntimeError
 from ..exceptions import ValidationError
+from ..exceptions import ValueError as FlValueError
 from ..log import log
 from .flow360_params.flow360_params import Flow360Params, UnvalidatedFlow360Params
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     Flow360Status,
     ResourceDraft,
     before_submit_only,
     is_object_cloud_resource,
 )
-from .utils import is_valid_uuid
+from .utils import is_valid_uuid, validate_type
 from .validator import Validator
 
 
 class CaseBase:
     """
     Case Base component
     """
@@ -108,15 +111,15 @@
 class CaseMeta(Flow360ResourceBaseModel):
     """
     CaseMeta data component
     """
 
     id: str = pd.Field(alias="caseId")
     case_mesh_id: str = pd.Field(alias="caseMeshId")
-    parent_id: str = pd.Field(alias="parentId")
+    parent_id: Union[str, None] = pd.Field(alias="parentId")
 
     def to_case(self) -> Case:
         """
         returns Case object from case meta info
         """
         return Case(self.id)
 
@@ -130,15 +133,15 @@
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         name: str,
         params: Flow360Params,
         volume_mesh_id: str = None,
         tags: List[str] = None,
-        parent_id=None,
+        parent_id: str = None,
         other_case: Case = None,
         parent_case: Case = None,
         solver_version: str = None,
     ):
         self.name = name
         self.params = params
         self.volume_mesh_id = volume_mesh_id
@@ -165,15 +168,15 @@
 
     @params.setter
     def params(self, value: Flow360Params):
         """
         sets case params (before submit only)
         """
         if not isinstance(value, Flow360Params) and not isinstance(value, UnvalidatedFlow360Params):
-            raise ValueError("params are not of type Flow360Params.")
+            raise FlValueError("params are not of type Flow360Params.")
         self._params = value
 
     @property
     def name(self) -> str:
         """
         returns case name
         """
@@ -196,14 +199,33 @@
     @volume_mesh_id.setter
     def volume_mesh_id(self, value):
         """
         sets volume mesh id
         """
         self._volume_mesh_id = value
 
+    def to_case(self) -> Case:
+        """Return Case from CaseDraft (must be after .submit())
+
+        Returns
+        -------
+        Case
+            Case representation
+
+        Raises
+        ------
+        RuntimeError
+            Raises error when case is before submission, i.e., is in draft state
+        """
+        if not self.is_cloud_resource():
+            raise FlRuntimeError(
+                f"Case name={self.name} is in draft state. Run .submit() before calling this function."
+            )
+        return Case(self.id)
+
     @before_submit_only
     def submit(self, force_submit: bool = False) -> Case:
         """
         submits case to cloud for running
         """
         assert self.name
         assert self.volume_mesh_id or self.other_case or self.parent_id or self.parent_case
@@ -213,23 +235,36 @@
 
         volume_mesh_id = self.volume_mesh_id
         parent_id = self.parent_id
         if parent_id is not None:
             self.parent_case = Case(self.parent_id)
 
         if isinstance(self.parent_case, CaseDraft):
-            self.parent_case = Case(self.parent_case.id)
+            self.parent_case = self.parent_case.to_case()
 
         if isinstance(self.other_case, CaseDraft):
-            self.other_case = Case(self.other_case.id)
+            self.other_case = self.other_case.to_case()
+
+        if self.other_case is not None and self.other_case.has_parent():
+            self.parent_case = self.other_case.parent
 
         if self.parent_case is not None:
             parent_id = self.parent_case.id
             volume_mesh_id = self.parent_case.volume_mesh_id
 
+            if (
+                self.solver_version is not None
+                and self.parent_case.solver_version != self.solver_version
+            ):
+                raise FlRuntimeError(
+                    error_messages.change_solver_version_error(
+                        self.parent_case.solver_version, self.solver_version
+                    )
+                )
+
         volume_mesh_id = volume_mesh_id or self.other_case.volume_mesh_id
 
         is_valid_uuid(volume_mesh_id)
         is_valid_uuid(parent_id, ignore_none=True)
         self.validator_api(
             self.params,
             volume_mesh_id=volume_mesh_id,
@@ -241,40 +276,41 @@
             "name": self.name,
             "meshId": volume_mesh_id,
             "runtimeParams": self.params.to_flow360_json(),
             "tags": self.tags,
             "parentId": parent_id,
         }
 
-        if self.solver_version:
+        if self.solver_version is not None:
             data["solverVersion"] = self.solver_version
 
         resp = RestApi(self._endpoint).post(
             json=data,
             path=f"volumemeshes/{volume_mesh_id}/case",
         )
         info = CaseMeta(**resp)
         self._id = info.id
 
         self._submitted_case = Case(self.id)
+        log.info(f"Case successfully submitted: {self._submitted_case.short_description()}")
         return self._submitted_case
 
     def validate_case_inputs(self, pre_submit_checks=False):
         """
         validates case inputs (before submit only)
         """
         if self.volume_mesh_id is not None and self.other_case is not None:
-            raise ValueError("You cannot specify both volume_mesh_id AND other_case.")
+            raise FlValueError("You cannot specify both volume_mesh_id AND other_case.")
 
         if self.parent_id is not None and self.parent_case is not None:
-            raise ValueError("You cannot specify both parent_id AND parent_case.")
+            raise FlValueError("You cannot specify both parent_id AND parent_case.")
 
         if self.parent_id is not None or self.parent_case is not None:
             if self.volume_mesh_id is not None or self.other_case is not None:
-                raise ValueError(
+                raise FlValueError(
                     "You cannot specify volume_mesh_id OR other_case when parent case provided."
                 )
 
         is_valid_uuid(self.volume_mesh_id, ignore_none=True)
 
         if pre_submit_checks:
             is_object_cloud_resource(self.other_case)
@@ -301,38 +337,34 @@
 
 # pylint: disable=too-many-instance-attributes
 class Case(CaseBase, Flow360Resource):
     """
     Case component
     """
 
-    def __init__(self, case_id: str = None, meta_info: CaseMeta = None):
-        if (case_id is None and meta_info is None) or (
-            case_id is not None and meta_info is not None
-        ):
-            raise ValueError("You must provide case_id OR meta_info to constructor.")
-
-        if meta_info is not None:
-            case_id = meta_info.id
-
-        assert case_id is not None
-
+    # pylint: disable=redefined-builtin
+    def __init__(self, id: str):
         super().__init__(
             resource_type="Case",
             info_type_class=CaseMeta,
             s3_transfer_method=S3TransferType.CASE,
             endpoint=self._endpoint,
-            id=case_id,
+            id=id,
         )
 
-        if meta_info is not None:
-            self._info = meta_info
         self._params = None
         self._results = CaseResults(self)
 
+    @classmethod
+    def _from_meta(cls, meta: CaseMeta):
+        validate_type(meta, "meta", CaseMeta)
+        case = cls(id=meta.id)
+        case._set_meta(meta)
+        return case
+
     @property
     def params(self) -> Flow360Params:
         """
         returns case params
         """
         if self._params is None:
             raw_params = json.loads(self.get(method="runtimeParams")["content"])
@@ -343,20 +375,42 @@
                     log.error(f"{err}")
                     self._params = raw_params
                 else:
                     raise ValidationError(f"{err}") from err
 
         return self._params
 
-    @property
-    def name(self) -> str:
-        """
-        returns case name
+    def has_parent(self) -> bool:
+        """Check if case has parent case
+
+        Returns
+        -------
+        bool
+            True when case has parent, False otherwise
         """
-        return self.info.name
+        print(f"has_parent {self.info.parent_id} (type={type(self.info.parent_id)})")
+        return self.info.parent_id is not None
+
+    @property
+    def parent(self) -> Case:
+        """parent case
+
+        Returns
+        -------
+        Case
+            parent case object
+
+        Raises
+        ------
+        RuntimeError
+            When case does not have parent
+        """
+        if self.has_parent():
+            return Case(self.info.parent_id)
+        raise FlRuntimeError("Case does not have parent case.")
 
     @property
     def info(self) -> CaseMeta:
         """
         returns metadata info for case
         """
         return super().info
@@ -442,15 +496,15 @@
     @classmethod
     def create(
         cls,
         name: str,
         params: Flow360Params,
         volume_mesh_id: str = None,
         tags: List[str] = None,
-        parent_id=None,
+        parent_id: str = None,
         other_case: Case = None,
         parent_case: Case = None,
         solver_version: str = None,
     ) -> CaseDraft:
         """
         Create new case
         :param name:
@@ -466,15 +520,15 @@
         assert name
         assert volume_mesh_id or other_case or parent_id or parent_case
         assert params
 
         if not isinstance(params, Flow360Params) and not isinstance(
             params, UnvalidatedFlow360Params
         ):
-            raise ValueError("params are not of type Flow360Params.")
+            raise FlValueError("params are not of type Flow360Params.")
 
         new_case = CaseDraft(
             name=name,
             volume_mesh_id=volume_mesh_id,
             params=params.copy(),
             parent_id=parent_id,
             other_case=other_case,
```

### Comparing `flow360-0.2.0b5/flow360/component/flow360_params/flow360_params.py` & `flow360-0.2.0b6/flow360/component/flow360_params/flow360_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,16 +422,16 @@
 
 class TimeSteppingCFL(Flow360BaseModel):
     """
     CFL for time stepping component
     """
 
     type: Optional[Literal["ramp", "adaptive"]] = pd.Field()
-    initial: Optional[int] = pd.Field()
-    final: Optional[int] = pd.Field()
+    initial: Optional[PositiveFloat] = pd.Field()
+    final: Optional[PositiveFloat] = pd.Field()
     ramp_steps: Optional[int] = pd.Field(alias="rampSteps")
     min: Optional[PositiveFloat] = pd.Field()
     max: Optional[PositiveFloat] = pd.Field()
     max_relative_change: Optional[PositiveFloat] = pd.Field(alias="maxRelativeChange")
     convergence_limiting_factor: Optional[PositiveFloat] = pd.Field(
         alias="convergenceLimitingFactor"
     )
```

### Comparing `flow360-0.2.0b5/flow360/component/flow360_params/params_base.py` & `flow360-0.2.0b6/flow360/component/flow360_params/params_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,15 +572,15 @@
             class_validators=None,
             config=cls.__config__,
         )
         cls.__fields__[TYPE_TAG_STR] = tag_field
 
     @classmethod
     def generate_docstring(cls) -> str:
-        """Generates a docstring for a Flow360 mode and saves it to the __doc__ of the class."""
+        """Generates a docstring for a Flow360 model and saves it to the __doc__ of the class."""
 
         # store the docstring in here
         doc = ""
 
         # if the model already has a docstring, get the first lines and save the rest
         original_docstrings = []
         if cls.__doc__:
```

### Comparing `flow360-0.2.0b5/flow360/component/flow360_params/solvers.py` & `flow360-0.2.0b6/flow360/component/flow360_params/solvers.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/component/meshing/params.py` & `flow360-0.2.0b6/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/component/resource_base.py` & `flow360-0.2.0b6/flow360/component/resource_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 import traceback
 from abc import ABC
 from datetime import datetime
 from enum import Enum
 from functools import wraps
 from typing import List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+import pydantic as pd
 
+from .. import error_messages
 from ..cloud.rest_api import RestApi
+from ..exceptions import RuntimeError as FlRuntimeError
 from ..log import log
 from ..user_config import UserConfig
+from .utils import is_valid_uuid, validate_type
 
 
 class Flow360Status(Enum):
     """
     Flow360Status component
     """
 
@@ -50,45 +53,53 @@
             Flow360Status.PROCESSED,
             Flow360Status.DELETED,
         ]:
             return True
         return False
 
 
-class Flow360ResourceBaseModel(BaseModel):
+class Flow360ResourceBaseModel(pd.BaseModel):
     """
     Flow360 base Model
     """
 
-    name: str = Field()
-    user_id: str = Field(alias="userId")
-    id: str = Field()
-    solver_version: Union[str, None] = Field(alias="solverVersion")
+    name: str = pd.Field()
+    user_id: str = pd.Field(alias="userId")
+    id: str = pd.Field()
+    solver_version: Union[str, None] = pd.Field(alias="solverVersion")
     status: Flow360Status
     tags: Optional[List[str]]
-    created_at: Optional[str] = Field(alias="createdAt")
-    updated_at: Optional[datetime] = Field(alias="updatedAt")
-    updated_by: Optional[str] = Field(alias="updatedBy")
+    created_at: Optional[str] = pd.Field(alias="createdAt")
+    updated_at: Optional[datetime] = pd.Field(alias="updatedAt")
+    updated_by: Optional[str] = pd.Field(alias="updatedBy")
     deleted: bool
 
+    # pylint: disable=no-self-argument
+    @pd.validator("*", pre=True)
+    def handle_none_str(cls, value):
+        """handle None strings"""
+        if value == "None":
+            value = None
+        return value
+
     # pylint: disable=missing-class-docstring,too-few-public-methods
     class Config:
-        extra = Extra.allow
+        extra = pd.Extra.allow
         allow_mutation = False
 
 
 def on_cloud_resource_only(func):
     """
     Wrapper for cloud functions only
     """
 
     @wraps(func)
     def wrapper(obj, *args, **kwargs):
         if not obj.is_cloud_resource():
-            raise RuntimeError(
+            raise FlRuntimeError(
                 'Resource does not have "id", it is not a cloud resource. Provide "id" before calling this function.'
             )
         return func(obj, *args, **kwargs)
 
     return wrapper
 
 
@@ -96,15 +107,15 @@
     """
     Wrapper for before submit functions only
     """
 
     @wraps(func)
     def wrapper(obj, *args, **kwargs):
         if obj.is_cloud_resource():
-            raise RuntimeError(
+            raise FlRuntimeError(
                 'Resource already have "id", cannot call this method. To modify and re-submit create a copy.'
             )
         return func(obj, *args, **kwargs)
 
     return wrapper
 
 
@@ -117,24 +128,16 @@
     traceback = None
 
     def __init__(self):
         # remove from traceback:
         # 1. This line (self.traceback)
         # 2. Call of this init
         self.traceback = traceback.format_stack()[:-2]
-
-        if not UserConfig.suppress_submit_warning():
-            log.warning(
-                f"""\
-Remeber to submit your {self.__class__.__name__} to cloud to have it processed.
-Please run .submit() after .create()
-To suppress this message run: flow360 configure --suppress-submit-warning"""
-            )
-            for line in self.traceback:
-                print(line.strip())
+        if not UserConfig.is_suppress_submit_warning():
+            log.warning(error_messages.submit_reminder(self.__class__.__name__))
 
     @property
     def id(self):
         """
         returns id of resource
         """
         return self._id
@@ -149,58 +152,74 @@
         """
         if self.id is None:
             return False
         return True
 
     def __del__(self):
         if self.is_cloud_resource() is False and self.traceback is not None:
-            print(
-                f"\
-WARNING: You have not submitted your {self.__class__.__name__} to cloud. \
-It will not be process. Please run .submit() after .create()"
-            )
+            print(error_messages.submit_warning(self.__class__.__name__))
             for line in self.traceback:
                 print(line.strip())
 
 
 class Flow360Resource(RestApi):
     """
     Flow360 base resource model
     """
 
-    def __init__(self, resource_type, info_type_class, *args, s3_transfer_method=None, **kwargs):
+    # pylint: disable=redefined-builtin
+    def __init__(
+        self, resource_type, info_type_class, *args, s3_transfer_method=None, id=None, **kwargs
+    ):
+        is_valid_uuid(id, ignore_none=False)
         self._resource_type = resource_type
         self.s3_transfer_method = s3_transfer_method
         self.info_type_class = info_type_class
         self._info = None
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, id=id, **kwargs)
 
     def __str__(self):
         return self.info.__str__()
 
     def __repr__(self):
         return self.info.__repr__()
 
     def is_cloud_resource(self):
         """
         returns true if is cloud resource
         """
         return self.id is not None
 
+    def _set_meta(self, meta: Flow360ResourceBaseModel):
+        """
+        set metadata info for resource
+        """
+        if self._info is None:
+            validate_type(meta, "meta", self.info_type_class)
+            self._info = meta
+        else:
+            raise FlRuntimeError(f"Resource already have metadata {self._info}. Cannot assign.")
+
+    @classmethod
+    def _from_meta(cls, meta):
+        raise NotImplementedError(
+            "This is abstract method. Needs to be implemented by specialised class."
+        )
+
     @on_cloud_resource_only
-    def get_info(self, force=False):
+    def get_info(self, force=False) -> Flow360ResourceBaseModel:
         """
         returns metadata info for resource
         """
         if self._info is None or force:
             self._info = self.info_type_class(**self.get())
         return self._info
 
     @property
-    def info(self):
+    def info(self) -> Flow360ResourceBaseModel:
         """
         returns metadata info for resource
         """
         return self.get_info()
 
     @property
     @on_cloud_resource_only
@@ -222,14 +241,28 @@
     @on_cloud_resource_only
     def name(self):
         """
         returns name of resource
         """
         return self.info.name
 
+    def short_description(self) -> str:
+        """short_description
+
+        Returns
+        -------
+        str
+            generates short description of resource (name, id, status)
+        """
+        return f"""
+        name   = {self.name}
+        id     = {self.id}
+        status = {self.status.value}
+        """
+
     @property
     @on_cloud_resource_only
     def solver_version(self):
         """
         returns solver version of resource
         """
         return self.info.solver_version
@@ -266,19 +299,17 @@
         )
 
 
 def is_object_cloud_resource(resource: Flow360Resource):
     """
     checks if object is cloud resource, raises RuntimeError
     """
-    msg = "Reference resource is not a cloud resource. "
-    msg += "If a case was retried or forked from other case, submit the other case first before submitting this case."
     if resource is not None:
         if not resource.is_cloud_resource():
-            raise RuntimeError(msg)
+            raise FlRuntimeError(error_messages.not_a_cloud_resource)
         return True
     return False
 
 
 class Flow360ResourceListBase(list, RestApi):
     """
     Flow360 ResourceList base component
@@ -311,15 +342,15 @@
 
             if limit is None:
                 limit = -1
 
             list.__init__(
                 self,
                 [
-                    resourceClass(meta_info=resourceClass._meta_class().parse_obj(item))
+                    resourceClass._from_meta(meta=resourceClass._meta_class().parse_obj(item))
                     for item in resp[:limit]
                 ],
             )
 
     @classmethod
     def from_cloud(cls):
         """
```

### Comparing `flow360-0.2.0b5/flow360/component/surface_mesh.py` & `flow360-0.2.0b6/flow360/component/surface_mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 
 import pydantic as pd
 
 from ..cloud.rest_api import RestApi
 from ..cloud.s3_utils import S3TransferType
 from ..exceptions import FileError as FlFileError
 from ..exceptions import ValueError as FlValueError
+from ..log import log
 from .flow360_params.params_base import params_generic_validator
 from .meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     ResourceDraft,
 )
+from .utils import validate_type
 from .validator import Validator
 from .volume_mesh import VolumeMeshDraft
 
 
 class SurfaceMeshDownloadable(Enum):
     """
     Surface Mesh downloadable files
@@ -143,15 +145,15 @@
 
         _, ext = os.path.splitext(self.geometry_file)
         remote_file_name = f"geometry{ext}"
         submitted_mesh.upload_file(
             remote_file_name, self.geometry_file, progress_callback=progress_callback
         )
         submitted_mesh._complete_upload(remote_file_name)
-
+        log.info(f"SurfaceMesh successfully submitted: {submitted_mesh.short_description()}")
         return submitted_mesh
 
     @classmethod
     def validator_api(cls, params: SurfaceMeshingParams, solver_version=None):
         """
         validation api: validates surface meshing parameters before submitting
         """
@@ -159,38 +161,32 @@
 
 
 class SurfaceMesh(SurfaceMeshBase, Flow360Resource):
     """
     Surface mesh component
     """
 
-    def __init__(self, surface_mesh_id: str = None, meta_info: SurfaceMeshMeta = None):
-        if (surface_mesh_id is None and meta_info is None) or (
-            surface_mesh_id is not None and meta_info is not None
-        ):
-            raise ValueError("You must provide surface_mesh_id OR meta_info to constructor.")
-
-        if meta_info is not None:
-            surface_mesh_id = meta_info.id
-
-        assert surface_mesh_id is not None
-
+    # pylint: disable=redefined-builtin
+    def __init__(self, id: str):
         super().__init__(
             resource_type="Surface Mesh",
             info_type_class=SurfaceMeshMeta,
             s3_transfer_method=S3TransferType.SURFACE_MESH,
             endpoint=self._endpoint,
-            id=surface_mesh_id,
+            id=id,
         )
-
-        if meta_info is not None:
-            self._info = meta_info
-
         self._params = None
 
+    @classmethod
+    def _from_meta(cls, meta: SurfaceMeshMeta):
+        validate_type(meta, "meta", SurfaceMeshMeta)
+        surface_mesh = cls(id=meta.id)
+        surface_mesh._set_meta(meta)
+        return surface_mesh
+
     @property
     def info(self) -> SurfaceMeshMeta:
         return super().info
 
     @property
     def params(self) -> SurfaceMeshingParams:
         """
```

### Comparing `flow360-0.2.0b5/flow360/component/types.py` & `flow360-0.2.0b6/flow360/component/types.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/component/utils.py` & `flow360-0.2.0b6/flow360/component/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Utility functions
 """
 import uuid
 from functools import wraps
 
+from ..exceptions import TypeError as FlTypeError
+from ..exceptions import ValueError as FlValueError
 from ..log import log
 
 
 # pylint: disable=redefined-builtin
 def is_valid_uuid(id, ignore_none=False):
     """
     Checks if id is valid
     """
     if id is None and ignore_none:
         return
     try:
         uuid.UUID(str(id))
     except Exception as exc:
-        raise ValueError(f"{id} is not a valid UUID.") from exc
+        raise FlValueError(f"{id} is not a valid UUID.") from exc
 
 
 def beta_feature(feature_name: str):
     """Prints warning message when used on a function which is BETA feature.
 
     Parameters
     ----------
@@ -43,7 +45,30 @@
 
 # pylint: disable=bare-except
 def _get_value_or_none(callable):
     try:
         return callable()
     except:
         return None
+
+
+def validate_type(value, parameter_name: str, expected_type):
+    """validate type
+
+    Parameters
+    ----------
+    value :
+        value to be validated
+    parameter_name : str
+        paremeter name - used for error message
+    expected_type : type
+        expected type for value
+
+    Raises
+    ------
+    TypeError
+        when value is not expected_type
+    """
+    if not isinstance(value, expected_type):
+        raise FlTypeError(
+            f"Expected type={expected_type} for {parameter_name}, but got value={value} (type={type(value)})"
+        )
```

### Comparing `flow360-0.2.0b5/flow360/component/validator.py` & `flow360-0.2.0b6/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/component/volume_mesh.py` & `flow360-0.2.0b6/flow360/component/volume_mesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     ResourceDraft,
 )
 from .types import COMMENTS
+from .utils import validate_type
 from .validator import Validator
 
 try:
     import h5py
 
     _H5PY_AVAILABLE = True
 except ImportError:
@@ -300,14 +301,15 @@
 
     id: str = Field(alias="meshId")
     name: str = Field(alias="meshName")
     created_at: str = Field(alias="meshAddTime")
     surface_mesh_id: Optional[str] = Field(alias="surfaceMeshId")
     mesh_params: Union[Flow360MeshParams, None, dict] = Field(alias="meshParams")
     mesh_format: Union[VolumeMeshFileFormat, None] = Field(alias="meshFormat")
+    file_name: Union[str, None] = Field(alias="fileName")
     endianness: UGRIDEndianness = Field(alias="meshEndianness")
     compression: CompressionFormat = Field(alias="meshCompression")
     boundaries: Union[List, None]
 
     @validator("mesh_params", pre=True)
     def init_mesh_params(cls, value):
         """
@@ -372,16 +374,20 @@
             )
 
         if isascii is True:
             raise Flow360NotImplementedError("isascii not supported")
 
         self.params = None
         if params is not None:
-            if not isinstance(params, Flow360MeshParams):
-                raise ValueError(f"params={params} are not of type Flow360MeshParams")
+            if not isinstance(params, Flow360MeshParams) and not isinstance(
+                params, VolumeMeshingParams
+            ):
+                raise ValueError(
+                    f"params={params} are not of type Flow360MeshParams OR VolumeMeshingParams"
+                )
             self.params = params.copy(deep=True)
 
         if name is None and file_name is not None:
             name = os.path.splitext(os.path.basename(file_name))[0]
 
         self.file_name = file_name
         self.name = name
@@ -407,14 +413,15 @@
         resp = RestApi(self._endpoint).post(body)
         if not resp:
             return None
 
         info = VolumeMeshMeta(**resp)
         self._id = info.id
         mesh = VolumeMesh(self.id)
+        log.info(f"VolumeMesh successfully submitted: {mesh.short_description()}")
         return mesh
 
     # pylint: disable=protected-access
     def _submit_upload_mesh(self, progress_callback=None):
         assert os.path.exists(self.file_name)
 
         compression, file_name_no_compression = CompressionFormat.detect(self.file_name)
@@ -443,14 +450,15 @@
 
         info = VolumeMeshMeta(**resp)
         self._id = info.id
         mesh = VolumeMesh(self.id)
         remote_file_name = mesh._remote_file_name(mesh_format, compression, endianness)
         mesh.upload_file(remote_file_name, self.file_name, progress_callback=progress_callback)
         mesh._complete_upload(remote_file_name)
+        log.info(f"VolumeMesh successfully uploaded: {mesh.short_description()}")
         return mesh
 
     def submit(self, progress_callback=None) -> VolumeMesh:
         """submit mesh to cloud
 
         Parameters
         ----------
@@ -482,38 +490,32 @@
 
 
 class VolumeMesh(VolumeMeshBase, Flow360Resource):
     """
     Volume mesh component
     """
 
-    def __init__(self, mesh_id: str = None, meta_info: VolumeMeshMeta = None):
-        if (mesh_id is None and meta_info is None) or (
-            mesh_id is not None and meta_info is not None
-        ):
-            raise ValueError("You must provide mesh_id OR meta_info to constructor.")
-
-        if meta_info is not None:
-            mesh_id = meta_info.id
-
-        assert mesh_id is not None
-
+    # pylint: disable=redefined-builtin
+    def __init__(self, id: str):
         super().__init__(
             resource_type="Volume Mesh",
             info_type_class=VolumeMeshMeta,
             s3_transfer_method=S3TransferType.VOLUME_MESH,
             endpoint=self._endpoint,
-            id=mesh_id,
+            id=id,
         )
-
-        if meta_info is not None:
-            self._info = meta_info
-
         self.__mesh_params = None
 
+    @classmethod
+    def _from_meta(cls, meta: VolumeMeshMeta):
+        validate_type(meta, "meta", VolumeMeshMeta)
+        volume_mesh = cls(id=meta.id)
+        volume_mesh._set_meta(meta)
+        return volume_mesh
+
     @property
     def info(self) -> VolumeMeshMeta:
         return super().info
 
     @property
     def _mesh_params(self) -> Flow360MeshParams:
         """
@@ -561,22 +563,29 @@
             file_name,
             to_file,
             keep_folder=keep_folder,
             overwrite=overwrite,
             progress_callback=progress_callback,
         )
 
-    def download(self, to_file=".", keep_folder: bool = True):
+    def download(self, to_file=".", keep_folder: bool = True, overwrite: bool = True):
         """
         Download volume mesh file
         :param to_file:
         :param keep_folder:
         :return:
         """
-        super().download_file(self._remote_file_name(), to_file, keep_folder)
+        status = self.status
+        if not status.is_final():
+            log.warning(f"Cannot download file because status={status}")
+        else:
+            remote_file_name = self.info.file_name
+            if remote_file_name is None:
+                remote_file_name = self._remote_file_name()
+            super().download_file(remote_file_name, to_file, keep_folder, overwrite=overwrite)
 
     def download_log(self, log_file: VolumeMeshLog, to_file=".", keep_folder: bool = True):
         """
         Download logs
         :param log_file:
         :param to_file: file name on local disk, could be either folder or file name.
         :param keep_folder: If true, the downloaded file will be put in the same folder as the file on cloud. Only work
```

### Comparing `flow360-0.2.0b5/flow360/environment.py` & `flow360-0.2.0b6/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b6/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b6/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b6/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b6/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/base_test_case.py` & `flow360-0.2.0b6/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b6/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b6/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b6/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b6/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b6/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b6/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b6/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b6/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b6/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b6/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/exceptions.py` & `flow360-0.2.0b6/flow360/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,30 +13,42 @@
 
 
 # pylint: disable=redefined-builtin
 class ValueError(Flow360Error):
     """Error with value."""
 
 
+class TypeError(Flow360Error):
+    """Error with type."""
+
+
 class ConfigError(Flow360Error):
     """Error when configuring Flow360."""
 
 
+class RuntimeError(Flow360Error):
+    """Error when runtime."""
+
+
 class Flow360KeyError(Flow360Error):
     """Could not find a key in a Flow360 dictionary."""
 
 
 class ValidationError(Flow360Error):
     """Error when constructing FLow360 components."""
 
 
 class FileError(Flow360Error):
     """Error reading or writing to file."""
 
 
+class CloudFileError(Flow360Error):
+    """Error when getting file from cloud."""
+
+
 class WebError(Flow360Error):
     """Error with the webAPI."""
 
 
 class WebNotFoundError(Flow360Error):
     """Error with the webAPI."""
```

### Comparing `flow360-0.2.0b5/flow360/log.py` & `flow360-0.2.0b6/flow360/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     stderr : bool
         If False, logs are directed to stdout, otherwise to stderr.
     """
     if "console" in log.handlers:
         previous_level = log.handlers["console"].level
     else:
         previous_level = DEFAULT_LEVEL
-    log.handlers["console"] = LogHandler(Console(stderr=stderr), previous_level)
+    log.handlers["console"] = LogHandler(Console(stderr=stderr, log_path=False), previous_level)
 
 
 def set_logging_file(
     fname: str,
     filemode: str = "w",
     level: LogValue = DEFAULT_LEVEL,
 ) -> None:
@@ -166,12 +166,12 @@
     try:
         # pylint: disable=consider-using-with,unspecified-encoding
         file = open(fname, filemode)
     except:  # pylint: disable=bare-except
         log.error(f"File {fname} could not be opened")
         return
 
-    log.handlers["file"] = LogHandler(Console(file=file), level)
+    log.handlers["file"] = LogHandler(Console(file=file, log_path=False), level)
 
 
 # Set default logging output
 set_logging_console()
```

### Comparing `flow360-0.2.0b5/flow360/solver_version.py` & `flow360-0.2.0b6/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b5/flow360/user_config.py` & `flow360-0.2.0b6/flow360/user_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     def __init__(self):
         self._read_config()
         self.set_profile(DEFAULT_PROFILE)
         self._check_env_profile()
         self._apikey = None
         self._check_env_apikey()
         self._do_validation = True
+        self._suppress_submit_warning = None
 
     def _check_env_profile(self):
         simcloud_profile = os.environ.get("SIMCLOUD_PROFILE", None)
         if simcloud_profile is not None and simcloud_profile != self.profile:
             log.info(f"Found env variable SIMCLOUD_PROFILE={simcloud_profile}")
             self.set_profile(simcloud_profile)
 
@@ -41,15 +42,15 @@
 
     @property
     def profile(self):
         """profile"""
         return self._profile
 
     def set_profile(self, profile: str = DEFAULT_PROFILE):
-        """_summary_
+        """set_profile
 
         Parameters
         ----------
         profile : str, optional
             profile to be used, eg. dev, default, by default "default"
         """
         self._profile = profile
@@ -73,21 +74,35 @@
         self._check_env_profile()
         self._check_env_apikey()
         if self._apikey is not None:
             return self._apikey
         return self.config.get(self.profile, {}).get("apikey", "")
 
     def suppress_submit_warning(self):
+        """locally suppress submit warning"""
+        self._suppress_submit_warning = True
+
+    def cancel_local_submit_warning_settings(self):
+        """cancel local submit warning settings"""
+        self._suppress_submit_warning = None
+
+    def show_submit_warning(self):
+        """locally show submit warning"""
+        self._suppress_submit_warning = False
+
+    def is_suppress_submit_warning(self):
         """suppress submit warning config
 
         Returns
         -------
         bool
             whether to suppress submit warnings
         """
+        if self._suppress_submit_warning is not None:
+            return self._suppress_submit_warning
         return self.config.get("user", {}).get("config", {}).get("suppress_submit_warning", False)
 
     @property
     def do_validation(self):
         """for handling user side validation (pydantic)
 
         Returns
```

### Comparing `flow360-0.2.0b5/pyproject.toml` & `flow360-0.2.0b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b5"
+version = "v0.2.0b6"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
```

### Comparing `flow360-0.2.0b5/PKG-INFO` & `flow360-0.2.0b6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b5
+Version: 0.2.0b6
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

