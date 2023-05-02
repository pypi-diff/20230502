# Comparing `tmp/openworld-sdk-python-core-0.5.0.tar.gz` & `tmp/openworld-sdk-python-core-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-core-0.5.0.tar", last modified: Tue Mar 21 17:45:26 2023, max compression
+gzip compressed data, was "openworld-sdk-python-core-0.6.0.tar", last modified: Tue May  2 13:14:47 2023, max compression
```

## Comparing `openworld-sdk-python-core-0.5.0.tar` & `openworld-sdk-python-core-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.917060 openworld-sdk-python-core-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-21 17:45:26.917060 openworld-sdk-python-core-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.909060 openworld-sdk-python-core-0.5.0/client/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/client/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/client/openworld_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/client/rapid_auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.909060 openworld-sdk-python-core-0.5.0/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/configuration/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/configuration/client_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.913060 openworld-sdk-python-core-0.5.0/constant/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/constant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/constant/body.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/constant/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/constant/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/constant/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/constant/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/constant/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.913060 openworld-sdk-python-core-0.5.0/model/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/model/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/model/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.917060 openworld-sdk-python-core-0.5.0/model/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/model/exception/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/model/exception/openworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/model/exception/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/model/rapid_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.917060 openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-21 17:45:26.000000 openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-21 17:45:26.000000 openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:45:26.000000 openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 17:45:26.000000 openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-21 17:45:26.000000 openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 17:45:26.917060 openworld-sdk-python-core-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:45:26.917060 openworld-sdk-python-core-0.5.0/util/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-21 17:45:14.000000 openworld-sdk-python-core-0.5.0/util/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/client/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/client/openworld_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/client/rapid_auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/configuration/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/configuration/client_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/constant/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/constant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/constant/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/constant/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/constant/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/constant/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/constant/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/constant/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/model/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/model/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/model/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/model/exception/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/model/exception/openworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/model/exception/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/model/rapid_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-02 13:14:47.000000 openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-02 13:14:47.000000 openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:14:47.000000 openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:14:47.000000 openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 13:14:47.000000 openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:14:47.185311 openworld-sdk-python-core-0.6.0/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-02 13:14:33.000000 openworld-sdk-python-core-0.6.0/util/log.py
```

### Comparing `openworld-sdk-python-core-0.5.0/PKG-INFO` & `openworld-sdk-python-core-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-core
-Version: 0.5.0
+Version: 0.6.0
 Summary: Open World SDK Core Library for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-core-0.5.0/__init__.py` & `openworld-sdk-python-core-0.6.0/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/client/__init__.py` & `openworld-sdk-python-core-0.6.0/client/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/client/api.py` & `openworld-sdk-python-core-0.6.0/client/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import enum
 import json
 import logging
+import uuid
 from http import HTTPStatus
 from typing import Any, Optional
 
 import pydantic
 import pydantic.schema
 import requests
+from pydantic import BaseModel
 
 from openworld.sdk.core.client.auth_client import AuthClient
 from openworld.sdk.core.configuration.client_config import ClientConfig
 from openworld.sdk.core.constant import header as header_constant
 from openworld.sdk.core.constant import log as log_constant
 from openworld.sdk.core.constant.constant import OK_STATUS_CODES_RANGE
 from openworld.sdk.core.model.error import Error
@@ -124,24 +126,25 @@
 
     @staticmethod
     def __fill_request_headers(request_headers: dict):
         if not request_headers:
             request_headers = dict()
 
         request_header_keys = request_headers.keys()
-        for key in header_constant.API_REQUEST.keys():
+        for key, value in header_constant.API_REQUEST.items():
             if key in request_header_keys:
                 continue
 
-            request_headers[key] = header_constant.API_REQUEST[key]
+            request_headers[key] = value
 
         return request_headers
 
     @staticmethod
     def __prepare_request_headers(headers: dict) -> dict:
         request_headers = dict()
         for header_key, header_value in headers.items():
             if not header_value:
                 continue
