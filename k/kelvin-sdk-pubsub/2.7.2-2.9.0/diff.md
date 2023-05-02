# Comparing `tmp/kelvin_sdk_pubsub-2.7.2-py3-none-any.whl.zip` & `tmp/kelvin_sdk_pubsub-2.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 15827 bytes, number of entries: 14
--rw-r--r--  2.0 unx      473 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/__init__.py
--rw-r--r--  2.0 unx     1946 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/client.py
--rw-r--r--  2.0 unx    19008 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/config.py
--rw-r--r--  2.0 unx    17914 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/connection.py
--rw-r--r--  2.0 unx      149 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/error.py
--rw-r--r--  2.0 unx     1988 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/prometheus.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/py.typed
--rw-r--r--  2.0 unx     5388 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/types.py
--rw-r--r--  2.0 unx      740 b- defN 23-Mar-13 16:37 kelvin/sdk/pubsub/utils.py
--rw-r--r--  2.0 unx      160 b- defN 23-Mar-13 16:44 kelvin/sdk/pubsub/version.py
--rw-r--r--  2.0 unx     3046 b- defN 23-Mar-13 16:44 kelvin_sdk_pubsub-2.7.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-13 16:44 kelvin_sdk_pubsub-2.7.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-13 16:44 kelvin_sdk_pubsub-2.7.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1179 b- defN 23-Mar-13 16:44 kelvin_sdk_pubsub-2.7.2.dist-info/RECORD
-14 files, 52090 bytes uncompressed, 13851 bytes compressed:  73.4%
+Zip file size: 15530 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      473 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/__init__.py
+-rw-r--r--  2.0 unx     1946 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/client.py
+-rw-r--r--  2.0 unx    18934 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/config.py
+-rw-r--r--  2.0 unx    17751 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/connection.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/error.py
+-rw-r--r--  2.0 unx     1988 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/prometheus.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/py.typed
+-rw-r--r--  2.0 unx     4578 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/types.py
+-rw-r--r--  2.0 unx      740 b- defN 23-Feb-17 16:01 kelvin/sdk/pubsub/utils.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Feb-17 16:08 kelvin/sdk/pubsub/version.py
+-rw-r--r--  2.0 unx     3046 b- defN 23-Feb-17 16:08 kelvin_sdk_pubsub-2.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-17 16:08 kelvin_sdk_pubsub-2.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Feb-17 16:08 kelvin_sdk_pubsub-2.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1179 b- defN 23-Feb-17 16:08 kelvin_sdk_pubsub-2.9.0.dist-info/RECORD
+14 files, 51043 bytes uncompressed, 13554 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: kelvin/sdk/pubsub/utils.py
 Comment: 
 
 Filename: kelvin/sdk/pubsub/version.py
 Comment: 
 
-Filename: kelvin_sdk_pubsub-2.7.2.dist-info/METADATA
+Filename: kelvin_sdk_pubsub-2.9.0.dist-info/METADATA
 Comment: 
 
-Filename: kelvin_sdk_pubsub-2.7.2.dist-info/WHEEL
+Filename: kelvin_sdk_pubsub-2.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: kelvin_sdk_pubsub-2.7.2.dist-info/top_level.txt
+Filename: kelvin_sdk_pubsub-2.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: kelvin_sdk_pubsub-2.7.2.dist-info/RECORD
+Filename: kelvin_sdk_pubsub-2.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kelvin/sdk/pubsub/config.py

```diff
@@ -295,17 +295,17 @@
             raise ValueError("Missing app type") from None
         if not isinstance(app_type, str):
             raise TypeError(f"Invalid app type {type(app_type).__name__!r}") from None
 
         app_config = deep_get(root_config, f"app.{app_type}", {})
 
         if app_type == "kelvin":
-            if "global" not in values and "global" in app_config:
-                defaults = app_config["global"] or {}
-                values["metric_defaults"] = {k: v for k, v in defaults.items() if k in SELECTORS}
+            values["metric_defaults"] = {
+                "asset_names": [asset["name"] for asset in app_config.get("assets", {})]
+            }
 
             for name in IO_FIELDS:
                 if name not in values and name in app_config:
                     keys = ["name", "data_type", "control_change", IO_FIELDS[name]]
                     default_opts: Dict[str, Any] = {}
                     if name == "outputs":
                         keys += ["storage", "retain"]
@@ -530,15 +530,14 @@
         """Input topics."""
 
         return sorted({topic for x in self.input_map.values() for topic, *_ in x})
 
     @cached_property
     def output_map(self) -> Dict[Selector, List[Tuple[str, str, str, bool, bool]]]:
         """Output map."""
-
         result: DefaultDict[Selector, Set[Tuple[str, str, str, bool, bool]]] = defaultdict(set)
 
         source = (self.node_name, self.workload_name)
 
         for io in self.outputs:
             for selector in io.combinations:
                 node_name, workload_name, asset_name, name = self._expand_selector(selector)
```

