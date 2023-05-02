# Comparing `tmp/granular_engine-0.2.2.tar.gz` & `tmp/granular_engine-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granular_engine-0.2.2.tar", max compression
+gzip compressed data, was "granular_engine-0.2.3.tar", max compression
```

## Comparing `granular_engine-0.2.2.tar` & `granular_engine-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0      743 2023-01-02 20:48:11.409336 granular_engine-0.2.2/README.rst
--rwxr-xr-x   0        0        0      238 2023-01-02 20:49:03.947363 granular_engine-0.2.2/engine/__init__.py
--rwxr-xr-x   0        0        0      881 2023-01-02 20:35:07.469529 granular_engine-0.2.2/engine/cli/__init__.py
--rwxr-xr-x   0        0        0     1608 2023-01-02 20:35:07.476528 granular_engine-0.2.2/engine/cli/auth.py
--rwxr-xr-x   0        0        0      964 2022-11-02 00:34:44.519544 granular_engine-0.2.2/engine/cli/experiment.py
--rwxr-xr-x   0        0        0     7725 2023-01-02 20:35:07.483527 granular_engine-0.2.2/engine/cli/project.py
--rwxr-xr-x   0        0        0      158 2023-01-01 23:04:46.429811 granular_engine-0.2.2/engine/connections/__init__.py
--rwxr-xr-x   0        0        0     5206 2023-01-02 20:35:07.492527 granular_engine-0.2.2/engine/connections/callisto.py
--rwxr-xr-x   0        0        0     4332 2022-12-29 23:25:52.426746 granular_engine-0.2.2/engine/connections/dione.py
--rwxr-xr-x   0        0        0     4946 2023-01-02 17:52:08.440775 granular_engine-0.2.2/engine/connections/europa.py
--rwxr-xr-x   0        0        0      574 2023-01-01 23:04:46.454812 granular_engine-0.2.2/engine/connections/neso.py
--rwxr-xr-x   0        0        0     3528 2022-12-29 23:25:52.433705 granular_engine-0.2.2/engine/grain.py
--rwxr-xr-x   0        0        0        0 2023-01-01 23:04:46.460920 granular_engine-0.2.2/engine/libs/__init__.py
--rwxr-xr-x   0        0        0     1240 2023-01-01 23:04:46.470932 granular_engine-0.2.2/engine/libs/inquirer.py
--rwxr-xr-x   0        0        0     1208 2023-01-02 20:49:03.944363 granular_engine-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 granular_engine-0.2.2/setup.py
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 granular_engine-0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0      743 2023-05-01 16:39:46.439016 granular_engine-0.2.3/README.rst
+-rwxr-xr-x   0        0        0      238 2023-05-01 16:41:33.140801 granular_engine-0.2.3/engine/__init__.py
+-rwxr-xr-x   0        0        0      881 2023-05-01 16:39:24.278291 granular_engine-0.2.3/engine/cli/__init__.py
+-rwxr-xr-x   0        0        0     1608 2023-05-01 16:39:24.293915 granular_engine-0.2.3/engine/cli/auth.py
+-rwxr-xr-x   0        0        0      964 2022-11-02 00:34:44.519544 granular_engine-0.2.3/engine/cli/experiment.py
+-rwxr-xr-x   0        0        0     7816 2023-05-01 16:41:21.750990 granular_engine-0.2.3/engine/cli/project.py
+-rwxr-xr-x   0        0        0      158 2023-05-01 16:39:24.340790 granular_engine-0.2.3/engine/connections/__init__.py
+-rwxr-xr-x   0        0        0     5206 2023-05-01 16:39:24.356418 granular_engine-0.2.3/engine/connections/callisto.py
+-rwxr-xr-x   0        0        0     4332 2022-12-29 23:25:52.426746 granular_engine-0.2.3/engine/connections/dione.py
+-rwxr-xr-x   0        0        0     4969 2023-05-01 16:41:21.769127 granular_engine-0.2.3/engine/connections/europa.py
+-rwxr-xr-x   0        0        0     1238 2023-05-01 16:41:21.782633 granular_engine-0.2.3/engine/connections/neso.py
+-rwxr-xr-x   0        0        0     3528 2022-12-29 23:25:52.433705 granular_engine-0.2.3/engine/grain.py
+-rwxr-xr-x   0        0        0        0 2023-05-01 16:39:24.387667 granular_engine-0.2.3/engine/libs/__init__.py
+-rwxr-xr-x   0        0        0     1240 2023-05-01 16:39:24.418916 granular_engine-0.2.3/engine/libs/inquirer.py
+-rwxr-xr-x   0        0        0     1208 2023-05-01 16:41:33.139594 granular_engine-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 granular_engine-0.2.3/setup.py
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 granular_engine-0.2.3/PKG-INFO
```

### Comparing `granular_engine-0.2.2/README.rst` & `granular_engine-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/engine/cli/__init__.py` & `granular_engine-0.2.3/engine/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/engine/cli/auth.py` & `granular_engine-0.2.3/engine/cli/auth.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/engine/cli/experiment.py` & `granular_engine-0.2.3/engine/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/engine/cli/project.py` & `granular_engine-0.2.3/engine/cli/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,20 @@
     if show_detail:
         if project["description"]:
             print (Fore.GREEN + "Description : " + Style.RESET_ALL, end="")
             print (Fore.GREEN + project['description'] + Style.RESET_ALL)
 
         if project["sensorIds"]:
             print (Fore.GREEN + "Sensors : " + Style.RESET_ALL, end="")
