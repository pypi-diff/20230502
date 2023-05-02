# Comparing `tmp/swiftshadow-0.2.0.tar.gz` & `tmp/swiftshadow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.2.0.tar", last modified: Thu Apr 27 09:54:34 2023, max compression
+gzip compressed data, was "swiftshadow-0.2.1.tar", last modified: Tue May  2 05:53:29 2023, max compression
```

## Comparing `swiftshadow-0.2.0.tar` & `swiftshadow-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-27 09:54:20.000000 swiftshadow-0.2.0/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:54:34.165935 swiftshadow-0.2.0/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 09:54:34.000000 swiftshadow-0.2.0/swiftshadow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/swiftshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/swiftshadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/swiftshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.2.0/LICENSE` & `swiftshadow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.0/PKG-INFO` & `swiftshadow-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `swiftshadow-0.2.0/README.md` & `swiftshadow-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.0/setup.py` & `swiftshadow-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     name="swiftshadow",
     author="Sachin Sankar",
     author_email="mail.sachinsankar@gmail.com",
     url="https://github.com/sachin-sankar/swiftshadow",
     description="Free IP Proxy rotator for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version=VERSION.get("__version__", "0.2.0"),
+    version=VERSION.get("__version__", "0.2.1"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.2.0/swiftshadow/constants.py` & `swiftshadow-0.2.1/swiftshadow/constants.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.0/swiftshadow/helpers.py` & `swiftshadow-0.2.1/swiftshadow/helpers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.0/swiftshadow/providers.py` & `swiftshadow-0.2.1/swiftshadow/providers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.0/swiftshadow/swiftshadow.py` & `swiftshadow-0.2.1/swiftshadow/swiftshadow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from requests import get
 from random import choice
 from datetime import datetime, timezone, timedelta
-from pickle import dump, load
+from json import dump, load
 from swiftshadow.helpers import log
 from swiftshadow.providers import Proxyscrape, Scrapingant
 import swiftshadow.cache as cache
 
 
 class Proxy:
     def __init__(
@@ -22,15 +22,15 @@
         Proxy class contains all necessary methods required to use swiftshadow.
 
         Args:
                 countries: ISO 3166-2 Two letter country codes to filter proxies.
                 protocol: HTTP/HTTPS protocol to filter proxies.
                 maxProxies: Maximum number of proxies to store and rotate from.
                 autoRotate: Rotates proxy when `Proxy.proxy()` function is called.
-                cachePeriod: Time to cache proxies in minutes.
+                cachePeriod: Time to cache proxies in seconds.
 
         Returns:
                 proxyClass (swiftshadow.Proxy): `swiftshadow.Proxy` class instance
 
         Examples:
                 Simplest way to get a proxy
                 >>> from swiftshadow.swiftshadow import Proxy
@@ -41,14 +41,15 @@
                 Proxies are sourced from **Proxyscrape** and **Scrapingant** websites which are freely available and validated locally.
         """
         self.countries = [i.upper() for i in countries]
         self.protocol = protocol
         self.maxProxies = maxProxies
         self.autoRotate = autoRotate
         self.cachePeriod = cachePeriod
+
         self.update()
 
     def checkIp(self, ip, cc, protocol):
         if (ip[1] == cc or cc == None) and ip[2] == protocol:
             proxy = {ip[2]: ip[0]}
             try:
                 oip = get(f"{protocol}://ipinfo.io/ip", proxies=proxy).text
@@ -59,17 +60,17 @@
             else:
                 return False
         else:
             return False
 
     def update(self):
         try:
-            with open(".swiftshadow.dat", "rb") as file:
+            with open(".swiftshadow.json", "r") as file:
                 data = load(file)
-                self.expiry = data[0]
+                self.expiry = datetime.fromisoformat(data[0])
                 expired = cache.checkExpiry(self.expiry)
             if not expired:
                 log(
                     "info",
                     f"Loaded proxies from cache",
                 )
                 self.proxies = data[1]
@@ -91,16 +92,16 @@
             )
         if len(self.proxies) == 0:
             log(
                 "warn",
                 "No proxies found for current settings. To prevent runtime error updating the proxy list again.",
             )
             self.update()
-        with open(".swiftshadow.dat", "wb") as file:
-            dump([cache.getExpiry(self.cachePeriod), self.proxies], file)
+        with open(".swiftshadow.json", "w") as file:
+            dump([cache.getExpiry(self.cachePeriod).isoformat(), self.proxies], file)
         self.current = self.proxies[0]
 
     def rotate(self):
         """
         Rotate the current proxy.
 
         Sets the current proxy to a random one from available proxies and also validates cache.
@@ -121,15 +122,7 @@
         """
         if cache.checkExpiry(self.expiry):
             self.update()
         if self.autoRotate == True:
             return choice(self.proxies)
         else:
             return self.current
-
-
-from time import sleep
-
-a = Proxy(cachePeriod=1, maxProxies=1)
-while True:
-    print(a.proxy())
-    sleep(1)
```

### Comparing `swiftshadow-0.2.0/swiftshadow.egg-info/PKG-INFO` & `swiftshadow-0.2.1/swiftshadow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

