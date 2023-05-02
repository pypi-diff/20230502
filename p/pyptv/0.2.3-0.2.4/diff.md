# Comparing `tmp/pyptv-0.2.3.tar.gz` & `tmp/pyptv-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyptv-0.2.3.tar", last modified: Wed Apr 26 14:16:11 2023, max compression
+gzip compressed data, was "pyptv-0.2.4.tar", last modified: Tue May  2 20:28:44 2023, max compression
```

## Comparing `pyptv-0.2.3.tar` & `pyptv-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.449212 pyptv-0.2.3/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2022-11-16 19:45:05.000000 pyptv-0.2.3/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)      297 2023-04-26 14:16:11.449212 pyptv-0.2.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1611 2023-03-05 14:40:34.000000 pyptv-0.2.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.445212 pyptv-0.2.3/pyptv/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-11-16 20:26:01.000000 pyptv-0.2.3/pyptv/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)       29 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    41516 2023-04-21 19:00:59.000000 pyptv-0.2.3/pyptv/calibration_gui.py
--rw-rw-r--   0 user      (1000) user      (1000)       37 2022-11-15 19:14:45.000000 pyptv-0.2.3/pyptv/cli.py
--rw-rw-r--   0 user      (1000) user      (1000)     2299 2023-03-12 06:56:19.000000 pyptv-0.2.3/pyptv/code_editor.py
--rw-rw-r--   0 user      (1000) user      (1000)    20362 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/detection_gui.py
--rw-rw-r--   0 user      (1000) user      (1000)      924 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/directory_editor.py
--rw-rw-r--   0 user      (1000) user      (1000)      831 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/draw_3d_target.py
--rw-rw-r--   0 user      (1000) user      (1000)     2723 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/ext_sequence_denis.py
--rw-rw-r--   0 user      (1000) user      (1000)     1280 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/ext_tracker_denis.py
--rw-rw-r--   0 user      (1000) user      (1000)     3135 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/image_inspector.py
--rw-rw-r--   0 user      (1000) user      (1000)     1377 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/imageplot.py
--rw-rw-r--   0 user      (1000) user      (1000)     7172 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/imread_chaco.py
--rw-rw-r--   0 user      (1000) user      (1000)    46489 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/parameter_gui.py
--rw-rw-r--   0 user      (1000) user      (1000)    42351 2023-04-21 19:16:14.000000 pyptv-0.2.3/pyptv/parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)    16707 2023-03-12 06:56:19.000000 pyptv-0.2.3/pyptv/ptv.py
--rw-rw-r--   0 user      (1000) user      (1000)     3958 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/pyptv_batch.py
--rw-rw-r--   0 user      (1000) user      (1000)    54729 2023-04-26 14:14:02.000000 pyptv-0.2.3/pyptv/pyptv_gui.py
--rw-rw-r--   0 user      (1000) user      (1000)     1974 2023-03-05 14:40:34.000000 pyptv-0.2.3/pyptv/quiver_demo.py
--rw-rw-r--   0 user      (1000) user      (1000)     4673 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/quiverplot.py
--rw-rw-r--   0 user      (1000) user      (1000)     3485 2023-03-12 06:56:19.000000 pyptv-0.2.3/pyptv/scatter_inspector2.py
--rw-rw-r--   0 user      (1000) user      (1000)     4277 2022-11-16 19:45:05.000000 pyptv-0.2.3/pyptv/text_box_overlay.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.449212 pyptv-0.2.3/pyptv.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      297 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      730 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       47 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      102 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-04-26 14:16:11.000000 pyptv-0.2.3/pyptv.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-26 14:16:11.449212 pyptv-0.2.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      727 2023-04-26 13:47:35.000000 pyptv-0.2.3/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-26 14:16:11.449212 pyptv-0.2.3/tests/
--rw-rw-r--   0 user      (1000) user      (1000)       88 2022-11-16 19:45:05.000000 pyptv-0.2.3/tests/test_cli.py
--rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-16 19:45:05.000000 pyptv-0.2.3/tests/test_pyptv_batch.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 20:28:44.046822 pyptv-0.2.4/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2022-11-16 19:45:05.000000 pyptv-0.2.4/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      297 2023-05-02 20:28:44.046822 pyptv-0.2.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1611 2023-03-05 14:40:34.000000 pyptv-0.2.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 20:28:44.042822 pyptv-0.2.4/pyptv/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-11-16 20:26:01.000000 pyptv-0.2.4/pyptv/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2022-11-16 19:45:05.000000 pyptv-0.2.4/pyptv/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    41802 2023-05-02 19:44:16.000000 pyptv-0.2.4/pyptv/calibration_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2022-11-15 19:14:45.000000 pyptv-0.2.4/pyptv/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2299 2023-03-12 06:56:19.000000 pyptv-0.2.4/pyptv/code_editor.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20362 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/detection_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)      924 2022-11-16 19:45:05.000000 pyptv-0.2.4/pyptv/directory_editor.py
+-rw-rw-r--   0 user      (1000) user      (1000)      831 2022-11-16 19:45:05.000000 pyptv-0.2.4/pyptv/draw_3d_target.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2723 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/ext_sequence_denis.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1280 2022-11-16 19:45:05.000000 pyptv-0.2.4/pyptv/ext_tracker_denis.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3135 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/image_inspector.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1377 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/imageplot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7172 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/imread_chaco.py
+-rw-rw-r--   0 user      (1000) user      (1000)    46489 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/parameter_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)    42351 2023-04-21 19:16:14.000000 pyptv-0.2.4/pyptv/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16707 2023-03-12 06:56:19.000000 pyptv-0.2.4/pyptv/ptv.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3958 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/pyptv_batch.py
+-rw-rw-r--   0 user      (1000) user      (1000)    54729 2023-05-02 20:07:40.000000 pyptv-0.2.4/pyptv/pyptv_gui.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1974 2023-03-05 14:40:34.000000 pyptv-0.2.4/pyptv/quiver_demo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4673 2022-11-16 19:45:05.000000 pyptv-0.2.4/pyptv/quiverplot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3485 2023-03-12 06:56:19.000000 pyptv-0.2.4/pyptv/scatter_inspector2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4277 2022-11-16 19:45:05.000000 pyptv-0.2.4/pyptv/text_box_overlay.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 20:28:44.046822 pyptv-0.2.4/pyptv.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      297 2023-05-02 20:28:43.000000 pyptv-0.2.4/pyptv.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      730 2023-05-02 20:28:44.000000 pyptv-0.2.4/pyptv.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-02 20:28:43.000000 pyptv-0.2.4/pyptv.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       47 2023-05-02 20:28:43.000000 pyptv-0.2.4/pyptv.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      102 2023-05-02 20:28:43.000000 pyptv-0.2.4/pyptv.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-05-02 20:28:43.000000 pyptv-0.2.4/pyptv.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-02 20:28:44.046822 pyptv-0.2.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      727 2023-05-02 20:07:40.000000 pyptv-0.2.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-02 20:28:44.046822 pyptv-0.2.4/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2022-11-16 19:45:05.000000 pyptv-0.2.4/tests/test_cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-16 19:45:05.000000 pyptv-0.2.4/tests/test_pyptv_batch.py
```

### Comparing `pyptv-0.2.3/LICENSE.txt` & `pyptv-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/README.md` & `pyptv-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/calibration_gui.py` & `pyptv-0.2.4/pyptv/calibration_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 import os
 import shutil
 import re
 from  pathlib import Path
 import numpy as np
 from skimage.io import imread
