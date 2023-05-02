# Comparing `tmp/proceso-0.0.4.tar.gz` & `tmp/proceso-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proceso-0.0.4.tar", last modified: Tue May  2 01:51:59 2023, max compression
+gzip compressed data, was "proceso-0.0.6.tar", last modified: Tue May  2 19:46:34 2023, max compression
```

## Comparing `proceso-0.0.4.tar` & `proceso-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:51:59.178625 proceso-0.0.4/
--rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.4/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     3060 2023-05-02 01:51:59.178671 proceso-0.0.4/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     2420 2023-05-02 01:51:45.000000 proceso-0.0.4/README.md
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.4/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-02 01:51:59.178887 proceso-0.0.4/setup.cfg
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:51:59.174850 proceso-0.0.4/src/
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:51:59.177247 proceso-0.0.4/src/proceso/
--rw-r--r--   0 nick       (501) staff       (20)    24171 2023-05-02 01:31:32.000000 proceso-0.0.4/src/proceso/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)       30 2023-05-02 00:36:31.000000 proceso-0.0.4/src/proceso/_binding.py
--rw-r--r--   0 nick       (501) staff       (20)      151 2023-05-02 00:36:38.000000 proceso-0.0.4/src/proceso/_setup.py
--rw-r--r--   0 nick       (501) staff       (20)    10191 2023-04-30 21:10:45.000000 proceso-0.0.4/src/proceso/colors.py
--rw-r--r--   0 nick       (501) staff       (20)     5797 2023-05-02 00:36:40.000000 proceso-0.0.4/src/proceso/constants.py
--rw-r--r--   0 nick       (501) staff       (20)     3250 2023-04-30 21:10:47.000000 proceso-0.0.4/src/proceso/data.py
--rw-r--r--   0 nick       (501) staff       (20)     8302 2023-04-30 22:18:10.000000 proceso-0.0.4/src/proceso/dom.py
--rw-r--r--   0 nick       (501) staff       (20)     8041 2023-04-30 21:10:49.000000 proceso-0.0.4/src/proceso/environment.py
--rw-r--r--   0 nick       (501) staff       (20)     1316 2023-04-30 21:10:50.000000 proceso-0.0.4/src/proceso/events.py
--rw-r--r--   0 nick       (501) staff       (20)    12718 2023-05-02 01:25:21.000000 proceso-0.0.4/src/proceso/images.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:51:59.178490 proceso-0.0.4/src/proceso/math/
--rw-r--r--   0 nick       (501) staff       (20)      543 2023-04-30 03:13:34.000000 proceso-0.0.4/src/proceso/math/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5281 2023-04-30 21:22:53.000000 proceso-0.0.4/src/proceso/math/calculation.py
--rw-r--r--   0 nick       (501) staff       (20)     3371 2023-04-30 21:22:51.000000 proceso-0.0.4/src/proceso/math/noise.py
--rw-r--r--   0 nick       (501) staff       (20)     1543 2023-04-29 23:47:36.000000 proceso-0.0.4/src/proceso/math/random.py
--rw-r--r--   0 nick       (501) staff       (20)     3428 2023-04-30 21:22:44.000000 proceso-0.0.4/src/proceso/math/trigonometry.py
--rw-r--r--   0 nick       (501) staff       (20)    61234 2023-04-29 22:58:38.000000 proceso-0.0.4/src/proceso/math/vector.py
--rw-r--r--   0 nick       (501) staff       (20)     5870 2023-05-02 01:39:49.000000 proceso-0.0.4/src/proceso/rendering.py
--rw-r--r--   0 nick       (501) staff       (20)    27097 2023-04-30 21:10:55.000000 proceso-0.0.4/src/proceso/shape.py
--rw-r--r--   0 nick       (501) staff       (20)     5609 2023-04-30 21:10:56.000000 proceso-0.0.4/src/proceso/structure.py
--rw-r--r--   0 nick       (501) staff       (20)    13928 2023-05-01 12:39:40.000000 proceso-0.0.4/src/proceso/three_d.py
--rw-r--r--   0 nick       (501) staff       (20)     6642 2023-04-30 21:23:05.000000 proceso-0.0.4/src/proceso/transform.py
--rw-r--r--   0 nick       (501) staff       (20)     5575 2023-04-30 21:10:59.000000 proceso-0.0.4/src/proceso/typography.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 01:51:59.177878 proceso-0.0.4/src/proceso.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     3060 2023-05-02 01:51:59.000000 proceso-0.0.4/src/proceso.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      762 2023-05-02 01:51:59.000000 proceso-0.0.4/src/proceso.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-02 01:51:59.000000 proceso-0.0.4/src/proceso.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-02 01:51:59.000000 proceso-0.0.4/src/proceso.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-02 01:51:59.000000 proceso-0.0.4/src/proceso.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.201693 proceso-0.0.6/
+-rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.6/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     3089 2023-05-02 19:46:34.201741 proceso-0.0.6/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     2449 2023-05-02 18:05:23.000000 proceso-0.0.6/README.md
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.6/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-02 19:46:34.201966 proceso-0.0.6/setup.cfg
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.197129 proceso-0.0.6/src/
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.200043 proceso-0.0.6/src/proceso/
+-rw-r--r--   0 nick       (501) staff       (20)     3787 2023-05-02 18:03:17.000000 proceso-0.0.6/src/proceso/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      341 2023-05-02 18:03:20.000000 proceso-0.0.6/src/proceso/_binding.py
+-rw-r--r--   0 nick       (501) staff       (20)    11523 2023-05-02 18:03:22.000000 proceso-0.0.6/src/proceso/colors.py
+-rw-r--r--   0 nick       (501) staff       (20)     9800 2023-05-02 18:03:25.000000 proceso-0.0.6/src/proceso/constants.py
+-rw-r--r--   0 nick       (501) staff       (20)     3563 2023-05-02 18:03:27.000000 proceso-0.0.6/src/proceso/data.py
+-rw-r--r--   0 nick       (501) staff       (20)     9197 2023-05-02 18:03:30.000000 proceso-0.0.6/src/proceso/dom.py
+-rw-r--r--   0 nick       (501) staff       (20)     8773 2023-05-02 18:03:32.000000 proceso-0.0.6/src/proceso/environment.py
+-rw-r--r--   0 nick       (501) staff       (20)     1516 2023-05-02 18:03:35.000000 proceso-0.0.6/src/proceso/events.py
+-rw-r--r--   0 nick       (501) staff       (20)    14015 2023-05-02 18:03:38.000000 proceso-0.0.6/src/proceso/images.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.201250 proceso-0.0.6/src/proceso/math/
+-rw-r--r--   0 nick       (501) staff       (20)      271 2023-05-02 16:58:34.000000 proceso-0.0.6/src/proceso/math/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     5959 2023-05-02 16:55:18.000000 proceso-0.0.6/src/proceso/math/calculation.py
+-rw-r--r--   0 nick       (501) staff       (20)     3644 2023-05-02 16:55:50.000000 proceso-0.0.6/src/proceso/math/noise.py
+-rw-r--r--   0 nick       (501) staff       (20)     1711 2023-05-02 16:57:42.000000 proceso-0.0.6/src/proceso/math/random.py
+-rw-r--r--   0 nick       (501) staff       (20)     3871 2023-05-02 16:56:53.000000 proceso-0.0.6/src/proceso/math/trigonometry.py
+-rw-r--r--   0 nick       (501) staff       (20)    61205 2023-05-02 18:29:09.000000 proceso-0.0.6/src/proceso/math/vector.py
+-rw-r--r--   0 nick       (501) staff       (20)     6462 2023-05-02 18:03:40.000000 proceso-0.0.6/src/proceso/rendering.py
+-rw-r--r--   0 nick       (501) staff       (20)    29994 2023-05-02 18:03:43.000000 proceso-0.0.6/src/proceso/shape.py
+-rw-r--r--   0 nick       (501) staff       (20)     6114 2023-05-02 18:03:46.000000 proceso-0.0.6/src/proceso/structure.py
+-rw-r--r--   0 nick       (501) staff       (20)    16233 2023-05-02 18:03:48.000000 proceso-0.0.6/src/proceso/sysvars.py
+-rw-r--r--   0 nick       (501) staff       (20)    15708 2023-05-02 18:03:51.000000 proceso-0.0.6/src/proceso/three_d.py
+-rw-r--r--   0 nick       (501) staff       (20)     7325 2023-05-02 18:03:55.000000 proceso-0.0.6/src/proceso/transform.py
+-rw-r--r--   0 nick       (501) staff       (20)     6198 2023-05-02 18:03:57.000000 proceso-0.0.6/src/proceso/typography.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.200628 proceso-0.0.6/src/proceso.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     3089 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      763 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/top_level.txt
```

### Comparing `proceso-0.0.4/LICENSE` & `proceso-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `proceso-0.0.4/PKG-INFO` & `proceso-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proceso
-Version: 0.0.4
+Version: 0.0.6
 Summary: A Python package for creative coding on the web.
 Home-page: https://github.com/nickmcintyre/proceso
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -43,15 +43,18 @@
     <py-script src="sketch.py"></py-script>
 </body>
 
 </html>
 ```
 
 ```python
-import proceso as p5
+from proceso import Sketch
+
+
+p5 = Sketch()
 
 
 pos = p5.Vector(200, 200)
 vel = p5.Vector.random(2)
 r = 25
 
 
@@ -73,15 +76,15 @@
     if pos.y < r or pos.y > p5.height - r:
         vel.y *= -1
 
     if p5.is_mouse_pressed == True:
         p5.background("dodgerblue")
 
 
-p5.run(setup=setup, draw=draw)
+p5.run_sketch(setup=setup, draw=draw)
 ```
 
 # Roadmap
 - Improve documentation
 - Fix known bugs
 - Finish API
 - Support JupyterLite
```

### Comparing `proceso-0.0.4/README.md` & `proceso-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     <py-script src="sketch.py"></py-script>
 </body>
 
 </html>
 ```
 
 ```python
-import proceso as p5
+from proceso import Sketch
+
+
+p5 = Sketch()
 
 
 pos = p5.Vector(200, 200)
 vel = p5.Vector.random(2)
 r = 25
 
 
@@ -56,15 +59,15 @@
     if pos.y < r or pos.y > p5.height - r:
         vel.y *= -1
 
     if p5.is_mouse_pressed == True:
         p5.background("dodgerblue")
 
 
-p5.run(setup=setup, draw=draw)
+p5.run_sketch(setup=setup, draw=draw)
 ```
 
 # Roadmap
 - Improve documentation
 - Fix known bugs
 - Finish API
 - Support JupyterLite
```

### Comparing `proceso-0.0.4/setup.cfg` & `proceso-0.0.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = proceso
-version = 0.0.4
+version = 0.0.6
 author = Nick McIntyre
 author_email = nick@mcintyre.io
 description = A Python package for creative coding on the web.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nickmcintyre/proceso
 project_urls =
```

### Comparing `proceso-0.0.4/src/proceso/colors.py` & `proceso-0.0.6/src/proceso/colors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,289 +1,278 @@
+from typing import Any
 from pyodide.ffi import to_js
 
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-# ==================
-# Creating & Reading
-# ==================
-def alpha(color: list[int] | str) -> int:
-    """Extracts the alpha value from a color or pixel array."""
-    if isinstance(color, list):
-        return _p5js.alpha(to_js(color))
-    return _p5js.alpha(color)
-
-
-def blue(color: list[int] | str) -> int:
-    """Extracts the blue value from a color or pixel array."""
-    if isinstance(color, list):
-        return _p5js.blue(to_js(color))
-    return _p5js.blue(color)
-
-
-def brightness(color: list[int] | str) -> int:
-    """Extracts the HSB brightness value from a color or pixel array."""
-    if isinstance(color, list):
-        return _p5js.brightness(to_js(color))
-    return _p5js.brightness(color)
-
-
-def color(
-    value: str | int | list[int],
-    v2: int | None = None,
-    v3: int | None = None,
-    v4: int | None = None,
-) -> str:
-    """Creates colors for storing in variables of the color datatype.
-    The parameters are interpreted as RGB or HSB values depending on the
-    current color_mode(). The default mode is RGB values from 0 to 255 and,
-    therefore, the function call color(255, 204, 0) will return a bright
-    yellow color.
-
-    Note that if only one value is provided to color(), it will be interpreted
-    as a grayscale value. Add a second value, and it will be used for alpha
-    transparency. When three values are specified, they are interpreted as
-    either RGB or HSB values. Adding a fourth value applies alpha
-    transparency.
-
-    If a single string argument is provided, RGB, RGBA and Hex CSS color
-    strings and all named color strings are supported. In this case, an alpha
-    number value as a second argument is not supported, the RGBA form should
-    be used.
-    """
-    if v4:
-        return _p5js.color(value, v2, v3, v4).toString()
-    if v3:
-        return _p5js.color(value, v2, v3).toString()
-    if v2:
-        return _p5js.color(value, v2).toString()
-    return _p5js.color(to_js(value)).toString()
-
-
-def green(color: str | list[int]) -> int:
-    """Extracts the green value from a color or pixel array."""
-    if isinstance(color, list):
-        return _p5js.green(to_js(color))
-    return _p5js.green(color)
-
-
-def hue(color: str | list[int]) -> int:
-    """Extracts the hue value from a color or pixel array.
-
-    Hue exists in both HSB and HSL. This function will return the
-    HSB-normalized hue when supplied with an HSB color object (or when
-    supplied with a pixel array while the color mode is HSB),but will
-    default to the HSL-normalized hue otherwise.
-    (The values will only be different if the maximum hue setting for
-    each system is different.)
-    """
-    if isinstance(color, list):
-        return _p5js.hue(to_js(color))
-    return _p5js.hue(color)
-
-
-def lerp_color(c1: str | list[int], c2: str | list[int], amt: float) -> str:
-    """Blends two colors to find a third color somewhere between them.
-    The amt parameter is the amount to interpolate between the two values
-    where 0.0 is equal to the first color, 0.1 is very near the first color,
-    0.5 is halfway in between, etc. An amount below 0 will be treated as 0.
-    Likewise, amounts above 1 will be capped at 1. This is different from the
-    behavior of lerp(), but necessary because otherwise numbers outside the
-    range will produce strange and unexpected colors.
-
-    The way that colors are interpolated depends on the current color mode.
-    """
-    _c1 = _p5js.color(to_js(c1))
-    _c2 = _p5js.color(to_js(c2))
-    return _p5js.lerpColor(_c1, _c2, amt).toString()
-
-
-def lightness(color: str | list[int]) -> int:
-    """Extracts the HSL lightness value from a color or pixel array."""
-    if isinstance(color, list):
-        return _p5js.lightness(to_js(color))
-    return _p5js.lightness(color)
-
-
-def red(color: str | list[int]) -> int:
-    """Extracts the red value from a color or pixel array."""
-    return _p5js.red(to_js(color))
-
-
-def saturation(color: str | list[int]) -> int:
-    """Extracts the saturation value from a color or pixel array.
-
-    Saturation is scaled differently in HSB and HSL. This function will return
-    the HSB saturation when supplied with an HSB color object (or when
-    supplied with a pixel array while the color mode is HSB), but will default
-    to the HSL saturation otherwise.
-    """
-    if isinstance(color, list):
-        return _p5js.saturation(to_js(color))
-    return _p5js.saturation(color)
-
-
-# =======
-# Setting
-# =======
-def background(
-    value: str | int | list[int],
-    v2: int | None = None,
-    v3: int | None = None,
-    v4: int | None = None,
-):
-    """The background() function sets the color used for the background of the p5 canvas.
-    The default background is transparent. This function is typically used within draw() to
-    clear the display window at the beginning of each frame, but it can be used inside setup()
-    to set the background on the first frame of animation or if the background need only be set once.
-
-    The color is either specified in terms of the RGB, HSB, or HSL color depending on the current color_mode.
-    (The default color space is RGB, with each value in the range from 0 to 255). The alpha range by default
-    is also 0 to 255.
-
-    A p5.Color object can also be provided to set the background color.
-    """
-    if v4:
-        _p5js.background(value, v2, v3, v4)
-    elif v3:
-        _p5js.background(value, v2, v3)
-    elif v2:
-        _p5js.background(value, v2)
-    else:
-        _p5js.background(to_js(value))
-
-
-def clear():
-    """Clears the pixels within a buffer.
-    This function only clears the canvas. It will not clear objects created by
-    create_x() functions such as createVideo() or createDiv(). Unlike the main
-    graphics context, pixels in additional graphics areas created with
-    create_graphics() can be entirely or partially transparent. This function
-    clears everything to make all of the pixels 100% transparent.
-
-    Note: In WebGL mode, this function can be passed normalized RGBA color
-    values in order to clear the screen to a specific color. In addition to
-    color, it will also clear the depth buffer. If you are not using the
-    WebGL renderer these color values will have no effect.
-    """
-    _p5js.clear()
-
-
-def color_mode(
-    mode: str,
-    max1: int | None = None,
-    max2: int | None = None,
-    max3: int | None = None,
-    max4: int | None = None,
-):
-    """color_mode() changes the way p5 interprets color data. By default,
-    the parameters for fill(), stroke(), background(), and color() are
-    defined by values between 0 and 255 using the RGB color model.
-    This is equivalent to setting color_mode(RGB, 255). Setting color_mode(HSB)
-    lets you use the HSB system instead. By default,
-    this is color_mode(HSB, 360, 100, 100, 1). You can also use HSL.
-
-    Note: existing color objects remember the mode that they were created in,
-    so you can change modes as you like without affecting their appearance.
-    """
-    if max4:
-        _p5js.colorMode(mode, max1, max2, max3, max4)
-    elif max3:
-        _p5js.colorMode(mode, max1, max2, max3)
-    elif max2:
-        _p5js.colorMode(mode, max1, max2)
-    elif max1:
-        _p5js.colorMode(mode, max1)
-    else:
-        _p5js.colorMode(mode)
-
-
-def fill(
-    value: str | int | list[int],
-    v2: int | None = None,
-    v3: int | None = None,
-    v4: int | None = None,
-):
-    """Sets the color used to fill shapes.
-    For example, if you run fill(204, 102, 0), all shapes drawn after the
-    fill() command will be filled with the color orange. This color is either
-    specified in terms of the RGB or HSB color depending on the current
-    color_mode(). (The default color space is RGB, with each value in the
-    range from 0 to 255). The alpha range by default is also 0 to 255.
-
-    If a single string argument is provided, RGB, RGBA and Hex CSS color
-    strings and all named color strings are supported. In this case, an alpha
-    number value as a second argument is not supported, the RGBA form should
-    be used.
-
-    A p5.Color object can also be provided to set the fill color.
-    """
-    if v4:
-        _p5js.fill(value, v2, v3, v4)
-    elif v3:
-        _p5js.fill(value, v2, v3)
-    elif v2:
-        _p5js.fill(value, v2)
-    else:
-        _p5js.fill(to_js(value))
-
-
-def no_fill():
-    """Disables filling geometry. If both no_stroke() and no_fill() are
-    called, nothing will be drawn to the screen.
-    """
-    _p5js.noFill()
-
-
-def no_stroke():
-    """Disables drawing the stroke (outline). If both no_stroke() and
-    no_fill() are called, nothing will be drawn to the screen.
-    """
-    _p5js.noStroke()
-
-
-def stroke(
-    value: str | int | list[int],
-    v2: int | None = None,
-    v3: int | None = None,
-    v4: int | None = None,
-):
-    """Sets the color used to draw lines and borders around shapes.
-    This color is either specified in terms of the RGB or HSB color depending
-    on the current color_mode() (the default color space is RGB, with each
-    value in the range from 0 to 255). The alpha range by default is also 0
-    to 255.
-
-    If a single string argument is provided, RGB, RGBA and Hex CSS color
-    strings and all named color strings are supported. In this case, an alpha
-    number value as a second argument is not supported, the RGBA form should
-    be used.
-
-    A p5.Color object can also be provided to set the stroke color.
-    """    
-    if v4:
-        _p5js.stroke(value, v2, v3, v4)
-    elif v3:
-        _p5js.stroke(value, v2, v3)
-    elif v2:
-        _p5js.stroke(value, v2)
-    else:
-        _p5js.stroke(to_js(value))
-
-
-def erase():
-    """All drawing that follows erase() will subtract from the canvas.
-    Erased areas will reveal the web page underneath the canvas. Erasing can
-    be canceled with no_rase().
-
-    Drawing done with image() and background() in between erase() and
-    no_erase() will not erase the canvas but works as usual.
-    """
-    _p5js.erase()
-
-
-def no_erase():
-    """Ends erasing that was started with erase().
-    The fill(), stroke(), and blend_mode() settings will return to what they
-    were prior to calling erase().
-    """
-    _p5js.noErase()
+class Colors(BaseSketch):
+    # ==================
+    # Creating & Reading
+    # ==================
+    def alpha(self, color: list[int] | str) -> int:
+        """Extracts the alpha value from a color or pixel array."""
+        if isinstance(color, list):
+            return self._p5js.alpha(to_js(color))
+        return self._p5js.alpha(color)
+
+    def blue(self, color: list[int] | str) -> int:
+        """Extracts the blue value from a color or pixel array."""
+        if isinstance(color, list):
+            return self._p5js.blue(to_js(color))
+        return self._p5js.blue(color)
+
+    def brightness(self, color: list[int] | str) -> int:
+        """Extracts the HSB brightness value from a color or pixel array."""
+        if isinstance(color, list):
+            return self._p5js.brightness(to_js(color))
+        return self._p5js.brightness(color)
+
+    def color(
+        self,
+        value: str | int | list[int],
+        v2: int | None = None,
+        v3: int | None = None,
+        v4: int | None = None,
+    ) -> str:
+        """Creates colors for storing in variables of the color datatype.
+        The parameters are interpreted as RGB or HSB values depending on the
+        current color_mode(). The default mode is RGB values from 0 to 255 and,
+        therefore, the function call color(255, 204, 0) will return a bright
+        yellow color.
+
+        Note that if only one value is provided to color(), it will be interpreted
+        as a grayscale value. Add a second value, and it will be used for alpha
+        transparency. When three values are specified, they are interpreted as
+        either RGB or HSB values. Adding a fourth value applies alpha
+        transparency.
+
+        If a single string argument is provided, RGB, RGBA and Hex CSS color
+        strings and all named color strings are supported. In this case, an alpha
+        number value as a second argument is not supported, the RGBA form should
+        be used.
+        """
+        if v4:
+            return self._p5js.color(value, v2, v3, v4).toString()
+        if v3:
+            return self._p5js.color(value, v2, v3).toString()
+        if v2:
+            return self._p5js.color(value, v2).toString()
+        return self._p5js.color(to_js(value)).toString()
+
+    def green(self, color: str | list[int]) -> int:
+        """Extracts the green value from a color or pixel array."""
+        if isinstance(color, list):
+            return self._p5js.green(to_js(color))
+        return self._p5js.green(color)
+
+    def hue(self, color: str | list[int]) -> int:
+        """Extracts the hue value from a color or pixel array.
+
+        Hue exists in both HSB and HSL. This function will return the
+        HSB-normalized hue when supplied with an HSB color object (or when
+        supplied with a pixel array while the color mode is HSB),but will
+        default to the HSL-normalized hue otherwise.
+        (The values will only be different if the maximum hue setting for
+        each system is different.)
+        """
+        if isinstance(color, list):
+            return self._p5js.hue(to_js(color))
+        return self._p5js.hue(color)
+
+    def lerp_color(self, c1: str | list[int], c2: str | list[int], amt: float) -> str:
+        """Blends two colors to find a third color somewhere between them.
+        The amt parameter is the amount to interpolate between the two values
+        where 0.0 is equal to the first color, 0.1 is very near the first color,
+        0.5 is halfway in between, etc. An amount below 0 will be treated as 0.
+        Likewise, amounts above 1 will be capped at 1. This is different from the
+        behavior of lerp(), but necessary because otherwise numbers outside the
+        range will produce strange and unexpected colors.
+
+        The way that colors are interpolated depends on the current color mode.
+        """
+        _c1 = self._p5js.color(to_js(c1))
+        _c2 = self._p5js.color(to_js(c2))
+        return self._p5js.lerpColor(_c1, _c2, amt).toString()
+
+    def lightness(self, color: str | list[int]) -> int:
+        """Extracts the HSL lightness value from a color or pixel array."""
+        if isinstance(color, list):
+            return self._p5js.lightness(to_js(color))
+        return self._p5js.lightness(color)
+
+    def red(self, color: str | list[int]) -> int:
+        """Extracts the red value from a color or pixel array."""
+        return self._p5js.red(to_js(color))
+
+    def saturation(self, color: str | list[int]) -> int:
+        """Extracts the saturation value from a color or pixel array.
+
+        Saturation is scaled differently in HSB and HSL. This function will return
+        the HSB saturation when supplied with an HSB color object (or when
+        supplied with a pixel array while the color mode is HSB), but will default
+        to the HSL saturation otherwise.
+        """
+        if isinstance(color, list):
+            return self._p5js.saturation(to_js(color))
+        return self._p5js.saturation(color)
+
+    # =======
+    # Setting
+    # =======
+    def background(
+        self,
+        value: str | int | list[int],
+        v2: int | None = None,
+        v3: int | None = None,
+        v4: int | None = None,
+    ):
+        """The background() function sets the color used for the background of the p5 canvas.
+        The default background is transparent. This function is typically used within draw() to
+        clear the display window at the beginning of each frame, but it can be used inside setup()
+        to set the background on the first frame of animation or if the background need only be set once.
+
+        The color is either specified in terms of the RGB, HSB, or HSL color depending on the current color_mode.
+        (The default color space is RGB, with each value in the range from 0 to 255). The alpha range by default
+        is also 0 to 255.
+
+        A p5.Color object can also be provided to set the background color.
+        """
+        if v4:
+            self._p5js.background(value, v2, v3, v4)
+        elif v3:
+            self._p5js.background(value, v2, v3)
+        elif v2:
+            self._p5js.background(value, v2)
+        else:
+            self._p5js.background(to_js(value))
+
+    def clear(self):
+        """Clears the pixels within a buffer.
+        This function only clears the canvas. It will not clear objects created by
+        create_x() functions such as createVideo() or createDiv(). Unlike the main
+        graphics context, pixels in additional graphics areas created with
+        create_graphics() can be entirely or partially transparent. This function
+        clears everything to make all of the pixels 100% transparent.
+
+        Note: In WebGL mode, this function can be passed normalized RGBA color
+        values in order to clear the screen to a specific color. In addition to
+        color, it will also clear the depth buffer. If you are not using the
+        WebGL renderer these color values will have no effect.
+        """
+        self._p5js.clear()
+
+    def color_mode(
+        self,
+        mode: str,
+        max1: int | None = None,
+        max2: int | None = None,
+        max3: int | None = None,
+        max4: int | None = None,
+    ):
+        """color_mode() changes the way p5 interprets color data. By default,
+        the parameters for fill(), stroke(), background(), and color() are
+        defined by values between 0 and 255 using the RGB color model.
+        This is equivalent to setting color_mode(RGB, 255). Setting color_mode(HSB)
+        lets you use the HSB system instead. By default,
+        this is color_mode(HSB, 360, 100, 100, 1). You can also use HSL.
+
+        Note: existing color objects remember the mode that they were created in,
+        so you can change modes as you like without affecting their appearance.
+        """
+        if max4:
+            self._p5js.colorMode(mode, max1, max2, max3, max4)
+        elif max3:
+            self._p5js.colorMode(mode, max1, max2, max3)
+        elif max2:
+            self._p5js.colorMode(mode, max1, max2)
+        elif max1:
+            self._p5js.colorMode(mode, max1)
+        else:
+            self._p5js.colorMode(mode)
+
+    def fill(
+        self,
+        value: str | int | list[int],
+        v2: int | None = None,
+        v3: int | None = None,
+        v4: int | None = None,
+    ):
+        """Sets the color used to fill shapes.
+        For example, if you run fill(204, 102, 0), all shapes drawn after the
+        fill() command will be filled with the color orange. This color is either
+        specified in terms of the RGB or HSB color depending on the current
+        color_mode(). (The default color space is RGB, with each value in the
+        range from 0 to 255). The alpha range by default is also 0 to 255.
+
+        If a single string argument is provided, RGB, RGBA and Hex CSS color
+        strings and all named color strings are supported. In this case, an alpha
+        number value as a second argument is not supported, the RGBA form should
+        be used.
+
+        A p5.Color object can also be provided to set the fill color.
+        """
+        if v4:
+            self._p5js.fill(value, v2, v3, v4)
+        elif v3:
+            self._p5js.fill(value, v2, v3)
+        elif v2:
+            self._p5js.fill(value, v2)
+        else:
+            self._p5js.fill(to_js(value))
+
+    def no_fill(self):
+        """Disables filling geometry. If both no_stroke() and no_fill() are
+        called, nothing will be drawn to the screen.
+        """
+        self._p5js.noFill()
+
+    def no_stroke(self):
+        """Disables drawing the stroke (outline). If both no_stroke() and
+        no_fill() are called, nothing will be drawn to the screen.
+        """
+        self._p5js.noStroke()
+
+    def stroke(
+        self,
+        value: str | int | list[int],
+        v2: int | None = None,
+        v3: int | None = None,
+        v4: int | None = None,
+    ):
+        """Sets the color used to draw lines and borders around shapes.
+        This color is either specified in terms of the RGB or HSB color depending
+        on the current color_mode() (the default color space is RGB, with each
+        value in the range from 0 to 255). The alpha range by default is also 0
+        to 255.
+
+        If a single string argument is provided, RGB, RGBA and Hex CSS color
+        strings and all named color strings are supported. In this case, an alpha
+        number value as a second argument is not supported, the RGBA form should
+        be used.
+
+        A p5.Color object can also be provided to set the stroke color.
+        """
+        if v4:
+            self._p5js.stroke(value, v2, v3, v4)
+        elif v3:
+            self._p5js.stroke(value, v2, v3)
+        elif v2:
+            self._p5js.stroke(value, v2)
+        else:
+            self._p5js.stroke(to_js(value))
+
+    def erase(self):
+        """All drawing that follows erase() will subtract from the canvas.
+        Erased areas will reveal the web page underneath the canvas. Erasing can
+        be canceled with no_rase().
+
+        Drawing done with image() and background() in between erase() and
+        no_erase() will not erase the canvas but works as usual.
+        """
+        self._p5js.erase()
+
+    def no_erase(self):
+        """Ends erasing that was started with erase().
+        The fill(), stroke(), and blend_mode() settings will return to what they
+        were prior to calling erase().
+        """
+        self._p5js.noErase()
```

### Comparing `proceso-0.0.4/src/proceso/data.py` & `proceso-0.0.6/src/proceso/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,89 @@
 from pyodide.ffi import to_js
 
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-# ================
-# String Functions
-# ================
-def nf(
-    num: float | list[float],
-    left: int | str | None = None,
-    right: int | str | None = None,
-) -> str | list[str]:
-    """Utility function for formatting numbers into strings.
-    There are two versions: one for formatting floats, and one for
-    formatting ints.
-
-    The values for the digits, left, and right parameters should always be
-    positive integers.
-
-    (NOTE): Be cautious when using left and right parameters as it prepends
-    numbers of 0's if the parameter if greater than the current length of the
-    number.
-
-    For example if number is 123.2 and left parameter passed is 4 which is
-    greater than length of 123 (integer part) i.e 3 than result will be
-    0123.2. Same case for right parameter i.e. if right is 3 than the result
-    will be 123.200.
-    """
-    return _p5js.nf(to_js(num), left, right)
-
-
-def nfc(
-    num: float | list[float],
-    right: int | str | None = None,
-) -> str | list[str]:
-    """Utility function for formatting numbers into strings and placing
-    appropriate commas to mark units of 1000.
-    There are two versions: one for formatting ints, and one for formatting
-    an array of ints. The value for the right parameter should always be a
-    positive integer.
-    """
-    return _p5js.nfc(to_js(num), right)
-
-
-def nfp(
-    num: float | list[float],
-    left: int | str | None = None,
-    right: int | str | None = None,
-) -> str | list[str]:
-    """Utility function for formatting numbers into strings.
-    Similar to nf() but puts a "+" in front of positive numbers and a "-"
-    in front of negative numbers. There are two versions: one for formatting
-    floats, and one for formatting ints. The values for left, and right
-    parameters should always be positive integers.
-    """
-    return _p5js.nfp(to_js(num), left, right)
-
-
-def nfs(
-    num: float | list[float],
-    left: int | str | None = None,
-    right: int | str | None = None,
-) -> str | list[str]:
-    """Utility function for formatting numbers into strings.
-    Similar to nf() but puts an additional "_" (space) in front of positive
-    numbers just in case to align it with negative numbers which includes "-"
-    (minus) sign.
-
-    The main usecase of nfs() can be seen when one wants to align the digits
-    (place values) of a non-negative number with some negative number (See
-    the example to get a clear picture). There are two versions: one for
-    formatting float, and one for formatting int.
-
-    The values for the digits, left, and right parameters should always be
-    positive integers.
-
-    (IMP): The result on the canvas basically the expected alignment can vary
-    based on the typeface you are using.
-
-    (NOTE): Be cautious when using left and right parameters as it prepends
-    numbers of 0's if the parameter if greater than the current length of the number.
-
-    For example if number is 123.2 and left parameter passed is 4 which is
-    greater than length of 123 (integer part) i.e 3 than result will be
-    0123.2. Same case for right parameter i.e. if right is 3 than the result
-    will be 123.200.
+class Data(BaseSketch):
+    def nf(
+        self,
+        num: float | list[float],
+        left: int | str | None = None,
+        right: int | str | None = None,
+    ) -> str | list[str]:
+        """Utility function for formatting numbers into strings.
+        There are two versions: one for formatting floats, and one for
+        formatting ints.
+
+        The values for the digits, left, and right parameters should always be
+        positive integers.
+
+        (NOTE): Be cautious when using left and right parameters as it prepends
+        numbers of 0's if the parameter if greater than the current length of the
+        number.
+
+        For example if number is 123.2 and left parameter passed is 4 which is
+        greater than length of 123 (integer part) i.e 3 than result will be
+        0123.2. Same case for right parameter i.e. if right is 3 than the result
+        will be 123.200.
+        """
+        return self._p5js.nf(to_js(num), left, right)
+
+    def nfc(
+        self,
+        num: float | list[float],
+        right: int | str | None = None,
+    ) -> str | list[str]:
+        """Utility function for formatting numbers into strings and placing
+        appropriate commas to mark units of 1000.
+        There are two versions: one for formatting ints, and one for formatting
+        an array of ints. The value for the right parameter should always be a
+        positive integer.
+        """
+        return self._p5js.nfc(to_js(num), right)
+
+    def nfp(
+        self,
+        num: float | list[float],
+        left: int | str | None = None,
+        right: int | str | None = None,
+    ) -> str | list[str]:
+        """Utility function for formatting numbers into strings.
+        Similar to nf() but puts a "+" in front of positive numbers and a "-"
+        in front of negative numbers. There are two versions: one for formatting
+        floats, and one for formatting ints. The values for left, and right
+        parameters should always be positive integers.
+        """
+        return self._p5js.nfp(to_js(num), left, right)
+
+    def nfs(
+        self,
+        num: float | list[float],
+        left: int | str | None = None,
+        right: int | str | None = None,
+    ) -> str | list[str]:
+        """Utility function for formatting numbers into strings.
+        Similar to nf() but puts an additional "_" (space) in front of positive
+        numbers just in case to align it with negative numbers which includes "-"
+        (minus) sign.
+
+        The main usecase of nfs() can be seen when one wants to align the digits
+        (place values) of a non-negative number with some negative number (See
+        the example to get a clear picture). There are two versions: one for
+        formatting float, and one for formatting int.
+
+        The values for the digits, left, and right parameters should always be
+        positive integers.
+
+        (IMP): The result on the canvas basically the expected alignment can vary
+        based on the typeface you are using.
+
+        (NOTE): Be cautious when using left and right parameters as it prepends
+        numbers of 0's if the parameter if greater than the current length of the number.
+
+        For example if number is 123.2 and left parameter passed is 4 which is
+        greater than length of 123 (integer part) i.e 3 than result will be
+        0123.2. Same case for right parameter i.e. if right is 3 than the result
+        will be 123.200.
 