## kelvin/sdk/pubsub/connection.py

```diff
@@ -64,17 +64,14 @@
 
     _input_count: int = 0
     _output_count: int = 0
     _connect_count: int = 0
 
     config: PubSubClientConfig
 
-    min_interval: float = 1.0
-    max_interval: float = 32.0
-
     def __init__(self, config: PubSubClientConfig) -> None:
         """Initialise the connection."""
 
         self.config = config
         self.prometheus_client = AssetMetricHeartbeat(workload=self.config.workload_name)
 
     @property
@@ -242,15 +239,15 @@
     def __init__(self, config: PubSubClientConfig) -> None:
         """Initialise the connection."""
 
         super().__init__(config)
 
         self._queue = Queue(maxsize=self.config.max_items)
 
-    def connect(self, max_attempts: Optional[int] = None) -> None:
+    def connect(self) -> None:
         """Open connection."""
 
         self._input_count = self._output_count = 0
 
         client = self._client
         if client is not None:
             try:
@@ -259,17 +256,14 @@
                 pass
 
         config = self.config
         client = self._client = config.broker_url.get_sync_client(
             config.client_id or f"pubsub-{uuid4()}",
             config.username,
             config.password,
-            max_attempts=max_attempts,
-            min_interval=self.min_interval,
-            max_interval=self.max_interval,
         )
         client.on_connect = self._on_connect
         client.on_message = self._on_message
 
         client.loop_start()
 
         if not self._connect_count:
@@ -335,15 +329,15 @@
         """Connect handler."""
 
         config = self.config
 
         topics = config.input_topics
         if topics:
             client.subscribe([(topic, config.qos) for topic in topics])
-            logger.info("Subscribed to topics", topic_sumarry=topics)
+            logger.info("Subscribed to topics", topic_summary=topics)
 
     def _on_message(self, client: Client, userdata: Any, message: MQTTMessage) -> None:
         """Message handler."""
 
         topic, payload = message.topic, message.payload
 
         try:
@@ -404,14 +398,17 @@
     """Asynchronous Pub-Sub Connection."""
 
     _client: AsyncClient
     _connecting: Lock
     _queue: AsyncQueue[MessagePayloadTuple]
     _send_task: Optional[Task] = None
 
+    min_interval: float = 1.0
+    max_interval: float = 32.0
+
     def __init__(self, config: PubSubClientConfig) -> None:
         """Initialise async connection."""
 
         super().__init__(config)
 
         config = self.config
```

## kelvin/sdk/pubsub/types.py

```diff
@@ -1,30 +1,24 @@
 """Types."""
 
 from __future__ import annotations
 
 import re
 from datetime import datetime, timedelta
 from enum import Enum, IntEnum
-from random import random
 from ssl import SSLContext
-from time import sleep
 from typing import Any, Callable, Iterator, Optional, TypeVar, Union, cast
 from urllib.parse import unquote
 
-import structlog
 from asyncio_mqtt import Client as AsyncClient
 from paho.mqtt.client import Client
 from pydantic import AnyUrl, BaseConfig, StrictStr, UrlSchemeError
-from pydantic.fields import ModelField
+from pydantic.main import ModelField
 from pydantic.tools import parse_obj_as
 
-logger = structlog.get_logger(__name__)
-
-
 TimeType = Union[int, float, datetime, timedelta]
 
 T = TypeVar("T")
 
 
 class Identifier(StrictStr):
     """Dotted-identifier name."""
@@ -69,17 +63,14 @@
         return result
 
     def get_sync_client(
         self,
         client_id: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
-        max_attempts: Optional[int] = None,
-        min_interval: float = 1.0,
-        max_interval: float = 32.0,
     ) -> Client:
         """Get synchronous client."""
 
         client = Client(client_id=client_id or "")
 
         if username is None and self.user:
             username = unquote(self.user)
@@ -88,30 +79,15 @@
 
         if username:
             client.username_pw_set(username, password)
 
         if self.scheme == "mqtts":
             client.tls_set_context()
 
-        host, port = self.host, int(cast(str, self.port))
-
-        interval, i = 0.0, 0
-        while True:
-            i += 1
-            try:
-                client.connect(host, port)
-            except Exception as e:
-                if max_attempts is not None and i >= max_attempts:
-                    raise ConnectionError(f"Unable to connect to broker: {e}")
-                logger.info("Retrying connection", interval=interval, attempt=i)
-                sleep(interval + random())  # nosec
-                interval = min(max(2.0 * interval, min_interval), max_interval)
-                continue
-            else:
-                break
+        client.connect(self.host, int(cast(str, self.port)))
 
         return client
 
     def get_async_client(
         self,
         client_id: Optional[str] = None,
         username: Optional[str] = None,
```

