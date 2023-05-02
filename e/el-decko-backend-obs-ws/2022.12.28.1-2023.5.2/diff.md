# Comparing `tmp/el_decko_backend_obs_ws-2022.12.28.1.tar.gz` & `tmp/el_decko_backend_obs_ws-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "el_decko_backend_obs_ws-2022.12.28.1.tar", last modified: Fri Dec 30 16:48:28 2022, max compression
+gzip compressed data, was "el_decko_backend_obs_ws-2023.5.2.tar", last modified: Tue May  2 20:04:09 2023, max compression
```

## Comparing `el_decko_backend_obs_ws-2022.12.28.1.tar` & `el_decko_backend_obs_ws-2023.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2022-12-30 16:48:28.661619 el_decko_backend_obs_ws-2022.12.28.1/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2022-12-25 21:52:46.000000 el_decko_backend_obs_ws-2022.12.28.1/LICENSE
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2248 2022-12-30 16:48:28.661619 el_decko_backend_obs_ws-2022.12.28.1/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1679 2022-12-30 16:47:19.000000 el_decko_backend_obs_ws-2022.12.28.1/README.md
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      991 2022-12-30 16:47:01.000000 el_decko_backend_obs_ws-2022.12.28.1/pyproject.toml
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2022-12-30 16:48:28.661619 el_decko_backend_obs_ws-2022.12.28.1/setup.cfg
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2022-12-30 16:48:28.661619 el_decko_backend_obs_ws-2022.12.28.1/src/
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2022-12-30 16:48:28.661619 el_decko_backend_obs_ws-2022.12.28.1/src/edb_obs_ws/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     3807 2022-12-30 16:47:06.000000 el_decko_backend_obs_ws-2022.12.28.1/src/edb_obs_ws/__init__.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      670 2022-12-28 18:51:48.000000 el_decko_backend_obs_ws-2022.12.28.1/src/edb_obs_ws/endpoints.py
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2022-12-30 16:48:28.661619 el_decko_backend_obs_ws-2022.12.28.1/src/el_decko_backend_obs_ws.egg-info/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2248 2022-12-30 16:48:28.000000 el_decko_backend_obs_ws-2022.12.28.1/src/el_decko_backend_obs_ws.egg-info/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      395 2022-12-30 16:48:28.000000 el_decko_backend_obs_ws-2022.12.28.1/src/el_decko_backend_obs_ws.egg-info/SOURCES.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2022-12-30 16:48:28.000000 el_decko_backend_obs_ws-2022.12.28.1/src/el_decko_backend_obs_ws.egg-info/dependency_links.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      146 2022-12-30 16:48:28.000000 el_decko_backend_obs_ws-2022.12.28.1/src/el_decko_backend_obs_ws.egg-info/entry_points.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       16 2022-12-30 16:48:28.000000 el_decko_backend_obs_ws-2022.12.28.1/src/el_decko_backend_obs_ws.egg-info/requires.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       11 2022-12-30 16:48:28.000000 el_decko_backend_obs_ws-2022.12.28.1/src/el_decko_backend_obs_ws.egg-info/top_level.txt
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-02 20:04:09.105918 el_decko_backend_obs_ws-2023.5.2/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_backend_obs_ws-2023.5.2/LICENSE
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     3654 2023-05-02 20:04:09.105918 el_decko_backend_obs_ws-2023.5.2/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     3089 2023-05-02 20:03:39.000000 el_decko_backend_obs_ws-2023.5.2/README.md
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      991 2023-03-22 10:21:15.000000 el_decko_backend_obs_ws-2023.5.2/pyproject.toml
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-02 20:04:09.105918 el_decko_backend_obs_ws-2023.5.2/setup.cfg
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-02 20:04:09.101918 el_decko_backend_obs_ws-2023.5.2/src/
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-02 20:04:09.105918 el_decko_backend_obs_ws-2023.5.2/src/edb_obs_ws/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4943 2023-05-02 19:15:36.000000 el_decko_backend_obs_ws-2023.5.2/src/edb_obs_ws/__init__.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1477 2023-05-02 19:30:32.000000 el_decko_backend_obs_ws-2023.5.2/src/edb_obs_ws/endpoints.py
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-02 20:04:09.105918 el_decko_backend_obs_ws-2023.5.2/src/el_decko_backend_obs_ws.egg-info/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     3654 2023-05-02 20:04:09.000000 el_decko_backend_obs_ws-2023.5.2/src/el_decko_backend_obs_ws.egg-info/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      395 2023-05-02 20:04:09.000000 el_decko_backend_obs_ws-2023.5.2/src/el_decko_backend_obs_ws.egg-info/SOURCES.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-02 20:04:09.000000 el_decko_backend_obs_ws-2023.5.2/src/el_decko_backend_obs_ws.egg-info/dependency_links.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      146 2023-05-02 20:04:09.000000 el_decko_backend_obs_ws-2023.5.2/src/el_decko_backend_obs_ws.egg-info/entry_points.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       16 2023-05-02 20:04:09.000000 el_decko_backend_obs_ws-2023.5.2/src/el_decko_backend_obs_ws.egg-info/requires.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       11 2023-05-02 20:04:09.000000 el_decko_backend_obs_ws-2023.5.2/src/el_decko_backend_obs_ws.egg-info/top_level.txt
```

### Comparing `el_decko_backend_obs_ws-2022.12.28.1/LICENSE` & `el_decko_backend_obs_ws-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `el_decko_backend_obs_ws-2022.12.28.1/PKG-INFO` & `el_decko_backend_obs_ws-2023.5.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: el_decko_backend_obs_ws
-Version: 2022.12.28.1
-Summary: OBS Studio websocket backend for El Decko. Allow your Elgato Stream Deck to control OBS Studio using it's webscoket server
-Author-email: Imo 'Vortex Acherontic' Hester <vortex@z-ray.de>
-License: GPL-3
-Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_backend_obs_ws
-Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_backend_obs_ws/issues
-Platform: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # El Decko Backend OBS Studio Websocket
 
 OBS Studio websocket based backend for El Decko.
 
 ## First run
 
 Upon running El Decko the first time with this backend installed it will create an empty default config to connect to
@@ -60,7 +47,57 @@
 
 #### GetSceneList
 
 Returns a list with all available Scenes within OBS Studio.
 
 Event name: `GetSceneList`  
 Parameters: `None`
+
+#### SetSceneItemEnabled
+
+Set the enabled state of an item inside a given scene  
+
+Event name: `SetSceneItemEnabled`
+Parameters:  
+`scene_name` -> The name of the scene  
+`item_id` -> The internal ID of the required item.  
+You can find this inside your OBS Scene Settings JSON.  
+`enabled` -> True or False to show/hide the item.
+
+##### Example JSON:
+````
+"key_config": {
+    "<key_number>": {
+        "backend": "edb_obs_ws",
+        "event": "SetSceneItemEnabled",
+        "event_parameters": {"scene_name":"S: Confeti", "item_id": 42, "enabled": false},
+        "image_idle": "<some_image_path>",
+        "image_pressed": null,
+        "label": "Hide Video"
+      },
+}
+````
+
+#### ToggleSceneItemEnabled
+
+Similar to SetSceneItemEnabled does this event show/hide an item in a given scene.  
+But additionally it queries the current item state and sets it to the opposite state. 
+
+Event name: `SetSceneItemEnabled`
+Parameters:  
+`scene_name` -> The name of the scene  
+`item_id` -> The internal ID of the required item.  
+You can find this inside your OBS Scene Settings JSON.  
+
+##### Example JSON:
+````
+"key_config": {
+    "<key_number>": {
+        "backend": "edb_obs_ws",
+        "event": "ToggleSceneItemEnabled",
+        "event_parameters": {"scene_name":"S: Confeti", "item_id": 2},
+        "image_idle": "<some_image_path>",
+        "image_pressed": null,
+        "label": "Confetti!"
+      },
+}
+````
```

