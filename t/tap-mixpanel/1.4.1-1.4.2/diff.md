# Comparing `tmp/tap-mixpanel-1.4.1.tar.gz` & `tmp/tap-mixpanel-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mixpanel-1.4.1.tar", last modified: Tue Dec  7 15:06:07 2021, max compression
+gzip compressed data, was "tap-mixpanel-1.4.2.tar", last modified: Tue May  2 18:04:21 2023, max compression
```

## Comparing `tap-mixpanel-1.4.1.tar` & `tap-mixpanel-1.4.2.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.510352 tap-mixpanel-1.4.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2021-12-07 15:06:07.510352 tap-mixpanel-1.4.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12637 2021-12-06 16:46:06.000000 tap-mixpanel-1.4.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2021-12-07 15:06:07.510352 tap-mixpanel-1.4.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2021-12-07 15:05:35.000000 tap-mixpanel-1.4.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.498352 tap-mixpanel-1.4.1/tap_mixpanel/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2778 2021-12-06 16:46:06.000000 tap-mixpanel-1.4.1/tap_mixpanel/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10005 2021-12-06 16:46:06.000000 tap-mixpanel-1.4.1/tap_mixpanel/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tap_mixpanel/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5787 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tap_mixpanel/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.502352 tap-mixpanel-1.4.1/tap_mixpanel/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tap_mixpanel/schemas/annotations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tap_mixpanel/schemas/cohort_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      510 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tap_mixpanel/schemas/cohorts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tap_mixpanel/schemas/engage.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      603 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tap_mixpanel/schemas/export.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3390 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tap_mixpanel/schemas/funnels.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tap_mixpanel/schemas/revenue.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26299 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tap_mixpanel/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1771 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tap_mixpanel/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3608 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tap_mixpanel/transform.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.502352 tap-mixpanel-1.4.1/tap_mixpanel.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      313 2021-12-07 15:06:07.000000 tap-mixpanel-1.4.1/tap_mixpanel.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1277 2021-12-07 15:06:07.000000 tap-mixpanel-1.4.1/tap_mixpanel.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-12-07 15:06:07.000000 tap-mixpanel-1.4.1/tap_mixpanel.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2021-12-07 15:06:07.000000 tap-mixpanel-1.4.1/tap_mixpanel.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       99 2021-12-07 15:06:07.000000 tap-mixpanel-1.4.1/tap_mixpanel.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2021-12-07 15:06:07.000000 tap-mixpanel-1.4.1/tap_mixpanel.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.502352 tap-mixpanel-1.4.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.502352 tap-mixpanel-1.4.1/tests/configuration/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tests/configuration/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2021-12-06 16:46:06.000000 tap-mixpanel-1.4.1/tests/configuration/fixtures.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.506352 tap-mixpanel-1.4.1/tests/tap_tester/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tests/tap_tester/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14828 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/tap_tester/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2460 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/tap_tester/test_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8729 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/tap_tester/test_bookmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6951 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/tap_tester/test_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6580 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/tap_tester/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7503 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/tap_tester/test_start_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1455 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/tap_tester/test_sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-07 15:06:07.510352 tap-mixpanel-1.4.1/tests/unittests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tests/unittests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21600 2021-12-06 16:46:06.000000 tap-mixpanel-1.4.1/tests/unittests/test_error_handling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4732 2021-09-27 18:04:29.000000 tap-mixpanel-1.4.1/tests/unittests/test_medium_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6150 2021-12-06 16:46:06.000000 tap-mixpanel-1.4.1/tests/unittests/test_request_timeout_param_value.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5633 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/unittests/test_support_eu_endpoints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2021-10-27 15:48:39.000000 tap-mixpanel-1.4.1/tests/unittests/test_transform_event_times.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    34523 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/LICENSE
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       52 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/MANIFEST.in
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      249 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/PKG-INFO
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    12637 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/README.md
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      125 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/setup.cfg
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      837 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/setup.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tap_mixpanel/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2778 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/__init__.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    10077 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/client.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      686 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/discover.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     5787 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schema.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tap_mixpanel/schemas/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      335 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/annotations.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      199 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/cohort_members.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      510 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/cohorts.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      139 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/engage.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      603 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/export.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3390 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/funnels.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      449 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/schemas/revenue.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    26299 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/streams.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1771 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/sync.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3608 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tap_mixpanel/transform.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      249 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/PKG-INFO
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1258 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        1 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       51 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/entry_points.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       99 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/requires.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       19 2023-05-02 18:04:21.000000 tap-mixpanel-1.4.2/tap_mixpanel.egg-info/top_level.txt
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tests/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/__init__.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.589726 tap-mixpanel-1.4.2/tests/configuration/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/configuration/__init__.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      443 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/configuration/fixtures.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/tests/tap_tester/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      164 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/__init__.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    14803 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/base.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     7586 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_all_fields_pagination.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2555 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_automatic_fields.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     8800 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_bookmark.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     7069 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_discovery.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     7517 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/tap_tester/test_start_date.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:04:21.593726 tap-mixpanel-1.4.2/tests/unittests/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/__init__.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    22322 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_error_handling.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     4732 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_medium_client.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     6150 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_request_timeout_param_value.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     5633 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_support_eu_endpoints.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1107 2023-05-02 18:02:59.000000 tap-mixpanel-1.4.2/tests/unittests/test_transform_event_times.py
```

### Comparing `tap-mixpanel-1.4.1/LICENSE` & `tap-mixpanel-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/README.md` & `tap-mixpanel-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/setup.py` & `tap-mixpanel-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-mixpanel',
-      version='1.4.1',
+      version='1.4.2',
       description='Singer.io tap for extracting data from the mixpanel API',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mixpanel'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/__init__.py` & `tap-mixpanel-1.4.2/tap_mixpanel/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/client.py` & `tap-mixpanel-1.4.2/tap_mixpanel/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import io
 
 import backoff
 import jsonlines
 import requests
 import singer
 from requests.exceptions import ConnectionError, Timeout
