# Comparing `tmp/hyperthought-0.9.8.tar.gz` & `tmp/hyperthought-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperthought-0.9.8.tar", last modified: Fri Oct 22 21:53:28 2021, max compression
+gzip compressed data, was "hyperthought-0.9.9.tar", last modified: Mon Oct 25 20:01:44 2021, max compression
```

## Comparing `hyperthought-0.9.8.tar` & `hyperthought-0.9.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.958212 hyperthought-0.9.8/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2021-10-22 21:53:11.000000 hyperthought-0.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2038 2021-10-22 21:53:28.959213 hyperthought-0.9.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1451 2021-10-22 21:53:11.000000 hyperthought-0.9.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      103 2021-10-22 21:53:11.000000 hyperthought-0.9.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      676 2021-10-22 21:53:28.959213 hyperthought-0.9.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2021-10-22 21:53:11.000000 hyperthought-0.9.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.948212 hyperthought-0.9.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.952212 hyperthought-0.9.8/src/hyperthought/
--rw-rw-rw-   0 root         (0) root         (0)       74 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.954212 hyperthought-0.9.8/src/hyperthought/api/
--rw-rw-rw-   0 root         (0) root         (0)      106 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4082 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4427 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/common.py
--rw-rw-rw-   0 root         (0) root         (0)    34806 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/files.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/metatron.py
--rw-rw-rw-   0 root         (0) root         (0)     3042 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.955212 hyperthought-0.9.8/src/hyperthought/api/workflow/
--rw-rw-rw-   0 root         (0) root         (0)    26153 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.955212 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/
--rw-rw-rw-   0 root         (0) root         (0)       40 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.956212 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)       42 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9154 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/root.py
--rw-rw-rw-   0 root         (0) root         (0)     5634 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/unionfind.py
--rw-rw-rw-   0 root         (0) root         (0)    11038 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/xml_generation.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/api/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)     8711 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4878 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.958212 hyperthought-0.9.8/src/hyperthought/parsers/
--rw-rw-rw-   0 root         (0) root         (0)     2988 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/_ayasdi.py
--rw-rw-rw-   0 root         (0) root         (0)     5093 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/_centerstreet.py
--rw-rw-rw-   0 root         (0) root         (0)     5729 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/_craic.py
--rw-rw-rw-   0 root         (0) root         (0)     6650 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/_fei_tiff.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/_hyperspy.py
--rw-rw-rw-   0 root         (0) root         (0)     3548 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/_midas.py
--rw-rw-rw-   0 root         (0) root         (0)     3633 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/_nsidat.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.958212 hyperthought-0.9.8/src/hyperthought/parsers/utils/
--rw-rw-rw-   0 root         (0) root         (0)      692 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2103 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/parsers/utils/flatten.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2021-10-22 21:53:11.000000 hyperthought-0.9.8/src/hyperthought/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-22 21:53:28.953212 hyperthought-0.9.8/src/hyperthought.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2038 2021-10-22 21:53:28.000000 hyperthought-0.9.8/src/hyperthought.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1386 2021-10-22 21:53:28.000000 hyperthought-0.9.8/src/hyperthought.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2021-10-22 21:53:28.000000 hyperthought-0.9.8/src/hyperthought.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2021-10-22 21:53:28.000000 hyperthought-0.9.8/src/hyperthought.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.758949 hyperthought-0.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2021-10-25 20:01:26.000000 hyperthought-0.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2038 2021-10-25 20:01:44.758949 hyperthought-0.9.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2021-10-25 20:01:26.000000 hyperthought-0.9.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      103 2021-10-25 20:01:26.000000 hyperthought-0.9.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      676 2021-10-25 20:01:44.759950 hyperthought-0.9.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2021-10-25 20:01:26.000000 hyperthought-0.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.749949 hyperthought-0.9.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.751949 hyperthought-0.9.9/src/hyperthought/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.754949 hyperthought-0.9.9/src/hyperthought/api/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4133 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4427 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    34806 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/files.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/metatron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.754949 hyperthought-0.9.9/src/hyperthought/api/workflow/
+-rw-rw-rw-   0 root         (0) root         (0)    26153 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.755949 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.756949 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9154 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/root.py
+-rw-rw-rw-   0 root         (0) root         (0)     5634 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/unionfind.py
+-rw-rw-rw-   0 root         (0) root         (0)    11038 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/xml_generation.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/api/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9096 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4878 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.758949 hyperthought-0.9.9/src/hyperthought/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/_ayasdi.py
+-rw-rw-rw-   0 root         (0) root         (0)     5093 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/_centerstreet.py
+-rw-rw-rw-   0 root         (0) root         (0)     5729 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/_craic.py
+-rw-rw-rw-   0 root         (0) root         (0)     6650 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/_fei_tiff.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/_hyperspy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3548 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/_midas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3633 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/_nsidat.py
+-rw-rw-rw-   0 root         (0) root         (0)     2748 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.758949 hyperthought-0.9.9/src/hyperthought/parsers/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/parsers/utils/flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2021-10-25 20:01:26.000000 hyperthought-0.9.9/src/hyperthought/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 20:01:44.752949 hyperthought-0.9.9/src/hyperthought.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2021-10-25 20:01:44.000000 hyperthought-0.9.9/src/hyperthought.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2021-10-25 20:01:44.000000 hyperthought-0.9.9/src/hyperthought.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2021-10-25 20:01:44.000000 hyperthought-0.9.9/src/hyperthought.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       13 2021-10-25 20:01:44.000000 hyperthought-0.9.9/src/hyperthought.egg-info/top_level.txt
```

### Comparing `hyperthought-0.9.8/LICENSE` & `hyperthought-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/PKG-INFO` & `hyperthought-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought
-Version: 0.9.8
+Version: 0.9.9
 Summary: Wrappers for HyperThought® API
 Home-page: https://gitlab.com/hyperthought/hyperthought-easy-api
 Author: Jason Thiese
 Author-email: jasonthiese@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/hyperthought/hyperthought-easy-api/issues
 Platform: UNKNOWN
