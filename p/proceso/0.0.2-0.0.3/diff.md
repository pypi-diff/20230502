# Comparing `tmp/proceso-0.0.2.tar.gz` & `tmp/proceso-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proceso-0.0.2.tar", last modified: Mon May  1 13:06:09 2023, max compression
+gzip compressed data, was "proceso-0.0.3.tar", last modified: Tue May  2 01:31:45 2023, max compression
```

## Comparing `proceso-0.0.2.tar` & `proceso-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.219085 proceso-0.0.2/
--rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.2/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     3026 2023-05-01 13:06:09.219133 proceso-0.0.2/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     2386 2023-04-30 21:36:21.000000 proceso-0.0.2/README.md
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.2/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-01 13:06:09.219378 proceso-0.0.2/setup.cfg
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.214849 proceso-0.0.2/src/
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.217652 proceso-0.0.2/src/proceso/
--rw-r--r--   0 nick       (501) staff       (20)    24151 2023-05-01 13:05:56.000000 proceso-0.0.2/src/proceso/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)       30 2023-04-30 21:10:44.000000 proceso-0.0.2/src/proceso/_binding.py
--rw-r--r--   0 nick       (501) staff       (20)      151 2023-04-30 21:10:54.000000 proceso-0.0.2/src/proceso/_setup.py
--rw-r--r--   0 nick       (501) staff       (20)    10191 2023-04-30 21:10:45.000000 proceso-0.0.2/src/proceso/colors.py
--rw-r--r--   0 nick       (501) staff       (20)     5797 2023-05-01 12:51:28.000000 proceso-0.0.2/src/proceso/constants.py
--rw-r--r--   0 nick       (501) staff       (20)     3250 2023-04-30 21:10:47.000000 proceso-0.0.2/src/proceso/data.py
--rw-r--r--   0 nick       (501) staff       (20)     8302 2023-04-30 22:18:10.000000 proceso-0.0.2/src/proceso/dom.py
--rw-r--r--   0 nick       (501) staff       (20)     8041 2023-04-30 21:10:49.000000 proceso-0.0.2/src/proceso/environment.py
--rw-r--r--   0 nick       (501) staff       (20)     1316 2023-04-30 21:10:50.000000 proceso-0.0.2/src/proceso/events.py
--rw-r--r--   0 nick       (501) staff       (20)    12620 2023-04-30 21:10:51.000000 proceso-0.0.2/src/proceso/images.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.218936 proceso-0.0.2/src/proceso/math/
--rw-r--r--   0 nick       (501) staff       (20)      543 2023-04-30 03:13:34.000000 proceso-0.0.2/src/proceso/math/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5281 2023-04-30 21:22:53.000000 proceso-0.0.2/src/proceso/math/calculation.py
--rw-r--r--   0 nick       (501) staff       (20)     3371 2023-04-30 21:22:51.000000 proceso-0.0.2/src/proceso/math/noise.py
--rw-r--r--   0 nick       (501) staff       (20)     1543 2023-04-29 23:47:36.000000 proceso-0.0.2/src/proceso/math/random.py
--rw-r--r--   0 nick       (501) staff       (20)     3428 2023-04-30 21:22:44.000000 proceso-0.0.2/src/proceso/math/trigonometry.py
--rw-r--r--   0 nick       (501) staff       (20)    61234 2023-04-29 22:58:38.000000 proceso-0.0.2/src/proceso/math/vector.py
--rw-r--r--   0 nick       (501) staff       (20)     4857 2023-04-30 21:10:52.000000 proceso-0.0.2/src/proceso/rendering.py
--rw-r--r--   0 nick       (501) staff       (20)    27097 2023-04-30 21:10:55.000000 proceso-0.0.2/src/proceso/shape.py
--rw-r--r--   0 nick       (501) staff       (20)     5609 2023-04-30 21:10:56.000000 proceso-0.0.2/src/proceso/structure.py
--rw-r--r--   0 nick       (501) staff       (20)    13928 2023-05-01 12:39:40.000000 proceso-0.0.2/src/proceso/three_d.py
--rw-r--r--   0 nick       (501) staff       (20)     6642 2023-04-30 21:23:05.000000 proceso-0.0.2/src/proceso/transform.py
--rw-r--r--   0 nick       (501) staff       (20)     5575 2023-04-30 21:10:59.000000 proceso-0.0.2/src/proceso/typography.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.218244 proceso-0.0.2/src/proceso.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     3026 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      762 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:31:45.300490 proceso-0.0.3/
+-rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.3/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     3026 2023-05-02 01:31:45.300534 proceso-0.0.3/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     2386 2023-04-30 21:36:21.000000 proceso-0.0.3/README.md
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.3/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-02 01:31:45.300752 proceso-0.0.3/setup.cfg
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:31:45.296851 proceso-0.0.3/src/
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:31:45.299173 proceso-0.0.3/src/proceso/
+-rw-r--r--   0 nick       (501) staff       (20)    24171 2023-05-02 01:31:32.000000 proceso-0.0.3/src/proceso/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)       30 2023-05-02 00:36:31.000000 proceso-0.0.3/src/proceso/_binding.py
+-rw-r--r--   0 nick       (501) staff       (20)      151 2023-05-02 00:36:38.000000 proceso-0.0.3/src/proceso/_setup.py
+-rw-r--r--   0 nick       (501) staff       (20)    10191 2023-04-30 21:10:45.000000 proceso-0.0.3/src/proceso/colors.py
+-rw-r--r--   0 nick       (501) staff       (20)     5797 2023-05-02 00:36:40.000000 proceso-0.0.3/src/proceso/constants.py
+-rw-r--r--   0 nick       (501) staff       (20)     3250 2023-04-30 21:10:47.000000 proceso-0.0.3/src/proceso/data.py
+-rw-r--r--   0 nick       (501) staff       (20)     8302 2023-04-30 22:18:10.000000 proceso-0.0.3/src/proceso/dom.py
+-rw-r--r--   0 nick       (501) staff       (20)     8041 2023-04-30 21:10:49.000000 proceso-0.0.3/src/proceso/environment.py
+-rw-r--r--   0 nick       (501) staff       (20)     1316 2023-04-30 21:10:50.000000 proceso-0.0.3/src/proceso/events.py
+-rw-r--r--   0 nick       (501) staff       (20)    12718 2023-05-02 01:25:21.000000 proceso-0.0.3/src/proceso/images.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:31:45.300360 proceso-0.0.3/src/proceso/math/
+-rw-r--r--   0 nick       (501) staff       (20)      543 2023-04-30 03:13:34.000000 proceso-0.0.3/src/proceso/math/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     5281 2023-04-30 21:22:53.000000 proceso-0.0.3/src/proceso/math/calculation.py
+-rw-r--r--   0 nick       (501) staff       (20)     3371 2023-04-30 21:22:51.000000 proceso-0.0.3/src/proceso/math/noise.py
+-rw-r--r--   0 nick       (501) staff       (20)     1543 2023-04-29 23:47:36.000000 proceso-0.0.3/src/proceso/math/random.py
+-rw-r--r--   0 nick       (501) staff       (20)     3428 2023-04-30 21:22:44.000000 proceso-0.0.3/src/proceso/math/trigonometry.py
+-rw-r--r--   0 nick       (501) staff       (20)    61234 2023-04-29 22:58:38.000000 proceso-0.0.3/src/proceso/math/vector.py
+-rw-r--r--   0 nick       (501) staff       (20)     5857 2023-05-02 01:25:24.000000 proceso-0.0.3/src/proceso/rendering.py
+-rw-r--r--   0 nick       (501) staff       (20)    27097 2023-04-30 21:10:55.000000 proceso-0.0.3/src/proceso/shape.py
+-rw-r--r--   0 nick       (501) staff       (20)     5609 2023-04-30 21:10:56.000000 proceso-0.0.3/src/proceso/structure.py
+-rw-r--r--   0 nick       (501) staff       (20)    13928 2023-05-01 12:39:40.000000 proceso-0.0.3/src/proceso/three_d.py
+-rw-r--r--   0 nick       (501) staff       (20)     6642 2023-04-30 21:23:05.000000 proceso-0.0.3/src/proceso/transform.py
+-rw-r--r--   0 nick       (501) staff       (20)     5575 2023-04-30 21:10:59.000000 proceso-0.0.3/src/proceso/typography.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:31:45.299698 proceso-0.0.3/src/proceso.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     3026 2023-05-02 01:31:45.000000 proceso-0.0.3/src/proceso.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      762 2023-05-02 01:31:45.000000 proceso-0.0.3/src/proceso.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-02 01:31:45.000000 proceso-0.0.3/src/proceso.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-02 01:31:45.000000 proceso-0.0.3/src/proceso.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-02 01:31:45.000000 proceso-0.0.3/src/proceso.egg-info/top_level.txt
```

### Comparing `proceso-0.0.2/LICENSE` & `proceso-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/PKG-INFO` & `proceso-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proceso
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for creative coding on the web.
 Home-page: https://github.com/nickmcintyre/proceso
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `proceso-0.0.2/README.md` & `proceso-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/setup.cfg` & `proceso-0.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = proceso
-version = 0.0.2
+version = 0.0.3
 author = Nick McIntyre
 author_email = nick@mcintyre.io
 description = A Python package for creative coding on the web.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nickmcintyre/proceso
 project_urls =
```