+from requests.models import ProtocolError
 from singer import metrics
 
 LOGGER = singer.get_logger()
 
 BACKOFF_MAX_TRIES_REQUEST = 7
 REQUEST_TIMEOUT = 300
 
@@ -133,15 +134,15 @@
         self.__verified = self.check_access()
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
         self.__session.close()
 
     @backoff.on_exception(backoff.expo,
-                          (Server5xxError, Server429Error, ReadTimeoutError, ConnectionError, Timeout),
+                          (Server5xxError, Server429Error, ReadTimeoutError, ConnectionError, Timeout, ProtocolError),
                           max_tries=5,
                           factor=2)
     def check_access(self):
         if self.__api_secret is None:
             raise Exception('Error: Missing api_secret in tap config.json.')
         headers = {}
         # Endpoint: simple API call to return a single record (org settings) to test access
@@ -170,15 +171,15 @@
             LOGGER.error('Error status_code = {}'.format(response.status_code))
             raise_for_error(response)
         else:
             return True
 
     @backoff.on_exception(
         backoff.expo,
-        (Server5xxError, Server429Error, ReadTimeoutError, ConnectionError, Timeout),
+        (Server5xxError, Server429Error, ReadTimeoutError, ConnectionError, Timeout, ProtocolError),
         max_tries=BACKOFF_MAX_TRIES_REQUEST,
         factor=3,
         logger=LOGGER)
     def perform_request(self,
                         method,
                         url=None,
                         params=None,
```

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/discover.py` & `tap-mixpanel-1.4.2/tap_mixpanel/discover.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/schema.py` & `tap-mixpanel-1.4.2/tap_mixpanel/schema.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/schemas/export.json` & `tap-mixpanel-1.4.2/tap_mixpanel/schemas/export.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/schemas/funnels.json` & `tap-mixpanel-1.4.2/tap_mixpanel/schemas/funnels.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/streams.py` & `tap-mixpanel-1.4.2/tap_mixpanel/streams.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/sync.py` & `tap-mixpanel-1.4.2/tap_mixpanel/sync.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel/transform.py` & `tap-mixpanel-1.4.2/tap_mixpanel/transform.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tap_mixpanel.egg-info/SOURCES.txt` & `tap-mixpanel-1.4.2/tap_mixpanel.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,19 +24,18 @@
 tap_mixpanel/schemas/funnels.json
 tap_mixpanel/schemas/revenue.json
 tests/__init__.py
 tests/configuration/__init__.py
 tests/configuration/fixtures.py
 tests/tap_tester/__init__.py
 tests/tap_tester/base.py
+tests/tap_tester/test_all_fields_pagination.py
 tests/tap_tester/test_automatic_fields.py
 tests/tap_tester/test_bookmark.py
 tests/tap_tester/test_discovery.py
-tests/tap_tester/test_pagination.py
 tests/tap_tester/test_start_date.py
-tests/tap_tester/test_sync.py
 tests/unittests/__init__.py
 tests/unittests/test_error_handling.py
 tests/unittests/test_medium_client.py
 tests/unittests/test_request_timeout_param_value.py
 tests/unittests/test_support_eu_endpoints.py
 tests/unittests/test_transform_event_times.py
```

### Comparing `tap-mixpanel-1.4.1/tests/tap_tester/base.py` & `tap-mixpanel-1.4.2/tests/tap_tester/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,37 +6,36 @@
 import unittest
 from datetime import datetime as dt
 from datetime import timedelta
 
 import dateutil.parser
 import pytz
 
-import tap_tester.connections as connections
-import tap_tester.runner as runner
+from tap_tester import connections
+from tap_tester import runner
 from tap_tester import menagerie
+from tap_tester.logger import LOGGER
+from tap_tester.base_case import BaseCase
 
 
-class TestMixPanelBase(unittest.TestCase):
+class TestMixPanelBase(BaseCase):
     """ Test the tap combined """
     START_DATE_FORMAT = "%Y-%m-%dT00:00:00Z"
     REPLICATION_KEYS = "valid-replication-keys"
     PRIMARY_KEYS = "table-key-properties"
     FOREIGN_KEYS = "table-foreign-key-properties"
     REPLICATION_METHOD = "forced-replication-method"
     INCREMENTAL = "INCREMENTAL"
     FULL_TABLE = "FULL_TABLE"
     API_LIMIT = 250
     TYPE = "platform.mixpanel"
     start_date = ""
     end_date = ""
     eu_residency = True
 
-    def name(self):
-        return "mixpnel-base"
-
     def tap_name(self):
         """The name of the tap"""
         return "tap-mixpanel"
 
     def expected_metadata(self):
         """The expected streams and metadata about the streams"""
         return {
@@ -84,14 +83,16 @@
         for cred in creds:
             if os.getenv(creds[cred]) == None:
                 missing_envs.append(creds[cred])
 
         if len(missing_envs) != 0:
             raise Exception("set " + ", ".join(missing_envs))
 
+        BaseCase.setUp(self)
+
     def get_type(self):
         """the expected url route ending"""
         return "platform.mixpanel"
 
     def get_properties(self, original: bool = True):
         """Configuration properties required for the tap."""
 
@@ -192,15 +193,15 @@
 
         found_catalog_names = set(
             map(lambda c: c['stream_name'], found_catalogs))
 
         subset = self.expected_streams().issubset(found_catalog_names)
         self.assertTrue(
             subset, msg="Expected check streams are not subset of discovered catalog")
-        print("discovered schemas are OK")
+        LOGGER.info("discovered schemas are OK")
 
         return found_catalogs
 
     def run_and_verify_sync(self, conn_id):
         """
         Run a sync job and make sure it exited properly.
         Return a dictionary with keys of streams synced
@@ -217,16 +218,15 @@
         # Verify actual rows were synced
         sync_record_count = runner.examine_target_output_file(
             self, conn_id, self.expected_streams(), self.expected_pks())
         self.assertGreater(
             sum(sync_record_count.values()), 0,
             msg="failed to replicate any data: {}".format(sync_record_count)
         )
-        print("total replicated row count: {}".format(
-            sum(sync_record_count.values())))
+        LOGGER.info(f"total replicated row count: {sum(sync_record_count.values())}")
 
         return sync_record_count
 
     def perform_and_verify_table_and_field_selection(self, conn_id, test_catalogs, select_all_fields=True):
         """
         Perform table and field selection based off of the streams to select
         set and field selection parameters.
@@ -245,28 +245,28 @@
 
         for cat in catalogs:
             catalog_entry = menagerie.get_annotated_schema(
                 conn_id, cat['stream_id'])
 
             # Verify all testable streams are selected
             selected = catalog_entry.get('annotated-schema').get('selected')
-            print("Validating selection on {}: {}".format(
-                cat['stream_name'], selected))
+            LOGGER.info(f"Validating selection on {cat['stream_name']}: {selected}")
+
             if cat['stream_name'] not in expected_selected:
                 self.assertFalse(
                     selected, msg="Stream selected, but not testable.")
                 continue  # Skip remaining assertions if we aren't selecting this stream
             self.assertTrue(selected, msg="Stream not selected.")
 
             if select_all_fields:
                 # Verify all fields within each selected stream are selected
                 for field, field_props in catalog_entry.get('annotated-schema').get('properties').items():
                     field_selected = field_props.get('selected')
-                    print("\tValidating selection on {}.{}: {}".format(
-                        cat['stream_name'], field, field_selected))
+                    LOGGER.info(f"\tValidating selection on {cat['stream_name']}.{field}: {field_selected}")
+
                     self.assertTrue(field_selected, msg="Field not selected.")
             else:
                 # Verify only automatic fields are selected
                 expected_automatic_fields = self.expected_automatic_fields().get(
                     cat['stream_name'])
                 selected_fields = self.get_selected_fields_from_metadata(
                     catalog_entry['metadata'])
```

### Comparing `tap-mixpanel-1.4.1/tests/tap_tester/test_automatic_fields.py` & `tap-mixpanel-1.4.2/tests/tap_tester/test_automatic_fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 class MixPanelAutomaticFieldsTest(TestMixPanelBase):
     """
     Ensure running the tap with all streams selected and all fields deselected results in the replication of just the
     primary keys and replication keys (automatic fields).
     """
 
-    def name(self):
+    @staticmethod
+    def name():
         return "mix_panel_automatic_fields_test"
 
     def automatic_fields_test_run(self):
         """
         Verify that for each stream you can get enough data
         when no fields are selected and only the automatic fields are replicated.
         """
@@ -43,21 +44,24 @@
                 data = synced_records.get(stream, {})
                 record_messages_keys = [set(row['data'].keys())
                                         for row in data.get('messages', [])]
 
                 # Verify that you get some records for each stream
                 self.assertGreater(
                     record_count_by_stream.get(stream, 0), 0,
-                    msg="The number of records is not over the stream max limit")
+                    msg="The number of records is not over the stream max limit",
+                )
 
                 # Verify that only the automatic fields are sent to the target
                 for actual_keys in record_messages_keys:
                     self.assertSetEqual(expected_keys, actual_keys)
 
-    def test_run(self):
-        #Automatic fields test for standard server
+
+    def test_standard_auto_fields(self):
+        """Automatic fields test for standard server"""
         self.eu_residency = False
         self.automatic_fields_test_run()
 
-        #Automatic fields test for EU recidency server
+    def test_eu_auto_fields(self):
+        """Automatic fields test for EU recidency server"""
         self.eu_residency = True
         self.automatic_fields_test_run()
```

### Comparing `tap-mixpanel-1.4.1/tests/tap_tester/test_bookmark.py` & `tap-mixpanel-1.4.2/tests/tap_tester/test_bookmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from base import TestMixPanelBase
 from tap_tester import menagerie
 
 
 class MixPanelBookMarkTest(TestMixPanelBase):
     """Test tap sets a bookmark and respects it for the next sync of a stream"""
 
-    def name(self):
+    @staticmethod
+    def name():
         return "mix_panel_bookmark_test"
 
     def bookmark_test_run(self):
         """
         Verify that for each stream you can do a sync which records bookmarks.
         That the bookmark is the maximum value sent to the target for the replication key.
         That a second sync respects the bookmark
@@ -23,15 +24,14 @@
 
         Verify that for full table stream, all data replicated in sync 1 is replicated again in sync 2.
 
         PREREQUISITE
         For EACH stream that is incrementally replicated there are multiple rows of data with
             different values for the replication key
         """
-
         expected_streams = self.expected_streams()
         expected_replication_keys = self.expected_replication_keys()
         expected_replication_methods = self.expected_replication_method()
 
         ##########################################################################
         # First Sync
         ##########################################################################
@@ -165,15 +165,16 @@
                             stream, expected_replication_method)
                     )
 
                 # Verify at least 1 record was replicated in the second sync
                 self.assertGreater(
                     second_sync_count, 0, msg="We are not fully testing bookmarking for {}".format(stream))
 
