# Comparing `tmp/sc2xmlreader-0.0.8.tar.gz` & `tmp/sc2xmlreader-0.1.0.tar.gz`

## Comparing `sc2xmlreader-0.0.8.tar` & `sc2xmlreader-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/integration_test/README
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/integration_test/demoLocal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/integration_test/sc2xmlreader_dev/__init__.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/integration_test/sc2xmlreader_dev/const.py
--rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/integration_test/sc2xmlreader_dev/sc2xmlreader.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/src/sc2xmlreader/__init__.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/src/sc2xmlreader/const.py
--rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/src/sc2xmlreader/sc2xmlreader.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/src/sc2xmlreader/sc2xmlreader_validator.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/tests/test_sc2xmlreader.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/tests/test_sc2xmlreader_validator.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/LICENSE
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/README.md
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 sc2xmlreader-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/integration_test/README
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/integration_test/demoLocal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/integration_test/sc2xmlreader_dev/__init__.py
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/integration_test/sc2xmlreader_dev/const.py
+-rw-r--r--   0        0        0    11228 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/integration_test/sc2xmlreader_dev/sc2xmlreader.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/src/sc2xmlreader/__init__.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/src/sc2xmlreader/const.py
+-rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/src/sc2xmlreader/sc2xmlreader.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/src/sc2xmlreader/sc2xmlreader_validator.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/tests/test_sc2xmlreader.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/tests/test_sc2xmlreader_validator.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/README.md
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.0/PKG-INFO
```

### Comparing `sc2xmlreader-0.0.8/integration_test/demoLocal.py` & `sc2xmlreader-0.1.0/integration_test/demoLocal.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/integration_test/sc2xmlreader_dev/const.py` & `sc2xmlreader-0.1.0/src/sc2xmlreader/const.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/integration_test/sc2xmlreader_dev/sc2xmlreader.py` & `sc2xmlreader-0.1.0/src/sc2xmlreader/sc2xmlreader.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py` & `sc2xmlreader-0.1.0/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/src/sc2xmlreader/const.py` & `sc2xmlreader-0.1.0/integration_test/sc2xmlreader_dev/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 MAP_SOLVIS_TO_NAME_BASIC["A6"] = "heating_circuit_3_pump"
 MAP_SOLVIS_TO_NAME_BASIC["A7"] = "NA"
 MAP_SOLVIS_TO_NAME_BASIC["A1"] = "NA"
 MAP_SOLVIS_TO_NAME_BASIC["A2"] = "NA"
 MAP_SOLVIS_TO_NAME_BASIC["RF1"] = "temperature_room_1"
 MAP_SOLVIS_TO_NAME_BASIC["RF2"] = "temperature_room_2"
 MAP_SOLVIS_TO_NAME_BASIC["RF3"] = "temperature_room_3"
+MAP_SOLVIS_TO_NAME_BASIC["BC"] = "burner_capacity"
+MAP_SOLVIS_TO_NAME_BASIC["OC"] = "burner_consumption"
 
 MAP_SOLVIS_TO_NAME_WITH_WARM_WATER_STATION = dict()
 MAP_SOLVIS_TO_NAME_WITH_WARM_WATER_STATION["S2"] = "temperature_warm_water_station"
 MAP_SOLVIS_TO_NAME_WITH_WARM_WATER_STATION["S11"] = "temperature_circulation"
 MAP_SOLVIS_TO_NAME_WITH_WARM_WATER_STATION["S18"] = "volume_stream_warm_water"
 MAP_SOLVIS_TO_NAME_WITH_WARM_WATER_STATION["A2"] = "warm_water_station_pump"
 MAP_SOLVIS_TO_NAME_WITH_WARM_WATER_STATION["A5"] = "circulation_pump"
```

### Comparing `sc2xmlreader-0.0.8/src/sc2xmlreader/sc2xmlreader.py` & `sc2xmlreader-0.1.0/integration_test/sc2xmlreader_dev/sc2xmlreader.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,31 +24,33 @@
     heating_circuit_2_sensor: bool
     heating_circuit_3: str | None
     heating_circuit_3_sensor: bool
 
     manufacturer: str | None
     model: str | None
     name: str | None
+    burner_capacity : float
     sw_version: str | None
     hw_version: str | None
     via_device: tuple[str, str]
 
