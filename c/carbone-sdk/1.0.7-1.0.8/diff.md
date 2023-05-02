# Comparing `tmp/carbone-sdk-1.0.7.tar.gz` & `tmp/carbone-sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbone-sdk-1.0.7.tar", last modified: Thu Jan 26 12:58:07 2023, max compression
+gzip compressed data, was "carbone-sdk-1.0.8.tar", last modified: Tue May  2 07:18:51 2023, max compression
```

## Comparing `carbone-sdk-1.0.7.tar` & `carbone-sdk-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 steeve     (501) staff       (20)        0 2023-01-26 12:58:07.252733 carbone-sdk-1.0.7/
--rw-r--r--   0 steeve     (501) staff       (20)    11357 2021-06-12 12:25:22.000000 carbone-sdk-1.0.7/LICENSE.txt
--rw-r--r--   0 steeve     (501) staff       (20)     4129 2023-01-26 12:58:07.252527 carbone-sdk-1.0.7/PKG-INFO
--rw-r--r--   0 steeve     (501) staff       (20)     3580 2023-01-26 12:53:12.000000 carbone-sdk-1.0.7/README.md
-drwxr-xr-x   0 steeve     (501) staff       (20)        0 2023-01-26 12:58:07.250776 carbone-sdk-1.0.7/carbone_sdk/
--rw-r--r--   0 steeve     (501) staff       (20)       35 2021-06-12 12:25:22.000000 carbone-sdk-1.0.7/carbone_sdk/__init__.py
--rw-r--r--   0 steeve     (501) staff       (20)     6256 2023-01-26 12:40:46.000000 carbone-sdk-1.0.7/carbone_sdk/carbone_sdk.py
-drwxr-xr-x   0 steeve     (501) staff       (20)        0 2023-01-26 12:58:07.252233 carbone-sdk-1.0.7/carbone_sdk.egg-info/
--rwxrwxrwx   0 steeve     (501) staff       (20)     4129 2023-01-26 12:58:07.000000 carbone-sdk-1.0.7/carbone_sdk.egg-info/PKG-INFO
--rwxrwxrwx   0 steeve     (501) staff       (20)      221 2023-01-26 12:58:07.000000 carbone-sdk-1.0.7/carbone_sdk.egg-info/SOURCES.txt
--rwxrwxrwx   0 steeve     (501) staff       (20)        1 2023-01-26 12:58:07.000000 carbone-sdk-1.0.7/carbone_sdk.egg-info/dependency_links.txt
--rwxrwxrwx   0 steeve     (501) staff       (20)       12 2023-01-26 12:58:07.000000 carbone-sdk-1.0.7/carbone_sdk.egg-info/top_level.txt
--rw-r--r--   0 steeve     (501) staff       (20)       38 2023-01-26 12:58:07.252797 carbone-sdk-1.0.7/setup.cfg
--rw-r--r--   0 steeve     (501) staff       (20)      782 2023-01-26 12:55:37.000000 carbone-sdk-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 07:18:51.091758 carbone-sdk-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-02 07:18:39.000000 carbone-sdk-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4345 2023-05-02 07:18:51.091758 carbone-sdk-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-05-02 07:18:39.000000 carbone-sdk-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 07:18:51.087758 carbone-sdk-1.0.8/carbone_sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-02 07:18:39.000000 carbone-sdk-1.0.8/carbone_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6586 2023-05-02 07:18:39.000000 carbone-sdk-1.0.8/carbone_sdk/carbone_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 07:18:51.087758 carbone-sdk-1.0.8/carbone_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4345 2023-05-02 07:18:51.000000 carbone-sdk-1.0.8/carbone_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-02 07:18:51.000000 carbone-sdk-1.0.8/carbone_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 07:18:51.000000 carbone-sdk-1.0.8/carbone_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-02 07:18:51.000000 carbone-sdk-1.0.8/carbone_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 07:18:51.091758 carbone-sdk-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2023-05-02 07:18:39.000000 carbone-sdk-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 07:18:51.087758 carbone-sdk-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    16266 2023-05-02 07:18:39.000000 carbone-sdk-1.0.8/tests/test_carbone_sdk.py
```

### Comparing `carbone-sdk-1.0.7/LICENSE.txt` & `carbone-sdk-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `carbone-sdk-1.0.7/PKG-INFO` & `carbone-sdk-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbone-sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Carbone API Python SDK to generate documents (PDF, docx, xlsx, ods, odt, ...) from a JSON and a template.
 Home-page: https://github.com/carboneio/carbone-sdk-python
 Author: CarboneIO
 Author-email: support@carbone.io
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,23 +31,27 @@
 ```sh
 pip install carbone-sdk
 ```
 
 ## Usage
 
 You can copy and run the code bellow to try.
+Get your API token on your Carbone account: https://account.carbone.io/.
+
 ```python
 import carbone_sdk
 
 # SDK constructor
 # The access token can be passed as an argument to the constructor CarboneSDK
 # Or by the environment variable "CARBONE_TOKEN", use the command "export CARBONE_TOKEN=secret-token"
 csdk = carbone_sdk.CarboneSDK("secret-token")
