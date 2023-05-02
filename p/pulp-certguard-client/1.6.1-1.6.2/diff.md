# Comparing `tmp/pulp_certguard-client-1.6.1.tar.gz` & `tmp/pulp_certguard-client-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_certguard-client-1.6.1.tar", last modified: Thu Mar 23 13:36:57 2023, max compression
+gzip compressed data, was "pulp_certguard-client-1.6.2.tar", last modified: Tue May  2 19:30:51 2023, max compression
```

## Comparing `pulp_certguard-client-1.6.1.tar` & `pulp_certguard-client-1.6.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.932014 pulp_certguard-client-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-23 13:36:57.932014 pulp_certguard-client-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.928014 pulp_certguard-client-1.6.1/pulp_certguard_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulp_certguard_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulp_certguard_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulp_certguard_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulp_certguard_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulp_certguard_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.928014 pulp_certguard-client-1.6.1/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.928014 pulp_certguard-client-1.6.1/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.932014 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.932014 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39373 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39181 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.932014 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-03-23 13:36:57.000000 pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-23 13:36:57.932014 pulp_certguard-client-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:36:57.932014 pulp_certguard-client-1.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_certguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_certguard_rhsm_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_certguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_certguard_x509_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_contentguards_rhsm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_contentguards_x509_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_paginatedcertguard_x509_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_patchedcertguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-23 13:36:56.000000 pulp_certguard-client-1.6.1/test/test_patchedcertguard_x509_cert_guard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 19:30:51.064302 pulp_certguard-client-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.056302 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-02 19:30:51.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.056302 pulp_certguard-client-1.6.2/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.056302 pulp_certguard-client-1.6.2/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41233 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 19:30:51.064302 pulp_certguard-client-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_contentguards_rhsm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_contentguards_x509_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_paginatedcertguard_x509_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_patchedcertguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_patchedcertguard_x509_cert_guard.py
```

### Comparing `pulp_certguard-client-1.6.1/README.md` & `pulp_certguard-client-1.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_certguard-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 1.6.1
+- Package version: 1.6.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_certguard-client-1.6.1/pulp_certguard_client.egg-info/SOURCES.txt` & `pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/__init__.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 # import apis into sdk package
 from pulpcore.client.pulp_certguard.api.contentguards_rhsm_api import ContentguardsRhsmApi
 from pulpcore.client.pulp_certguard.api.contentguards_x509_api import ContentguardsX509Api
 
 # import ApiClient
 from pulpcore.client.pulp_certguard.api_client import ApiClient
