# Comparing `tmp/python-bring-api-1.0.2.tar.gz` & `tmp/python-bring-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/OneDrive/Projects/Programming/Python/python-bring-api/dist/tmpqaavo8_1/python-bring-api-1.0.2.tar", last modified: Sun Jan 30 10:54:34 2022, max compression
+gzip compressed data, was "python-bring-api-1.1.0.tar", last modified: Tue May  2 19:54:44 2023, max compression
```

## Comparing `python-bring-api-1.0.2.tar` & `python-bring-api-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 elias     (1000) elias     (1000)        0 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/
--rwxrwxrwx   0 elias     (1000) elias     (1000)     1114 2022-01-27 12:36:43.000000 python-bring-api-1.0.2/LICENSE
--rwxrwxrwx   0 elias     (1000) elias     (1000)     1805 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/PKG-INFO
--rwxrwxrwx   0 elias     (1000) elias     (1000)      108 2022-01-30 10:52:36.000000 python-bring-api-1.0.2/pyproject.toml
--rwxrwxrwx   0 elias     (1000) elias     (1000)     1327 2022-01-30 10:30:29.000000 python-bring-api-1.0.2/README.md
--rwxrwxrwx   0 elias     (1000) elias     (1000)      657 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/setup.cfg
-drwxrwxrwx   0 elias     (1000) elias     (1000)        0 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/
-drwxrwxrwx   0 elias     (1000) elias     (1000)        0 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/python_bring_api/
--rwxrwxrwx   0 elias     (1000) elias     (1000)     4960 2022-01-30 10:28:24.000000 python-bring-api-1.0.2/src/python_bring_api/bring.py
--rwxrwxrwx   0 elias     (1000) elias     (1000)        0 2022-01-27 12:29:47.000000 python-bring-api-1.0.2/src/python_bring_api/__init__.py
-drwxrwxrwx   0 elias     (1000) elias     (1000)        0 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/python_bring_api.egg-info/
--rwxrwxrwx   0 elias     (1000) elias     (1000)        1 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/python_bring_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 elias     (1000) elias     (1000)     1805 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/python_bring_api.egg-info/PKG-INFO
--rwxrwxrwx   0 elias     (1000) elias     (1000)        9 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/python_bring_api.egg-info/requires.txt
--rwxrwxrwx   0 elias     (1000) elias     (1000)      324 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/python_bring_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 elias     (1000) elias     (1000)       17 2022-01-30 10:54:34.000000 python-bring-api-1.0.2/src/python_bring_api.egg-info/top_level.txt
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.791806 python-bring-api-1.1.0/
+-rw-------   0 elias     (1000) elias     (1000)     1114 2022-01-27 12:36:43.000000 python-bring-api-1.1.0/LICENSE
+-rw-r--r--   0 elias     (1000) elias     (1000)     1860 2023-05-02 19:54:44.791806 python-bring-api-1.1.0/PKG-INFO
+-rw-------   0 elias     (1000) elias     (1000)     1433 2023-05-02 19:53:41.000000 python-bring-api-1.1.0/README.md
+-rw-------   0 elias     (1000) elias     (1000)      108 2022-01-30 10:52:36.000000 python-bring-api-1.1.0/pyproject.toml
+-rw-------   0 elias     (1000) elias     (1000)      657 2023-05-02 19:54:44.792806 python-bring-api-1.1.0/setup.cfg
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.789806 python-bring-api-1.1.0/src/
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.790806 python-bring-api-1.1.0/src/python_bring_api/
+-rw-------   0 elias     (1000) elias     (1000)        0 2022-01-27 12:29:47.000000 python-bring-api-1.1.0/src/python_bring_api/__init__.py
+-rw-r--r--   0 elias     (1000) elias     (1000)     5583 2023-05-02 19:46:28.000000 python-bring-api-1.1.0/src/python_bring_api/bring.py
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.791806 python-bring-api-1.1.0/src/python_bring_api.egg-info/
+-rw-------   0 elias     (1000) elias     (1000)     1860 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/PKG-INFO
+-rw-------   0 elias     (1000) elias     (1000)      324 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/SOURCES.txt
+-rw-------   0 elias     (1000) elias     (1000)        1 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/dependency_links.txt
+-rw-------   0 elias     (1000) elias     (1000)        9 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/requires.txt
+-rw-------   0 elias     (1000) elias     (1000)       17 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-bring-api-1.0.2/LICENSE` & `python-bring-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bring-api-1.0.2/PKG-INFO` & `python-bring-api-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: python-bring-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Unofficial python package to access Bring! shopping lists API.
 Home-page: https://github.com/blue1stone/python-bring-api
 Author: Elias Ball
 Author-email: contact.eliasball@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bring Shopping Lists API
