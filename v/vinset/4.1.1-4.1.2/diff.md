# Comparing `tmp/vinset-4.1.1.tar.gz` & `tmp/vinset-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinset-4.1.1.tar", last modified: Fri Apr 28 20:52:00 2023, max compression
+gzip compressed data, was "vinset-4.1.2.tar", last modified: Mon May  1 23:34:28 2023, max compression
```

## Comparing `vinset-4.1.1.tar` & `vinset-4.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 20:52:00.213810 vinset-4.1.1/
--rw-rw-rw-   0        0        0    11558 2023-02-15 23:27:28.000000 vinset-4.1.1/LICENSE
--rw-rw-rw-   0        0        0      581 2023-04-28 20:52:00.213810 vinset-4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9583 2023-04-27 05:44:25.000000 vinset-4.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 20:52:00.213810 vinset-4.1.1/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-04-28 20:42:21.000000 vinset-4.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 20:52:00.202888 vinset-4.1.1/vinset/
--rw-rw-rw-   0        0        0        0 2023-02-15 23:27:29.000000 vinset-4.1.1/vinset/__init__.py
--rw-rw-rw-   0        0        0    59855 2023-04-28 20:51:06.000000 vinset-4.1.1/vinset/vin.py
-drwxrwxrwx   0        0        0        0 2023-04-28 20:52:00.212813 vinset-4.1.1/vinset.egg-info/
--rw-rw-rw-   0        0        0      581 2023-04-28 20:52:00.000000 vinset-4.1.1/vinset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-28 20:52:00.000000 vinset-4.1.1/vinset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 20:52:00.000000 vinset-4.1.1/vinset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-28 20:52:00.000000 vinset-4.1.1/vinset.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-28 20:51:50.000000 vinset-4.1.1/vinset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-04-28 20:52:00.000000 vinset-4.1.1/vinset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 20:52:00.000000 vinset-4.1.1/vinset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 23:34:28.652453 vinset-4.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-02-15 23:27:28.000000 vinset-4.1.2/LICENSE
+-rw-rw-rw-   0        0        0      581 2023-05-01 23:34:28.652453 vinset-4.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9522 2023-04-28 22:47:57.000000 vinset-4.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 23:34:28.652453 vinset-4.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-05-01 23:34:16.000000 vinset-4.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:34:28.641482 vinset-4.1.2/vinset/
+-rw-rw-rw-   0        0        0        0 2023-02-15 23:27:29.000000 vinset-4.1.2/vinset/__init__.py
+-rw-rw-rw-   0        0        0    62469 2023-05-01 23:34:16.000000 vinset-4.1.2/vinset/vin.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:34:28.651455 vinset-4.1.2/vinset.egg-info/
+-rw-rw-rw-   0        0        0      581 2023-05-01 23:34:28.000000 vinset-4.1.2/vinset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-01 23:34:28.000000 vinset-4.1.2/vinset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 23:34:28.000000 vinset-4.1.2/vinset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-01 23:34:28.000000 vinset-4.1.2/vinset.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 23:34:19.000000 vinset-4.1.2/vinset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-05-01 23:34:28.000000 vinset-4.1.2/vinset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 23:34:28.000000 vinset-4.1.2/vinset.egg-info/top_level.txt
```

### Comparing `vinset-4.1.1/LICENSE` & `vinset-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vinset-4.1.1/PKG-INFO` & `vinset-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.1.1
+Version: 4.1.2
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
 Platform: UNKNOWN
```

### Comparing `vinset-4.1.1/README.md` & `vinset-4.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ```
 _________________________________
 # User guide
 There are 2 types of vinset image overlay in version 4.0.0 and above which are  
 1.  graph overlay  
 2.  text overlay  
 ```
