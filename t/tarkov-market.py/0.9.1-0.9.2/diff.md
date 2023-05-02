# Comparing `tmp/tarkov-market.py-0.9.1.tar.gz` & `tmp/tarkov-market.py-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarkov-market.py-0.9.1.tar", last modified: Sun Oct  3 16:02:30 2021, max compression
+gzip compressed data, was "tarkov-market.py-0.9.2.tar", last modified: Sat Oct  9 09:41:30 2021, max compression
```

## Comparing `tarkov-market.py-0.9.1.tar` & `tarkov-market.py-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-10-03 16:02:30.746810 tarkov-market.py-0.9.1/
--rw-rw-rw-   0        0        0     1081 2021-08-22 15:18:29.000000 tarkov-market.py-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     2622 2021-10-03 16:02:30.745809 tarkov-market.py-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2293 2021-09-07 14:34:19.000000 tarkov-market.py-0.9.1/README.rst
--rw-rw-rw-   0        0        0       42 2021-10-03 16:02:30.746810 tarkov-market.py-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      800 2021-09-07 13:30:22.000000 tarkov-market.py-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-03 16:02:30.715803 tarkov-market.py-0.9.1/tarkov_market/
--rw-rw-rw-   0        0        0      358 2021-10-03 16:02:03.000000 tarkov-market.py-0.9.1/tarkov_market/__init__.py
--rw-rw-rw-   0        0        0     6118 2021-10-03 16:01:20.000000 tarkov-market.py-0.9.1/tarkov_market/client.py
--rw-rw-rw-   0        0        0     4733 2021-08-27 11:25:24.000000 tarkov-market.py-0.9.1/tarkov_market/enums.py
--rw-rw-rw-   0        0        0     1093 2021-08-25 07:51:44.000000 tarkov-market.py-0.9.1/tarkov_market/errors.py
--rw-rw-rw-   0        0        0     5980 2021-09-27 16:12:38.000000 tarkov-market.py-0.9.1/tarkov_market/http.py
--rw-rw-rw-   0        0        0     5193 2021-09-29 14:40:20.000000 tarkov-market.py-0.9.1/tarkov_market/item.py
--rw-rw-rw-   0        0        0      571 2021-09-05 06:09:03.000000 tarkov-market.py-0.9.1/tarkov_market/traders.py
-drwxrwxrwx   0        0        0        0 2021-10-03 16:02:30.744809 tarkov-market.py-0.9.1/tarkov_market/types/
--rw-rw-rw-   0        0        0      100 2021-08-25 10:15:07.000000 tarkov-market.py-0.9.1/tarkov_market/types/__init__.py
--rw-rw-rw-   0        0        0     3471 2021-09-29 14:38:51.000000 tarkov-market.py-0.9.1/tarkov_market/types/item.py
--rw-rw-rw-   0        0        0      304 2021-08-26 17:44:32.000000 tarkov-market.py-0.9.1/tarkov_market/types/trader.py
--rw-rw-rw-   0        0        0      361 2021-08-25 09:34:28.000000 tarkov-market.py-0.9.1/tarkov_market/utils.py
-drwxrwxrwx   0        0        0        0 2021-10-03 16:02:30.738808 tarkov-market.py-0.9.1/tarkov_market.py.egg-info/
--rw-rw-rw-   0        0        0     2622 2021-10-03 16:02:30.000000 tarkov-market.py-0.9.1/tarkov_market.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2021-10-03 16:02:30.000000 tarkov-market.py-0.9.1/tarkov_market.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-03 16:02:30.000000 tarkov-market.py-0.9.1/tarkov_market.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2021-10-03 16:02:30.000000 tarkov-market.py-0.9.1/tarkov_market.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-10-09 09:41:30.379503 tarkov-market.py-0.9.2/
+-rw-rw-rw-   0        0        0     1081 2021-08-22 15:18:29.000000 tarkov-market.py-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0     2622 2021-10-09 09:41:30.378504 tarkov-market.py-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2293 2021-09-07 14:34:19.000000 tarkov-market.py-0.9.2/README.rst
+-rw-rw-rw-   0        0        0       42 2021-10-09 09:41:30.379503 tarkov-market.py-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      800 2021-09-07 13:30:22.000000 tarkov-market.py-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-09 09:41:30.306486 tarkov-market.py-0.9.2/tarkov_market/
+-rw-rw-rw-   0        0        0      358 2021-10-09 09:41:04.000000 tarkov-market.py-0.9.2/tarkov_market/__init__.py
+-rw-rw-rw-   0        0        0     6142 2021-10-09 09:40:37.000000 tarkov-market.py-0.9.2/tarkov_market/client.py
+-rw-rw-rw-   0        0        0     4733 2021-08-27 11:25:24.000000 tarkov-market.py-0.9.2/tarkov_market/enums.py
+-rw-rw-rw-   0        0        0     1093 2021-08-25 07:51:44.000000 tarkov-market.py-0.9.2/tarkov_market/errors.py
+-rw-rw-rw-   0        0        0     5980 2021-09-27 16:12:38.000000 tarkov-market.py-0.9.2/tarkov_market/http.py
+-rw-rw-rw-   0        0        0     5193 2021-09-29 14:40:20.000000 tarkov-market.py-0.9.2/tarkov_market/item.py
+-rw-rw-rw-   0        0        0      571 2021-09-05 06:09:03.000000 tarkov-market.py-0.9.2/tarkov_market/traders.py
+drwxrwxrwx   0        0        0        0 2021-10-09 09:41:30.376502 tarkov-market.py-0.9.2/tarkov_market/types/
+-rw-rw-rw-   0        0        0      100 2021-08-25 10:15:07.000000 tarkov-market.py-0.9.2/tarkov_market/types/__init__.py
+-rw-rw-rw-   0        0        0     3471 2021-09-29 14:38:51.000000 tarkov-market.py-0.9.2/tarkov_market/types/item.py
+-rw-rw-rw-   0        0        0      304 2021-08-26 17:44:32.000000 tarkov-market.py-0.9.2/tarkov_market/types/trader.py
+-rw-rw-rw-   0        0        0      361 2021-08-25 09:34:28.000000 tarkov-market.py-0.9.2/tarkov_market/utils.py
+drwxrwxrwx   0        0        0        0 2021-10-09 09:41:30.322491 tarkov-market.py-0.9.2/tarkov_market.py.egg-info/
+-rw-rw-rw-   0        0        0     2622 2021-10-09 09:41:29.000000 tarkov-market.py-0.9.2/tarkov_market.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2021-10-09 09:41:29.000000 tarkov-market.py-0.9.2/tarkov_market.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-09 09:41:29.000000 tarkov-market.py-0.9.2/tarkov_market.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2021-10-09 09:41:29.000000 tarkov-market.py-0.9.2/tarkov_market.py.egg-info/top_level.txt
```

### Comparing `tarkov-market.py-0.9.1/LICENSE` & `tarkov-market.py-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/PKG-INFO` & `tarkov-market.py-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarkov-market.py
-Version: 0.9.1
+Version: 0.9.2
 Summary: async API wrapper for Tarkov Market written in Python.
 Home-page: https://github.com/Hostagen/tarkov-market.py
 Author: Hostagen
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
```

### Comparing `tarkov-market.py-0.9.1/README.rst` & `tarkov-market.py-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/setup.py` & `tarkov-market.py-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/tarkov_market/client.py` & `tarkov-market.py-0.9.2/tarkov_market/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,19 +95,15 @@
     ) -> List[Item]:
 
         result = []
 
         if check is MISSING:
 
             def check(i: Item):
