# Comparing `tmp/dynatrace_opentelemetry_core-1.261.5-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_core-1.263.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 397161 bytes, number of entries: 126
+Zip file size: 397160 bytes, number of entries: 126
 -rw-r--r--  2.0 unx     1706 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/__init__.py
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/_version.py
 -rw-r--r--  2.0 unx     1449 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/any_pb2.py
 -rw-r--r--  2.0 unx     2857 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/api_pb2.py
 -rw-r--r--  2.0 unx    46761 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor.py
 -rw-r--r--  2.0 unx     6819 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor_database.py
 -rw-r--r--  2.0 unx   116074 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor_pb2.py
@@ -117,12 +117,12 @@
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/__init__.py
 -rw-r--r--  2.0 unx     3559 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/byteops.py
 -rw-r--r--  2.0 unx     2035 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/context.py
 -rw-r--r--  2.0 unx     6002 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/exceptions.py
 -rw-r--r--  2.0 unx     3287 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/hashes.py
 -rw-r--r--  2.0 unx     3307 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/meta.py
 -rw-r--r--  2.0 unx     1626 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/tenant.py
-?rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.261.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.261.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.261.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx    13788 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.261.5.dist-info/RECORD
-126 files, 1643863 bytes uncompressed, 374225 bytes compressed:  77.2%
+?rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.263.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.263.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.263.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx    13788 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.263.2.dist-info/RECORD
+126 files, 1643863 bytes uncompressed, 374224 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -360,20 +360,20 @@
 
 Filename: dynatrace/opentelemetry/tracing/_util/meta.py
 Comment: 
 
 Filename: dynatrace/opentelemetry/tracing/_util/tenant.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.261.5.dist-info/METADATA
+Filename: dynatrace_opentelemetry_core-1.263.2.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.261.5.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_core-1.263.2.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.261.5.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_core-1.263.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.261.5.dist-info/RECORD
+Filename: dynatrace_opentelemetry_core-1.263.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/tracing/version.py

```diff
@@ -1,7 +1,7 @@
-__version__ = "1.261.5"
+__version__ = "1.263.2"
 
-FULL_VERSION = "1.261.5.20230309-143152"
-BUILD_DATE = "2023.03.09 14:31:52"
-SCM_REVISION = "6357fd73764eb86cb7253b777e8a3a9710a52c98"
+FULL_VERSION = "1.263.2.20230310-042307"
+BUILD_DATE = "2023.03.10 04:23:07"
+SCM_REVISION = "0c555345a3ba0da379df5f05ee0f8d0ff85ddaf8"
 IS_DEV_VERSION = False
 IS_PACKAGE_MODE = True
```

## Comparing `dynatrace_opentelemetry_core-1.261.5.dist-info/METADATA` & `dynatrace_opentelemetry_core-1.263.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynatrace-opentelemetry-core
-Version: 1.261.5
+Version: 1.263.2
 Summary: Dynatrace OpenTelemetry core package
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `dynatrace_opentelemetry_core-1.261.5.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_core-1.263.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dynatrace_opentelemetry_core-1.261.5.dist-info/RECORD` & `dynatrace_opentelemetry_core-1.263.2.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 dynatrace/odin/proto/trace/v1/trace_pb2.py,sha256=6qFXDDS5U9_tshiqUjk0FTWHxMl9WOxcgE2yK6w10Aw,5585
 dynatrace/odin/semconv/_version.py,sha256=rvjjo5RBC86V0X6_1Q4um7329CS2s96rCFsLW9nfU7Q,39
 dynatrace/odin/semconv/v1/__init__.py,sha256=hWRbd7IEJZsM6Snn0kY4M10fb2IPwHY6DHjwDXJMpco,61795
 dynatrace/opentelemetry/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/api.py,sha256=c7Rb1TkphWCUqKerxW5E310Smvj-VBqIfJsJlu5VEtk,1012
 dynatrace/opentelemetry/tracing/api.pyi,sha256=QkVFJRNMk2p5loY3VO5rCFHQxz8MacstxiWQzKY2DfY,1678
 dynatrace/opentelemetry/tracing/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dynatrace/opentelemetry/tracing/version.py,sha256=tD1NaeGqYL-QJAZCkmLOPI1Fxs1IwgbJ_zko0zmSdZA,205
+dynatrace/opentelemetry/tracing/version.py,sha256=t9VegHzrAaXAs-27Q2ZfLNP2yXY2Yx4PV-Y3kSnDeJM,205
 dynatrace/opentelemetry/tracing/_config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_config/banner.py,sha256=HKXTTNkvvSy8j1Kwik_9kbjqve9RaivwNNSfbnn4H2U,3752
 dynatrace/opentelemetry/tracing/_config/configure.py,sha256=zC2p9ba7isZh-aOnfwd0Y9Fx5k2Njx0iagSzqt9ncgU,1780
 dynatrace/opentelemetry/tracing/_config/reader.py,sha256=52wMwG_9MbS97y0H4OeG4d7uWgBfyEfB6o4AkraVGKE,10949
 dynatrace/opentelemetry/tracing/_config/settings.py,sha256=SUiUyRfz5YJ0g3OBX51GAxjjprB5XPd3ISfzN1FUs68,18329
 dynatrace/opentelemetry/tracing/_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_export/exporter.py,sha256=PVj1EG2i_BUvyfcH_1KexngKSlP6qc3nz-_mnDtlH0Y,13769
@@ -116,11 +116,11 @@
 dynatrace/opentelemetry/tracing/_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_util/byteops.py,sha256=d9NPDsMmu338laXMgDjX4EIooSeEvgXkdneQLm9-Qhs,3559
 dynatrace/opentelemetry/tracing/_util/context.py,sha256=1QZpjw33kLAaSYT1CjlKuP-moRWGvCrC47O-ZtbTEYo,2035
 dynatrace/opentelemetry/tracing/_util/exceptions.py,sha256=XLYTvsqoNfhHeHheSFTizqQKaltYDqCuseGITDXz-aA,6002
 dynatrace/opentelemetry/tracing/_util/hashes.py,sha256=Ea7W7XVS1iOdp85qlaqK9ue3YLSJJvErkb4Ja646sqc,3287
 dynatrace/opentelemetry/tracing/_util/meta.py,sha256=BkkQp6X6JgkH6beoUJqSfNovZd3LAT8FGKo7s8mAjOA,3307
 dynatrace/opentelemetry/tracing/_util/tenant.py,sha256=tIuLrPLpD3rhcBzv3i7inj4LIP6mgeRWY72DLL_DKvU,1626
-dynatrace_opentelemetry_core-1.261.5.dist-info/METADATA,sha256=DMpMNHxEJQAfwfvQhLtWWrXGDWuidGSqg4cHPCrl80U,1153
-dynatrace_opentelemetry_core-1.261.5.dist-info/WHEEL,sha256=Fd6mP6ydyRguakwUJ05oBE7fh2IPxgtDN9IwHJ9OqJQ,87
-dynatrace_opentelemetry_core-1.261.5.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
-dynatrace_opentelemetry_core-1.261.5.dist-info/RECORD,,
+dynatrace_opentelemetry_core-1.263.2.dist-info/METADATA,sha256=nuKlrIxrG5sZuwYUcioy-20kHneh4S5mE88dVQUH5lg,1153
+dynatrace_opentelemetry_core-1.263.2.dist-info/WHEEL,sha256=Fd6mP6ydyRguakwUJ05oBE7fh2IPxgtDN9IwHJ9OqJQ,87
+dynatrace_opentelemetry_core-1.263.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
+dynatrace_opentelemetry_core-1.263.2.dist-info/RECORD,,
```

