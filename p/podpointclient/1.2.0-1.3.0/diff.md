# Comparing `tmp/podpointclient-1.2.0.tar.gz` & `tmp/podpointclient-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podpointclient-1.2.0.tar", last modified: Thu Jan 12 21:37:33 2023, max compression
+gzip compressed data, was "podpointclient-1.3.0.tar", last modified: Tue May  2 15:25:45 2023, max compression
```

## Comparing `podpointclient-1.2.0.tar` & `podpointclient-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 21:37:33.100207 podpointclient-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-12 21:37:18.000000 podpointclient-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-01-12 21:37:33.100207 podpointclient-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-01-12 21:37:18.000000 podpointclient-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 21:37:33.096207 podpointclient-1.2.0/podpointclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 21:37:33.100207 podpointclient-1.2.0/podpointclient/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/helpers/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-12 21:37:18.000000 podpointclient-1.2.0/podpointclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 21:37:33.100207 podpointclient-1.2.0/podpointclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-01-12 21:37:33.000000 podpointclient-1.2.0/podpointclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-01-12 21:37:33.000000 podpointclient-1.2.0/podpointclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 21:37:33.000000 podpointclient-1.2.0/podpointclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-12 21:37:33.000000 podpointclient-1.2.0/podpointclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-12 21:37:33.000000 podpointclient-1.2.0/podpointclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-12 21:37:18.000000 podpointclient-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 21:37:33.100207 podpointclient-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-12 21:37:18.000000 podpointclient-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:45.322381 podpointclient-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 15:25:28.000000 podpointclient-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-02 15:25:45.322381 podpointclient-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-02 15:25:28.000000 podpointclient-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:45.322381 podpointclient-1.3.0/podpointclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/charge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/charge_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:45.322381 podpointclient-1.3.0/podpointclient/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/helpers/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15361 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 15:25:28.000000 podpointclient-1.3.0/podpointclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:45.322381 podpointclient-1.3.0/podpointclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-02 15:25:45.000000 podpointclient-1.3.0/podpointclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-02 15:25:45.000000 podpointclient-1.3.0/podpointclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:25:45.000000 podpointclient-1.3.0/podpointclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 15:25:45.000000 podpointclient-1.3.0/podpointclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 15:25:45.000000 podpointclient-1.3.0/podpointclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 15:25:28.000000 podpointclient-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:25:45.322381 podpointclient-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 15:25:28.000000 podpointclient-1.3.0/setup.py
```

### Comparing `podpointclient-1.2.0/LICENSE` & `podpointclient-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/PKG-INFO` & `podpointclient-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.2.0
+Version: 1.3.0
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.2.0/README.md` & `podpointclient-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/podpointclient/charge.py` & `podpointclient-1.3.0/podpointclient/charge.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/podpointclient/errors.py` & `podpointclient-1.3.0/podpointclient/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,7 +15,12 @@
         message = f'Session Error ({status}) - {response}'
         super().__init__(message)
 
 class ApiConnectionError(APIError):
     """An error relating to connecting to pod point"""
     def __init__(self, message):
         super().__init__(f'Connection Error: {message}')
