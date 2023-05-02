# Comparing `tmp/amazon-braket-pennylane-plugin-1.8.0.tar.gz` & `tmp/amazon-braket-pennylane-plugin-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-pennylane-plugin-1.8.0.tar", last modified: Fri Sep 16 19:18:14 2022, max compression
+gzip compressed data, was "amazon-braket-pennylane-plugin-1.9.0.tar", last modified: Wed Sep 21 16:15:50 2022, max compression
```

## Comparing `amazon-braket-pennylane-plugin-1.8.0.tar` & `amazon-braket-pennylane-plugin-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 19:18:14.706418 amazon-braket-pennylane-plugin-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     7646 2022-09-16 19:18:14.706418 amazon-braket-pennylane-plugin-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6773 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-16 19:18:14.706418 amazon-braket-pennylane-plugin-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 19:18:14.702418 amazon-braket-pennylane-plugin-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 19:18:14.702418 amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7646 2022-09-16 19:18:14.000000 amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-09-16 19:18:14.000000 amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 19:18:14.000000 amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-16 19:18:14.000000 amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-09-16 19:18:14.000000 amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-16 19:18:14.000000 amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 19:18:14.702418 amazon-braket-pennylane-plugin-1.8.0/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 19:18:14.706418 amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    18283 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/braket_device.py
--rw-r--r--   0 runner    (1001) docker     (121)    13651 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)    13737 2022-09-16 19:18:06.000000 amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/translation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 16:15:50.777763 amazon-braket-pennylane-plugin-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     7646 2022-09-21 16:15:50.777763 amazon-braket-pennylane-plugin-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6773 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-21 16:15:50.777763 amazon-braket-pennylane-plugin-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 16:15:50.777763 amazon-braket-pennylane-plugin-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 16:15:50.777763 amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7646 2022-09-21 16:15:50.000000 amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-09-21 16:15:50.000000 amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 16:15:50.000000 amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-21 16:15:50.000000 amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-09-21 16:15:50.000000 amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-21 16:15:50.000000 amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 16:15:50.777763 amazon-braket-pennylane-plugin-1.9.0/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 16:15:50.777763 amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18283 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/braket_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13651 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/ops.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13849 2022-09-21 16:15:43.000000 amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/translation.py
```

### Comparing `amazon-braket-pennylane-plugin-1.8.0/LICENSE` & `amazon-braket-pennylane-plugin-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/PKG-INFO` & `amazon-braket-pennylane-plugin-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-pennylane-plugin
-Version: 1.8.0
+Version: 1.9.0
 Summary: An open source framework for using Amazon Braket devices with the PennyLane quantum machine learning library
 Home-page: https://github.com/aws/amazon-braket-pennylane-plugin-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-pennylane-plugin-1.8.0/README.rst` & `amazon-braket-pennylane-plugin-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/setup.cfg` & `amazon-braket-pennylane-plugin-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/setup.py` & `amazon-braket-pennylane-plugin-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/PKG-INFO` & `amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-pennylane-plugin
-Version: 1.8.0
+Version: 1.9.0
 Summary: An open source framework for using Amazon Braket devices with the PennyLane quantum machine learning library
 Home-page: https://github.com/aws/amazon-braket-pennylane-plugin-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-pennylane-plugin-1.8.0/src/amazon_braket_pennylane_plugin.egg-info/SOURCES.txt` & `amazon-braket-pennylane-plugin-1.9.0/src/amazon_braket_pennylane_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/__init__.py` & `amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/_version.py` & `amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
```

### Comparing `amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/braket_device.py` & `amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/braket_device.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/ops.py` & `amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/ops.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-pennylane-plugin-1.8.0/src/braket/pennylane_plugin/translation.py` & `amazon-braket-pennylane-plugin-1.9.0/src/braket/pennylane_plugin/translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     CPhaseShift01,
     CPhaseShift10,
     GPi,
     GPi2,
 )
 
 _BRAKET_TO_PENNYLANE_OPERATIONS = {
+    "i": "Identity",
     "x": "PauliX",
     "y": "PauliY",
     "z": "PauliZ",
     "h": "Hadamard",
     "ry": "RY",
     "rx": "RX",
     "rz": "RZ",
@@ -125,14 +126,19 @@
 def _translate_operation(operation: Operation, _parameters) -> Gate:
     raise NotImplementedError(
         f"Braket PennyLane plugin does not support operation {operation.name}."
     )
 
 
 @_translate_operation.register
+def _(_: qml.Identity, _parameters):
+    return gates.I()
+
+
+@_translate_operation.register
 def _(_: qml.Hadamard, _parameters):
     return gates.H()
 
 
 @_translate_operation.register
 def _(_: qml.PauliX, _parameters):
     return gates.X()
```