-from skimage import img_as_ubyte
+from skimage.util import img_as_ubyte
 from skimage.color import rgb2gray
 
 from traits.api import HasTraits, Str, Int, Bool, Instance, Button
 from traitsui.api import View, Item, HGroup, VGroup, ListEditor
 from enable.component_editor import ComponentEditor
+    
 from chaco.api import (
     Plot,
     ArrayPlotData,
     gray,
     ArrayDataSource,
     LinearMapper,
 )
@@ -118,46 +119,52 @@
         self._plot = Plot(self._plot_data, default_origin="top left")
         self._plot.padding = (padd, padd, padd, padd)
         # self._quiverplots = []
 
         # -------------------------------------------------------------
 
     def left_clicked_event(self):
+        """ left click event """
         print("left clicked")
         if len(self._x) < 4:
             self._x.append(self._click_tool.x)
             self._y.append(self._click_tool.y)
         print(self._x, self._y)
 
         self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
-        self._plot.overlays.clear()
+        
+        if self._plot.overlays is not None:
+            self._plot.overlays.clear() # type: ignore
         self.plot_num_overlay(self._x, self._y, self.man_ori)
 
     def right_clicked_event(self):
+        """ right click event """
         print("right clicked")
         if len(self._x) > 0:
             self._x.pop()
             self._y.pop()
             print(self._x, self._y)
 
             self.drawcross("coord_x", "coord_y", self._x, self._y, "red", 5)
