# Comparing `tmp/pulp_certguard-client-1.6.2.tar.gz` & `tmp/pulp_certguard-client-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_certguard-client-1.6.2.tar", last modified: Tue May  2 19:30:51 2023, max compression
+gzip compressed data, was "pulp_certguard-client-1.6.3.tar", last modified: Tue May  2 20:16:55 2023, max compression
```

## Comparing `pulp_certguard-client-1.6.2.tar` & `pulp_certguard-client-1.6.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 19:30:51.064302 pulp_certguard-client-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.056302 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-02 19:30:51.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:30:50.000000 pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.056302 pulp_certguard-client-1.6.2/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.056302 pulp_certguard-client-1.6.2/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41233 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 19:30:51.064302 pulp_certguard-client-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:30:51.060302 pulp_certguard-client-1.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_contentguards_rhsm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_contentguards_x509_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_paginatedcertguard_x509_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_patchedcertguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 19:30:49.000000 pulp_certguard-client-1.6.2/test/test_patchedcertguard_x509_cert_guard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.323337 pulp_certguard-client-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 20:16:55.323337 pulp_certguard-client-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.315337 pulp_certguard-client-1.6.3/pulp_certguard_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 20:16:55.000000 pulp_certguard-client-1.6.3/pulp_certguard_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-02 20:16:55.000000 pulp_certguard-client-1.6.3/pulp_certguard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:16:55.000000 pulp_certguard-client-1.6.3/pulp_certguard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 20:16:55.000000 pulp_certguard-client-1.6.3/pulp_certguard_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 20:16:55.000000 pulp_certguard-client-1.6.3/pulp_certguard_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.315337 pulp_certguard-client-1.6.3/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.315337 pulp_certguard-client-1.6.3/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.319337 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.319337 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41233 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.319337 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 20:16:55.323337 pulp_certguard-client-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:16:55.323337 pulp_certguard-client-1.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_certguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_certguard_rhsm_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_certguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_certguard_x509_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_contentguards_rhsm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_contentguards_x509_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_paginatedcertguard_x509_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_patchedcertguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 20:16:54.000000 pulp_certguard-client-1.6.3/test/test_patchedcertguard_x509_cert_guard.py
```

### Comparing `pulp_certguard-client-1.6.2/README.md` & `pulp_certguard-client-1.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_certguard-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 1.6.2
+- Package version: 1.6.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_certguard-client-1.6.2/pulp_certguard_client.egg-info/SOURCES.txt` & `pulp_certguard-client-1.6.3/pulp_certguard_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/__init__.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.6.2"
+__version__ = "1.6.3"
 
 # import apis into sdk package
 from pulpcore.client.pulp_certguard.api.contentguards_rhsm_api import ContentguardsRhsmApi
 from pulpcore.client.pulp_certguard.api.contentguards_x509_api import ContentguardsX509Api
 
 # import ApiClient
 from pulpcore.client.pulp_certguard.api_client import ApiClient
```

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/api_client.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.6.2/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/configuration.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 1.6.2".\
+               "SDK Package Version: 1.6.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/exceptions.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/__init__.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/pulpcore/client/pulp_certguard/rest.py` & `pulp_certguard-client-1.6.3/pulpcore/client/pulp_certguard/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/setup.py` & `pulp_certguard-client-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_certguard-client"
-VERSION = "1.6.2"
+VERSION = "1.6.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.3/test/test_certguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_certguard_rhsm_cert_guard_response.py` & `pulp_certguard-client-1.6.3/test/test_certguard_rhsm_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.3/test/test_certguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_certguard_x509_cert_guard_response.py` & `pulp_certguard-client-1.6.3/test/test_certguard_x509_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_contentguards_rhsm_api.py` & `pulp_certguard-client-1.6.3/test/test_contentguards_rhsm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_contentguards_x509_api.py` & `pulp_certguard-client-1.6.3/test/test_contentguards_x509_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py` & `pulp_certguard-client-1.6.3/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_paginatedcertguard_x509_cert_guard_response_list.py` & `pulp_certguard-client-1.6.3/test/test_paginatedcertguard_x509_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_patchedcertguard_rhsm_cert_guard.py` & `pulp_certguard-client-1.6.3/test/test_patchedcertguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-1.6.2/test/test_patchedcertguard_x509_cert_guard.py` & `pulp_certguard-client-1.6.3/test/test_patchedcertguard_x509_cert_guard.py`

 * *Files identical despite different names*

