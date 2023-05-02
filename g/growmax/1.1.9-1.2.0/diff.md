# Comparing `tmp/growmax-1.1.9.tar.gz` & `tmp/growmax-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growmax-1.1.9.tar", last modified: Sun Mar 26 02:48:31 2023, max compression
+gzip compressed data, was "growmax-1.2.0.tar", last modified: Tue May  2 07:05:33 2023, max compression
```

## Comparing `growmax-1.1.9.tar` & `growmax-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-26 02:48:16.000000 growmax-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-26 02:48:31.922046 growmax-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-26 02:48:16.000000 growmax-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-26 02:48:16.000000 growmax-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-26 02:48:31.922046 growmax-1.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.918046 growmax-1.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.918046 growmax-1.1.9/src/growmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/atlas_ph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/import_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/set_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/atlas_ph/uart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/displays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/displays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/displays/sh1107.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/displays/ssd1327.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/moisture.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/ntpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/pump.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/routine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/sensors/adafruit_scd4x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.922046 growmax-1.1.9/src/growmax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/water.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-26 02:48:16.000000 growmax-1.1.9/src/growmax/utils/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 02:48:31.918046 growmax-1.1.9/src/growmax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-26 02:48:31.000000 growmax-1.1.9/src/growmax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.574210 growmax-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-02 07:05:21.000000 growmax-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-02 07:05:33.574210 growmax-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-02 07:05:21.000000 growmax-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 07:05:21.000000 growmax-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 07:05:33.574210 growmax-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.566210 growmax-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/atlas_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/import_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/set_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/uart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/displays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/displays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/displays/sh1107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/displays/ssd1327.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/moisture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/ntpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/pump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/routine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/sensors/adafruit_scd4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/sensors/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.574210 growmax-1.2.0/src/growmax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/top_level.txt
```

### Comparing `growmax-1.1.9/LICENSE` & `growmax-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/PKG-INFO` & `growmax-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.1.9
+Version: 1.2.0
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.1.9/README.md` & `growmax-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/setup.cfg` & `growmax-1.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = growmax
-version = 1.1.9
+version = 1.2.0
 author = Matt Davis and OpenSensor.io
 author_email = matteius@gmail.com
 description = Micropython routines for automated plant watering and monitoring.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/opensensor/growmax
 project_urls =
```

### Comparing `growmax-1.1.9/src/growmax/atlas_ph/calibration.py` & `growmax-1.2.0/src/growmax/atlas_ph/calibration.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax/atlas_ph/i2c.py` & `growmax-1.2.0/src/growmax/atlas_ph/i2c.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import machine
 import utime
-from growmax.utils.i2c import i2c_channel_pins
+from growmax.utils.mcu import i2c_channel_pins
 
 import config
 
 
 DEFAULT_ADDRESS = 0x63
```

### Comparing `growmax-1.1.9/src/growmax/config.py` & `growmax-1.2.0/src/growmax/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,20 +29,22 @@
 ATLAS_PH_I2C_CHANNEL = 0
 ATLAS_PH_METER_ADDRESS = None
 
 # I2C Displays
 DISPLAY = None   # To enable a display, define an import from growmax.displays, Ex: "SSD1327_I2C", "SH1107_I2C"
 DISPLAY_I2C_CHANNEL = 0  # 0 for QWIIC_I2C0 or 1 for QWIIC_I2C1
 DISPLAY_I2C_ADDRESS = None  # The address of the display
-DISPLAY_SWITCH = None  # Set GPIO Pin number of the input switch
-DISPLAY_SWITCH_PULL = None  # Set to be None, machine.Pin.PULL_UP or machine.Pin.PULL_DOOWN
+DISPLAY_SWITCH = None  # Set GPIO Pin of the input switch or None to disable
+DISPLAY_SWITCH_CLASS = None  # When set to None, Pin is used directly with interrupt.  Also available: "MotionSensor"
+DISPLAY_SWITCH_DURATION_MS = 10000  # When using MotionSensor, this sets how long to turn on display for in ms
+DISPLAY_SWITCH_PULL = None  # When using pin directly: Set to be None, machine.Pin.PULL_UP or machine.Pin.PULL_DOWN
 DISPLAY_SWITCH_TRIGGER = machine.Pin.IRQ_FALLING | machine.Pin.IRQ_RISING
 
 # Wi-Fi SSID and password
 WIFI_ENABLED = False
 WIFI_SSID = "SSID"
 WIFI_PASSWORD = ""
 
 # Data collection w/ api.opensensor.io (early alpha testing)
