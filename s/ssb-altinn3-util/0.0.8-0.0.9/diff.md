# Comparing `tmp/ssb_altinn3_util-0.0.8.tar.gz` & `tmp/ssb_altinn3_util-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn3_util-0.0.8.tar", last modified: Tue May 31 11:12:26 2022, max compression
+gzip compressed data, was "ssb_altinn3_util-0.0.9.tar", last modified: Thu Jun  2 12:25:10 2022, max compression
```

## Comparing `ssb_altinn3_util-0.0.8.tar` & `ssb_altinn3_util-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.655688 ssb_altinn3_util-0.0.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-05-31 11:12:26.655688 ssb_altinn3_util-0.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1526 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      591 2022-05-31 11:12:26.655688 ssb_altinn3_util-0.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.647688 ssb_altinn3_util-0.0.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.651688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.651688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.651688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3961 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/altinn_api_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.651688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/api/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/api/application.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1695 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/api/storage.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.651688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1806 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/altinn_auth_client.py
--rw-r--r--   0 vsts      (1001) docker     (121)      841 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/altinn_auth_client_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.655688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      694 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/altinn_client.py
--rw-r--r--   0 vsts      (1001) docker     (121)      811 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/guardian_client.py
--rw-r--r--   0 vsts      (1001) docker     (121)      713 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/http_helper.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1031 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/keycloak_client.py
--rw-r--r--   0 vsts      (1001) docker     (121)      728 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/secret_manager_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.655688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/decorators/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/decorators/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      401 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/decorators/simple_exception_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.655688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/gcp/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/gcp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1525 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/gcp/publisher.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1967 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/gcp/subscriber_thread.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.655688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/models/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      769 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/models/altinn3_cloud_event.py
--rw-r--r--   0 vsts      (1001) docker     (121)      215 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/models/basic_file.py
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-31 11:12:15.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-31 11:12:26.651688 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-05-31 11:12:26.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1536 2022-05-31 11:12:26.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-31 11:12:26.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       57 2022-05-31 11:12:26.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       17 2022-05-31 11:12:26.000000 ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.297974 ssb_altinn3_util-0.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-06-02 12:25:10.297974 ssb_altinn3_util-0.0.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1526 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)      591 2022-06-02 12:25:10.297974 ssb_altinn3_util-0.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      941 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3961 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/altinn_api_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/api/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/api/application.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1695 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/api/storage.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1806 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/altinn_auth_client.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      841 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/altinn_auth_client_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      694 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/altinn_client.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      811 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/guardian_client.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      713 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/http_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1031 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/keycloak_client.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      728 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/secret_manager_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/decorators/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/decorators/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      401 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/decorators/simple_exception_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/gcp/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/gcp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1525 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/gcp/publisher.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1967 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/gcp/subscriber_thread.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.297974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/database/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/database/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      613 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/database/altinn_mottak_db_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5151 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/database/crud.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1562 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/database/schema.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      358 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/database/wireup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.297974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/models/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      769 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/models/altinn3_cloud_event.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      215 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/models/basic_file.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-02 12:25:02.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-02 12:25:10.293974 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-06-02 12:25:10.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1754 2022-06-02 12:25:10.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-02 12:25:10.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       77 2022-06-02 12:25:10.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       17 2022-06-02 12:25:10.000000 ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/top_level.txt
```

### Comparing `ssb_altinn3_util-0.0.8/PKG-INFO` & `ssb_altinn3_util-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb_altinn3_util
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small library package containing various tools and utilities
 Home-page: https://github.com/statisticsnorway/ssb-altinn3-util
 Author: Team Cumulus
 Author-email: nhk@ssb.no, lrb@ssb.no, gij@ssb.no, kuv@ssb.no
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssb_altinn3_util-0.0.8/README.md` & `ssb_altinn3_util-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/setup.cfg` & `ssb_altinn3_util-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/setup.py` & `ssb_altinn3_util-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ssb_altinn3_util",
-    version="0.0.8",
+    version="0.0.9",
     author="Team Cumulus",
     author_email="nhk@ssb.no, lrb@ssb.no, gij@ssb.no, kuv@ssb.no",
     description="A small library package containing various tools and utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/statisticsnorway/ssb-altinn3-util",
     project_urls={
@@ -20,12 +20,14 @@
     ],
     package_data={"": ["py.typed"]},
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         'google-cloud-pubsub',
         'google-cloud-secret-manager',
-        'pydantic'
+        'pydantic',
+        'sqlalchemy',
+        'psycopg2'
     ],
 
     python_requires=">=3.6",
 )
```

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/altinn_api_client.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/altinn_api_client.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/altinn/api/storage.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/altinn/api/storage.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/altinn_auth_client.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/altinn_auth_client.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/altinn_auth_client_config.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/altinn_auth_client_config.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/altinn_client.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/altinn_client.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/guardian_client.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/guardian_client.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/http_helper.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/keycloak_client.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/keycloak_client.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/auth/helpers/secret_manager_client.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/auth/helpers/secret_manager_client.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/gcp/publisher.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/gcp/publisher.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/clients/gcp/subscriber_thread.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/clients/gcp/subscriber_thread.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util/models/altinn3_cloud_event.py` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util/models/altinn3_cloud_event.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/PKG-INFO` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn3-util
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small library package containing various tools and utilities
 Home-page: https://github.com/statisticsnorway/ssb-altinn3-util
 Author: Team Cumulus
 Author-email: nhk@ssb.no, lrb@ssb.no, gij@ssb.no, kuv@ssb.no
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssb_altinn3_util-0.0.8/src/ssb_altinn3_util.egg-info/SOURCES.txt` & `ssb_altinn3_util-0.0.9/src/ssb_altinn3_util.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,10 +24,15 @@
 src/ssb_altinn3_util/clients/auth/helpers/keycloak_client.py
 src/ssb_altinn3_util/clients/auth/helpers/secret_manager_client.py
 src/ssb_altinn3_util/clients/decorators/__init__.py
 src/ssb_altinn3_util/clients/decorators/simple_exception_wrapper.py
 src/ssb_altinn3_util/clients/gcp/__init__.py
 src/ssb_altinn3_util/clients/gcp/publisher.py
 src/ssb_altinn3_util/clients/gcp/subscriber_thread.py
+src/ssb_altinn3_util/database/__init__.py
+src/ssb_altinn3_util/database/altinn_mottak_db_adapter.py
+src/ssb_altinn3_util/database/crud.py
+src/ssb_altinn3_util/database/schema.py
+src/ssb_altinn3_util/database/wireup.py
 src/ssb_altinn3_util/models/__init__.py
 src/ssb_altinn3_util/models/altinn3_cloud_event.py
 src/ssb_altinn3_util/models/basic_file.py
```

