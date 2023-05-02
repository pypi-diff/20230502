# Comparing `tmp/fortigate_api-1.2.3.tar.gz` & `tmp/fortigate_api-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortigate_api-1.2.3.tar", max compression
+gzip compressed data, was "fortigate_api-1.2.4.tar", max compression
```

## Comparing `fortigate_api-1.2.3.tar` & `fortigate_api-1.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      182 2023-04-22 19:54:39.920341 fortigate_api-1.2.3/fortigate_api/__init__.py
--rw-r--r--   0        0        0      371 2023-04-27 14:37:09.194122 fortigate_api-1.2.3/fortigate_api/address.py
--rw-r--r--   0        0        0      394 2023-04-24 14:23:05.431830 fortigate_api-1.2.3/fortigate_api/address_group.py
--rw-r--r--   0        0        0      380 2023-04-24 14:23:05.294154 fortigate_api-1.2.3/fortigate_api/antivirus.py
--rw-r--r--   0        0        0      387 2023-04-24 14:23:05.324135 fortigate_api-1.2.3/fortigate_api/application.py
--rw-r--r--   0        0        0     8427 2023-04-24 14:23:05.461818 fortigate_api-1.2.3/fortigate_api/base.py
--rw-r--r--   0        0        0     9884 2023-04-22 19:54:39.939001 fortigate_api-1.2.3/fortigate_api/ccp.py
--rw-r--r--   0        0        0     1851 2023-04-24 14:23:05.273914 fortigate_api-1.2.3/fortigate_api/dhcp_server.py
--rw-r--r--   0        0        0     7997 2023-04-27 05:52:33.482301 fortigate_api-1.2.3/fortigate_api/extended_filters.py
--rw-r--r--   0        0        0      418 2023-04-24 14:23:05.401820 fortigate_api-1.2.3/fortigate_api/external_resource.py
--rw-r--r--   0        0        0    15118 2023-04-27 14:24:49.223872 fortigate_api-1.2.3/fortigate_api/fortigate.py
--rw-r--r--   0        0        0     4494 2023-04-24 14:18:26.735329 fortigate_api-1.2.3/fortigate_api/fortigate_api.py
--rw-r--r--   0        0        0     9009 2023-04-22 19:54:39.958643 fortigate_api-1.2.3/fortigate_api/helpers.py
--rw-r--r--   0        0        0     1456 2023-04-24 14:23:05.280313 fortigate_api-1.2.3/fortigate_api/interface.py
--rw-r--r--   0        0        0      415 2023-04-24 14:23:05.394817 fortigate_api-1.2.3/fortigate_api/internet_service.py
--rw-r--r--   0        0        0      369 2023-04-24 14:23:05.238970 fortigate_api-1.2.3/fortigate_api/ip_pool.py
--rw-r--r--   0        0        0     3266 2023-04-27 10:18:44.889532 fortigate_api-1.2.3/fortigate_api/policy.py
--rw-r--r--   0        0        0        0 2022-07-14 18:32:10.557000 fortigate_api-1.2.3/fortigate_api/py.typed
--rw-r--r--   0        0        0      384 2023-04-24 14:23:05.382817 fortigate_api-1.2.3/fortigate_api/schedule.py
--rw-r--r--   0        0        0      378 2023-04-24 14:23:05.248330 fortigate_api-1.2.3/fortigate_api/service.py
--rw-r--r--   0        0        0      415 2023-04-24 14:23:05.375819 fortigate_api-1.2.3/fortigate_api/service_category.py
--rw-r--r--   0        0        0      400 2023-04-24 14:23:05.317116 fortigate_api-1.2.3/fortigate_api/service_group.py
--rw-r--r--   0        0        0     1315 2023-04-24 14:23:05.254332 fortigate_api-1.2.3/fortigate_api/snmp_community.py
--rw-r--r--   0        0        0     3347 2023-04-22 19:54:39.983169 fortigate_api-1.2.3/fortigate_api/ssh.py
--rw-r--r--   0        0        0      765 2023-04-27 14:24:49.224875 fortigate_api-1.2.3/fortigate_api/types_.py
--rw-r--r--   0        0        0      378 2023-04-24 14:23:05.306114 fortigate_api-1.2.3/fortigate_api/virtual_ip.py
--rw-r--r--   0        0        0      354 2023-04-24 14:23:05.388817 fortigate_api-1.2.3/fortigate_api/zone.py
--rw-r--r--   0        0        0     1091 2022-07-14 18:32:10.542000 fortigate_api-1.2.3/LICENSE.txt
--rw-r--r--   0        0        0     1611 2023-04-27 14:24:49.226871 fortigate_api-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    43039 2023-04-27 14:39:37.781191 fortigate_api-1.2.3/README.rst
--rw-r--r--   0        0        0    43520 1970-01-01 00:00:00.000000 fortigate_api-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      182 2023-04-22 19:54:39.920341 fortigate_api-1.2.4/fortigate_api/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-02 14:54:38.999252 fortigate_api-1.2.4/fortigate_api/address.py
+-rw-r--r--   0        0        0      394 2023-04-24 14:23:05.431830 fortigate_api-1.2.4/fortigate_api/address_group.py
+-rw-r--r--   0        0        0      380 2023-04-24 14:23:05.294154 fortigate_api-1.2.4/fortigate_api/antivirus.py
+-rw-r--r--   0        0        0      387 2023-04-24 14:23:05.324135 fortigate_api-1.2.4/fortigate_api/application.py
+-rw-r--r--   0        0        0     8427 2023-05-02 15:16:32.213086 fortigate_api-1.2.4/fortigate_api/base.py
+-rw-r--r--   0        0        0     9884 2023-04-22 19:54:39.939001 fortigate_api-1.2.4/fortigate_api/ccp.py
+-rw-r--r--   0        0        0     1851 2023-04-24 14:23:05.273914 fortigate_api-1.2.4/fortigate_api/dhcp_server.py
+-rw-r--r--   0        0        0     7997 2023-05-02 15:27:10.225589 fortigate_api-1.2.4/fortigate_api/extended_filters.py
+-rw-r--r--   0        0        0      418 2023-04-24 14:23:05.401820 fortigate_api-1.2.4/fortigate_api/external_resource.py
+-rw-r--r--   0        0        0    15235 2023-05-02 15:38:13.367533 fortigate_api-1.2.4/fortigate_api/fortigate.py
+-rw-r--r--   0        0        0     4494 2023-04-24 14:18:26.735329 fortigate_api-1.2.4/fortigate_api/fortigate_api.py
+-rw-r--r--   0        0        0     9009 2023-04-22 19:54:39.958643 fortigate_api-1.2.4/fortigate_api/helpers.py
+-rw-r--r--   0        0        0     1456 2023-04-24 14:23:05.280313 fortigate_api-1.2.4/fortigate_api/interface.py
+-rw-r--r--   0        0        0      415 2023-04-24 14:23:05.394817 fortigate_api-1.2.4/fortigate_api/internet_service.py
+-rw-r--r--   0        0        0      369 2023-04-24 14:23:05.238970 fortigate_api-1.2.4/fortigate_api/ip_pool.py
+-rw-r--r--   0        0        0     3266 2023-04-27 10:18:44.889532 fortigate_api-1.2.4/fortigate_api/policy.py
+-rw-r--r--   0        0        0        0 2022-07-14 18:32:10.557000 fortigate_api-1.2.4/fortigate_api/py.typed
+-rw-r--r--   0        0        0      384 2023-04-24 14:23:05.382817 fortigate_api-1.2.4/fortigate_api/schedule.py
+-rw-r--r--   0        0        0      378 2023-04-24 14:23:05.248330 fortigate_api-1.2.4/fortigate_api/service.py
+-rw-r--r--   0        0        0      415 2023-04-24 14:23:05.375819 fortigate_api-1.2.4/fortigate_api/service_category.py
+-rw-r--r--   0        0        0      400 2023-04-24 14:23:05.317116 fortigate_api-1.2.4/fortigate_api/service_group.py
+-rw-r--r--   0        0        0     1315 2023-04-24 14:23:05.254332 fortigate_api-1.2.4/fortigate_api/snmp_community.py
+-rw-r--r--   0        0        0     3347 2023-04-22 19:54:39.983169 fortigate_api-1.2.4/fortigate_api/ssh.py
+-rw-r--r--   0        0        0      765 2023-04-27 14:24:49.224875 fortigate_api-1.2.4/fortigate_api/types_.py
+-rw-r--r--   0        0        0      378 2023-04-24 14:23:05.306114 fortigate_api-1.2.4/fortigate_api/virtual_ip.py
+-rw-r--r--   0        0        0      354 2023-04-24 14:23:05.388817 fortigate_api-1.2.4/fortigate_api/zone.py
+-rw-r--r--   0        0        0     1091 2022-07-14 18:32:10.542000 fortigate_api-1.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     1611 2023-05-02 13:49:33.388197 fortigate_api-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    43135 2023-05-02 15:22:05.376297 fortigate_api-1.2.4/README.rst
+-rw-r--r--   0        0        0    43613 1970-01-01 00:00:00.000000 fortigate_api-1.2.4/PKG-INFO
```

### Comparing `fortigate_api-1.2.3/fortigate_api/base.py` & `fortigate_api-1.2.4/fortigate_api/base.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/ccp.py` & `fortigate_api-1.2.4/fortigate_api/ccp.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/dhcp_server.py` & `fortigate_api-1.2.4/fortigate_api/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/extended_filters.py` & `fortigate_api-1.2.4/fortigate_api/extended_filters.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/fortigate.py` & `fortigate_api-1.2.4/fortigate_api/fortigate.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from __future__ import annotations
 
 import json
 import logging
 import re
 from typing import Callable, Iterable, Optional
