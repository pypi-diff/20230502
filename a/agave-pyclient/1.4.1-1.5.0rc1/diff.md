# Comparing `tmp/agave_pyclient-1.4.1.tar.gz` & `tmp/agave_pyclient-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agave_pyclient-1.4.1.tar", last modified: Tue Jul  5 23:36:57 2022, max compression
+gzip compressed data, was "agave_pyclient-1.5.0rc1.tar", last modified: Mon May  1 22:25:53 2023, max compression
```

## Comparing `agave_pyclient-1.4.1.tar` & `agave_pyclient-1.5.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 23:36:57.340057 agave_pyclient-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-07-05 23:36:57.340057 agave_pyclient-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 23:36:57.340057 agave_pyclient-1.4.1/agave_pyclient/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/agave_pyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28775 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/agave_pyclient/agave.py
--rw-r--r--   0 runner    (1001) docker     (121)     6976 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/agave_pyclient/commandbuffer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 23:36:57.340057 agave_pyclient-1.4.1/agave_pyclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-07-05 23:36:57.000000 agave_pyclient-1.4.1/agave_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-07-05 23:36:57.000000 agave_pyclient-1.4.1/agave_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 23:36:57.000000 agave_pyclient-1.4.1/agave_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-05 23:36:57.000000 agave_pyclient-1.4.1/agave_pyclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 23:36:57.000000 agave_pyclient-1.4.1/agave_pyclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-07-05 23:36:57.000000 agave_pyclient-1.4.1/agave_pyclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-05 23:36:57.000000 agave_pyclient-1.4.1/agave_pyclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 23:36:57.340057 agave_pyclient-1.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/docs/agave_renderer.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     5379 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-07-05 23:36:57.340057 agave_pyclient-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-07-05 23:36:52.000000 agave_pyclient-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:25:53.515018 agave_pyclient-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-01 22:25:53.515018 agave_pyclient-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:25:53.515018 agave_pyclient-1.5.0rc1/agave_pyclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/agave_pyclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/agave_pyclient/agave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/agave_pyclient/commandbuffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:25:53.515018 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-01 22:25:53.000000 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-01 22:25:53.000000 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:25:53.000000 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 22:25:53.000000 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:25:53.000000 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-01 22:25:53.000000 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 22:25:53.000000 agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:25:53.515018 agave_pyclient-1.5.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/docs/agave_renderer.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5384 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 22:25:53.515018 agave_pyclient-1.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-01 22:25:40.000000 agave_pyclient-1.5.0rc1/setup.py
```

### Comparing `agave_pyclient-1.4.1/CONTRIBUTING.md` & `agave_pyclient-1.5.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.4.1/LICENSE` & `agave_pyclient-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.4.1/PKG-INFO` & `agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: agave_pyclient
-Version: 1.4.1
+Name: agave-pyclient
+Version: 1.5.0rc1
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
 Platform: UNKNOWN
@@ -45,21 +45,27 @@
 
 You must have Agave installed. On command line, run:
 
 ```
 agave --server &
 ```
 
+For Linux headless operation, you need to tell the Qt library to use the offscreen platform plugin:
+
+```
+agave -platform offscreen --server &
+```
+
 ```python
 from agave_pyclient import AgaveRenderer
 
 # 1. connect to the agave server
 r = agave_pyclient.AgaveRenderer()
 # 2. tell it what data to load
-r.load_volume_from_file("my_favorite.ome.tiff", 0, 0)
+r.load_data("my_favorite.ome.tiff")
 # 3. set some render settings (abbreviated list here)
 r.set_resolution(681, 612)
 r.background_color(0, 0, 0)
 r.render_iterations(128)
 r.set_primary_ray_step_size(4)
 r.set_secondary_ray_step_size(4)
 r.set_voxel_scale(0.270833, 0.270833, 0.53)
```

### Comparing `agave_pyclient-1.4.1/README.md` & `agave_pyclient-1.5.0rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,27 @@
 
 You must have Agave installed. On command line, run:
 
 ```
 agave --server &
 ```
 