-    def test_run(self):
-        #Bookmark test for standard server
+    def test_standard_bookmarks(self):
+        """Bookmark test for standard server"""
         self.eu_residency = False
         self.bookmark_test_run()
 
-        #Bookmark test for EU recidency server
+    def test_eu_bookmarks(self):
+        """Bookmark test for EU recidency server"""
         self.eu_residency = True
         self.bookmark_test_run()
```

### Comparing `tap-mixpanel-1.4.1/tests/tap_tester/test_discovery.py` & `tap-mixpanel-1.4.2/tests/tap_tester/test_discovery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
+from tap_tester import menagerie, connections
+from tap_tester.logger import LOGGER
 
-import tap_tester.connections as connections
 from base import TestMixPanelBase
-from tap_tester import menagerie
-
 
 class MixPanelDiscoverTest(TestMixPanelBase):
     """
         Testing that discovery creates the appropriate catalog with valid metadata.
         • Verify number of actual streams discovered match expected
         • Verify the stream names discovered were what we expect
         • Verify stream names follow naming convention
@@ -18,39 +17,45 @@
         • verify that if there is a replication key we are doing INCREMENTAL otherwise FULL
         • verify the actual replication matches our expected replication method
         • verify that primary, replication and foreign keys
           are given the inclusion of automatic.
         • verify that all other fields have inclusion of available metadata.
     """
 