-from urllib.parse import urlencode
+from urllib.parse import urlencode, urljoin
 
 import requests
 from requests import Session, Response
 from requests.exceptions import SSLError
 from requests.packages import urllib3  # type: ignore
 
 from fortigate_api import helpers as h
@@ -419,12 +419,15 @@
         try:
             response: Response = method_(**params)
         except Exception as ex:
             raise self._hide_secret_ex(ex)
         return response
 
     def _valid_url(self, url: str) -> str:
-        """Add "https://" to `url` if absent."""
+        """Return a valid URL string.
+
+        Add "https://" to `url` if it is absent and remove any trailing "/" character.
+        """
         if re.match("http(s)?://", url):
-            return url
-        url = url.strip("/")
-        return f"{self.url}/{url}/"
+            return url.rstrip("/")
+        path = url.strip("/")
+        return urljoin(self.url, path)
```

### Comparing `fortigate_api-1.2.3/fortigate_api/fortigate_api.py` & `fortigate_api-1.2.4/fortigate_api/fortigate_api.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/helpers.py` & `fortigate_api-1.2.4/fortigate_api/helpers.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/interface.py` & `fortigate_api-1.2.4/fortigate_api/interface.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/policy.py` & `fortigate_api-1.2.4/fortigate_api/policy.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/snmp_community.py` & `fortigate_api-1.2.4/fortigate_api/snmp_community.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/ssh.py` & `fortigate_api-1.2.4/fortigate_api/ssh.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/fortigate_api/types_.py` & `fortigate_api-1.2.4/fortigate_api/types_.py`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/LICENSE.txt` & `fortigate_api-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortigate_api-1.2.3/pyproject.toml` & `fortigate_api-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fortigate_api"
-version = "1.2.3"
+version = "1.2.4"
 description = "Python package to configure Fortigate (Fortios) devices using REST API and SSH"
 authors = ["Vladimir Prusakov <vladimir.prusakovs@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/vladimirs-git/fortigate-api"
 repository = "https://github.com/vladimirs-git/fortigate-api"
 readme = "README.rst"
 keywords = ["fortigate", "api", "fortios", "firewall", "networking", "telecommunication"]
@@ -40,8 +40,8 @@
 types-requests = "2.28.11.17"
 
 [tool.poetry.extras]
 test = ["pytest"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/vladimirs-git/fortigate-api/issues"
-"Download URL" = "https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.3.tar.gz"
+"Download URL" = "https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.4.tar.gz"
```