-vinset -i input.mp4 [-d gaze.csv] -o output.mp4 -c config.json [-t graph or text]
+vinset -i input.mp4 [-d gaze.csv] -o output.mp4 -c config.json [-t graph or text] [-tl timeline.json]
 ```
 The argument -d is mandatory in graph overlay and does not require in text overlay.
 ## Graph Overlay Example usage
 ```
 vinset -i input_video.mp4 -o output_video.mp4 -d gaze.csv -c config.json 
 ```
 (or)  
@@ -183,23 +183,22 @@
 
 #### Note: 
 1.  Color information can be tuple string eg. "(0,0,255)" or 6 hex color code eg. "#ffffff" or basic color strings which are "red", "green", "blue", "yellow", "black", "white" and "magenta".
 2.  Zero line will be displayed if it is enabled and it is actually can be drawn according to the lower limit and upper limit. eg. If lower limit is 1 and upper limit is 2, zero line cannot be drawn.  
 
 ## Text Overlay Example usage  
 ```
-vinset -t text -i input_video.mp4 -o output_video.mp4 -c config.json 
+vinset -t text -i input_video.mp4 -o output_video.mp4 -c config.json -tl timeline.json
 ```
-The argument -t is mandatory in text overlay  
+The argument -t and -tl are mandatory in text overlay.  
 
 ### Example configuration file for text overlay
 #### logmar_level_right_bottom.json  
 ```
 { "display": "True",
-  "timeline_file_name": "timeline.json",
   "text_info": {
     "text_marker": "event_marker",
     "text_marker_location": "event->event->logmar_level",
     "text_color": "green",
     "text_font_size":  0.7,
     "text_thickness": 2,
     "time_marker": "timestamp",
@@ -211,16 +210,14 @@
   "va_text_display_location": {"x": 550, "y": 530}
 }
 ```
 ### Configuration format explanation for text overlay
 
 #### display = video will be displayed during producing video if it is true.
 
-#### timeline_file_name = directory location of timeline.json.
-
 #### text_info = the information of text.
 
 1.  text_marker = the name of event marker to be captured in timeline.json file.
 2.  text_marker_location = the directory indicator string of where text marker is located in timeline.json.
 3.  text_color = the color of text.
 4.  text_font_size = the font size of text.
 5.  text_thickness = the pixel thickness of the text.
```

### Comparing `vinset-4.1.1/setup.py` & `vinset-4.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw the graph from video and csv files.'
 
 setup(
     name='vinset',
-    version='4.1.1',
+    version='4.1.2',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/vinset',
     description='gaze visualisation program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

### Comparing `vinset-4.1.1/vinset/vin.py` & `vinset-4.1.2/vinset/vin.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     # width = height and height = width when we rotate the image
     f_w = frame_height_input
     f_h = frame_width_input
     tem_image = np.zeros([int(f_w), int(f_h), 3], dtype=np.uint8)
     x_edit = int(frame_height_input - y_input)
     y_edit = x_input
     co_ord_input = (x_edit, y_edit)
-    # draw
+
     cv2.putText(tem_image, put_text_input, co_ord_input, cv2.FONT_HERSHEY_SIMPLEX, font_input,
                 color_search_input, thick_input)
     # rotate
     out_image = cv2.rotate(tem_image, cv2.ROTATE_90_COUNTERCLOCKWISE)
     # capture position to return
     color_index_output = np.where(np.all(out_image == color_search_input, axis=-1))
 
@@ -497,15 +497,15 @@
                 for i in range(0, t_w):
                     space_value = i * x_scale_interval_width
                     # end_point_x_scale_level = start_point_x_scale - height_of_scale
                     cv2.line(raw_image, (axes_pos_x + space_value,
                                          axes_pos_h + axes_pos_y),
                              (axes_pos_x + space_value,
                               axes_pos_h + axes_pos_y - height_of_scale),
-                             box_color, box_thickness)
+                             box_color, box_thickness, cv2.LINE_AA)
                 # after this points, the raw black image is filled with
                 # all graphs and labels
 
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         v_writer = cv2.VideoWriter(output_video_file, fourcc, int(frame_rate), (int(frame_width), int(frame_height)))
         whole_t = time.time()
         count = 0
@@ -532,15 +532,15 @@
                         h = axes_pos["height"]
                         axes_bg = axes_info["background"]
                         bg_fill = axes_bg["fill"]
                         color_input = change_string_to_color_tuple(bg_fill)
                         bg_opacity = axes_bg["opacity"]
                         # copy a frame to draw boundary
                         overlay_frame = frame.copy()
-                        boundary_space = 50
+                        boundary_space = axes_bg["space"]
                         # draw boundary to graph
                         cv2.rectangle(overlay_frame,
                                       (x - boundary_space, y - boundary_space),
                                       (x + w + boundary_space,
                                        y + h + boundary_space),
                                       color_input, -1)
                         # overlay by original frame
@@ -633,15 +633,15 @@
                             pointer_position_info_name = info_name + "_pointer_info"
 
                             if len(final_display_arr) > 0:
                                 for ind, num in enumerate(final_display_arr):
                                     if zero_display:
                                         cv2.line(clone_frame, (zero_line_start_x, zero_line_y),
                                                  (zero_line_end_x, zero_line_y),
-                                                 line_color, zero_line_thick)
+                                                 line_color, zero_line_thick, cv2.LINE_AA)
                                     if type(num[1]) == str:
                                         if ind == 0:
                                             no_first_value = True
 
                                     elif math.isnan(num[1]):
                                         value_to_draw = False
 
