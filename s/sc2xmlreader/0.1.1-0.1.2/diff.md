# Comparing `tmp/sc2xmlreader-0.1.1.tar.gz` & `tmp/sc2xmlreader-0.1.2.tar.gz`

## Comparing `sc2xmlreader-0.1.1.tar` & `sc2xmlreader-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/integration_test/README
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/integration_test/demoLocal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/integration_test/sc2xmlreader_dev/__init__.py
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/integration_test/sc2xmlreader_dev/const.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/integration_test/sc2xmlreader_dev/sc2xmlreader.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/src/sc2xmlreader/__init__.py
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/src/sc2xmlreader/const.py
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/src/sc2xmlreader/sc2xmlreader.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/src/sc2xmlreader/sc2xmlreader_validator.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/tests/test_sc2xmlreader.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/tests/test_sc2xmlreader_validator.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/LICENSE
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/README.md
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/integration_test/README
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/integration_test/demoLocal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/integration_test/sc2xmlreader_dev/__init__.py
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/integration_test/sc2xmlreader_dev/const.py
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/integration_test/sc2xmlreader_dev/sc2xmlreader.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/src/sc2xmlreader/__init__.py
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/src/sc2xmlreader/const.py
+-rw-r--r--   0        0        0    11413 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/src/sc2xmlreader/sc2xmlreader.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/src/sc2xmlreader/sc2xmlreader_validator.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/tests/test_sc2xmlreader.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/tests/test_sc2xmlreader_validator.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/README.md
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 sc2xmlreader-0.1.2/PKG-INFO
```

### Comparing `sc2xmlreader-0.1.1/integration_test/demoLocal.py` & `sc2xmlreader-0.1.2/integration_test/demoLocal.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/integration_test/sc2xmlreader_dev/const.py` & `sc2xmlreader-0.1.2/integration_test/sc2xmlreader_dev/const.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/integration_test/sc2xmlreader_dev/sc2xmlreader.py` & `sc2xmlreader-0.1.2/integration_test/sc2xmlreader_dev/sc2xmlreader.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py` & `sc2xmlreader-0.1.2/integration_test/sc2xmlreader_dev/sc2xmlreader_validator.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/src/sc2xmlreader/const.py` & `sc2xmlreader-0.1.2/src/sc2xmlreader/const.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/src/sc2xmlreader/sc2xmlreader.py` & `sc2xmlreader-0.1.2/src/sc2xmlreader/sc2xmlreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         )
 
         data_array[self.MAP_SOLVIS_TO_NAME["BC"]] = self.create_data_entry(
             "BC", "Capacity Oil Burner", round(self.burner_capacity, 2), "kW"
         )
 
         value_float = 0.0
-        value_float = data_array["Z1"]["Value"] * self.burner_capacity
+        value_float = data_array[self.MAP_SOLVIS_TO_NAME["Z1"]]["Value"] * self.burner_capacity
         data_array[self.MAP_SOLVIS_TO_NAME["OC"]] = self.create_data_entry(
             "OC", "Power Consumption Oil Burner", round(value_float, 2), "kWh"
         )
 
         value_float = 0.0
         if (self.solar):
             value_float = data_array["temperature_solar_flow"]["Value"] - data_array["temperature_solar_return"]["Value"]
```

### Comparing `sc2xmlreader-0.1.1/src/sc2xmlreader/sc2xmlreader_validator.py` & `sc2xmlreader-0.1.2/src/sc2xmlreader/sc2xmlreader_validator.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/tests/test_sc2xmlreader.py` & `sc2xmlreader-0.1.2/tests/test_sc2xmlreader.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/tests/test_sc2xmlreader_validator.py` & `sc2xmlreader-0.1.2/tests/test_sc2xmlreader_validator.py`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/.gitignore` & `sc2xmlreader-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/LICENSE` & `sc2xmlreader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/README.md` & `sc2xmlreader-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sc2xmlreader-0.1.1/pyproject.toml` & `sc2xmlreader-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sc2xmlreader"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="lurchi70", email="hjleu@web.de" },
 ]
 description = "Reads and interprets XML data from solvis remote device"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sc2xmlreader-0.1.1/PKG-INFO` & `sc2xmlreader-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc2xmlreader
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reads and interprets XML data from solvis remote device
 Project-URL: Homepage, https://github.com/Lurchi70/sc2xmlreader_pypi_package
 Project-URL: Bug Tracker, https://github.com/Lurchi70/sc2xmlreader_pypi_package/issues
 Author-email: lurchi70 <hjleu@web.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