-    def name(self):
+    @staticmethod
+    def name():
         return "mix_panel_discover_test"
 
     def discovery_test_run(self):
+
+        region = "EU" if self.eu_residency else "Standard"
+        LOGGER.info(f"Testing against {region} account.")
+
+        self.assertion_logging_enabled = True
+
         streams_to_test = self.expected_streams()
 
         conn_id = connections.ensure_connection(self, payload_hook=None)
 
         # Verify that there are catalogs found
-        found_catalogs = found_catalogs = self.run_and_verify_check_mode(
-            conn_id)
+        found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # Verify stream names follow naming convention
         # streams should only have lowercase alphas and underscores
         found_catalog_names = {c['tap_stream_id'] for c in found_catalogs}
         self.assertTrue(all([re.fullmatch(r"[a-z_]+",  name) for name in found_catalog_names]),
-                        msg="One or more streams don't follow standard naming")
+                        logging="asserting all streams defined in catalog follow the naming convention '[a-z_]+'")
 
         for stream in streams_to_test:
             with self.subTest(stream=stream):
 
-                # Verify ensure the caatalog is found for a given stream
+                # Verify the caatalog is found for a given stream
                 catalog = next(iter([catalog for catalog in found_catalogs
                                      if catalog["stream_name"] == stream]))
