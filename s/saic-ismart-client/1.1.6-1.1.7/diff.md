# Comparing `tmp/saic_ismart_client-1.1.6.tar.gz` & `tmp/saic_ismart_client-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.1.6.tar", last modified: Tue Apr 25 08:06:03 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.1.7.tar", last modified: Tue May  2 17:21:11 2023, max compression
```

## Comparing `saic_ismart_client-1.1.6.tar` & `saic_ismart_client-1.1.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.350740 saic_ismart_client-1.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.350740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_ws_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.439565 saic_ismart_client-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:21:11.439565 saic_ismart_client-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.431565 saic_ismart_client-1.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.431565 saic_ismart_client-1.1.7/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.431565 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-02 17:21:11.000000 saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-02 17:21:11.000000 saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:21:11.000000 saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 17:21:11.000000 saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 17:21:11.000000 saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:21:11.435565 saic_ismart_client-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-05-02 17:21:00.000000 saic_ismart_client-1.1.7/tests/test_ws_api.py
```

### Comparing `saic_ismart_client-1.1.6/LICENSE` & `saic_ismart_client-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/PKG-INFO` & `saic_ismart_client-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.1.6
+Version: 1.1.7
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.1.6/README.md` & `saic_ismart_client-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/pyproject.toml` & `saic_ismart_client-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.1.7/src/saic_ismart_client/saic_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import logging
 import time
 import urllib.parse
 from typing import cast
 
 import requests as requests
 
-from saic_ismart_client.common_model import MessageV2, MessageBodyV2, Header
+from saic_ismart_client.common_model import MessageV2, MessageBodyV2, Header, AbstractMessageBody
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
 from saic_ismart_client.ota_v1_1.data_model import VinInfo, MpUserLoggingInReq, MpUserLoggingInRsp, AlarmSwitchReq, \
     MpAlarmSettingType, AlarmSwitch, MessageBodyV11, MessageV11, MessageListReq, StartEndNumber, MessageListResp, \
     Timestamp, Message, AbortSendMessageReq
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
 from saic_ismart_client.ota_v2_1.data_model import OtaRvmVehicleStatusReq, OtaRvmVehicleStatusResp25857, OtaRvcReq,\
     RvcReqParam
 from saic_ismart_client.ota_v3_0.Message import MessageCoderV30, MessageV30, MessageBodyV30
 from saic_ismart_client.ota_v3_0.data_model import OtaChrgMangDataResp
 
 UID_INIT = '0000000000000000000000000000000000000000000000000#'
+AVG_SMS_DELIVERY_TIME = 15
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.INFO)
 
 
 class SaicMessage:
     def __init__(self, message_id: int, message_type: str, title: str, message_time: datetime, sender: str,
                  content: str, read_status: int, vin: str):
         self.message_id = message_id
@@ -236,15 +237,16 @@
     def send_vehicle_ctrl_cmd_with_retry(self, vin_info: VinInfo, rvc_req_type: bytes, rvc_params: list) -> None:
         vehicle_control_cmd_rsp_msg = self.send_vehicle_control_command(vin_info, rvc_req_type, rvc_params)
         retry = 1
         while (
                 vehicle_control_cmd_rsp_msg.body.error_message is not None
                 and retry < 3
         ):
-            time.sleep(float(2))
+            self.handle_error(vehicle_control_cmd_rsp_msg.body)
+
             event_id = vehicle_control_cmd_rsp_msg.body.event_id
             vehicle_control_cmd_rsp_msg = self.send_vehicle_control_command(vin_info, rvc_req_type, rvc_params,
                                                                             event_id)
             retry += 1
 
         if vehicle_control_cmd_rsp_msg.body.error_message is not None:
             raise SaicApiException(vehicle_control_cmd_rsp_msg.body.error_message.decode(),
@@ -255,15 +257,15 @@
 
         retry = 0
         while (
                 message_list_rsp_msg.application_data is None
                 and retry < 3
         ):
             if message_list_rsp_msg.body.error_message is not None:
-                logging.error(message_list_rsp_msg.body.error_message.decode())
+                self.handle_error(message_list_rsp_msg.body)
             else:
                 waiting_time = retry * 60
                 logging.debug(
                     f'Update message list request returned no application data. Waiting {waiting_time} seconds')
                 time.sleep(float(waiting_time))
                 retry += 1
 
@@ -431,14 +433,31 @@
     def get_token(self):
         if self.token_expiration is not None:
             token_expiration = cast(Timestamp, self.token_expiration)
             if token_expiration.get_timestamp() < datetime.datetime.now():
                 self.login()
         return self.token
 
+    def handle_error(self, message_body: AbstractMessageBody):
+        message = f'application ID: {message_body.application_id},'\
+              + f' protocol version: {message_body.application_data_protocol_version},'\
+              + f' message: {message_body.error_message.decode()}'\
+              + f' result code: {message_body.result}'
+
+        if message_body.result == 2:
+            # re-login
+            logging.debug(message)
+            self.login()
+        elif message_body.result == 4:
+            # please try again later
+            logging.debug(message)
+            time.sleep(float(AVG_SMS_DELIVERY_TIME))
+        else:
+            logging.error(message)
+
 
 def hash_md5(password: str) -> str:
     return hashlib.md5(password.encode('utf-8')).hexdigest()
 
 
 def create_alarm_switch(alarm_setting_type: MpAlarmSettingType) -> AlarmSwitch:
     alarm_switch = AlarmSwitch()
```

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.1.6
+Version: 1.1.7
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.1.7/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/tests/test_Message_v1_1.py` & `saic_ismart_client-1.1.7/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/tests/test_Message_v2_1.py` & `saic_ismart_client-1.1.7/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/tests/test_Message_v3_0.py` & `saic_ismart_client-1.1.7/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/tests/test_abrp_api.py` & `saic_ismart_client-1.1.7/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.6/tests/test_ws_api.py` & `saic_ismart_client-1.1.7/tests/test_ws_api.py`

 * *Files identical despite different names*