-# Set API version
+# Set API version (default : 4)
 csdk.set_api_version("4")
+# Set API URL for Carbone On-Premise for example (default: "https://api.carbone.io")
+csdk.set_api_url("https://api.carbone.io")
 
 # The template ID, it could be an ODT, DOCX, PPTX, XLSX, ODS file, etc...
 template_id = "template"
 render_options = {
   # REQUIRED: the "data" object contains all the data to inject into the template
   "data": {
     "id": 42,
```

### Comparing `carbone-sdk-1.0.7/README.md` & `carbone-sdk-1.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,23 +16,27 @@
 ```sh
 pip install carbone-sdk
 ```
 
 ## Usage
 
 You can copy and run the code bellow to try.
+Get your API token on your Carbone account: https://account.carbone.io/.
+
 ```python
 import carbone_sdk
 
 # SDK constructor
 # The access token can be passed as an argument to the constructor CarboneSDK
 # Or by the environment variable "CARBONE_TOKEN", use the command "export CARBONE_TOKEN=secret-token"
 csdk = carbone_sdk.CarboneSDK("secret-token")
-# Set API version
+# Set API version (default : 4)
 csdk.set_api_version("4")
+# Set API URL for Carbone On-Premise for example (default: "https://api.carbone.io")
+csdk.set_api_url("https://api.carbone.io")
 
 # The template ID, it could be an ODT, DOCX, PPTX, XLSX, ODS file, etc...
 template_id = "template"
 render_options = {
   # REQUIRED: the "data" object contains all the data to inject into the template
   "data": {
     "id": 42,
```

### Comparing `carbone-sdk-1.0.7/carbone_sdk/carbone_sdk.py` & `carbone-sdk-1.0.8/carbone_sdk/carbone_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,22 @@
     if isinstance(api_version, str):
       self._api_headers["carbone-version"] = api_version
     elif isinstance(api_version, int):
       self._api_headers["carbone-version"] = str(api_version)
     else:
       raise ValueError('Carbone SDK set_api_version error: an argument is invalid: api_version is not a number nor a string')
 
+  def set_api_url(self, api_url = None):
+    if api_url is None:
+      raise ValueError('Carbone SDK set_api_url error: argument is missing: api_url')
+    if isinstance(api_url, str):
+      self._api_url = api_url
+    else:
+      raise ValueError('Carbone SDK set_api_url error: an argument is invalid: api_url is not a string')
+
   def render(self, file_or_template_id = None, json_data = None, payload = ""):
     if file_or_template_id is None:
       raise ValueError('Carbone SDK render error: argument is missing: file_or_template_id')
     if json_data is None:
       raise ValueError('Carbone SDK render error: argument is missing: json_data')
     resp = None
     # 1 - if file_or_template_id is a template_id => render from the template_id
```

### Comparing `carbone-sdk-1.0.7/carbone_sdk.egg-info/PKG-INFO` & `carbone-sdk-1.0.8/carbone_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbone-sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Carbone API Python SDK to generate documents (PDF, docx, xlsx, ods, odt, ...) from a JSON and a template.
 Home-page: https://github.com/carboneio/carbone-sdk-python
 Author: CarboneIO
 Author-email: support@carbone.io
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,23 +31,27 @@
 ```sh
 pip install carbone-sdk
 ```
 
 ## Usage
 
 You can copy and run the code bellow to try.
+Get your API token on your Carbone account: https://account.carbone.io/.
+
 ```python
 import carbone_sdk
 
 # SDK constructor
 # The access token can be passed as an argument to the constructor CarboneSDK
 # Or by the environment variable "CARBONE_TOKEN", use the command "export CARBONE_TOKEN=secret-token"
 csdk = carbone_sdk.CarboneSDK("secret-token")
-# Set API version
+# Set API version (default : 4)
 csdk.set_api_version("4")
+# Set API URL for Carbone On-Premise for example (default: "https://api.carbone.io")
+csdk.set_api_url("https://api.carbone.io")
 
 # The template ID, it could be an ODT, DOCX, PPTX, XLSX, ODS file, etc...
 template_id = "template"
 render_options = {
   # REQUIRED: the "data" object contains all the data to inject into the template
   "data": {
     "id": 42,
```

### Comparing `carbone-sdk-1.0.7/setup.py` & `carbone-sdk-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="carbone-sdk",
-    version="1.0.7",
+    version="1.0.8",
     author="CarboneIO",
     author_email="support@carbone.io",
     description="Carbone API Python SDK to generate documents (PDF, docx, xlsx, ods, odt, ...) from a JSON and a template.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/carboneio/carbone-sdk-python",
     packages=setuptools.find_packages(),
```