@@ -718,15 +718,15 @@
                             pointer_position_info_name = info_name + "_pointer_info"
 
                             if len(final_display_arr) > 0:
                                 for ind, num in enumerate(final_display_arr):
                                     if zero_display:
                                         cv2.line(clone_frame, (zero_line_start_x, zero_line_y),
                                                  (zero_line_end_x, zero_line_y),
-                                                 line_color, zero_line_thick)
+                                                 line_color, zero_line_thick, cv2.LINE_AA)
                                     if type(num[1]) == str:
                                         pass
 
                                     elif math.isnan(num[1]):
                                         value_to_draw = False
 
                                     else:
@@ -802,26 +802,37 @@
         input_video.release()
         v_writer.release()
         cv2.destroyAllWindows()
 
 
 def overlay_text(draw_able_input, config_info_input, input_video_file, output_video_file, timeline_file):
     text_info = config_info_input["text_info"]
-    text_font_size = text_info["text_font_size"]
-    text_color = text_info["text_color"]
-    text_color_tuple = change_string_to_color_tuple(text_color)
-    text_thickness = text_info["text_thickness"]
+    va_text_color = text_info["va_text_color"]
+    va_text_font_size = text_info["va_text_font_size"]
+    va_text_color_tuple = change_string_to_color_tuple(va_text_color)
+    va_text_thickness = text_info["va_text_thickness"]
+    stimulus_text_color = text_info["stimulus_text_color"]
+    stimulus_text_font_size = text_info["stimulus_text_font_size"]
+    stimulus_text_color_tuple = change_string_to_color_tuple(stimulus_text_color)
+    stimulus_text_thickness = text_info["stimulus_text_thickness"]
     timeline_info = None
     stimulus_text_display_location = config_info_input["stimulus_text_display_location"]
     va_text_display_location = config_info_input["va_text_display_location"]
     sti_x_position = stimulus_text_display_location["x"]
     sti_y_position = stimulus_text_display_location["y"]
     va_x_position = va_text_display_location["x"]
     va_y_position = va_text_display_location["y"]
     minimum_va_decimal = text_info["minimum_va_decimal"]
+    extra_draw = config_info_input["base_draw"]
+    if extra_draw:
+        extra_draw_names = config_info_input["base_draw_names"]
+        extra_draw_info = config_info_input["base_draw_info"]
+    else:
+        extra_draw_names = None
+        extra_draw_info = None
 
     try:
         f = open(timeline_file)
         timeline_info = json.load(f)
         print(f"{timeline_file} is loaded successfully by json.")
         # print(timeline_info)
     except ValueError:
@@ -868,31 +879,58 @@
             # start_tt = time.time()
             ret, frame = input_video.read()
             # end_tt = time.time()
             print_percent_done(count, frame_count)
             check_timer = frame_count_to_time(count, frame_rate)
 
             if ret:
+                if extra_draw_names and extra_draw_info:
+                    for name in extra_draw_names:
+                        info = get_extra_draw_info(name, extra_draw_info)
+                        if info:
+                            info_type = info["info_type"]
+                            info_details = info["info_details"]
+                            if info_type == "box":
+                                boundary_space = info_details["boundary_space"]
+                                x = info_details["x"]
+                                y = info_details["y"]
+                                w = info_details["w"]
+                                h = info_details["h"]
+                                color = info_details["color"]
+                                opacity = info_details["opacity"]
+                                color_input = change_string_to_color_tuple(color)
+                                # copy a frame to draw boundary
+                                overlay_frame = frame.copy()
+                                # draw boundary to graph
+                                cv2.rectangle(overlay_frame,
+                                              (x - boundary_space, y - boundary_space),
+                                              (x + w + boundary_space,
+                                               y + h + boundary_space),
+                                              color_input, -1)
+                                # overlay by original frame
+                                frame = cv2.addWeighted(overlay_frame, opacity,
+                                                        frame, 1 - opacity, 0)
+
                 if stimulus_index < final_stimulus_level_array_length:
                     stimulus_timestamp_to_check = final_stimulus_level_array[stimulus_index]["timestamp"] * 1000
                     if check_timer >= stimulus_timestamp_to_check:
                         start_drawing = True
                         stimulus_display_text = str(final_stimulus_level_array[stimulus_index]["logmar"])
                         sweep_order = final_stimulus_level_array[stimulus_index]["sweep_order"]
                         stimulus_index += 1
 
                 if start_drawing:
                     nearest_stimulus_text = get_nearest_stimulus(stimulus_display_text)
-                    cv2.putText(frame, f"Stimulus Level:{str(nearest_stimulus_text)}", (sti_x_position, sti_y_position),
-                                cv2.FONT_HERSHEY_SIMPLEX, text_font_size,
-                                text_color_tuple, text_thickness)
+                    cv2.putText(frame, f"showing {str(nearest_stimulus_text)} logMAR", (sti_x_position, sti_y_position),
+                                cv2.FONT_HERSHEY_TRIPLEX, stimulus_text_font_size,
+                                stimulus_text_color_tuple, stimulus_text_thickness, cv2.LINE_AA)
                     va_display_text = get_va_from_stimulus(str(stimulus_display_text), sweep_order, minimum_va_decimal)
-                    cv2.putText(frame, f"VA       Level:{str(va_display_text)}", (va_x_position, va_y_position),
-                                cv2.FONT_HERSHEY_SIMPLEX, text_font_size,
-                                text_color_tuple, text_thickness)
+                    cv2.putText(frame, f"{str(va_display_text)} logMAR", (va_x_position, va_y_position),
+                                cv2.FONT_HERSHEY_TRIPLEX, va_text_font_size,
+                                va_text_color_tuple, va_text_thickness, cv2.LINE_AA)
                     if sweep_order == "resting":
                         start_drawing = False
 
                 if display_able:
                     cv2.imshow("Frame", frame)
                     # cv2.imshow("F", clone_frame)
                     # vsr_t = time.time()
@@ -1066,17 +1104,27 @@
         if float(string_input) == 0:
             string_input = "0.0"
         if float(string_input) < stimulus_value:
             string_input = str(round(float(string_input) + 0.1, 1))
     return string_input
 
 
+def get_extra_draw_info(name_input, info_array_input):
+    draw_info = None
+    for info in info_array_input:
+        info_name = info["info_name"]
+        if info_name == name_input:
+            draw_info = info
+            break
+    return draw_info
+
+
 def main():
     parser = argparse.ArgumentParser(prog='vinset', description='VINSET package.')
-    parser.add_argument('--version', action='version', version='4.1.1'),
+    parser.add_argument('--version', action='version', version='4.1.2'),
     parser.add_argument("-i", dest="input_filename", required=True, type=argparse.FileType('r'), default=sys.stdin,
                         help="input mp4 file", metavar="input.mp4")
     parser.add_argument("-d", dest="input_data_filename", required=False, type=argparse.FileType('r'),
                         default=sys.stdin,
                         help="input csv data file", metavar="data.csv")
     parser.add_argument("-o", dest="output_filename", required=True, type=argparse.FileType('w'), default=sys.stdout,
                         help="output mp4 file", metavar="output.mp4")
```

### Comparing `vinset-4.1.1/vinset.egg-info/PKG-INFO` & `vinset-4.1.2/vinset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinset
-Version: 4.1.1
+Version: 4.1.2
 Summary: gaze visualisation program
 Home-page: https://github.com/jtur044/vinset
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: gaze visualisation program vinset
 Platform: UNKNOWN
```