-            neso = Neso(callisto, None)
-            sensors = neso.get_sensors()
+            if org:
+                neso = Neso(callisto, org["id"])
+            else:
+                neso = Neso(callisto, None)
             sensor_ids = project['sensorIds']
+            sensors = neso.get_sensors()
             sensor_names = [sensors[sensor_id]["name"] for sensor_id in sensor_ids]
             print (Fore.GREEN + ', '.join(sensor_names) + Style.RESET_ALL)
 
         if project["problemType"]:
             print (Fore.GREEN + "Problem Type : " + Style.RESET_ALL, end="")
             print (Fore.GREEN + project['problemType'] + Style.RESET_ALL)
```

### Comparing `granular_engine-0.2.2/engine/connections/callisto.py` & `granular_engine-0.2.3/engine/connections/callisto.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/engine/connections/dione.py` & `granular_engine-0.2.3/engine/connections/dione.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/engine/connections/europa.py` & `granular_engine-0.2.3/engine/connections/europa.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,47 +22,47 @@
             for i in range(len(labels[key])):
                 llist.append(labelmaps[i][labels[key][i]])
             labels[key] = llist
         
         return labels
 
     def get_image_details(self, id):
-        image_url = f'{self.callisto.host}/europa/api/v1/images/{id}'
+        image_url = f'{self.callisto.host}/europa/api/v2/projects/{id}'
 
         response = requests.get(image_url, headers=self.callisto.headers)
 
         if response.status_code == 200:
             image = response.json()['image']
             return image['tiles'], image['geometry'], image['status']
         else:
             print(f'Image details cannot be retrieved')
             print(f'Image meta endpoint {image_url} returned with HTTP status code : {response.status_code}')
             return None, None, None
             
     def get_projects(self):
         if self.org:
-            get_project_url = f'{self.callisto.host}/europa/api/v1/tasks?orgId={self.org}'
+            get_project_url = f'{self.callisto.host}/europa/api/v2/projects?orgId={self.org}'
         else:
-            get_project_url = f"{self.callisto.host}/europa/api/v1/tasks?search=&status=all&isPublic=true"
+            get_project_url = f"{self.callisto.host}/europa/api/v2/projects?search=&status=all&isPublic=true"
         response = requests.get(get_project_url, headers=self.callisto.headers)
 
         if response.status_code == 200:
             projects = response.json()['results']
 
             return projects
         else:
             print(f'All GeoEngine projects cannot be retrieved')
             print(f'Projects endpoint {get_project_url} returned with HTTP status code : {response.status_code}\n')
             return None
 
     def get_project_details(self, id, verbose=True):
         if self.org:
-            project_details_url = f'{self.callisto.host}/europa/api/v1/tasks/{id}?orgId={self.org}'
+            project_details_url = f'{self.callisto.host}/europa/api/v2/projects/{id}?orgId={self.org}'
         else:
