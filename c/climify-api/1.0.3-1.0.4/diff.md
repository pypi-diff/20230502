# Comparing `tmp/climify_api-1.0.3.tar.gz` & `tmp/climify_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climify_api-1.0.3.tar", last modified: Tue May  2 09:26:36 2023, max compression
+gzip compressed data, was "climify_api-1.0.4.tar", last modified: Tue May  2 09:39:39 2023, max compression
```

## Comparing `climify_api-1.0.3.tar` & `climify_api-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.287683 climify_api-1.0.3/
--rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      932 2023-05-02 09:26:36.286681 climify_api-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.240746 climify_api-1.0.3/climify_api/
--rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.3/climify_api/ApiController.py
--rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.3/climify_api/REST.py
--rw-rw-rw-   0        0        0      904 2023-05-02 09:23:35.000000 climify_api-1.0.3/climify_api/__init__.py
--rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.3/climify_api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.272050 climify_api-1.0.3/climify_api/apis/
--rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.3/climify_api/apis/PathBase.py
--rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.3/climify_api/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.276476 climify_api-1.0.3/climify_api/apis/v1/
--rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.3/climify_api/apis/v1/ApiController.py
--rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.3/climify_api/apis/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.280159 climify_api-1.0.3/climify_api/apis/v1/paths/
--rw-rw-rw-   0        0        0      986 2023-04-11 09:18:57.000000 climify_api-1.0.3/climify_api/apis/v1/paths/__init__.py
--rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.3/climify_api/auth.py
--rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.3/climify_api/configuration.py
--rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.3/climify_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.283661 climify_api-1.0.3/climify_api/models/
--rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.3/climify_api/models/__init__.py
--rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.3/climify_api/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.265134 climify_api-1.0.3/climify_api.egg-info/
--rw-rw-rw-   0        0        0      932 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1516 2023-05-02 09:23:30.000000 climify_api-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 09:26:36.287683 climify_api-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.285191 climify_api-1.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      932 2023-05-02 09:39:39.284189 climify_api-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.159267 climify_api-1.0.4/climify_api/
+-rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.4/climify_api/ApiController.py
+-rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.4/climify_api/REST.py
+-rw-rw-rw-   0        0        0      904 2023-05-02 09:38:06.000000 climify_api-1.0.4/climify_api/__init__.py
+-rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.4/climify_api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.173710 climify_api-1.0.4/climify_api/apis/
+-rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.4/climify_api/apis/PathBase.py
+-rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.4/climify_api/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.176705 climify_api-1.0.4/climify_api/apis/v1/
+-rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.4/climify_api/apis/v1/ApiController.py
+-rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.4/climify_api/apis/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.178712 climify_api-1.0.4/climify_api/apis/v1/paths/
+-rw-rw-rw-   0        0        0      986 2023-04-11 09:18:57.000000 climify_api-1.0.4/climify_api/apis/v1/paths/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.188721 climify_api-1.0.4/climify_api/apis/v1/paths/buildings_id/
+-rw-rw-rw-   0        0        0       70 2023-03-21 09:44:46.000000 climify_api-1.0.4/climify_api/apis/v1/paths/buildings_id/__init__.py
+-rw-rw-rw-   0        0        0     3225 2023-04-04 10:10:47.000000 climify_api-1.0.4/climify_api/apis/v1/paths/buildings_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.199640 climify_api-1.0.4/climify_api/apis/v1/paths/buildings_id_devices/
+-rw-rw-rw-   0        0        0       85 2023-03-21 09:44:47.000000 climify_api-1.0.4/climify_api/apis/v1/paths/buildings_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3286 2023-04-04 10:10:55.000000 climify_api-1.0.4/climify_api/apis/v1/paths/buildings_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.207511 climify_api-1.0.4/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/
+-rw-rw-rw-   0        0        0      115 2023-04-11 09:18:32.000000 climify_api-1.0.4/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/__init__.py
+-rw-rw-rw-   0        0        0     4283 2023-04-11 11:58:43.000000 climify_api-1.0.4/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.218059 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id/
+-rw-rw-rw-   0        0        0       70 2023-03-21 09:44:49.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id/__init__.py
+-rw-rw-rw-   0        0        0     3135 2023-04-04 10:11:09.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.224113 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_change_temperature/
+-rw-rw-rw-   0        0        0      101 2023-03-21 09:44:51.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_change_temperature/__init__.py
+-rw-rw-rw-   0        0        0     3585 2023-04-04 10:11:23.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_change_temperature/post.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.233518 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_devices/
+-rw-rw-rw-   0        0        0       85 2023-03-21 09:44:53.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3218 2023-04-04 10:11:55.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.240520 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_sensor_values/
+-rw-rw-rw-   0        0        0       96 2023-03-21 09:44:54.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_sensor_values/__init__.py
+-rw-rw-rw-   0        0        0     5894 2023-04-11 14:16:47.000000 climify_api-1.0.4/climify_api/apis/v1/paths/locations_id_sensor_values/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.249517 climify_api-1.0.4/climify_api/apis/v1/paths/maps_id/
+-rw-rw-rw-   0        0        0       60 2023-03-21 09:44:58.000000 climify_api-1.0.4/climify_api/apis/v1/paths/maps_id/__init__.py
+-rw-rw-rw-   0        0        0     3028 2023-04-04 10:11:55.000000 climify_api-1.0.4/climify_api/apis/v1/paths/maps_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.255517 climify_api-1.0.4/climify_api/apis/v1/paths/maps_id_devices/
+-rw-rw-rw-   0        0        0       75 2023-03-21 09:45:00.000000 climify_api-1.0.4/climify_api/apis/v1/paths/maps_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3162 2023-04-04 10:11:55.000000 climify_api-1.0.4/climify_api/apis/v1/paths/maps_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.264520 climify_api-1.0.4/climify_api/apis/v1/paths/organisations_id/
+-rw-rw-rw-   0        0        0       78 2023-03-21 09:45:02.000000 climify_api-1.0.4/climify_api/apis/v1/paths/organisations_id/__init__.py
+-rw-rw-rw-   0        0        0     3295 2023-04-04 10:11:55.000000 climify_api-1.0.4/climify_api/apis/v1/paths/organisations_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.270519 climify_api-1.0.4/climify_api/apis/v1/paths/organisations_id_devices/
+-rw-rw-rw-   0        0        0       93 2023-03-21 09:45:03.000000 climify_api-1.0.4/climify_api/apis/v1/paths/organisations_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3341 2023-04-04 10:11:55.000000 climify_api-1.0.4/climify_api/apis/v1/paths/organisations_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.277522 climify_api-1.0.4/climify_api/apis/v1/paths/resources/
+-rw-rw-rw-   0        0        0       71 2023-03-21 09:45:05.000000 climify_api-1.0.4/climify_api/apis/v1/paths/resources/__init__.py
+-rw-rw-rw-   0        0        0     2543 2023-04-04 10:11:47.000000 climify_api-1.0.4/climify_api/apis/v1/paths/resources/get.py
+-rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.4/climify_api/auth.py
+-rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.4/climify_api/configuration.py
+-rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.4/climify_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.282192 climify_api-1.0.4/climify_api/models/
+-rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.4/climify_api/models/__init__.py
+-rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.4/climify_api/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:39:39.170529 climify_api-1.0.4/climify_api.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-05-02 09:39:39.000000 climify_api-1.0.4/climify_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1940 2023-05-02 09:39:39.000000 climify_api-1.0.4/climify_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:39:39.000000 climify_api-1.0.4/climify_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-05-02 09:39:39.000000 climify_api-1.0.4/climify_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 09:39:39.000000 climify_api-1.0.4/climify_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2144 2023-05-02 09:39:21.000000 climify_api-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:39:39.285191 climify_api-1.0.4/setup.cfg
```

### Comparing `climify_api-1.0.3/LICENSE` & `climify_api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/PKG-INFO` & `climify_api-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify_api
-Version: 1.0.3
+Version: 1.0.4
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.3/climify_api/REST.py` & `climify_api-1.0.4/climify_api/REST.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/__init__.py` & `climify_api-1.0.4/climify_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Provides a REST endpoints for Climify applications and 3rd party solutions.  # noqa: E501
 
     The version of the OpenAPI document: 1.2.3
     Generated by: https://openapi-generator.tech
 """
 
 __name__ = 'climify_api'
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 # import ApiClient
 from climify_api.api_client import ApiClient
 
 # import Configuration
 from climify_api.configuration import Configuration, ClimifyRegion
```

### Comparing `climify_api-1.0.3/climify_api/api_client.py` & `climify_api-1.0.4/climify_api/api_client.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/apis/PathBase.py` & `climify_api-1.0.4/climify_api/apis/PathBase.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/apis/v1/ApiController.py` & `climify_api-1.0.4/climify_api/apis/v1/ApiController.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/apis/v1/paths/__init__.py` & `climify_api-1.0.4/climify_api/apis/v1/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/auth.py` & `climify_api-1.0.4/climify_api/auth.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/configuration.py` & `climify_api-1.0.4/climify_api/configuration.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/exceptions.py` & `climify_api-1.0.4/climify_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/models/__init__.py` & `climify_api-1.0.4/climify_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api/schemas.py` & `climify_api-1.0.4/climify_api/schemas.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.3/climify_api.egg-info/PKG-INFO` & `climify_api-1.0.4/climify_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