### Comparing `proceso-0.0.2/src/proceso/__init__.py` & `proceso-0.0.3/src/proceso/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,18 +213,18 @@
     image,
     tint,
     no_tint,
     image_mode,
     # Pixels
     blend,
     copy,
-    filter,
-    get,
+    apply_filter,
+    get_pixels,
     load_pixels,
-    set,
+    set_pixels,
     update_pixels,
 )
 from .math import (
     # Calculation
     abs,
     ceil,
     constrain,
@@ -584,17 +584,17 @@
     The turn_axis variable is only defined within the scope of
     device_turned().
     """,
 ] = _p5js.turnAxis
 # device_moved = _p5js.deviceMoved
 # device_turned = _p5js.deviceTurned
 # device_shaken = _p5js.deviceShaken
-key_is_pressed: Annotated[
+is_key_pressed: Annotated[
     bool,
-    """The boolean system variable key_is_pressed is True if any key is
+    """The boolean system variable is_key_pressed is True if any key is
     pressed and False if no keys are pressed.
     """,
 ] = _p5js.keyIsPressed
 key: Annotated[
     str,
     """The system variable key always contains the value of the most recent
     key on the keyboard that was typed.
@@ -696,17 +696,17 @@
     str,
     """p5 automatically tracks if the mouse button is pressed and which button
     is pressed. The value of the system variable mouse_button is either LEFT,
     RIGHT, or CENTER depending on which button was pressed last. Warning:
     different browsers may track mouse_button differently.
     """,
 ] = _p5js.mouseButton
-mouse_is_pressed: Annotated[
+is_mouse_pressed: Annotated[
     bool,
-    """The boolean system variable mouse_is_pressed is True if the mouse is
+    """The boolean system variable is_mouse_pressed is True if the mouse is
     pressed and False if not.
     """,
 ] = _p5js.mouseIsPressed
 # touch_started = _p5js.touchStarted
 # touch_moved = _p5js.touchMoved
 # touch_ended = _p5js.touchEnded
 touches: Annotated[
@@ -744,18 +744,18 @@
     global frame_count, delta_time, focused, display_width, display_height
     global window_width, window_height, width, height
     # Events
     global device_orientation, acceleration_x, acceleration_y, acceleration_z
     global pacceleration_x, pacceleration_y, pacceleration_z
     global rotation_x, rotation_y, rotation_z
     global protation_x, protation_y, protation_z
-    global turn_axis, key_is_pressed, key, key_code
+    global turn_axis, is_key_pressed, key, key_code
     global moved_x, moved_y, mouse_x, mouse_y, pmouse_x, pmouse_y
     global winmouse_x, winmouse_y, pwinmouse_x, pwinmouse_y
-    global mouse_button, mouse_is_pressed
+    global mouse_button, is_mouse_pressed
     global touches
     global pixels
 
     # Environment
     frame_count = _p5js.frameCount
     delta_time = _p5js.deltaTime
     focused = _p5js.focused
@@ -776,29 +776,29 @@
     rotation_x = _p5js.rotationX
     rotation_y = _p5js.rotationY
     rotation_z = _p5js.rotationZ
     protation_x = _p5js.pRotationX
     protation_y = _p5js.pRotationY
     protation_z = _p5js.pRotationZ
     turn_axis = _p5js.turnAxis
-    key_is_pressed = _p5js.keyIsPressed
+    is_key_pressed = _p5js.keyIsPressed
     key = _p5js.key
     key_code = _p5js.keyCode
     moved_x = _p5js.movedX
     moved_y = _p5js.movedY
     mouse_x = _p5js.mouseX
     mouse_y = _p5js.mouseY
     pmouse_x = _p5js.pmouseX
     pmouse_y = _p5js.pmouseY
     winmouse_x = _p5js.winMouseX
     winmouse_y = _p5js.winMouseY
     pwinmouse_x = _p5js.pwinMouseX
     pwinmouse_y = _p5js.pwinMouseY
     mouse_button = _p5js.mouseButton
-    mouse_is_pressed = _p5js.mouseIsPressed
+    is_mouse_pressed = _p5js.mouseIsPressed
     touches = _p5js.touches
     pixels = _p5js.pixels
 
 
 def run(
     preload: Callable | None = None,
     setup: Callable | None = None,
```

### Comparing `proceso-0.0.2/src/proceso/colors.py` & `proceso-0.0.3/src/proceso/colors.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/constants.py` & `proceso-0.0.3/src/proceso/constants.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/data.py` & `proceso-0.0.3/src/proceso/data.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/dom.py` & `proceso-0.0.3/src/proceso/dom.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/environment.py` & `proceso-0.0.3/src/proceso/environment.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/events.py` & `proceso-0.0.3/src/proceso/events.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/images.py` & `proceso-0.0.3/src/proceso/images.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     buffer with the width and height parameters.
 
     .pixels gives access to a list containing the values for all the pixels
     in the display window. These values are numbers. This list is the size
     (including an appropriate factor for the pixel_density) of the display
     window x4, representing the R, G, B, A values in order for each pixel,
     moving from left to right across each row, then down each column. See
-    .pixels for more info. It may also be simpler to use set() or get().
+    .pixels for more info. It may also be simpler to use set_pixels() or get_pixels().
 
     Before accessing the pixels of an image, the data must loaded with the
     load_pixels() function. After the list data has been modified, the
     update_pixels() function must be run to update the changes.
     """
     return _p5js.createImage(width, height)
 
@@ -201,15 +201,15 @@
     sy: int,
     sw: int,
     sh: int,
     dx: int,
     dy: int,
     dw: int,
     dh: int,
-    blend_mode: str
+    blend_mode: str,
 ):
     """Copies a region of pixels from one image to another, using a specified
     blend mode to do the operation.
     """
     _p5js.blend(src_image, sx, sy, sw, sh, dx, dy, dw, dh, blend_mode)
 
 
@@ -229,15 +229,15 @@
     the canvas src_image is specified this is used as the source.
     If the source and destination regions aren't the same size, it will
     automatically resize source pixels to fit the specified target region.
     """
     _p5js.copy(src_image, sx, sy, sw, sh, dx, dy, dw, dh)
 
 
-def filter(filter_type: str, filter_param: float | None = None):
+def apply_filter(filter_type: str, filter_param: float | None = None):
     """Applies a filter to the canvas.
     The presets options are:
 
     THRESHOLD Converts the image to black and white pixels depending if they
     are above or below the threshold defined by the level parameter. The
     parameter must be between 0.0 (black) and 1.0 (white). If no level is
     specified, 0.5 is used.
@@ -257,71 +257,73 @@
     extent of the blurring. If no parameter is used, the blur is equivalent to
     Gaussian blur of radius 1. Larger values increase the blur.
 
     ERODE Reduces the light areas. No parameter is used.
 
     DILATE Increases the light areas. No parameter is used.
 
-    filter() does not work in WEBGL mode. A similar effect can be achieved in
+    apply_filter() does not work in WEBGL mode. A similar effect can be achieved in
     WEBGL mode using custom shaders. Adam Ferriss has written a selection of
     shader examples that contains many of the effects present in the filter
     examples.
     """
     _p5js.filter(filter_type, filter_param)
 
 
-def get(x: int, y: int, width: int | None = None, height: int | None = None) -> list[float] | object:
+def get_pixels(
+    x: int, y: int, width: int | None = None, height: int | None = None
+) -> list[float] | object:
     """Get a region of pixels, or a single pixel, from the canvas.
 
     Returns a list of [R,G,B,A] values for any pixel or grabs a section of
     an image. If no parameters are specified, the entire image is returned.
     Use the x and y parameters to get the value of one pixel. Get a section of
     the display window by specifying additional w and h parameters. When
     getting an image, the x and y parameters define the coordinates for the
     upper-left corner of the image, regardless of the current image_mode().
 
-    Getting the color of a single pixel with get(x, y) is easy, but not as
+    Getting the color of a single pixel with get_pixels(x, y) is easy, but not as
     fast as grabbing the data directly from pixels[].
     """
     return _p5js.get(x, y, width, height)
 
 
 def load_pixels():
     """Loads the pixel data for the display window into the pixels[] list.
     This function must always be called before reading from or writing to
-    pixels[]. Note that only changes made with set() or direct manipulation of
+    pixels[]. Note that only changes made with set_pixels() or direct manipulation of
     pixels[] will occur.
     """
     _p5js.loadPixels()
 
 
-def set(x: int, y: int, c: float | list[float] | object):
+def set_pixels(x: int, y: int, c: float | list[float] | object):
     """Changes the color of any pixel, or writes an image directly to the
     display window.
     The x and y parameters specify the pixel to change and the c parameter
     specifies the color value. This can be a p5.Color object, or [R, G, B, A]
     pixel list. It can also be a single grayscale value. When setting an
     image, the x and y parameters define the coordinates for the upper-left
     corner of the image, regardless of the current imageMode().
 
-    After using set(), you must call updatePixels() for your changes to
+    After using set_pixels(), you must call update_pixels() for your changes to
     appear. This should be called once all pixels have been set, and must be
-    called before calling .get() or drawing the image.
+    called before calling get_pixels() or drawing the image.
 
-    Setting the color of a single pixel with set(x, y) is easy, but not as
+    Setting the color of a single pixel with set_pixels(x, y) is easy, but not as
     fast as putting the data directly into pixels[]. Setting the pixels[]
     values directly may be complicated when working with a retina display, but
     will perform better when lots of pixels need to be set directly on every
     loop. See the reference for pixels[] for more information.
     """
     _p5js.set(x, y, c)
 
 
 def update_pixels():
     """Updates the display window with the data in the pixels[] list.
     Use in conjunction with loadPixels(). If you're only reading pixels from
-    the list, there's no need to call updatePixels() — updating is only
-    necessary to apply changes. updatePixels() should be called anytime the
-    pixels list is manipulated or set() is called, and only changes made with
-    set() or direct changes to pixels[] will occur.
+    the list, there's no need to call update_pixels() — updating is only
+    necessary to apply changes. update_pixels() should be called anytime the
+    pixels list is manipulated or set_pixels() is called, and only changes made with
+    set_pixels() or direct changes to pixels[] will occur.
     """
     _p5js.updatePixels()
```

### Comparing `proceso-0.0.2/src/proceso/math/__init__.py` & `proceso-0.0.3/src/proceso/math/__init__.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/math/calculation.py` & `proceso-0.0.3/src/proceso/math/calculation.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/math/noise.py` & `proceso-0.0.3/src/proceso/math/noise.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/math/random.py` & `proceso-0.0.3/src/proceso/math/random.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/math/trigonometry.py` & `proceso-0.0.3/src/proceso/math/trigonometry.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/math/vector.py` & `proceso-0.0.3/src/proceso/math/vector.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/rendering.py` & `proceso-0.0.3/src/proceso/rendering.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def create_canvas(width: int, height: int, renderer: str = P2D) -> object:
     """Creates a canvas element in the document and sets its dimensions in
     pixels.
 
     This method should be called only once at the start of setup(). Calling
-    create_canvas more than once in a sketch will result in very unpredictable
+    create_canvas() more than once in a sketch will result in very unpredictable
     behavior. If you want more than one drawing canvas you could use
     create_graphics() (hidden by default but it can be shown).
 
     Important note: in 2D mode (i.e. when p5.Renderer is not set) the origin
     (0,0) is positioned at the top left of the screen. In 3D mode (i.e. when
     p5.Renderer is set to WEBGL), the origin is positioned at the center of
     the canvas. See this issue for more information.
@@ -21,14 +21,36 @@
     The system variables width and height are set by the parameters passed to
     this function. If create_canvas() is not used, the window will be given a
     default size of 100×100 pixels.
     """
     return _p5js.createCanvas(width, height, renderer)
 
 
+def size(width: int, height: int, renderer: str = P2D) -> object:
+    """Alias of create_canvas().
+    Creates a canvas element in the document and sets its dimensions in
+    pixels.
+
+    This method should be called only once at the start of setup(). Calling
+    size() more than once in a sketch will result in very unpredictable
+    behavior. If you want more than one drawing canvas you could use
+    create_graphics() (hidden by default but it can be shown).
+
+    Important note: in 2D mode (i.e. when p5.Renderer is not set) the origin
+    (0,0) is positioned at the top left of the screen. In 3D mode (i.e. when
+    p5.Renderer is set to WEBGL), the origin is positioned at the center of
+    the canvas. See this issue for more information.
+
+    The system variables width and height are set by the parameters passed to
+    this function. If size() is not used, the window will be given a
+    default size of 100×100 pixels.
+    """
+    return _p5js.createCanvas(width, height, renderer)
+
+
 def resize_canvas(width: int, height: int, no_redraw: bool | None = None):
     """Resizes the canvas to given width and height.
     The canvas will be cleared and draw will be called immediately, allowing
     the sketch to re-render itself in the resized canvas.
     """
     _p5js.resizeCanvas(width, height, no_redraw)
```

### Comparing `proceso-0.0.2/src/proceso/shape.py` & `proceso-0.0.3/src/proceso/shape.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/structure.py` & `proceso-0.0.3/src/proceso/structure.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/three_d.py` & `proceso-0.0.3/src/proceso/three_d.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/transform.py` & `proceso-0.0.3/src/proceso/transform.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso/typography.py` & `proceso-0.0.3/src/proceso/typography.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.2/src/proceso.egg-info/PKG-INFO` & `proceso-0.0.3/src/proceso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proceso
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for creative coding on the web.
 Home-page: https://github.com/nickmcintyre/proceso
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `proceso-0.0.2/src/proceso.egg-info/SOURCES.txt` & `proceso-0.0.3/src/proceso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