-            project_details_url = f"{self.callisto.host}/europa/api/v1/tasks/{id}?search=&status=all&isPublic=true"
+            project_details_url = f"{self.callisto.host}/europa/api/v2/projects/{id}?search=&status=all&isPublic=true"
 
         response = requests.get(project_details_url, headers=self.callisto.headers)
         
         if response.status_code == 200:
             project = response.json()['task']
             
             if verbose:
@@ -84,15 +84,15 @@
             return project
         else:
             print(f'Project details cannot be retrieved')
             print(f'Project details endpoint {project_details_url} returned with HTTP status code : {response.status_code}\n')
             return None 
             
     # def export_annotations(self, id):
-    #     export_url = f'{self.callisto.host}/europa/api/v1/tasks/{id}/export'
+    #     export_url = f'{self.callisto.host}/europa/api/v2/projects/{id}/export'
 
     #     print(f'exporting annotations for task id : {id}')
 
     #     response = requests.post(export_url, headers=self.callisto.headers)
 
     #     if response.status_code != 200:
     #         print('cannot export annotations')
@@ -100,17 +100,17 @@
     #         return
     #     else:
     #         print('annotations export requested')
 
     
     def get_project_exports(self, id):
         if self.org:
-            project_exports_url = f'{self.callisto.host}/europa/api/v1/tasks/{id}/datasets?orgId={self.org}'
+            project_exports_url = f'{self.callisto.host}/europa/api/v2/projects/{id}/datasets?orgId={self.org}'
         else:
-            project_exports_url = f"{self.callisto.host}/europa/api/v1/tasks/{id}/datasets?search=&status=all&isPublic=true"
+            project_exports_url = f"{self.callisto.host}/europa/api/v2/projects/{id}/datasets?search=&status=all&isPublic=true"
 
         response = requests.get(project_exports_url, headers=self.callisto.headers)
         
         response = requests.get(project_exports_url, headers=self.callisto.headers)
 
         if response.status_code == 200:
             exports = response.json()['results']
```

### Comparing `granular_engine-0.2.2/engine/grain.py` & `granular_engine-0.2.3/engine/grain.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/engine/libs/inquirer.py` & `granular_engine-0.2.3/engine/libs/inquirer.py`

 * *Files identical despite different names*

### Comparing `granular_engine-0.2.2/pyproject.toml` & `granular_engine-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "granular-engine"
-version = "v0.2.2"
+version = "v0.2.3"
 description = "Experiment tracking for GeoSpatial Machine Learning on GeoEngine"
 authors = ["Sagar Verma <sagar@granular.ai>", "Siddharth Gupta <sid@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "engine"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `granular_engine-0.2.2/setup.py` & `granular_engine-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'yacs>=0.1.8,<0.2.0']
 
 entry_points = \
 {'console_scripts': ['engine = engine.cli:cli']}
 
 setup_kwargs = {
     'name': 'granular-engine',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Experiment tracking for GeoSpatial Machine Learning on GeoEngine',
     'long_description': 'Engine\n======\n\nA Utility Library that assists in Geospatial Machine Learning Experiment\nTracking.\n\nInstallation\n------------\n\n.. code:: shell\n\n   pip install granular-engine\n\nUsage\n-----\n\nCLI\n~~~\n\n.. figure:: https://user-images.githubusercontent.com/2713531/210276844-16d3867d-461c-44ba-870b-00d6d6266dbf.gif\n   :alt: engine_cli\n\n   engine_cli\n\nExperiment Tracking\n~~~~~~~~~~~~~~~~~~~\n\n.. code:: python\n\n   from engine import Engine\n\n   engine = Engine("test_config.yaml")\n\n   for epoch in enumerate(epochs):\n      # train \n      # eval\n      engine.log(step=epoch, train_loss=train_loss, val_loss=val_loss)\n\n   engine.done()\n\nLicense\n-------\n\nGPLv3\n\nDocumentation\n-------------\n\nView documentation ``here <https://engine.granular.ai/>``\\ \\_\n',
     'author': 'Sagar Verma',
     'author_email': 'sagar@granular.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/granularai/engine',
```

### Comparing `granular_engine-0.2.2/PKG-INFO` & `granular_engine-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granular-engine
-Version: 0.2.2
+Version: 0.2.3
 Summary: Experiment tracking for GeoSpatial Machine Learning on GeoEngine
 Home-page: https://github.com/granularai/engine
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

