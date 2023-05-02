# Comparing `tmp/quakesaver_client-1.1.1.tar.gz` & `tmp/quakesaver_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quakesaver_client-1.1.1.tar", max compression
+gzip compressed data, was "quakesaver_client-1.2.0.tar", max compression
```

## Comparing `quakesaver_client-1.1.1.tar` & `quakesaver_client-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1497 2023-04-20 10:23:55.210679 quakesaver_client-1.1.1/LICENSE
--rw-r--r--   0        0        0     4233 2023-04-20 10:23:55.210679 quakesaver_client-1.1.1/README.md
--rw-r--r--   0        0        0     2291 2023-04-20 10:24:59.847141 quakesaver_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3869 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/__init__.py
--rw-r--r--   0        0        0      624 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/errors.py
--rw-r--r--   0        0        0       56 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/data_product_query.py
--rw-r--r--   0        0        0     4078 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/data_products.py
--rw-r--r--   0        0        0     2377 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/measurement.py
--rw-r--r--   0        0        0      365 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/permission.py
--rw-r--r--   0        0        0     9762 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/sensor.py
--rw-r--r--   0        0        0    69437 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/sensor_state.py
--rw-r--r--   0        0        0      205 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/token.py
--rw-r--r--   0        0        0      743 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/models/warnings.py
--rw-r--r--   0        0        0      387 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/types.py
--rw-r--r--   0        0        0     1718 2023-04-20 10:23:55.214679 quakesaver_client-1.1.1/quakesaver_client/util.py
--rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 quakesaver_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5076 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/README.md
+-rw-r--r--   0        0        0     2334 2023-05-02 16:48:59.228949 quakesaver_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4428 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/__init__.py
+-rw-r--r--   0        0        0     3220 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/client_websocket.py
+-rw-r--r--   0        0        0      710 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/errors.py
+-rw-r--r--   0        0        0     1969 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/fdsnws.py
+-rw-r--r--   0        0        0       56 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/models/__init__.py
+-rw-r--r--   0        0        0     9978 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/models/cloud_sensor.py
+-rw-r--r--   0        0        0     1763 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/models/data_product_query.py
+-rw-r--r--   0        0        0     4078 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/models/data_products.py
+-rw-r--r--   0        0        0     6256 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/models/local_sensor.py
+-rw-r--r--   0        0        0     2377 2023-05-02 16:48:07.985180 quakesaver_client-1.2.0/quakesaver_client/models/measurement.py
+-rw-r--r--   0        0        0      365 2023-05-02 16:48:07.989180 quakesaver_client-1.2.0/quakesaver_client/models/permission.py
+-rw-r--r--   0        0        0    69437 2023-05-02 16:48:07.989180 quakesaver_client-1.2.0/quakesaver_client/models/sensor_state.py
+-rw-r--r--   0        0        0      205 2023-05-02 16:48:07.989180 quakesaver_client-1.2.0/quakesaver_client/models/token.py
+-rw-r--r--   0        0        0      743 2023-05-02 16:48:07.989180 quakesaver_client-1.2.0/quakesaver_client/models/warnings.py
+-rw-r--r--   0        0        0      436 2023-05-02 16:48:07.989180 quakesaver_client-1.2.0/quakesaver_client/models/websocket.py
+-rw-r--r--   0        0        0      387 2023-05-02 16:48:07.989180 quakesaver_client-1.2.0/quakesaver_client/types.py
+-rw-r--r--   0        0        0     1718 2023-05-02 16:48:07.989180 quakesaver_client-1.2.0/quakesaver_client/util.py
+-rw-r--r--   0        0        0     5918 1970-01-01 00:00:00.000000 quakesaver_client-1.2.0/PKG-INFO
```

### Comparing `quakesaver_client-1.1.1/LICENSE` & `quakesaver_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.1/README.md` & `quakesaver_client-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 ## Getting Started
 
 ### Setting up the client
 
 `EMAIL` and `PASSWORD` correspond to the credentials you use to log in at [https://network.quakesaver.net](https://network.quakesaver.net).
 
 ```python
-from quakesaver_client import QSClient
+from quakesaver_client import QSCloudClient
 
 EMAIL = "user@yourorganisation.net"
 PASSWORD = "!verstrongpassword1"
 
-client = QSClient(email=EMAIL, password=PASSWORD)
+client = QSCloudClient(email=EMAIL, password=PASSWORD)
 ```
 
-### Full example script
+### Example to stream from the cloud
 
 Authenticate against the quakesaver server and download raw, as well as processed data.
 
 Please note, that for security reasons each login session is only valid for 15 minutes. Thus, the client is not designed for long-term connections but for repeated queries.
 
 ```python
 """Example script for quakesaver_client usage."""
@@ -36,23 +36,23 @@
 import sys
 from datetime import datetime, timedelta
 from pprint import pp
 
 import obspy
 from obspy import Stream
 
-from quakesaver_client import QSClient
+from quakesaver_client import QSCloudClient
 from quakesaver_client.models.data_product_query import DataProductQuery
 from quakesaver_client.models.measurement import MeasurementQuery
 
 EMAIL = "user@yourorganisation.net"
 PASSWORD = "!verstrongpassword1"
 DATA_PATH = "./data"
 
-client = QSClient(email=EMAIL, password=PASSWORD)
+client = QSCloudClient(email=EMAIL, password=PASSWORD)
 
 # Get a list of all available sensor IDs:
 sensor_ids = client.get_sensor_ids()
 pp(sensor_ids)
 
 if len(sensor_ids) == 0:
     print("No sensors available")
@@ -127,7 +127,47 @@
 )
 
 # Read the file into obspy for further processing...
 stream: Stream = obspy.read(file_path)
 for trace in stream.traces:
     print(trace.stats)
 ```
+
+## `QSLocalClient` Examples
+
+Interact with sensors on your local network using the `QSLocalClient`.
+
+### Streaming Data
+
+```python
+import asyncio
+from quakesaver_client import QSLocalClient
+
+
+async def run():
+    client = QSLocalClient()
+
+    sensor = client.get_sensor("qssensor.local")
+    stream = sensor.get_waveform_stream()
+    async for chunk in stream.start():
+        print(chunk)
+
+
+asyncio.run(run())
+```
+
+### Downloading Data
+
+Download the latest 10 minutes from a local sensor and write that into a file:
+
+```python
+import datetime
+from quakesaver_client import QSLocalClient
+
+client = QSLocalClient()
+sensor = client.get_sensor("qssensor.local")
+
+tmax = datetime.datetime.utcnow()
+tmin = tmax - datetime.timedelta(minutes=10)
+file_path = sensor.get_waveform_data(tmin, tmax)
+print(file_path)
+```
```

#### html2text {}

```diff
@@ -4,41 +4,42 @@
 QuakeSaver/quakesaver-client/actions/workflows/test.yml/badge.svg)](https://
 github.com/QuakeSaver/quakesaver-client/actions/workflows/test.yml) [Code
 style:_black] This is the client for the [QuakeSaver](https://quakesaver.net/
 ) Sensor services. You can find the documentation [here](https://
 quakesaver.github.io/quakesaver-client/). ## Getting Started ### Setting up the
 client `EMAIL` and `PASSWORD` correspond to the credentials you use to log in
 at [https://network.quakesaver.net](https://network.quakesaver.net). ```python
-from quakesaver_client import QSClient EMAIL = "user@yourorganisation.net"
-PASSWORD = "!verstrongpassword1" client = QSClient(email=EMAIL,
-password=PASSWORD) ``` ### Full example script Authenticate against the
-quakesaver server and download raw, as well as processed data. Please note,
-that for security reasons each login session is only valid for 15 minutes.
-Thus, the client is not designed for long-term connections but for repeated
-queries. ```python """Example script for quakesaver_client usage.""" import sys
-from datetime import datetime, timedelta from pprint import pp import obspy
-from obspy import Stream from quakesaver_client import QSClient from
-quakesaver_client.models.data_product_query import DataProductQuery from
-quakesaver_client.models.measurement import MeasurementQuery EMAIL =
-"user@yourorganisation.net" PASSWORD = "!verstrongpassword1" DATA_PATH = "./
-data" client = QSClient(email=EMAIL, password=PASSWORD) # Get a list of all
-available sensor IDs: sensor_ids = client.get_sensor_ids() pp(sensor_ids) if
-len(sensor_ids) == 0: print("No sensors available") sys.exit() # For
-demonstration, we use the first sensor in the list sensor_uid_to_get =
-sensor_ids[0] # Get the sensor from the client sensor = client.get_sensor
-(sensor_uid_to_get) pp(sensor.dict()) # Queries such as waveforms, station
-metadata and measurements (data products calculated # on the sensor) # require
-that you select a time window. We use that last 5 hours of data end_time =
-datetime.utcnow() start_time = end_time - timedelta(hours=5) # Query various
-Measurements. In this case we calculate a rolling `mean` over 10 minutes # time
-windows. # Other `aggregators` are: # * None (default) # * max # * min query =
-MeasurementQuery( start_time=start_time, end_time=end_time, interval=timedelta
-(minutes=10), aggregator="mean", ) result = sensor.get_jma_intensity(query)
-print(result) result = sensor.get_peak_ground_acceleration(query) print(result)
-result = sensor.get_spectral_intensity(query) print(result) result =
+from quakesaver_client import QSCloudClient EMAIL = "user@yourorganisation.net"
+PASSWORD = "!verstrongpassword1" client = QSCloudClient(email=EMAIL,
+password=PASSWORD) ``` ### Example to stream from the cloud Authenticate
+against the quakesaver server and download raw, as well as processed data.
+Please note, that for security reasons each login session is only valid for 15
+minutes. Thus, the client is not designed for long-term connections but for
+repeated queries. ```python """Example script for quakesaver_client usage."""
+import sys from datetime import datetime, timedelta from pprint import pp
+import obspy from obspy import Stream from quakesaver_client import
+QSCloudClient from quakesaver_client.models.data_product_query import
+DataProductQuery from quakesaver_client.models.measurement import
+MeasurementQuery EMAIL = "user@yourorganisation.net" PASSWORD =
+"!verstrongpassword1" DATA_PATH = "./data" client = QSCloudClient(email=EMAIL,
+password=PASSWORD) # Get a list of all available sensor IDs: sensor_ids =
+client.get_sensor_ids() pp(sensor_ids) if len(sensor_ids) == 0: print("No
+sensors available") sys.exit() # For demonstration, we use the first sensor in
+the list sensor_uid_to_get = sensor_ids[0] # Get the sensor from the client
+sensor = client.get_sensor(sensor_uid_to_get) pp(sensor.dict()) # Queries such
+as waveforms, station metadata and measurements (data products calculated # on
+the sensor) # require that you select a time window. We use that last 5 hours
+of data end_time = datetime.utcnow() start_time = end_time - timedelta(hours=5)
+# Query various Measurements. In this case we calculate a rolling `mean` over
+10 minutes # time windows. # Other `aggregators` are: # * None (default) # *
+max # * min query = MeasurementQuery( start_time=start_time, end_time=end_time,
+interval=timedelta(minutes=10), aggregator="mean", ) result =
+sensor.get_jma_intensity(query) print(result) result =
+sensor.get_peak_ground_acceleration(query) print(result) result =
+sensor.get_spectral_intensity(query) print(result) result =
 sensor.get_rms_offset(query) print(result) # Query various Data Products. You
 can only get 100 results at once, which is why there # are limit and skip
 values. You can get data products from a specific time frame, by # specifying
 start and end times. end_time = datetime.utcnow() start_time = end_time -
 timedelta(hours=5) query = DataProductQuery( start_time=start_time,
 end_time=end_time, limit=100, skip=0, ) result = sensor.get_event_records
 (query) print(result) result = sensor.get_hv_spectra(query) print(result)
@@ -47,8 +48,18 @@
 = sensor.get_stationxml( starttime=start_time, endtime=end_time,
 level="response", location_to_store=DATA_PATH, ) with open(file_path, "r") as
 file: print(file.read()) # Download raw full waveforms from the sensor. Note
 that you can only query what is in # the sensor's ringbuffer (usually the last
 ~ 48 hours). file_path = sensor.get_waveform_data( start_time=start_time,
 end_time=end_time, location_to_store=DATA_PATH ) # Read the file into obspy for
 further processing... stream: Stream = obspy.read(file_path) for trace in
-stream.traces: print(trace.stats) ```
+stream.traces: print(trace.stats) ``` ## `QSLocalClient` Examples Interact with
+sensors on your local network using the `QSLocalClient`. ### Streaming Data
+```python import asyncio from quakesaver_client import QSLocalClient async def
+run(): client = QSLocalClient() sensor = client.get_sensor("qssensor.local")
+stream = sensor.get_waveform_stream() async for chunk in stream.start(): print
+(chunk) asyncio.run(run()) ``` ### Downloading Data Download the latest 10
+minutes from a local sensor and write that into a file: ```python import
+datetime from quakesaver_client import QSLocalClient client = QSLocalClient()
+sensor = client.get_sensor("qssensor.local") tmax = datetime.datetime.utcnow()
+tmin = tmax - datetime.timedelta(minutes=10) file_path =
+sensor.get_waveform_data(tmin, tmax) print(file_path) ```
```

### Comparing `quakesaver_client-1.1.1/pyproject.toml` & `quakesaver_client-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "quakesaver-client"
-version = "1.1.1"
+version = "1.2.0"
 description = "Client library for interacting with the QuakeSaver sensor fleet."
 authors = ["QuakeSaver <info@quakesaver.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "quakesaver_client"}]
 homepage = "https://quakesaver.net/"
 repository = "https://github.com/QuakeSaver/quakesaver-client"
 documentation = "https://quakesaver.github.io/quakesaver-client/"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pydantic = "~=1.10.5"
 requests = "~=2.28.2"
+aiohttp = "^3.8.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 Sphinx = "^6.1.0"
 pre-commit = "^3.1.0"
@@ -73,14 +74,15 @@
     ".eggs",
     ".git",
     ".pytype",
     ".ruff_cache",
     "__pypackages__",
     "build",
     "dist",
+    "tests/conftest.py"
 ]
 line-length = 88
 target-version = "py310"
 
 [tool.ruff.per-file-ignores]
 # due to autogeneration
 "quakesaver_client/models/data_products.py" = ["D100", "D101", "D106", "F722", "F821"]
```

### Comparing `quakesaver_client-1.1.1/quakesaver_client/__init__.py` & `quakesaver_client-1.2.0/quakesaver_client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
 import requests
 from pydantic import ValidationError
 
 from quakesaver_client.errors import (
     CorruptedDataError,
 )
-from quakesaver_client.models.sensor import Sensor
+from quakesaver_client.models.cloud_sensor import CloudSensor
+from quakesaver_client.models.local_sensor import LocalSensor
 from quakesaver_client.models.token import Token
 from quakesaver_client.util import handle_response
 
 DecoratedFunction = TypeVar("DecoratedFunction", bound=Callable[..., Any])
 
 
 def _needs_token(function: DecoratedFunction) -> DecoratedFunction:
     @wraps(function)
     def request_token_if_needed(
-        self: QSClient, *args: list, **kwargs: dict
+        self: QSCloudClient, *args: list, **kwargs: dict
     ) -> DecoratedFunction:
         if not self._token:
-            logging.debug("QSClient requesting user _token.")
+            logging.debug("QSCloudClient requesting user _token.")
             response = requests.post(
                 url=f"{self._api_base_url}/user/get_token",
                 data=f"username={self._email}&password={self._password}",
                 headers={"Content-Type": "application/x-www-form-urlencoded"},
             )
             response_data = handle_response(response)
             try:
@@ -38,28 +39,28 @@
             self._token = token
 
         return function(self, *args, **kwargs)
 
     return request_token_if_needed
 
 
-class QSClient:
+class QSCloudClient:
     """A class representing a client to the backend."""
 
     _base_domain: str
 
     _email: str
     _password: str
     _token: Token | None
 
     _api_base_url: str
     _fdsn_base_url: str
 
     def __init__(
-        self: QSClient,
+        self: QSCloudClient,
         email: str,
         password: str,
         base_domain: str | None = "network.quakesaver.net",
     ) -> None:
         """Create an instance of the class.
 
         Args:
@@ -73,49 +74,64 @@
 
         self._base_domain = base_domain
 
         self._api_base_url = f"https://api.{base_domain}/api/v1"
         self._fdsn_base_url = f"https://fdsnws.{base_domain}/fdsnws"
 
     @_needs_token
-    def _get_authorization_headers(self: QSClient) -> dict:
+    def _get_authorization_headers(self: QSCloudClient) -> dict:
         return {"Authorization": f"{self._token.token_type} {self._token.access_token}"}
 
-    def get_sensor_ids(self: QSClient) -> list[str]:
+    def get_sensor_ids(self: QSCloudClient) -> list[str]:
         """Fetch all sensor UIDs the user has access to.
 
         Returns:
             list[str]: The list of sensor UIDs.
         """
-        logging.debug("QSClient requesting sensor ids.")
+        logging.debug("QSCloudClient requesting sensor ids.")
         response = requests.get(
             url=f"{self._api_base_url}/user/me/sensors",
             headers=self._get_authorization_headers(),
         )
         response_data = handle_response(response)
         return list(response_data.keys())
 
-    def get_sensor(self: QSClient, sensor_uid: str) -> Sensor:
+    def get_sensor(self: QSCloudClient, sensor_uid: str) -> CloudSensor:
         """Fetch sensor data.
 
         Args:
             sensor_uid: The UID to request data from.
 
         Returns:
-            Sensor: A sensor model to work with.
+            CloudSensor: A sensor model to work with.
         """
-        logging.debug("QSClient requesting sensor %s.", sensor_uid)
+        logging.debug("QSCloudClient requesting sensor %s.", sensor_uid)
         response = requests.get(
             url=f"{self._api_base_url}/sensors/{sensor_uid}",
             headers=self._get_authorization_headers(),
         )
         response_data = handle_response(response)
         try:
-            sensor = Sensor(
+            sensor = CloudSensor(
                 api_base_url=self._api_base_url,
                 fdsn_base_url=self._fdsn_base_url,
                 headers=self._get_authorization_headers(),
                 **response_data,
             )
         except ValidationError as e:
             raise CorruptedDataError from e
         return sensor
+
+
+class QSLocalClient:
+    """Client to interact with sensors on your local network."""
+
+    @classmethod
+    def get_sensor(cls: QSLocalClient, sensor_url: str) -> LocalSensor:
+        """Get a `LocalSensor` from the url."""
+        try:
+            sensor = LocalSensor.get_sensor(sensor_url)
+
+        except Exception as e:
+            raise Exception(f"Failed to get sensor at {sensor_url}") from e
+
+        return sensor
```

### Comparing `quakesaver_client-1.1.1/quakesaver_client/errors.py` & `quakesaver_client-1.2.0/quakesaver_client/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,13 +9,17 @@
     """An error to raise if wrong authentication details where provided."""
 
 
 class CorruptedDataError(ValueError):
     """An error to raise if data was incomplete or wrong."""
 
 
+class NoDataError(ValueError):
+    """An error to raise if no data is available."""
+
+
 class SessionExpiredError(RuntimeError):
     """An error to raise if the token is expired."""
 
 
 class InsufficientPermissionError(RuntimeError):
     """An error to raise if the user is not allowed to read or do things."""
```

### Comparing `quakesaver_client-1.1.1/quakesaver_client/models/data_product_query.py` & `quakesaver_client-1.2.0/quakesaver_client/models/data_product_query.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.1/quakesaver_client/models/data_products.py` & `quakesaver_client-1.2.0/quakesaver_client/models/data_products.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.1/quakesaver_client/models/measurement.py` & `quakesaver_client-1.2.0/quakesaver_client/models/measurement.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.1/quakesaver_client/models/sensor.py` & `quakesaver_client-1.2.0/quakesaver_client/models/cloud_sensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,58 +23,62 @@
 from quakesaver_client.models.permission import Permission
 from quakesaver_client.models.sensor_state import SensorState
 from quakesaver_client.models.warnings import SensorWarnings
 from quakesaver_client.types import StationDetailLevel
 from quakesaver_client.util import assure_output_path, handle_response
 
 
-class Sensor(SensorState):
+class CloudSensor(SensorState):
     """A base schema for other schemas to derive from."""
 
     _headers: dict
     _api_base_url: str
     _fdsn_base_url: str
 
     first_seen: datetime
     last_updated: datetime
     permission: Permission
     warnings: SensorWarnings
     max_data_product_count: int
 
     def __init__(
-        self: Sensor, api_base_url: str, fdsn_base_url: str, headers: dict, **data: dict
+        self: CloudSensor,
+        api_base_url: str,
+        fdsn_base_url: str,
+        headers: dict,
+        **data: dict,
     ) -> None:
         """Create an instance of the class."""
         super().__init__(**data)
         self._headers = headers
         self._api_base_url = api_base_url
         self._fdsn_base_url = fdsn_base_url
 
     def _get_data_product(
-        self: Sensor,
+        self: CloudSensor,
         data_product_name: str,
         query: DataProductQuery,
     ) -> dict:
         """Request data products of the sensor."""
         logging.debug(
-            "QSClient requesting data product %s for sensor %s.",
+            "QSCloudClient requesting data product %s for sensor %s.",
             data_product_name,
             self.uid,
         )
         response = requests.post(
             url=f"{self._api_base_url}/sensors/{self.uid}/data_products/{data_product_name}",
             headers=self._headers,
             params=query.dict(),
             data=[],
         )
         response_data = handle_response(response)
         return response_data
 
     def get_event_records(
-        self: Sensor, query: DataProductQuery
+        self: CloudSensor, query: DataProductQuery
     ) -> EventRecordQueryResult:
         """Get Event Records of the sensor.
 
         Args:
             query: The query parameters like time limit and time frame.
 
         Returns:
@@ -84,15 +88,17 @@
 
         try:
             result = EventRecordQueryResult.parse_obj(result)
         except ValidationError as e:
             raise CorruptedDataError() from e
         return result
 
-    def get_hv_spectra(self: Sensor, query: DataProductQuery) -> HVSpectraQueryResult:
+    def get_hv_spectra(
+        self: CloudSensor, query: DataProductQuery
+    ) -> HVSpectraQueryResult:
         """Get HV Spectres of the sensor.
 
         Args:
             query: The query parameters like time limit and time frame.
 
         Returns:
             HVSpectraQueryResult: The queried data products.
@@ -102,15 +108,15 @@
         try:
             result = HVSpectraQueryResult.parse_obj(result)
         except ValidationError as e:
             raise CorruptedDataError() from e
         return result
 
     def get_noise_autocorrelations(
-        self: Sensor, query: DataProductQuery
+        self: CloudSensor, query: DataProductQuery
     ) -> NoiseAutocorrelationQueryResult:
         """Get the Event Records of the sensor.
 
         Args:
             query: The query parameters like time limit and time frame.
 
         Returns:
@@ -121,76 +127,80 @@
         try:
             result = NoiseAutocorrelationQueryResult.parse_obj(result)
         except ValidationError as e:
             raise CorruptedDataError() from e
         return result
 
     def _get_measurement(
-        self: Sensor, query: MeasurementQueryFull
+        self: CloudSensor, query: MeasurementQueryFull
     ) -> MeasurementResult:
         """Request measurements of the sensor."""
-        logging.debug("QSClient requesting measurement for sensor %s.", self.uid)
+        logging.debug("QSCloudClient requesting measurement for sensor %s.", self.uid)
         response = requests.post(
             url=f"{self._api_base_url}/sensors/{self.uid}/measurements",
             headers=self._headers,
             data=query.json(),
         )
         response_data = handle_response(response)
         try:
             result = MeasurementResult(**response_data)
         except ValidationError as e:
             raise CorruptedDataError() from e
         return result
 
     def get_peak_horizontal_acceleration(
-        self: Sensor, query: MeasurementQuery
+        self: CloudSensor, query: MeasurementQuery
     ) -> MeasurementResult:
         """Get the PGA measurement of the sensor.
 
         Args:
             query: The query parameters like time frame and aggregator.
 
         Returns:
             MeasurementQuery: The queried data (if exists) as time series.
         """
         full_query = MeasurementQueryFull(
             **query.dict(), field="pga", measurement="rt_peak_ground_motion"
         )
         return self._get_measurement(query=full_query)
 
-    def get_jma_intensity(self: Sensor, query: MeasurementQuery) -> MeasurementResult:
+    def get_jma_intensity(
+        self: CloudSensor, query: MeasurementQuery
+    ) -> MeasurementResult:
         """Get the JMA Intensity measurement of the sensor.
 
         Args:
             query: The query parameters like time frame and aggregator.
 
         Returns:
             MeasurementQuery: The queried data (if exists) as time series.
         """
         full_query = MeasurementQueryFull(
             **query.dict(), field="intensity", measurement="rt_jma_intensity"
         )
         return self._get_measurement(query=full_query)
 
-    def get_rms_amplitude(self: Sensor, query: MeasurementQuery) -> MeasurementResult:
+    def get_rms_amplitude(
+        self: CloudSensor, query: MeasurementQuery
+    ) -> MeasurementResult:
         """Get the RMS Amplitude measurement of the sensor.
 
         Args:
             query: The query parameters like time frame and aggregator.
 
         Returns:
             MeasurementQuery: The queried data (if exists) as time series.
         """
         full_query = MeasurementQueryFull(
             **query.dict(), field="rms_amplitude", measurement="rms_amplitude"
         )
         return self._get_measurement(query=full_query)
 
     def get_spectral_intensity(
-        self: Sensor, query: MeasurementQuery
+        self: CloudSensor, query: MeasurementQuery
     ) -> MeasurementResult:
         """Get the Spectral Intensity measurement of the sensor.
 
         Args:
             query: The query parameters like time frame and aggregator.
 
         Returns:
@@ -199,68 +209,70 @@
         full_query = MeasurementQueryFull(
             **query.dict(),
             field="spectral_intensity",
             measurement="rt_spectral_intensity",
         )
         return self._get_measurement(query=full_query)
 
-    def get_rms_offset(self: Sensor, query: MeasurementQuery) -> MeasurementResult:
+    def get_rms_offset(self: CloudSensor, query: MeasurementQuery) -> MeasurementResult:
         """Get the RMS Offset measurement of the sensor.
 
         Args:
             query: The query parameters like time frame and aggregator.
 
         Returns:
             MeasurementQuery: The queried data (if exists) as time series.
         """
         full_query = MeasurementQueryFull(
             **query.dict(), field="rms_offset", measurement="chrony"
         )
         return self._get_measurement(query=full_query)
 
     def get_waveform_data(
-        self: Sensor,
+        self: CloudSensor,
         start_time: datetime,
         end_time: datetime,
         location_to_store: Path | str = None,
     ) -> Path | None:
         """Request FDSN waveform dat of the sensor."""
-        logging.debug("QSClient requesting waveform data for sensor %s.", self.uid)
+        logging.debug("QSCloudClient requesting waveform data for sensor %s.", self.uid)
 
         location_to_store = assure_output_path(location_to_store)
 
         params = {"starttime": start_time, "endtime": end_time, "sensor_uids": self.uid}
         response = requests.get(
             url=f"{self._fdsn_base_url}/dataselect/1/queryauth_jwt_by_id",
             headers=self._headers,
             params=params,
         )
 
         if response.status_code != 200:
             raise CorruptedDataError(response.text)
 
-        filename = response.headers["Content-Disposition"].split("=")[1]
+        filename = response.headers.get(
+            "Content-Disposition", "filename=qsdata.mseed"
+        ).split("=")[1]
         storage_path = location_to_store / filename
         with open(storage_path, "wb") as file:
             file.write(response.content)
         return storage_path
 
     def get_stationxml(
-        self: Sensor,
+        self: CloudSensor,
         start_time: datetime,
         end_time: datetime,
         minlatitude: float = -90,
         maxlatitude: float = 90,
         minlongitude: float = -180,
         maxlongitude: float = 180,
         level: StationDetailLevel = "station",
         location_to_store: Path | str = None,
     ) -> Path:
         """Request FDSN StationXML metadata of the sensor."""
-        logging.debug("QSClient requesting stationxml for sensor %s.", self.uid)
+        logging.debug("QSCloudClient requesting stationxml for sensor %s.", self.uid)
 
         location_to_store = assure_output_path(location_to_store)
 
         params = {
             "starttime": start_time,
             "endtime": end_time,
             "sensor_uids": self.uid,
```

### Comparing `quakesaver_client-1.1.1/quakesaver_client/models/sensor_state.py` & `quakesaver_client-1.2.0/quakesaver_client/models/sensor_state.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.1/quakesaver_client/models/warnings.py` & `quakesaver_client-1.2.0/quakesaver_client/models/warnings.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.1/quakesaver_client/util.py` & `quakesaver_client-1.2.0/quakesaver_client/util.py`

 * *Files identical despite different names*

### Comparing `quakesaver_client-1.1.1/PKG-INFO` & `quakesaver_client-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: quakesaver-client
-Version: 1.1.1
+Version: 1.2.0
 Summary: Client library for interacting with the QuakeSaver sensor fleet.
 Home-page: https://quakesaver.net/
 License: BSD-3-Clause
 Author: QuakeSaver
 Author-email: info@quakesaver.net
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: pydantic (>=1.10.5,<1.11.0)
 Requires-Dist: requests (>=2.28.2,<2.29.0)
 Project-URL: Documentation, https://quakesaver.github.io/quakesaver-client/
 Project-URL: Repository, https://github.com/QuakeSaver/quakesaver-client
 Description-Content-Type: text/markdown
 
 # QuakeSaver Client
@@ -32,23 +33,23 @@
 ## Getting Started
 
 ### Setting up the client
 
 `EMAIL` and `PASSWORD` correspond to the credentials you use to log in at [https://network.quakesaver.net](https://network.quakesaver.net).
 
 ```python
-from quakesaver_client import QSClient
+from quakesaver_client import QSCloudClient
 
 EMAIL = "user@yourorganisation.net"
 PASSWORD = "!verstrongpassword1"
 
-client = QSClient(email=EMAIL, password=PASSWORD)
+client = QSCloudClient(email=EMAIL, password=PASSWORD)
 ```
 
-### Full example script
+### Example to stream from the cloud
 
 Authenticate against the quakesaver server and download raw, as well as processed data.
 
 Please note, that for security reasons each login session is only valid for 15 minutes. Thus, the client is not designed for long-term connections but for repeated queries.
 
 ```python
 """Example script for quakesaver_client usage."""
@@ -56,23 +57,23 @@
 import sys
 from datetime import datetime, timedelta
 from pprint import pp
 
 import obspy
 from obspy import Stream
 
-from quakesaver_client import QSClient
+from quakesaver_client import QSCloudClient
 from quakesaver_client.models.data_product_query import DataProductQuery
 from quakesaver_client.models.measurement import MeasurementQuery
 
 EMAIL = "user@yourorganisation.net"
 PASSWORD = "!verstrongpassword1"
 DATA_PATH = "./data"
 
-client = QSClient(email=EMAIL, password=PASSWORD)
+client = QSCloudClient(email=EMAIL, password=PASSWORD)
 
 # Get a list of all available sensor IDs:
 sensor_ids = client.get_sensor_ids()
 pp(sensor_ids)
 
 if len(sensor_ids) == 0:
     print("No sensors available")
@@ -148,7 +149,47 @@
 
 # Read the file into obspy for further processing...
 stream: Stream = obspy.read(file_path)
 for trace in stream.traces:
     print(trace.stats)
 ```
 
+## `QSLocalClient` Examples
+
+Interact with sensors on your local network using the `QSLocalClient`.
+
+### Streaming Data
+
+```python
+import asyncio
+from quakesaver_client import QSLocalClient
+
+
+async def run():
+    client = QSLocalClient()
+
+    sensor = client.get_sensor("qssensor.local")
+    stream = sensor.get_waveform_stream()
+    async for chunk in stream.start():
+        print(chunk)
+
+
+asyncio.run(run())
+```
+
+### Downloading Data
+
+Download the latest 10 minutes from a local sensor and write that into a file:
+
+```python
+import datetime
+from quakesaver_client import QSLocalClient
+
+client = QSLocalClient()
+sensor = client.get_sensor("qssensor.local")
+
+tmax = datetime.datetime.utcnow()
+tmin = tmax - datetime.timedelta(minutes=10)
+file_path = sensor.get_waveform_data(tmin, tmax)
+print(file_path)
+```
+
```

#### html2text {}

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 2.1 Name: quakesaver-client Version: 1.1.1 Summary: Client
+Metadata-Version: 2.1 Name: quakesaver-client Version: 1.2.0 Summary: Client
 library for interacting with the QuakeSaver sensor fleet. Home-page: https://
 quakesaver.net/ License: BSD-3-Clause Author: QuakeSaver Author-email:
 info@quakesaver.net Requires-Python: >=3.9,<3.12 Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10.5,<1.11.0) Requires-Dist: requests
-(>=2.28.2,<2.29.0) Project-URL: Documentation, https://quakesaver.github.io/
-quakesaver-client/ Project-URL: Repository, https://github.com/QuakeSaver/
-quakesaver-client Description-Content-Type: text/markdown # QuakeSaver Client
-[![PyPI](https://img.shields.io/pypi/v/quakesaver-client)](https://pypi.org/
-project/quakesaver-client) ![PyPI - Python Version](https://img.shields.io/
-pypi/pyversions/quakesaver-client) [![Test](https://github.com/QuakeSaver/
-quakesaver-client/actions/workflows/test.yml/badge.svg)](https://github.com/
-QuakeSaver/quakesaver-client/actions/workflows/test.yml) [Code_style:_black]
-This is the client for the [QuakeSaver](https://quakesaver.net/) Sensor
-services. You can find the documentation [here](https://quakesaver.github.io/
-quakesaver-client/). ## Getting Started ### Setting up the client `EMAIL` and
-`PASSWORD` correspond to the credentials you use to log in at [https://
-network.quakesaver.net](https://network.quakesaver.net). ```python from
-quakesaver_client import QSClient EMAIL = "user@yourorganisation.net" PASSWORD
-= "!verstrongpassword1" client = QSClient(email=EMAIL, password=PASSWORD) ```
-### Full example script Authenticate against the quakesaver server and download
-raw, as well as processed data. Please note, that for security reasons each
-login session is only valid for 15 minutes. Thus, the client is not designed
-for long-term connections but for repeated queries. ```python """Example script
-for quakesaver_client usage.""" import sys from datetime import datetime,
-timedelta from pprint import pp import obspy from obspy import Stream from
-quakesaver_client import QSClient from
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: pydantic
+(>=1.10.5,<1.11.0) Requires-Dist: requests (>=2.28.2,<2.29.0) Project-URL:
+Documentation, https://quakesaver.github.io/quakesaver-client/ Project-URL:
+Repository, https://github.com/QuakeSaver/quakesaver-client Description-
+Content-Type: text/markdown # QuakeSaver Client [![PyPI](https://
+img.shields.io/pypi/v/quakesaver-client)](https://pypi.org/project/quakesaver-
+client) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
+quakesaver-client) [![Test](https://github.com/QuakeSaver/quakesaver-client/
+actions/workflows/test.yml/badge.svg)](https://github.com/QuakeSaver/
+quakesaver-client/actions/workflows/test.yml) [Code_style:_black] This is the
+client for the [QuakeSaver](https://quakesaver.net/) Sensor services. You can
+find the documentation [here](https://quakesaver.github.io/quakesaver-client/).
+## Getting Started ### Setting up the client `EMAIL` and `PASSWORD` correspond
+to the credentials you use to log in at [https://network.quakesaver.net](https:
+//network.quakesaver.net). ```python from quakesaver_client import
+QSCloudClient EMAIL = "user@yourorganisation.net" PASSWORD =
+"!verstrongpassword1" client = QSCloudClient(email=EMAIL, password=PASSWORD)
+``` ### Example to stream from the cloud Authenticate against the quakesaver
+server and download raw, as well as processed data. Please note, that for
+security reasons each login session is only valid for 15 minutes. Thus, the
+client is not designed for long-term connections but for repeated queries.
+```python """Example script for quakesaver_client usage.""" import sys from
+datetime import datetime, timedelta from pprint import pp import obspy from
+obspy import Stream from quakesaver_client import QSCloudClient from
 quakesaver_client.models.data_product_query import DataProductQuery from
 quakesaver_client.models.measurement import MeasurementQuery EMAIL =
 "user@yourorganisation.net" PASSWORD = "!verstrongpassword1" DATA_PATH = "./
-data" client = QSClient(email=EMAIL, password=PASSWORD) # Get a list of all
-available sensor IDs: sensor_ids = client.get_sensor_ids() pp(sensor_ids) if
-len(sensor_ids) == 0: print("No sensors available") sys.exit() # For
+data" client = QSCloudClient(email=EMAIL, password=PASSWORD) # Get a list of
+all available sensor IDs: sensor_ids = client.get_sensor_ids() pp(sensor_ids)
+if len(sensor_ids) == 0: print("No sensors available") sys.exit() # For
 demonstration, we use the first sensor in the list sensor_uid_to_get =
 sensor_ids[0] # Get the sensor from the client sensor = client.get_sensor
 (sensor_uid_to_get) pp(sensor.dict()) # Queries such as waveforms, station
 metadata and measurements (data products calculated # on the sensor) # require
 that you select a time window. We use that last 5 hours of data end_time =
 datetime.utcnow() start_time = end_time - timedelta(hours=5) # Query various
 Measurements. In this case we calculate a rolling `mean` over 10 minutes # time
@@ -58,8 +59,18 @@
 = sensor.get_stationxml( starttime=start_time, endtime=end_time,
 level="response", location_to_store=DATA_PATH, ) with open(file_path, "r") as
 file: print(file.read()) # Download raw full waveforms from the sensor. Note
 that you can only query what is in # the sensor's ringbuffer (usually the last
 ~ 48 hours). file_path = sensor.get_waveform_data( start_time=start_time,
 end_time=end_time, location_to_store=DATA_PATH ) # Read the file into obspy for
 further processing... stream: Stream = obspy.read(file_path) for trace in
-stream.traces: print(trace.stats) ```
+stream.traces: print(trace.stats) ``` ## `QSLocalClient` Examples Interact with
+sensors on your local network using the `QSLocalClient`. ### Streaming Data
+```python import asyncio from quakesaver_client import QSLocalClient async def
+run(): client = QSLocalClient() sensor = client.get_sensor("qssensor.local")
+stream = sensor.get_waveform_stream() async for chunk in stream.start(): print
+(chunk) asyncio.run(run()) ``` ### Downloading Data Download the latest 10
+minutes from a local sensor and write that into a file: ```python import
+datetime from quakesaver_client import QSLocalClient client = QSLocalClient()
+sensor = client.get_sensor("qssensor.local") tmax = datetime.datetime.utcnow()
+tmin = tmax - datetime.timedelta(minutes=10) file_path =
+sensor.get_waveform_data(tmin, tmax) print(file_path) ```
```