```

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,80 +21,80 @@
 from pulpcore.client.pulp_certguard.api_client import ApiClient
 from pulpcore.client.pulp_certguard.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ContentguardsRhsmApi(object):
+class ContentguardsX509Api(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create(self, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
-        """Create a rhsm cert guard  # noqa: E501
+    def create(self, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
+        """Create a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create(certguard_rhsm_cert_guard, async_req=True)
+        >>> thread = api.create(certguard_x509_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
+        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardRHSMCertGuardResponse
+        :return: CertguardX509CertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_with_http_info(certguard_rhsm_cert_guard,  **kwargs)  # noqa: E501
+        return self.create_with_http_info(certguard_x509_cert_guard,  **kwargs)  # noqa: E501
 
-    def create_with_http_info(self, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
-        """Create a rhsm cert guard  # noqa: E501
+    def create_with_http_info(self, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
+        """Create a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_with_http_info(certguard_rhsm_cert_guard, async_req=True)
+        >>> thread = api.create_with_http_info(certguard_x509_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
+        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_rhsm_cert_guard'
+            'certguard_x509_cert_guard'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -105,96 +105,96 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method create" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_rhsm_cert_guard' is set
-        if self.api_client.client_side_validation and ('certguard_rhsm_cert_guard' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_rhsm_cert_guard'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_rhsm_cert_guard` when calling `create`")  # noqa: E501
+        # verify the required parameter 'certguard_x509_cert_guard' is set
+        if self.api_client.client_side_validation and ('certguard_x509_cert_guard' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_x509_cert_guard'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard` when calling `create`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'certguard_rhsm_cert_guard' in local_var_params:
-            body_params = local_var_params['certguard_rhsm_cert_guard']
+        if 'certguard_x509_cert_guard' in local_var_params:
+            body_params = local_var_params['certguard_x509_cert_guard']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/x-www-form-urlencoded', 'multipart/form-data'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/contentguards/certguard/rhsm/', 'POST',
+            '/pulp/api/v3/contentguards/certguard/x509/', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
+            response_type='CertguardX509CertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
-        """Delete a rhsm cert guard  # noqa: E501
+    def delete(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
+        """Delete a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.delete(certguard_r_h_s_m_cert_guard_href, async_req=True)
+        >>> thread = api.delete(certguard_x509_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param str certguard_x509_cert_guard_href: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_with_http_info(certguard_r_h_s_m_cert_guard_href,  **kwargs)  # noqa: E501
+        return self.delete_with_http_info(certguard_x509_cert_guard_href,  **kwargs)  # noqa: E501
 
-    def delete_with_http_info(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
-        """Delete a rhsm cert guard  # noqa: E501
+    def delete_with_http_info(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
+        """Delete a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.delete_with_http_info(certguard_r_h_s_m_cert_guard_href, async_req=True)
+        >>> thread = api.delete_with_http_info(certguard_x509_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param str certguard_x509_cert_guard_href: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -204,15 +204,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_r_h_s_m_cert_guard_href'
+            'certguard_x509_cert_guard_href'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -223,38 +223,38 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method delete" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `delete`")  # noqa: E501
+        # verify the required parameter 'certguard_x509_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
-            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
+        if 'certguard_x509_cert_guard_href' in local_var_params:
+            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_r_h_s_m_cert_guard_href}', 'DELETE',
+            '{certguard_x509_cert_guard_href}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
@@ -262,77 +262,81 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def list(self,  **kwargs):  # noqa: E501
-        """List rhsm cert guards  # noqa: E501
+        """List x509 cert guards  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `description` - Description * `-description` - Description (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: PaginatedcertguardRHSMCertGuardResponseList
+        :return: PaginatedcertguardX509CertGuardResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.list_with_http_info( **kwargs)  # noqa: E501
 
     def list_with_http_info(self,  **kwargs):  # noqa: E501
-        """List rhsm cert guards  # noqa: E501
+        """List x509 cert guards  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `description` - Description * `-description` - Description (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(PaginatedcertguardRHSMCertGuardResponseList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PaginatedcertguardX509CertGuardResponseList, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -340,14 +344,16 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -384,14 +390,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
             collection_formats['exclude_fields'] = 'multi'  # noqa: E501
 
@@ -405,86 +417,86 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/contentguards/certguard/rhsm/', 'GET',
+            '/pulp/api/v3/contentguards/certguard/x509/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedcertguardRHSMCertGuardResponseList',  # noqa: E501
+            response_type='PaginatedcertguardX509CertGuardResponseList',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def partial_update(self, certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
-        """Update a rhsm cert guard  # noqa: E501
+    def partial_update(self, certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard,  **kwargs):  # noqa: E501
+        """Update a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.partial_update(certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard, async_req=True)
+        >>> thread = api.partial_update(certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
-        :param PatchedcertguardRHSMCertGuard patchedcertguard_rhsm_cert_guard: (required)
+        :param str certguard_x509_cert_guard_href: (required)
+        :param PatchedcertguardX509CertGuard patchedcertguard_x509_cert_guard: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardRHSMCertGuardResponse
+        :return: CertguardX509CertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.partial_update_with_http_info(certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard,  **kwargs)  # noqa: E501
+        return self.partial_update_with_http_info(certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard,  **kwargs)  # noqa: E501
 
-    def partial_update_with_http_info(self, certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
-        """Update a rhsm cert guard  # noqa: E501
+    def partial_update_with_http_info(self, certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard,  **kwargs):  # noqa: E501
+        """Update a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.partial_update_with_http_info(certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard, async_req=True)
+        >>> thread = api.partial_update_with_http_info(certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
-        :param PatchedcertguardRHSMCertGuard patchedcertguard_rhsm_cert_guard: (required)
+        :param str certguard_x509_cert_guard_href: (required)
+        :param PatchedcertguardX509CertGuard patchedcertguard_x509_cert_guard: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_r_h_s_m_cert_guard_href',
-            'patchedcertguard_rhsm_cert_guard'
+            'certguard_x509_cert_guard_href',
+            'patchedcertguard_x509_cert_guard'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -495,124 +507,124 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method partial_update" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `partial_update`")  # noqa: E501
-        # verify the required parameter 'patchedcertguard_rhsm_cert_guard' is set
-        if self.api_client.client_side_validation and ('patchedcertguard_rhsm_cert_guard' not in local_var_params or  # noqa: E501
-                                                        local_var_params['patchedcertguard_rhsm_cert_guard'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `patchedcertguard_rhsm_cert_guard` when calling `partial_update`")  # noqa: E501
+        # verify the required parameter 'certguard_x509_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `partial_update`")  # noqa: E501
+        # verify the required parameter 'patchedcertguard_x509_cert_guard' is set
+        if self.api_client.client_side_validation and ('patchedcertguard_x509_cert_guard' not in local_var_params or  # noqa: E501
+                                                        local_var_params['patchedcertguard_x509_cert_guard'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `patchedcertguard_x509_cert_guard` when calling `partial_update`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
-            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
+        if 'certguard_x509_cert_guard_href' in local_var_params:
+            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'patchedcertguard_rhsm_cert_guard' in local_var_params:
-            body_params = local_var_params['patchedcertguard_rhsm_cert_guard']
+        if 'patchedcertguard_x509_cert_guard' in local_var_params:
+            body_params = local_var_params['patchedcertguard_x509_cert_guard']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/x-www-form-urlencoded', 'multipart/form-data'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_r_h_s_m_cert_guard_href}', 'PATCH',
+            '{certguard_x509_cert_guard_href}', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
+            response_type='CertguardX509CertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
-        """Inspect a rhsm cert guard  # noqa: E501
+    def read(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
+        """Inspect a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read(certguard_r_h_s_m_cert_guard_href, async_req=True)
+        >>> thread = api.read(certguard_x509_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param str certguard_x509_cert_guard_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardRHSMCertGuardResponse
+        :return: CertguardX509CertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(certguard_r_h_s_m_cert_guard_href,  **kwargs)  # noqa: E501
+        return self.read_with_http_info(certguard_x509_cert_guard_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
-        """Inspect a rhsm cert guard  # noqa: E501
+    def read_with_http_info(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
+        """Inspect a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read_with_http_info(certguard_r_h_s_m_cert_guard_href, async_req=True)
+        >>> thread = api.read_with_http_info(certguard_x509_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param str certguard_x509_cert_guard_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_r_h_s_m_cert_guard_href',
+            'certguard_x509_cert_guard_href',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -625,24 +637,24 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method read" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `read`")  # noqa: E501
+        # verify the required parameter 'certguard_x509_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `read`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
-            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
+        if 'certguard_x509_cert_guard_href' in local_var_params:
+            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
 
         query_params = []
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
@@ -658,86 +670,86 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_r_h_s_m_cert_guard_href}', 'GET',
+            '{certguard_x509_cert_guard_href}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
+            response_type='CertguardX509CertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update(self, certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
-        """Update a rhsm cert guard  # noqa: E501
+    def update(self, certguard_x509_cert_guard_href, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
+        """Update a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update(certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard, async_req=True)
+        >>> thread = api.update(certguard_x509_cert_guard_href, certguard_x509_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
-        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
+        :param str certguard_x509_cert_guard_href: (required)
+        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardRHSMCertGuardResponse
+        :return: CertguardX509CertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_with_http_info(certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard,  **kwargs)  # noqa: E501
+        return self.update_with_http_info(certguard_x509_cert_guard_href, certguard_x509_cert_guard,  **kwargs)  # noqa: E501
 
-    def update_with_http_info(self, certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
-        """Update a rhsm cert guard  # noqa: E501
+    def update_with_http_info(self, certguard_x509_cert_guard_href, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
+        """Update a x509 cert guard  # noqa: E501
 
-        RHSMCertGuard API Viewsets.  # noqa: E501
+        X509CertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_with_http_info(certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard, async_req=True)
+        >>> thread = api.update_with_http_info(certguard_x509_cert_guard_href, certguard_x509_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_r_h_s_m_cert_guard_href: (required)
-        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
+        :param str certguard_x509_cert_guard_href: (required)
+        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_r_h_s_m_cert_guard_href',
-            'certguard_rhsm_cert_guard'
+            'certguard_x509_cert_guard_href',
+            'certguard_x509_cert_guard'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -748,58 +760,58 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method update" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `update`")  # noqa: E501
-        # verify the required parameter 'certguard_rhsm_cert_guard' is set
-        if self.api_client.client_side_validation and ('certguard_rhsm_cert_guard' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_rhsm_cert_guard'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_rhsm_cert_guard` when calling `update`")  # noqa: E501
+        # verify the required parameter 'certguard_x509_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `update`")  # noqa: E501
+        # verify the required parameter 'certguard_x509_cert_guard' is set
+        if self.api_client.client_side_validation and ('certguard_x509_cert_guard' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_x509_cert_guard'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard` when calling `update`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
-            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
+        if 'certguard_x509_cert_guard_href' in local_var_params:
+            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'certguard_rhsm_cert_guard' in local_var_params:
-            body_params = local_var_params['certguard_rhsm_cert_guard']
+        if 'certguard_x509_cert_guard' in local_var_params:
+            body_params = local_var_params['certguard_x509_cert_guard']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/x-www-form-urlencoded', 'multipart/form-data'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_r_h_s_m_cert_guard_href}', 'PUT',
+            '{certguard_x509_cert_guard_href}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
+            response_type='CertguardX509CertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,80 +21,80 @@
 from pulpcore.client.pulp_certguard.api_client import ApiClient
 from pulpcore.client.pulp_certguard.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ContentguardsX509Api(object):
+class ContentguardsRhsmApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create(self, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
-        """Create a x509 cert guard  # noqa: E501
+    def create(self, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
+        """Create a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create(certguard_x509_cert_guard, async_req=True)
+        >>> thread = api.create(certguard_rhsm_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
+        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardX509CertGuardResponse
+        :return: CertguardRHSMCertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_with_http_info(certguard_x509_cert_guard,  **kwargs)  # noqa: E501
+        return self.create_with_http_info(certguard_rhsm_cert_guard,  **kwargs)  # noqa: E501
 
-    def create_with_http_info(self, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
-        """Create a x509 cert guard  # noqa: E501
+    def create_with_http_info(self, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
+        """Create a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_with_http_info(certguard_x509_cert_guard, async_req=True)
+        >>> thread = api.create_with_http_info(certguard_rhsm_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
+        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_x509_cert_guard'
+            'certguard_rhsm_cert_guard'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -105,96 +105,96 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method create" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_x509_cert_guard' is set
-        if self.api_client.client_side_validation and ('certguard_x509_cert_guard' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_x509_cert_guard'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard` when calling `create`")  # noqa: E501
+        # verify the required parameter 'certguard_rhsm_cert_guard' is set
+        if self.api_client.client_side_validation and ('certguard_rhsm_cert_guard' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_rhsm_cert_guard'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_rhsm_cert_guard` when calling `create`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'certguard_x509_cert_guard' in local_var_params:
-            body_params = local_var_params['certguard_x509_cert_guard']
+        if 'certguard_rhsm_cert_guard' in local_var_params:
+            body_params = local_var_params['certguard_rhsm_cert_guard']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/x-www-form-urlencoded', 'multipart/form-data'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/contentguards/certguard/x509/', 'POST',
+            '/pulp/api/v3/contentguards/certguard/rhsm/', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardX509CertGuardResponse',  # noqa: E501
+            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
-        """Delete a x509 cert guard  # noqa: E501
+    def delete(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
+        """Delete a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.delete(certguard_x509_cert_guard_href, async_req=True)
+        >>> thread = api.delete(certguard_r_h_s_m_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_with_http_info(certguard_x509_cert_guard_href,  **kwargs)  # noqa: E501
+        return self.delete_with_http_info(certguard_r_h_s_m_cert_guard_href,  **kwargs)  # noqa: E501
 
-    def delete_with_http_info(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
-        """Delete a x509 cert guard  # noqa: E501
+    def delete_with_http_info(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
+        """Delete a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.delete_with_http_info(certguard_x509_cert_guard_href, async_req=True)
+        >>> thread = api.delete_with_http_info(certguard_r_h_s_m_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -204,15 +204,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_x509_cert_guard_href'
+            'certguard_r_h_s_m_cert_guard_href'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -223,38 +223,38 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method delete" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_x509_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `delete`")  # noqa: E501
+        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_x509_cert_guard_href' in local_var_params:
-            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
+        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
+            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_x509_cert_guard_href}', 'DELETE',
+            '{certguard_r_h_s_m_cert_guard_href}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
@@ -262,77 +262,81 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def list(self,  **kwargs):  # noqa: E501
-        """List x509 cert guards  # noqa: E501
+        """List rhsm cert guards  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `description` - Description * `-description` - Description (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: PaginatedcertguardX509CertGuardResponseList
+        :return: PaginatedcertguardRHSMCertGuardResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.list_with_http_info( **kwargs)  # noqa: E501
 
     def list_with_http_info(self,  **kwargs):  # noqa: E501
-        """List x509 cert guards  # noqa: E501
+        """List rhsm cert guards  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `description` - Description * `-description` - Description (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(PaginatedcertguardX509CertGuardResponseList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PaginatedcertguardRHSMCertGuardResponseList, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -340,14 +344,16 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -384,14 +390,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
             collection_formats['exclude_fields'] = 'multi'  # noqa: E501
 
@@ -405,86 +417,86 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/contentguards/certguard/x509/', 'GET',
+            '/pulp/api/v3/contentguards/certguard/rhsm/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedcertguardX509CertGuardResponseList',  # noqa: E501
+            response_type='PaginatedcertguardRHSMCertGuardResponseList',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def partial_update(self, certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard,  **kwargs):  # noqa: E501
-        """Update a x509 cert guard  # noqa: E501
+    def partial_update(self, certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
+        """Update a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.partial_update(certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard, async_req=True)
+        >>> thread = api.partial_update(certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
-        :param PatchedcertguardX509CertGuard patchedcertguard_x509_cert_guard: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param PatchedcertguardRHSMCertGuard patchedcertguard_rhsm_cert_guard: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardX509CertGuardResponse
+        :return: CertguardRHSMCertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.partial_update_with_http_info(certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard,  **kwargs)  # noqa: E501
+        return self.partial_update_with_http_info(certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard,  **kwargs)  # noqa: E501
 
-    def partial_update_with_http_info(self, certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard,  **kwargs):  # noqa: E501
-        """Update a x509 cert guard  # noqa: E501
+    def partial_update_with_http_info(self, certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
+        """Update a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.partial_update_with_http_info(certguard_x509_cert_guard_href, patchedcertguard_x509_cert_guard, async_req=True)
+        >>> thread = api.partial_update_with_http_info(certguard_r_h_s_m_cert_guard_href, patchedcertguard_rhsm_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
-        :param PatchedcertguardX509CertGuard patchedcertguard_x509_cert_guard: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param PatchedcertguardRHSMCertGuard patchedcertguard_rhsm_cert_guard: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_x509_cert_guard_href',
-            'patchedcertguard_x509_cert_guard'
+            'certguard_r_h_s_m_cert_guard_href',
+            'patchedcertguard_rhsm_cert_guard'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -495,124 +507,124 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method partial_update" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_x509_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `partial_update`")  # noqa: E501
-        # verify the required parameter 'patchedcertguard_x509_cert_guard' is set
-        if self.api_client.client_side_validation and ('patchedcertguard_x509_cert_guard' not in local_var_params or  # noqa: E501
-                                                        local_var_params['patchedcertguard_x509_cert_guard'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `patchedcertguard_x509_cert_guard` when calling `partial_update`")  # noqa: E501
+        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `partial_update`")  # noqa: E501
+        # verify the required parameter 'patchedcertguard_rhsm_cert_guard' is set
+        if self.api_client.client_side_validation and ('patchedcertguard_rhsm_cert_guard' not in local_var_params or  # noqa: E501
+                                                        local_var_params['patchedcertguard_rhsm_cert_guard'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `patchedcertguard_rhsm_cert_guard` when calling `partial_update`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_x509_cert_guard_href' in local_var_params:
-            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
+        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
+            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'patchedcertguard_x509_cert_guard' in local_var_params:
-            body_params = local_var_params['patchedcertguard_x509_cert_guard']
+        if 'patchedcertguard_rhsm_cert_guard' in local_var_params:
+            body_params = local_var_params['patchedcertguard_rhsm_cert_guard']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/x-www-form-urlencoded', 'multipart/form-data'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_x509_cert_guard_href}', 'PATCH',
+            '{certguard_r_h_s_m_cert_guard_href}', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardX509CertGuardResponse',  # noqa: E501
+            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
-        """Inspect a x509 cert guard  # noqa: E501
+    def read(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
+        """Inspect a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read(certguard_x509_cert_guard_href, async_req=True)
+        >>> thread = api.read(certguard_r_h_s_m_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardX509CertGuardResponse
+        :return: CertguardRHSMCertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(certguard_x509_cert_guard_href,  **kwargs)  # noqa: E501
+        return self.read_with_http_info(certguard_r_h_s_m_cert_guard_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, certguard_x509_cert_guard_href,  **kwargs):  # noqa: E501
-        """Inspect a x509 cert guard  # noqa: E501
+    def read_with_http_info(self, certguard_r_h_s_m_cert_guard_href,  **kwargs):  # noqa: E501
+        """Inspect a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read_with_http_info(certguard_x509_cert_guard_href, async_req=True)
+        >>> thread = api.read_with_http_info(certguard_r_h_s_m_cert_guard_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_x509_cert_guard_href',
+            'certguard_r_h_s_m_cert_guard_href',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -625,24 +637,24 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method read" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_x509_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `read`")  # noqa: E501
+        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `read`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_x509_cert_guard_href' in local_var_params:
-            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
+        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
+            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
 
         query_params = []
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
@@ -658,86 +670,86 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_x509_cert_guard_href}', 'GET',
+            '{certguard_r_h_s_m_cert_guard_href}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardX509CertGuardResponse',  # noqa: E501
+            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update(self, certguard_x509_cert_guard_href, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
-        """Update a x509 cert guard  # noqa: E501
+    def update(self, certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
+        """Update a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update(certguard_x509_cert_guard_href, certguard_x509_cert_guard, async_req=True)
+        >>> thread = api.update(certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
-        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: CertguardX509CertGuardResponse
+        :return: CertguardRHSMCertGuardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_with_http_info(certguard_x509_cert_guard_href, certguard_x509_cert_guard,  **kwargs)  # noqa: E501
+        return self.update_with_http_info(certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard,  **kwargs)  # noqa: E501
 
-    def update_with_http_info(self, certguard_x509_cert_guard_href, certguard_x509_cert_guard,  **kwargs):  # noqa: E501
-        """Update a x509 cert guard  # noqa: E501
+    def update_with_http_info(self, certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard,  **kwargs):  # noqa: E501
+        """Update a rhsm cert guard  # noqa: E501
 
-        X509CertGuard API Viewsets.  # noqa: E501
+        RHSMCertGuard API Viewsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_with_http_info(certguard_x509_cert_guard_href, certguard_x509_cert_guard, async_req=True)
+        >>> thread = api.update_with_http_info(certguard_r_h_s_m_cert_guard_href, certguard_rhsm_cert_guard, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str certguard_x509_cert_guard_href: (required)
-        :param CertguardX509CertGuard certguard_x509_cert_guard: (required)
+        :param str certguard_r_h_s_m_cert_guard_href: (required)
+        :param CertguardRHSMCertGuard certguard_rhsm_cert_guard: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(CertguardX509CertGuardResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(CertguardRHSMCertGuardResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'certguard_x509_cert_guard_href',
-            'certguard_x509_cert_guard'
+            'certguard_r_h_s_m_cert_guard_href',
+            'certguard_rhsm_cert_guard'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -748,58 +760,58 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method update" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'certguard_x509_cert_guard_href' is set
-        if self.api_client.client_side_validation and ('certguard_x509_cert_guard_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_x509_cert_guard_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard_href` when calling `update`")  # noqa: E501
-        # verify the required parameter 'certguard_x509_cert_guard' is set
-        if self.api_client.client_side_validation and ('certguard_x509_cert_guard' not in local_var_params or  # noqa: E501
-                                                        local_var_params['certguard_x509_cert_guard'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `certguard_x509_cert_guard` when calling `update`")  # noqa: E501
+        # verify the required parameter 'certguard_r_h_s_m_cert_guard_href' is set
+        if self.api_client.client_side_validation and ('certguard_r_h_s_m_cert_guard_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_r_h_s_m_cert_guard_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_r_h_s_m_cert_guard_href` when calling `update`")  # noqa: E501
+        # verify the required parameter 'certguard_rhsm_cert_guard' is set
+        if self.api_client.client_side_validation and ('certguard_rhsm_cert_guard' not in local_var_params or  # noqa: E501
+                                                        local_var_params['certguard_rhsm_cert_guard'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `certguard_rhsm_cert_guard` when calling `update`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'certguard_x509_cert_guard_href' in local_var_params:
-            path_params['certguard_x509_cert_guard_href'] = local_var_params['certguard_x509_cert_guard_href']  # noqa: E501
+        if 'certguard_r_h_s_m_cert_guard_href' in local_var_params:
+            path_params['certguard_r_h_s_m_cert_guard_href'] = local_var_params['certguard_r_h_s_m_cert_guard_href']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'certguard_x509_cert_guard' in local_var_params:
-            body_params = local_var_params['certguard_x509_cert_guard']
+        if 'certguard_rhsm_cert_guard' in local_var_params:
+            body_params = local_var_params['certguard_rhsm_cert_guard']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/x-www-form-urlencoded', 'multipart/form-data'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{certguard_x509_cert_guard_href}', 'PUT',
+            '{certguard_r_h_s_m_cert_guard_href}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CertguardX509CertGuardResponse',  # noqa: E501
+            response_type='CertguardRHSMCertGuardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/api_client.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.6.1/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/configuration.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 1.6.1".\
+               "SDK Package Version: 1.6.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/exceptions.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/__init__.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/pulpcore/client/pulp_certguard/rest.py` & `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/setup.py` & `pulp_certguard-client-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_certguard-client"
-VERSION = "1.6.1"
+VERSION = "1.6.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_certguard-client-1.6.1/test/test_certguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_certguard_rhsm_cert_guard_response.py` & `pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_certguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_certguard_x509_cert_guard_response.py` & `pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_contentguards_rhsm_api.py` & `pulp_certguard-client-1.6.2/test/test_contentguards_rhsm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_contentguards_x509_api.py` & `pulp_certguard-client-1.6.2/test/test_contentguards_x509_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py` & `pulp_certguard-client-1.6.2/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_paginatedcertguard_x509_cert_guard_response_list.py` & `pulp_certguard-client-1.6.2/test/test_paginatedcertguard_x509_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_patchedcertguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.2/test/test_patchedcertguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.1/test/test_patchedcertguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.2/test/test_patchedcertguard_x509_cert_guard.py`

 * *Files identical despite different names*

