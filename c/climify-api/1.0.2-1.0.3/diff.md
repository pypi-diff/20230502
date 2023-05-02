# Comparing `tmp/climify_api-1.0.2.tar.gz` & `tmp/climify_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climify_api-1.0.2.tar", last modified: Tue May  2 09:17:47 2023, max compression
+gzip compressed data, was "climify_api-1.0.3.tar", last modified: Tue May  2 09:26:36 2023, max compression
```

## Comparing `climify_api-1.0.2.tar` & `climify_api-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 09:17:47.109111 climify_api-1.0.2/
--rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      932 2023-05-02 09:17:47.108611 climify_api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 09:17:47.076435 climify_api-1.0.2/climify_api/
--rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.2/climify_api/ApiController.py
--rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.2/climify_api/REST.py
--rw-rw-rw-   0        0        0      904 2023-05-02 09:17:00.000000 climify_api-1.0.2/climify_api/__init__.py
--rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.2/climify_api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:17:47.094762 climify_api-1.0.2/climify_api/apis/
--rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.2/climify_api/apis/PathBase.py
--rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.2/climify_api/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:17:47.102815 climify_api-1.0.2/climify_api/apis/v1/
--rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.2/climify_api/apis/v1/ApiController.py
--rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.2/climify_api/apis/v1/__init__.py
--rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.2/climify_api/auth.py
--rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.2/climify_api/configuration.py
--rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.2/climify_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:17:47.105570 climify_api-1.0.2/climify_api/models/
--rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.2/climify_api/models/__init__.py
--rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.2/climify_api/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-02 09:17:47.087860 climify_api-1.0.2/climify_api.egg-info/
--rw-rw-rw-   0        0        0      932 2023-05-02 09:17:47.000000 climify_api-1.0.2/climify_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-05-02 09:17:47.000000 climify_api-1.0.2/climify_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 09:17:47.000000 climify_api-1.0.2/climify_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-05-02 09:17:47.000000 climify_api-1.0.2/climify_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 09:17:47.000000 climify_api-1.0.2/climify_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1484 2023-05-02 09:16:46.000000 climify_api-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 09:17:47.109111 climify_api-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.287683 climify_api-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      932 2023-05-02 09:26:36.286681 climify_api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.240746 climify_api-1.0.3/climify_api/
+-rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.3/climify_api/ApiController.py
+-rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.3/climify_api/REST.py
+-rw-rw-rw-   0        0        0      904 2023-05-02 09:23:35.000000 climify_api-1.0.3/climify_api/__init__.py
+-rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.3/climify_api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.272050 climify_api-1.0.3/climify_api/apis/
+-rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.3/climify_api/apis/PathBase.py
+-rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.3/climify_api/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.276476 climify_api-1.0.3/climify_api/apis/v1/
+-rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.3/climify_api/apis/v1/ApiController.py
+-rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.3/climify_api/apis/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.280159 climify_api-1.0.3/climify_api/apis/v1/paths/
+-rw-rw-rw-   0        0        0      986 2023-04-11 09:18:57.000000 climify_api-1.0.3/climify_api/apis/v1/paths/__init__.py
+-rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.3/climify_api/auth.py
+-rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.3/climify_api/configuration.py
+-rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.3/climify_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.283661 climify_api-1.0.3/climify_api/models/
+-rw-rw-rw-   0        0        0     6718 2023-04-11 13:31:23.000000 climify_api-1.0.3/climify_api/models/__init__.py
+-rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.3/climify_api/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:26:36.265134 climify_api-1.0.3/climify_api.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 09:26:36.000000 climify_api-1.0.3/climify_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1516 2023-05-02 09:23:30.000000 climify_api-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:26:36.287683 climify_api-1.0.3/setup.cfg
```

### Comparing `climify_api-1.0.2/LICENSE` & `climify_api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/PKG-INFO` & `climify_api-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.2/climify_api/REST.py` & `climify_api-1.0.3/climify_api/REST.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/__init__.py` & `climify_api-1.0.3/climify_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Provides a REST endpoints for Climify applications and 3rd party solutions.  # noqa: E501
 
     The version of the OpenAPI document: 1.2.3
     Generated by: https://openapi-generator.tech
 """
 
 __name__ = 'climify_api'
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 # import ApiClient
 from climify_api.api_client import ApiClient
 
 # import Configuration
 from climify_api.configuration import Configuration, ClimifyRegion
```

### Comparing `climify_api-1.0.2/climify_api/api_client.py` & `climify_api-1.0.3/climify_api/api_client.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/apis/PathBase.py` & `climify_api-1.0.3/climify_api/apis/PathBase.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/apis/v1/ApiController.py` & `climify_api-1.0.3/climify_api/apis/v1/ApiController.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/auth.py` & `climify_api-1.0.3/climify_api/auth.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/configuration.py` & `climify_api-1.0.3/climify_api/configuration.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/exceptions.py` & `climify_api-1.0.3/climify_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/models/__init__.py` & `climify_api-1.0.3/climify_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api/schemas.py` & `climify_api-1.0.3/climify_api/schemas.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.2/climify_api.egg-info/PKG-INFO` & `climify_api-1.0.3/climify_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.2/climify_api.egg-info/SOURCES.txt` & `climify_api-1.0.3/climify_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 climify_api.egg-info/dependency_links.txt
 climify_api.egg-info/requires.txt
 climify_api.egg-info/top_level.txt
 climify_api/apis/PathBase.py
 climify_api/apis/__init__.py
 climify_api/apis/v1/ApiController.py
 climify_api/apis/v1/__init__.py
+climify_api/apis/v1/paths/__init__.py
 climify_api/models/__init__.py
```

### Comparing `climify_api-1.0.2/pyproject.toml` & `climify_api-1.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "climify_api"
-version = "1.0.2"
+version = "1.0.3"
 keywords=['Climify','Environmental engineering']
 authors = [
   { name="Climify Aps", email="info@climify.com" },
 ]
 description = "A wrapper library for the Climify REST API"
 #long_description = "A wrapper library for the Climify REST API, used to query sensor data and interact with Climify systems programmatically"
 readme = "README.md"
@@ -44,13 +44,14 @@
   "pydantic"
 ]
 
 [tool.setuptools]
 packages=[
   'climify_api',
   'climify_api.apis',
-  'climify_api.apis.v1'
+  'climify_api.apis.v1',
+  'climify_api.apis.v1.paths'
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.climify.com/climify/python-api-lib"
 "Bug Tracker" = "https://gitlab.climify.com/climify/python-api-lib/-/issues"
```