-    def __init__(self, url: str, username: str, password: str, withWarmWaterStation=True, withSolar=True, withEastWest=False, withOven=False) -> None:
+    def __init__(self, url: str, username: str, password: str, withWarmWaterStation=True, withSolar=True, withEastWest=False, withOven=False, burnerCapacity=27.0) -> None:
         """Initialize the data interpreter."""
         self.data = {}
         self.MAP_SOLVIS_TO_NAME = MAP_SOLVIS_TO_NAME_BASIC
         uri = f"""{url}/sc2_val.xml"""
 
         self.solar = withSolar
         self.east_west_solar = withEastWest
 
         self.oven = withOven
         self.warm_water_station = withWarmWaterStation
         self.manufacturer = HEATING_MANUFACTURER
         self.model = HEATING_DEVICE_TYPE.SolvisMax.name
+        self.burner_capacity = burnerCapacity
         self.name = None
         self.sw_version = None
         self.hw_version = None
 
         try:
             basic = HTTPDigestAuth(username, password)
             response = requests.get(uri, stream=True, auth=basic, timeout=10)
@@ -216,19 +218,25 @@
         value_float = value_int / 10
         data_sc2 = data_sc2[4:]
         data_array[self.MAP_SOLVIS_TO_NAME["SL"]] = self.create_data_entry(
             "SL", "Solarpower", value_float, "kW"
         )
 
         value_float = 0.0
+        value_float = data_array["Z1"]["Value"] * self.burner_capacity;
+        data_array[self.MAP_SOLVIS_TO_NAME["OC"]] = self.create_data_entry(
+            "OC", "Power Consumption Oil Burner", round(value_float, 2), "kWh"
+        )
+
+        value_float = 0.0
         if (self.solar):
             value_float = data_array["temperature_solar_flow"]["Value"] - data_array["temperature_solar_return"]["Value"]
         data_array[self.MAP_SOLVIS_TO_NAME["SD"]] = self.create_data_entry(
             "SD", "Delta Solar Flow and Return ", round(value_float, 2), "°K"
-        )
+        )        
 
         return data_array
 
     def print_data(self, array_=None):
         """Write sensor data to logger."""
         for value_ in array_:
             if value_["Key"][0:1] == "S":
```

### Comparing `sc2xmlreader-0.0.8/src/sc2xmlreader/sc2xmlreader_validator.py` & `sc2xmlreader-0.1.0/src/sc2xmlreader/sc2xmlreader_validator.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/tests/test_sc2xmlreader.py` & `sc2xmlreader-0.1.0/tests/test_sc2xmlreader.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/tests/test_sc2xmlreader_validator.py` & `sc2xmlreader-0.1.0/tests/test_sc2xmlreader_validator.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/.gitignore` & `sc2xmlreader-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/LICENSE` & `sc2xmlreader-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.0.8/README.md` & `sc2xmlreader-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -58,16 +58,20 @@
 
 ## Sensor data provided
 The following sensors are available in the data:
 
 | key | name                         | Unit   | Description   |
 |-----|------------------------------|--------|:-------------------------------------------|
 | time| last_update                  |        | Timestamp of latest data update.                |
+| Z1  | runtime_burner               | h      | Total runtime of the oil burner. |
+| Z2  | total_burner_start           |        | Total number of oil burner starts. |
+| Z3  | total_burner_2nd_start       |        | Total number of 2nd oil burner starts. |
 | Z4  | runtime_solar_pump           | h      | Total output runtime of the solar pump. |
 | SL  | solar_power                  | W      | Current solar power from the solar panels. |
+| SD  | temperature_solar_diff_flow_return | °K | Temperature difference between solar flow and solar return. |
 | S7  | solar_pressure               | bar    | Current pressure in the solar pipes. |
 | SE  | solar_yield                  | kWh    | Total yield of the solar panels to the heating system |
 | S1  | temperature_buffer_top       | °C     | current temperature in the buffer top |
 | S3  | temperature_buffer_reference | °C     | current reference temperature in the buffer |
 | S4  | temperature_H_buffer_top     | °C     | current temperature in the heating buffer top |
 | S9  | temperature_H_buffer_bottom  | °C     | current temperature in the heating buffer bottom |
 | S2  | temperature_warm_water_station | °C     | current temperature warm water station |