+
 An unofficial python package to access the Bring! shopping lists API.
 
 > This is a **minimal** python port of the [node-bring-api](https://github.com/foxriver76/node-bring-api) by [foxriver76](https://github.com/foxriver76). All credit goes to him for making this awesome API possible!
 
 ## Disclaimer
+
 The developers of this module are in no way endorsed by or affiliated with Bring! Labs AG, or any associated subsidiaries, logos or trademarks.
 
 ## Installation
-```pip install python-bring-api```
+
+`pip install python-bring-api`
 
 ## Usage Example
+
 ```python
 from python_bring_api.bring import Bring
 
 # Create Bring instance with email and password
 bring = Bring("EMAIL", "PASSWORD")
 # Login
 bring.login()
@@ -45,16 +47,24 @@
 print(items['purchase']) # [{'specification': 'low fat', 'name': 'Milk'}]
 
 # Remove an item from a list
 bring.removeItem(lists['lists'][0]['listUuid'], 'Milk')
 ```
 
 ## Changelog
+
+### 1.1.0
+
+Add item details endpoint, thanks to [@Dielee](https://github.com/Dielee)!
+
 ### 1.0.2
+
 Fixed error handling
 Added response return to login
+
 ### 1.0.1
+
 Add github repo
-### 1.0.0 
-Initial release
 
+### 1.0.0
 
+Initial release
```

### Comparing `python-bring-api-1.0.2/README.md` & `python-bring-api-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Bring Shopping Lists API
+
 An unofficial python package to access the Bring! shopping lists API.
 
 > This is a **minimal** python port of the [node-bring-api](https://github.com/foxriver76/node-bring-api) by [foxriver76](https://github.com/foxriver76). All credit goes to him for making this awesome API possible!
 
 ## Disclaimer
+
 The developers of this module are in no way endorsed by or affiliated with Bring! Labs AG, or any associated subsidiaries, logos or trademarks.
 
 ## Installation
-```pip install python-bring-api```
+
+`pip install python-bring-api`
 
 ## Usage Example
+
 ```python
 from python_bring_api.bring import Bring
 
 # Create Bring instance with email and password
 bring = Bring("EMAIL", "PASSWORD")
 # Login
 bring.login()
@@ -29,14 +33,24 @@
 print(items['purchase']) # [{'specification': 'low fat', 'name': 'Milk'}]
 
 # Remove an item from a list
 bring.removeItem(lists['lists'][0]['listUuid'], 'Milk')
 ```
 
 ## Changelog
+
+### 1.1.0
+
+Add item details endpoint, thanks to [@Dielee](https://github.com/Dielee)!
+
 ### 1.0.2
+
 Fixed error handling
 Added response return to login
+
 ### 1.0.1
+
 Add github repo
-### 1.0.0 
+
+### 1.0.0
+
 Initial release
```

### Comparing `python-bring-api-1.0.2/setup.cfg` & `python-bring-api-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-bring-api
-version = 1.0.2
+version = 1.1.0
 author = Elias Ball
 author_email = contact.eliasball@gmail.com
 description = Unofficial python package to access Bring! shopping lists API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/blue1stone/python-bring-api
```

### Comparing `python-bring-api-1.0.2/src/python_bring_api/bring.py` & `python-bring-api-1.1.0/src/python_bring_api/bring.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,38 @@
             r = requests.get(f'{self.url}bringlists/{listUuid}', headers = self.headers);
             return r.json();
         except:
             print(f'Exception: Cannot get items for list {listUuid}:')
             traceback.print_exc()
             raise
 
+
+    def getAllItemDetails(self, listUuid):
+        """
+        Get all details from a shopping list.
+
+        Parameters
+        ----------
+        listUuid : str
+            A list uuid returned by loadLists()
+
+        Returns
+        -------
+        list
+            The JSON response as a list.
+        """
+        try:
+            r = requests.get(f'{self.url}bringlists/{listUuid}/details', headers = self.headers);
+            return r.json();
+        except:
+            print(f'Exception: Cannot get item details for list {listUuid}:')
+            traceback.print_exc()
+            raise
+
+
     def saveItem(self, listUuid, itemName, specification=''):
         """
         Save an item to a shopping list.
 
         Parameters
         ----------
         listUuid : str
```

### Comparing `python-bring-api-1.0.2/src/python_bring_api.egg-info/PKG-INFO` & `python-bring-api-1.1.0/src/python_bring_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: python-bring-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Unofficial python package to access Bring! shopping lists API.
 Home-page: https://github.com/blue1stone/python-bring-api
 Author: Elias Ball
 Author-email: contact.eliasball@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bring Shopping Lists API
+
 An unofficial python package to access the Bring! shopping lists API.
 
 > This is a **minimal** python port of the [node-bring-api](https://github.com/foxriver76/node-bring-api) by [foxriver76](https://github.com/foxriver76). All credit goes to him for making this awesome API possible!
 
 ## Disclaimer
+
 The developers of this module are in no way endorsed by or affiliated with Bring! Labs AG, or any associated subsidiaries, logos or trademarks.
 
 ## Installation
-```pip install python-bring-api```
+
+`pip install python-bring-api`
 
 ## Usage Example
+
 ```python
 from python_bring_api.bring import Bring
 
 # Create Bring instance with email and password
 bring = Bring("EMAIL", "PASSWORD")
 # Login
 bring.login()
@@ -45,16 +47,24 @@
 print(items['purchase']) # [{'specification': 'low fat', 'name': 'Milk'}]
 
 # Remove an item from a list
 bring.removeItem(lists['lists'][0]['listUuid'], 'Milk')
 ```
 
 ## Changelog
+
+### 1.1.0
+
+Add item details endpoint, thanks to [@Dielee](https://github.com/Dielee)!
+
 ### 1.0.2
+
 Fixed error handling
 Added response return to login
+
 ### 1.0.1
+
 Add github repo
-### 1.0.0 
-Initial release
 
+### 1.0.0
 
+Initial release
```

