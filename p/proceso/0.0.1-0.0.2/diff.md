# Comparing `tmp/proceso-0.0.1.tar.gz` & `tmp/proceso-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proceso-0.0.1.tar", last modified: Sun Apr 30 22:22:37 2023, max compression
+gzip compressed data, was "proceso-0.0.2.tar", last modified: Mon May  1 13:06:09 2023, max compression
```

## Comparing `proceso-0.0.1.tar` & `proceso-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-30 22:22:37.610510 proceso-0.0.1/
--rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.1/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     3026 2023-04-30 22:22:37.610558 proceso-0.0.1/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     2386 2023-04-30 21:36:21.000000 proceso-0.0.1/README.md
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.1/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      778 2023-04-30 22:22:37.610795 proceso-0.0.1/setup.cfg
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-30 22:22:37.606214 proceso-0.0.1/src/
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-30 22:22:37.609086 proceso-0.0.1/src/proceso/
--rw-r--r--   0 nick       (501) staff       (20)    24088 2023-04-30 22:18:14.000000 proceso-0.0.1/src/proceso/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)       30 2023-04-30 21:10:44.000000 proceso-0.0.1/src/proceso/_binding.py
--rw-r--r--   0 nick       (501) staff       (20)      151 2023-04-30 21:10:54.000000 proceso-0.0.1/src/proceso/_setup.py
--rw-r--r--   0 nick       (501) staff       (20)    10191 2023-04-30 21:10:45.000000 proceso-0.0.1/src/proceso/colors.py
--rw-r--r--   0 nick       (501) staff       (20)     5736 2023-04-30 21:10:46.000000 proceso-0.0.1/src/proceso/constants.py
--rw-r--r--   0 nick       (501) staff       (20)     3250 2023-04-30 21:10:47.000000 proceso-0.0.1/src/proceso/data.py
--rw-r--r--   0 nick       (501) staff       (20)     8302 2023-04-30 22:18:10.000000 proceso-0.0.1/src/proceso/dom.py
--rw-r--r--   0 nick       (501) staff       (20)     8041 2023-04-30 21:10:49.000000 proceso-0.0.1/src/proceso/environment.py
--rw-r--r--   0 nick       (501) staff       (20)     1316 2023-04-30 21:10:50.000000 proceso-0.0.1/src/proceso/events.py
--rw-r--r--   0 nick       (501) staff       (20)    12620 2023-04-30 21:10:51.000000 proceso-0.0.1/src/proceso/images.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-30 22:22:37.610373 proceso-0.0.1/src/proceso/math/
--rw-r--r--   0 nick       (501) staff       (20)      543 2023-04-30 03:13:34.000000 proceso-0.0.1/src/proceso/math/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5281 2023-04-30 21:22:53.000000 proceso-0.0.1/src/proceso/math/calculation.py
--rw-r--r--   0 nick       (501) staff       (20)     3371 2023-04-30 21:22:51.000000 proceso-0.0.1/src/proceso/math/noise.py
--rw-r--r--   0 nick       (501) staff       (20)     1543 2023-04-29 23:47:36.000000 proceso-0.0.1/src/proceso/math/random.py
--rw-r--r--   0 nick       (501) staff       (20)     3428 2023-04-30 21:22:44.000000 proceso-0.0.1/src/proceso/math/trigonometry.py
--rw-r--r--   0 nick       (501) staff       (20)    61234 2023-04-29 22:58:38.000000 proceso-0.0.1/src/proceso/math/vector.py
--rw-r--r--   0 nick       (501) staff       (20)     4857 2023-04-30 21:10:52.000000 proceso-0.0.1/src/proceso/rendering.py
--rw-r--r--   0 nick       (501) staff       (20)    27097 2023-04-30 21:10:55.000000 proceso-0.0.1/src/proceso/shape.py
--rw-r--r--   0 nick       (501) staff       (20)     5609 2023-04-30 21:10:56.000000 proceso-0.0.1/src/proceso/structure.py
--rw-r--r--   0 nick       (501) staff       (20)    13897 2023-04-30 21:10:57.000000 proceso-0.0.1/src/proceso/three_d.py
--rw-r--r--   0 nick       (501) staff       (20)     6642 2023-04-30 21:23:05.000000 proceso-0.0.1/src/proceso/transform.py
--rw-r--r--   0 nick       (501) staff       (20)     5575 2023-04-30 21:10:59.000000 proceso-0.0.1/src/proceso/typography.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-30 22:22:37.609686 proceso-0.0.1/src/proceso.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     3026 2023-04-30 22:22:37.000000 proceso-0.0.1/src/proceso.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      762 2023-04-30 22:22:37.000000 proceso-0.0.1/src/proceso.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-30 22:22:37.000000 proceso-0.0.1/src/proceso.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       12 2023-04-30 22:22:37.000000 proceso-0.0.1/src/proceso.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        8 2023-04-30 22:22:37.000000 proceso-0.0.1/src/proceso.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.219085 proceso-0.0.2/
+-rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.2/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     3026 2023-05-01 13:06:09.219133 proceso-0.0.2/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     2386 2023-04-30 21:36:21.000000 proceso-0.0.2/README.md
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.2/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-01 13:06:09.219378 proceso-0.0.2/setup.cfg
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.214849 proceso-0.0.2/src/
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.217652 proceso-0.0.2/src/proceso/
+-rw-r--r--   0 nick       (501) staff       (20)    24151 2023-05-01 13:05:56.000000 proceso-0.0.2/src/proceso/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)       30 2023-04-30 21:10:44.000000 proceso-0.0.2/src/proceso/_binding.py
+-rw-r--r--   0 nick       (501) staff       (20)      151 2023-04-30 21:10:54.000000 proceso-0.0.2/src/proceso/_setup.py
+-rw-r--r--   0 nick       (501) staff       (20)    10191 2023-04-30 21:10:45.000000 proceso-0.0.2/src/proceso/colors.py
+-rw-r--r--   0 nick       (501) staff       (20)     5797 2023-05-01 12:51:28.000000 proceso-0.0.2/src/proceso/constants.py
+-rw-r--r--   0 nick       (501) staff       (20)     3250 2023-04-30 21:10:47.000000 proceso-0.0.2/src/proceso/data.py
+-rw-r--r--   0 nick       (501) staff       (20)     8302 2023-04-30 22:18:10.000000 proceso-0.0.2/src/proceso/dom.py
+-rw-r--r--   0 nick       (501) staff       (20)     8041 2023-04-30 21:10:49.000000 proceso-0.0.2/src/proceso/environment.py
+-rw-r--r--   0 nick       (501) staff       (20)     1316 2023-04-30 21:10:50.000000 proceso-0.0.2/src/proceso/events.py
+-rw-r--r--   0 nick       (501) staff       (20)    12620 2023-04-30 21:10:51.000000 proceso-0.0.2/src/proceso/images.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.218936 proceso-0.0.2/src/proceso/math/
+-rw-r--r--   0 nick       (501) staff       (20)      543 2023-04-30 03:13:34.000000 proceso-0.0.2/src/proceso/math/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     5281 2023-04-30 21:22:53.000000 proceso-0.0.2/src/proceso/math/calculation.py
+-rw-r--r--   0 nick       (501) staff       (20)     3371 2023-04-30 21:22:51.000000 proceso-0.0.2/src/proceso/math/noise.py
+-rw-r--r--   0 nick       (501) staff       (20)     1543 2023-04-29 23:47:36.000000 proceso-0.0.2/src/proceso/math/random.py
+-rw-r--r--   0 nick       (501) staff       (20)     3428 2023-04-30 21:22:44.000000 proceso-0.0.2/src/proceso/math/trigonometry.py
+-rw-r--r--   0 nick       (501) staff       (20)    61234 2023-04-29 22:58:38.000000 proceso-0.0.2/src/proceso/math/vector.py
+-rw-r--r--   0 nick       (501) staff       (20)     4857 2023-04-30 21:10:52.000000 proceso-0.0.2/src/proceso/rendering.py
+-rw-r--r--   0 nick       (501) staff       (20)    27097 2023-04-30 21:10:55.000000 proceso-0.0.2/src/proceso/shape.py
+-rw-r--r--   0 nick       (501) staff       (20)     5609 2023-04-30 21:10:56.000000 proceso-0.0.2/src/proceso/structure.py
+-rw-r--r--   0 nick       (501) staff       (20)    13928 2023-05-01 12:39:40.000000 proceso-0.0.2/src/proceso/three_d.py
+-rw-r--r--   0 nick       (501) staff       (20)     6642 2023-04-30 21:23:05.000000 proceso-0.0.2/src/proceso/transform.py
+-rw-r--r--   0 nick       (501) staff       (20)     5575 2023-04-30 21:10:59.000000 proceso-0.0.2/src/proceso/typography.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-01 13:06:09.218244 proceso-0.0.2/src/proceso.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     3026 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      762 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-01 13:06:09.000000 proceso-0.0.2/src/proceso.egg-info/top_level.txt
```

### Comparing `proceso-0.0.1/LICENSE` & `proceso-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/PKG-INFO` & `proceso-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proceso
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for creative coding on the web.
 Home-page: https://github.com/nickmcintyre/proceso
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `proceso-0.0.1/README.md` & `proceso-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/setup.cfg` & `proceso-0.0.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = proceso
-version = 0.0.1
+version = 0.0.2
 author = Nick McIntyre
 author_email = nick@mcintyre.io
 description = A Python package for creative coding on the web.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nickmcintyre/proceso
 project_urls =
```