-    """
-    return _p5js.nfs(to_js(num), left, right)
+        """
+        return self._p5js.nfs(to_js(num), left, right)
```

### Comparing `proceso-0.0.4/src/proceso/dom.py` & `proceso-0.0.6/src/proceso/dom.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,203 +1,195 @@
 from typing import Callable
 from pyodide.ffi import create_proxy, to_js
 
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-def select(selectors: str, container: str | None = None) -> object:
-    """Searches the page for the first element that matches the given CSS
-    selector string (can be an ID, class, tag name or a combination) and
-    returns it as a p5.Element.
-    The DOM node itself can be accessed with .elt. Returns null if none found.
-    You can also specify a container to search within.
-    """
-    return _p5js.select(selectors, container)
-
-
-def select_all(selectors: str, container: str | None = None) -> list[object]:
-    """Searches the page for elements that match the given CSS selector
-    string (can be an ID a class, tag name or a combination) and returns them
-    as p5.Elements in an array.
-    The DOM node itself can be accessed with .elt. Returns an empty array if
-    none found. You can also specify a container to search within.
-    """
-    return _p5js.selectAll(selectors, container)
-
-
-def remove_elements():
-    """Removes all elements created by p5, except any canvas / graphics
-    elements created by create_canvas or create_graphics.
-    Event handlers are removed, and element is removed from the DOM.
-    """
-    _p5js.removeElements()
-
-
-def create_div(html: str | None = None) -> object:
-    """Creates a <div></div> element in the DOM with given inner HTML."""
-    return _p5js.createDiv(html)
-
-
-def create_p(html: str | None = None) -> object:
-    """Creates a <p></p> element in the DOM with given inner HTML.
-    Used for paragraph length text.
-    """
-    return _p5js.createP(html)
-
-
-def create_span(html: str | None = None) -> object:
-    """Creates a <span></span> element in the DOM with given inner HTML."""
-    return _p5js.createSpan(html)
-
-
-def create_img(src: str, alt: str, cross_origin: str | None = None) -> object:
-    """Creates an <img> element in the DOM with given src and alternate text."""
-    return _p5js.createImg(src, alt, cross_origin)
-
-
-def create_a(html: str | None = None) -> object:
-    """Creates an <a></a> element in the DOM for including a hyperlink."""
-    return _p5js.createA(html)
-
-
-def create_slider(
-    min: float, max: float, value: float | None = None, step: float | None = None
-) -> object:
-    """Creates a slider <input></input> element in the DOM.
-    Use .size() to set the display length of the slider.
-    """
-    return _p5js.createSlider(min, max, value, step)
-
-
-def create_button(label: str, value: str | None = None) -> object:
-    """Creates a <button></button> element in the DOM.
-    Use .size() to set the display size of the button. Use .mousePressed() to
-    specify behavior on press.
-    """
-    return _p5js.createButton(label, value)
-
-
-def create_checkbox(label: str | None = None, value: str | None = None) -> object:
-    """Creates a checkbox <input></input> element in the DOM.
-    Calling .checked() on a checkbox returns a boolean indicating whether it
-    is checked or not.
-    """
-    return _p5js.createCheckbox(label, value)
-
-
-def create_select(multiple: bool | None = None) -> object:
-    """Creates a dropdown menu <select></select> element in the DOM.
-    It also assigns select-related methods to p5.Element when selecting an
-    existing select box. Options in the menu are unique by name (the display
-    text).
-
-    .option(name, [value]) can be used to add an option with name (the display
-    text) and value to the select element. If an option with name already
-    exists within the select element, this method will change its value to
-    value.
-
-    .value() will return the currently selected option.
-
-    .selected() will return the current dropdown element which is an instance
-    of p5.Element.
-
-    .selected(value) can be used to make given option selected by default
-    when the page first loads.
-
-    .disable() marks the whole dropdown element as disabled.
-
-    .disable(value) marks a given option as disabled.
-    """
-    return _p5js.createSelect(multiple)
-
-
-def create_radio() -> object:
-    """Creates a radio button element in the DOM.
-    It also helps existing radio buttons assign methods of p5.Element.
-
-    .option(value, [label]) can be used to create a new option for the
-    element. If an option with a value already exists, it will be returned. It
-    is recommended to use string values as input for value. Optionally, a
-    label can be provided as second argument for the option.
-
-    .remove(value) can be used to remove an option for the element. String
-    values recommended as input for value.
-
-    .value() method will return the currently selected value.
-
-    .selected() method will return the currently selected input element.
-
-    .selected(value) method will select the option and return it. String
-    values recommended as input for value.
-
-    .disable(Boolean) method will enable/disable the whole radio button element.
-    """
-    return _p5js.createRadio()
-
-
-def create_color_picker(color: str = None) -> object:
-    """Creates a color picker element in the DOM for color input.
-    The .value() method will return a hex string (#rrggbb) of the color.
-    The .color() method will return a p5.Color object with the current chosen
-    color.
-    """
-    return _p5js.createColorPicker(color)
-
-
-def create_input(value: str | None = None, type: str | None = None) -> object:
-    """Creates an <input></input> element in the DOM for text input.
-    Use .size() to set the display length of the box.
-    """
-    return _p5js.createInput(value, type)
-
-
-def create_file_input(callback: Callable, multiple: bool | None = None) -> object:
-    """Creates an <input></input> element in the DOM of type 'file'.
-    This allows users to select local files for use in a sketch.
-    """
-    return _p5js.createFileInput(create_proxy(callback), multiple)
-
-
-def create_video(src: str, callback: Callable | None = None) -> object:
-    """Creates an HTML5 <video> element in the DOM for simple playback of
-    audio/video.
-    Shown by default, can be hidden with .hide() and drawn into canvas using
-    image(). The first parameter can be either a single string path to a video
-    file, or an array of string paths to different formats of the same video.
-    This is useful for ensuring that your video can play across different
-    browsers, as each supports different formats. See this page for further
-    information about supported formats.
-    """
-    if callback:
-        return _p5js.createVideo(src, create_proxy(callback))
-    return _p5js.createCanvas(src)
-
-
-def create_audio(src: str | list[str], callback: Callable | None = None) -> object:
-    """Creates a hidden HTML5 <audio> element in the DOM for simple audio
-    playback.
-    The first parameter can be either a single string path to a audio file,
-    or an array of string paths to different formats of the same audio. This
-    is useful for ensuring that your audio can play across different browsers,
-    as each supports different formats. See this page for further information
-    about supported formats.
-    """
-    if callback:
-        return _p5js.createAudio(to_js(src), create_proxy(callback))
-    return _p5js.createAudio(to_js(src))
-
-
-def create_capture(type: str, callback: Callable | None = None) -> object:
-    """Creates a new HTML5 <video> element that contains the audio/video feed from a webcam. The element is separate from the canvas and is displayed by default. The element can be hidden using .hide(). The feed can be drawn onto the canvas using image(). The loadedmetadata property can be used to detect when the element has fully loaded (see second example).
-
-    More specific properties of the feed can be passing in a Constraints object. See the W3C spec for possible properties. Note that not all of these are supported by all browsers.
-
-    Security note: A new browser security specification requires that getUserMedia, which is behind createCapture(), only works when you're running the code locally, or on HTTPS. Learn more here and here.
-    """
-    if callback:
-        return _p5js.createCapture(type, create_proxy(callback))
-    return _p5js.createCapture(type)
-
-
-def create_element(tag: str, content: str | None = None) -> object:
-    """Creates element with given tag in the DOM with given content."""
-    return _p5js.createElement(tag, content)
+class DOM(BaseSketch):
+    def select(self, selectors: str, container: str | None = None) -> object:
+        """Searches the page for the first element that matches the given CSS
+        selector string (can be an ID, class, tag name or a combination) and
+        returns it as a p5.Element.
+        The DOM node itself can be accessed with .elt. Returns null if none found.
+        You can also specify a container to search within.
+        """
+        return self._p5js.select(selectors, container)
+
+    def select_all(self, selectors: str, container: str | None = None) -> list[object]:
+        """Searches the page for elements that match the given CSS selector
+        string (can be an ID a class, tag name or a combination) and returns them
+        as p5.Elements in an array.
+        The DOM node itself can be accessed with .elt. Returns an empty array if
+        none found. You can also specify a container to search within.
+        """
+        return self._p5js.selectAll(selectors, container)
+
+    def remove_elements(self):
+        """Removes all elements created by p5, except any canvas / graphics
+        elements created by create_canvas or create_graphics.
+        Event handlers are removed, and element is removed from the DOM.
+        """
+        self._p5js.removeElements()
+
+    def create_div(self, html: str | None = None) -> object:
+        """Creates a <div></div> element in the DOM with given inner HTML."""
+        return self._p5js.createDiv(html)
+
+    def create_p(self, html: str | None = None) -> object:
+        """Creates a <p></p> element in the DOM with given inner HTML.
+        Used for paragraph length text.
+        """
+        return self._p5js.createP(html)
+
+    def create_span(self, html: str | None = None) -> object:
+        """Creates a <span></span> element in the DOM with given inner HTML."""
+        return self._p5js.createSpan(html)
+
+    def create_img(self, src: str, alt: str, cross_origin: str | None = None) -> object:
+        """Creates an <img> element in the DOM with given src and alternate text."""
+        return self._p5js.createImg(src, alt, cross_origin)
+
+    def create_a(self, html: str | None = None) -> object:
+        """Creates an <a></a> element in the DOM for including a hyperlink."""
+        return self._p5js.createA(html)
+
+    def create_slider(
+        self,
+        min: float,
+        max: float,
+        value: float | None = None,
+        step: float | None = None,
+    ) -> object:
+        """Creates a slider <input></input> element in the DOM.
+        Use .size() to set the display length of the slider.
+        """
+        return self._p5js.createSlider(min, max, value, step)
+
+    def create_button(self, label: str, value: str | None = None) -> object:
+        """Creates a <button></button> element in the DOM.
+        Use .size() to set the display size of the button. Use .mousePressed() to
+        specify behavior on press.
+        """
+        return self._p5js.createButton(label, value)
+
+    def create_checkbox(
+        self, label: str | None = None, value: str | None = None
+    ) -> object:
+        """Creates a checkbox <input></input> element in the DOM.
+        Calling .checked() on a checkbox returns a boolean indicating whether it
+        is checked or not.
+        """
+        return self._p5js.createCheckbox(label, value)
+
+    def create_select(self, multiple: bool | None = None) -> object:
+        """Creates a dropdown menu <select></select> element in the DOM.
+        It also assigns select-related methods to p5.Element when selecting an
+        existing select box. Options in the menu are unique by name (the display
+        text).
+
+        .option(name, [value]) can be used to add an option with name (the display
+        text) and value to the select element. If an option with name already
+        exists within the select element, this method will change its value to
+        value.
+
+        .value() will return the currently selected option.
+
+        .selected() will return the current dropdown element which is an instance
+        of p5.Element.
+
+        .selected(value) can be used to make given option selected by default
+        when the page first loads.
+
+        .disable() marks the whole dropdown element as disabled.
+
+        .disable(value) marks a given option as disabled.
+        """
+        return self._p5js.createSelect(multiple)
+
+    def create_radio(self) -> object:
+        """Creates a radio button element in the DOM.
+        It also helps existing radio buttons assign methods of p5.Element.
+
+        .option(value, [label]) can be used to create a new option for the
+        element. If an option with a value already exists, it will be returned. It
+        is recommended to use string values as input for value. Optionally, a
+        label can be provided as second argument for the option.
+
+        .remove(value) can be used to remove an option for the element. String
+        values recommended as input for value.
+
+        .value() method will return the currently selected value.
+
+        .selected() method will return the currently selected input element.
+
+        .selected(value) method will select the option and return it. String
+        values recommended as input for value.
+
+        .disable(Boolean) method will enable/disable the whole radio button element.
+        """
+        return self._p5js.createRadio()
+
+    def create_color_picker(self, color: str = None) -> object:
+        """Creates a color picker element in the DOM for color input.
+        The .value() method will return a hex string (#rrggbb) of the color.
+        The .color() method will return a p5.Color object with the current chosen
+        color.
+        """
+        return self._p5js.createColorPicker(color)
+
+    def create_input(self, value: str | None = None, type: str | None = None) -> object:
+        """Creates an <input></input> element in the DOM for text input.
+        Use .size() to set the display length of the box.
+        """
+        return self._p5js.createInput(value, type)
+
+    def create_file_input(
+        self, callback: Callable, multiple: bool | None = None
+    ) -> object:
+        """Creates an <input></input> element in the DOM of type 'file'.
+        This allows users to select local files for use in a sketch.
+        """
+        return self._p5js.createFileInput(create_proxy(callback), multiple)
+
+    def create_video(self, src: str, callback: Callable | None = None) -> object:
+        """Creates an HTML5 <video> element in the DOM for simple playback of
+        audio/video.
+        Shown by default, can be hidden with .hide() and drawn into canvas using
+        image(). The first parameter can be either a single string path to a video
+        file, or an array of string paths to different formats of the same video.
+        This is useful for ensuring that your video can play across different
+        browsers, as each supports different formats. See this page for further
+        information about supported formats.
+        """
+        if callback:
+            return self._p5js.createVideo(src, create_proxy(callback))
+        return self._p5js.createCanvas(src)
+
+    def create_audio(
+        self, src: str | list[str], callback: Callable | None = None
+    ) -> object:
+        """Creates a hidden HTML5 <audio> element in the DOM for simple audio
+        playback.
+        The first parameter can be either a single string path to a audio file,
+        or an array of string paths to different formats of the same audio. This
+        is useful for ensuring that your audio can play across different browsers,
+        as each supports different formats. See this page for further information
+        about supported formats.
+        """
+        if callback:
+            return self._p5js.createAudio(to_js(src), create_proxy(callback))
+        return self._p5js.createAudio(to_js(src))
+
+    def create_capture(self, type: str, callback: Callable | None = None) -> object:
+        """Creates a new HTML5 <video> element that contains the audio/video feed from a webcam. The element is separate from the canvas and is displayed by default. The element can be hidden using .hide(). The feed can be drawn onto the canvas using image(). The loadedmetadata property can be used to detect when the element has fully loaded (see second example).
+
+        More specific properties of the feed can be passing in a Constraints object. See the W3C spec for possible properties. Note that not all of these are supported by all browsers.
+
+        Security note: A new browser security specification requires that getUserMedia, which is behind createCapture(), only works when you're running the code locally, or on HTTPS. Learn more here and here.
+        """
+        if callback:
+            return self._p5js.createCapture(type, create_proxy(callback))
+        return self._p5js.createCapture(type)
+
+    def create_element(self, tag: str, content: str | None = None) -> object:
+        """Creates element with given tag in the DOM with given content."""
+        return self._p5js.createElement(tag, content)
```

### Comparing `proceso-0.0.4/src/proceso/environment.py` & `proceso-0.0.6/src/proceso/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,180 +1,167 @@
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-def describe(text: str, display: str | None = None):
-    """Creates a screen reader accessible description for the canvas.
-    The first parameter should be a string with a description of the canvas.
-    The second parameter is optional. If specified, it determines how the
-    description is displayed.
-
-    describe(text, LABEL) displays the description to all users as a tombstone
-    or exhibit label/caption in a div adjacent to the canvas. You can style it
-    as you wish in your CSS.
-
-    describe(text, FALLBACK) makes the description accessible to screen-reader
-    users only, in a sub DOM inside the canvas element. If a second parameter
-    is not specified, by default, the description will only be available to
-    screen-reader users.
-    """
-    _p5js.describe(text, display)
-
-
-def describe_element(name: str, text: str, display: str | None = None):
-    """This function creates a screen-reader accessible description for
-    elements —shapes or groups of shapes that create meaning together— in
-    the canvas.
-    The first paramater should be the name of the element. The second
-    parameter should be a string with a description of the element. The third
-    parameter is optional. If specified, it determines how the element
-    description is displayed.
-
-    describe_element(name, text, LABEL) displays the element description to
-    all users as a tombstone or exhibit label/caption in a div adjacent to
-    the canvas. You can style it as you wish in your CSS.
-
-    describe_element(name, text, FALLBACK) makes the element description
-    accessible to screen-reader users only, in a sub DOM inside the canvas
-    element. If a second parameter is not specified, by default, the element
-    description will only be available to screen-reader users.
-    """
-    _p5js.describeElement(name, text, display)
-
-
-def text_output(display: str | None = None):
-    """text_output() creates a screenreader accessible output that describes
-    the shapes present on the canvas. The general description of the canvas
-    includes canvas size, canvas color, and number of elements in the canvas
-    (example: 'Your output is a, 400 by 400 pixels, lavender blue canvas
-    containing the following 4 shapes:'). This description is followed by a
-    list of shapes where the color, position, and area of each shape are
-    described (example: "orange ellipse at top left covering 1% of the
-    canvas"). Each element can be selected to get more details. A table of
-    elements is also provided. In this table, shape, color, location,
-    coordinates and area are described (example: "orange ellipse
-    location=top left area=2").
-
-    text_output() and text_output(FALLBACK) make the output available in a
-    sub DOM inside the canvas element which is accessible to screen readers.
-    text_output(LABEL) creates an additional div with the output adjacent to
-    the canvas, this is useful for non-screen reader users that might want to
-    display the output outside of the canvas' sub DOM as they code. However,
-    using LABEL will create unnecessary redundancy for screen reader users.
-    We recommend using LABEL only as part of the development process of a
-    sketch and removing it before publishing or sharing with screen reader
-    users.
-    """
-    _p5js.textOutput(display)
-
-
-
-def grid_output(display: str | None = None):
-    """grid_output() lays out the content of the canvas in the form of a grid
-    (html table) based on the spatial location of each shape.
-    A brief description of the canvas is available before the table output.
-    This description includes: color of the background, size of the canvas,
-    number of objects, and object types (example: "lavender blue canvas is
-    200 by 200 and contains 4 objects - 3 ellipses 1 rectangle"). The grid
-    describes the content spatially, each element is placed on a cell of the
-    table depending on its position. Within each cell an element the color
-    and type of shape of that element are available (example:
-    "orange ellipse"). These descriptions can be selected individually to
-    get more details. A list of elements where shape, color, location, and
-    area are described (example: "orange ellipse location=top left area=1%")
-    is also available.
-
-    grid_output() and grid_output(FALLBACK) make the output available in a
-    sub DOM inside the canvas element which is accessible to screen readers.
-    grid_output(LABEL) creates an additional div with the output adjacent to
-    the canvas, this is useful for non-screen reader users that might want to
-    display the output outside of the canvas' sub DOM as they code. However,
-    using LABEL will create unnecessary redundancy for screen reader users.
-    We recommend using LABEL only as part of the development process of a
-    sketch and removing it before publishing or sharing with screen reader
-    users.
-    """
-    _p5js.gridOutput(display)
-
-
-def cursor(type: str, x: float | None = None, y: float | None = None):
-    """Sets the cursor to a predefined symbol or an image, or makes it
-    visible if already hidden.
-    If you are trying to set an image as the cursor, the recommended size is
-    16×16 or 32×32 pixels. The values for parameters x and y must be less than
-    the dimensions of the image.
-    """
-    _p5js.cursor(type, x, y)
-
-
-def frame_rate(fps: float | None = None) -> float | None:
-    """Specifies the number of frames to be displayed every second.
-    For example, the function call frame_rate(30) will attempt to refresh 30
-    times a second. If the processor is not fast enough to maintain the
-    specified rate, the frame rate will not be achieved. Setting the frame
-    rate within setup() is recommended. The default frame rate is based on the
-    frame rate of the display (here also called "refresh rate"), which is set
-    to 60 frames per second on most computers. A frame rate of 24 frames per
-    second (usual for movies) or above will be enough for smooth animations.
-
-    Calling frame_rate() with no arguments returns the current framerate. The
-    draw function must run at least once before it will return a value. This
-    is the same as get_frame_rate().
-
-    Calling frame_rate() with arguments that are not of the type Number or are
-    non-positive also returns current framerate.
-    """
-    return _p5js.frameRate(fps)
-
-
-def get_target_frame_rate() -> float:
-    """Returns _targetFrameRate variable.
-    The default _targetFrameRate is set to 60. This could be changed by
-    calling frame_rate() and setting it to the desired value. When
-    get_target_frame_rate() is called, it should return the value that was set.
-    """
-    return _p5js.getTargetFrameRate()
-
-
-def hide_cursor():
-    """Hides the cursor from view."""
-    _p5js.hideCursor()
-
-
-def fullscreen(val: bool | None = None) -> bool:
-    """If argument is given, sets the sketch to fullscreen or not based on the
-    value of the argument.
-    If no argument is given, returns the current fullscreen state. Note that
-    due to browser restrictions this can only be called on user input, for
-    example, on mouse press like the example below.
-    """
-    return _p5js.fullscreen(val)
-
-
-def pixel_density(val: float) -> float | None:
-    """Sets the pixel scaling for high pixel density displays.
-    By default pixel density is set to match display density, call
-    pixel_density(1) to turn this off. Calling pixel_density() with no
-    arguments returns the current pixel density of the sketch.
-    """
-    return _p5js.pixelDensity(val)
-
-
-def display_density() -> float:
-    """Returns the pixel density of the current display the sketch is running
-    on.
-    """
-    return _p5js.displayDensity()
-
-
-def get_url() -> str:
-    """Gets the current URL."""
-    return _p5js.getURL()
-
-
-def get_url_path() -> list[str]:
-    """Gets the current URL path as an array."""
-    return _p5js.getURLPath()
-
-
-def get_url_params() -> dict:
-    """Gets the current URL params as a dictionary."""
-    return _p5js.getURLParams()
+class Environment(BaseSketch):
+    def describe(self, text: str, display: str | None = None):
+        """Creates a screen reader accessible description for the canvas.
+        The first parameter should be a string with a description of the canvas.
+        The second parameter is optional. If specified, it determines how the
+        description is displayed.
+
+        describe(text, LABEL) displays the description to all users as a tombstone
+        or exhibit label/caption in a div adjacent to the canvas. You can style it
+        as you wish in your CSS.
+
+        describe(text, FALLBACK) makes the description accessible to screen-reader
+        users only, in a sub DOM inside the canvas element. If a second parameter
+        is not specified, by default, the description will only be available to
+        screen-reader users.
+        """
+        self._p5js.describe(text, display)
+
+    def describe_element(self, name: str, text: str, display: str | None = None):
+        """This function creates a screen-reader accessible description for
+        elements —shapes or groups of shapes that create meaning together— in
+        the canvas.
+        The first paramater should be the name of the element. The second
+        parameter should be a string with a description of the element. The third
+        parameter is optional. If specified, it determines how the element
+        description is displayed.
+
+        describe_element(name, text, LABEL) displays the element description to
+        all users as a tombstone or exhibit label/caption in a div adjacent to
+        the canvas. You can style it as you wish in your CSS.
+
+        describe_element(name, text, FALLBACK) makes the element description
+        accessible to screen-reader users only, in a sub DOM inside the canvas
+        element. If a second parameter is not specified, by default, the element
+        description will only be available to screen-reader users.
+        """
+        self._p5js.describeElement(name, text, display)
+
+    def text_output(self, display: str | None = None):
+        """text_output() creates a screenreader accessible output that describes
+        the shapes present on the canvas. The general description of the canvas
+        includes canvas size, canvas color, and number of elements in the canvas
+        (example: 'Your output is a, 400 by 400 pixels, lavender blue canvas
+        containing the following 4 shapes:'). This description is followed by a
+        list of shapes where the color, position, and area of each shape are
+        described (example: "orange ellipse at top left covering 1% of the
+        canvas"). Each element can be selected to get more details. A table of
+        elements is also provided. In this table, shape, color, location,
+        coordinates and area are described (example: "orange ellipse
+        location=top left area=2").
+
+        text_output() and text_output(FALLBACK) make the output available in a
+        sub DOM inside the canvas element which is accessible to screen readers.
+        text_output(LABEL) creates an additional div with the output adjacent to
+        the canvas, this is useful for non-screen reader users that might want to
+        display the output outside of the canvas' sub DOM as they code. However,
+        using LABEL will create unnecessary redundancy for screen reader users.
+        We recommend using LABEL only as part of the development process of a
+        sketch and removing it before publishing or sharing with screen reader
+        users.
+        """
+        self._p5js.textOutput(display)
+
+    def grid_output(self, display: str | None = None):
+        """grid_output() lays out the content of the canvas in the form of a grid
+        (html table) based on the spatial location of each shape.
+        A brief description of the canvas is available before the table output.
+        This description includes: color of the background, size of the canvas,
+        number of objects, and object types (example: "lavender blue canvas is
+        200 by 200 and contains 4 objects - 3 ellipses 1 rectangle"). The grid
+        describes the content spatially, each element is placed on a cell of the
+        table depending on its position. Within each cell an element the color
+        and type of shape of that element are available (example:
+        "orange ellipse"). These descriptions can be selected individually to
+        get more details. A list of elements where shape, color, location, and
+        area are described (example: "orange ellipse location=top left area=1%")
+        is also available.
+
+        grid_output() and grid_output(FALLBACK) make the output available in a
+        sub DOM inside the canvas element which is accessible to screen readers.
+        grid_output(LABEL) creates an additional div with the output adjacent to
+        the canvas, this is useful for non-screen reader users that might want to
+        display the output outside of the canvas' sub DOM as they code. However,
+        using LABEL will create unnecessary redundancy for screen reader users.
+        We recommend using LABEL only as part of the development process of a
+        sketch and removing it before publishing or sharing with screen reader
+        users.
+        """
+        self._p5js.gridOutput(display)
+
+    def cursor(self, type: str, x: float | None = None, y: float | None = None):
+        """Sets the cursor to a predefined symbol or an image, or makes it
+        visible if already hidden.
+        If you are trying to set an image as the cursor, the recommended size is
+        16×16 or 32×32 pixels. The values for parameters x and y must be less than
+        the dimensions of the image.
+        """
+        self._p5js.cursor(type, x, y)
+
+    def frame_rate(self, fps: float | None = None) -> float | None:
+        """Specifies the number of frames to be displayed every second.
+        For example, the function call frame_rate(30) will attempt to refresh 30
+        times a second. If the processor is not fast enough to maintain the
+        specified rate, the frame rate will not be achieved. Setting the frame
+        rate within setup() is recommended. The default frame rate is based on the
+        frame rate of the display (here also called "refresh rate"), which is set
+        to 60 frames per second on most computers. A frame rate of 24 frames per
+        second (usual for movies) or above will be enough for smooth animations.
+
+        Calling frame_rate() with no arguments returns the current framerate. The
+        draw function must run at least once before it will return a value. This
+        is the same as get_frame_rate().
+
+        Calling frame_rate() with arguments that are not of the type Number or are
+        non-positive also returns current framerate.
+        """
+        return self._p5js.frameRate(fps)
+
+    def get_target_frame_rate(self) -> float:
+        """Returns _targetFrameRate variable.
+        The default _targetFrameRate is set to 60. This could be changed by
+        calling frame_rate() and setting it to the desired value. When
+        get_target_frame_rate() is called, it should return the value that was set.
+        """
+        return self._p5js.getTargetFrameRate()
+
+    def hide_cursor(self):
+        """Hides the cursor from view."""
+        self._p5js.hideCursor()
+
+    def fullscreen(self, val: bool | None = None) -> bool:
+        """If argument is given, sets the sketch to fullscreen or not based on the
+        value of the argument.
+        If no argument is given, returns the current fullscreen state. Note that
+        due to browser restrictions this can only be called on user input, for
+        example, on mouse press like the example below.
+        """
+        return self._p5js.fullscreen(val)
+
+    def pixel_density(self, val: float) -> float | None:
+        """Sets the pixel scaling for high pixel density displays.
+        By default pixel density is set to match display density, call
+        pixel_density(1) to turn this off. Calling pixel_density() with no
+        arguments returns the current pixel density of the sketch.
+        """
+        return self._p5js.pixelDensity(val)
+
+    def display_density(self) -> float:
+        """Returns the pixel density of the current display the sketch is running
+        on.
+        """
+        return self._p5js.displayDensity()
+
+    def get_url(self) -> str:
+        """Gets the current URL."""
+        return self._p5js.getURL()
+
+    def get_url_path(self) -> list[str]:
+        """Gets the current URL path as an array."""
+        return self._p5js.getURLPath()
+
+    def get_url_params(self) -> dict:
+        """Gets the current URL params as a dictionary."""
+        return self._p5js.getURLParams()
```

### Comparing `proceso-0.0.4/src/proceso/events.py` & `proceso-0.0.6/src/proceso/events.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-# ============
-# Acceleration
-# ============
-def set_move_threshold(value: float):
-    """The set_move_threshold() function is used to set the movement threshold
-    for the device_moved() function.
-    The default threshold is set to 0.5.
-    """
-    _p5js.setMoveThreshold(value)
-
-
-def set_shake_threshold(value: float):
-    """The set_shake_threshold() function is used to set the movement
-    threshold for the device_shaken() function.
-    The default threshold is set to 30.
-    """
-    _p5js.setShakeThreshold(value)
-
-
-# =====
-# Mouse
-# =====
-def request_pointer_lock():
-    """The function request_pointer_lock() locks the pointer to its current
-    position and makes it invisible.
-    Use moved_x and moved_y to get the difference the mouse was moved since
-    the last call of draw. Note that not all browsers support this feature.
-    This enables you to create experiences that aren't limited by the mouse
-    moving out of the screen even if it is repeatedly moved into one
-    direction. For example, a first person perspective experience.
-    """
-    _p5js.requestPointerLock()
-
-
-def exit_pointer_lock():
-    """The function exit_pointer_lock() exits a previously triggered
-    pointerLock for example to make ui elements usable etc.
-    """
-    _p5js.exitPointerLock()
+class Events(BaseSketch):
+    # ============
+    # Acceleration
+    # ============
+    def set_move_threshold(self, value: float):
+        """The set_move_threshold() function is used to set the movement threshold
+        for the device_moved() function.
+        The default threshold is set to 0.5.
+        """
+        self._p5js.setMoveThreshold(value)
+
+    def set_shake_threshold(self, value: float):
+        """The set_shake_threshold() function is used to set the movement
+        threshold for the device_shaken() function.
+        The default threshold is set to 30.
+        """
+        self._p5js.setShakeThreshold(value)
+
+    # =====
+    # Mouse
+    # =====
+    def request_pointer_lock(self):
+        """The function request_pointer_lock() locks the pointer to its current
+        position and makes it invisible.
+        Use moved_x and moved_y to get the difference the mouse was moved since
+        the last call of draw. Note that not all browsers support this feature.
+        This enables you to create experiences that aren't limited by the mouse
+        moving out of the screen even if it is repeatedly moved into one
+        direction. For example, a first person perspective experience.
+        """
+        self._p5js.requestPointerLock()
+
+    def exit_pointer_lock(self):
+        """The function exit_pointer_lock() exits a previously triggered
+        pointerLock for example to make ui elements usable etc.
+        """
+        self._p5js.exitPointerLock()
```

### Comparing `proceso-0.0.4/src/proceso/images.py` & `proceso-0.0.6/src/proceso/images.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,329 +1,321 @@
 from pyodide.ffi import to_js
 
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-def create_image(width: int, height: int) -> object:
-    """Creates a new p5.Image (the datatype for storing images).
-    This provides a fresh buffer of pixels to play with. Set the size of the
-    buffer with the width and height parameters.
-
-    .pixels gives access to a list containing the values for all the pixels
-    in the display window. These values are numbers. This list is the size
-    (including an appropriate factor for the pixel_density) of the display
-    window x4, representing the R, G, B, A values in order for each pixel,
-    moving from left to right across each row, then down each column. See
-    .pixels for more info. It may also be simpler to use set_pixels() or get_pixels().
-
-    Before accessing the pixels of an image, the data must loaded with the
-    load_pixels() function. After the list data has been modified, the
-    update_pixels() function must be run to update the changes.
-    """
-    return _p5js.createImage(width, height)
-
-
-def save_canvas(filename: str, extension: str):
-    """Save the current canvas as an image.
-    The browser will either save the file immediately, or prompt the user
-    with a dialogue window.
-    """
-    _p5js.saveCanvas(filename, extension)
-
-
-def save_frames(
-    filename: str,
-    extension: str,
-    duration: float,
-    framerate: float,
-):
-    """Capture a sequence of frames that can be used to create a movie.
-    Accepts a callback. For example, you may wish to send the frames to a
-    server where they can be stored or converted into a movie. If no
-    callback is provided, the browser will pop up save dialogues in an
-    attempt to download all of the images that have just been created. With
-    the callback provided the image data isn't saved by default but instead
-    passed as an argument to the callback function as a list of objects,
-    with the size of list equal to the total number of frames.
-
-    The arguments duration and framerate are constrained to be less or equal
-    to 15 and 22, respectively, which means you can only download a maximum of
-    15 seconds worth of frames at 22 frames per second, adding up to 330
-    frames. This is done in order to avoid memory problems since a large
-    enough canvas can fill up the memory in your computer very easily and
-    crash your program or even your browser.
-
-    To export longer animations, you might look into a library like
-    ccapture.js.
-    """
-    _p5js.saveFrames(filename, extension, duration, framerate)
-
-
-# ====================
-# Loading & Displaying
-# ====================
-def load_image(path: str) -> object:
-    """Loads an image from a path and creates a p5.Image from it.
-
-    The image may not be immediately available for rendering. If you want to
-    ensure that the image is ready before doing anything with it, place the
-    loadImage() call in preload(). You may also supply a callback function to
-    handle the image when it's ready.
-
-    The path to the image should be relative to the HTML file that links in
-    your sketch. Loading an image from a URL or other remote location may be
-    blocked due to your browser's built-in security.
-
-    You can also pass in a string of a base64 encoded image as an alternative
-    to the file path. Remember to add "data:image/png;base64," in front of the
-    string.
-    """
-    return _p5js.loadImage(path)
-
-
-def save_gif(
-    filename: str,
-    duration: int,
-    options: dict | None = None,
-):
-    """Generates a gif of your current animation and downloads it to your
-    computer!
-
-    The duration argument specifies how many seconds you want to record from
-    your animation. This value is then converted to the necessary number of
-    frames to generate it, depending on the value of units. More on that on
-    the next paragraph.
-
-    An optional object that can contain two more arguments: delay (number) and
-    units (string).
-
-    delay, specifying how much time we should wait before recording
-
-    units, a string that can be either 'seconds' or 'frames'. By default it's
-    'seconds'.
-
-    units specifies how the duration and delay arguments will behave. If
-    'seconds', these arguments will correspond to seconds, meaning that 3
-    seconds worth of animation will be created. If 'frames', the arguments
-    now correspond to the number of frames you want your animation to be, if
-    you are very sure of this number.
-
-    This may be called in setup, or, like in the example below, inside an
-    event function, like key_pressed or mouse_pressed.
-    """
-    _p5js.saveGif(filename, duration, options)
-
-
-def image(
-    img: object,
-    x: float,
-    y: float,
-    width: float | None = None,
-    height: float | None = None,
-):
-    """Draw an image to the p5 canvas.
-
-    This function can be used with different numbers of parameters. The
-    simplest use requires only three parameters: img, x, and y—where (x, y) is
-    the position of the image. Two more parameters can optionally be added to
-    specify the width and height of the image.
-
-    This function can also be used with eight Number parameters. To
-    differentiate between all these parameters, p5.js uses the language of
-    "destination rectangle" (which corresponds to "dx", "dy", etc.) and
-    "source image" (which corresponds to "sx", "sy", etc.) below. Specifying
-    the "source image" dimensions can be useful when you want to display a
-    subsection of the source image instead of the whole thing.
-    """
-    _p5js.image(img, x, y, width, height)
-
-
-def tint(
-    value: str | int | list[int],
-    v2: int | None = None,
-    v3: int | None = None,
-    v4: int | None = None,
-):
-    """Sets the fill value for displaying images.
-    Images can be tinted to specified colors or made transparent by including
-    an alpha value.
-
-    To apply transparency to an image without affecting its color, use white
-    as the tint color and specify an alpha value. For instance, tint(255, 128)
-    will make an image 50% transparent (assuming the default alpha range of
-    0-255, which can be changed with color_mode()).
-
-    The value for the gray parameter must be less than or equal to the current
-    maximum value as specified by color_mode(). The default maximum value is
-    255.
-    """
-    if v4:
-        _p5js.tint(value, v2, v3, v4)
-    elif v3:
-        _p5js.tint(value, v2, v3)
-    elif v2:
-        _p5js.tint(value, v2)
-    else:
-        _p5js.tint(to_js(value))
-
-
-def no_tint():
-    """Removes the current fill value for displaying images and reverts to
-    displaying images with their original hues.
-    """
-    _p5js.noTint()
-
-
-def image_mode(mode: str):
-    """Set image mode. Modifies the location from which images are drawn by
-    changing the way in which parameters given to image() are interpreted.
-    The default mode is image_mode(CORNER), which interprets the second and
-    third parameters of image() as the upper-left corner of the image. If two
-    additional parameters are specified, they are used to set the image's
-    width and height.
-
-    image_mode(CORNERS) interprets the second and third parameters of image()
-    as the location of one corner, and the fourth and fifth parameters as the
-    opposite corner.
-
-    image_mode(CENTER) interprets the second and third parameters of image() as
-    the image's center point. If two additional parameters are specified, they
-    are used to set the image's width and height.
-    """
-    _p5js.imageMode(mode)
-
-
-# ======
-# Pixels
-# ======
-def blend(
-    src_image: object,
-    sx: int,
-    sy: int,
-    sw: int,
-    sh: int,
-    dx: int,
-    dy: int,
-    dw: int,
-    dh: int,
-    blend_mode: str,
-):
-    """Copies a region of pixels from one image to another, using a specified
-    blend mode to do the operation.
-    """
-    _p5js.blend(src_image, sx, sy, sw, sh, dx, dy, dw, dh, blend_mode)
-
-
-def copy(
-    src_image: object,
-    sx: int,
-    sy: int,
-    sw: int,
-    sh: int,
-    dx: int,
-    dy: int,
-    dw: int,
-    dh: int,
-):
-    """Copies a region of the canvas to another region of the canvas and
-    copies a region of pixels from an image used as the srcImg parameter into
-    the canvas src_image is specified this is used as the source.
-    If the source and destination regions aren't the same size, it will
-    automatically resize source pixels to fit the specified target region.
-    """
-    _p5js.copy(src_image, sx, sy, sw, sh, dx, dy, dw, dh)
-
-
-def apply_filter(filter_type: str, filter_param: float | None = None):
-    """Applies a filter to the canvas.
-    The presets options are:
-
-    THRESHOLD Converts the image to black and white pixels depending if they
-    are above or below the threshold defined by the level parameter. The
-    parameter must be between 0.0 (black) and 1.0 (white). If no level is
-    specified, 0.5 is used.
-
-    GRAY Converts any colors in the image to grayscale equivalents. No
-    parameter is used.
-
-    OPAQUE Sets the alpha channel to entirely opaque. No parameter is used.
-
-    INVERT Sets each pixel to its inverse value. No parameter is used.
-
-    POSTERIZE Limits each channel of the image to the number of colors
-    specified as the parameter. The parameter can be set to values between 2
-    and 255, but results are most noticeable in the lower ranges.
-
-    BLUR Executes a Gaussian blur with the level parameter specifying the
-    extent of the blurring. If no parameter is used, the blur is equivalent to
-    Gaussian blur of radius 1. Larger values increase the blur.
-
-    ERODE Reduces the light areas. No parameter is used.
-
-    DILATE Increases the light areas. No parameter is used.
-
-    apply_filter() does not work in WEBGL mode. A similar effect can be achieved in
-    WEBGL mode using custom shaders. Adam Ferriss has written a selection of
-    shader examples that contains many of the effects present in the filter
-    examples.
-    """
-    _p5js.filter(filter_type, filter_param)
-
-
-def get_pixels(
-    x: int, y: int, width: int | None = None, height: int | None = None
-) -> list[float] | object:
-    """Get a region of pixels, or a single pixel, from the canvas.
-
-    Returns a list of [R,G,B,A] values for any pixel or grabs a section of
-    an image. If no parameters are specified, the entire image is returned.
-    Use the x and y parameters to get the value of one pixel. Get a section of
-    the display window by specifying additional w and h parameters. When
-    getting an image, the x and y parameters define the coordinates for the
-    upper-left corner of the image, regardless of the current image_mode().
-
-    Getting the color of a single pixel with get_pixels(x, y) is easy, but not as
-    fast as grabbing the data directly from pixels[].
-    """
-    return _p5js.get(x, y, width, height)
-
-
-def load_pixels():
-    """Loads the pixel data for the display window into the pixels[] list.
-    This function must always be called before reading from or writing to
-    pixels[]. Note that only changes made with set_pixels() or direct manipulation of
-    pixels[] will occur.
-    """
-    _p5js.loadPixels()
-
-
-def set_pixels(x: int, y: int, c: float | list[float] | object):
-    """Changes the color of any pixel, or writes an image directly to the
-    display window.
-    The x and y parameters specify the pixel to change and the c parameter
-    specifies the color value. This can be a p5.Color object, or [R, G, B, A]
-    pixel list. It can also be a single grayscale value. When setting an
-    image, the x and y parameters define the coordinates for the upper-left
-    corner of the image, regardless of the current imageMode().
-
-    After using set_pixels(), you must call update_pixels() for your changes to
-    appear. This should be called once all pixels have been set, and must be
-    called before calling get_pixels() or drawing the image.
-
-    Setting the color of a single pixel with set_pixels(x, y) is easy, but not as
-    fast as putting the data directly into pixels[]. Setting the pixels[]
-    values directly may be complicated when working with a retina display, but
-    will perform better when lots of pixels need to be set directly on every
-    loop. See the reference for pixels[] for more information.
-    """
-    _p5js.set(x, y, c)
-
-
-def update_pixels():
-    """Updates the display window with the data in the pixels[] list.
-    Use in conjunction with loadPixels(). If you're only reading pixels from
-    the list, there's no need to call update_pixels() — updating is only
-    necessary to apply changes. update_pixels() should be called anytime the
-    pixels list is manipulated or set_pixels() is called, and only changes made with
-    set_pixels() or direct changes to pixels[] will occur.
-    """
-    _p5js.updatePixels()
+class Images(BaseSketch):
+    def create_image(self, width: int, height: int) -> object:
+        """Creates a new p5.Image (the datatype for storing images).
+        This provides a fresh buffer of pixels to play with. Set the size of the
+        buffer with the width and height parameters.
+
+        .pixels gives access to a list containing the values for all the pixels
+        in the display window. These values are numbers. This list is the size
+        (including an appropriate factor for the pixel_density) of the display
+        window x4, representing the R, G, B, A values in order for each pixel,
+        moving from left to right across each row, then down each column. See
+        .pixels for more info. It may also be simpler to use set_pixels() or get_pixels().
+
+        Before accessing the pixels of an image, the data must loaded with the
+        load_pixels() function. After the list data has been modified, the
+        update_pixels() function must be run to update the changes.
+        """
+        return self._p5js.createImage(width, height)
+
+    def save_canvas(self, filename: str, extension: str):
+        """Save the current canvas as an image.
+        The browser will either save the file immediately, or prompt the user
+        with a dialogue window.
+        """
+        self._p5js.saveCanvas(filename, extension)
+
+    def save_frames(
+        self,
+        filename: str,
+        extension: str,
+        duration: float,
+        framerate: float,
+    ):
+        """Capture a sequence of frames that can be used to create a movie.
+        Accepts a callback. For example, you may wish to send the frames to a
+        server where they can be stored or converted into a movie. If no
+        callback is provided, the browser will pop up save dialogues in an
+        attempt to download all of the images that have just been created. With
+        the callback provided the image data isn't saved by default but instead
+        passed as an argument to the callback function as a list of objects,
+        with the size of list equal to the total number of frames.
+
+        The arguments duration and framerate are constrained to be less or equal
+        to 15 and 22, respectively, which means you can only download a maximum of
+        15 seconds worth of frames at 22 frames per second, adding up to 330
+        frames. This is done in order to avoid memory problems since a large
+        enough canvas can fill up the memory in your computer very easily and
+        crash your program or even your browser.
+
+        To export longer animations, you might look into a library like
+        ccapture.js.
+        """
+        self._p5js.saveFrames(filename, extension, duration, framerate)
+
+    # ====================
+    # Loading & Displaying
+    # ====================
+    def load_image(self, path: str) -> object:
+        """Loads an image from a path and creates a p5.Image from it.
+
+        The image may not be immediately available for rendering. If you want to
+        ensure that the image is ready before doing anything with it, place the
+        loadImage() call in preload(). You may also supply a callback function to
+        handle the image when it's ready.
+
+        The path to the image should be relative to the HTML file that links in
+        your sketch. Loading an image from a URL or other remote location may be
+        blocked due to your browser's built-in security.
+
+        You can also pass in a string of a base64 encoded image as an alternative
+        to the file path. Remember to add "data:image/png;base64," in front of the
+        string.
+        """
+        return self._p5js.loadImage(path)
+
+    def save_gif(
+        self,
+        filename: str,
+        duration: int,
+        options: dict | None = None,
+    ):
+        """Generates a gif of your current animation and downloads it to your
+        computer!
+
+        The duration argument specifies how many seconds you want to record from
+        your animation. This value is then converted to the necessary number of
+        frames to generate it, depending on the value of units. More on that on
+        the next paragraph.
+
+        An optional object that can contain two more arguments: delay (number) and
+        units (string).
+
+        delay, specifying how much time we should wait before recording
+
+        units, a string that can be either 'seconds' or 'frames'. By default it's
+        'seconds'.
+
+        units specifies how the duration and delay arguments will behave. If
+        'seconds', these arguments will correspond to seconds, meaning that 3
+        seconds worth of animation will be created. If 'frames', the arguments
+        now correspond to the number of frames you want your animation to be, if
+        you are very sure of this number.
+
+        This may be called in setup, or, like in the example below, inside an
+        event function, like key_pressed or mouse_pressed.
+        """
+        self._p5js.saveGif(filename, duration, options)
+
+    def image(
+        self,
+        img: object,
+        x: float,
+        y: float,
+        width: float | None = None,
+        height: float | None = None,
+    ):
+        """Draw an image to the p5 canvas.
+
+        This function can be used with different numbers of parameters. The
+        simplest use requires only three parameters: img, x, and y—where (x, y) is
+        the position of the image. Two more parameters can optionally be added to
+        specify the width and height of the image.
+
+        This function can also be used with eight Number parameters. To
+        differentiate between all these parameters, p5.js uses the language of
+        "destination rectangle" (which corresponds to "dx", "dy", etc.) and
+        "source image" (which corresponds to "sx", "sy", etc.) below. Specifying
+        the "source image" dimensions can be useful when you want to display a
+        subsection of the source image instead of the whole thing.
+        """
+        self._p5js.image(img, x, y, width, height)
+
+    def tint(
+        self,
+        value: str | int | list[int],
+        v2: int | None = None,
+        v3: int | None = None,
+        v4: int | None = None,
+    ):
+        """Sets the fill value for displaying images.
+        Images can be tinted to specified colors or made transparent by including
+        an alpha value.
+
+        To apply transparency to an image without affecting its color, use white
+        as the tint color and specify an alpha value. For instance, tint(255, 128)
+        will make an image 50% transparent (assuming the default alpha range of
+        0-255, which can be changed with color_mode()).
+
+        The value for the gray parameter must be less than or equal to the current
+        maximum value as specified by color_mode(). The default maximum value is
+        255.
+        """
+        if v4:
+            self._p5js.tint(value, v2, v3, v4)
+        elif v3:
+            self._p5js.tint(value, v2, v3)
+        elif v2:
+            self._p5js.tint(value, v2)
+        else:
+            self._p5js.tint(to_js(value))
+
+    def no_tint(self):
+        """Removes the current fill value for displaying images and reverts to
+        displaying images with their original hues.
+        """
+        self._p5js.noTint()
+
+    def image_mode(self, mode: str):
+        """Set image mode. Modifies the location from which images are drawn by
+        changing the way in which parameters given to image() are interpreted.
+        The default mode is image_mode(CORNER), which interprets the second and
+        third parameters of image() as the upper-left corner of the image. If two
+        additional parameters are specified, they are used to set the image's
+        width and height.
+
+        image_mode(CORNERS) interprets the second and third parameters of image()
+        as the location of one corner, and the fourth and fifth parameters as the
+        opposite corner.
+
+        image_mode(CENTER) interprets the second and third parameters of image() as
+        the image's center point. If two additional parameters are specified, they
+        are used to set the image's width and height.
+        """
+        self._p5js.imageMode(mode)
+
+    # ======
+    # Pixels
+    # ======
+    def blend(
+        self,
+        src_image: object,
+        sx: int,
+        sy: int,
+        sw: int,
+        sh: int,
+        dx: int,
+        dy: int,
+        dw: int,
+        dh: int,
+        blend_mode: str,
+    ):
+        """Copies a region of pixels from one image to another, using a specified
+        blend mode to do the operation.
+        """
+        self._p5js.blend(src_image, sx, sy, sw, sh, dx, dy, dw, dh, blend_mode)
+
+    def copy(
+        self,
+        src_image: object,
+        sx: int,
+        sy: int,
+        sw: int,
+        sh: int,
+        dx: int,
+        dy: int,
+        dw: int,
+        dh: int,
+    ):
+        """Copies a region of the canvas to another region of the canvas and
+        copies a region of pixels from an image used as the srcImg parameter into
+        the canvas src_image is specified this is used as the source.
+        If the source and destination regions aren't the same size, it will
+        automatically resize source pixels to fit the specified target region.
+        """
+        self._p5js.copy(src_image, sx, sy, sw, sh, dx, dy, dw, dh)
+
+    def apply_filter(self, filter_type: str, filter_param: float | None = None):
+        """Applies a filter to the canvas.
+        The presets options are:
+
+        THRESHOLD Converts the image to black and white pixels depending if they
+        are above or below the threshold defined by the level parameter. The
+        parameter must be between 0.0 (black) and 1.0 (white). If no level is
+        specified, 0.5 is used.
+
+        GRAY Converts any colors in the image to grayscale equivalents. No
+        parameter is used.
+
+        OPAQUE Sets the alpha channel to entirely opaque. No parameter is used.
+
+        INVERT Sets each pixel to its inverse value. No parameter is used.
+
+        POSTERIZE Limits each channel of the image to the number of colors
+        specified as the parameter. The parameter can be set to values between 2
+        and 255, but results are most noticeable in the lower ranges.
+
+        BLUR Executes a Gaussian blur with the level parameter specifying the
+        extent of the blurring. If no parameter is used, the blur is equivalent to
+        Gaussian blur of radius 1. Larger values increase the blur.
+
+        ERODE Reduces the light areas. No parameter is used.
+
+        DILATE Increases the light areas. No parameter is used.
+
+        apply_filter() does not work in WEBGL mode. A similar effect can be achieved in
+        WEBGL mode using custom shaders. Adam Ferriss has written a selection of
+        shader examples that contains many of the effects present in the filter
+        examples.
+        """
+        self._p5js.filter(filter_type, filter_param)
+
+    def get_pixels(
+        self, x: int, y: int, width: int | None = None, height: int | None = None
+    ) -> list[float] | object:
+        """Get a region of pixels, or a single pixel, from the canvas.
+
+        Returns a list of [R,G,B,A] values for any pixel or grabs a section of
+        an image. If no parameters are specified, the entire image is returned.
+        Use the x and y parameters to get the value of one pixel. Get a section of
+        the display window by specifying additional w and h parameters. When
+        getting an image, the x and y parameters define the coordinates for the
+        upper-left corner of the image, regardless of the current image_mode().
+
+        Getting the color of a single pixel with get_pixels(x, y) is easy, but not as
+        fast as grabbing the data directly from pixels[].
+        """
+        return self._p5js.get(x, y, width, height)
+
+    def load_pixels(self):
+        """Loads the pixel data for the display window into the pixels[] list.
+        This function must always be called before reading from or writing to
+        pixels[]. Note that only changes made with set_pixels() or direct manipulation of
+        pixels[] will occur.
+        """
+        self._p5js.loadPixels()
+
+    def set_pixels(self, x: int, y: int, c: float | list[float] | object):
+        """Changes the color of any pixel, or writes an image directly to the
+        display window.
+        The x and y parameters specify the pixel to change and the c parameter
+        specifies the color value. This can be a p5.Color object, or [R, G, B, A]
+        pixel list. It can also be a single grayscale value. When setting an
+        image, the x and y parameters define the coordinates for the upper-left
+        corner of the image, regardless of the current imageMode().
+
+        After using set_pixels(), you must call update_pixels() for your changes to
+        appear. This should be called once all pixels have been set, and must be
+        called before calling get_pixels() or drawing the image.
+
+        Setting the color of a single pixel with set_pixels(x, y) is easy, but not as
+        fast as putting the data directly into pixels[]. Setting the pixels[]
+        values directly may be complicated when working with a retina display, but
+        will perform better when lots of pixels need to be set directly on every
+        loop. See the reference for pixels[] for more information.
+        """
+        self._p5js.set(x, y, c)
+
+    def update_pixels(self):
+        """Updates the display window with the data in the pixels[] list.
+        Use in conjunction with loadPixels(). If you're only reading pixels from
+        the list, there's no need to call update_pixels() — updating is only
+        necessary to apply changes. update_pixels() should be called anytime the
+        pixels list is manipulated or set_pixels() is called, and only changes made with
+        set_pixels() or direct changes to pixels[] will occur.
+        """
+        self._p5js.updatePixels()
```

### Comparing `proceso-0.0.4/src/proceso/math/calculation.py` & `proceso-0.0.6/src/proceso/math/calculation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,162 +1,146 @@
 import math
 