-            self._plot.overlays.clear()
+            if self._plot.overlays is not None:
+                self._plot.overlays.clear() # type: ignore
             self.plot_num_overlay(self._x, self._y, self.man_ori)
         else:
             if self._right_click_avail:
                 print("deleting point")
                 self.py_rclick_delete(
                     self._click_tool.x, self._click_tool.y, self.cameraN
                 )
                 x = []
                 y = []
                 self.py_get_pix_N(x, y, self.cameraN)
                 self.drawcross("x", "y", x[0], y[0], "blue", 4)
 
     def attach_tools(self):
+        """ Attaches the necessary tools to the plot """
         self._click_tool = ClickerTool(self._img_plot)
         self._click_tool.on_trait_change(
             self.left_clicked_event, "left_changed"
         )
         self._click_tool.on_trait_change(
             self.right_clicked_event, "right_changed"
         )
@@ -617,16 +624,16 @@
             if len(self.camera[i]._x) < 4:
                 print(f"Camera {i} less than 4 points: {self.camera[i]._x}")
                 points_set = False
             else:
                 print(f"Camera {i} has 4 points: {self.camera[i]._x}")
 
         if points_set:
-            print(f'Manual orientation file is {man_ori_path}')
-            with open(self.man_ori_path, "w", encoding="utf-8") as f:
+            print(f'Manual orientation file is {self.man_ori_dat_path}')
+            with open(self.man_ori_dat_path, "w", encoding="utf-8") as f:
                 if f is None:
                     self.status_text = "Error saving man_ori.dat."
                 else:
                     for i in range(self.n_cams):
                         for j in range(4):
                             f.write(
                                 "%f %f\n"
```

### Comparing `pyptv-0.2.3/pyptv/code_editor.py` & `pyptv-0.2.4/pyptv/code_editor.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/detection_gui.py` & `pyptv-0.2.4/pyptv/detection_gui.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/directory_editor.py` & `pyptv-0.2.4/pyptv/directory_editor.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/draw_3d_target.py` & `pyptv-0.2.4/pyptv/draw_3d_target.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/ext_sequence_denis.py` & `pyptv-0.2.4/pyptv/ext_sequence_denis.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/ext_tracker_denis.py` & `pyptv-0.2.4/pyptv/ext_tracker_denis.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/image_inspector.py` & `pyptv-0.2.4/pyptv/image_inspector.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/imageplot.py` & `pyptv-0.2.4/pyptv/imageplot.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/imread_chaco.py` & `pyptv-0.2.4/pyptv/imread_chaco.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/parameter_gui.py` & `pyptv-0.2.4/pyptv/parameter_gui.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/parameters.py` & `pyptv-0.2.4/pyptv/parameters.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/ptv.py` & `pyptv-0.2.4/pyptv/ptv.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/pyptv_batch.py` & `pyptv-0.2.4/pyptv/pyptv_batch.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/pyptv_gui.py` & `pyptv-0.2.4/pyptv/pyptv_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1183,15 +1183,15 @@
                     show_label=False,
                 ),
                 orientation="horizontal",
                 show_left=False,
             ),
             orientation="vertical",
         ),
-        title="pyPTV ver. 0.2.3",
+        title="pyPTV ver. 0.2.4",
         id="main_view",
         width=1.0,
         height=1.0,
         resizable=True,
         handler=TreeMenuHandler(),  # <== Handler class is attached
         menubar=menu_bar,
     )
```

### Comparing `pyptv-0.2.3/pyptv/quiver_demo.py` & `pyptv-0.2.4/pyptv/quiver_demo.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/quiverplot.py` & `pyptv-0.2.4/pyptv/quiverplot.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/scatter_inspector2.py` & `pyptv-0.2.4/pyptv/scatter_inspector2.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv/text_box_overlay.py` & `pyptv-0.2.4/pyptv/text_box_overlay.py`

 * *Files identical despite different names*

### Comparing `pyptv-0.2.3/pyptv.egg-info/SOURCES.txt` & `pyptv-0.2.4/pyptv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