+For Linux headless operation, you need to tell the Qt library to use the offscreen platform plugin:
+
+```
+agave -platform offscreen --server &
+```
+
 ```python
 from agave_pyclient import AgaveRenderer
 
 # 1. connect to the agave server
 r = agave_pyclient.AgaveRenderer()
 # 2. tell it what data to load
-r.load_volume_from_file("my_favorite.ome.tiff", 0, 0)
+r.load_data("my_favorite.ome.tiff")
 # 3. set some render settings (abbreviated list here)
 r.set_resolution(681, 612)
 r.background_color(0, 0, 0)
 r.render_iterations(128)
 r.set_primary_ray_step_size(4)
 r.set_secondary_ray_step_size(4)
 r.set_voxel_scale(0.270833, 0.270833, 0.53)
```

### Comparing `agave_pyclient-1.4.1/agave_pyclient/agave.py` & `agave_pyclient-1.5.0rc1/agave_pyclient/agave.py`

 * *Files 6% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             This name is the path where volume images are located.
         """
         # 1
         self.cb.add_command("ASSET_PATH", name)
 
     def load_ome_tif(self, name: str):
         """
-        DEPRECATED. Use load_volume_from_file
+        DEPRECATED. Use load_data
         """
         # 2
         self.cb.add_command("LOAD_OME_TIF", name)
 
     def eye(self, x: float, y: float, z: float):
         """
         Set the viewer camera position.
@@ -812,25 +812,15 @@
             intensity value.  All others are linearly interpolated.
         """
         # 38
         self.cb.add_command("SET_CONTROL_POINTS", channel, data)
 
     def load_volume_from_file(self, path: str, scene: int, time: int):
         """
-        Load a volume
-
-        Parameters
-        ----------
-        path: str
-            The file path must be locally accessible from where the AGAVE server is
-            running.
-        scene: int
-            zero-based index to select the scene, for multi-scene files. Defaults to 0
-        time: int
-            zero-based index to select the time sample.  Defaults to 0
+        DEPRECATED. Use load_data
         """
         # 39
         self.cb.add_command("LOAD_VOLUME_FROM_FILE", path, scene, time)
 
     def set_time(self, time: int):
         """
         Load a time from the current volume file
@@ -867,14 +857,53 @@
         ----------
         on: int
             0 to hide bounding box, 1 to show it
         """
         # 42
         self.cb.add_command("SHOW_BOUNDING_BOX", on)
 
+    def load_data(
+        self,
+        path: str,
+        scene: int = 0,
+        multiresolution_level: int = 0,
+        time: int = 0,
+        channels: List[int] = [],
+        region: List[int] = [],
+    ):
+        """
+        Completely specify volume data to load
+
+        Parameters
+        ----------
+        path: str
+            URL or directory or file path to the data. The path must be locally
+            accessible from the AGAVE server.
+
+        scene: int
+            zero-based index to select the scene, for multi-scene files. Defaults to 0
+
+        multiresolution_level: int
+            zero-based index to select the multiresolution level.  Defaults to 0
+
+        time: int
+            zero-based index to select the time sample.  Defaults to 0
+
+        channels: List[int]
+            zero-based indices to select the channels.  Defaults to all channels
+
+        region: List[int]
+            6 integers specifying the region to load.  Defaults to the entire volume.
+            Any list length other than 0 or 6 is an error.
+        """
+        # 44
+        self.cb.add_command(
+            "LOAD_DATA", path, scene, multiresolution_level, time, channels, region
+        )
+
     def batch_render_turntable(
         self, number_of_frames=90, direction=1, output_name="frame", first_frame=0
     ):
         """
         Loop to render a turntable sequence, a 360 degree rotation about the vertical
         axis.  Other commands must have been previously issued to load the data and set
         all the viewing parameters.