-OPEN_SENSOR_COLLECT_DATA = False  # Please don't enable this for now
-OPEN_SENSOR_API_KEY = None  # Not yet supported
+OPEN_SENSOR_COLLECT_DATA = False
+OPEN_SENSOR_API_KEY = None  # Register your device for a key at https://opensensor.io/members/profile
 DEVICE_NAME = ""
```

### Comparing `growmax-1.1.9/src/growmax/constants.py` & `growmax-1.2.0/src/growmax/constants.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax/displays/sh1107.py` & `growmax-1.2.0/src/growmax/displays/sh1107.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax/displays/ssd1327.py` & `growmax-1.2.0/src/growmax/displays/ssd1327.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax/moisture.py` & `growmax-1.2.0/src/growmax/moisture.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,14 @@
         """
         rp2040_pin = constants.MOISTURE_GPIOS[channel - 1]
         self._gpio_pin = get_gpio_for_mcu(rp2040_pin)
         pin = machine.Pin(self._gpio_pin, machine.Pin.IN, machine.Pin.PULL_UP)
 
         self._count = 0
         self._reading = 0
-        self._history = []
-        self._history_length = 200
         self._last_pulse = utime.time()
         self._new_data = False
         self._wet_point = wet_point if wet_point is not None else 0.7
         self._dry_point = dry_point if dry_point is not None else 27.6
         self._time_last_reading = utime.time()
         try:
             pin.irq(trigger=machine.Pin.IRQ_RISING, handler=self._event_handler)
@@ -42,32 +40,19 @@
         self._time_start = utime.time()
 
     def _event_handler(self, pin):
         self._count += 1
         self._last_pulse = utime.time()
         if self._time_elapsed >= 3.0:
             self._reading = self._count / self._time_elapsed
-            self._history.insert(0, self._reading)
-            self._history = self._history[:self._history_length]
             self._count = 0
             self._time_last_reading = utime.time()
             self._new_data = True
 
     @property
-    def history(self):
-        history = []
-
-        for moisture in self._history:
-            saturation = float(moisture - self._dry_point) / self.range
-            saturation = round(saturation, 3)
-            history.append(max(0.0, min(1.0, saturation)))
-
-        return history
-
-    @property
     def _time_elapsed(self):
         return utime.time() - self._time_last_reading
 
     def set_wet_point(self, value=None):
         """Set the sensor wet point.
         This is the watered, wet state of your soil.
         It should be set shortly after watering. Leave ~5 mins for moisture to permeate.
```

### Comparing `growmax-1.1.9/src/growmax/ntpclient.py` & `growmax-1.2.0/src/growmax/ntpclient.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax/pump.py` & `growmax-1.2.0/src/growmax/pump.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax/routine.py` & `growmax-1.2.0/src/growmax/routine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import gc
 import random
 import utime
 from machine import Pin
 
+from growmax.atlas_ph.i2c import AtlasPHI2C
 from growmax.moisture import Moisture
 from growmax.pump import Pump
 from growmax.utils import api
 from growmax.utils.configs import get_moisture_threshold_for_position
-from growmax.utils.displays import boot_sequence, display_basic_stats, display_ph_reading
+from growmax.utils.displays import boot_sequence, display_basic_stats, display_ph_reading, display_scd4x_reading
+from growmax.utils.mcu import get_gpio_for_mcu
+from growmax.utils.sensors import init_adafruit_scd4x, read_adafruit_scd4x
 from growmax.utils.water import statistically_has_water
 from growmax.utils.wifi import ensure_wifi_connected
 
 # User's config file
 import config
 
 # set the random seed, so messages are randomized
@@ -19,15 +22,15 @@
 
 
 def main():
     boot_sequence()
 
     water_sensor = None
     if config.WATER_SENSOR_LOW_ENABLED:
-        water_sensor = Pin(config.WATER_SENSOR_LOW, Pin.IN, Pin.PULL_DOWN)
+        water_sensor = Pin(get_gpio_for_mcu(config.WATER_SENSOR_LOW), Pin.IN, Pin.PULL_DOWN)
     scd40x = None
     atlas_ph = None
 
     soil_sensors = [Moisture(channel=1), Moisture(channel=2), Moisture(channel=3), Moisture(channel=4),
                     Moisture(channel=5), Moisture(channel=6), Moisture(channel=7), Moisture(channel=8)]
     pumps = [Pump(channel=1), Pump(channel=2), Pump(channel=3), Pump(channel=4),
              Pump(channel=5), Pump(channel=6), Pump(channel=7), Pump(channel=8)]
@@ -38,20 +41,21 @@
             ensure_wifi_connected()
             utime.sleep(0.5)
         except Exception:
             # Potentially no wi-fi
             pass
 
         if config.ADAFRUIT_SCD4X_ENABLED and scd40x is None:
-            from growmax.utils.sensors import init_adafruit_scd4x
             scd40x = init_adafruit_scd4x(config.ADAFRUIT_SCD4X_I2C_CHANNEL)
 
         if hasattr(config, "ATLAS_PH_METER_ENABLED") and config.ATLAS_PH_METER_ENABLED:
-            from growmax.atlas_ph.i2c import AtlasPHI2C
-            atlas_ph = AtlasPHI2C(config.ATLAS_PH_I2C_CHANNEL)
+            try:
+                atlas_ph = AtlasPHI2C(config.ATLAS_PH_I2C_CHANNEL)
+            except Exception as e:
+                print(f"Error initializing Atlas pH probe: {e}")
 
         soil_moistures = []
         for position, soil_sensor in enumerate(soil_sensors):
             try:
                 pump_position = str(position + 1)
                 soil_moisture = soil_sensor.moisture
                 soil_moistures.append(soil_moisture)
@@ -64,27 +68,37 @@
                 if (config.PUMP_WHEN_DRY or has_water) and soil_moisture >= moisture_config:
                     print("position: ", pump_position)
                     pumps[position].dose(1, config.PUMP_CYCLE_DURATION)
                 utime.sleep(2)
             except Exception as e:
                 print("Exception: ", str(e))
 
+        ph_reading = None
+        temp, rh, ppm_carbon_dioxide = None, None, None
+        if atlas_ph:
+            utime.sleep(1.0)
+            ph_reading = atlas_ph.obtain_ph_reading()
+        if scd40x:
+            temp, rh, ppm_carbon_dioxide = read_adafruit_scd4x(scd40x)
         if config.OPEN_SENSOR_COLLECT_DATA:
             report_data = api.get_device_metadata()
             if scd40x:
-                api.read_adafruit_scd4x_(scd40x, report_data)
+                api.add_adafruit_scd4x_data_to_report(report_data, temp, rh, ppm_carbon_dioxide)
             report_data["moisture"] = {
                 "readings": soil_moistures
             }
+            if atlas_ph and ph_reading:
+                report_data["pH"] = {
+                    "pH": ph_reading
+                }
             api.report_environment_data(report_data)
-        elif scd40x:
-                from growmax.utils.sensors import read_adafruit_scd4x
-                read_adafruit_scd4x(scd40x)
+        if scd40x:
+            display_scd4x_reading(temp, rh, ppm_carbon_dioxide)
+            utime.sleep(3)
         if atlas_ph:
-            ph_reading = atlas_ph.obtain_ph_reading()
             display_ph_reading(ph_reading)
             utime.sleep(3)
 
         print("Completed iteration; soil_moisture's = ", str(soil_moistures))
         print("Free mem before garbage collection: ", str(gc.mem_free()))
         gc.collect()
         print("Free mem after garbage collection: ", str(gc.mem_free()))
```

### Comparing `growmax-1.1.9/src/growmax/sensors/adafruit_scd4x.py` & `growmax-1.2.0/src/growmax/sensors/adafruit_scd4x.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax/utils/api.py` & `growmax-1.2.0/src/growmax/utils/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import machine
 import ubinascii
 import time
-from growmax.utils import sensors
 
 import config
 
 headers = {'content-type': 'application/json'}
 
 
 def get_device_metadata():