-from .._binding import _p5js
+from .._binding import BaseSketch
 
 
-def abs(n: float) -> float:
-    """Calculates the absolute value (magnitude) of a number.
-    The absolute value of a number is always positive.
-    """
-    return _p5js.abs(n)
-
-
-def ceil(n: float) -> int:
-    """Calculates the closest int value that is greater than or equal to the
-    value of the parameter.
-    Maps to math.ceil(). For example, ceil(9.03) returns the value 10.
-    """
-    return math.ceil(n)
-
-
-def constrain(n: float, low: float, high: float) -> float:
-    """Constrains a value between a minimum and maximum value."""
-    return _p5js.constrain(n, low, high)
-
-
-def dist(x1: float, y1: float, x2: float, y2: float, *args) -> float:
-    """Calculates the distance between two points, in either two or three
-    dimensions.
-    """
-    return _p5js.dist(x1, y2, x2, y2, *args)
-
-
-def exp(n: float) -> float:
-    """Returns Euler's number e (2.71828...) raised to the power of the n
-    parameter.
-    Maps to math.exp().
-    """
-    return math.exp(n)
-
-
-def floor(n: float) -> int:
-    """Calculates the closest int value that is less than or equal to the
-    value of the parameter.
-    Maps to math.floor().
-    """
-    return math.floor(n)
-
-
-def lerp(start: float, stop: float, amt: float) -> float:
-    """Calculates a number between two numbers at a specific increment.
-    The amt parameter is the amount to interpolate between the two values
-    where 0.0 is equal to the first point, 0.1 is very near the first point,
-    0.5 is half-way in between, and 1.0 is equal to the second point. If the
-    value of amt is more than 1.0 or less than 0.0, the number will be
-    calculated accordingly in the ratio of the two given numbers. The lerp()
-    function is convenient for creating motion along a straight path and for
-    drawing dotted lines.
-    """
-    return _p5js.lerp(start, stop, amt)
-
-
-def log(n: float) -> float:
-    """Calculates the natural logarithm (the base-e logarithm) of a number.
-    This function expects the n parameter to be a value greater than 0.0.
-    Maps to math.log().
-    """
-    return math.log(n)
-
-
-def mag(a: float, b: float) -> float:
-    """Calculates the magnitude (or length) of a vector.
-    A vector is a direction in space commonly used in computer graphics and
-    linear algebra. Because it has no "start" position, the magnitude of a
-    vector can be thought of as the distance from the coordinate 0,0 to its
-    x,y value. Therefore, mag() is a shortcut for writing dist(0, 0, x, y).
-    """
-    return dist(0, 0, a, b)
-
-
-def remap(
-    value: float,
-    start1: float,
-    stop1: float,
-    start2: float,
-    stop2: float,
-    within_bounds: bool | None = None,
-):
-    """Re-maps a number from one range to another.
-
-    In the first example above, the number 25 is converted from a value in
-    the range of 0 to 100 into a value that ranges from the left edge of the
-    window (0) to the right edge (width).
-    """
-    return _p5js.map(value, start1, stop1, start2, stop2, within_bounds)
-
-
-def max(n: float | list[float], n1: float | None = None) -> float:
-    """Determines the largest value in a sequence of numbers, and then
-    returns that value.
-    max() accepts any number of float parameters, or a list of any length.
-    """
-    if n1:
-        return _p5js.max(n, n1)
-    return _p5js.max(n)
-
-
-def min(n: float | list[float], n1: float | None = None) -> float:
-    """Determines the smallest value in a sequence of numbers, and then
-    returns that value.
-    min() accepts any number of float parameters, or a list of any length.
-    """
-    if n1:
-        return _p5js.min(n, n1)
-    return _p5js.min(n)
-
-
-def norm(value: float, start: float, stop: float) -> float:
-    """Normalizes a number from another range into a value between 0 and 1.
-    Identical to map(value, low, high, 0, 1). Numbers outside of the range are
-    not clamped to 0 and 1, because out-of-range values are often intentional
-    and useful. (See the example above.)
-    """
-    return _p5js.norm(value, start, stop)
-
-
-def pow(n: float, e: float) -> float:
-    """Facilitates exponential expressions.
-    The pow() function is an efficient way of multiplying numbers by
-    themselves (or their reciprocals) in large quantities. For example,
-    pow(3, 5) is equivalent to the expression 3 × 3 × 3 × 3 × 3 and pow(3, -5)
-    is equivalent to 1 / 3 × 3 × 3 × 3 × 3. Maps to math.pow().
-    """
-    return math.pow(n, e)
-
-
-def round(n: float, decimals: int | None = None) -> float:
-    """Calculates the integer closest to the n parameter.
-    For example, round(133.8) returns the value 134.
-    """
-    return _p5js.round(n, decimals)
-
-
-def sq(n: float) -> float:
-    """Squares a number (multiplies a number by itself).
-    The result is always a positive number, as multiplying two negative
-    numbers always yields a positive result. For example, -1 * -1 = 1.
-    """
-    return n * n
-
-
-def sqrt(n: float) -> float:
-    """Squares a number (multiplies a number by itself).
-    The result is always a positive number, as multiplying two negative
-    numbers always yields a positive result. For example, -1 * -1 = 1.
-    """
-    return math.sqrt(n)
-
-
-def fract(n: float) -> float:
-    """Calculates the fractional part of a number."""
-    return _p5js.fract(n)
-
+class Calculation(BaseSketch):
+    def abs(self, n: float) -> float:
+        """Calculates the absolute value (magnitude) of a number.
+        The absolute value of a number is always positive.
+        """
+        return self._p5js.abs(n)
+
+    def ceil(self, n: float) -> int:
+        """Calculates the closest int value that is greater than or equal to the
+        value of the parameter.
+        Maps to math.ceil(). For example, ceil(9.03) returns the value 10.
+        """
+        return math.ceil(n)
+
+    def constrain(self, n: float, low: float, high: float) -> float:
+        """Constrains a value between a minimum and maximum value."""
+        return self._p5js.constrain(n, low, high)
+
+    def dist(self, x1: float, y1: float, x2: float, y2: float, *args) -> float:
+        """Calculates the distance between two points, in either two or three
+        dimensions.
+        """
+        return self._p5js.dist(x1, y2, x2, y2, *args)
+
+    def exp(self, n: float) -> float:
+        """Returns Euler's number e (2.71828...) raised to the power of the n
+        parameter.
+        Maps to math.exp().
+        """
+        return math.exp(n)
+
+    def floor(self, n: float) -> int:
+        """Calculates the closest int value that is less than or equal to the
+        value of the parameter.
+        Maps to math.floor().
+        """
+        return math.floor(n)
+
+    def lerp(self, start: float, stop: float, amt: float) -> float:
+        """Calculates a number between two numbers at a specific increment.
+        The amt parameter is the amount to interpolate between the two values
+        where 0.0 is equal to the first point, 0.1 is very near the first point,
+        0.5 is half-way in between, and 1.0 is equal to the second point. If the
+        value of amt is more than 1.0 or less than 0.0, the number will be
+        calculated accordingly in the ratio of the two given numbers. The lerp()
+        function is convenient for creating motion along a straight path and for
+        drawing dotted lines.
+        """
+        return self._p5js.lerp(start, stop, amt)
+
+    def log(self, n: float) -> float:
+        """Calculates the natural logarithm (the base-e logarithm) of a number.
+        This function expects the n parameter to be a value greater than 0.0.
+        Maps to math.log().
+        """
+        return math.log(n)
+
+    def mag(self, a: float, b: float) -> float:
+        """Calculates the magnitude (or length) of a vector.
+        A vector is a direction in space commonly used in computer graphics and
+        linear algebra. Because it has no "start" position, the magnitude of a
+        vector can be thought of as the distance from the coordinate 0,0 to its
+        x,y value. Therefore, mag() is a shortcut for writing dist(0, 0, x, y).
+        """
+        return dist(0, 0, a, b)
+
+    def remap(
+        self,
+        value: float,
+        start1: float,
+        stop1: float,
+        start2: float,
+        stop2: float,
+        within_bounds: bool | None = None,
+    ):
+        """Re-maps a number from one range to another.
+
+        In the first example above, the number 25 is converted from a value in
+        the range of 0 to 100 into a value that ranges from the left edge of the
+        window (0) to the right edge (width).
+        """
+        return self._p5js.map(value, start1, stop1, start2, stop2, within_bounds)
+
+    def max(self, n: float | list[float], n1: float | None = None) -> float:
+        """Determines the largest value in a sequence of numbers, and then
+        returns that value.
+        max() accepts any number of float parameters, or a list of any length.
+        """
+        if n1:
+            return self._p5js.max(n, n1)
+        return self._p5js.max(n)
+
+    def min(self, n: float | list[float], n1: float | None = None) -> float:
+        """Determines the smallest value in a sequence of numbers, and then
+        returns that value.
+        min() accepts any number of float parameters, or a list of any length.
+        """
+        if n1:
+            return self._p5js.min(n, n1)
+        return self._p5js.min(n)
+
+    def norm(self, value: float, start: float, stop: float) -> float:
+        """Normalizes a number from another range into a value between 0 and 1.
+        Identical to map(value, low, high, 0, 1). Numbers outside of the range are
+        not clamped to 0 and 1, because out-of-range values are often intentional
+        and useful. (See the example above.)
+        """
+        return self._p5js.norm(value, start, stop)
+
+    def pow(self, n: float, e: float) -> float:
+        """Facilitates exponential expressions.
+        The pow() function is an efficient way of multiplying numbers by
+        themselves (or their reciprocals) in large quantities. For example,
+        pow(3, 5) is equivalent to the expression 3 × 3 × 3 × 3 × 3 and pow(3, -5)
+        is equivalent to 1 / 3 × 3 × 3 × 3 × 3. Maps to math.pow().
+        """
+        return math.pow(n, e)
+
+    def round(self, n: float, decimals: int | None = None) -> float:
+        """Calculates the integer closest to the n parameter.
+        For example, round(133.8) returns the value 134.
+        """
+        return self._p5js.round(n, decimals)
+
+    def sq(self, n: float) -> float:
+        """Squares a number (multiplies a number by itself).
+        The result is always a positive number, as multiplying two negative
+        numbers always yields a positive result. For example, -1 * -1 = 1.
+        """
+        return n * n
+
+    def sqrt(self, n: float) -> float:
+        """Squares a number (multiplies a number by itself).
+        The result is always a positive number, as multiplying two negative
+        numbers always yields a positive result. For example, -1 * -1 = 1.
+        """
+        return math.sqrt(n)
+
+    def fract(self, n: float) -> float:
+        """Calculates the fractional part of a number."""
+        return self._p5js.fract(n)
```

### Comparing `proceso-0.0.4/src/proceso/math/noise.py` & `proceso-0.0.6/src/proceso/math/noise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,62 @@
-from .._binding import _p5js
+from .._binding import BaseSketch
 
 
-def noise(x: float, y: float | None = None, z: float | None = None) -> float:
-    """Returns the Perlin noise value at specified coordinates.
-    Perlin noise is a random sequence generator producing a more naturally
-    ordered, harmonic succession of numbers compared to the standard random()
-    function. It was invented by Ken Perlin in the 1980s and been used since
-    in graphical applications to produce procedural textures, natural motion,
-    shapes, terrains etc.
-
-    The main difference to the random() function is that Perlin noise is
-    defined in an infinite n-dimensional space where each pair of coordinates
-    corresponds to a fixed semi-random value (fixed only for the lifespan of
-    the program; see the noise_seed() function). p5.js can compute 1D, 2D and
-    3D noise, depending on the number of coordinates given. The resulting
-    value will always be between 0.0 and 1.0. The noise value can be animated
-    by moving through the noise space as demonstrated in the example above.
-    The 2nd and 3rd dimensions can also be interpreted as time.
-
-    The actual noise is structured similar to an audio signal, in respect to
-    the function's use of frequencies. Similar to the concept of harmonics in
-    physics, Perlin noise is computed over several octaves which are added
-    together for the final result.
-
-    Another way to adjust the character of the resulting sequence is the scale
-    of the input coordinates. As the function works within an infinite space
-    the value of the coordinates doesn't matter as such, only the distance
-    between successive coordinates does (eg. when using noise() within a
-    loop). As a general rule the smaller the difference between coordinates,
-    the smoother the resulting noise sequence will be. Steps of 0.005-0.03
-    work best for most applications, but this will differ depending on use.
-    """
-    return _p5js.noise(x, y, z)
-
-
-def noise_detail(lod: float, falloff: float):
-    """Adjusts the character and level of detail produced by the Perlin noise
-    function.
-    Similar to harmonics in physics, noise is computed over several octaves.
-    Lower octaves contribute more to the output signal and as such define the
-    overall intensity of the noise, whereas higher octaves create
-    finer-grained details in the noise sequence. By default, noise is
-    computed over 4 octaves with each octave contributing exactly half as much
-    as its predecessor, starting at 50% strength for the 1st octave. This
-    falloff amount can be changed by adding an additional function parameter.
-    Eg. a falloff factor of 0.75 means each octave will now have 75% impact
-    (25% less) of the previous lower octave. Any value between 0.0 and 1.0 is
-    valid, however, note that values greater than 0.5 might result in greater
-    than 1.0 values returned by noise(). By changing these parameters, the
-    signal created by the noise() function can be adapted to fit very
-    specific needs and characteristics.
-    """
-    _p5js.noiseDetail(lod, falloff)
-
-
-def noise_seed(seed: float):
-    """Sets the seed value for noise().
-    By default, noise() produces different results each time the program is
-    run. Set the seed parameter to a constant to return the same
-    pseudo-random numbers each time the software is run.
-    """
-    _p5js.noiseSeed(seed)
+class Noise(BaseSketch):
+    def noise(self, x: float, y: float | None = None, z: float | None = None) -> float:
+        """Returns the Perlin noise value at specified coordinates.
+        Perlin noise is a random sequence generator producing a more naturally
+        ordered, harmonic succession of numbers compared to the standard random()
+        function. It was invented by Ken Perlin in the 1980s and been used since
+        in graphical applications to produce procedural textures, natural motion,
+        shapes, terrains etc.
+
+        The main difference to the random() function is that Perlin noise is
+        defined in an infinite n-dimensional space where each pair of coordinates
+        corresponds to a fixed semi-random value (fixed only for the lifespan of
+        the program; see the noise_seed() function). p5.js can compute 1D, 2D and
+        3D noise, depending on the number of coordinates given. The resulting
+        value will always be between 0.0 and 1.0. The noise value can be animated
+        by moving through the noise space as demonstrated in the example above.
+        The 2nd and 3rd dimensions can also be interpreted as time.
+
+        The actual noise is structured similar to an audio signal, in respect to
+        the function's use of frequencies. Similar to the concept of harmonics in
+        physics, Perlin noise is computed over several octaves which are added
+        together for the final result.
+
+        Another way to adjust the character of the resulting sequence is the scale
+        of the input coordinates. As the function works within an infinite space
+        the value of the coordinates doesn't matter as such, only the distance
+        between successive coordinates does (eg. when using noise() within a
+        loop). As a general rule the smaller the difference between coordinates,
+        the smoother the resulting noise sequence will be. Steps of 0.005-0.03
+        work best for most applications, but this will differ depending on use.
+        """
+        return self._p5js.noise(x, y, z)
+
+    def noise_detail(self, lod: float, falloff: float):
+        """Adjusts the character and level of detail produced by the Perlin noise
+        function.
+        Similar to harmonics in physics, noise is computed over several octaves.
+        Lower octaves contribute more to the output signal and as such define the
+        overall intensity of the noise, whereas higher octaves create
+        finer-grained details in the noise sequence. By default, noise is
+        computed over 4 octaves with each octave contributing exactly half as much
+        as its predecessor, starting at 50% strength for the 1st octave. This
+        falloff amount can be changed by adding an additional function parameter.
+        Eg. a falloff factor of 0.75 means each octave will now have 75% impact
+        (25% less) of the previous lower octave. Any value between 0.0 and 1.0 is
+        valid, however, note that values greater than 0.5 might result in greater
+        than 1.0 values returned by noise(). By changing these parameters, the
+        signal created by the noise() function can be adapted to fit very
+        specific needs and characteristics.
+        """
+        self._p5js.noiseDetail(lod, falloff)
+
+    def noise_seed(self, seed: float):
+        """Sets the seed value for noise().
+        By default, noise() produces different results each time the program is
+        run. Set the seed parameter to a constant to return the same
+        pseudo-random numbers each time the software is run.
+        """
+        self._p5js.noiseSeed(seed)
```

### Comparing `proceso-0.0.4/src/proceso/math/random.py` & `proceso-0.0.6/src/proceso/math/random.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import random as rnd
 
 
-def random_seed(seed: float):
-    """Sets the seed value for random().
-
-    By default, random() produces different results each time the program is
-    run. Set the seed parameter to a constant to return the same
-    pseudo-random numbers each time the software is run.
-    """
-    rnd.seed(seed)
-
-
-def random(min: float, max: float | None = None) -> float:
-    """Return a random floating-point number.
-
-    Takes either 1 or 2 arguments.
-
-    If one argument is given and it is a number, returns a random number from
-    0 up to (but not including) the number.
-
-    If two arguments are given, returns a random number from the first
-    argument up to (but not including) the second argument.
-    """
-    if max:
-        return rnd.uniform(min, max)
-    else:
-        return rnd.uniform(0, min)
-
-
-def random_gaussian(mean: float | None = None, sd: float | None = None) -> float:
-    """Returns a random number fitting a Gaussian, or normal, distribution.
-    There is theoretically no minimum or maximum value that random_gaussian()
-    might return. Rather, there is just a very low probability that values far
-    from the mean will be returned; and a higher probability that numbers near
-    the mean will be returned. Takes either 0, 1 or 2 arguments.
-    If no args, the mean is 0 and the standard deviation is 1.
-    If one arg, that arg is the mean and the standard deviation is 1.
-    If two args, the first arg is the mean and the second is the standard
-    deviation.
-    """
-    return rnd.gauss(mean, sd)
+class Random:
+    def random_seed(self, seed: float):
+        """Sets the seed value for random().
+
+        By default, random() produces different results each time the program is
+        run. Set the seed parameter to a constant to return the same
+        pseudo-random numbers each time the software is run.
+        """
+        rnd.seed(seed)
+
+    def random(self, min: float, max: float | None = None) -> float:
+        """Return a random floating-point number.
+
+        Takes either 1 or 2 arguments.
+
+        If one argument is given and it is a number, returns a random number from
+        0 up to (but not including) the number.
+
+        If two arguments are given, returns a random number from the first
+        argument up to (but not including) the second argument.
+        """
+        if max:
+            return rnd.uniform(min, max)
+        else:
+            return rnd.uniform(0, min)
+
+    def random_gaussian(
+        self, mean: float | None = None, sd: float | None = None
+    ) -> float:
+        """Returns a random number fitting a Gaussian, or normal, distribution.
+        There is theoretically no minimum or maximum value that random_gaussian()
+        might return. Rather, there is just a very low probability that values far
+        from the mean will be returned; and a higher probability that numbers near
+        the mean will be returned. Takes either 0, 1 or 2 arguments.
+        If no args, the mean is 0 and the standard deviation is 1.
+        If one arg, that arg is the mean and the standard deviation is 1.
+        If two args, the first arg is the mean and the second is the standard
+        deviation.
+        """
+        return rnd.gauss(mean, sd)
```

### Comparing `proceso-0.0.4/src/proceso/math/trigonometry.py` & `proceso-0.0.6/src/proceso/math/trigonometry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,90 @@
-from .._binding import _p5js
+from .._binding import BaseSketch
 
 
-def acos(value: float) -> float:
-    """The inverse of cos(), returns the arc cosine of a value.
-    This function expects the values in the range of -1 to 1 and values are
-    returned in the range 0 to PI (3.1415927) if the angle_mode() is RADIANS
-    or 0 to 180 if the angle_mode() is DEGREES.
-    """
-    return _p5js.acos(value)
-
-
-def asin(value: float) -> float:
-    """The inverse of sin(), returns the arc sine of a value.
-    This function expects the values in the range of -1 to 1 and values are
-    returned in the range -PI/2 to PI/2 if the angle_mode is RADIANS or -90 to
-    90 if the angle mode is DEGREES.
-    """
-    return _p5js.asin(value)
-
-
-def atan(value: float) -> float:
-    """The inverse of tan(), returns the arc tangent of a value.
-    This function expects the values in the range of -Infinity to Infinity
-    (exclusive) and values are returned in the range -PI/2 to PI/2 if the
-    angle_mode is RADIANS or -90 to 90 if the angle_mode is DEGREES.
-    """
-    return _p5js.atan(value)
-
-
-def atan2(y, x) -> float:
-    """Calculates the angle (in radians) from a specified point to the
-    coordinate origin as measured from the positive x-axis.
-    Values are returned as a float in the range from PI to -PI if the
-    angle_mode() is RADIANS or 180 to -180 if the angle_mode() is DEGREES.
-    The atan2() function is most often used for orienting geometry to the
-    position of the cursor.
-
-    Note: The y-coordinate of the point is the first parameter, and the
-    x-coordinate is the second parameter, due to the structure of calculating
-    the tangent.
-    """
-    return _p5js.atan2(y, x)
-
-
-def cos(value: float) -> float:
-    """Calculates the cosine of an angle.
-    This function takes into account the current angle_mode. Values are
-    returned in the range -1 to 1.
-    """
-    return _p5js.cos(value)
-
-
-def sin(value: float) -> float:
-    """Calculates the sine of an angle.
-    This function takes into account the current angle_mode. Values are
-    returned in the range -1 to 1.
-    """
-    return _p5js.sin(value)
-
-
-def tan(value: float) -> float:
-    """Calculates the tangent of an angle.
-    This function takes into account the current angle_mode. Values are
-    returned in the range of all real numbers.
-    """
-    return _p5js.tan(value)
-
-
-def degrees(radians: float) -> float:
-    """Converts a radian measurement to its corresponding value in degrees.
-    Radians and degrees are two ways of measuring the same thing. There are
-    360 degrees in a circle and 2*PI radians in a circle. For example,
-    90° = PI/2 = 1.5707964. This function does not take into account the
-    current angle_mode.
-    """
-    return _p5js.degrees(radians)
-
-
-def radians(degrees: float) -> float:
-    """Converts a degree measurement to its corresponding value in radians.
-    Radians and degrees are two ways of measuring the same thing. There are
-    360 degrees in a circle and 2*PI radians in a circle. For example,
-    90° = PI/2 = 1.5707964. This function does not take into account the
-    current angle_mode.
-    """
-    return _p5js.radians(degrees)
-
-
-def angle_mode(mode: str | None = None) -> None | str:
-    """Sets the current mode of p5 to the given mode.
-    Default mode is RADIANS.
-
-    Calling angle_mode() with no arguments returns current angle_mode.
-    """
-    if not mode:
-        return _p5js.angleMode()
-    _p5js.angleMode(mode)
+class Trigonometry(BaseSketch):
+    def acos(self, value: float) -> float:
+        """The inverse of cos(), returns the arc cosine of a value.
+        This function expects the values in the range of -1 to 1 and values are
+        returned in the range 0 to PI (3.1415927) if the angle_mode() is RADIANS
+        or 0 to 180 if the angle_mode() is DEGREES.
+        """
+        return self._p5js.acos(value)
+
+    def asin(self, value: float) -> float:
+        """The inverse of sin(), returns the arc sine of a value.
+        This function expects the values in the range of -1 to 1 and values are
+        returned in the range -PI/2 to PI/2 if the angle_mode is RADIANS or -90 to
+        90 if the angle mode is DEGREES.
+        """
+        return self._p5js.asin(value)
+
+    def atan(self, value: float) -> float:
+        """The inverse of tan(), returns the arc tangent of a value.
+        This function expects the values in the range of -Infinity to Infinity
+        (exclusive) and values are returned in the range -PI/2 to PI/2 if the
+        angle_mode is RADIANS or -90 to 90 if the angle_mode is DEGREES.
+        """
+        return self._p5js.atan(value)
+
+    def atan2(self, y, x) -> float:
+        """Calculates the angle (in radians) from a specified point to the
+        coordinate origin as measured from the positive x-axis.
+        Values are returned as a float in the range from PI to -PI if the
+        angle_mode() is RADIANS or 180 to -180 if the angle_mode() is DEGREES.
+        The atan2() function is most often used for orienting geometry to the
+        position of the cursor.
+
+        Note: The y-coordinate of the point is the first parameter, and the
+        x-coordinate is the second parameter, due to the structure of calculating
+        the tangent.
+        """
+        return self._p5js.atan2(y, x)
+
+    def cos(self, value: float) -> float:
+        """Calculates the cosine of an angle.
+        This function takes into account the current angle_mode. Values are
+        returned in the range -1 to 1.
+        """
+        return self._p5js.cos(value)
+
+    def sin(self, value: float) -> float:
+        """Calculates the sine of an angle.
+        This function takes into account the current angle_mode. Values are
+        returned in the range -1 to 1.
+        """
+        return self._p5js.sin(value)
+
+    def tan(self, value: float) -> float:
+        """Calculates the tangent of an angle.
+        This function takes into account the current angle_mode. Values are
+        returned in the range of all real numbers.
+        """
+        return self._p5js.tan(value)
+
+    def degrees(self, radians: float) -> float:
+        """Converts a radian measurement to its corresponding value in degrees.
+        Radians and degrees are two ways of measuring the same thing. There are
+        360 degrees in a circle and 2*PI radians in a circle. For example,
+        90° = PI/2 = 1.5707964. This function does not take into account the
+        current angle_mode.
+        """
+        return self._p5js.degrees(radians)
+
+    def radians(self, degrees: float) -> float:
+        """Converts a degree measurement to its corresponding value in radians.
+        Radians and degrees are two ways of measuring the same thing. There are
+        360 degrees in a circle and 2*PI radians in a circle. For example,
+        90° = PI/2 = 1.5707964. This function does not take into account the
+        current angle_mode.
+        """
+        return self._p5js.radians(degrees)
+
+    def angle_mode(self, mode: str | None = None) -> None | str:
+        """Sets the current mode of p5 to the given mode.
+        Default mode is RADIANS.
+
+        Calling angle_mode() with no arguments returns current angle_mode.
+        """
+        if not mode:
+            return self._p5js.angleMode()
+        self._p5js.angleMode(mode)
```

### Comparing `proceso-0.0.4/src/proceso/math/vector.py` & `proceso-0.0.6/src/proceso/math/vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #   along with this library. If not, see <https://www.gnu.org/licenses/>.
 #
 # *****************************************************************************
 from __future__ import annotations
 import operator
 from collections.abc import Sequence, Iterable
 import re