## kelvin/sdk/pubsub/version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '2.7.2'
-__version_tuple__ = version_tuple = (2, 7, 2)
+__version__ = version = '2.9.0'
+__version_tuple__ = version_tuple = (2, 9, 0)
```

## Comparing `kelvin_sdk_pubsub-2.7.2.dist-info/METADATA` & `kelvin_sdk_pubsub-2.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kelvin-sdk-pubsub
-Version: 2.7.2
+Version: 2.9.0
 Summary: Kelvin Pub-Sub Client
 Home-page: https://kelvininc.com/
 Author: Kelvin Inc
 Author-email: engineering@kelvininc.com
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `kelvin_sdk_pubsub-2.7.2.dist-info/RECORD` & `kelvin_sdk_pubsub-2.9.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 kelvin/sdk/pubsub/__init__.py,sha256=bh0J3qAcQVxlaLBhlZX1SH1AQx0vAuu0klD0ehVSwOM,473
 kelvin/sdk/pubsub/client.py,sha256=NJX2ru0DdL8PSfFmY9pMbHhYRrbFg63ZZLDKnuBr9-Q,1946
-kelvin/sdk/pubsub/config.py,sha256=EPbouJB_X3EYpPKnN-4dcH7hAyS6jRK2XzekQUO15uM,19008
-kelvin/sdk/pubsub/connection.py,sha256=ECsjREwg-nuke-nKZ31L5Ssog4at2OdaVwJ6TNV2LPo,17914
+kelvin/sdk/pubsub/config.py,sha256=eqPDv1Oqf66AgGsiIEfpXhKDlP07W0CZt7I8gnDSgx0,18934
+kelvin/sdk/pubsub/connection.py,sha256=6OuVbcsqcunGCdC5MCLf1Yn1KZ5F9d9KwXDfnOeiMlM,17751
 kelvin/sdk/pubsub/error.py,sha256=muFeb6nK3hm8VBjv_ErFYvRJdmJ4uNeLSYmpgSSA-IU,149
 kelvin/sdk/pubsub/prometheus.py,sha256=LbJfB6YVOrry2YwXlo9IjO8pbzGcsK873xGrBp5Id00,1988
 kelvin/sdk/pubsub/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kelvin/sdk/pubsub/types.py,sha256=rxo8O_F0kmTinscatg8VwLJrfpr2j9ODyp03_TthlRw,5388
+kelvin/sdk/pubsub/types.py,sha256=2znkQMm8TI6Tc4H7BoGBn2mmFdSK4esJC98TH-JeFds,4578
 kelvin/sdk/pubsub/utils.py,sha256=JqsTPzuAEqHZd7Y1FqUYSqMq6cvqKd67fOjlQWjTfKY,740
-kelvin/sdk/pubsub/version.py,sha256=HcPrGg1wZwagQtkv5QY0SbWMh2OAJ989PkQbXgf_B1I,160
-kelvin_sdk_pubsub-2.7.2.dist-info/METADATA,sha256=XnExfUsK7cJ-DTCTR_YGuFnvNld3TdEqqCWgsXGkacU,3046
-kelvin_sdk_pubsub-2.7.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-kelvin_sdk_pubsub-2.7.2.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
-kelvin_sdk_pubsub-2.7.2.dist-info/RECORD,,
+kelvin/sdk/pubsub/version.py,sha256=DQyUhRu_7fq06kf_Gh4HJ9ljlsH-BdBjaLFBKw7WDmg,160
+kelvin_sdk_pubsub-2.9.0.dist-info/METADATA,sha256=yJFj8O3MeN-5xOrNbcMtOCnB2EtDbVlTp5-18Jjb9dA,3046
+kelvin_sdk_pubsub-2.9.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+kelvin_sdk_pubsub-2.9.0.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
+kelvin_sdk_pubsub-2.9.0.dist-info/RECORD,,
```