```

### Comparing `agave_pyclient-1.4.1/agave_pyclient/commandbuffer.py` & `agave_pyclient-1.5.0rc1/agave_pyclient/commandbuffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # command id will be int32 to future-proof it.
 # note that the server needs to know these signatures too.
 COMMANDS = {
     # tell server to identify this session?
     "SESSION": [0, "S"],
     # tell server where files might be (appends to existing)
     "ASSET_PATH": [1, "S"],
-    # load a volume
+    # load a volume (DEPRECATED)
     "LOAD_OME_TIF": [2, "S"],
     # set camera pos
     "EYE": [3, "F32", "F32", "F32"],
     # set camera target pt
     "TARGET": [4, "F32", "F32", "F32"],
     # set camera up direction
     "UP": [5, "F32", "F32", "F32"],
@@ -61,20 +61,23 @@
     "SET_SECONDARY_RAY_STEP_SIZE": [35, "F32"],
     # r, g, b
     "BACKGROUND_COLOR": [36, "F32", "F32", "F32"],
     # channel index, isovalue, isorange
     "SET_ISOVALUE_THRESHOLD": [37, "I32", "F32", "F32"],
     # channel index, array of [stop, r, g, b, a]
     "SET_CONTROL_POINTS": [38, "I32", "F32A"],
-    # path, scene, time
+    # path, scene, time (DEPRECATED)
     "LOAD_VOLUME_FROM_FILE": [39, "S", "I32", "I32"],
+    # causes data to be loaded
     "SET_TIME": [40, "I32"],
     "SET_BOUNDING_BOX_COLOR": [41, "F32", "F32", "F32"],
     "SHOW_BOUNDING_BOX": [42, "I32"],
     "TRACKBALL_CAMERA": [43, "F32", "F32"],
+    # path, scene, multiresolution level, t, channel indices, region
+    "LOAD_DATA": [44, "S", "I32", "I32", "I32", "I32A", "I32A"],
 }
 
 
 # strategy: add elements to prebuffer,
 # and then traverse prebuffer to convert to binary before sending?
 class CommandBuffer:
     def __init__(self, command_list=None):
@@ -120,14 +123,19 @@
                 elif argtype == "I32":
                     bytesize += 4
                 elif argtype == "F32A":
                     # one int32 for array length
                     bytesize += 4
                     # followed by one float for each element in the array
                     bytesize += 4 * len(command[j + 1])
+                elif argtype == "I32A":
+                    # one int32 for array length
+                    bytesize += 4
+                    # followed by one int32 for each element in the array
+                    bytesize += 4 * len(command[j + 1])
         return bytesize
 
     def make_buffer(self):
         bytesize = self.compute_size()
 
         # allocate arraybuffer and then fill it.
         self.buffer = bytearray(bytesize)
@@ -163,14 +171,21 @@
                 elif argtype == "F32A":
                     flist = cmd[j + 1]
                     struct.pack_into(">i", self.buffer, offset, len(flist))
                     offset += 4
                     for k in flist:
                         struct.pack_into("f", self.buffer, offset, k)
                         offset += 4
+                elif argtype == "I32A":
+                    ilist = cmd[j + 1]
+                    struct.pack_into(">i", self.buffer, offset, len(ilist))
+                    offset += 4
+                    for k in ilist:
+                        struct.pack_into(">i", self.buffer, offset, k)
+                        offset += 4
 
         # result is in this.buffer
         return self.buffer
 
     # commands are added by command code string name
     # followed by appropriate signature args.
     def add_command(self, *args):
```

### Comparing `agave_pyclient-1.4.1/agave_pyclient.egg-info/PKG-INFO` & `agave_pyclient-1.5.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: agave-pyclient
-Version: 1.4.1
+Name: agave_pyclient
+Version: 1.5.0rc1
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
 Platform: UNKNOWN
@@ -45,21 +45,27 @@
 
 You must have Agave installed. On command line, run:
 
 ```
 agave --server &
 ```
 
