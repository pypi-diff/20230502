# Comparing `tmp/ansys-api-geometry-0.2.7.tar.gz` & `tmp/ansys-api-geometry-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-geometry-0.2.7.tar", last modified: Mon Mar 27 20:50:06 2023, max compression
+gzip compressed data, was "ansys-api-geometry-0.2.dev0.tar", last modified: Tue May  2 16:12:30 2023, max compression
```

## Comparing `ansys-api-geometry-0.2.7.tar` & `ansys-api-geometry-0.2.dev0.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:50:06.419535 ansys-api-geometry-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-27 20:50:06.419535 ansys-api-geometry-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:50:06.415535 ansys-api-geometry-0.2.7/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:50:06.415535 ansys-api-geometry-0.2.7/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:50:06.415535 ansys-api-geometry-0.2.7/ansys/api/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:50:06.419535 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/admin.proto
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/api.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/bodies.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/commands.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/components.proto
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/coordinatesystems.proto
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/curves.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/designs.proto
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/edges.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/faces.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/facettools.proto
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/geometryapi.proto
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/geometryapplication.proto
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/materials.proto
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/meshes.proto
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/models.proto
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/namedselections.proto
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/parts.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/preparetools.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/repairtools.proto
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/streaming.proto
--rw-r--r--   0 runner    (1001) docker     (123)    45437 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/ansys/api/geometry/v0/units.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:50:06.419535 ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-27 20:50:06.000000 ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-27 20:50:06.000000 ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:50:06.000000 ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-27 20:50:06.000000 ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 20:50:06.000000 ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 20:50:06.000000 ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:50:06.419535 ansys-api-geometry-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-27 20:49:53.000000 ansys-api-geometry-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.245654 ansys-api-geometry-0.2.dev0/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.245654 ansys-api-geometry-0.2.dev0/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.249654 ansys-api-geometry-0.2.dev0/ansys/api/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/admin.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/bodies.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/commands.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/components.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/coordinatesystems.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/curves.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/designs.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/edges.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/faces.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/facettools.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapi.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapplication.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/materials.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/meshes.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/models.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/namedselections.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/parts.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/preparetools.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/repairtools.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/streaming.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 16:12:30.000000 ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:12:30.253654 ansys-api-geometry-0.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-02 16:12:11.000000 ansys-api-geometry-0.2.dev0/setup.py
```

### Comparing `ansys-api-geometry-0.2.7/LICENSE` & `ansys-api-geometry-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/PKG-INFO` & `ansys-api-geometry-0.2.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-geometry
-Version: 0.2.7
-Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 20:50:06 on 27 March 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 16:12:30 on 02 May 2023
 Home-page: https://github.com/ansys/ansys-api-geometry
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-geometry-0.2.7/README.md` & `ansys-api-geometry-0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/admin.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/admin.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/api.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapi.proto`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-// ©2021, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+// ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 syntax = "proto3";
-package ansys.api.geometry.v0;
-option csharp_namespace = "Ansys.Api.Geometry.V0";
+package ansys.api.geometry.v0.GeometryApi;
+
+option csharp_namespace = "Ansys.Api.Geometry.V0.GeometryApi";
 option go_package = "ansys/api/geometry/v0";
 
 // Api
 //
-service Api{
-    // Sets the current scripting version.
-    rpc SetVersion(SetVersionRequest) returns(SetVersionResponse) ;
+service GeometryApi{
+  // Sets the current scripting version.
+  rpc SetVersion(SetVersionRequest) returns(SetVersionResponse) ;
 
-      // Sets the current scripting version.
-    rpc GetVersion(GetVersionRequest) returns(GetVersionResponse) ;
+  // Sets the current scripting version.
+  rpc GetVersion(GetVersionRequest) returns(GetVersionResponse) ;
 }
 
 message GetVersionRequest{
 }
 
 message GetVersionResponse{
-    string result = 1;
+  ApiVersion version = 1;
 }
 
 message SetVersionRequest{
-    // The set api operation being requested.
-    ApiVersion version = 1;
+  // The set api operation being requested.
+  ApiVersion version = 1;
 }
 
 message SetVersionResponse{
-    string result = 1;
+  string result = 1;
 }
 
 enum ApiVersion {
-    V_21 = 0;
-    V_22 = 1;
-    V_231 = 2;
-    V_232 = 3;
+  V_21 = 0;
+  V_22 = 1;
+  V_231 = 2;
+  V_232 = 3;
 }
```

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/bodies.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/bodies.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/commands.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/commands.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/components.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/components.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/coordinatesystems.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/coordinatesystems.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/curves.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/curves.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/designs.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/designs.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/edges.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/edges.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/faces.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/faces.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/facettools.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/facettools.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/geometryapplication.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/geometryapplication.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/models.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/models.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/namedselections.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/namedselections.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/parts.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/parts.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/preparetools.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/preparetools.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys/api/geometry/v0/repairtools.proto` & `ansys-api-geometry-0.2.dev0/ansys/api/geometry/v0/repairtools.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/PKG-INFO` & `ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-geometry
-Version: 0.2.7
-Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 20:50:06 on 27 March 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-geometry, built on 16:12:30 on 02 May 2023
 Home-page: https://github.com/ansys/ansys-api-geometry
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-geometry-0.2.7/ansys_api_geometry.egg-info/SOURCES.txt` & `ansys-api-geometry-0.2.dev0/ansys_api_geometry.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.py
 ansys/api/geometry/VERSION
 ansys/api/geometry/__init__.py
 ansys/api/geometry/py.typed
 ansys/api/geometry/v0/__init__.py
 ansys/api/geometry/v0/admin.proto
-ansys/api/geometry/v0/api.proto
 ansys/api/geometry/v0/bodies.proto
 ansys/api/geometry/v0/commands.proto
 ansys/api/geometry/v0/components.proto
 ansys/api/geometry/v0/coordinatesystems.proto
 ansys/api/geometry/v0/curves.proto
 ansys/api/geometry/v0/designs.proto
 ansys/api/geometry/v0/edges.proto
@@ -23,14 +22,13 @@
 ansys/api/geometry/v0/meshes.proto
 ansys/api/geometry/v0/models.proto
 ansys/api/geometry/v0/namedselections.proto
 ansys/api/geometry/v0/parts.proto
 ansys/api/geometry/v0/preparetools.proto
 ansys/api/geometry/v0/repairtools.proto
 ansys/api/geometry/v0/streaming.proto
-ansys/api/geometry/v0/units.proto
 ansys_api_geometry.egg-info/PKG-INFO
 ansys_api_geometry.egg-info/SOURCES.txt
 ansys_api_geometry.egg-info/dependency_links.txt
 ansys_api_geometry.egg-info/entry_points.txt
 ansys_api_geometry.egg-info/requires.txt
 ansys_api_geometry.egg-info/top_level.txt
```

### Comparing `ansys-api-geometry-0.2.7/setup.py` & `ansys-api-geometry-0.2.dev0/setup.py`

 * *Files identical despite different names*

