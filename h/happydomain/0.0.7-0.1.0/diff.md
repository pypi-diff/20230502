# Comparing `tmp/happydomain-0.0.7.tar.gz` & `tmp/happydomain-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happydomain-0.0.7.tar", last modified: Mon Apr 17 10:32:07 2023, max compression
+gzip compressed data, was "happydomain-0.1.0.tar", last modified: Tue May  2 18:40:45 2023, max compression
```

## Comparing `happydomain-0.0.7.tar` & `happydomain-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:32:07.138746 happydomain-0.0.7/
--rw-r--r--   0 root         (0) root         (0)    21781 2023-04-17 10:31:18.000000 happydomain-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-17 10:32:07.134746 happydomain-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-17 10:31:18.000000 happydomain-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:32:07.122747 happydomain-0.0.7/happydomain/
--rw-r--r--   0 root         (0) root         (0)     1667 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/admin.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/api.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/authuser.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/domain.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/error.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/provider.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/service.py
--rw-r--r--   0 root         (0) root         (0)     3699 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:32:07.134746 happydomain-0.0.7/happydomain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-17 10:31:18.000000 happydomain-0.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 10:32:07.138746 happydomain-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-17 10:31:18.000000 happydomain-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:40:45.337999 happydomain-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)    21781 2023-05-02 18:39:56.000000 happydomain-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-02 18:40:45.333999 happydomain-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-02 18:39:56.000000 happydomain-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:40:45.322000 happydomain-0.1.0/happydomain/
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/admin.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/api.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/authuser.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/domain.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/error.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/provider.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/service.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2023-05-02 18:39:56.000000 happydomain-0.1.0/happydomain/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 18:40:45.333999 happydomain-0.1.0/happydomain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-02 18:40:44.000000 happydomain-0.1.0/happydomain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-05-02 18:40:44.000000 happydomain-0.1.0/happydomain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 18:40:44.000000 happydomain-0.1.0/happydomain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-02 18:40:44.000000 happydomain-0.1.0/happydomain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-02 18:40:44.000000 happydomain-0.1.0/happydomain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      894 2023-05-02 18:39:56.000000 happydomain-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 18:40:45.337999 happydomain-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-05-02 18:39:56.000000 happydomain-0.1.0/setup.py
```

### Comparing `happydomain-0.0.7/LICENSE` & `happydomain-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.7/PKG-INFO` & `happydomain-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.7
+Version: 0.1.0
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.7/happydomain/__init__.py` & `happydomain-0.1.0/happydomain/__init__.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.7/happydomain/admin.py` & `happydomain-0.1.0/happydomain/admin.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.7/happydomain/api.py` & `happydomain-0.1.0/happydomain/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             raise HappyError(r.status_code, **json.loads(r.text))
 
         ret = []
         val = json.loads(r.text)
 
         if val is not None:
             for au in val:
-                ret.append(Domain(self, **au))
+                ret.append(Domain(self, zone_history_are_ids=True, **au))
 
         return ret
 
     # Providers
 
     def provider_list(self):
         r = self.session.get(
```

### Comparing `happydomain-0.0.7/happydomain/authuser.py` & `happydomain-0.1.0/happydomain/authuser.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.7/happydomain/domain.py` & `happydomain-0.1.0/happydomain/domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import json
 from urllib.parse import quote
 
 from .error import HappyError
-from .zone import ZoneMeta, Zone
+from .zone import UncompleteZoneMeta, ZoneMeta, Zone
 
 class Domain:
 
-    def __init__(self, _session, id, id_owner, id_provider, domain, zone_history, group=""):
+    def __init__(self, _session, id, id_owner, id_provider, domain, zone_history, zone_history_are_ids=False, group=""):
         self._session = _session
 
         self.id = id
         self.id_owner = id_owner
         self.id_provider = id_provider
         self.domain = domain
         self.group = group
-        self.zone_history = zone_history if zone_history is not None else []
+        if zone_history_are_ids:
+            self.zone_history = [UncompleteZoneMeta(self, zid) for zid in zone_history]
+        else:
+            self.zone_history = zone_history if zone_history is not None else []
 
     def _dumps(self):
         return json.dumps({
             "id": self.id,
             "id_owner": self.id_owner,
             "id_provider": self.id_provider,
             "domain": self.domain,
```

### Comparing `happydomain-0.0.7/happydomain/provider.py` & `happydomain-0.1.0/happydomain/provider.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.7/happydomain/service.py` & `happydomain-0.1.0/happydomain/service.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.7/happydomain.egg-info/PKG-INFO` & `happydomain-0.1.0/happydomain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.7
+Version: 0.1.0
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.7/pyproject.toml` & `happydomain-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "happydomain"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="happyDomain's team", email="contact+pypi@happydomain.org" },
 ]
 description = "Finally a simple interface for domain names."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `happydomain-0.0.7/setup.py` & `happydomain-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from glob import glob
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.0.7"
+version = "0.1.0"
 
 setup(
     name = "happydomain",
     version = version,
     description = "Finally a simple interface for domain names.",
     long_description = open('README.md').read(),
```