-                self.assertIsNotNone(catalog)
+                self.assertIsNotNone(catalog, logging="asserting entry is present in catalog")
 
                 # collecting expected values
                 expected_primary_keys = self.expected_pks()[stream]
                 expected_replication_keys = self.expected_replication_keys()[
                     stream]
                 expected_automatic_fields = self.expected_automatic_fields().get(stream)
                 expected_replication_method = self.expected_replication_method()[
@@ -78,61 +83,60 @@
                 )
 
                 ##########################################################################
                 # metadata assertions
                 ##########################################################################
 
                 # verify there is only 1 top level breadcrumb in metadata
-                self.assertTrue(len(stream_properties) == 1,
-                                msg="There is NOT only one top level breadcrumb for {}".format(stream) +
-                                "\nstream_properties | {}".format(stream_properties))
+                self.assertEqual(len(stream_properties), 1,
+                                 logging='asserting there is only 1 top level breadcrumb in metadata')
 
                 # verify that if there is a replication key we are doing INCREMENTAL otherwise FULL
                 if actual_replication_keys:
-                    self.assertTrue(actual_replication_method == self.INCREMENTAL,
-                                    msg="Expected INCREMENTAL replication "
-                                        "since there is a replication key")
+                    self.assertEqual(
+                        actual_replication_method, self.INCREMENTAL,
+                        logging=f"asserting replication method is {self.INCREMENTAL} when replication keys are defined"
+                    )
                 else:
-                    self.assertTrue(actual_replication_method == self.FULL_TABLE,
-                                    msg="Expected FULL replication "
-                                    "since there is no replication key")
+                    self.assertEqual(
+                        actual_replication_method, self.FULL_TABLE,
+                        logging=f"asserting replication method is {self.FULL_TABLE} when replication keys are not defined"
+                    )
 
                 # verify the actual replication matches our expected replication method
                 self.assertEqual(expected_replication_method, actual_replication_method,
-                                    msg="The actual replication method {} doesn't match the expected {}".format(
-                                        actual_replication_method, expected_replication_method))
+                                 logging=f"asserting replication method is {expected_replication_method}")
 
-                print(stream_properties[0].get(
-                    "metadata", {self.REPLICATION_KEYS: []}))
                 # verify replication key(s)
                 self.assertEqual(expected_replication_keys, actual_replication_keys,
-                                 msg="expected replication key {} but actual is {}".format(
-                                     expected_replication_keys, actual_replication_keys))
+                                 logging=f"asserting replication keys are {expected_replication_keys}")
+
 
                 # verify primary key(s) match expectations
-                self.assertSetEqual(
-                    expected_primary_keys, actual_primary_keys,
-                )
+                self.assertSetEqual(expected_primary_keys, actual_primary_keys,
+                                    logging=f"asserting primary keys are {expected_primary_keys}")
 
                 # verify that primary keys and replication keys
                 # are given the inclusion of automatic in metadata.
-                self.assertSetEqual(expected_automatic_fields,
-                                    actual_automatic_fields)
+                self.assertSetEqual(expected_automatic_fields, actual_automatic_fields,
+                                    logging=f"asserting primary and replication keys {expected_automatic_fields} are automatic")
 
                 # verify that all other fields have inclusion of available
                 # This assumes there are no unsupported fields for SaaS sources
                 self.assertTrue(
                     all({item.get("metadata").get("inclusion") == "available"
                          for item in metadata
                          if item.get("breadcrumb", []) != []
                          and item.get("breadcrumb", ["properties", None])[1]
                          not in actual_automatic_fields}),
-                    msg="Not all non key properties are set to available in metadata")
+                    logging=f"asserting non-key-property fields are available for field selection")
+
 
-    def test_run(self):
-        #Discovery test for standard server
+    def test_standard_discovery(self):
+        """Discovery test for standard server"""
         self.eu_residency = False
         self.discovery_test_run()
 
-        #Discovery test for EU recidency server
+    def test_eu_discovery(self):
+        """Discovery test for EU recidency server"""
         self.eu_residency = True
         self.discovery_test_run()
```

### Comparing `tap-mixpanel-1.4.1/tests/tap_tester/test_pagination.py` & `tap-mixpanel-1.4.2/tests/tap_tester/test_all_fields_pagination.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,56 @@
+from math import ceil
+
 import tap_tester.connections as connections
 import tap_tester.runner as runner
 import tap_tester.menagerie as menagerie
+from tap_tester.logger import LOGGER
+
 from base import TestMixPanelBase
 
 
-class MixPanelPaginationTest(TestMixPanelBase):
-    def name(self):
-        return "mix_panel_pagination_test"
+class MixPanelPaginationAllFieldsTest(TestMixPanelBase):
+
+    @staticmethod
+    def name():
+        return "mixpanel_pagination_all_fields_test"
 
     def pagination_test_run(self):
         """
-        • Verify that for each stream you can get multiple pages of data
+        All Fields Test
         • and that when all fields are selected more than the automatic fields are replicated.
         • Verify no unexpected streams were replicated
         • Verify that more than just the automatic fields are replicated for each stream.
         • verify all fields for each stream are replicated
         • verify that the automatic fields are sent to the target
 
+
+        Pagination Test
+        • Verify that for each stream you can get multiple pages of data
+        • Verify no duplicate pages are replicated
+        • Verify no unexpected streams were replicated
+
         PREREQUISITE
         For EACH stream add enough data that you surpass the limit of a single
         fetch of data.  For instance if you have a limit of 250 records ensure
         that 251 (or more) records have been posted for that stream.
         """
 
         # Only following below 2 streams support pagination