+
+class ChargeOverrideValidationError(Exception):
+    """An error relating to connecting to pod point"""
+    def __init__(self):
+        super().__init__(f'A validate error occured when processing charge override. Please ensure that an hour, minute or second value is passed and that it is > 0.')
```

### Comparing `podpointclient-1.2.0/podpointclient/factories.py` & `podpointclient-1.3.0/podpointclient/factories.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Factories used to create top level objects such as pods, sessions and charges"""
 from typing import Dict, Any, List
 from .pod import Pod, Firmware
 from .user import User
 from .schedule import Schedule, ScheduleStatus
 from .charge import Charge
+from .charge_override import ChargeOverride
 
 class PodFactory:
     """Factory for creating Pod objects"""
     def build_pods(self, pods_response: Dict[str, Any]) -> List[Pod]:
         """Build a number of pod objects based off of a response from pod point"""
         pods = []
 
@@ -58,14 +59,22 @@
             return charges
 
         for charge in charge_data:
             charges.append(Charge(data=charge))
 
         return charges
 
+class ChargeOverrideFactory:
+    """Factory  for creating Charge objects"""
+    def build_charge_override(self, charge_override_response: Dict[str, Any]) -> ChargeOverride:
+        """Build a list of charge objects based off of a response from pod point"""
+        if charge_override_response is None:
+            return None
+
+        return ChargeOverride(data=charge_override_response)
 
 class FirmwareFactory:
     """Factory  for creating Firmware objects"""
     def build_firmwares(self, firmware_response: Dict[str, Any]) -> List[Firmware]:
         """Build a list of firmware objects based off of a response from pod point"""
         firmwares = []
```

### Comparing `podpointclient-1.2.0/podpointclient/helpers/api_wrapper.py` & `podpointclient-1.3.0/podpointclient/helpers/api_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,30 @@
             url=url,
             params=params,
             data=body,
             headers=headers,
             exception_class=exception_class
         )
 
+    async def delete(
+        self,
+        url: str,
+        headers: Dict[str, Any],
+        params: Dict[str, Any] = None,
+        exception_class=APIError
+    ) -> aiohttp.ClientResponse:
+        """Make a GET request"""
+        return await self.__wrapper(
+            method="delete",
+            url=url,
+            params=params,
+            headers=headers,
+            exception_class=exception_class
+        )
+
     async def __wrapper(
         self,
         method: str,
         url: str,
         data: Dict[str, Any] = None,
         headers: Dict[str, Any] = None,
         params: Dict[str, Any] = None,
@@ -111,27 +127,31 @@
                 elif method == "post":
                     response = await self._session.post(
                         url,
                         headers=headers,
                         params=params,
                         json=data
                     )
+
+                elif method == "delete":
+                    response = await self._session.delete(url, headers=headers, params=params)
+
                 else:
                     raise ValueError(f'Method \'{method}\' not supported')
 
                 if response is None:
                     raise APIError(
                         "Unexpected error from Pod Point API. \
 Received a None response when querying."
                     )
 
                 end_time = time.time()
                 _LOGGER.debug("%s - %ss", response.status, end_time - start_time)
 
-                if response.status < 200 or response.status > 202:
+                if response.status < 200 or response.status > 204:
                     await self.__handle_response_error(
                         response=response,
                         exception_class=exception_class
                     )
 
                 return response
 
@@ -144,15 +164,15 @@
                 "Error parsing information from %s - %s",
                 url,
                 exception,
             )
             raise exception
 
         except (aiohttp.ClientError, gaierror) as exception:
-            message = "Error connecting to Pod Point ({url}) - {exception}"
+            message = f"Error connecting to Pod Point ({url}) - {exception}"
             raise ApiConnectionError(message) from exception
 
         except (AuthError, SessionError) as exception:
             _LOGGER.error(
                 "Authentication error when creating auth or session. (%s)",
                 type(exception)
             )
```

### Comparing `podpointclient-1.2.0/podpointclient/helpers/auth.py` & `podpointclient-1.3.0/podpointclient/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/podpointclient/helpers/functions.py` & `podpointclient-1.3.0/podpointclient/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/podpointclient/helpers/session.py` & `podpointclient-1.3.0/podpointclient/helpers/session.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/podpointclient/pod.py` & `podpointclient-1.3.0/podpointclient/pod.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from enum import auto
 import json
 from strenum import StrEnum, KebabCaseStrEnum
 
 from .helpers.functions import lazy_convert_to_datetime, lazy_iso_format_datetime
 from .schedule import Schedule, ScheduleStatus
 from .charge import Charge
+from .charge_mode import ChargeMode
+from .charge_override import ChargeOverride
 
 
 class StatusName(StrEnum):
     """An ENUM representing the statuses for a given connector/door on a pod point pod"""
     AVAILABLE      = "Available"
     UNAVAILABLE    = "Unavailable"
     CHARGING       = "Charging"
@@ -238,14 +240,19 @@
                     start_time = charge_schedule_data.get('start_time', None),
                     end_day = charge_schedule_data.get('end_day', None),
                     end_time = charge_schedule_data.get('end_time', None),
                     status = status_obj
                 )
             )
 
+        self.charge_override = None
+        charge_override_data = data.get('charge_override', None)
+        if charge_override_data is not None:
+            self.charge_override = ChargeOverride(data=charge_override_data)
+
 
     @property
     def dict(self) -> Dict[str, Any]:
         """Dictionary representaion of a Pod"""
         dictionary = {
             "id": self.id,
             "name": self.name,
@@ -268,15 +275,16 @@
             "statuses": [],
             "unit_connectors": [],
             "charge_schedules": [],
             "total_kwh": self.total_kwh,
             "total_charge_seconds": self.total_charge_seconds,
             "current_kwh": self.current_kwh,
             "total_cost": self.total_cost,
-            "firmware": None
+            "firmware": None,
+            "charge_override": None
         }
 
         for status in self.statuses:
             dictionary['statuses'].append(status.dict)
 
         for unit_connector in self.unit_connectors:
             dictionary['unit_connectors'].append(
@@ -285,20 +293,40 @@
 
         for charge_schedule in self.charge_schedules:
             dictionary['charge_schedules'].append(charge_schedule.dict)
 
         if isinstance(self.firmware, Firmware):
             dictionary['firmware'] = self.firmware.dict
 
+        if isinstance(self.charge_override, ChargeOverride):
+            dictionary['charge_override'] = self.charge_override.dict
+
         return dictionary
 
     def to_json(self) -> str:
         """JSON representation of a Pod"""
         return json.dumps(self.dict, ensure_ascii=False)
+    
+    @property
+    def charge_mode(self) -> ChargeMode:
+        """what is the current charge override mode?"""
+        override = self.charge_override
+
+        if override is None or override.ppid is None:
+            return ChargeMode.SMART
 
+        if override.active:
+            return ChargeMode.OVERRIDE
+
+        elif override.requested_at is not None and self.recieved_at is not None and self.ends_at is None:
+            return ChargeMode.MANUAL
+
+        else:
+            _LOGGER.warn("Unable to caclculate charge mode")
+            return None
 
     @dataclass
     class Model:
         """Representation of a Model within a Pod from pod point"""
         id: int
         name: str
         vendor: str
```

### Comparing `podpointclient-1.2.0/podpointclient/schedule.py` & `podpointclient-1.3.0/podpointclient/schedule.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/podpointclient/user.py` & `podpointclient-1.3.0/podpointclient/user.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.2.0/podpointclient.egg-info/PKG-INFO` & `podpointclient-1.3.0/podpointclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.2.0
+Version: 1.3.0
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.2.0/podpointclient.egg-info/SOURCES.txt` & `podpointclient-1.3.0/podpointclient.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 podpointclient/__init__.py
 podpointclient/charge.py
+podpointclient/charge_mode.py
+podpointclient/charge_override.py
 podpointclient/client.py
 podpointclient/endpoints.py
 podpointclient/errors.py
 podpointclient/factories.py
 podpointclient/pod.py
 podpointclient/schedule.py
 podpointclient/user.py
```

### Comparing `podpointclient-1.2.0/setup.py` & `podpointclient-1.3.0/setup.py`

 * *Files identical despite different names*