+import warnings
 
 import numpy as np
 
 
 class Vector(Sequence):
     """Class to describe a 2D, 3D, or 4D vector.
 
@@ -747,17 +748,15 @@
         Notes
         -----
 
         The vector's magnitude. Setting this property to a non-negative number will
         adjust the vector's magnitude to that value. Negative values will result in an
         error.
         """
-        if mag < 0:
-            raise RuntimeError("Cannot set magnitude to a negative number")
-        elif mag == 0:
+        if mag == 0:
             self._data[:] = 0
         else:
             self.normalize()
             self._data *= mag
         return self
 
     def _get_mag_sq(self) -> float:
@@ -802,15 +801,17 @@
         normalized.
         """
         mag = np.sum(self._data**2) ** 0.5
         if mag > 0:
             self._data /= mag
             return self
         else:
-            raise RuntimeError("Cannot normalize Vector of zeros")
+            warnings.warn(
+                "Using normalize on a zero vector has no effect", stacklevel=2
+            )
 
     def _get_norm(self) -> Vector:
         """Normalized copy of the vector.
 
         Notes
         -----
```

### Comparing `proceso-0.0.4/src/proceso/rendering.py` & `proceso-0.0.6/src/proceso/rendering.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
 from typing import Any
 
-from ._binding import _p5js
-from .constants import P2D
+from ._binding import BaseSketch
 
 
-def create_canvas(width: int, height: int, renderer: str = P2D) -> object:
-    """Creates a canvas element in the document and sets its dimensions in
-    pixels. Alias of size().
-
-    This method should be called only once at the start of setup(). Calling
-    create_canvas() more than once in a sketch will result in very unpredictable
-    behavior. If you want more than one drawing canvas you could use
-    create_graphics() (hidden by default but it can be shown).
-
-    Important note: in 2D mode (i.e. when p5.Renderer is not set) the origin
-    (0,0) is positioned at the top left of the screen. In 3D mode (i.e. when
-    p5.Renderer is set to WEBGL), the origin is positioned at the center of
-    the canvas. See this issue for more information.
-
-    The system variables width and height are set by the parameters passed to
-    this function. If create_canvas() is not used, the window will be given a
-    default size of 100×100 pixels.
-    """
-    return _p5js.createCanvas(width, height, renderer)
-
-
-def size(width: int, height: int, renderer: str = P2D) -> object:
-    """Creates a canvas element in the document and sets its dimensions in
-    pixels. Alias of create_canvas().
-
-    This method should be called only once at the start of setup(). Calling
-    size() more than once in a sketch will result in very unpredictable
-    behavior. If you want more than one drawing canvas you could use
-    create_graphics() (hidden by default but it can be shown).
-
-    Important note: in 2D mode (i.e. when p5.Renderer is not set) the origin
-    (0,0) is positioned at the top left of the screen. In 3D mode (i.e. when
-    p5.Renderer is set to WEBGL), the origin is positioned at the center of
-    the canvas. See this issue for more information.
-
-    The system variables width and height are set by the parameters passed to
-    this function. If size() is not used, the window will be given a
-    default size of 100×100 pixels.
-    """
-    return _p5js.createCanvas(width, height, renderer)
-
-
-def resize_canvas(width: int, height: int, no_redraw: bool | None = None):
-    """Resizes the canvas to given width and height.
-    The canvas will be cleared and draw will be called immediately, allowing
-    the sketch to re-render itself in the resized canvas.
-    """
-    _p5js.resizeCanvas(width, height, no_redraw)
-
-
-def no_canvas():
-    """Removes the default canvas for a p5 sketch that doesn't require a
-    canvas.
-    """
-    _p5js.noCanvas()
-
-
-def create_graphics(width: int, height: int, renderer: str = P2D) -> object:
-    """Creates and returns a new p5.Renderer object.
-    Use this class if you need to draw into an off-screen graphics buffer. The
-    two parameters define the width and height in pixels.
-    """
-    return _p5js.createGraphics(width, height, renderer)
-
-
-def blend_mode(mode: str):
-    """Blends the pixels in the display window according to the defined mode.
-    There is a choice of the following modes to blend the source pixels (A)
-    with the ones of pixels already in the display window (B):
-
-    BLEND - linear interpolation of colours: C = A*factor + B. This is the
-    default blending mode.
-    ADD - sum of A and B
-    DARKEST - only the darkest colour succeeds: C = min(A*factor, B).
-    LIGHTEST - only the lightest colour succeeds: C = max(A*factor, B).
-    DIFFERENCE - subtract colors from underlying image. (2D)
-    EXCLUSION - similar to DIFFERENCE, but less extreme.
-    MULTIPLY - multiply the colors, result will always be darker.
-    SCREEN - opposite multiply, uses inverse values of the colors.
-    REPLACE - the pixels entirely replace the others and don't utilize alpha
-    (transparency) values.
-    REMOVE - removes pixels from B with the alpha strength of A.
-    OVERLAY - mix of MULTIPLY and SCREEN . Multiplies dark values, and screens
-    light values. (2D)
-    HARD_LIGHT - SCREEN when greater than 50% gray, MULTIPLY when lower. (2D)
-    SOFT_LIGHT - mix of DARKEST and LIGHTEST. Works like OVERLAY, but not as
-    harsh. (2D)
-    DODGE - lightens light tones and increases contrast, ignores darks. (2D)
-    BURN - darker areas are applied, increasing contrast, ignores lights. (2D)
-    SUBTRACT - remainder of A and B (3D)
-
-    (2D) indicates that this blend mode only works in the 2D renderer.
-    (3D) indicates that this blend mode only works in the WEBGL renderer.
-    """
-    _p5js.blendMode(mode)
-
-
-def set_attributes(key: str, value: Any):
-    """Set attributes for the WebGL Drawing context.
-    This is a way of adjusting how the WebGL renderer works to fine-tune the
-    display and performance.
-
-    Note that this will reinitialize the drawing context if called after the
-    WebGL canvas is made.
-
-    If an object is passed as the parameter, all attributes not declared in
-    the object will be set to defaults.
-
-    The available attributes are:
-    alpha - indicates if the canvas contains an alpha buffer default is True
-
-    depth - indicates whether the drawing buffer has a depth buffer of at
-    least 16 bits - default is True
-
-    stencil - indicates whether the drawing buffer has a stencil buffer of at
-    least 8 bits
-
-    antialias - indicates whether or not to perform anti-aliasing default is
-    False (True in Safari)
-
-    premultipliedAlpha - indicates that the page compositor will assume the
-    drawing buffer contains colors with pre-multiplied alpha default is True
-
-    preserveDrawingBuffer - if true the buffers will not be cleared and and
-    will preserve their values until cleared or overwritten by author
-    (note that p5 clears automatically on draw loop) default is True
-
-    perPixelLighting - if True, per-pixel lighting will be used in the
-    lighting shader otherwise per-vertex lighting is used. default is True.
-    """
-    _p5js.setAttributes(key, value)
+class Rendering(BaseSketch):
+    def create_canvas(
+        self, width: int, height: int, renderer: str | None = None
+    ) -> object:
+        """Creates a canvas element in the document and sets its dimensions in
+        pixels. Alias of size().
+
+        This method should be called only once at the start of setup(). Calling
+        create_canvas() more than once in a sketch will result in very unpredictable
+        behavior. If you want more than one drawing canvas you could use
+        create_graphics() (hidden by default but it can be shown).
+
+        Important note: in 2D mode (i.e. when p5.Renderer is not set) the origin
+        (0,0) is positioned at the top left of the screen. In 3D mode (i.e. when
+        p5.Renderer is set to WEBGL), the origin is positioned at the center of
+        the canvas. See this issue for more information.
+
+        The system variables width and height are set by the parameters passed to
+        this function. If create_canvas() is not used, the window will be given a
+        default size of 100×100 pixels.
+        """
+        self.width = width
+        self.height = height
+        return self._p5js.createCanvas(width, height, renderer)
+
+    def size(self, width: int, height: int, renderer: str | None = None) -> object:
+        """Creates a canvas element in the document and sets its dimensions in
+        pixels. Alias of create_canvas().
+
+        This method should be called only once at the start of setup(). Calling
+        size() more than once in a sketch will result in very unpredictable
+        behavior. If you want more than one drawing canvas you could use
+        create_graphics() (hidden by default but it can be shown).
+
+        Important note: in 2D mode (i.e. when p5.Renderer is not set) the origin
+        (0,0) is positioned at the top left of the screen. In 3D mode (i.e. when
+        p5.Renderer is set to WEBGL), the origin is positioned at the center of
+        the canvas. See this issue for more information.
+
+        The system variables width and height are set by the parameters passed to
+        this function. If size() is not used, the window will be given a
+        default size of 100×100 pixels.
+        """
+        return self._p5js.createCanvas(width, height, renderer)
+
+    def resize_canvas(self, width: int, height: int, no_redraw: bool | None = None):
+        """Resizes the canvas to given width and height.
+        The canvas will be cleared and draw will be called immediately, allowing
+        the sketch to re-render itself in the resized canvas.
+        """
+        self._p5js.resizeCanvas(width, height, no_redraw)
+
+    def no_canvas(self):
+        """Removes the default canvas for a p5 sketch that doesn't require a
+        canvas.
+        """
+        self._p5js.noCanvas()
+
+    def create_graphics(
+        self, width: int, height: int, renderer: str | None = None
+    ) -> object:
+        """Creates and returns a new p5.Renderer object.
+        Use this class if you need to draw into an off-screen graphics buffer. The
+        two parameters define the width and height in pixels.
+        """
+        return self._p5js.createGraphics(width, height, renderer)
+
+    def blend_mode(self, mode: str):
+        """Blends the pixels in the display window according to the defined mode.
+        There is a choice of the following modes to blend the source pixels (A)
+        with the ones of pixels already in the display window (B):
+
+        BLEND - linear interpolation of colours: C = A*factor + B. This is the
+        default blending mode.
+        ADD - sum of A and B
+        DARKEST - only the darkest colour succeeds: C = min(A*factor, B).
+        LIGHTEST - only the lightest colour succeeds: C = max(A*factor, B).
+        DIFFERENCE - subtract colors from underlying image. (2D)
+        EXCLUSION - similar to DIFFERENCE, but less extreme.
+        MULTIPLY - multiply the colors, result will always be darker.
+        SCREEN - opposite multiply, uses inverse values of the colors.
+        REPLACE - the pixels entirely replace the others and don't utilize alpha
+        (transparency) values.
+        REMOVE - removes pixels from B with the alpha strength of A.
+        OVERLAY - mix of MULTIPLY and SCREEN . Multiplies dark values, and screens
+        light values. (2D)
+        HARD_LIGHT - SCREEN when greater than 50% gray, MULTIPLY when lower. (2D)
+        SOFT_LIGHT - mix of DARKEST and LIGHTEST. Works like OVERLAY, but not as
+        harsh. (2D)
+        DODGE - lightens light tones and increases contrast, ignores darks. (2D)
+        BURN - darker areas are applied, increasing contrast, ignores lights. (2D)
+        SUBTRACT - remainder of A and B (3D)
+
+        (2D) indicates that this blend mode only works in the 2D renderer.
+        (3D) indicates that this blend mode only works in the WEBGL renderer.
+        """
+        self._p5js.blendMode(mode)
+
+    def set_attributes(self, key: str, value: Any):
+        """Set attributes for the WebGL Drawing context.
+        This is a way of adjusting how the WebGL renderer works to fine-tune the
+        display and performance.
+
+        Note that this will reinitialize the drawing context if called after the
+        WebGL canvas is made.
+
+        If an object is passed as the parameter, all attributes not declared in
+        the object will be set to defaults.
+
+        The available attributes are:
+        alpha - indicates if the canvas contains an alpha buffer default is True
+
+        depth - indicates whether the drawing buffer has a depth buffer of at
+        least 16 bits - default is True
+
+        stencil - indicates whether the drawing buffer has a stencil buffer of at
+        least 8 bits
+
+        antialias - indicates whether or not to perform anti-aliasing default is
+        False (True in Safari)
+
+        premultipliedAlpha - indicates that the page compositor will assume the
+        drawing buffer contains colors with pre-multiplied alpha default is True
+
+        preserveDrawingBuffer - if true the buffers will not be cleared and and
+        will preserve their values until cleared or overwritten by author
+        (note that p5 clears automatically on draw loop) default is True
+
+        perPixelLighting - if True, per-pixel lighting will be used in the
+        lighting shader otherwise per-vertex lighting is used. default is True.
+        """
+        self._p5js.setAttributes(key, value)
```

### Comparing `proceso-0.0.4/src/proceso/shape.py` & `proceso-0.0.6/src/proceso/shape.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,715 +1,692 @@
 from pyodide.ffi import to_js
 
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-# =============
-# 2D Primitives
-# =============
-def arc(
-    x: float,
-    y: float,
-    w: float,
-    h: float,
-    start: float,
-    stop: float,
-    mode: str | None = None,
-    detail: int = 25,
-):
-    """Draw an arc to the screen.
-    If called with only x, y, w, h, start and stop, the arc will be drawn and
-    filled as an open pie segment. If a mode parameter is provided, the arc
-    will be filled like an open semi-circle (OPEN), a closed semi-circle
-    (CHORD), or as a closed pie segment (PIE). The origin may be changed with
-    the ellipse_mode() function.
-
-    The arc is always drawn clockwise from wherever start falls to wherever
-    stop falls on the ellipse. Adding or subtracting TWO_PI to either angle
-    does not change where they fall. If both start and stop fall at the same
-    place, a full ellipse will be drawn. Be aware that the y-axis increases in
-    the downward direction, therefore angles are measured clockwise from the
-    positive x-direction ("3 o'clock").
-    """
-    _p5js.arc(x, y, w, h, start, stop, to_js(mode), detail)
-
-
-def ellipse(x: float, y: float, w: float, h: float | None = None, detail: int = 25):
-    """Draws an ellipse (oval) to the screen.
-    By default, the first two parameters set the location of the center of the
-    ellipse, and the third and fourth parameters set the shape's width and
-    height. If no height is specified, the value of width is used for both the
-    width and height. If a negative height or width is specified, the absolute
-    value is taken.
-
-    An ellipse with equal width and height is a circle. The origin may be
-    changed with the ellipse_mode() function.
-    """
-    _p5js.ellipse(x, y, w, h, detail)
-
-
-def circle(x: float, y: float, d: float):
-    """Draws a circle to the screen.
-    A circle is a simple closed shape. It is the set of all points in a plane
-    that are at a given distance from a given point, the center. This function
-    is a special case of the ellipse() function, where the width and height of
-    the ellipse are the same. Height and width of the ellipse correspond to
-    the diameter of the circle. By default, the first two parameters set the
-    location of the center of the circle, the third sets the diameter of the
-    circle.
-    """
-    _p5js.circle(x, y, d)
-
-
-def line(x1: float, y1: float, x2: float, y2: float, *args):
-    """Draws a line (a direct path between two points) to the screen.
-    If called with only 4 parameters, it will draw a line in 2D with a default
-    width of 1 pixel. This width can be modified by using the stroke_weight()
-    function. A line cannot be filled, therefore the fill() function will not
-    affect the color of a line. So to color a line, use the stroke() function.
-    """
-    _p5js.line(x1, y1, x2, y2, *args)
-
-
-def point(x: float, y: float, z: float | None = None):
-    """Draws a point, a coordinate in space at the dimension of one pixel.
-    The first parameter is the horizontal value for the point, the second
-    param is the vertical value for the point. The color of the point is
-    changed with the stroke() function. The size of the point can be changed
-    with the stroke_weight() function.
-    """
-    _p5js.point(x, y, z)
-
-
-def quad(
-    x1: float,
-    y1: float,
-    x2: float,
-    y2: float,
-    x3: float,
-    y3: float,
-    x4: float,
-    y4: float,
-    detail_x: int | None = None,
-    detail_y: int | None = None,
-    *args,
-):
-    """Draws a quad on the canvas.
-    A quad is a quadrilateral, a four-sided polygon. It is similar to a
-    rectangle, but the angles between its edges are not constrained to ninety
-    degrees. The first pair of parameters (x1,y1) sets the first vertex and
-    the subsequent pairs should proceed clockwise or counter-clockwise around
-    the defined shape. z-arguments only work when quad() is used in WEBGL
-    mode.
-    """
-    _p5js.quad(x1, y1, x2, y2, x3, y3, x4, y4, detail_x, detail_y, *args)
-
-
-def rect(
-    x: float,
-    y: float,
-    w: float,
-    h: float,
-    r: float | None = None,
-    tr: float | None = None,
-    br: float | None = None,
-    bl: float | None = None,
-):
-    """Draws a rectangle on the canvas.
-    A rectangle is a four-sided closed shape with every angle at ninety
-    degrees. By default, the first two parameters set the location of the
-    upper-left corner, the third sets the width, and the fourth sets the
-    height. The way these parameters are interpreted may be changed with the
-    rect_mode() function.
-
-    The fifth, sixth, seventh and eighth parameters, if specified, determine
-    corner radius for the top-left, top-right, lower-right and lower-left
-    corners, respectively. An omitted corner radius parameter is set to the
-    value of the previously specified radius value in the parameter list.
-    """
-    _p5js.rect(x, y, w, h, r, tr, br, bl)
-
-
-def square(
-    x: float,
-    y: float,
-    s: float,
-    tl: float | None = None,
-    tr: float | None = None,
-    br: float | None = None,
-    bl: float | None = None,
-):
-    """Draws a square to the screen.
-    A square is a four-sided shape with every angle at ninety degrees, and
-    equal side size. This function is a special case of the rect() function,
-    where the width and height are the same, and the parameter is called "s"
-    for side size. By default, the first two parameters set the location of
-    the upper-left corner, the third sets the side size of the square. The way
-    these parameters are interpreted, may be changed with the rect_mode()
-    function.
-
-    The fourth, fifth, sixth and seventh parameters, if specified, determine
-    corner radius for the top-left, top-right, lower-right and lower-left
-    corners, respectively. An omitted corner radius parameter is set to the
-    value of the previously specified radius value in the parameter list.
-    """
-    _p5js.square(x, y, s, tl, tr, br, bl)
-
-
-def triangle(x1: float, y1: float, x2: float, y2: float, x3: float, y3: float):
-    """Draws a triangle to the canvas.
-    A triangle is a plane created by connecting three points. The first two
-    arguments specify the first point, the middle two arguments specify the
-    second point, and the last two arguments specify the third point.
-    """
-    _p5js.triangle(x1, y1, x2, y2, x3, y3)
-
-
-# ==========
-# Attributes
-# ==========
-def ellipse_mode(mode: str):
-    """Modifies the location from which ellipses are drawn by changing the way
-    in which parameters given to ellipse(), circle() and arc() are
-    interpreted.
-
-    The default mode is CENTER, in which the first two parameters are
-    interpreted as the shape's center point's x and y coordinates
-    respectively, while the third and fourth parameters are its width and
-    height.
-
-    ellipse_mode(RADIUS) also uses the first two parameters as the shape's
-    center point's x and y coordinates, but uses the third and fourth
-    parameters to specify half of the shapes's width and height.
-
-    ellipse_mode(CORNER) interprets the first two parameters as the upper-left
-    corner of the shape, while the third and fourth parameters are its width
-    and height.
-
-    ellipse_mode(CORNERS) interprets the first two parameters as the location
-    of one corner of the ellipse's bounding box, and the third and fourth
-    parameters as the location of the opposite corner.
-
-    The parameter to this function must be written in ALL CAPS because they
-    are predefined as constants in ALL CAPS and Python is a case-sensitive
-    language.
-    """
-    _p5js.ellipseMode(mode)
-
-
-def no_smooth():
-    """Draws all geometry with jagged (aliased) edges.
-
-    Note that smooth() is active by default in 2D mode, so it is necessary to
-    call no_smooth() to disable smoothing of geometry, images, and fonts.
-
-    In 3D mode, no_smooth() is enabled by default, so it is necessary to call
-    smooth() if you would like smooth (antialiased) edges on your geometry.
-    """
-    _p5js.noSmooth()
-
-
-def rect_mode(mode: str):
-    """Modifies the location from which rectangles are drawn by changing the
-    way in which parameters given to rect() are interpreted.
-
-    The default mode is CORNER, which interprets the first two parameters as
-    the upper-left corner of the shape, while the third and fourth parameters
-    are its width and height.
-
-    rectMode(CORNERS) interprets the first two parameters as the location of
-    one of the corners, and the third and fourth parameters as the location
-    of the diagonally opposite corner. Note, the rectangle is drawn between
-    the coordinates, so it is not necessary that the first corner be the
-    upper left corner.
-
-    rectMode(CENTER) interprets the first two parameters as the shape's center
-    point, while the third and fourth parameters are its width and height.
-
-    rectMode(RADIUS) also uses the first two parameters as the shape's center
-    point, but uses the third and fourth parameters to specify half of the
-    shape's width and height respectively.
-
-    The parameter to this function must be written in ALL CAPS because they
-    are predefined as constants in ALL CAPS and Python is a case-sensitive
-    language.
-    """
-    _p5js.rectMode(mode)
-
-
-def smooth():
-    """Draws all geometry with smooth (anti-aliased) edges.
-    smooth() will also improve image quality of resized images.
-
-    Note that smooth() is active by default in 2D mode; no_smooth() can be
-    used to disable smoothing of geometry, images, and fonts.
-
-    In 3D mode, no_smooth() is enabled by default, so it is necessary to call
-    smooth() if you would like smooth (antialiased) edges on your geometry.
-    """
-    _p5js.smooth()
-
-
-def stroke_cap(cap: str):
-    """Sets the style for rendering line endings.
-    These ends are either rounded, squared, or extended, each of which
-    specified with the corresponding parameters: ROUND, SQUARE, or PROJECT.
-    The default cap is ROUND.
-
-    The parameter to this function must be written in ALL CAPS because they
-    are predefined as constants in ALL CAPS and Python is a case-sensitive
-    language.
-    """
-    _p5js.strokeCap(cap)
-
-
-def stroke_join(join: str):
-    """Sets the style of the joints which connect line segments.
-    These joints are either mitered, beveled, or rounded and specified with
-    the corresponding parameters: MITER, BEVEL, or ROUND. The default joint is
-    MITER in 2D mode and ROUND in WebGL mode.
-
-    The parameter to this function must be written in ALL CAPS because they
-    are predefined as constants in ALL CAPS and Python is a case-sensitive
-    language.
-    """
-    _p5js.strokeJoin(join)
-
-
-def stroke_weight(weight: float):
-    """Sets the width of the stroke used for lines, points, and the border
-    around shapes.
-    All widths are set in units of pixels.
-
-    Note that it is affected by any transformation or scaling that has been
-    applied previously.
-    """
-    _p5js.strokeWeight(weight)
-
-
-# ======
-# Curves
-# ======
-def bezier(
-    x1: float,
-    y1: float,
-    x2: float,
-    y2: float,
-    x3: float,
-    y3: float,
-    x4: float,
-    y4: float,
-    *args,
-):
-    """Draws a cubic Bezier curve on the screen.
-    These curves are defined by a series of anchor and control points. The
-    first two parameters specify the first anchor point and the last two
-    parameters specify the other anchor point, which become the first and
-    last points on the curve. The middle parameters specify the two control
-    points which define the shape of the curve. Approximately speaking,
-    control points "pull" the curve towards them.
-
-    Bezier curves were developed by French automotive engineer Pierre Bezier,
-    and are commonly used in computer graphics to define gently sloping
-    curves. See also curve().
-    """
-    _p5js.bezier(x1, y1, x2, y2, x3, y3, x4, y4, *args)
-
-
-def bezier_detail(detail: float):
-    """Sets the resolution at which Bezier's curve is displayed.
-    The default value is 20.
-
-    Note, This function is only useful when using the WEBGL renderer as the
-    default canvas renderer does not use this information.
-    """
-    _p5js.bezierDetail(detail)
-
-
-def bezier_point(a: float, b: float, c: float, d: float, t: float):
-    """Given the x or y co-ordinate values of control and anchor points of a
-    bezier curve, it evaluates the x or y coordinate of the bezier at position
-    t.
-    The parameters a and d are the x or y coordinates of first and last points
-    on the curve while b and c are of the control points.The final parameter t
-    is the position of the resultant point which is given between 0 and 1.
-    This can be done once with the x coordinates and a second time with the y
-    coordinates to get the location of a bezier curve at t.
-    """
-    _p5js.bezierPoint(a, b, c, d, t)
-
-
-def bezier_tangent(a: float, b: float, c: float, d: float, t: float):
-    """Evaluates the tangent to the Bezier at position t for points
-    a, b, c, d.
-    The parameters a and d are the first and last points on the curve, and b
-    and c are the control points. The final parameter t varies between 0
-    and 1.
-    """
-    _p5js.bezierTangent(a, b, c, d, t)
-
-
-def curve(
-    x1: float,
-    y1: float,
-    x2: float,
-    y2: float,
-    x3: float,
-    y3: float,
-    x4: float,
-    y4: float,
-    *args,
-):
-    """Draws a curved line on the screen between two points, given as the
-    middle four parameters. The first two parameters are a control point, as
-    if the curve came from this point even though it's not drawn. The last two
-    parameters similarly describe the other control point.
-
-    Longer curves can be created by putting a series of curve() functions
-    together or using curve_vertex(). An additional function called
-    curve_tightness() provides control for the visual quality of the curve.
-    The curve() function is an implementation of Catmull-Rom splines.
-    """
-    _p5js.curve(x1, y1, x2, y2, x3, y3, x4, y4, *args)
-
-
-def curve_detail(resolution: float):
-    """Sets the resolution at which curves display.
-    The default value is 20 while the minimum value is 3.
-
-    This function is only useful when using the WEBGL renderer as the default
-    canvas renderer does not use this information.
-    """
-    _p5js.curveDetail(resolution)
-
-
-def curve_tightness(amount: float):
-    """Modifies the quality of forms created with curve() and
-    curve_vertex().
-    The parameter tightness determines how the curve fits to the vertex
-    points. The value 0.0 is the default value for tightness (this value
-    defines the curves to be Catmull-Rom splines) and the value 1.0 connects
-    all the points with straight lines. Values within the range -5.0 and 5.0
-    will deform the curves but will leave them recognizable and as values
-    increase in magnitude, they will continue to deform.
-    """
-    _p5js.curveTightness(amount)
-
-
-def curve_point(a: float, b: float, c: float, d: float, t: float):
-    """Evaluates the curve at position t for points a, b, c, d.
-    The parameter t varies between 0 and 1, a and d are control points of the
-    curve, and b and c are the start and end points of the curve. This can be
-    done once with the x coordinates and a second time with the y coordinates
-    to get the location of a curve at t.
-    """
-    _p5js.curvePoint(a, b, c, d, t)
-
-
-def curve_tangent(a: float, b: float, c: float, d: float, t: float):
-    """Evaluates the tangent to the curve at position t for points a, b, c, d.
-    The parameter t varies between 0 and 1, a and d are points on the curve,
-    and b and c are the control points.
-    """
-    _p5js.curveTangent(a, b, c, d, t)
-
-
-# ======
-# Vertex
-# ======
-def begin_contour():
-    """Use the begin_contour() and end_contour() functions to create negative
-    shapes within shapes such as the center of the letter 'O'.
-    begin_contour() begins recording vertices for the shape and end_contour()
-    stops recording. The vertices that define a negative shape must "wind" in
-    the opposite direction from the exterior shape. First draw vertices for
-    the exterior clockwise order, then for internal shapes, draw vertices
-    shape in counter-clockwise.
-
-    These functions can only be used within a begin_shape()/end_shape() pair
-    and transformations such as translate(), rotate(), and scale() do not
-    work within a begin_contour()/end_contour() pair. It is also not possible
-    to use other shapes, such as ellipse() or rect() within.
-    """
-    _p5js.beginContour()
-
-
-def begin_shape(kind: str | None = None):
-    """Using the begin_shape() and end_shape() functions allow creating more
-    complex forms.
-    begin_shape() begins recording vertices for a shape and end_shape() stops
-    recording. The value of the kind parameter tells it which types of shapes
-    to create from the provided vertices. With no mode specified, the shape
-    can be any irregular polygon.
-
-    The parameters available for begin_shape() are:
-
-    POINTS Draw a series of points
-
-    LINES Draw a series of unconnected line segments (individual lines)
-
-    TRIANGLES Draw a series of separate triangles
-
-    TRIANGLE_FAN Draw a series of connected triangles sharing the first vertex
-    in a fan-like fashion
-
-    TRIANGLE_STRIP Draw a series of connected triangles in strip fashion
-
-    QUADS Draw a series of separate quads
-
-    QUAD_STRIP Draw quad strip using adjacent edges to form the next quad
-
-    TESS (WEBGL only) Handle irregular polygon for filling curve by explicit
-    tessellation
-
-    After calling the begin_shape() function, a series of vertex() commands
-    must follow. To stop drawing the shape, call end_shape(). Each shape will
-    be outlined with the current stroke color and filled with the fill color.
-
-    Transformations such as translate(), rotate(), and scale() do not work
-    within begin_shape(). It is also not possible to use other shapes, such as
-    ellipse() or rect() within begin_shape().
-
-    """
-    _p5js.beginShape(kind)
-
-
-def bezier_vertex(
-    x2: float, y2: float, x3: float, y3: float, x4: float, y4: float, *args
-):
-    """Specifies vertex coordinates for Bezier curves.
-    Each call to bezier_vertex() defines the position of two control points
-    and one anchor point of a Bezier curve, adding a new segment to a line or
-    shape. For WebGL mode bezier_vertex() can be used in 2D as well as 3D
-    mode. 2D mode expects 6 parameters, while 3D mode expects 9 parameters
-    (including z coordinates).
-
-    The first time bezier_vertex() is used within a begin_shape() call, it
-    must be prefaced with a call to vertex() to set the first anchor point.
-    This function must be used between begin_shape() and end_shape() and only
-    when there is no MODE or POINTS parameter specified to begin_shape().
-    """
-    _p5js.bezierVertex(x2, y2, x3, y3, x4, y4, *args)
-
-
-def curve_vertex(x: float, y: float, z: float | None = None):
-    """Specifies vertex coordinates for curves.
-    This function may only be used between begin_shape() and end_shape() and
-    only when there is no MODE parameter specified to begin_shape().
-    For WebGL mode curve_vertex() can be used in 2D as well as 3D mode. 2D
-    mode expects 2 parameters, while 3D mode expects 3 parameters.
-
-    The first and last points in a series of curve_vertex() lines will be used
-    to guide the beginning and end of the curve. A minimum of four points is
-    required to draw a tiny curve between the second and third points. Adding
-    a fifth point with curve_vertex() will draw the curve between the second,
-    third, and fourth points. The curve_vertex() function is an implementation
-    of Catmull-Rom splines.
-    """
-    _p5js.curveVertex(x, y, z)
-
-
-def end_contour():
-    """Use the begin_contour() and end_contour() functions to create negative
-    shapes within shapes such as the center of the letter 'O'.
-    begin_contour() begins recording vertices for the shape and end_contour()
-    stops recording. The vertices that define a negative shape must "wind" in
-    the opposite direction from the exterior shape. First draw vertices for
-    the exterior clockwise order, then for internal shapes, draw vertices
-    shape in counter-clockwise.
-
-    These functions can only be used within a begin_shape()/end_shape() pair
-    and transformations such as translate(), rotate(), and scale() do not work
-    within a begin_contour()/end_contour() pair. It is also not possible to
-    use other shapes, such as ellipse() or rect() within.
-    """
-    _p5js.endContour()
-
-
-def end_shape(mode: str | None = None):
-    """The end_shape() function is the companion to begin_shape() and may
-    only be called after begin_shape().
-    When end_shape() is called, all of the image data defined since the
-    previous call to begin_shape() is written into the image buffer. The
-    constant CLOSE as the value for the mode parameter to close the shape (to
-    connect the beginning and the end).
-    """
-    _p5js.endShape(mode)
-
-
-def quadratic_vertex(cx: float, cy: float, x3: float, y3: float, *args):
-    """Specifies vertex coordinates for quadratic Bezier curves.
-    Each call to quadratic_vertex() defines the position of one control points
-    and one anchor point of a Bezier curve, adding a new segment to a line or
-    shape. The first time quadratic_vertex() is used within a begin_shape()
-    call, it must be prefaced with a call to vertex() to set the first anchor
-    point. For WebGL mode quadratic_vertex() can be used in 2D as well as 3D
-    mode. 2D mode expects 4 parameters, while 3D mode expects 6 parameters
-    (including z coordinates).
-
-    This function must be used between begin_shape() and end_shape() and only
-    when there is no MODE or POINTS parameter specified to begin_shape().
-    """
-    _p5js.quadraticVertex(cx, cy, x3, y3, *args)
-
-
-def vertex(
-    x: float,
-    y: float,
-    z: float | None = None,
-    u: float | None = None,
-    v: float | None = None,
-):
-    """All shapes are constructed by connecting a series of vertices.
-    vertex() is used to specify the vertex coordinates for points, lines,
-    triangles, quads, and polygons. It is used exclusively within the
-    begin_shape() and end_shape() functions.
-    """
-    _p5js.vertex(x, y, z, u, v)
-
-
-def normal(x: float, y: float, z: float):
-    """Sets the 3d vertex normal to use for subsequent vertices drawn with
-    vertex().
-    A normal is a vector that is generally nearly perpendicular to a shape's
-    surface which controls how much light will be reflected from that part of
-    the surface.
-    """
-    _p5js.normal(x, y, z)
-
-
-# =============
-# 3D Primitives
-# =============
-def plane(
-    width: float | None = None,
-    height: float | None = None,
-    detail_x: int | None = None,
-    detail_y: int | None = None,
-):
-    """Draw a plane with given a width and height."""
-    _p5js.plane(width, height, detail_x, detail_y)
-
-
-def box(
-    width: float | None = None,
-    height: float | None = None,
-    depth: float | None = None,
-    detail_x: int | None = None,
-    detail_y: int | None = None,
-):
-    """Draw a box with given width, height and depth."""
-    _p5js.box(width, height, depth, detail_x, detail_y)
-
-
-def sphere(
-    radius: float | None = None,
-    detail_x: int | None = None,
-    detail_y: int | None = None,
-):
-    """Draw a sphere with given radius.
-
-    detail_x and detail_y determine the number of subdivisions in the
-    x-dimension and the y-dimension of a sphere. More subdivisions make the
-    sphere seem smoother. The recommended maximum values are both 24. Using a
-    value greater than 24 may cause a warning or slow down the browser.
-    """
-    _p5js.sphere(radius, detail_x, detail_y)
-
-
-def cylinder(
-    radius: float | None = None,
-    height: float | None = None,
-    detail_x: int | None = None,
-    detail_y: int | None = None,
-    bottom_cap: bool | None = None,
-    top_cap: bool | None = None,
-):
-    """Draw a cylinder with given radius and height.
-
-    detail_x and detail_y determines the number of subdivisions in the
-    x-dimension and the y-dimension of a cylinder. More subdivisions make the
-    cylinder seem smoother. The recommended maximum value for detailX is 24.
-    Using a value greater than 24 may cause a warning or slow down the
-    browser.
-    """
-    _p5js.cylinder(radius, height, detail_x, detail_y, bottom_cap, top_cap)
-
-
-def cone(
-    radius: float | None = None,
-    height: float | None = None,
-    detail_x: float | None = None,
-    detail_y: float | None = None,
-    cap: bool | None = None,
-):
-    """Draw a cone with given radius and height
-
-    detail_x and detail_y determine the number of subdivisions in the
-    x-dimension and the y-dimension of a cone. More subdivisions make the
-    cone seem smoother. The recommended maximum value for detailX is 24.
-    Using a value greater than 24 may cause a warning or slow down the
-    browser.
-    """
-    _p5js.cone(radius, height, detail_x, detail_y, cap)
-
-
-def ellipsoid(
-    radius_x: float | None = None,
-    radius_y: float | None = None,
-    radius_z: float | None = None,
-    detail_x: int | None = None,
-    detail_y: int | None = None,
-):
-    """Draw an ellipsoid with given radius.
-
-    detail_x and detail_y determine the number of subdivisions in the
-    x-dimension and the y-dimension of a cone. More subdivisions make the
-    ellipsoid appear to be smoother. Avoid detail number above 150, it may
-    crash the browser.
-    """
-    _p5js.ellipsoid(radius_x, radius_y, radius_z, detail_x, detail_y)
-
-
-def torus(
-    radius: float | None = None,
-    tube_radius: float | None = None,
-    detail_x: int | None = None,
-    detail_y: int | None = None,
-):
-    """Draw a torus with given radius and tube radius.
-
-    detail_x and detail_y determine the number of subdivisions in the
-    x-dimension and the y-dimension of a torus. More subdivisions make the
-    torus appear to be smoother. The default and maximum values for detail_x
-    and detail_y are 24 and 16, respectively. Setting them to relatively small
-    values like 4 and 6 allows you to create new shapes other than a torus.
-    """
-    _p5js.torus(radius, tube_radius, detail_x, detail_y)
-
-
-# =========
-# 3D Models
-# =========
-def load_model(path: str) -> object:
-    """Load a 3d model from an OBJ or STL file.
-
-    load_model() should be placed inside of preload(). This allows the model to
-    load fully before the rest of your code is run.
-
-    One of the limitations of the OBJ and STL format is that it doesn't have a
-    built-in sense of scale. This means that models exported from different
-    programs might be very different sizes. If your model isn't displaying,
-    try calling load_model() with the normalized parameter set to true. This
-    will resize the model to a scale appropriate for p5. You can also make
-    additional changes to the final size of your model with the scale()
-    function.
-
-    Also, the support for colored STL files is not present. STL files with
-    color will be rendered without color properties.
-    """
-    return _p5js.loadModel(path)
-
-
-def model(model: object):
-    """Render a 3d model to the screen."""
-    _p5js.model(model)
+class Shape(BaseSketch):
+    # =============
+    # 2D Primitives
+    # =============
+    def arc(
+        self,
+        x: float,
+        y: float,
+        w: float,
+        h: float,
+        start: float,
+        stop: float,
+        mode: str | None = None,
+        detail: int = 25,
+    ):
+        """Draw an arc to the screen.
+        If called with only x, y, w, h, start and stop, the arc will be drawn and
+        filled as an open pie segment. If a mode parameter is provided, the arc
+        will be filled like an open semi-circle (OPEN), a closed semi-circle
+        (CHORD), or as a closed pie segment (PIE). The origin may be changed with
+        the ellipse_mode() function.
+
+        The arc is always drawn clockwise from wherever start falls to wherever
+        stop falls on the ellipse. Adding or subtracting TWO_PI to either angle
+        does not change where they fall. If both start and stop fall at the same
+        place, a full ellipse will be drawn. Be aware that the y-axis increases in
+        the downward direction, therefore angles are measured clockwise from the
+        positive x-direction ("3 o'clock").
+        """
+        self._p5js.arc(x, y, w, h, start, stop, to_js(mode), detail)
+
+    def ellipse(
+        self, x: float, y: float, w: float, h: float | None = None, detail: int = 25
+    ):
+        """Draws an ellipse (oval) to the screen.
+        By default, the first two parameters set the location of the center of the
+        ellipse, and the third and fourth parameters set the shape's width and
+        height. If no height is specified, the value of width is used for both the
+        width and height. If a negative height or width is specified, the absolute
+        value is taken.
+
+        An ellipse with equal width and height is a circle. The origin may be
+        changed with the ellipse_mode() function.
+        """
+        self._p5js.ellipse(x, y, w, h, detail)
+
+    def circle(self, x: float, y: float, d: float):
+        """Draws a circle to the screen.
+        A circle is a simple closed shape. It is the set of all points in a plane
+        that are at a given distance from a given point, the center. This function
+        is a special case of the ellipse() function, where the width and height of
+        the ellipse are the same. Height and width of the ellipse correspond to
+        the diameter of the circle. By default, the first two parameters set the
+        location of the center of the circle, the third sets the diameter of the
+        circle.
+        """
+        self._p5js.circle(x, y, d)
+
+    def line(self, x1: float, y1: float, x2: float, y2: float, *args):
+        """Draws a line (a direct path between two points) to the screen.
+        If called with only 4 parameters, it will draw a line in 2D with a default
+        width of 1 pixel. This width can be modified by using the stroke_weight()
+        function. A line cannot be filled, therefore the fill() function will not
+        affect the color of a line. So to color a line, use the stroke() function.
+        """
+        self._p5js.line(x1, y1, x2, y2, *args)
+
+    def point(self, x: float, y: float, z: float | None = None):
+        """Draws a point, a coordinate in space at the dimension of one pixel.
+        The first parameter is the horizontal value for the point, the second
+        param is the vertical value for the point. The color of the point is
+        changed with the stroke() function. The size of the point can be changed
+        with the stroke_weight() function.
+        """
+        self._p5js.point(x, y, z)
+
+    def quad(
+        self,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        x3: float,
+        y3: float,
+        x4: float,
+        y4: float,
+        detail_x: int | None = None,
+        detail_y: int | None = None,
+        *args,
+    ):
+        """Draws a quad on the canvas.
+        A quad is a quadrilateral, a four-sided polygon. It is similar to a
+        rectangle, but the angles between its edges are not constrained to ninety
+        degrees. The first pair of parameters (x1,y1) sets the first vertex and
+        the subsequent pairs should proceed clockwise or counter-clockwise around
+        the defined shape. z-arguments only work when quad() is used in WEBGL
+        mode.
+        """
+        self._p5js.quad(x1, y1, x2, y2, x3, y3, x4, y4, detail_x, detail_y, *args)
+
+    def rect(
+        self,
+        x: float,
+        y: float,
+        w: float,
+        h: float,
+        r: float | None = None,
+        tr: float | None = None,
+        br: float | None = None,
+        bl: float | None = None,
+    ):
+        """Draws a rectangle on the canvas.
+        A rectangle is a four-sided closed shape with every angle at ninety
+        degrees. By default, the first two parameters set the location of the
+        upper-left corner, the third sets the width, and the fourth sets the
+        height. The way these parameters are interpreted may be changed with the
+        rect_mode() function.
+
+        The fifth, sixth, seventh and eighth parameters, if specified, determine
+        corner radius for the top-left, top-right, lower-right and lower-left
+        corners, respectively. An omitted corner radius parameter is set to the
+        value of the previously specified radius value in the parameter list.
+        """
+        self._p5js.rect(x, y, w, h, r, tr, br, bl)
+
+    def square(
+        self,
+        x: float,
+        y: float,
+        s: float,
+        tl: float | None = None,
+        tr: float | None = None,
+        br: float | None = None,
+        bl: float | None = None,
+    ):
+        """Draws a square to the screen.
+        A square is a four-sided shape with every angle at ninety degrees, and
+        equal side size. This function is a special case of the rect() function,
+        where the width and height are the same, and the parameter is called "s"
+        for side size. By default, the first two parameters set the location of
+        the upper-left corner, the third sets the side size of the square. The way
+        these parameters are interpreted, may be changed with the rect_mode()
+        function.
+
+        The fourth, fifth, sixth and seventh parameters, if specified, determine
+        corner radius for the top-left, top-right, lower-right and lower-left
+        corners, respectively. An omitted corner radius parameter is set to the
+        value of the previously specified radius value in the parameter list.
+        """
+        self._p5js.square(x, y, s, tl, tr, br, bl)
+
+    def triangle(
+        self, x1: float, y1: float, x2: float, y2: float, x3: float, y3: float
+    ):
+        """Draws a triangle to the canvas.
+        A triangle is a plane created by connecting three points. The first two
+        arguments specify the first point, the middle two arguments specify the
+        second point, and the last two arguments specify the third point.
+        """
+        self._p5js.triangle(x1, y1, x2, y2, x3, y3)
+
+    # ==========
+    # Attributes
+    # ==========
+    def ellipse_mode(self, mode: str):
+        """Modifies the location from which ellipses are drawn by changing the way
+        in which parameters given to ellipse(), circle() and arc() are
+        interpreted.
+
+        The default mode is CENTER, in which the first two parameters are
+        interpreted as the shape's center point's x and y coordinates
+        respectively, while the third and fourth parameters are its width and
+        height.
+
+        ellipse_mode(RADIUS) also uses the first two parameters as the shape's
+        center point's x and y coordinates, but uses the third and fourth
+        parameters to specify half of the shapes's width and height.
+
+        ellipse_mode(CORNER) interprets the first two parameters as the upper-left
+        corner of the shape, while the third and fourth parameters are its width
+        and height.
+
+        ellipse_mode(CORNERS) interprets the first two parameters as the location
+        of one corner of the ellipse's bounding box, and the third and fourth
+        parameters as the location of the opposite corner.
+
+        The parameter to this function must be written in ALL CAPS because they
+        are predefined as constants in ALL CAPS and Python is a case-sensitive
+        language.
+        """
+        self._p5js.ellipseMode(mode)
+
+    def no_smooth(self):
+        """Draws all geometry with jagged (aliased) edges.
+
+        Note that smooth() is active by default in 2D mode, so it is necessary to
+        call no_smooth() to disable smoothing of geometry, images, and fonts.
+
+        In 3D mode, no_smooth() is enabled by default, so it is necessary to call
+        smooth() if you would like smooth (antialiased) edges on your geometry.
+        """
+        self._p5js.noSmooth()
+
+    def rect_mode(self, mode: str):
+        """Modifies the location from which rectangles are drawn by changing the
+        way in which parameters given to rect() are interpreted.
+
+        The default mode is CORNER, which interprets the first two parameters as
+        the upper-left corner of the shape, while the third and fourth parameters
+        are its width and height.
+
+        rectMode(CORNERS) interprets the first two parameters as the location of
+        one of the corners, and the third and fourth parameters as the location
+        of the diagonally opposite corner. Note, the rectangle is drawn between
+        the coordinates, so it is not necessary that the first corner be the
+        upper left corner.
+
+        rectMode(CENTER) interprets the first two parameters as the shape's center
+        point, while the third and fourth parameters are its width and height.
+
+        rectMode(RADIUS) also uses the first two parameters as the shape's center
+        point, but uses the third and fourth parameters to specify half of the
+        shape's width and height respectively.
+
+        The parameter to this function must be written in ALL CAPS because they
+        are predefined as constants in ALL CAPS and Python is a case-sensitive
+        language.
+        """
+        self._p5js.rectMode(mode)
+
+    def smooth(self):
+        """Draws all geometry with smooth (anti-aliased) edges.
+        smooth() will also improve image quality of resized images.
+
+        Note that smooth() is active by default in 2D mode; no_smooth() can be
+        used to disable smoothing of geometry, images, and fonts.
+
+        In 3D mode, no_smooth() is enabled by default, so it is necessary to call
+        smooth() if you would like smooth (antialiased) edges on your geometry.
+        """
+        self._p5js.smooth()
+
+    def stroke_cap(self, cap: str):
+        """Sets the style for rendering line endings.
+        These ends are either rounded, squared, or extended, each of which
+        specified with the corresponding parameters: ROUND, SQUARE, or PROJECT.
+        The default cap is ROUND.
+
+        The parameter to this function must be written in ALL CAPS because they
+        are predefined as constants in ALL CAPS and Python is a case-sensitive
+        language.
+        """
+        self._p5js.strokeCap(cap)
+
+    def stroke_join(self, join: str):
+        """Sets the style of the joints which connect line segments.
+        These joints are either mitered, beveled, or rounded and specified with
+        the corresponding parameters: MITER, BEVEL, or ROUND. The default joint is
+        MITER in 2D mode and ROUND in WebGL mode.
+
+        The parameter to this function must be written in ALL CAPS because they
+        are predefined as constants in ALL CAPS and Python is a case-sensitive
+        language.
+        """
+        self._p5js.strokeJoin(join)
+
+    def stroke_weight(self, weight: float):
+        """Sets the width of the stroke used for lines, points, and the border
+        around shapes.
+        All widths are set in units of pixels.
+
+        Note that it is affected by any transformation or scaling that has been
+        applied previously.
+        """
+        self._p5js.strokeWeight(weight)
+
+    # ======
+    # Curves
+    # ======
+    def bezier(
+        self,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        x3: float,
+        y3: float,
+        x4: float,
+        y4: float,
+        *args,
+    ):
+        """Draws a cubic Bezier curve on the screen.
+        These curves are defined by a series of anchor and control points. The
+        first two parameters specify the first anchor point and the last two
+        parameters specify the other anchor point, which become the first and
+        last points on the curve. The middle parameters specify the two control
+        points which define the shape of the curve. Approximately speaking,
+        control points "pull" the curve towards them.
+
+        Bezier curves were developed by French automotive engineer Pierre Bezier,
+        and are commonly used in computer graphics to define gently sloping
+        curves. See also curve().
+        """
+        self._p5js.bezier(x1, y1, x2, y2, x3, y3, x4, y4, *args)
+
+    def bezier_detail(self, detail: float):
+        """Sets the resolution at which Bezier's curve is displayed.
+        The default value is 20.
+
+        Note, This function is only useful when using the WEBGL renderer as the
+        default canvas renderer does not use this information.
+        """
+        self._p5js.bezierDetail(detail)
+
+    def bezier_point(self, a: float, b: float, c: float, d: float, t: float):
+        """Given the x or y co-ordinate values of control and anchor points of a
+        bezier curve, it evaluates the x or y coordinate of the bezier at position
+        t.
+        The parameters a and d are the x or y coordinates of first and last points
+        on the curve while b and c are of the control points.The final parameter t
+        is the position of the resultant point which is given between 0 and 1.
+        This can be done once with the x coordinates and a second time with the y
+        coordinates to get the location of a bezier curve at t.
+        """
+        self._p5js.bezierPoint(a, b, c, d, t)
+
+    def bezier_tangent(self, a: float, b: float, c: float, d: float, t: float):
+        """Evaluates the tangent to the Bezier at position t for points
+        a, b, c, d.
+        The parameters a and d are the first and last points on the curve, and b
+        and c are the control points. The final parameter t varies between 0
+        and 1.
+        """
+        self._p5js.bezierTangent(a, b, c, d, t)
+
+    def curve(
+        self,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        x3: float,
+        y3: float,
+        x4: float,
+        y4: float,
+        *args,
+    ):
+        """Draws a curved line on the screen between two points, given as the
+        middle four parameters. The first two parameters are a control point, as
+        if the curve came from this point even though it's not drawn. The last two
+        parameters similarly describe the other control point.
+
+        Longer curves can be created by putting a series of curve() functions
+        together or using curve_vertex(). An additional function called
+        curve_tightness() provides control for the visual quality of the curve.
+        The curve() function is an implementation of Catmull-Rom splines.
+        """
+        self._p5js.curve(x1, y1, x2, y2, x3, y3, x4, y4, *args)
+
+    def curve_detail(self, resolution: float):
+        """Sets the resolution at which curves display.
+        The default value is 20 while the minimum value is 3.
+
+        This function is only useful when using the WEBGL renderer as the default
+        canvas renderer does not use this information.
+        """
+        self._p5js.curveDetail(resolution)
+
+    def curve_tightness(self, amount: float):
+        """Modifies the quality of forms created with curve() and
+        curve_vertex().
+        The parameter tightness determines how the curve fits to the vertex
+        points. The value 0.0 is the default value for tightness (this value
+        defines the curves to be Catmull-Rom splines) and the value 1.0 connects
+        all the points with straight lines. Values within the range -5.0 and 5.0
+        will deform the curves but will leave them recognizable and as values
+        increase in magnitude, they will continue to deform.
+        """
+        self._p5js.curveTightness(amount)
+
+    def curve_point(self, a: float, b: float, c: float, d: float, t: float):
+        """Evaluates the curve at position t for points a, b, c, d.
+        The parameter t varies between 0 and 1, a and d are control points of the
+        curve, and b and c are the start and end points of the curve. This can be
+        done once with the x coordinates and a second time with the y coordinates
+        to get the location of a curve at t.
+        """
+        self._p5js.curvePoint(a, b, c, d, t)
+
+    def curve_tangent(self, a: float, b: float, c: float, d: float, t: float):
+        """Evaluates the tangent to the curve at position t for points a, b, c, d.
+        The parameter t varies between 0 and 1, a and d are points on the curve,
+        and b and c are the control points.
+        """
+        self._p5js.curveTangent(a, b, c, d, t)
+
+    # ======
+    # Vertex
+    # ======
+    def begin_contour(self):
+        """Use the begin_contour() and end_contour() functions to create negative
+        shapes within shapes such as the center of the letter 'O'.
+        begin_contour() begins recording vertices for the shape and end_contour()
+        stops recording. The vertices that define a negative shape must "wind" in
+        the opposite direction from the exterior shape. First draw vertices for
+        the exterior clockwise order, then for internal shapes, draw vertices
+        shape in counter-clockwise.
+
+        These functions can only be used within a begin_shape()/end_shape() pair
+        and transformations such as translate(), rotate(), and scale() do not
+        work within a begin_contour()/end_contour() pair. It is also not possible
+        to use other shapes, such as ellipse() or rect() within.
+        """
+        self._p5js.beginContour()
+
+    def begin_shape(self, kind: str | None = None):
+        """Using the begin_shape() and end_shape() functions allow creating more
+        complex forms.
+        begin_shape() begins recording vertices for a shape and end_shape() stops
+        recording. The value of the kind parameter tells it which types of shapes
+        to create from the provided vertices. With no mode specified, the shape
+        can be any irregular polygon.
+
+        The parameters available for begin_shape() are:
+
+        POINTS Draw a series of points
+
+        LINES Draw a series of unconnected line segments (individual lines)
+
+        TRIANGLES Draw a series of separate triangles
+
+        TRIANGLE_FAN Draw a series of connected triangles sharing the first vertex
+        in a fan-like fashion
+
+        TRIANGLE_STRIP Draw a series of connected triangles in strip fashion
+
+        QUADS Draw a series of separate quads
+
+        QUAD_STRIP Draw quad strip using adjacent edges to form the next quad
+
+        TESS (WEBGL only) Handle irregular polygon for filling curve by explicit
+        tessellation
+
+        After calling the begin_shape() function, a series of vertex() commands
+        must follow. To stop drawing the shape, call end_shape(). Each shape will
+        be outlined with the current stroke color and filled with the fill color.
+
+        Transformations such as translate(), rotate(), and scale() do not work
+        within begin_shape(). It is also not possible to use other shapes, such as
+        ellipse() or rect() within begin_shape().
+
+        """
+        self._p5js.beginShape(kind)
+
+    def bezier_vertex(
+        self, x2: float, y2: float, x3: float, y3: float, x4: float, y4: float, *args
+    ):
+        """Specifies vertex coordinates for Bezier curves.
+        Each call to bezier_vertex() defines the position of two control points
+        and one anchor point of a Bezier curve, adding a new segment to a line or
+        shape. For WebGL mode bezier_vertex() can be used in 2D as well as 3D
+        mode. 2D mode expects 6 parameters, while 3D mode expects 9 parameters
+        (including z coordinates).
+
+        The first time bezier_vertex() is used within a begin_shape() call, it
+        must be prefaced with a call to vertex() to set the first anchor point.
+        This function must be used between begin_shape() and end_shape() and only
+        when there is no MODE or POINTS parameter specified to begin_shape().
+        """
+        self._p5js.bezierVertex(x2, y2, x3, y3, x4, y4, *args)
+
+    def curve_vertex(self, x: float, y: float, z: float | None = None):
+        """Specifies vertex coordinates for curves.
+        This function may only be used between begin_shape() and end_shape() and
+        only when there is no MODE parameter specified to begin_shape().
+        For WebGL mode curve_vertex() can be used in 2D as well as 3D mode. 2D
+        mode expects 2 parameters, while 3D mode expects 3 parameters.
+
+        The first and last points in a series of curve_vertex() lines will be used
+        to guide the beginning and end of the curve. A minimum of four points is
+        required to draw a tiny curve between the second and third points. Adding
+        a fifth point with curve_vertex() will draw the curve between the second,
+        third, and fourth points. The curve_vertex() function is an implementation
+        of Catmull-Rom splines.
+        """
+        self._p5js.curveVertex(x, y, z)
+
+    def end_contour(self):
+        """Use the begin_contour() and end_contour() functions to create negative
+        shapes within shapes such as the center of the letter 'O'.
+        begin_contour() begins recording vertices for the shape and end_contour()
+        stops recording. The vertices that define a negative shape must "wind" in
+        the opposite direction from the exterior shape. First draw vertices for
+        the exterior clockwise order, then for internal shapes, draw vertices
+        shape in counter-clockwise.
+
+        These functions can only be used within a begin_shape()/end_shape() pair
+        and transformations such as translate(), rotate(), and scale() do not work
+        within a begin_contour()/end_contour() pair. It is also not possible to
+        use other shapes, such as ellipse() or rect() within.
+        """
+        self._p5js.endContour()
+
+    def end_shape(self, mode: str | None = None):
+        """The end_shape() function is the companion to begin_shape() and may
+        only be called after begin_shape().
+        When end_shape() is called, all of the image data defined since the
+        previous call to begin_shape() is written into the image buffer. The
+        constant CLOSE as the value for the mode parameter to close the shape (to
+        connect the beginning and the end).
+        """
+        self._p5js.endShape(mode)
+
+    def quadratic_vertex(self, cx: float, cy: float, x3: float, y3: float, *args):
+        """Specifies vertex coordinates for quadratic Bezier curves.
+        Each call to quadratic_vertex() defines the position of one control points
+        and one anchor point of a Bezier curve, adding a new segment to a line or
+        shape. The first time quadratic_vertex() is used within a begin_shape()
+        call, it must be prefaced with a call to vertex() to set the first anchor
+        point. For WebGL mode quadratic_vertex() can be used in 2D as well as 3D
+        mode. 2D mode expects 4 parameters, while 3D mode expects 6 parameters
+        (including z coordinates).
+
+        This function must be used between begin_shape() and end_shape() and only
+        when there is no MODE or POINTS parameter specified to begin_shape().
+        """
+        self._p5js.quadraticVertex(cx, cy, x3, y3, *args)
+
+    def vertex(
+        self,
+        x: float,
+        y: float,
+        z: float | None = None,
+        u: float | None = None,
+        v: float | None = None,
+    ):
+        """All shapes are constructed by connecting a series of vertices.
+        vertex() is used to specify the vertex coordinates for points, lines,
+        triangles, quads, and polygons. It is used exclusively within the
+        begin_shape() and end_shape() functions.
+        """
+        self._p5js.vertex(x, y, z, u, v)
+
+    def normal(self, x: float, y: float, z: float):
+        """Sets the 3d vertex normal to use for subsequent vertices drawn with
+        vertex().
+        A normal is a vector that is generally nearly perpendicular to a shape's
+        surface which controls how much light will be reflected from that part of
+        the surface.
+        """
+        self._p5js.normal(x, y, z)
+
+    # =============
+    # 3D Primitives
+    # =============
+    def plane(
+        self,
+        width: float | None = None,
+        height: float | None = None,
+        detail_x: int | None = None,
+        detail_y: int | None = None,
+    ):
+        """Draw a plane with given a width and height."""
+        self._p5js.plane(width, height, detail_x, detail_y)
+
+    def box(
+        self,
+        width: float | None = None,
+        height: float | None = None,
+        depth: float | None = None,
+        detail_x: int | None = None,
+        detail_y: int | None = None,
+    ):
+        """Draw a box with given width, height and depth."""
+        self._p5js.box(width, height, depth, detail_x, detail_y)
+
+    def sphere(
+        self,
+        radius: float | None = None,
+        detail_x: int | None = None,
+        detail_y: int | None = None,
+    ):
+        """Draw a sphere with given radius.
+
+        detail_x and detail_y determine the number of subdivisions in the
+        x-dimension and the y-dimension of a sphere. More subdivisions make the
+        sphere seem smoother. The recommended maximum values are both 24. Using a
+        value greater than 24 may cause a warning or slow down the browser.
+        """
+        self._p5js.sphere(radius, detail_x, detail_y)
+
+    def cylinder(
+        self,
+        radius: float | None = None,
+        height: float | None = None,
+        detail_x: int | None = None,
+        detail_y: int | None = None,
+        bottom_cap: bool | None = None,
+        top_cap: bool | None = None,
+    ):
+        """Draw a cylinder with given radius and height.
+
+        detail_x and detail_y determines the number of subdivisions in the
+        x-dimension and the y-dimension of a cylinder. More subdivisions make the
+        cylinder seem smoother. The recommended maximum value for detailX is 24.
+        Using a value greater than 24 may cause a warning or slow down the
+        browser.
+        """
+        self._p5js.cylinder(radius, height, detail_x, detail_y, bottom_cap, top_cap)
+
+    def cone(
+        self,
+        radius: float | None = None,
+        height: float | None = None,
+        detail_x: float | None = None,
+        detail_y: float | None = None,
+        cap: bool | None = None,
+    ):
+        """Draw a cone with given radius and height
+
+        detail_x and detail_y determine the number of subdivisions in the
+        x-dimension and the y-dimension of a cone. More subdivisions make the
+        cone seem smoother. The recommended maximum value for detailX is 24.
+        Using a value greater than 24 may cause a warning or slow down the
+        browser.
+        """
+        self._p5js.cone(radius, height, detail_x, detail_y, cap)
+
+    def ellipsoid(
+        self,
+        radius_x: float | None = None,
+        radius_y: float | None = None,
+        radius_z: float | None = None,
+        detail_x: int | None = None,
+        detail_y: int | None = None,
+    ):
+        """Draw an ellipsoid with given radius.
+
+        detail_x and detail_y determine the number of subdivisions in the
+        x-dimension and the y-dimension of a cone. More subdivisions make the
+        ellipsoid appear to be smoother. Avoid detail number above 150, it may
+        crash the browser.
+        """
+        self._p5js.ellipsoid(radius_x, radius_y, radius_z, detail_x, detail_y)
+
+    def torus(
+        self,
+        radius: float | None = None,
+        tube_radius: float | None = None,
+        detail_x: int | None = None,
+        detail_y: int | None = None,
+    ):
+        """Draw a torus with given radius and tube radius.
+
+        detail_x and detail_y determine the number of subdivisions in the
+        x-dimension and the y-dimension of a torus. More subdivisions make the
+        torus appear to be smoother. The default and maximum values for detail_x
+        and detail_y are 24 and 16, respectively. Setting them to relatively small
+        values like 4 and 6 allows you to create new shapes other than a torus.
+        """
+        self._p5js.torus(radius, tube_radius, detail_x, detail_y)
+
+    # =========
+    # 3D Models
+    # =========
+    def load_model(self, path: str) -> object:
+        """Load a 3d model from an OBJ or STL file.
+
+        load_model() should be placed inside of preload(). This allows the model to
+        load fully before the rest of your code is run.
+
+        One of the limitations of the OBJ and STL format is that it doesn't have a
+        built-in sense of scale. This means that models exported from different
+        programs might be very different sizes. If your model isn't displaying,
+        try calling load_model() with the normalized parameter set to true. This
+        will resize the model to a scale appropriate for p5. You can also make
+        additional changes to the final size of your model with the scale()
+        function.
+
+        Also, the support for colored STL files is not present. STL files with
+        color will be rendered without color properties.
+        """
+        return self._p5js.loadModel(path)
+
+    def model(self, model: object):
+        """Render a 3d model to the screen."""
+        self._p5js.model(model)
```

### Comparing `proceso-0.0.4/src/proceso/structure.py` & `proceso-0.0.6/src/proceso/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,130 +1,125 @@
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-def remove():
-    """Removes the entire p5 sketch.
-    This will remove the canvas and any elements created by p5.js. It will
-    also stop the draw loop and unbind any properties or methods from the
-    window global scope. It will leave a variable p5 in case you wanted to
-    create a new p5 sketch. If you like, you can set p5 = null to erase it.
-    While all functions and variables and objects created by the p5 library
-    will be removed, any other global variables created by your code will
-    remain.
-    """
-    _p5js.remove()
-
-
-def no_loop():
-    """Stops p5.js from continuously executing the code within draw().
-    If loop() is called, the code in draw() begins to run continuously again.
-    If using no_loop() in setup(), it should be the last line inside the
-    block.
-
-    When noLoop() is used, it's not possible to manipulate or access the screen
-    inside event handling functions such as mouse_pressed() or key_pressed().
-    Instead, use those functions to call redraw() or loop(), which will run
-    draw(), which can update the screen properly. This means that when
-    no_loop() has been called, no drawing can happen, and functions like
-    save_frames() or load_pixels() may not be used.
-
-    Note that if the sketch is resized, redraw() will be called to update the
-    sketch, even after no_loop() has been specified. Otherwise, the sketch
-    would enter an odd state until loop() was called.
-
-    Use is_looping() to check the current state of loop().
-    """
-    _p5js.noLoop()
-
-
-def loop():
-    """By default, p5 loops through draw() continuously, executing the code
-    within it.
-    However, the draw() loop may be stopped by calling no_loop(). In that
-    case, the draw() loop can be resumed with loop().
-
-    Avoid calling loop() from inside setup().
-
-    Use is_looping() to check the current state of loop().
-    """
-    _p5js.loop()
-
-
-def is_looping() -> bool:
-    """By default, p5 loops through draw() continuously, executing the code
-    within it.
-    If the sketch is stopped with no_loop() or resumed with loop(),
-    is_looping() returns the current state for use within custom event handlers.
-    """
-    return _p5js.isLooping()
-
-
-def push():
-    """The push() function saves the current drawing style settings and
-    transformations, while pop() restores these settings.
-    Note that these functions are always used together. They allow you to
-    change the style and transformation settings and later return to what you
-    had. When a new state is started with push(), it builds on the current
-    style and transform information. The push() and pop() functions can be
-    embedded to provide more control. (See the second example for a
-    demonstration.)
-
-    push() stores information related to the current transformation state and
-    style settings controlled by the following functions: fill(), no_fill(),
-    no_stroke(), stroke(), tint(), no_tint(), stroke_weight(), stroke_cap(),
-    stroke_join(), image_mode(), rect_mode(), ellipse_mode(), color_mode(),
-    text_align(), text_font(), text_size(), text_leading(), apply_matrix(),
-    reset_matrix(), rotate(), scale(), shear_x(), shear_y(), translate(),
-    noise_seed().
-
-    In WEBGL mode additional style settings are stored. These are controlled
-    by the following functions: set_camera(), ambient_light(),
-    directional_light(), point_light(), texture(), specular_material(),
-    shininess(), normal_material() and shader().
-    """
-    _p5js.push()
-
-
-def pop():
-    """The push() function saves the current drawing style settings and
-    transformations, while pop() restores these settings.
-    Note that these functions are always used together. They allow you to
-    change the style and transformation settings and later return to what you
-    had. When a new state is started with push(), it builds on the current
-    style and transform information. The push() and pop() functions can be
-    embedded to provide more control. (See the second example for a
-    demonstration.)
-
-    push() stores information related to the current transformation state and
-    style settings controlled by the following functions: fill(), no_fill(),
-    no_stroke(), stroke(), tint(), no_tint(), stroke_weight(), stroke_cap(),
-    stroke_join(), image_mode(), rect_mode(), ellipse_mode(), color_mode(),
-    text_align(), text_font(), text_size(), text_leading(), apply_matrix(),
-    reset_matrix(), rotate(), scale(), shear_x(), shear_y(), translate(),
-    noise_seed().
-
-    In WEBGL mode additional style settings are stored. These are controlled
-    by the following functions: set_camera(), ambient_light(),
-    directional_light(), point_light(), texture(), specular_material(),
-    shininess(), normal_material() and shader().
-    """
-    _p5js.pop()
-
-
-def redraw(n: int | None = None):
-    """Executes the code within draw() one time.
-    This function allows the program to update the display window only when
-    necessary, for example when an event registered by mouse_pressed()
-    or key_pressed() occurs.
-
-    In structuring a program, it only makes sense to call redraw() within
-    events such as mouse_pressed(). This is because redraw() does not run
-    draw() immediately (it only sets a flag that indicates an update is
-    needed).
-
-    The redraw() function does not work properly when called inside draw().
-    To enable/disable animations, use loop() and no_loop().
-
-    In addition you can set the number of redraws per method call. Just add an
-    integer as single parameter for the number of redraws.
-    """
-    _p5js.redraw(n)
+class Structure(BaseSketch):
+    def remove(self):
+        """Removes the entire p5 sketch.
+        This will remove the canvas and any elements created by p5.js. It will
+        also stop the draw loop and unbind any properties or methods from the
+        window global scope. It will leave a variable p5 in case you wanted to
+        create a new p5 sketch. If you like, you can set p5 = null to erase it.
+        While all functions and variables and objects created by the p5 library
+        will be removed, any other global variables created by your code will
+        remain.
+        """
+        self._p5js.remove()
+
+    def no_loop(self):
+        """Stops p5.js from continuously executing the code within draw().
+        If loop() is called, the code in draw() begins to run continuously again.
+        If using no_loop() in setup(), it should be the last line inside the
+        block.
+
+        When noLoop() is used, it's not possible to manipulate or access the screen
+        inside event handling functions such as mouse_pressed() or key_pressed().
+        Instead, use those functions to call redraw() or loop(), which will run
+        draw(), which can update the screen properly. This means that when
+        no_loop() has been called, no drawing can happen, and functions like
+        save_frames() or load_pixels() may not be used.
+
+        Note that if the sketch is resized, redraw() will be called to update the
+        sketch, even after no_loop() has been specified. Otherwise, the sketch
+        would enter an odd state until loop() was called.
+
+        Use is_looping() to check the current state of loop().
+        """
+        self._p5js.noLoop()
+
+    def loop(self):
+        """By default, p5 loops through draw() continuously, executing the code
+        within it.
+        However, the draw() loop may be stopped by calling no_loop(). In that
+        case, the draw() loop can be resumed with loop().
+
+        Avoid calling loop() from inside setup().
+
+        Use is_looping() to check the current state of loop().
+        """
+        self._p5js.loop()
+
+    def is_looping(self) -> bool:
+        """By default, p5 loops through draw() continuously, executing the code
+        within it.
+        If the sketch is stopped with no_loop() or resumed with loop(),
+        is_looping() returns the current state for use within custom event handlers.
+        """
+        return self._p5js.isLooping()
+
+    def push(self):
+        """The push() function saves the current drawing style settings and
+        transformations, while pop() restores these settings.
+        Note that these functions are always used together. They allow you to
+        change the style and transformation settings and later return to what you
+        had. When a new state is started with push(), it builds on the current
+        style and transform information. The push() and pop() functions can be
+        embedded to provide more control. (See the second example for a
+        demonstration.)
+
+        push() stores information related to the current transformation state and
+        style settings controlled by the following functions: fill(), no_fill(),
+        no_stroke(), stroke(), tint(), no_tint(), stroke_weight(), stroke_cap(),
+        stroke_join(), image_mode(), rect_mode(), ellipse_mode(), color_mode(),
+        text_align(), text_font(), text_size(), text_leading(), apply_matrix(),
+        reset_matrix(), rotate(), scale(), shear_x(), shear_y(), translate(),
+        noise_seed().
+
+        In WEBGL mode additional style settings are stored. These are controlled
+        by the following functions: set_camera(), ambient_light(),
+        directional_light(), point_light(), texture(), specular_material(),
+        shininess(), normal_material() and shader().
+        """
+        self._p5js.push()
+
+    def pop(self):
+        """The push() function saves the current drawing style settings and
+        transformations, while pop() restores these settings.
+        Note that these functions are always used together. They allow you to
+        change the style and transformation settings and later return to what you
+        had. When a new state is started with push(), it builds on the current
+        style and transform information. The push() and pop() functions can be
+        embedded to provide more control. (See the second example for a
+        demonstration.)
+
+        push() stores information related to the current transformation state and
+        style settings controlled by the following functions: fill(), no_fill(),
+        no_stroke(), stroke(), tint(), no_tint(), stroke_weight(), stroke_cap(),
+        stroke_join(), image_mode(), rect_mode(), ellipse_mode(), color_mode(),
+        text_align(), text_font(), text_size(), text_leading(), apply_matrix(),
+        reset_matrix(), rotate(), scale(), shear_x(), shear_y(), translate(),
+        noise_seed().
+
+        In WEBGL mode additional style settings are stored. These are controlled
+        by the following functions: set_camera(), ambient_light(),
+        directional_light(), point_light(), texture(), specular_material(),
+        shininess(), normal_material() and shader().
+        """
+        self._p5js.pop()
+
+    def redraw(self, n: int | None = None):
+        """Executes the code within draw() one time.
+        This function allows the program to update the display window only when
+        necessary, for example when an event registered by mouse_pressed()
+        or key_pressed() occurs.
+
+        In structuring a program, it only makes sense to call redraw() within
+        events such as mouse_pressed(). This is because redraw() does not run
+        draw() immediately (it only sets a flag that indicates an update is
+        needed).
+
+        The redraw() function does not work properly when called inside draw().
+        To enable/disable animations, use loop() and no_loop().
+
+        In addition you can set the number of redraws per method call. Just add an
+        integer as single parameter for the number of redraws.
+        """
+        self._p5js.redraw(n)
```

### Comparing `proceso-0.0.4/src/proceso/three_d.py` & `proceso-0.0.6/src/proceso/three_d.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,397 +1,397 @@
 from pyodide.ffi import to_js
 
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-# ===========
-# Interaction
-# ===========
-def orbit_control(
-    sensitivity_x: float | None = None,
-    sensitivity_y: float | None = None,
-    sensitivity_z: float | None = None,
-):
-    """Allows movement around a 3D sketch using a mouse or trackpad.
-    Left-clicking and dragging will rotate the camera position about the
-    center of the sketch, right-clicking and dragging will pan the camera
-    position without rotation, and using the mouse wheel (scrolling) will
-    move the camera closer or further from the center of the sketch. This
-    function can be called with parameters dictating sensitivity to mouse
-    movement along the X and Y axes. Calling this function without parameters
-    is equivalent to calling orbit_control(1,1). To reverse direction of
-    movement in either axis, enter a negative number for sensitivity.
-    """
-    _p5js.orbitControl(sensitivity_x, sensitivity_y, sensitivity_z)
-
-
-def debug_mode(mode: str | None = None):
-    """debug_mode() helps visualize 3D space by adding a grid to indicate
-    where the ‘ground’ is in a sketch and an axes icon which indicates the +X,
-    +Y, and +Z directions. This function can be called without parameters to
-    create a default grid and axes icon. The grid is drawn using the most
-    recently set stroke color and weight. To specify these parameters, add a
-    call to stroke() and stroke_weight() just before the end of the draw()
-    loop.
-
-    By default, the grid will run through the origin (0,0,0) of the sketch
-    along the XZ plane and the axes icon will be offset from the origin. Both
-    the grid and axes icon will be sized according to the current canvas size.
-    Note that because the grid runs parallel to the default camera view, it is
-    often helpful to use debug_mode along with orbit_control to allow full
-    view of the grid.
-    """
-    _p5js.debugMode(mode)
-
-
-def no_debug_mode():
-    """Turns off debug_mode() in a 3D sketch."""
-    _p5js.noDebugMode()
-
-
-# ======
-# Lights
-# ======
-def ambient_light(
-    value: str | int | list[int],
-    v2: int | None = None,
-    v3: int | None = None,
-    v4: int | None = None,
-):
-    """Creates an ambient light with the given color.
-
-    Ambient light does not come from a specific direction. Objects are evenly
-    lit from all sides. Ambient lights are almost always used in combination
-    with other types of lights.
-
-    Note: lights need to be called (whether directly or indirectly) within
-    draw() to remain persistent in a looping program. Placing them in setup()
-    will cause them to only have an effect the first time through the loop.
-    """
-    if v4:
-        _p5js.ambientLight(value, v2, v3, v4)
-    elif v3:
-        _p5js.ambientLight(value, v2, v3)
-    elif v2:
-        _p5js.ambientLight(value, v2)
-    else:
-        _p5js.ambientLight(to_js(value))
-
-
-def specular_color(
-    value: str | int | list[int],
-    v2: int | None = None,
-    v3: int | None = None,
-):
-    """Sets the color of the specular highlight of a non-ambient light
-    (i.e. all lights except ambient_light()).
-
-    specularColor() affects only the lights which are created after it in the
-    code.
-
-    This function is used in combination with specular_material(). If a
-    geometry does not use specular_material(), this function will have no
-    effect.
-
-    The default color is white (255, 255, 255), which is used if
-    specular_color() is not explicitly called.
-
-    Note: specular_color is equivalent to the Processing function
-    lightSpecular.
-    """
-    if v3:
-        _p5js.specularColor(value, v2, v3)
-    elif v2:
-        _p5js.specularColor(value, v2)
-    else:
-        _p5js.specularColor(to_js(value))
-
-
-def directional_light(
-    v1: float,
-    v2: float,
-    v3: float,
-    x: float,
-    y: float,
-    z: float,
-):
-    """Creates a directional light with the given color and direction.
-
-    Directional light comes from one direction. The direction is specified as
-    numbers inclusively between -1 and 1. For example, setting the direction
-    as (0, -1, 0) will cause the geometry to be lit from below (since the
-    light will be facing directly upwards). Similarly, setting the direction
-    as (1, 0, 0) will cause the geometry to be lit from the left (since the
-    light will be facing directly rightwards).
-
-    Directional lights do not have a specific point of origin, and therefore
-    cannot be positioned closer or farther away from a geometry.
-
-    A maximum of 5 directional lights can be active at once.
-
-    Note: lights need to be called (whether directly or indirectly) within
-    draw() to remain persistent in a looping program. Placing them in setup()
-    will cause them to only have an effect the first time through the loop.
-    """
-    _p5js.directionalLight(v1, v2, v3, x, y, z)
-
-
-def point_light(
-    v1: float,
-    v2: float,
-    v3: float,
-    x: float,
-    y: float,
-    z: float,
-):
-    """Creates a point light with the given color and position.
-
-    A point light emits light from a single point in all directions. Because
-    the light is emitted from a specific point (position), it has a different
-    effect when it is positioned farther vs. nearer an object.
-
-    A maximum of 5 point lights can be active at once.
-
-    Note: lights need to be called (whether directly or indirectly) within
-    draw() to remain persistent in a looping program. Placing them in setup()
-    will cause them to only have an effect the first time through the loop.
-    """
-    _p5js.pointLight(v1, v2, v3, x, y, z)
-
-
-def lights():
-    """Places an ambient and directional light in the scene.
-    The lights are set to ambient_light(128, 128, 128) and
-    directional_light(128, 128, 128, 0, 0, -1).
-
-    Note: lights need to be called (whether directly or indirectly) within
-    draw() to remain persistent in a looping program. Placing them in setup()
-    will cause them to only have an effect the first time through the loop.
-    """
-    _p5js.lights()
-
-
-def light_falloff(constant: float, linear: float, quadratic: float):
-    """Sets the falloff rate for point_light() and spot_light().
-
-    light_falloff() affects only the lights which are created after it in the
-    code.
-
-    The constant, linear, an quadratic parameters are used to calculate
-    falloff as follows:
-
-    d = distance from light position to vertex position
-
-    falloff = 1 / (CONSTANT + d * LINEAR + (d * d) * QUADRATIC)
-    """
-    _p5js.lightFalloff(constant, linear, quadratic)
-
-
-def spot_light(
-    v1: float,
-    v2: float,
-    v3: float,
-    x: float,
-    y: float,
-    z: float,
-    rx: float,
-    ry: float,
-    rz: float,
-    angle: float | None = None,
-    concentration: float | None = None,
-):
-    """Creates a spot light with the given color, position, light direction,
-    angle, and concentration.
-
-    Like a point_light(), a spot_light() emits light from a specific point
-    (position). It has a different effect when it is positioned farther vs.
-    nearer an object.
-
-    However, unlike a point_light(), the light is emitted in one direction
-    along a conical shape. The shape of the cone can be controlled using the
-    angle and concentration parameters.
-
-    The angle parameter is used to determine the radius of the cone. And the
-    concentration parameter is used to focus the light towards the center of
-    the cone. Both parameters are optional, however if you want to specify
-    concentration, you must also specify angle. The minimum concentration
-    value is 1.
-
-    A maximum of 5 spot lights can be active at once.
-
-    Note: lights need to be called (whether directly or indirectly) within
-    draw() to remain persistent in a looping program. Placing them in setup()
-    will cause them to only have an effect the first time through the loop.
-    """
-    if concentration:
-        _p5js.spotLight(v1, v2, v3, x, y, z, rx, ry, rz, angle, concentration)
-    elif angle:
-        _p5js.spotLight(v1, v2, v3, x, y, z, rx, ry, rz, angle)
-    else:
-        _p5js.spotLight(v1, v2, v3, x, y, z, rx, ry, rz)
-
-
-def no_lights():
-    """Removes all lights present in a sketch.
-
-    All subsequent geometry is rendered without lighting (until a new light
-    is created with a call to one of the lighting functions (lights(),
-    ambient_light(), directional_light(), point_light(), spot_light()).
-    """
-    _p5js.noLights()
-
-
-# ======
-# Camera
-# ======
-def camera(
-    x: float | None = None,
-    y: float | None = None,
-    z: float | None = None,
-    center_x: float | None = None,
-    center_y: float | None = None,
-    center_z: float | None = None,
-    up_x: float | None = None,
-    up_y: float | None = None,
-    up_z: float | None = None,
-):
-    """Sets the position of the current camera in a 3D sketch.
-    Parameters for this function define the camera's position, the center of
-    the sketch (where the camera is pointing), and an up direction (the
-    orientation of the camera).
-
-    This function simulates the movements of the camera, allowing objects to
-    be viewed from various angles. Remember, it does not move the objects
-    themselves but the camera instead. For example when the centerX value is
-    positive, and the camera is rotating to the right side of the sketch, the
-    object will seem like it's moving to the left.
-
-    See this example to view the position of your camera.
-
-    If no parameters are given, the following default is used:
-    camera(0, 0, (height/2) / tan(PI/6), 0, 0, 0, 0, 1, 0)
-    """
-    if not up_z:
-        _p5js.camera(0, 0, (_p5js.height * 0.5) / 0.5773502691896256, 0, 0, 0, 0, 1, 0)
-    else:
-        _p5js.camera(x, y, z, center_x, center_y, center_z, up_x, up_y, up_z)
-
-
-def perspective(
-    fovy: float | None = None,
-    aspect: float | None = None,
-    near: float | None = None,
-    far: float | None = None,
-):
-    """Sets a perspective projection for the current camera in a 3D sketch.
-    This projection represents depth through foreshortening: objects that are
-    close to the camera appear their actual size while those that are further
-    away from the camera appear smaller.
-
-    The parameters to this function define the viewing frustum (the truncated
-    pyramid within which objects are seen by the camera) through vertical
-    field of view, aspect ratio (usually width/height), and near and far
-    clipping planes.
-
-    If no parameters are given, the following default is used:
-    perspective(PI/3, width/height, eyeZ/10, eyeZ*10), where eyeZ is equal to
-    ((height/2) / tan(PI/6)).
-    """
-    if not far:
-        eye_z = _p5js.height * 0.5 / 0.5773502691896256
-        _p5js.perspective(
-            1.0471975511965976, _p5js.width / _p5js.height, eye_z * 0.1, eye_z * 10
-        )
-    else:
-        _p5js.perspective(fovy, aspect, near, far)
-
-
-def ortho(
-    left: float | None = None,
-    right: float | None = None,
-    bottom: float | None = None,
-    top: float | None = None,
-    near: float | None = None,
-    far: float | None = None,
-):
-    """Sets an orthographic projection for the current camera in a 3D sketch
-    and defines a box-shaped viewing frustum within which objects are seen.
-    In this projection, all objects with the same dimension appear the same
-    size, regardless of whether they are near or far from the camera.
-
-    The parameters to this function specify the viewing frustum where left and
-    right are the minimum and maximum x values, top and bottom are the minimum
-    and maximum y values, and near and far are the minimum and maximum z
-    values.
-
-    If no parameters are given, the following default is used:
-    ortho(-width/2, width/2, -height/2, height/2).
-    """
-    if not far:
-        _p5js.ortho(
-            -_p5js.width * 0.5,
-            _p5js.width * 0.5,
-            -_p5js.height * 0.5,
-            _p5js.height * 0.5,
-            _p5js.height * 0.5,
-            0,
-        )
-    else:
-        _p5js.ortho(left, right, bottom, top, near, far)
-
-
-def frustum(
-    left: float | None = None,
-    right: float | None = None,
-    bottom: float | None = None,
-    top: float | None = None,
-    near: float | None = None,
-    far: float | None = None,
-):
-    """Sets the frustum of the current camera as defined by the parameters.
-
-    A frustum is a geometric form: a pyramid with its top cut off. With the
-    viewer's eye at the imaginary top of the pyramid, the six planes of the
-    frustum act as clipping planes when rendering a 3D view. Thus, any form
-    inside the clipping planes is visible; anything outside those planes is
-    not visible.
-
-    Setting the frustum changes the perspective of the scene being rendered.
-    This can be achieved more simply in many cases by using perspective().
-
-    If no parameters are given, the following default is used:
-    frustum(-width/2, width/2, -height/2, height/2, 0, max(width, height)).
-    """
-    if not far:
-        _p5js.frustum(
-            -_p5js.width * 0.5,
-            _p5js.width * 0.5,
-            -_p5js.height * 0.5,
-            _p5js.height * 0.5,
-            0,
-            _p5js.max(_p5js.width, _p5js.height),
-        )
-    else:
-        _p5js.frustum(left, right, bottom, top, near, far)
-
-
-def create_camera() -> object:
-    """Creates a new p5.Camera object and sets it as the current (active)
-    camera.
-
-    The new camera is initialized with a default position (see camera()) and
-    a default perspective projection (see perspective()). Its properties can
-    be controlled with the p5.Camera methods.
-
-    Note: Every 3D sketch starts with a default camera initialized. This
-    camera can be controlled with the global methods camera(),
-    perspective(), ortho(), and frustum() if it is the only camera in the
-    scene.
-    """
-    return _p5js.createCamera()
-
-
-def set_camera(cam: object):
-    """Sets the current (active) camera of a 3D sketch.
-    Allows for switching between multiple cameras.
-    """
-    _p5js.setCamera(cam)
+class ThreeD(BaseSketch):
+    # ===========
+    # Interaction
+    # ===========
+    def orbit_control(
+        self,
+        sensitivity_x: float | None = None,
+        sensitivity_y: float | None = None,
+        sensitivity_z: float | None = None,
+    ):
+        """Allows movement around a 3D sketch using a mouse or trackpad.
+        Left-clicking and dragging will rotate the camera position about the
+        center of the sketch, right-clicking and dragging will pan the camera
+        position without rotation, and using the mouse wheel (scrolling) will
+        move the camera closer or further from the center of the sketch. This
+        function can be called with parameters dictating sensitivity to mouse
+        movement along the X and Y axes. Calling this function without parameters
+        is equivalent to calling orbit_control(1,1). To reverse direction of
+        movement in either axis, enter a negative number for sensitivity.
+        """
+        self._p5js.orbitControl(sensitivity_x, sensitivity_y, sensitivity_z)
+
+    def debug_mode(self, mode: str | None = None):
+        """debug_mode() helps visualize 3D space by adding a grid to indicate
+        where the ‘ground’ is in a sketch and an axes icon which indicates the +X,
+        +Y, and +Z directions. This function can be called without parameters to
+        create a default grid and axes icon. The grid is drawn using the most
+        recently set stroke color and weight. To specify these parameters, add a
+        call to stroke() and stroke_weight() just before the end of the draw()
+        loop.
+
+        By default, the grid will run through the origin (0,0,0) of the sketch
+        along the XZ plane and the axes icon will be offset from the origin. Both
+        the grid and axes icon will be sized according to the current canvas size.
+        Note that because the grid runs parallel to the default camera view, it is
+        often helpful to use debug_mode along with orbit_control to allow full
+        view of the grid.
+        """
+        self._p5js.debugMode(mode)
+
+    def no_debug_mode(self):
+        """Turns off debug_mode() in a 3D sketch."""
+        self._p5js.noDebugMode()
+
+    # ======
+    # Lights
+    # ======
+    def ambient_light(
+        self,
+        value: str | int | list[int],
+        v2: int | None = None,
+        v3: int | None = None,
+        v4: int | None = None,
+    ):
+        """Creates an ambient light with the given color.
+
+        Ambient light does not come from a specific direction. Objects are evenly
+        lit from all sides. Ambient lights are almost always used in combination
+        with other types of lights.
+
+        Note: lights need to be called (whether directly or indirectly) within
+        draw() to remain persistent in a looping program. Placing them in setup()
+        will cause them to only have an effect the first time through the loop.
+        """
+        if v4:
+            self._p5js.ambientLight(value, v2, v3, v4)
+        elif v3:
+            self._p5js.ambientLight(value, v2, v3)
+        elif v2:
+            self._p5js.ambientLight(value, v2)
+        else:
+            self._p5js.ambientLight(to_js(value))
+
+    def specular_color(
+        self,
+        value: str | int | list[int],
+        v2: int | None = None,
+        v3: int | None = None,
+    ):
+        """Sets the color of the specular highlight of a non-ambient light
+        (i.e. all lights except ambient_light()).
+
+        specularColor() affects only the lights which are created after it in the
+        code.
+
+        This function is used in combination with specular_material(). If a
+        geometry does not use specular_material(), this function will have no
+        effect.
+
+        The default color is white (255, 255, 255), which is used if
+        specular_color() is not explicitly called.
+
+        Note: specular_color is equivalent to the Processing function
+        lightSpecular.
+        """
+        if v3:
+            self._p5js.specularColor(value, v2, v3)
+        elif v2:
+            self._p5js.specularColor(value, v2)
+        else:
+            self._p5js.specularColor(to_js(value))
+
+    def directional_light(
+        self,
+        v1: float,
+        v2: float,
+        v3: float,
+        x: float,
+        y: float,
+        z: float,
+    ):
+        """Creates a directional light with the given color and direction.
+
+        Directional light comes from one direction. The direction is specified as
+        numbers inclusively between -1 and 1. For example, setting the direction
+        as (0, -1, 0) will cause the geometry to be lit from below (since the
+        light will be facing directly upwards). Similarly, setting the direction
+        as (1, 0, 0) will cause the geometry to be lit from the left (since the
+        light will be facing directly rightwards).
+
+        Directional lights do not have a specific point of origin, and therefore
+        cannot be positioned closer or farther away from a geometry.
+
+        A maximum of 5 directional lights can be active at once.
+
+        Note: lights need to be called (whether directly or indirectly) within
+        draw() to remain persistent in a looping program. Placing them in setup()
+        will cause them to only have an effect the first time through the loop.
+        """
+        self._p5js.directionalLight(v1, v2, v3, x, y, z)
+
+    def point_light(
+        self,
+        v1: float,
+        v2: float,
+        v3: float,
+        x: float,
+        y: float,
+        z: float,
+    ):
+        """Creates a point light with the given color and position.
+
+        A point light emits light from a single point in all directions. Because
+        the light is emitted from a specific point (position), it has a different
+        effect when it is positioned farther vs. nearer an object.
+
+        A maximum of 5 point lights can be active at once.
+
+        Note: lights need to be called (whether directly or indirectly) within
+        draw() to remain persistent in a looping program. Placing them in setup()
+        will cause them to only have an effect the first time through the loop.
+        """
+        self._p5js.pointLight(v1, v2, v3, x, y, z)
+
+    def lights(self):
+        """Places an ambient and directional light in the scene.
+        The lights are set to ambient_light(128, 128, 128) and
+        directional_light(128, 128, 128, 0, 0, -1).
+
+        Note: lights need to be called (whether directly or indirectly) within
+        draw() to remain persistent in a looping program. Placing them in setup()
+        will cause them to only have an effect the first time through the loop.
+        """
+        self._p5js.lights()
+
+    def light_falloff(self, constant: float, linear: float, quadratic: float):
+        """Sets the falloff rate for point_light() and spot_light().
+
+        light_falloff() affects only the lights which are created after it in the
+        code.
+
+        The constant, linear, an quadratic parameters are used to calculate
+        falloff as follows:
+
+        d = distance from light position to vertex position
+
+        falloff = 1 / (CONSTANT + d * LINEAR + (d * d) * QUADRATIC)
+        """
+        self._p5js.lightFalloff(constant, linear, quadratic)
+
+    def spot_light(
+        self,
+        v1: float,
+        v2: float,
+        v3: float,
+        x: float,
+        y: float,
+        z: float,
+        rx: float,
+        ry: float,
+        rz: float,
+        angle: float | None = None,
+        concentration: float | None = None,
+    ):
+        """Creates a spot light with the given color, position, light direction,
+        angle, and concentration.
+
+        Like a point_light(), a spot_light() emits light from a specific point
+        (position). It has a different effect when it is positioned farther vs.
+        nearer an object.
+
+        However, unlike a point_light(), the light is emitted in one direction
+        along a conical shape. The shape of the cone can be controlled using the
+        angle and concentration parameters.
+
+        The angle parameter is used to determine the radius of the cone. And the
+        concentration parameter is used to focus the light towards the center of
+        the cone. Both parameters are optional, however if you want to specify
+        concentration, you must also specify angle. The minimum concentration
+        value is 1.
+
+        A maximum of 5 spot lights can be active at once.
+
+        Note: lights need to be called (whether directly or indirectly) within
+        draw() to remain persistent in a looping program. Placing them in setup()
+        will cause them to only have an effect the first time through the loop.
+        """
+        if concentration:
+            self._p5js.spotLight(v1, v2, v3, x, y, z, rx, ry, rz, angle, concentration)
+        elif angle:
+            self._p5js.spotLight(v1, v2, v3, x, y, z, rx, ry, rz, angle)
+        else:
+            self._p5js.spotLight(v1, v2, v3, x, y, z, rx, ry, rz)
+
+    def no_lights(self):
+        """Removes all lights present in a sketch.
+
+        All subsequent geometry is rendered without lighting (until a new light
+        is created with a call to one of the lighting functions (lights(),
+        ambient_light(), directional_light(), point_light(), spot_light()).
+        """
+        self._p5js.noLights()
+
+    # ======
+    # Camera
+    # ======
+    def camera(
+        self,
+        x: float | None = None,
+        y: float | None = None,
+        z: float | None = None,
+        center_x: float | None = None,
+        center_y: float | None = None,
+        center_z: float | None = None,
+        up_x: float | None = None,
+        up_y: float | None = None,
+        up_z: float | None = None,
+    ):
+        """Sets the position of the current camera in a 3D sketch.
+        Parameters for this function define the camera's position, the center of
+        the sketch (where the camera is pointing), and an up direction (the
+        orientation of the camera).
+
+        This function simulates the movements of the camera, allowing objects to
+        be viewed from various angles. Remember, it does not move the objects
+        themselves but the camera instead. For example when the centerX value is
+        positive, and the camera is rotating to the right side of the sketch, the
+        object will seem like it's moving to the left.
+
+        See this example to view the position of your camera.
+
+        If no parameters are given, the following default is used:
+        camera(0, 0, (height/2) / tan(PI/6), 0, 0, 0, 0, 1, 0)
+        """
+        if not up_z:
+            self._p5js.camera(
+                0, 0, (self._p5js.height * 0.5) / 0.5773502691896256, 0, 0, 0, 0, 1, 0
+            )
+        else:
+            self._p5js.camera(x, y, z, center_x, center_y, center_z, up_x, up_y, up_z)
+
+    def perspective(
+        self,
+        fovy: float | None = None,
+        aspect: float | None = None,
+        near: float | None = None,
+        far: float | None = None,
+    ):
+        """Sets a perspective projection for the current camera in a 3D sketch.
+        This projection represents depth through foreshortening: objects that are
+        close to the camera appear their actual size while those that are further
+        away from the camera appear smaller.
+
+        The parameters to this function define the viewing frustum (the truncated
+        pyramid within which objects are seen by the camera) through vertical
+        field of view, aspect ratio (usually width/height), and near and far
+        clipping planes.
+
+        If no parameters are given, the following default is used:
+        perspective(PI/3, width/height, eyeZ/10, eyeZ*10), where eyeZ is equal to
+        ((height/2) / tan(PI/6)).
+        """
+        if not far:
+            eye_z = self._p5js.height * 0.5 / 0.5773502691896256
+            self._p5js.perspective(
+                1.0471975511965976,
+                self._p5js.width / self._p5js.height,
+                eye_z * 0.1,
+                eye_z * 10,
+            )
+        else:
+            self._p5js.perspective(fovy, aspect, near, far)
+
+    def ortho(
+        self,
+        left: float | None = None,
+        right: float | None = None,
+        bottom: float | None = None,
+        top: float | None = None,
+        near: float | None = None,
+        far: float | None = None,
+    ):
+        """Sets an orthographic projection for the current camera in a 3D sketch
+        and defines a box-shaped viewing frustum within which objects are seen.
+        In this projection, all objects with the same dimension appear the same
+        size, regardless of whether they are near or far from the camera.
+
+        The parameters to this function specify the viewing frustum where left and
+        right are the minimum and maximum x values, top and bottom are the minimum
+        and maximum y values, and near and far are the minimum and maximum z
+        values.
+
+        If no parameters are given, the following default is used:
+        ortho(-width/2, width/2, -height/2, height/2).
+        """
+        if not far:
+            self._p5js.ortho(
+                -self._p5js.width * 0.5,
+                self._p5js.width * 0.5,
+                -self._p5js.height * 0.5,
+                self._p5js.height * 0.5,
+                self._p5js.height * 0.5,
+                0,
+            )
+        else:
+            self._p5js.ortho(left, right, bottom, top, near, far)
+
+    def frustum(
+        self,
+        left: float | None = None,
+        right: float | None = None,
+        bottom: float | None = None,
+        top: float | None = None,
+        near: float | None = None,
+        far: float | None = None,
+    ):
+        """Sets the frustum of the current camera as defined by the parameters.
+
+        A frustum is a geometric form: a pyramid with its top cut off. With the
+        viewer's eye at the imaginary top of the pyramid, the six planes of the
+        frustum act as clipping planes when rendering a 3D view. Thus, any form
+        inside the clipping planes is visible; anything outside those planes is
+        not visible.
+
+        Setting the frustum changes the perspective of the scene being rendered.
+        This can be achieved more simply in many cases by using perspective().
+
+        If no parameters are given, the following default is used:
+        frustum(-width/2, width/2, -height/2, height/2, 0, max(width, height)).
+        """
+        if not far:
+            self._p5js.frustum(
+                -self._p5js.width * 0.5,
+                self._p5js.width * 0.5,
+                -self._p5js.height * 0.5,
+                self._p5js.height * 0.5,
+                0,
+                self._p5js.max(self._p5js.width, self._p5js.height),
+            )
+        else:
+            self._p5js.frustum(left, right, bottom, top, near, far)
+
+    def create_camera(self) -> object:
+        """Creates a new p5.Camera object and sets it as the current (active)
+        camera.
+
+        The new camera is initialized with a default position (see camera()) and
+        a default perspective projection (see perspective()). Its properties can
+        be controlled with the p5.Camera methods.
+
+        Note: Every 3D sketch starts with a default camera initialized. This
+        camera can be controlled with the global methods camera(),
+        perspective(), ortho(), and frustum() if it is the only camera in the
+        scene.
+        """
+        return self._p5js.createCamera()
+
+    def set_camera(self, cam: object):
+        """Sets the current (active) camera of a 3D sketch.
+        Allows for switching between multiple cameras.
+        """
+        self._p5js.setCamera(cam)
```

### Comparing `proceso-0.0.4/src/proceso/transform.py` & `proceso-0.0.6/src/proceso/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,174 +1,167 @@
 import collections
 from pyodide.ffi import to_js
 
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-def apply_matrix(
-    a: float | list[float],
-    b: float | None = None,
-    c: float | None = None,
-    d: float | None = None,
-    e: float | None = None,
-    f: float | None = None,
-    g: float | None = None,
-    h: float | None = None,
-    i: float | None = None,
-    j: float | None = None,
-    k: float | None = None,
-    l: float | None = None,
-    m: float | None = None,
-    n: float | None = None,
-    o: float | None = None,
-    p: float | None = None,
-):
-    """Multiplies the current matrix by the one specified through the
-    parameters.
-    This is a powerful operation that can perform the equivalent of translate,
-    scale, shear and rotate all at once. You can learn more about
-    transformation matrices online:
-
-    https://en.wikipedia.org/wiki/Transformation_matrix
-    
-    https://html.spec.whatwg.org/multipage/canvas.html#dom-context-2d-transform
-    """
-    if p:
-        _p5js.applyMatrix(a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p)
-    elif f:
-        _p5js.applyMatrix(a, b, c, d, e, f)
-    elif isinstance(a, collections.Sequence):
-        _p5js.applyMatrix(to_js(a))
-
-
-def reset_matrix():
-    """Replaces the current matrix with the identity matrix."""
-    _p5js.resetMatrix()
-
-
-def rotate(angle: float):
-    """Rotates a shape by the amount specified by the angle parameter.
-    This function accounts for angle_mode, so angles can be entered in either
-    RADIANS or DEGREES.
-
-    Objects are always rotated around their relative position to the origin
-    and positive numbers rotate objects in a clockwise direction.
-    Transformations apply to everything that happens after and subsequent
-    calls to the function accumulate the effect. For example, calling
-    rotate(HALF_PI) and then rotate(HALF_PI) is the same as rotate(PI).
-    All transformations are reset when draw() begins again.
-
-    Technically, rotate() multiplies the current transformation matrix by a
-    rotation matrix. This function can be further controlled by push() and
-    pop().
-    """
-    _p5js.rotate(angle)
-
-
-def rotate_x(angle: float):
-    """Rotates a shape around X axis by the amount specified in angle
-    parameter.
-    The angles can be entered in either RADIANS or DEGREES.
-
-    Objects are always rotated around their relative position to the origin
-    and positive numbers rotate objects in a clockwise direction. All
-    transformations are reset when draw() begins again.
-    """
-    _p5js.rotateX(angle)
-
-
-def rotate_y(angle: float):
-    """Rotates a shape around Y axis by the amount specified in angle
-    parameter.
-    The angles can be entered in either RADIANS or DEGREES.
-
-    Objects are always rotated around their relative position to the origin
-    and positive numbers rotate objects in a clockwise direction. All
-    transformations are reset when draw() begins again.
-    """
-    _p5js.rotateY(angle)
-
-
-def rotate_z(angle: float):
-    """Rotates a shape around Z axis by the amount specified in angle
-    parameter.
-    The angles can be entered in either RADIANS or DEGREES.
-
-    This method works in WEBGL mode only.
-
-    Objects are always rotated around their relative position to the origin
-    and positive numbers rotate objects in a clockwise direction. All
-    transformations are reset when draw() begins again.
-    """
-    _p5js.rotateZ(angle)
-
-
-def scale(s: float, y: float | None = None, z: float | None = None):
-    """Increases or decreases the size of a shape by expanding or
-    contracting vertices.
-    Objects always scale from their relative origin to the coordinate system.
-    Scale values are specified as decimal percentages. For example, the
-    function call scale(2.0) increases the dimension of a shape by 200%.
-
-    Transformations apply to everything that happens after and subsequent
-    calls to the function multiply the effect. For example, calling scale(2.0)
-    and then scale(1.5) is the same as scale(3.0). If scale() is called within
-    draw(), the transformation is reset when the loop begins again.
-
-    Using this function with the z parameter is only available in WEBGL mode.
-    This function can be further controlled with push() and pop().
-
-    """
-    _p5js.scale(s, y, z)
-
-
-def shear_x(angle: float):
-    """Shears a shape around the x-axis by the amount specified by the angle
-    parameter.
-    Angles should be specified in the current angleMode. Objects are always
-    sheared around their relative position to the origin and positive numbers
-    shear objects in a clockwise direction.
-
-    Transformations apply to everything that happens after and subsequent
-    calls to the function accumulates the effect. For example, calling
-    shear_x(PI/2) and then shear_x(PI/2) is the same as shear_x(PI). If
-    shear_x() is called within the draw(), the transformation is reset when
-    the loop begins again.
-
-    Technically, shear_x() multiplies the current transformation matrix by a
-    rotation matrix. This function can be further controlled by the push()
-    and pop() functions.
-    """
-    _p5js.shearX(angle)
-
-
-def shear_y(angle: float):
-    """Shears a shape around the y-axis the amount specified by the angle
-    parameter.
-    Angles should be specified in the current angleMode. Objects are always
-    sheared around their relative position to the origin and positive numbers
-    shear objects in a clockwise direction.
-
-    Transformations apply to everything that happens after and subsequent
-    calls to the function accumulates the effect. For example, calling
-    shear_y(PI/2) and then shear_y(PI/2) is the same as shear_y(PI). If
-    shear_y() is called within the draw(), the transformation is reset when
-    the loop begins again.
-
-    Technically, shear_y() multiplies the current transformation matrix by a rotation matrix. This function can be further controlled by the push() and pop() functions.
-    """
-    _p5js.shearY(angle)
-
-
-def translate(x: float, y: float, z: float | None = None):
-    """Specifies an amount to displace objects within the display window.
-    The x parameter specifies left/right translation, the y parameter
-    specifies up/down translation.
-
-    Transformations are cumulative and apply to everything that happens after
-    and subsequent calls to the function accumulates the effect. For example,
-    calling translate(50, 0) and then translate(20, 0) is the same as
-    translate(70, 0). If translate() is called within draw(), the
-    transformation is reset when the loop begins again. This function can be
-    further controlled by using push() and pop().
-    """
-    _p5js.translate(x, y, z)
+class Transform(BaseSketch):
+    def apply_matrix(
+        self,
+        a: float | list[float],
+        b: float | None = None,
+        c: float | None = None,
+        d: float | None = None,
+        e: float | None = None,
+        f: float | None = None,
+        g: float | None = None,
+        h: float | None = None,
+        i: float | None = None,
+        j: float | None = None,
+        k: float | None = None,
+        l: float | None = None,
+        m: float | None = None,
+        n: float | None = None,
+        o: float | None = None,
+        p: float | None = None,
+    ):
+        """Multiplies the current matrix by the one specified through the
+        parameters.
+        This is a powerful operation that can perform the equivalent of translate,
+        scale, shear and rotate all at once. You can learn more about
+        transformation matrices online:
+
+        https://en.wikipedia.org/wiki/Transformation_matrix
+
+        https://html.spec.whatwg.org/multipage/canvas.html#dom-context-2d-transform
+        """
+        if p:
+            self._p5js.applyMatrix(a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p)
+        elif f:
+            self._p5js.applyMatrix(a, b, c, d, e, f)
+        elif isinstance(a, collections.Sequence):
+            self._p5js.applyMatrix(to_js(a))
+
+    def reset_matrix(self):
+        """Replaces the current matrix with the identity matrix."""
+        self._p5js.resetMatrix()
+
+    def rotate(self, angle: float):
+        """Rotates a shape by the amount specified by the angle parameter.
+        This function accounts for angle_mode, so angles can be entered in either
+        RADIANS or DEGREES.
+
+        Objects are always rotated around their relative position to the origin
+        and positive numbers rotate objects in a clockwise direction.
+        Transformations apply to everything that happens after and subsequent
+        calls to the function accumulate the effect. For example, calling
+        rotate(HALF_PI) and then rotate(HALF_PI) is the same as rotate(PI).
+        All transformations are reset when draw() begins again.
+
+        Technically, rotate() multiplies the current transformation matrix by a
+        rotation matrix. This function can be further controlled by push() and
+        pop().
+        """
+        self._p5js.rotate(angle)
+
+    def rotate_x(self, angle: float):
+        """Rotates a shape around X axis by the amount specified in angle
+        parameter.
+        The angles can be entered in either RADIANS or DEGREES.
+
+        Objects are always rotated around their relative position to the origin
+        and positive numbers rotate objects in a clockwise direction. All
+        transformations are reset when draw() begins again.
+        """
+        self._p5js.rotateX(angle)
+
+    def rotate_y(self, angle: float):
+        """Rotates a shape around Y axis by the amount specified in angle
+        parameter.
+        The angles can be entered in either RADIANS or DEGREES.
+
+        Objects are always rotated around their relative position to the origin
+        and positive numbers rotate objects in a clockwise direction. All
+        transformations are reset when draw() begins again.
+        """
+        self._p5js.rotateY(angle)
+
+    def rotate_z(self, angle: float):
+        """Rotates a shape around Z axis by the amount specified in angle
+        parameter.
+        The angles can be entered in either RADIANS or DEGREES.
+
+        This method works in WEBGL mode only.
+
+        Objects are always rotated around their relative position to the origin
+        and positive numbers rotate objects in a clockwise direction. All
+        transformations are reset when draw() begins again.
+        """
+        self._p5js.rotateZ(angle)
+
+    def scale(self, s: float, y: float | None = None, z: float | None = None):
+        """Increases or decreases the size of a shape by expanding or
+        contracting vertices.
+        Objects always scale from their relative origin to the coordinate system.
+        Scale values are specified as decimal percentages. For example, the
+        function call scale(2.0) increases the dimension of a shape by 200%.
+
+        Transformations apply to everything that happens after and subsequent
+        calls to the function multiply the effect. For example, calling scale(2.0)
+        and then scale(1.5) is the same as scale(3.0). If scale() is called within
+        draw(), the transformation is reset when the loop begins again.
+
+        Using this function with the z parameter is only available in WEBGL mode.
+        This function can be further controlled with push() and pop().
+
+        """
+        self._p5js.scale(s, y, z)
+
+    def shear_x(self, angle: float):
+        """Shears a shape around the x-axis by the amount specified by the angle
+        parameter.
+        Angles should be specified in the current angleMode. Objects are always
+        sheared around their relative position to the origin and positive numbers
+        shear objects in a clockwise direction.
+
+        Transformations apply to everything that happens after and subsequent
+        calls to the function accumulates the effect. For example, calling
+        shear_x(PI/2) and then shear_x(PI/2) is the same as shear_x(PI). If
+        shear_x() is called within the draw(), the transformation is reset when
+        the loop begins again.
+
+        Technically, shear_x() multiplies the current transformation matrix by a
+        rotation matrix. This function can be further controlled by the push()
+        and pop() functions.
+        """
+        self._p5js.shearX(angle)
+
+    def shear_y(self, angle: float):
+        """Shears a shape around the y-axis the amount specified by the angle
+        parameter.
+        Angles should be specified in the current angleMode. Objects are always
+        sheared around their relative position to the origin and positive numbers
+        shear objects in a clockwise direction.
+
+        Transformations apply to everything that happens after and subsequent
+        calls to the function accumulates the effect. For example, calling
+        shear_y(PI/2) and then shear_y(PI/2) is the same as shear_y(PI). If
+        shear_y() is called within the draw(), the transformation is reset when
+        the loop begins again.
+
+        Technically, shear_y() multiplies the current transformation matrix by a rotation matrix. This function can be further controlled by the push() and pop() functions.
+        """
+        self._p5js.shearY(angle)
+
+    def translate(self, x: float, y: float, z: float | None = None):
+        """Specifies an amount to displace objects within the display window.
+        The x parameter specifies left/right translation, the y parameter
+        specifies up/down translation.
+
+        Transformations are cumulative and apply to everything that happens after
+        and subsequent calls to the function accumulates the effect. For example,
+        calling translate(50, 0) and then translate(20, 0) is the same as
+        translate(70, 0). If translate() is called within draw(), the
+        transformation is reset when the loop begins again. This function can be
+        further controlled by using push() and pop().
+        """
+        self._p5js.translate(x, y, z)
```

### Comparing `proceso-0.0.4/src/proceso/typography.py` & `proceso-0.0.6/src/proceso/typography.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,139 @@
-from ._binding import _p5js
+from ._binding import BaseSketch
 
 
-# ==========
-# Attributes
-# ==========
-def text_align(horiz_align: str, vert_align: str | None = None):
-    """Sets the current alignment for drawing text.
-    Accepts two arguments: horiz_align (LEFT, CENTER, or RIGHT) and
-    vert_align (TOP, BOTTOM, CENTER, or BASELINE).
-
-    The horiz_align parameter is in reference to the x value of the text()
-    function, while the vert_align parameter is in reference to the y value.
-
-    So if you write text_align(LEFT), you are aligning the left edge of your
-    text to the x value you give in text(). If you write
-    text_align(RIGHT, TOP), you are aligning the right edge of your text to
-    the x value and the top edge of the text to the y value.
-    """
-    _p5js.textAlign(horiz_align, vert_align)
-
-
-def text_leading(leading: float):
-    """Sets/gets the spacing, in pixels, between lines of text.
-    This setting will be used in all subsequent calls to the text() function.
-    """
-    _p5js.textAlign(leading)
-
-
-def text_size(size: float) -> float:
-    """Sets/gets the current font size.
-    This size will be used in all subsequent calls to the text() function.
-    Font size is measured in pixels.
-    """
-    return _p5js.textSize(size)
-
-
-def text_style(style: str):
-    """Sets/gets the style of the text for system fonts to NORMAL, ITALIC,
-    BOLD or BOLDITALIC.
-    Note: this may be is overridden by CSS styling. For non-system fonts
-    (opentype, truetype, etc.) please load styled fonts instead.
-    """
-    _p5js.textStyle(style)
-
-
-def text_width(text: str) -> float:
-    """Calculates and returns the width of any character or text string."""
-    return _p5js.textWidth(text)
-
-
-def text_ascent() -> float:
-    """Returns the ascent of the current font at its current size.
-    The ascent represents the distance, in pixels, of the tallest character
-    above the baseline.
-    """
-    return _p5js.textAscent()
-
-
-def text_descent() -> float:
-    """Returns the descent of the current font at its current size.
-    The descent represents the distance, in pixels, of the character with the
-    longest descender below the baseline.
-    """
-    return _p5js.textDescent()
-
-
-def text_wrap(style: str):
-    """Specifies how lines of text are wrapped within a text box.
-    This requires a max-width set on the text area, specified in text() as
-    parameter x2.
-
-    WORD wrap style only breaks lines at spaces. A single string without
-    spaces that exceeds the boundaries of the canvas or text area is not
-    truncated, and will overflow the desired area, disappearing at the canvas
-    edge.
-
-    CHAR wrap style breaks lines wherever needed to stay within the text box.
-
-    WORD is the default wrap style, and both styles will still break lines at
-    any line breaks (\n) specified in the original text. The text area
-    max-height parameter (y2) also still applies to wrapped text in both
-    styles, lines of text that do not fit within the text area will not be
-    drawn to the screen.
-    """
-    _p5js.textWrap(style)
-
-
-# ====================
-# Loading & Displaying
-# ====================
-def load_font(path: str) -> object:
-    """Loads an opentype font file (.otf, .ttf) from a file or a URL, and
-    returns a p5.Font object.
-    This function is asynchronous, meaning it may not finish before the next
-    line in your sketch is executed.
-
-    The path to the font should be relative to the HTML file that links in
-    your sketch. Loading fonts from a URL or other remote location may be
-    blocked due to your browser's built-in security.
-    """
-    return _p5js.loadFont(path)
-
-
-def text(
-    txt: str, x: float, y: float, x2: float | None = None, y2: float | None = None
-):
-    """Draws text to the screen.
-    Displays the information specified in the first parameter on the screen in
-    the position specified by the additional parameters. A default font will
-    be used unless a font is set with the textFont() function and a default
-    size will be used unless a font is set with text_size(). Change the color
-    of the text with the fill() function. Change the outline of the text with
-    the stroke() and strokeWeight() functions.
-
-    The text displays in relation to the text_align() function, which gives
-    the option to draw to the left, right, and center of the coordinates.
-
-    The x2 and y2 parameters define a rectangular area to display within and
-    may only be used with string data. When these parameters are specified,
-    they are interpreted based on the current rect_mode() setting. Text that
-    does not fit completely within the rectangle specified will not be drawn
-    to the screen. If x2 and y2 are not specified, the baseline alignment is
-    the default, which means that the text will be drawn upwards from x and y.
-
-    WEBGL: Only opentype/truetype fonts are supported. You must load a font
-    using the loadFont() method (see the example above). stroke() currently
-    has no effect in WebGL mode. Learn more about working with text in WebGL
-    mode on the wiki.
-    """
-    _p5js.text(txt, x, y, x2, y2)
-
-
-def text_font(font: str | object, size: float | None = None):
-    """Sets the current font that will be drawn with the text() function.
-    If text_font() is called without any argument, it will return the current
-    font if one has been set already. If not, it will return the name of the
-    default font as a string. If text_font() is called with a font to use, it
-    will return the p5 object.
-
-    WEBGL: Only fonts loaded via load_font() are supported.
-    """
-    _p5js.textFont(font, size)
+class Typography(BaseSketch):
+    # ==========
+    # Attributes
+    # ==========
+    def text_align(self, horiz_align: str, vert_align: str | None = None):
+        """Sets the current alignment for drawing text.
+        Accepts two arguments: horiz_align (LEFT, CENTER, or RIGHT) and
+        vert_align (TOP, BOTTOM, CENTER, or BASELINE).
+
+        The horiz_align parameter is in reference to the x value of the text()
+        function, while the vert_align parameter is in reference to the y value.
+
+        So if you write text_align(LEFT), you are aligning the left edge of your
+        text to the x value you give in text(). If you write
+        text_align(RIGHT, TOP), you are aligning the right edge of your text to
+        the x value and the top edge of the text to the y value.
+        """
+        self._p5js.textAlign(horiz_align, vert_align)
+
+    def text_leading(self, leading: float):
+        """Sets/gets the spacing, in pixels, between lines of text.
+        This setting will be used in all subsequent calls to the text() function.
+        """
+        self._p5js.textAlign(leading)
+
+    def text_size(self, size: float) -> float:
+        """Sets/gets the current font size.
+        This size will be used in all subsequent calls to the text() function.
+        Font size is measured in pixels.
+        """
+        return self._p5js.textSize(size)
+
+    def text_style(self, style: str):
+        """Sets/gets the style of the text for system fonts to NORMAL, ITALIC,
+        BOLD or BOLDITALIC.
+        Note: this may be is overridden by CSS styling. For non-system fonts
+        (opentype, truetype, etc.) please load styled fonts instead.
+        """
+        self._p5js.textStyle(style)
+
+    def text_width(self, text: str) -> float:
+        """Calculates and returns the width of any character or text string."""
+        return self._p5js.textWidth(text)
+
+    def text_ascent(self) -> float:
+        """Returns the ascent of the current font at its current size.
+        The ascent represents the distance, in pixels, of the tallest character
+        above the baseline.
+        """
+        return self._p5js.textAscent()
+
+    def text_descent(self) -> float:
+        """Returns the descent of the current font at its current size.
+        The descent represents the distance, in pixels, of the character with the
+        longest descender below the baseline.
+        """
+        return self._p5js.textDescent()
+
+    def text_wrap(self, style: str):
+        """Specifies how lines of text are wrapped within a text box.
+        This requires a max-width set on the text area, specified in text() as
+        parameter x2.
+
+        WORD wrap style only breaks lines at spaces. A single string without
+        spaces that exceeds the boundaries of the canvas or text area is not
+        truncated, and will overflow the desired area, disappearing at the canvas
+        edge.
+
+        CHAR wrap style breaks lines wherever needed to stay within the text box.
+
+        WORD is the default wrap style, and both styles will still break lines at
+        any line breaks (\n) specified in the original text. The text area
+        max-height parameter (y2) also still applies to wrapped text in both
+        styles, lines of text that do not fit within the text area will not be
+        drawn to the screen.
+        """
+        self._p5js.textWrap(style)
+
+    # ====================
+    # Loading & Displaying
+    # ====================
+    def load_font(self, path: str) -> object:
+        """Loads an opentype font file (.otf, .ttf) from a file or a URL, and
+        returns a p5.Font object.
+        This function is asynchronous, meaning it may not finish before the next
+        line in your sketch is executed.
+
+        The path to the font should be relative to the HTML file that links in
+        your sketch. Loading fonts from a URL or other remote location may be
+        blocked due to your browser's built-in security.
+        """
+        return self._p5js.loadFont(path)
+
+    def text(
+        self,
+        txt: str,
+        x: float,
+        y: float,
+        x2: float | None = None,
+        y2: float | None = None,
+    ):
+        """Draws text to the screen.
+        Displays the information specified in the first parameter on the screen in
+        the position specified by the additional parameters. A default font will
+        be used unless a font is set with the textFont() function and a default
+        size will be used unless a font is set with text_size(). Change the color
+        of the text with the fill() function. Change the outline of the text with
+        the stroke() and strokeWeight() functions.
+
+        The text displays in relation to the text_align() function, which gives
+        the option to draw to the left, right, and center of the coordinates.
+
+        The x2 and y2 parameters define a rectangular area to display within and
+        may only be used with string data. When these parameters are specified,
+        they are interpreted based on the current rect_mode() setting. Text that
+        does not fit completely within the rectangle specified will not be drawn
+        to the screen. If x2 and y2 are not specified, the baseline alignment is
+        the default, which means that the text will be drawn upwards from x and y.
+
+        WEBGL: Only opentype/truetype fonts are supported. You must load a font
+        using the loadFont() method (see the example above). stroke() currently
+        has no effect in WebGL mode. Learn more about working with text in WebGL
+        mode on the wiki.
+        """
+        self._p5js.text(txt, x, y, x2, y2)
+
+    def text_font(self, font: str | object, size: float | None = None):
+        """Sets the current font that will be drawn with the text() function.
+        If text_font() is called without any argument, it will return the current
+        font if one has been set already. If not, it will return the name of the
+        default font as a string. If text_font() is called with a font to use, it
+        will return the p5 object.
+
+        WEBGL: Only fonts loaded via load_font() are supported.
+        """
+        self._p5js.textFont(font, size)
```

### Comparing `proceso-0.0.4/src/proceso.egg-info/PKG-INFO` & `proceso-0.0.6/src/proceso.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proceso
-Version: 0.0.4
+Version: 0.0.6
 Summary: A Python package for creative coding on the web.
 Home-page: https://github.com/nickmcintyre/proceso
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -43,15 +43,18 @@
     <py-script src="sketch.py"></py-script>
 </body>
 
 </html>
 ```
 
 ```python