-
-                if item_name.lower() in i.name.lower() or item_name.lower() in i.short_name.lower():
-                    return True
-
-                return False
+                return item_name.lower() in i.name.lower() or item_name.lower() in i.short_name.lower()
 
         for item in self.items:
 
             if not check(item):
                 continue
 
             result.append(item)
@@ -193,14 +189,18 @@
             async with self.http as session:
                 await session.recreate()
 
                 data = await session.get_all_items()
 
                 for payload in data:
                     item = Item(http=self.http, payload=payload)
+
+                    if item.name in self._items:
+                        continue
+
                     self._items[item.name] = item
                     self._uid_items[item.uid] = item.name
 
                 bsg_item = await session.get_all_bsg_items()
 
                 if bsg_item:
                     map(self._add_bsg_item, bsg_item.values())
```

### Comparing `tarkov-market.py-0.9.1/tarkov_market/enums.py` & `tarkov-market.py-0.9.2/tarkov_market/enums.py`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/tarkov_market/errors.py` & `tarkov-market.py-0.9.2/tarkov_market/errors.py`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/tarkov_market/http.py` & `tarkov-market.py-0.9.2/tarkov_market/http.py`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/tarkov_market/item.py` & `tarkov-market.py-0.9.2/tarkov_market/item.py`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/tarkov_market/traders.py` & `tarkov-market.py-0.9.2/tarkov_market/traders.py`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/tarkov_market/types/item.py` & `tarkov-market.py-0.9.2/tarkov_market/types/item.py`

 * *Files identical despite different names*

### Comparing `tarkov-market.py-0.9.1/tarkov_market.py.egg-info/PKG-INFO` & `tarkov-market.py-0.9.2/tarkov_market.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarkov-market.py
-Version: 0.9.1
+Version: 0.9.2
 Summary: async API wrapper for Tarkov Market written in Python.
 Home-page: https://github.com/Hostagen/tarkov-market.py
 Author: Hostagen
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
```