-            request_headers[header_key] = json.dumps(header_value, default=pydantic.schema.pydantic_encoder)
+            needs_serialization: bool = isinstance(header_value, BaseModel) or isinstance(header_value, enum.Enum) or isinstance(header_value, uuid.UUID)
+            request_headers[header_key] = json.dumps(header_value, default=pydantic.schema.pydantic_encoder) if needs_serialization else header_value
 
         return ApiClient.__fill_request_headers(request_headers)
```

### Comparing `openworld-sdk-python-core-0.5.0/client/auth_client.py` & `openworld-sdk-python-core-0.6.0/client/auth_client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/client/openworld_auth_client.py` & `openworld-sdk-python-core-0.6.0/client/openworld_auth_client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/client/rapid_auth_client.py` & `openworld-sdk-python-core-0.6.0/client/rapid_auth_client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/configuration/__init__.py` & `openworld-sdk-python-core-0.6.0/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/configuration/auth_config.py` & `openworld-sdk-python-core-0.6.0/configuration/auth_config.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/configuration/client_config.py` & `openworld-sdk-python-core-0.6.0/configuration/client_config.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/constant/__init__.py` & `openworld-sdk-python-core-0.6.0/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/constant/body.py` & `openworld-sdk-python-core-0.6.0/constant/body.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/constant/constant.py` & `openworld-sdk-python-core-0.6.0/constant/constant.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/constant/header.py` & `openworld-sdk-python-core-0.6.0/constant/header.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,25 @@
 
 CONTENT_TYPE: str = "Content-type"
 
 JSON_CONTENT_TYPE: str = "application/json"
 
 ACCEPT: str = "Accept"
 
+ACCEPT_ENCODING: str = "Accept-Encoding"
+
+GZIP: str = "gzip"
+
 TRANSACTION_ID: str = "transaction-id"
 
 USER_AGENT: str = "User-agent"
 
 OPENWORLD_SDK_PYTHON: str = "open-world-sdk-python/"
 
-API_REQUEST: dict = {CONTENT_TYPE: JSON_CONTENT_TYPE, ACCEPT: JSON_CONTENT_TYPE}
+API_REQUEST: dict = {CONTENT_TYPE: JSON_CONTENT_TYPE, ACCEPT: JSON_CONTENT_TYPE, ACCEPT_ENCODING: GZIP}
 
 EAN: str = "EAN"
 
 API_KEY: str = "APIKey"
 
 SIGNATURE: str = "Signature"
```

### Comparing `openworld-sdk-python-core-0.5.0/constant/log.py` & `openworld-sdk-python-core-0.6.0/constant/log.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/constant/message.py` & `openworld-sdk-python-core-0.6.0/constant/message.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/constant/url.py` & `openworld-sdk-python-core-0.6.0/constant/url.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/model/__init__.py` & `openworld-sdk-python-core-0.6.0/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/model/authentication.py` & `openworld-sdk-python-core-0.6.0/model/authentication.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/model/error.py` & `openworld-sdk-python-core-0.6.0/model/error.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/model/exception/client.py` & `openworld-sdk-python-core-0.6.0/model/exception/client.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/model/exception/openworld.py` & `openworld-sdk-python-core-0.6.0/model/exception/openworld.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/model/exception/service.py` & `openworld-sdk-python-core-0.6.0/model/exception/service.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/model/rapid_auth.py` & `openworld-sdk-python-core-0.6.0/model/rapid_auth.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/PKG-INFO` & `openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-core
-Version: 0.5.0
+Version: 0.6.0
 Summary: Open World SDK Core Library for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-core-0.5.0/openworld_sdk_python_core.egg-info/SOURCES.txt` & `openworld-sdk-python-core-0.6.0/openworld_sdk_python_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/setup.py` & `openworld-sdk-python-core-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/util/__init__.py` & `openworld-sdk-python-core-0.6.0/util/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-core-0.5.0/util/log.py` & `openworld-sdk-python-core-0.6.0/util/log.py`

 * *Files identical despite different names*