+For Linux headless operation, you need to tell the Qt library to use the offscreen platform plugin:
+
+```
+agave -platform offscreen --server &
+```
+
 ```python
 from agave_pyclient import AgaveRenderer
 
 # 1. connect to the agave server
 r = agave_pyclient.AgaveRenderer()
 # 2. tell it what data to load
-r.load_volume_from_file("my_favorite.ome.tiff", 0, 0)
+r.load_data("my_favorite.ome.tiff")
 # 3. set some render settings (abbreviated list here)
 r.set_resolution(681, 612)
 r.background_color(0, 0, 0)
 r.render_iterations(128)
 r.set_primary_ray_step_size(4)
 r.set_secondary_ray_step_size(4)
 r.set_voxel_scale(0.270833, 0.270833, 0.53)
```

### Comparing `agave_pyclient-1.4.1/agave_pyclient.egg-info/requires.txt` & `agave_pyclient-1.5.0rc1/agave_pyclient.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 numpy
 ws4py==0.5.1
-Pillow==9.0.1
+Pillow==9.3.0
 
 [all]
 numpy
 ws4py==0.5.1
-Pillow==9.0.1
+Pillow==9.3.0
 pytest-runner>=5.2
 black>=19.10b0
-codecov>=2.1.4
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
@@ -24,15 +23,14 @@
 tox>=3.15.2
 twine>=3.1.1
 wheel>=0.34.2
 
 [dev]
 pytest-runner>=5.2
 black>=19.10b0
-codecov>=2.1.4
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
@@ -46,13 +44,12 @@
 wheel>=0.34.2
 
 [setup]
 pytest-runner>=5.2
 
 [test]
 black>=19.10b0
-codecov>=2.1.4
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
```

### Comparing `agave_pyclient-1.4.1/docs/Makefile` & `agave_pyclient-1.5.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.4.1/docs/conf.py` & `agave_pyclient-1.5.0rc1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 author = u"Daniel Toloudis"
 
 # The version info for the project you"re documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The full version, including alpha/beta/rc tags
-release = "1.4.1"
+release = "1.5.0-rc.1"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `agave_pyclient-1.4.1/docs/index.rst` & `agave_pyclient-1.5.0rc1/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 .. code-block:: python
 
    from agave_pyclient import AgaveRenderer
 
    # 1. connect to the agave server
    r = agave_pyclient.AgaveRenderer()
    # 2. tell it what data to load
-   r.load_volume_from_file("my_favorite.ome.tiff", 0, 0)
+   r.load_data("my_favorite.ome.tiff", 0, 0, 0, [], [])
    # 3. set some render settings (abbreviated list here)
    r.set_resolution(681, 612)
    r.background_color(0, 0, 0)
    r.render_iterations(128)
    r.set_primary_ray_step_size(4)
    r.set_secondary_ray_step_size(4)
    r.set_voxel_scale(0.270833, 0.270833, 0.53)
```

### Comparing `agave_pyclient-1.4.1/docs/make.bat` & `agave_pyclient-1.5.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.4.1/setup.py` & `agave_pyclient-1.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 setup_requirements = [
     "pytest-runner>=5.2",
 ]
 
 test_requirements = [
     "black>=19.10b0",
-    "codecov>=2.1.4",
     "flake8>=3.8.3",
     "flake8-debugger>=3.2.1",
     "pytest>=5.4.3",
     "pytest-cov>=2.9.0",
     "pytest-raises>=0.11",
 ]
 
@@ -33,15 +32,15 @@
     "Sphinx>=3.4.3",
     "sphinx_rtd_theme>=0.5.1",
     "tox>=3.15.2",
     "twine>=3.1.1",
     "wheel>=0.34.2",
 ]
 
-requirements = ["numpy", "ws4py==0.5.1", "Pillow==9.0.1"]
+requirements = ["numpy", "ws4py==0.5.1", "Pillow==9.3.0"]
 
 extra_requirements = {
     "setup": setup_requirements,
     "test": test_requirements,
     "dev": dev_requirements,
     "all": [*requirements, *dev_requirements,],
 }
@@ -80,10 +79,10 @@
     setup_requires=setup_requirements,
     test_suite="agave_pyclient/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/allen-cell-animated/agave",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="1.4.1",
+    version="1.5.0-rc.1",
     zip_safe=False,
 )
```

