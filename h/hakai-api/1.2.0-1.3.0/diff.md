# Comparing `tmp/hakai_api-1.2.0.tar.gz` & `tmp/hakai_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakai_api-1.2.0.tar", last modified: Thu Sep  1 17:36:32 2022, max compression
+gzip compressed data, was "hakai_api-1.3.0.tar", last modified: Tue May  2 18:41:39 2023, max compression
```

## Comparing `hakai_api-1.2.0.tar` & `hakai_api-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:36:32.404260 hakai_api-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3407 2022-09-01 17:36:32.404260 hakai_api-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-09-01 17:36:18.000000 hakai_api-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:36:32.404260 hakai_api-1.2.0/hakai_api/
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-09-01 17:36:18.000000 hakai_api-1.2.0/hakai_api/Client.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-01 17:36:18.000000 hakai_api-1.2.0/hakai_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 17:36:32.404260 hakai_api-1.2.0/hakai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3407 2022-09-01 17:36:32.000000 hakai_api-1.2.0/hakai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-01 17:36:32.000000 hakai_api-1.2.0/hakai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 17:36:32.000000 hakai_api-1.2.0/hakai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-01 17:36:32.000000 hakai_api-1.2.0/hakai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-01 17:36:32.000000 hakai_api-1.2.0/hakai_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-01 17:36:32.404260 hakai_api-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-09-01 17:36:18.000000 hakai_api-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:41:39.709599 hakai_api-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 18:41:39.709599 hakai_api-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-02 18:41:24.000000 hakai_api-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:41:39.709599 hakai_api-1.3.0/hakai_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-02 18:41:24.000000 hakai_api-1.3.0/hakai_api/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 18:41:24.000000 hakai_api-1.3.0/hakai_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:41:39.709599 hakai_api-1.3.0/hakai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 18:41:39.000000 hakai_api-1.3.0/hakai_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:41:39.709599 hakai_api-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 18:41:24.000000 hakai_api-1.3.0/setup.py
```

### Comparing `hakai_api-1.2.0/PKG-INFO` & `hakai_api-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakai_api
-Version: 1.2.0
+Version: 1.3.0
 Summary: Get Hakai database resources using http calls
 Home-page: https://github.com/HakaiInstitute/hakai-api-client-python
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hakai_api-1.2.0/README.md` & `hakai_api-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hakai_api-1.2.0/hakai_api/Client.py` & `hakai_api-1.3.0/hakai_api/Client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Get authorized requests to the Hakai API using the requests library.
 
 Written by: Taylor Denouden, Chris Davis, and Nate Rosenstock
 Last updated: April 2021
 """
 
 import os
-import pickle
+import json
 from datetime import datetime
 from time import mktime, sleep
 from typing import Dict, Union
 
-from pytz import utc
 from requests_oauthlib import OAuth2Session
 
 
 class Client(OAuth2Session):
     _credentials_file = os.path.expanduser("~/.hakai-api-auth")
 
     def __init__(
@@ -64,34 +63,34 @@
     @classmethod
     def reset_credentials(cls):
         if os.path.isfile(cls._credentials_file):
             os.remove(cls._credentials_file)
 
     def _save_credentials(self, credentials: Dict):
         """Save the credentials object to a file."""
-        with open(self._credentials_file, "wb") as outfile:
-            pickle.dump(credentials, outfile)
+        with open(self._credentials_file, "w") as outfile:
+            json.dump(credentials, outfile)
 
     def _try_to_load_credentials_file(self) -> Union[Dict, bool]:
         """Try to load the cached credentials file."""
         if not os.path.isfile(self._credentials_file):
             return False
 
         with open(self._credentials_file, "rb") as infile:
             try:
-                credentials = pickle.load(infile)
+                credentials = json.load(infile)
                 expires_at = int(credentials["expires_at"])
             except (KeyError, ValueError):
                 os.remove(self._credentials_file)
                 return False
 
             now = int(
                 (
-                    mktime(datetime.now(tz=utc).timetuple())
-                    + datetime.now(tz=utc).microsecond / 1000000.0
+                    mktime(datetime.now().timetuple())
+                    + datetime.now().microsecond / 1000000.0
                 )
             )  # utc timestamp
 
             if now > expires_at:
                 os.remove(self._credentials_file)
                 return False
```

### Comparing `hakai_api-1.2.0/hakai_api.egg-info/PKG-INFO` & `hakai_api-1.3.0/hakai_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakai-api
-Version: 1.2.0
+Version: 1.3.0
 Summary: Get Hakai database resources using http calls
 Home-page: https://github.com/HakaiInstitute/hakai-api-client-python
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hakai_api-1.2.0/setup.py` & `hakai_api-1.3.0/setup.py`

 * *Files identical despite different names*