@@ -78,14 +82,16 @@
 | S5  | temperature_solar_flow       | °C     | current flow temperature of solar heating  |
 | S8  | temperature_solar_panel      | °C     | current temperature on the solar panel(s)  |
 | S16 | temperature_solar_panel2     | °C     | current temperature on the solar2 panel(s) (if east/ west option) |
 | S16 | temperature_oven             | °C     | current temperature on the solar2 panel(s) (if oven option) |
 | S6  | temperature_solar_return     | °C     | current return temperature of solar heating  |
 | S17 | volume_solar_pump            | l/h    | current volume of fluid stream in solar heating  |
 | S18 | volume_warm_water            | l/min  | current volume of fluid stream in warm water station  |
+| BC  | burner_capacity              | kW     | capacity of oil burner |
+| OC  | burner_power_consumption     | kWh    | Power consumption of oil burner (calculated)  |
 
 ## Binary states
 The following binary states are available in the data:
 
 |     | name                         | Description   |
 |-----|------------------------------|:-------------------------------------------|
 | A12 | burner                       | oil/gas burner started. |
```

### Comparing `sc2xmlreader-0.0.8/pyproject.toml` & `sc2xmlreader-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sc2xmlreader"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   { name="lurchi70", email="hjleu@web.de" },
 ]
 description = "Reads and interprets XML data from solvis remote device"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sc2xmlreader-0.0.8/PKG-INFO` & `sc2xmlreader-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc2xmlreader
-Version: 0.0.8
+Version: 0.1.0
 Summary: Reads and interprets XML data from solvis remote device
 Project-URL: Homepage, https://github.com/Lurchi70/sc2xmlreader_pypi_package
 Project-URL: Bug Tracker, https://github.com/Lurchi70/sc2xmlreader_pypi_package/issues
 Author-email: lurchi70 <hjleu@web.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -75,16 +75,20 @@
 
 ## Sensor data provided
 The following sensors are available in the data:
 
 | key | name                         | Unit   | Description   |
 |-----|------------------------------|--------|:-------------------------------------------|
 | time| last_update                  |        | Timestamp of latest data update.                |
+| Z1  | runtime_burner               | h      | Total runtime of the oil burner. |
+| Z2  | total_burner_start           |        | Total number of oil burner starts. |
+| Z3  | total_burner_2nd_start       |        | Total number of 2nd oil burner starts. |
 | Z4  | runtime_solar_pump           | h      | Total output runtime of the solar pump. |
 | SL  | solar_power                  | W      | Current solar power from the solar panels. |
+| SD  | temperature_solar_diff_flow_return | °K | Temperature difference between solar flow and solar return. |
 | S7  | solar_pressure               | bar    | Current pressure in the solar pipes. |
 | SE  | solar_yield                  | kWh    | Total yield of the solar panels to the heating system |
 | S1  | temperature_buffer_top       | °C     | current temperature in the buffer top |
 | S3  | temperature_buffer_reference | °C     | current reference temperature in the buffer |
 | S4  | temperature_H_buffer_top     | °C     | current temperature in the heating buffer top |
 | S9  | temperature_H_buffer_bottom  | °C     | current temperature in the heating buffer bottom |
 | S2  | temperature_warm_water_station | °C     | current temperature warm water station |
@@ -95,14 +99,16 @@
 | S5  | temperature_solar_flow       | °C     | current flow temperature of solar heating  |
 | S8  | temperature_solar_panel      | °C     | current temperature on the solar panel(s)  |
 | S16 | temperature_solar_panel2     | °C     | current temperature on the solar2 panel(s) (if east/ west option) |
 | S16 | temperature_oven             | °C     | current temperature on the solar2 panel(s) (if oven option) |
 | S6  | temperature_solar_return     | °C     | current return temperature of solar heating  |
 | S17 | volume_solar_pump            | l/h    | current volume of fluid stream in solar heating  |
 | S18 | volume_warm_water            | l/min  | current volume of fluid stream in warm water station  |
+| BC  | burner_capacity              | kW     | capacity of oil burner |
+| OC  | burner_power_consumption     | kWh    | Power consumption of oil burner (calculated)  |
 
 ## Binary states
 The following binary states are available in the data:
 
 |     | name                         | Description   |
 |-----|------------------------------|:-------------------------------------------|
 | A12 | burner                       | oil/gas burner started. |
```

