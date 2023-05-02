# Comparing `tmp/climify_api-1.0.0.tar.gz` & `tmp/climify_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climify_api-1.0.0.tar", last modified: Thu Apr 13 08:44:16 2023, max compression
+gzip compressed data, was "climify_api-1.0.1.tar", last modified: Tue May  2 08:29:21 2023, max compression
```

## Comparing `climify_api-1.0.0.tar` & `climify_api-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 08:44:16.007822 climify_api-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      932 2023-04-13 08:44:16.006823 climify_api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 08:44:15.993706 climify_api-1.0.0/climify_api/
--rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.0/climify_api/ApiController.py
--rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.0/climify_api/REST.py
--rw-rw-rw-   0        0        0      904 2023-04-13 08:43:41.000000 climify_api-1.0.0/climify_api/__init__.py
--rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.0/climify_api/api_client.py
--rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.0/climify_api/auth.py
--rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.0/climify_api/configuration.py
--rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.0/climify_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:44:16.005824 climify_api-1.0.0/climify_api/models/
--rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.0/climify_api/models/__init__.py
--rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.0/climify_api/schemas.py
-drwxrwxrwx   0        0        0        0 2023-04-13 08:44:16.003806 climify_api-1.0.0/climify_api.egg-info/
--rw-rw-rw-   0        0        0      932 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 08:44:15.000000 climify_api-1.0.0/climify_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1429 2023-04-13 08:43:29.000000 climify_api-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 08:44:16.007822 climify_api-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 08:29:21.554568 climify_api-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      932 2023-05-02 08:29:21.553474 climify_api-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 08:29:21.536721 climify_api-1.0.1/climify_api/
+-rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.1/climify_api/ApiController.py
+-rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.1/climify_api/REST.py
+-rw-rw-rw-   0        0        0      904 2023-05-02 08:27:22.000000 climify_api-1.0.1/climify_api/__init__.py
+-rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.1/climify_api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:29:21.547477 climify_api-1.0.1/climify_api/apis/
+-rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.1/climify_api/apis/PathBase.py
+-rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.1/climify_api/auth.py
+-rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.1/climify_api/configuration.py
+-rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.1/climify_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:29:21.552475 climify_api-1.0.1/climify_api/models/
+-rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.1/climify_api/models/__init__.py
+-rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.1/climify_api/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:29:21.544475 climify_api-1.0.1/climify_api.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-05-02 08:29:21.000000 climify_api-1.0.1/climify_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-05-02 08:29:21.000000 climify_api-1.0.1/climify_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 08:29:21.000000 climify_api-1.0.1/climify_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-05-02 08:29:21.000000 climify_api-1.0.1/climify_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 08:29:21.000000 climify_api-1.0.1/climify_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1458 2023-05-02 08:25:25.000000 climify_api-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 08:29:21.554568 climify_api-1.0.1/setup.cfg
```

### Comparing `climify_api-1.0.0/LICENSE` & `climify_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/PKG-INFO` & `climify_api-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.0/climify_api/REST.py` & `climify_api-1.0.1/climify_api/REST.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/climify_api/__init__.py` & `climify_api-1.0.1/climify_api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Provides a REST endpoints for Climify applications and 3rd party solutions.  # noqa: E501
 
     The version of the OpenAPI document: 1.2.3
     Generated by: https://openapi-generator.tech
 """
 
 __name__ = 'climify_api'
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 # import ApiClient
 from climify_api.api_client import ApiClient
 
 # import Configuration
 from climify_api.configuration import Configuration, ClimifyRegion
```

### Comparing `climify_api-1.0.0/climify_api/api_client.py` & `climify_api-1.0.1/climify_api/api_client.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/climify_api/auth.py` & `climify_api-1.0.1/climify_api/auth.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/climify_api/configuration.py` & `climify_api-1.0.1/climify_api/configuration.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/climify_api/exceptions.py` & `climify_api-1.0.1/climify_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/climify_api/models/__init__.py` & `climify_api-1.0.1/climify_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/climify_api/schemas.py` & `climify_api-1.0.1/climify_api/schemas.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.0/climify_api.egg-info/PKG-INFO` & `climify_api-1.0.1/climify_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.0/pyproject.toml` & `climify_api-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "climify_api"
-version = "1.0.0"
+version = "1.0.1"
 keywords=['Climify','Environmental engineering']
 authors = [
   { name="Climify Aps", email="info@climify.com" },
 ]
 description = "A wrapper library for the Climify REST API"
 #long_description = "A wrapper library for the Climify REST API, used to query sensor data and interact with Climify systems programmatically"
 readme = "README.md"
@@ -41,12 +41,15 @@
   "pyyaml",
   "oauthlib",
   "varname",
   "pydantic"
 ]
 
 [tool.setuptools]
-packages=['climify_api']
+packages=[
+  'climify_api',
+  'climify_api.apis'
+]
 
 [project.urls]
 "Homepage" = "https://gitlab.climify.com/climify/python-api-lib"
 "Bug Tracker" = "https://gitlab.climify.com/climify/python-api-lib/-/issues"
```