### Comparing `proceso-0.0.1/src/proceso/__init__.py` & `proceso-0.0.2/src/proceso/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,17 @@
     # ACCESSIBILITY
     GRID,
     AXES,
     LABEL,
     FALLBACK,
     CONTAIN,
     COVER,
+    # CAMERA
+    VIDEO,
+    AUDIO,
 )
 from .colors import (
     # Creating & Reading
     alpha,
     blue,
     brightness,
     color,
@@ -334,15 +337,15 @@
 )
 from .three_d import (
     # Interaction
     orbit_control,
     debug_mode,
     no_debug_mode,
     # Lights
-    lights,
+    ambient_light,
     specular_color,
     directional_light,
     point_light,
     lights,
     light_falloff,
     spot_light,
     no_lights,
@@ -873,10 +876,10 @@
     if callable(mouse_wheel):
         _p5js.mouseWheel = create_proxy(mouse_wheel)
     if callable(request_pointer_lock):
         _p5js.requestPointerLock = create_proxy(request_pointer_lock)
     if callable(exit_pointer_lock):
         _p5js.exitPointerLock = create_proxy(exit_pointer_lock)
 
-    # FIXME: This is a hack
+    # FIXME: This is a hack to make preload work
     _p5js.remove()
     _init_global_mode()
```

### Comparing `proceso-0.0.1/src/proceso/colors.py` & `proceso-0.0.2/src/proceso/colors.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/constants.py` & `proceso-0.0.2/src/proceso/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,7 +270,12 @@
 LABEL: str = _p5js.LABEL
 
 FALLBACK: str = _p5js.FALLBACK
 
 CONTAIN: str = _p5js.CONTAIN
 
 COVER: str = _p5js.COVER
+
+# CAMERA
+VIDEO: str = _p5js.VIDEO
+
+AUDIO: str = _p5js.AUDIO
```

### Comparing `proceso-0.0.1/src/proceso/data.py` & `proceso-0.0.2/src/proceso/data.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/dom.py` & `proceso-0.0.2/src/proceso/dom.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/environment.py` & `proceso-0.0.2/src/proceso/environment.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/events.py` & `proceso-0.0.2/src/proceso/events.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/images.py` & `proceso-0.0.2/src/proceso/images.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/math/__init__.py` & `proceso-0.0.2/src/proceso/math/__init__.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/math/calculation.py` & `proceso-0.0.2/src/proceso/math/calculation.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/math/noise.py` & `proceso-0.0.2/src/proceso/math/noise.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/math/random.py` & `proceso-0.0.2/src/proceso/math/random.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/math/trigonometry.py` & `proceso-0.0.2/src/proceso/math/trigonometry.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/math/vector.py` & `proceso-0.0.2/src/proceso/math/vector.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/rendering.py` & `proceso-0.0.2/src/proceso/rendering.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/shape.py` & `proceso-0.0.2/src/proceso/shape.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/structure.py` & `proceso-0.0.2/src/proceso/structure.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/three_d.py` & `proceso-0.0.2/src/proceso/three_d.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     """Turns off debug_mode() in a 3D sketch."""
     _p5js.noDebugMode()
 
 
 # ======
 # Lights
 # ======
-def lights(
+def ambient_light(
     value: str | int | list[int],
     v2: int | None = None,
     v3: int | None = None,
     v4: int | None = None,
 ):
     """Creates an ambient light with the given color.
 
@@ -64,21 +64,21 @@
     with other types of lights.
 
     Note: lights need to be called (whether directly or indirectly) within
     draw() to remain persistent in a looping program. Placing them in setup()
     will cause them to only have an effect the first time through the loop.
     """
     if v4:
-        _p5js.lights(value, v2, v3, v4)
+        _p5js.ambientLight(value, v2, v3, v4)
     elif v3:
-        _p5js.lights(value, v2, v3)
+        _p5js.ambientLight(value, v2, v3)
     elif v2:
-        _p5js.lights(value, v2)
+        _p5js.ambientLight(value, v2)
     else:
-        _p5js.lights(to_js(value))
+        _p5js.ambientLight(to_js(value))
 
 
 def specular_color(
     value: str | int | list[int],
     v2: int | None = None,
     v3: int | None = None,
 ):
```

### Comparing `proceso-0.0.1/src/proceso/transform.py` & `proceso-0.0.2/src/proceso/transform.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso/typography.py` & `proceso-0.0.2/src/proceso/typography.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.1/src/proceso.egg-info/PKG-INFO` & `proceso-0.0.2/src/proceso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proceso
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for creative coding on the web.
 Home-page: https://github.com/nickmcintyre/proceso
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `proceso-0.0.1/src/proceso.egg-info/SOURCES.txt` & `proceso-0.0.2/src/proceso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