### Comparing `fortigate_api-1.2.3/README.rst` & `fortigate_api-1.2.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.3.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.4.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
 
@@ -862,14 +862,16 @@
 to work with any objects available through the REST API. `Fortigate`_ is useful for working with
 objects that are not implemented in `FortigateAPI`_
 
 Python examples `./examples/fortigate.py`_
 
 Python examples `./examples/fortigate_token.py`_
 
+Python examples `./examples/monitor.py`_
+
 .. code:: python
 
     from fortigate_api import Fortigate
 
     fgt = Fortigate(host="host", username="username", password="password")
 
     # Create address in the Fortigate
@@ -1080,20 +1082,21 @@
 .. _`./examples/yml/service_category.yml`: ./examples/yml/service_category.yml
 .. _`./examples/yml/service_group.yml`: ./examples/yml/service_group.yml
 .. _`./examples/yml/snmp_community.yml`: ./examples/yml/snmp_community.yml
 .. _`./examples/yml/virtual_ip.yml`: ./examples/yml/virtual_ip.yml
 .. _`./examples/yml/zone.yml`: ./examples/yml/zone.yml
 
 .. _`./examples/address.py`: ./examples/address.py
-.. _`./examples/address_token.py`: ./examples/address_token.py
 .. _`./examples/address_group.py`: ./examples/address_group.py