-import proceso as p5
+from proceso import Sketch
+
+
+p5 = Sketch()
 
 
 pos = p5.Vector(200, 200)
 vel = p5.Vector.random(2)
 r = 25
 
 
@@ -73,15 +76,15 @@
     if pos.y < r or pos.y > p5.height - r:
         vel.y *= -1
 
     if p5.is_mouse_pressed == True:
         p5.background("dodgerblue")
 
 
-p5.run(setup=setup, draw=draw)
+p5.run_sketch(setup=setup, draw=draw)
 ```
 
 # Roadmap
 - Improve documentation
 - Fix known bugs
 - Finish API
 - Support JupyterLite
```

### Comparing `proceso-0.0.4/src/proceso.egg-info/SOURCES.txt` & `proceso-0.0.6/src/proceso.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/proceso/__init__.py
 src/proceso/_binding.py
-src/proceso/_setup.py
 src/proceso/colors.py
 src/proceso/constants.py
 src/proceso/data.py
 src/proceso/dom.py
 src/proceso/environment.py
 src/proceso/events.py
 src/proceso/images.py
 src/proceso/rendering.py
 src/proceso/shape.py
 src/proceso/structure.py
+src/proceso/sysvars.py
 src/proceso/three_d.py
 src/proceso/transform.py
 src/proceso/typography.py
 src/proceso.egg-info/PKG-INFO
 src/proceso.egg-info/SOURCES.txt
 src/proceso.egg-info/dependency_links.txt
 src/proceso.egg-info/requires.txt
```