### Comparing `el_decko_backend_obs_ws-2022.12.28.1/pyproject.toml` & `el_decko_backend_obs_ws-2023.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `el_decko_backend_obs_ws-2022.12.28.1/src/edb_obs_ws/__init__.py` & `el_decko_backend_obs_ws-2023.5.2/src/edb_obs_ws/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     xdg_data_home,
     xdg_runtime_dir,
     xdg_state_home,
 )
 
 from edb_obs_ws import endpoints
 
-VERSION = "2022.12.28.1"
+VERSION = "2023.5.2"
 
 config_path: str = str(xdg_config_home()) + "/eldecko/backend/"
 config_file: str = config_path + "obsws.json"
 host = "localhost"
 port = "4455"
 password = "1234IsABadPassword"
 websocket: WebSocketClient = None
@@ -62,14 +62,26 @@
         "GetVersion": {"human_readable_name": "Get OBS Studio Version"},
         "SetCurrentProgramScene": {
             "human_readable_name": "Switch OBS Studio Scene",
             "name": "string"
         },
         "GetSceneList": {
             "human_readable_name": "Returns list of all available scenes"
+        },
+        "SetSceneItemEnabled": {
+            "human_readable_name": "Set the enabled state of a given scene Item in a given scene",
+            "scene_name": "string",
+            "item_id": "integer",
+            "enabled": "boolean"
+        },
+        "ToggleSceneItemEnabled": {
+            "human_readable_name": "Toggles the enabled state of a Set the enabled state of a given item in a scene",
+            "scene_name": "string",
+            "item_id": "integer",
+            "enabled": "boolean"
         }
     }
 
 
 def __load_obs_ws_config():
     global host
     global port
@@ -114,9 +126,17 @@
     match even_type:
         case "GetVersion":
             result = await endpoints.__get_version(websocket)
         case "SetCurrentProgramScene":
             result = await endpoints.__set_current_program_scene(websocket, event_properties["name"])
         case "GetSceneList":
             result = await endpoints.__get_scene_list(websocket)
+        case "SetSceneItemEnabled":
+            result = await endpoints.__set_scene_item_enabled(websocket,
+                                                              event_properties["scene_name"],
+                                                              event_properties["item_id"],
+                                                              event_properties["enabled"])
+        case "ToggleSceneItemEnabled":
+            result = await endpoints.__toggle_scene_item_enabled(websocket, event_properties["scene_name"],
+                                                                 event_properties["item_id"])
         case other:
             pass
```