-        streams_to_test = ['engage', 'cohort_members']
-
-        # Streams to verify all fields tests
-        expected_streams = self.expected_streams()
+        streams_to_test_all_fields = self.expected_streams()
+        streams_to_test_pagination = {'engage', 'cohort_members'}
 
         expected_automatic_fields = self.expected_automatic_fields()
         conn_id = connections.ensure_connection(self)
 
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # table and field selection
         test_catalogs_all_fields = [catalog for catalog in found_catalogs
-                                    if catalog.get('tap_stream_id') in expected_streams]
+                                    if catalog.get('tap_stream_id') in streams_to_test_all_fields]
 
         self.perform_and_verify_table_and_field_selection(
             conn_id, test_catalogs_all_fields)
 
         # grab metadata after performing table-and-field selection to set expectations
         # used for asserting all fields are replicated
         stream_to_all_catalog_fields = dict()
@@ -57,29 +67,31 @@
 
         actual_fields_by_stream = runner.examine_target_output_for_fields()
 
         synced_records = runner.get_records_from_target_output()
 
         # Verify no unexpected streams were replicated
         synced_stream_names = set(synced_records.keys())
-        self.assertSetEqual(expected_streams, synced_stream_names)
+        self.assertSetEqual(streams_to_test_all_fields, synced_stream_names)
 
-        for stream in expected_streams:
-            with self.subTest(stream=stream):
+        # All Fields Test
+        for stream in streams_to_test_all_fields:
+            with self.subTest(logging="Primary Functional Test", stream=stream):
 
                 # expected values
-                expected_primary_keys = self.expected_pks()[stream]
                 expected_all_keys = stream_to_all_catalog_fields[stream]
                 expected_automatic_keys = expected_automatic_fields.get(
                     stream, set())
 
                 # collect actual values
                 messages = synced_records.get(stream)
-                actual_all_keys = [set(message['data'].keys()) for message in messages['messages']
-                                   if message['action'] == 'upsert'][0]
+                actual_all_keys = set()
+                for message in messages['messages']:
+                    if message['action'] == 'upsert':
+                        actual_all_keys.update(set(message['data'].keys()))
 
                 # verify that the automatic fields are sent to the target
                 self.assertTrue(
                     actual_fields_by_stream.get(stream, set()).issuperset(
                         expected_automatic_keys),
                     msg="The fields sent to the target don't include all automatic fields")
 
@@ -97,37 +109,55 @@
                     expected_all_keys = expected_all_keys - {'labels', 'sampling_factor', 'dataset', 'mp_reserved_duration_s', 'mp_reserved_origin_end',
                                                              'mp_reserved_origin_start', 'mp_reserved_event_count'}
 
                 # verify all fields for each stream are replicated
                 if not stream == "engage": #Skip engage as it return records in random manner with dynamic fields.
                     self.assertSetEqual(expected_all_keys, actual_all_keys)
 
-                if stream in streams_to_test:
-                    # verify that we can paginate with all fields selected
-                    record_count_sync = record_count_by_stream.get(stream, 0)
-                    self.assertGreater(record_count_sync, self.API_LIMIT,
-                                       msg="The number of records is not over the stream max limit")
-
-                    primary_keys_list = [tuple([message.get('data').get(expected_pk) for expected_pk in expected_primary_keys])
-                                         for message in synced_records.get(stream).get('messages')
-                                         if message.get('action') == 'upsert']
-
-                    if record_count_sync > self.API_LIMIT:
-
-                        primary_keys_list_1 = primary_keys_list[:self.API_LIMIT]
-                        primary_keys_list_2 = primary_keys_list[self.API_LIMIT:2*self.API_LIMIT]
-
-                        primary_keys_page_1 = set(primary_keys_list_1)
-                        primary_keys_page_2 = set(primary_keys_list_2)
-
-                        # Verify by private keys that data is unique for page
-                        self.assertTrue(
-                            primary_keys_page_1.isdisjoint(primary_keys_page_2))
+        # Pagination Test
+        for stream in streams_to_test_pagination:
+            with self.subTest(stream=stream):
+
+                # expected values
+                expected_primary_keys = self.expected_pks()[stream]
+
+                # collect actual values
+                messages = synced_records.get(stream)
+                primary_keys_list = [tuple([message['data'][expected_pk] for expected_pk in expected_primary_keys])
+                                     for message in messages['messages'] if message['action'] == 'upsert']
+
+                # verify that we can paginate with all fields selected
+                record_count_sync = record_count_by_stream.get(stream, 0)
+                self.assertGreater(record_count_sync, self.API_LIMIT,
+                                   msg="The number of records is not over the stream max limit")
+
+
+                # Chunk the replicated records (just primary keys) into expected pages
+                pages = []
+                page_count = ceil(len(primary_keys_list) / self.API_LIMIT)
+                page_size = self.API_LIMIT
+                for page_index in range(page_count):
+                    page_start = page_index * page_size
+                    page_end = (page_index + 1) * page_size
+                    pages.append(set(primary_keys_list[page_start:page_end]))
+
+                # Verify by primary keys that data is unique for each page
+                for current_index, current_page in enumerate(pages):
+                    with self.subTest(current_page_primary_keys=current_page):
+
+                        for other_index, other_page in enumerate(pages):
+                            if current_index == other_index:
+                                continue  # don't compare the page to itself
+
+                            self.assertTrue(
+                                current_page.isdisjoint(other_page), msg=f'other_page_primary_keys={other_page}'
+                            )
 
     def test_run(self):
