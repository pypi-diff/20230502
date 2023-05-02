# Comparing `tmp/inori-0.0.8.tar.gz` & `tmp/inori-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inori-0.0.8.tar", last modified: Wed Nov 23 22:15:34 2022, max compression
+gzip compressed data, was "inori-0.0.9.tar", last modified: Mon Feb 27 22:08:15 2023, max compression
```

## Comparing `inori-0.0.8.tar` & `inori-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-23 22:15:34.654484 inori-0.0.8/
--rw-rw-rw-   0        0        0    35149 2021-02-06 02:35:18.000000 inori-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1690 2022-11-23 22:15:34.654484 inori-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2021-10-07 20:23:41.000000 inori-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-23 22:15:34.648500 inori-0.0.8/inori/
--rw-rw-rw-   0        0        0       89 2021-10-07 00:45:09.000000 inori-0.0.8/inori/__init__.py
--rw-rw-rw-   0        0        0     7029 2022-11-23 21:43:25.000000 inori-0.0.8/inori/client.py
--rw-rw-rw-   0        0        0     6571 2022-11-23 21:47:01.000000 inori-0.0.8/inori/route.py
-drwxrwxrwx   0        0        0        0 2022-11-23 22:15:34.653487 inori-0.0.8/inori/utils/
--rw-rw-rw-   0        0        0        0 2021-10-07 14:14:23.000000 inori-0.0.8/inori/utils/__init__.py
--rw-rw-rw-   0        0        0      714 2021-10-07 21:06:33.000000 inori-0.0.8/inori/utils/headerdict.py
--rw-rw-rw-   0        0        0      330 2021-10-07 00:45:09.000000 inori-0.0.8/inori/utils/safe_keyword.py
--rw-rw-rw-   0        0        0     1631 2021-10-13 15:34:00.000000 inori-0.0.8/inori/utils/string_template.py
-drwxrwxrwx   0        0        0        0 2022-11-23 22:15:34.651492 inori-0.0.8/inori.egg-info/
--rw-rw-rw-   0        0        0     1690 2022-11-23 22:15:34.000000 inori-0.0.8/inori.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2022-11-23 22:15:34.000000 inori-0.0.8/inori.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-23 22:15:34.000000 inori-0.0.8/inori.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-11-23 22:15:34.000000 inori-0.0.8/inori.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-23 22:15:34.000000 inori-0.0.8/inori.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-23 22:15:34.654484 inori-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1025 2022-11-23 22:01:20.000000 inori-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-27 22:08:15.659909 inori-0.0.9/
+-rw-rw-rw-   0        0        0    35149 2021-02-06 02:35:18.000000 inori-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1690 2023-02-27 22:08:15.659909 inori-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2021-10-07 20:23:41.000000 inori-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-02-27 22:08:15.652927 inori-0.0.9/inori/
+-rw-rw-rw-   0        0        0       89 2021-10-07 00:45:09.000000 inori-0.0.9/inori/__init__.py
+-rw-rw-rw-   0        0        0     7258 2023-02-27 21:17:41.000000 inori-0.0.9/inori/client.py
+-rw-rw-rw-   0        0        0     6578 2023-02-27 21:13:00.000000 inori-0.0.9/inori/route.py
+drwxrwxrwx   0        0        0        0 2023-02-27 22:08:15.658912 inori-0.0.9/inori/utils/
+-rw-rw-rw-   0        0        0        0 2021-10-07 14:14:23.000000 inori-0.0.9/inori/utils/__init__.py
+-rw-rw-rw-   0        0        0      714 2021-10-07 21:06:33.000000 inori-0.0.9/inori/utils/headerdict.py
+-rw-rw-rw-   0        0        0      330 2021-10-07 00:45:09.000000 inori-0.0.9/inori/utils/safe_keyword.py
+-rw-rw-rw-   0        0        0     1631 2021-10-13 15:34:00.000000 inori-0.0.9/inori/utils/string_template.py
+drwxrwxrwx   0        0        0        0 2023-02-27 22:08:15.656918 inori-0.0.9/inori.egg-info/
+-rw-rw-rw-   0        0        0     1690 2023-02-27 22:08:15.000000 inori-0.0.9/inori.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-02-27 22:08:15.000000 inori-0.0.9/inori.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-27 22:08:15.000000 inori-0.0.9/inori.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-02-27 22:08:15.000000 inori-0.0.9/inori.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-02-27 22:08:15.000000 inori-0.0.9/inori.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-27 22:08:15.660906 inori-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-02-27 22:02:12.000000 inori-0.0.9/setup.py
```

### Comparing `inori-0.0.8/LICENSE` & `inori-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inori-0.0.8/PKG-INFO` & `inori-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inori
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Universal API Client Constructor.
 Home-page: https://github.com/jsfehler/inori
 Author: Joshua Fehler
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `inori-0.0.8/README.rst` & `inori-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `inori-0.0.8/inori/client.py` & `inori-0.0.9/inori/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import uuid
 from typing import Dict, List, Optional, Union
 
+import requests
+
 import shibari
 
 from .route import Route
 from .utils.headerdict import HeaderDict
 from .utils.safe_keyword import safe_keyword
 
 
@@ -120,14 +122,21 @@
 
         self.logger_response_message = (
             '\n{http_method} response from {route}'
             '\n Status Code {status_code}'
             '\n Body: {text}'
         )
 
+    def new_session(self) -> requests.Session:
+        """Get a new instance of requests.Session.
+
+        Route objects will call this method during init.
+        """
+        return requests.Session()
+
     def add_route(self, path: str, trailing_slash: bool = False) -> Route:
         """Take a path string and create Route objects from it.
 
         Route objects are automatically set as attributes of
         the Client instance.
 
         Arguments:
```

### Comparing `inori-0.0.8/inori/route.py` & `inori-0.0.9/inori/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.children: Dict[str, Route] = {}
 
         # Parameters from parent Route
         # ie: in /foo/${barId}/${bazId}, bazId stores barId's value
         # This gets overwritten if new values are given
         self.prev_kwargs: Mapping[str, str] = {}
 
-        self.session = requests.Session()
+        self.session = self.client.new_session()
         self.session.auth = self.client.auth
 
     def __deepcopy__(self, memodict):
         """Copy in such a way as to avoid copying the client object."""
         new = type(self)(self.client, str(self.url), self.trailing_slash)
         new.callables = copy.deepcopy(self.callables)
         new.children = copy.deepcopy(self.children)
```

### Comparing `inori-0.0.8/inori/utils/headerdict.py` & `inori-0.0.9/inori/utils/headerdict.py`

 * *Files identical despite different names*

### Comparing `inori-0.0.8/inori/utils/string_template.py` & `inori-0.0.9/inori/utils/string_template.py`

 * *Files identical despite different names*

### Comparing `inori-0.0.8/inori.egg-info/PKG-INFO` & `inori-0.0.9/inori.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inori
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Universal API Client Constructor.
 Home-page: https://github.com/jsfehler/inori
 Author: Joshua Fehler
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `inori-0.0.8/setup.py` & `inori-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     path = os.path.join(os.path.dirname(__file__), filename)
     with open(path, 'r') as f:
         return f.read()
 
 
 setup(
     name="inori",
-    version="0.0.8",
+    version="0.0.9",
     description="The Universal API Client Constructor.",
     long_description=read('README.rst'),
     author="Joshua Fehler",
     license="GPLv3",
     url="https://github.com/jsfehler/inori",
     packages=find_packages(),
     install_requires=[
```

