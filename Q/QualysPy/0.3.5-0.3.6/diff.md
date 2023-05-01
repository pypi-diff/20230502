# Comparing `tmp/qualyspy-0.3.5.tar.gz` & `tmp/qualyspy-0.3.6.tar.gz`

## Comparing `qualyspy-0.3.5.tar` & `qualyspy-0.3.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/remove_cookies.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 qualyspy-0.3.5/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.5/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/__init__.py
--rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/qutils.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/urls.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/api_input.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    14938 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.5/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.5/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.5/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.5/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.5/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.5/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/remove_cookies.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 qualyspy-0.3.6/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.6/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/exceptions.py
+-rw-r--r--   0        0        0    16827 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/api_input.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    14938 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.6/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.6/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.6/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.6/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.6/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.6/PKG-INFO
```

### Comparing `qualyspy-0.3.5/.vscode/launch.json` & `qualyspy-0.3.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/debug/dtd.txt` & `qualyspy-0.3.6/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/debug/output.txt` & `qualyspy-0.3.6/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/debug/parse_dtd.py` & `qualyspy-0.3.6/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/debug/quickscan.py` & `qualyspy-0.3.6/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/debug/remove_cookies.py` & `qualyspy-0.3.6/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/docs/Makefile` & `qualyspy-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/docs/make.bat` & `qualyspy-0.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/docs/source/conf.py` & `qualyspy-0.3.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/qualysapi.py` & `qualyspy-0.3.6/qualyspy/qualysapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import lxml.objectify
 import requests
 
 import ssl
 import urllib3
 
 from . import qutils
+from .exceptions import Qualys_API_Error
 
 JSON_IN_JSON_OUT_HEADERS = {
     "Accept": "application/json",
     "Content-Type": "application/json",
 }
 JSON_IN_XML_OUT_HEADERS = {
     "Accept": "application/json",
@@ -60,18 +61,14 @@
 API_GATEWAY_ROOT = qutils.config["AUTHENTICATION"]["api_gateway_root"]
 CREDENTIALS = {
     "username": qutils.config["AUTHENTICATION"]["username"],
     "password": qutils.config["AUTHENTICATION"]["password"],
 }
 
 
-class Qualys_API_Error(Exception):
-    """Exception raised when the Qualys API returns a non-200 response, or some other error."""
-
-
 class Connection:
     """A connection to a Qualys API endpoint.
 
     When an object of this class is removed from memory, a logout API request will be made.
 
     Attributes:
         add_headers:
```

### Comparing `qualyspy-0.3.5/qualyspy/qutils.py` & `qualyspy-0.3.6/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/urls.json` & `qualyspy-0.3.6/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/api_input.py` & `qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/api_input.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/asset_mgmt_tagging/tag.py` & `qualyspy-0.3.6/qualyspy/asset_mgmt_tagging/tag.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/assets/host_list.py` & `qualyspy-0.3.6/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/assets/host_list_detection.py` & `qualyspy-0.3.6/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/certview/certificate.py` & `qualyspy-0.3.6/qualyspy/certview/certificate.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.3.6/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/.gitignore` & `qualyspy-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/LICENSE` & `qualyspy-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.5/pyproject.toml` & `qualyspy-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.3.5/PKG-INFO` & `qualyspy-0.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

