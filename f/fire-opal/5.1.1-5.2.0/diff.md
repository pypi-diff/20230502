# Comparing `tmp/fire_opal-5.1.1.tar.gz` & `tmp/fire_opal-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-5.1.1.tar", max compression
+gzip compressed data, was "fire_opal-5.2.0.tar", max compression
```

## Comparing `fire_opal-5.1.1.tar` & `fire_opal-5.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    36653 2023-04-24 20:59:10.328677 fire_opal-5.1.1/LICENSE
--rw-r--r--   0        0        0      524 2023-04-24 20:59:10.328677 fire_opal-5.1.1/README.md
--rw-r--r--   0        0        0      743 2023-04-24 20:59:34.204823 fire_opal-5.1.1/fireopal/__init__.py
--rw-r--r--   0        0        0      697 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/admin.py
--rw-r--r--   0        0        0     2753 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/config.py
--rw-r--r--   0        0        0      868 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/constants.py
--rw-r--r--   0        0        0      891 2023-04-24 20:59:34.208824 fire_opal-5.1.1/fireopal/functions/__init__.py
--rw-r--r--   0        0        0      818 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/base.py
--rw-r--r--   0        0        0     1087 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/benchmark.py
--rw-r--r--   0        0        0     1772 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/create_calibration_data.py
--rw-r--r--   0        0        0      979 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/create_mitigation_data.py
--rw-r--r--   0        0        0     1711 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/execute.py
--rw-r--r--   0        0        0      838 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/read_data.py
--rw-r--r--   0        0        0      845 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     2145 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1556 2023-04-24 20:59:10.328677 fire_opal-5.1.1/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2724 2023-04-24 20:59:34.196823 fire_opal-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 fire_opal-5.1.1/setup.py
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 fire_opal-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-05-02 03:26:14.965359 fire_opal-5.2.0/LICENSE
+-rw-r--r--   0        0        0      524 2023-05-02 03:26:14.965359 fire_opal-5.2.0/README.md
+-rw-r--r--   0        0        0      743 2023-05-02 03:26:39.862620 fire_opal-5.2.0/fireopal/__init__.py
+-rw-r--r--   0        0        0      697 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/admin.py
+-rw-r--r--   0        0        0     3120 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/config.py
+-rw-r--r--   0        0        0      869 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/constants.py
+-rw-r--r--   0        0        0      891 2023-05-02 03:26:39.862620 fire_opal-5.2.0/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0      818 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/base.py
+-rw-r--r--   0        0        0     1087 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/benchmark.py
+-rw-r--r--   0        0        0     1772 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/create_calibration_data.py
+-rw-r--r--   0        0        0      979 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/create_mitigation_data.py
+-rw-r--r--   0        0        0     1711 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/execute.py
+-rw-r--r--   0        0        0      838 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0      845 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     2145 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1556 2023-05-02 03:26:14.965359 fire_opal-5.2.0/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2724 2023-05-02 03:26:39.854620 fire_opal-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 fire_opal-5.2.0/setup.py
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 fire_opal-5.2.0/PKG-INFO
```

### Comparing `fire_opal-5.1.1/LICENSE` & `fire_opal-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/README.md` & `fire_opal-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/__init__.py` & `fire_opal-5.2.0/fireopal/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/admin.py` & `fire_opal-5.2.0/fireopal/admin.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/constants.py` & `fire_opal-5.2.0/fireopal/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
+
 INVALID_SUBSCRIPTION_ERROR = """
 ---------------------------------------------------------------------
 Your authentication succeeded, but your subscription is invalid for
 this product.
 
 Please access `https://fire.q-ctrl.com` for more details.
 ---------------------------------------------------------------------
```

### Comparing `fire_opal-5.1.1/fireopal/functions/__init__.py` & `fire_opal-5.2.0/fireopal/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/base.py` & `fire_opal-5.2.0/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/benchmark.py` & `fire_opal-5.2.0/fireopal/functions/benchmark.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/create_calibration_data.py` & `fire_opal-5.2.0/fireopal/functions/create_calibration_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/create_mitigation_data.py` & `fire_opal-5.2.0/fireopal/functions/create_mitigation_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/execute.py` & `fire_opal-5.2.0/fireopal/functions/execute.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/read_data.py` & `fire_opal-5.2.0/fireopal/functions/read_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/show_supported_devices.py` & `fire_opal-5.2.0/fireopal/functions/show_supported_devices.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/solve_qaoa.py` & `fire_opal-5.2.0/fireopal/functions/solve_qaoa.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/fireopal/functions/validate.py` & `fire_opal-5.2.0/fireopal/functions/validate.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.1.1/pyproject.toml` & `fire_opal-5.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "5.1.1"
+version = "5.2.0"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -69,15 +69,15 @@
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
-qctrl-client = "^5.0.0"
+qctrl-client = "^7.0.0"
 click = "^8.1.0"
 qctrl-commons = "^18.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
```

### Comparing `fire_opal-5.1.1/setup.py` & `fire_opal-5.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 ['fireopal', 'fireopal.functions']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.0,<9.0.0',
- 'qctrl-client>=5.0.0,<6.0.0',
+ 'qctrl-client>=7.0.0,<8.0.0',
  'qctrl-commons>=18.0.0,<19.0.0']
 
 setup_kwargs = {
     'name': 'fire-opal',
-    'version': '5.1.1',
+    'version': '5.2.0',
     'description': 'Fire Opal Client',
     'long_description': "# Fire Opal Client\n\nThe Fire Opal Client package is a Python client for Q-CTRL's Fire Opal product.\nFire Opal is a simple and powerful package for algorithm developers and quantum computer end users.\nBy applying a complete suite of error suppression techniques, Fire Opal automatically reduces error and vastly improves the quality of quantum algorithm results. This often transforms quantum computer outputs from random to useful.\n\nPlease see how you can [get started](https://docs.q-ctrl.com/fire-opal/get-started) today.\n",
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
```

### Comparing `fire_opal-5.1.1/PKG-INFO` & `fire_opal-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 5.1.1
+Version: 5.2.0
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: click (>=8.1.0,<9.0.0)
-Requires-Dist: qctrl-client (>=5.0.0,<6.0.0)
+Requires-Dist: qctrl-client (>=7.0.0,<8.0.0)
 Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
```

