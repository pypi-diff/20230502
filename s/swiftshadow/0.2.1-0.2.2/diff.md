# Comparing `tmp/swiftshadow-0.2.1.tar.gz` & `tmp/swiftshadow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.2.1.tar", last modified: Tue May  2 05:53:29 2023, max compression
+gzip compressed data, was "swiftshadow-0.2.2.tar", last modified: Tue May  2 06:54:21 2023, max compression
```

## Comparing `swiftshadow-0.2.1.tar` & `swiftshadow-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-02 05:53:16.000000 swiftshadow-0.2.1/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:53:29.826251 swiftshadow-0.2.1/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 05:53:29.000000 swiftshadow-0.2.1/swiftshadow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:54:21.390941 swiftshadow-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 06:54:21.386941 swiftshadow-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 06:54:21.390941 swiftshadow-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:54:21.386941 swiftshadow-0.2.2/swiftshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/swiftshadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:54:21.386941 swiftshadow-0.2.2/swiftshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.2.1/LICENSE` & `swiftshadow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.1/PKG-INFO` & `swiftshadow-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `swiftshadow-0.2.1/README.md` & `swiftshadow-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.1/setup.py` & `swiftshadow-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     name="swiftshadow",
     author="Sachin Sankar",
     author_email="mail.sachinsankar@gmail.com",
     url="https://github.com/sachin-sankar/swiftshadow",
     description="Free IP Proxy rotator for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version=VERSION.get("__version__", "0.2.1"),
+    version=VERSION.get("__version__", "0.2.2"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.2.1/swiftshadow/constants.py` & `swiftshadow-0.2.2/swiftshadow/constants.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.1/swiftshadow/providers.py` & `swiftshadow-0.2.2/swiftshadow/providers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.1/swiftshadow/swiftshadow.py` & `swiftshadow-0.2.2/swiftshadow/swiftshadow.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         Proxy class contains all necessary methods required to use swiftshadow.
 
         Args:
                 countries: ISO 3166-2 Two letter country codes to filter proxies.
                 protocol: HTTP/HTTPS protocol to filter proxies.
                 maxProxies: Maximum number of proxies to store and rotate from.
                 autoRotate: Rotates proxy when `Proxy.proxy()` function is called.
-                cachePeriod: Time to cache proxies in seconds.
+                cachePeriod: Time to cache proxies in minutes.
 
         Returns:
                 proxyClass (swiftshadow.Proxy): `swiftshadow.Proxy` class instance
 
         Examples:
                 Simplest way to get a proxy
                 >>> from swiftshadow.swiftshadow import Proxy
@@ -62,22 +62,23 @@
         else:
             return False
 
     def update(self):
         try:
             with open(".swiftshadow.json", "r") as file:
                 data = load(file)
-                self.expiry = datetime.fromisoformat(data[0])
+                self.expiry = data[0]
                 expired = cache.checkExpiry(self.expiry)
             if not expired:
                 log(
                     "info",
                     f"Loaded proxies from cache",
                 )
                 self.proxies = data[1]
+                self.expiry = data[0]
                 self.current = self.proxies[0]
                 return
             else:
                 log(
                     "info",
                     f"Cache expired. Updating cache...",
                 )
@@ -88,20 +89,21 @@
         self.proxies.extend(Proxyscrape(self.maxProxies, self.countries, self.protocol))
         if len(self.proxies) != self.maxProxies:
             self.proxies.extend(
                 Scrapingant(self.maxProxies, self.countries, self.protocol)
             )
         if len(self.proxies) == 0:
             log(
-                "warn",
+                "warning",
                 "No proxies found for current settings. To prevent runtime error updating the proxy list again.",
             )
             self.update()
         with open(".swiftshadow.json", "w") as file:
-            dump([cache.getExpiry(self.cachePeriod).isoformat(), self.proxies], file)
+            self.expiry = cache.getExpiry(self.cachePeriod).isoformat()
+            dump([self.expiry, self.proxies], file)
         self.current = self.proxies[0]
 
     def rotate(self):
         """
         Rotate the current proxy.
 
         Sets the current proxy to a random one from available proxies and also validates cache.
```

### Comparing `swiftshadow-0.2.1/swiftshadow.egg-info/PKG-INFO` & `swiftshadow-0.2.2/swiftshadow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