```

### Comparing `hyperthought-0.9.8/README.rst` & `hyperthought-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/setup.cfg` & `hyperthought-0.9.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hyperthought
-version = 0.9.8
+version = 0.9.9
 author = Jason Thiese
 author_email = jasonthiese@gmail.com
 description = Wrappers for HyperThought® API
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://gitlab.com/hyperthought/hyperthought-easy-api
 project_urls =
```

### Comparing `hyperthought-0.9.8/src/hyperthought/api/base.py` & `hyperthought-0.9.9/src/hyperthought/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,16 @@
                 )
 
                 if r.status_code >= 300:
                     raise APIError(
                         f"status code: {r.status_code}\n"
                         f"content: {r.content.decode()}"
                     )
+                else:
+                    return r
             except (requests.ConnectionError, APIError) as e:
                 attempts -= 1
 
                 if attempts == 0:
                     raise e
 
                 sleep(sleep_time)
```

### Comparing `hyperthought-0.9.8/src/hyperthought/api/common.py` & `hyperthought-0.9.9/src/hyperthought/api/common.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/files.py` & `hyperthought-0.9.9/src/hyperthought/api/files.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/metatron.py` & `hyperthought-0.9.9/src/hyperthought/api/metatron.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/search.py` & `hyperthought-0.9.9/src/hyperthought/api/search.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/workflow/__init__.py` & `hyperthought-0.9.9/src/hyperthought/api/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/coordinates.py` & `hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/coordinates.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/root.py` & `hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/root.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/algorithms/unionfind.py` & `hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/algorithms/unionfind.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/workflow/_construction/xml_generation.py` & `hyperthought-0.9.9/src/hyperthought/api/workflow/_construction/xml_generation.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/api/workspaces.py` & `hyperthought-0.9.9/src/hyperthought/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/auth.py` & `hyperthought-0.9.9/src/hyperthought/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This is a convenience module designed to manage OpenID Connect authorization
 to the HyperThought system.  Detailed usage instructions can be found in the
 Authorization class.
 """
 
 import base64
 from datetime import datetime
+from datetime import timedelta
 import json
 from threading import Thread
 from time import sleep
 
 import dateutil.parser
 from dateutil.tz import tzlocal
 import requests
@@ -109,17 +110,18 @@
         # This cookie is needed to avoid being redirected to the HyperThought
         # banner page.
         self._cookies = {
             'dodAccessBanner': 'true'
         }
 
         # Time to sleep prior to requesting an access token refresh.
-        expiration_time = dateutil.parser.parse(auth_payload['expiresAt'])
+        self._expiration_time = dateutil.parser.parse(
+            auth_payload['expiresAt'])
         current_time = datetime.now(tzlocal())
-        time_delta = expiration_time - current_time
+        time_delta = self._expiration_time - current_time
         self._seconds_to_expiration = time_delta.total_seconds()
 
         # Define a refresh thread without starting it.
         self._refresh_thread = Thread(target=self._refresh)
         self._refresh_thread.setDaemon(True)
         self._refresh_thread.start()
 
@@ -211,15 +213,21 @@
         if self._seconds_to_expiration < 0:
             raise AuthExpirationException(
                 "Unable to authenticate with expired token")
 
         # Request object, defined here for post-loop error handling.
         r = None
 
-        while self._seconds_to_expiration >= 0:
+        def remaining_time():
+            """Time remaining until token expiration, in seconds."""
+            return (
+                self._expiration_time - datetime.now(tzlocal())
+            ).total_seconds()
+
+        while remaining_time() >= 0:
             if self._delayed_refresh:
                 sleep_time = max(
                     self._seconds_to_expiration - REFRESH_WINDOW, 0)
                 sleep(sleep_time)
                 # Delayed refresh is only relevant for the first loop
                 # iteration.
                 self._delayed_refresh = False
@@ -242,15 +250,16 @@
                 sleep(REFRESH_RETRY_SLEEP_TIME)
                 continue
 
             auth_info = r.json()
             self._access_token = auth_info['access_token']
             self._refresh_token = auth_info['refresh_token']
             self._seconds_to_expiration = auth_info['expires_in']
-
+            self._expiration_time = datetime.now(tzlocal()) + timedelta(
+                seconds=self._seconds_to_expiration)
             sleep_time = max(self._seconds_to_expiration - REFRESH_WINDOW, 0)
             sleep(sleep_time)
 
         if r is not None:
             raise AuthExpirationException(
                 "Unable to refresh token. "
                 f"Call to {self._token_url} has failed. "
```

### Comparing `hyperthought-0.9.8/src/hyperthought/metadata.py` & `hyperthought-0.9.9/src/hyperthought/metadata.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/__init__.py` & `hyperthought-0.9.9/src/hyperthought/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/_ayasdi.py` & `hyperthought-0.9.9/src/hyperthought/parsers/_ayasdi.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/_centerstreet.py` & `hyperthought-0.9.9/src/hyperthought/parsers/_centerstreet.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/_craic.py` & `hyperthought-0.9.9/src/hyperthought/parsers/_craic.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/_fei_tiff.py` & `hyperthought-0.9.9/src/hyperthought/parsers/_fei_tiff.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/_hyperspy.py` & `hyperthought-0.9.9/src/hyperthought/parsers/_hyperspy.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/_midas.py` & `hyperthought-0.9.9/src/hyperthought/parsers/_midas.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/_nsidat.py` & `hyperthought-0.9.9/src/hyperthought/parsers/_nsidat.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/base.py` & `hyperthought-0.9.9/src/hyperthought/parsers/base.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/utils/__init__.py` & `hyperthought-0.9.9/src/hyperthought/parsers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/parsers/utils/flatten.py` & `hyperthought-0.9.9/src/hyperthought/parsers/utils/flatten.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought/utils.py` & `hyperthought-0.9.9/src/hyperthought/utils.py`

 * *Files identical despite different names*

### Comparing `hyperthought-0.9.8/src/hyperthought.egg-info/PKG-INFO` & `hyperthought-0.9.9/src/hyperthought.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought
-Version: 0.9.8
+Version: 0.9.9
 Summary: Wrappers for HyperThought® API
 Home-page: https://gitlab.com/hyperthought/hyperthought-easy-api
 Author: Jason Thiese
 Author-email: jasonthiese@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/hyperthought/hyperthought-easy-api/issues
 Platform: UNKNOWN
```

### Comparing `hyperthought-0.9.8/src/hyperthought.egg-info/SOURCES.txt` & `hyperthought-0.9.9/src/hyperthought.egg-info/SOURCES.txt`

 * *Files identical despite different names*

