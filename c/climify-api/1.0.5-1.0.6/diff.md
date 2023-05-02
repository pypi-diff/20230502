# Comparing `tmp/climify_api-1.0.5.tar.gz` & `tmp/climify_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climify_api-1.0.5.tar", last modified: Tue May  2 09:47:35 2023, max compression
+gzip compressed data, was "climify_api-1.0.6.tar", last modified: Tue May  2 10:00:20 2023, max compression
```

## Comparing `climify_api-1.0.5.tar` & `climify_api-1.0.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.327955 climify_api-1.0.5/
--rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      932 2023-05-02 09:47:35.327401 climify_api-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.237488 climify_api-1.0.5/climify_api/
--rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.5/climify_api/ApiController.py
--rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.5/climify_api/REST.py
--rw-rw-rw-   0        0        0      904 2023-05-02 09:47:10.000000 climify_api-1.0.5/climify_api/__init__.py
--rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.5/climify_api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.256799 climify_api-1.0.5/climify_api/apis/
--rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.5/climify_api/apis/PathBase.py
--rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.5/climify_api/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.261331 climify_api-1.0.5/climify_api/apis/v1/
--rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.5/climify_api/apis/v1/ApiController.py
--rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.5/climify_api/apis/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.263635 climify_api-1.0.5/climify_api/apis/v1/paths/
--rw-rw-rw-   0        0        0      986 2023-04-11 09:18:57.000000 climify_api-1.0.5/climify_api/apis/v1/paths/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.268047 climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id/
--rw-rw-rw-   0        0        0       70 2023-03-21 09:44:46.000000 climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id/__init__.py
--rw-rw-rw-   0        0        0     3225 2023-04-04 10:10:47.000000 climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.274262 climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id_devices/
--rw-rw-rw-   0        0        0       85 2023-03-21 09:44:47.000000 climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3286 2023-04-04 10:10:55.000000 climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.279380 climify_api-1.0.5/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/
--rw-rw-rw-   0        0        0      115 2023-04-11 09:18:32.000000 climify_api-1.0.5/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/__init__.py
--rw-rw-rw-   0        0        0     4283 2023-04-11 11:58:43.000000 climify_api-1.0.5/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.284597 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id/
--rw-rw-rw-   0        0        0       70 2023-03-21 09:44:49.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id/__init__.py
--rw-rw-rw-   0        0        0     3135 2023-04-04 10:11:09.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.289006 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_change_temperature/
--rw-rw-rw-   0        0        0      101 2023-03-21 09:44:51.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_change_temperature/__init__.py
--rw-rw-rw-   0        0        0     3585 2023-04-04 10:11:23.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_change_temperature/post.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.293289 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_devices/
--rw-rw-rw-   0        0        0       85 2023-03-21 09:44:53.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3218 2023-04-04 10:11:55.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.297777 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_sensor_values/
--rw-rw-rw-   0        0        0       96 2023-03-21 09:44:54.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_sensor_values/__init__.py
--rw-rw-rw-   0        0        0     5894 2023-04-11 14:16:47.000000 climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_sensor_values/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.302590 climify_api-1.0.5/climify_api/apis/v1/paths/maps_id/
--rw-rw-rw-   0        0        0       60 2023-03-21 09:44:58.000000 climify_api-1.0.5/climify_api/apis/v1/paths/maps_id/__init__.py
--rw-rw-rw-   0        0        0     3028 2023-04-04 10:11:55.000000 climify_api-1.0.5/climify_api/apis/v1/paths/maps_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.307682 climify_api-1.0.5/climify_api/apis/v1/paths/maps_id_devices/
--rw-rw-rw-   0        0        0       75 2023-03-21 09:45:00.000000 climify_api-1.0.5/climify_api/apis/v1/paths/maps_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3162 2023-04-04 10:11:55.000000 climify_api-1.0.5/climify_api/apis/v1/paths/maps_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.312351 climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id/
--rw-rw-rw-   0        0        0       78 2023-03-21 09:45:02.000000 climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id/__init__.py
--rw-rw-rw-   0        0        0     3295 2023-04-04 10:11:55.000000 climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.317243 climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id_devices/
--rw-rw-rw-   0        0        0       93 2023-03-21 09:45:03.000000 climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3341 2023-04-04 10:11:55.000000 climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.321952 climify_api-1.0.5/climify_api/apis/v1/paths/resources/
--rw-rw-rw-   0        0        0       71 2023-03-21 09:45:05.000000 climify_api-1.0.5/climify_api/apis/v1/paths/resources/__init__.py
--rw-rw-rw-   0        0        0     2543 2023-04-04 10:11:47.000000 climify_api-1.0.5/climify_api/apis/v1/paths/resources/get.py
--rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.5/climify_api/auth.py
--rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.5/climify_api/configuration.py
--rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.5/climify_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.324865 climify_api-1.0.5/climify_api/models/
--rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.5/climify_api/models/__init__.py
--rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.5/climify_api/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:47:35.250977 climify_api-1.0.5/climify_api.egg-info/
--rw-rw-rw-   0        0        0      932 2023-05-02 09:47:35.000000 climify_api-1.0.5/climify_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-05-02 09:47:35.000000 climify_api-1.0.5/climify_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:47:35.000000 climify_api-1.0.5/climify_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2023-05-02 09:47:35.000000 climify_api-1.0.5/climify_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 09:47:35.000000 climify_api-1.0.5/climify_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2157 2023-05-02 09:47:07.000000 climify_api-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 09:47:35.328971 climify_api-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.235200 climify_api-1.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      932 2023-05-02 10:00:20.234454 climify_api-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.154647 climify_api-1.0.6/climify_api/
+-rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.6/climify_api/ApiController.py
+-rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.6/climify_api/REST.py
+-rw-rw-rw-   0        0        0      904 2023-05-02 09:59:57.000000 climify_api-1.0.6/climify_api/__init__.py
+-rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.6/climify_api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.168706 climify_api-1.0.6/climify_api/apis/
+-rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.6/climify_api/apis/PathBase.py
+-rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.6/climify_api/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.171707 climify_api-1.0.6/climify_api/apis/v1/
+-rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.6/climify_api/apis/v1/ApiController.py
+-rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.6/climify_api/apis/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.173133 climify_api-1.0.6/climify_api/apis/v1/paths/
+-rw-rw-rw-   0        0        0      986 2023-04-11 09:18:57.000000 climify_api-1.0.6/climify_api/apis/v1/paths/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.177013 climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id/
+-rw-rw-rw-   0        0        0       70 2023-03-21 09:44:46.000000 climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id/__init__.py
+-rw-rw-rw-   0        0        0     3225 2023-04-04 10:10:47.000000 climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.180846 climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id_devices/
+-rw-rw-rw-   0        0        0       85 2023-03-21 09:44:47.000000 climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3286 2023-04-04 10:10:55.000000 climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.184960 climify_api-1.0.6/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/
+-rw-rw-rw-   0        0        0      115 2023-04-11 09:18:32.000000 climify_api-1.0.6/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/__init__.py
+-rw-rw-rw-   0        0        0     4283 2023-04-11 11:58:43.000000 climify_api-1.0.6/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.188104 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id/
+-rw-rw-rw-   0        0        0       70 2023-03-21 09:44:49.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id/__init__.py
+-rw-rw-rw-   0        0        0     3135 2023-04-04 10:11:09.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.193107 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_change_temperature/
+-rw-rw-rw-   0        0        0      101 2023-03-21 09:44:51.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_change_temperature/__init__.py
+-rw-rw-rw-   0        0        0     3585 2023-04-04 10:11:23.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_change_temperature/post.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.198777 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_devices/
+-rw-rw-rw-   0        0        0       85 2023-03-21 09:44:53.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3218 2023-04-04 10:11:55.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.203316 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_sensor_values/
+-rw-rw-rw-   0        0        0       96 2023-03-21 09:44:54.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_sensor_values/__init__.py
+-rw-rw-rw-   0        0        0     5894 2023-04-11 14:16:47.000000 climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_sensor_values/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.210307 climify_api-1.0.6/climify_api/apis/v1/paths/maps_id/
+-rw-rw-rw-   0        0        0       60 2023-03-21 09:44:58.000000 climify_api-1.0.6/climify_api/apis/v1/paths/maps_id/__init__.py
+-rw-rw-rw-   0        0        0     3028 2023-04-04 10:11:55.000000 climify_api-1.0.6/climify_api/apis/v1/paths/maps_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.214064 climify_api-1.0.6/climify_api/apis/v1/paths/maps_id_devices/
+-rw-rw-rw-   0        0        0       75 2023-03-21 09:45:00.000000 climify_api-1.0.6/climify_api/apis/v1/paths/maps_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3162 2023-04-04 10:11:55.000000 climify_api-1.0.6/climify_api/apis/v1/paths/maps_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.219081 climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id/
+-rw-rw-rw-   0        0        0       78 2023-03-21 09:45:02.000000 climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id/__init__.py
+-rw-rw-rw-   0        0        0     3295 2023-04-04 10:11:55.000000 climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.224087 climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id_devices/
+-rw-rw-rw-   0        0        0       93 2023-03-21 09:45:03.000000 climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3341 2023-04-04 10:11:55.000000 climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.228592 climify_api-1.0.6/climify_api/apis/v1/paths/resources/
+-rw-rw-rw-   0        0        0       71 2023-03-21 09:45:05.000000 climify_api-1.0.6/climify_api/apis/v1/paths/resources/__init__.py
+-rw-rw-rw-   0        0        0     2543 2023-04-04 10:11:47.000000 climify_api-1.0.6/climify_api/apis/v1/paths/resources/get.py
+-rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.6/climify_api/auth.py
+-rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.6/climify_api/configuration.py
+-rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.6/climify_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.232367 climify_api-1.0.6/climify_api/models/
+-rw-rw-rw-   0        0        0     6779 2023-05-02 09:59:34.000000 climify_api-1.0.6/climify_api/models/__init__.py
+-rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.6/climify_api/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:00:20.165408 climify_api-1.0.6/climify_api.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-05-02 10:00:20.000000 climify_api-1.0.6/climify_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1940 2023-05-02 10:00:20.000000 climify_api-1.0.6/climify_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 10:00:20.000000 climify_api-1.0.6/climify_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-05-02 10:00:20.000000 climify_api-1.0.6/climify_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 10:00:20.000000 climify_api-1.0.6/climify_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2157 2023-05-02 09:59:45.000000 climify_api-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 10:00:20.235200 climify_api-1.0.6/setup.cfg
```

### Comparing `climify_api-1.0.5/LICENSE` & `climify_api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/PKG-INFO` & `climify_api-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.5/climify_api/REST.py` & `climify_api-1.0.6/climify_api/REST.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/__init__.py` & `climify_api-1.0.6/climify_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Provides a REST endpoints for Climify applications and 3rd party solutions.  # noqa: E501
 
     The version of the OpenAPI document: 1.2.3
     Generated by: https://openapi-generator.tech
 """
 
 __name__ = 'climify_api'
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 # import ApiClient
 from climify_api.api_client import ApiClient
 
 # import Configuration
 from climify_api.configuration import Configuration, ClimifyRegion
```

### Comparing `climify_api-1.0.5/climify_api/api_client.py` & `climify_api-1.0.6/climify_api/api_client.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/PathBase.py` & `climify_api-1.0.6/climify_api/apis/PathBase.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/ApiController.py` & `climify_api-1.0.6/climify_api/apis/v1/ApiController.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/__init__.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/buildings_id_devices/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/buildings_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/locations_id/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/locations_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_change_temperature/post.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_change_temperature/post.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_devices/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/locations_id_sensor_values/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/locations_id_sensor_values/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/maps_id/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/maps_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/maps_id_devices/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/maps_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/organisations_id_devices/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/organisations_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/apis/v1/paths/resources/get.py` & `climify_api-1.0.6/climify_api/apis/v1/paths/resources/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/auth.py` & `climify_api-1.0.6/climify_api/auth.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/configuration.py` & `climify_api-1.0.6/climify_api/configuration.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/exceptions.py` & `climify_api-1.0.6/climify_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api/models/__init__.py` & `climify_api-1.0.6/climify_api/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,17 @@
     values: Optional[Dict[str, Any]] = None
 
 
 class SensorDataExtDto(BaseModel):
     devId: Optional[str] = None
     data: Optional[Union[List[Data],DataFrame]] = None
 
+    class Config:
+        arbitrary_types_allowed = True
+
 
 class BuildingDto(BaseModel):
     id: Optional[int] = None
     status: Optional[Status] = None
     name: Optional[constr(min_length=0, max_length=200)] = None
     country: Optional[constr(min_length=0, max_length=2)] = None
     address: Optional[constr(min_length=0, max_length=100)] = None
```

### Comparing `climify_api-1.0.5/climify_api/schemas.py` & `climify_api-1.0.6/climify_api/schemas.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/climify_api.egg-info/PKG-INFO` & `climify_api-1.0.6/climify_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.5/climify_api.egg-info/SOURCES.txt` & `climify_api-1.0.6/climify_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.5/pyproject.toml` & `climify_api-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "climify_api"
-version = "1.0.5"
+version = "1.0.6"
 keywords=['Climify','Environmental engineering']
 authors = [
   { name="Climify Aps", email="info@climify.com" },
 ]
 description = "A wrapper library for the Climify REST API"
 #long_description = "A wrapper library for the Climify REST API, used to query sensor data and interact with Climify systems programmatically"
 readme = "README.md"
```