+.. _`./examples/address_token.py`: ./examples/address_token.py
 .. _`./examples/dhcp_server.py`: ./examples/dhcp_server.py
 .. _`./examples/external_resource.py`: ./examples/external_resource.py
 .. _`./examples/fortigate.py`: ./examples/fortigate.py
 .. _`./examples/fortigate_token.py`: ./examples/fortigate_token.py
 .. _`./examples/interface.py`: ./examples/interface.py
 .. _`./examples/ip_pool.py`: ./examples/ip_pool.py
+.. _`./examples/monitor.py`: ./examples/monitor.py
 .. _`./examples/policy.py`: ./examples/policy.py
 .. _`./examples/policy_extended_filter.py`: ./examples/policy_extended_filter.py
 .. _`./examples/snmp_community.py`: ./examples/snmp_community.py
 .. _`./examples/ssh.py`: ./examples/ssh.py
 .. _`./examples/ssh_vdom.py`: ./examples/ssh_vdom.py
```

### Comparing `fortigate_api-1.2.3/PKG-INFO` & `fortigate_api-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortigate-api
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python package to configure Fortigate (Fortios) devices using REST API and SSH
 Home-page: https://github.com/vladimirs-git/fortigate-api
 License: MIT
 Keywords: fortigate,api,fortios,firewall,networking,telecommunication
 Author: Vladimir Prusakov
 Author-email: vladimir.prusakovs@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Networking :: Firewalls
 Provides-Extra: test
 Requires-Dist: ciscoconfparse (>=1.7,<2.0)
 Requires-Dist: netmiko (>=4.1,<5.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Project-URL: Bug Tracker, https://github.com/vladimirs-git/fortigate-api/issues
-Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.3.tar.gz
+Project-URL: Download URL, https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.4.tar.gz
 Project-URL: Repository, https://github.com/vladimirs-git/fortigate-api
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://img.shields.io/pypi/v/fortigate-api.svg
    :target: https://pypi.python.org/pypi/fortigate-api
 .. image:: https://img.shields.io/pypi/pyversions/fortigate-api.svg
@@ -79,15 +79,15 @@
 
     pip install fortigate-api
 
 or install the package from github.com release
 
 .. code:: bash
 
-    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.3.tar.gz
+    pip install https://github.com/vladimirs-git/fortigate-api/archive/refs/tags/1.2.4.tar.gz
 
 or install the package from github.com repository
 
 .. code:: bash
 
     pip install git+https://github.com/vladimirs-git/fortigate-api
 
@@ -896,14 +896,16 @@
 to work with any objects available through the REST API. `Fortigate`_ is useful for working with
 objects that are not implemented in `FortigateAPI`_
 
 Python examples `./examples/fortigate.py`_
 
 Python examples `./examples/fortigate_token.py`_
 
+Python examples `./examples/monitor.py`_
+
 .. code:: python
 
     from fortigate_api import Fortigate
 
     fgt = Fortigate(host="host", username="username", password="password")
 
     # Create address in the Fortigate
@@ -1114,21 +1116,22 @@
 .. _`./examples/yml/service_category.yml`: ./examples/yml/service_category.yml
 .. _`./examples/yml/service_group.yml`: ./examples/yml/service_group.yml
 .. _`./examples/yml/snmp_community.yml`: ./examples/yml/snmp_community.yml
 .. _`./examples/yml/virtual_ip.yml`: ./examples/yml/virtual_ip.yml
 .. _`./examples/yml/zone.yml`: ./examples/yml/zone.yml
 
 .. _`./examples/address.py`: ./examples/address.py
-.. _`./examples/address_token.py`: ./examples/address_token.py
 .. _`./examples/address_group.py`: ./examples/address_group.py
+.. _`./examples/address_token.py`: ./examples/address_token.py
 .. _`./examples/dhcp_server.py`: ./examples/dhcp_server.py
 .. _`./examples/external_resource.py`: ./examples/external_resource.py
 .. _`./examples/fortigate.py`: ./examples/fortigate.py
 .. _`./examples/fortigate_token.py`: ./examples/fortigate_token.py
 .. _`./examples/interface.py`: ./examples/interface.py
 .. _`./examples/ip_pool.py`: ./examples/ip_pool.py
+.. _`./examples/monitor.py`: ./examples/monitor.py
 .. _`./examples/policy.py`: ./examples/policy.py
 .. _`./examples/policy_extended_filter.py`: ./examples/policy_extended_filter.py
 .. _`./examples/snmp_community.py`: ./examples/snmp_community.py
 .. _`./examples/ssh.py`: ./examples/ssh.py
 .. _`./examples/ssh_vdom.py`: ./examples/ssh_vdom.py
```

