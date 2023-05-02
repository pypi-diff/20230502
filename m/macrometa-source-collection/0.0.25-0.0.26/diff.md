# Comparing `tmp/macrometa-source-collection-0.0.25.tar.gz` & `tmp/macrometa-source-collection-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.25.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.26.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.25.tar` & `macrometa-source-collection-0.0.26.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8346 2023-04-27 08:54:31.255945 macrometa-source-collection-0.0.25/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     7366 2023-04-27 08:54:31.255945 macrometa-source-collection-0.0.25/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-04-27 08:54:31.595942 macrometa-source-collection-0.0.25/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.25/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0     8346 2023-05-02 07:14:48.605730 macrometa-source-collection-0.0.26/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     7978 2023-05-02 07:14:48.605730 macrometa-source-collection-0.0.26/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-05-02 07:14:48.877739 macrometa-source-collection-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.26/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.26/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.25/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.26/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.25/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.26/macrometa_source_collection/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 from datetime import datetime
 from prometheus_client import start_http_server, Counter, Histogram
 from singer import utils
 from singer.catalog import CatalogEntry
 
 LOGGER = singer.get_logger('macrometa_source_collection')
 
+region_label = os.getenv("GDN_FEDERATION", "NA")
+tenant_label = os.getenv("GDN_TENANT", "NA")
+fabric_label = os.getenv("GDN_FABRIC", "NA")
+workflow_label = os.getenv("WORKFLOW_UUID", "NA")
+metric_service_url = os.getenv("METRIC_SERVICE_API")
+
 class GDNCollectionClient:
     """Client for handling GDN collection streams."""
 
     def __init__(self, config) -> None:
         """Init new GDN Collection Client."""
         self._host = config.get("region")
         self._fabric = config.get("fabric")
@@ -34,20 +40,20 @@
         )
         self._auth = pulsar.AuthenticationToken(_apikey)
         self._tenant = self._c8_client.tenant(apikey=_apikey).tenant_name
 
         # enable collection stream on the source collection.
         self._c8_client.update_collection_properties(self._collection, has_stream=True)
 
-        self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections")
-        self.exported_documents = Counter("exported_documents", "Total number of documents exported from GDN collections")
-        self.export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections")
-        self.export_lag = Histogram("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources")
-        self.io_compute_time_ms = Histogram("io_compute_time_ms", "Time between the moment the first byte is replicated to the last byte")
-
+        self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
+        self.exported_documents = Counter("exported_documents", "Total number of documents exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
+        self.export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
+        self.export_lag = Histogram("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources", ['region', 'tenant', 'fabric', 'workflow'])
+        
+        # Start the Prometheus HTTP server for exposing metrics
         start_http_server(8000)
 
     def sync(self, stream):
         """Return documents in target GDN collection as records."""
         if self._c8_client.has_collection(self._collection):
             self.send_schema_message(stream)
             columns = list(stream.schema.properties.keys())
@@ -94,24 +100,24 @@
                             singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                             singer.write_message(singer_record)
                     elif props["op"] == "DELETE":
                         # Currently, we don't have a way to validate schema here
                         j['_sdc_deleted_at'] = singer.utils.strftime(utils.now())
                         singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                         singer.write_message(singer_record)
-                    self.exported_bytes.inc(len(data))
-                    self.exported_documents.inc()
+                    self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(data))
+                    self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     time = datetime.fromtimestamp(msg.publish_timestamp()/1000)
                     time_str = time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
                     event_time = datetime.strptime(time_str, "%Y-%m-%dT%H:%M:%S.%fZ")
-                    self.export_lag.observe((utils.now() - event_time).total_seconds())
+                    self.export_lag.labels(region_label, tenant_label, fabric_label, workflow_label).observe((utils.now() - event_time).total_seconds())
                     _consumer.acknowledge(msg.message_id())
                 except Exception as e:
                     LOGGER.warn(f"Exception received: {e}")
-                    self.export_errors.inc()
+                    self.export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
 
     def load_existing_data(self, stream, columns, schema_properties):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
```

### Comparing `macrometa-source-collection-0.0.25/pyproject.toml` & `macrometa-source-collection-0.0.26/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.25'
+version='0.0.26'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.25/setup.py` & `macrometa-source-collection-0.0.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.25',
+    'version': '0.0.26',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.25/PKG-INFO` & `macrometa-source-collection-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.25
+Version: 0.0.26
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