@@ -13,46 +12,44 @@
     try:
         time.sleep(1.0)
         device_id = ubinascii.hexlify(machine.unique_id()).decode()
         time.sleep(1.0)
         report_data["device_metadata"] = {
             "device_id": device_id,
             "name": config.DEVICE_NAME,
+            "api_key": config.OPEN_SENSOR_API_KEY,
         }
     except Exception as e:
         print(e)
     return report_data
 
 
-def read_adafruit_scd4x_(scd4x, report_data):
-    try:
-        time.sleep(1.0)
-        data = sensors.read_adafruit_scd4x(scd4x)
-        time.sleep(1.0)
+def add_adafruit_scd4x_data_to_report(report_data, temp, rh, ppm_carbon_dioxide):
+    if temp:
         report_data["temp"] = {
-            "temp": data[0],
+            "temp": temp,
             "unit": "C"
         }
+    if rh:
         report_data["rh"] = {
-            "rh": data[1],
+            "rh": rh,
         }
+    if ppm_carbon_dioxide:
         report_data["co2"] = {
-            "ppm": data[2],
+            "ppm": ppm_carbon_dioxide,
         }
-    except Exception as e:
-        print(e)
 
 
 def report_environment_data(report_data):
-    """This method requires installing urequests and ujson from pypi."""
+    """ This method requires installing urequests from pypi. """
     try:
         import urequests
-        import ujson
+        import json
         time.sleep(1.0)
         resp = urequests.post(
             "https://api.opensensor.io/environment/",
             headers=headers,
-            data=ujson.dumps(report_data))
+            data=json.dumps(report_data))
         print(resp.status_code)
         resp.close()
     except Exception as e:
         print(e)
```

### Comparing `growmax-1.1.9/src/growmax/utils/sensors.py` & `growmax-1.2.0/src/growmax/utils/sensors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import machine
 import time
 from growmax.sensors import adafruit_scd4x
-from growmax.utils.i2c import i2c_channel_pins
+from growmax.utils.mcu import i2c_channel_pins
 
 
 def init_adafruit_scd4x(i2c_channel=0):
     pin_scl, pin_sda = i2c_channel_pins(i2c_channel)
     try:
         time.sleep(2.0)
         i2c = machine.I2C(
             i2c_channel,
             scl=machine.Pin(pin_scl),
             sda=machine.Pin(pin_sda),
-            freq=5000
+            freq=100000
         )
         time.sleep(2.0)
         scd4x = adafruit_scd4x.SCD4X(i2c)
         time.sleep(2.0)
         print("Serial number:", [hex(i) for i in scd4x.serial_number])
         time.sleep(1.0)
         scd4x.start_periodic_measurement()
@@ -25,17 +25,15 @@
         return scd4x
     except Exception as e:
         print(e)
     return None
 
 
 def read_adafruit_scd4x(scd4x):
+    time.sleep(2.0)
     if scd4x.data_ready:
         ppm_carbon_dioxide = scd4x.CO2
         temp = scd4x.temperature
         rh = scd4x.relative_humidity
-        print("Temperature: %0.1f *C" % temp)
-        print("Humidity: %0.1f %%" % rh)
-        print("CO2: %d ppm" % ppm_carbon_dioxide)
         return [temp, rh, ppm_carbon_dioxide]
     print("SCD-40 data not available")
-    return []
+    return [None, None, None]
```

### Comparing `growmax-1.1.9/src/growmax/utils/wifi.py` & `growmax-1.2.0/src/growmax/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `growmax-1.1.9/src/growmax.egg-info/PKG-INFO` & `growmax-1.2.0/src/growmax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.1.9
+Version: 1.2.0
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.1.9/src/growmax.egg-info/SOURCES.txt` & `growmax-1.2.0/src/growmax.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 src/growmax/atlas_ph/set_i2c.py
 src/growmax/atlas_ph/uart_read.py
 src/growmax/displays/__init__.py
 src/growmax/displays/sh1107.py
 src/growmax/displays/ssd1327.py
 src/growmax/sensors/__init__.py
 src/growmax/sensors/adafruit_scd4x.py
+src/growmax/sensors/motion.py
 src/growmax/utils/__init__.py
 src/growmax/utils/api.py
 src/growmax/utils/configs.py
 src/growmax/utils/displays.py
-src/growmax/utils/i2c.py
 src/growmax/utils/mcu.py
 src/growmax/utils/sensors.py
 src/growmax/utils/water.py
 src/growmax/utils/wifi.py
```