-        #Pagination test for standard server
+        # Pagination test for standard server
         self.eu_residency = False
         self.pagination_test_run()
 
-        #Pagination test for EU recidency server
+
+        # Pagination test for EU residency server
         self.eu_residency = True
         self.pagination_test_run()
```

### Comparing `tap-mixpanel-1.4.1/tests/tap_tester/test_start_date.py` & `tap-mixpanel-1.4.2/tests/tap_tester/test_start_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from base import TestMixPanelBase
 
 
 class MixPanelStartDateTest(TestMixPanelBase):
     start_date_1 = ""
     start_date_2 = ""
 
-    def name(self):
+    @staticmethod
+    def name():
         return "mix_panel_start_date_test"
 
     def start_date_test_run(self):
         """Instantiate start date according to the desired data set and run the test"""
 
         self.start_date_1 = self.get_properties().get('start_date')
         self.start_date_2 = self.timedelta_formatted(self.start_date_1, days=15)
```

### Comparing `tap-mixpanel-1.4.1/tests/unittests/test_error_handling.py` & `tap-mixpanel-1.4.2/tests/unittests/test_error_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,10 +381,27 @@
     def test_check_access_handle_timeout_error(self, mock_request, mock_sleep):
         '''
         Check whether the request backoffs properly for `check_access` method for 5 times in case of Timeout error.
         '''
         mock_client = client.MixpanelClient(api_secret="mock_api_secret", api_domain="mock_api_domain", request_timeout=REQUEST_TIMEOUT)
         with self.assertRaises(client.ReadTimeoutError):
             mock_client.check_access()
-    
+
         # Verify that requests.Session.request is called 5 times
-        self.assertEqual(mock_request.call_count, 5)
+        self.assertEqual(mock_request.call_count, 5)
+
+
+
+
+class TestMixpanelConnectionResetErrorHandling(unittest.TestCase):
+
+    @mock.patch("requests.Session.request", side_effect=requests.models.ProtocolError)
+    def test_check_access_handle_timeout_error(self, mock_request):
+        '''
+        Check whether the request backoffs properly for `check_access` method for 5 times in case of Timeout error.
+        '''
+        mock_client = client.MixpanelClient(api_secret="mock_api_secret", api_domain="mock_api_domain", request_timeout=REQUEST_TIMEOUT)
+        with self.assertRaises(requests.models.ProtocolError):
+            mock_client.check_access()
+
+        # Verify that requests.Session.request is called 5 times
+        self.assertEqual(mock_request.call_count, 5)
```

### Comparing `tap-mixpanel-1.4.1/tests/unittests/test_medium_client.py` & `tap-mixpanel-1.4.2/tests/unittests/test_medium_client.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tests/unittests/test_request_timeout_param_value.py` & `tap-mixpanel-1.4.2/tests/unittests/test_request_timeout_param_value.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tests/unittests/test_support_eu_endpoints.py` & `tap-mixpanel-1.4.2/tests/unittests/test_support_eu_endpoints.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.1/tests/unittests/test_transform_event_times.py` & `tap-mixpanel-1.4.2/tests/unittests/test_transform_event_times.py`

 * *Files identical despite different names*

