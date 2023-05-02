# Comparing `tmp/burrowkv-0.0.3.tar.gz` & `tmp/burrowkv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burrowkv-0.0.3.tar", last modified: Fri Apr 28 16:01:40 2023, max compression
+gzip compressed data, was "burrowkv-0.0.4.tar", last modified: Tue May  2 15:32:04 2023, max compression
```

## Comparing `burrowkv-0.0.3.tar` & `burrowkv-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.222696 burrowkv-0.0.3/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1064 2023-04-27 20:35:40.000000 burrowkv-0.0.3/LICENSE
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-04-28 16:01:40.222696 burrowkv-0.0.3/PKG-INFO
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1503 2023-04-28 13:02:04.000000 burrowkv-0.0.3/README.md
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.218696 burrowkv-0.0.3/burrowkv/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       55 2023-04-28 13:02:04.000000 burrowkv-0.0.3/burrowkv/__init__.py
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     4722 2023-04-28 16:00:24.000000 burrowkv-0.0.3/burrowkv/burrowkv.py
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.218696 burrowkv-0.0.3/burrowkv.egg-info/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/PKG-INFO
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      237 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/SOURCES.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        1 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/dependency_links.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       15 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/top_level.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       38 2023-04-28 16:01:40.222696 burrowkv-0.0.3/setup.cfg
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      694 2023-04-28 15:59:11.000000 burrowkv-0.0.3/setup.py
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.222696 burrowkv-0.0.3/tests/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 10:10:31.000000 burrowkv-0.0.3/tests/__init__.py
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1708 2023-04-28 15:07:59.000000 burrowkv-0.0.3/tests/test_burrowkv.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-02 15:32:04.846227 burrowkv-0.0.4/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1064 2023-04-27 20:35:40.000000 burrowkv-0.0.4/LICENSE
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-05-02 15:32:04.846227 burrowkv-0.0.4/PKG-INFO
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1503 2023-04-28 13:02:04.000000 burrowkv-0.0.4/README.md
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-02 15:32:04.846227 burrowkv-0.0.4/burrowkv/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       55 2023-04-28 13:02:04.000000 burrowkv-0.0.4/burrowkv/__init__.py
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     4812 2023-05-02 15:31:11.000000 burrowkv-0.0.4/burrowkv/burrowkv.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-02 15:32:04.846227 burrowkv-0.0.4/burrowkv.egg-info/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-05-02 15:32:04.000000 burrowkv-0.0.4/burrowkv.egg-info/PKG-INFO
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      237 2023-05-02 15:32:04.000000 burrowkv-0.0.4/burrowkv.egg-info/SOURCES.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        1 2023-05-02 15:32:04.000000 burrowkv-0.0.4/burrowkv.egg-info/dependency_links.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       15 2023-05-02 15:32:04.000000 burrowkv-0.0.4/burrowkv.egg-info/top_level.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       38 2023-05-02 15:32:04.846227 burrowkv-0.0.4/setup.cfg
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      694 2023-05-02 15:31:34.000000 burrowkv-0.0.4/setup.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-02 15:32:04.846227 burrowkv-0.0.4/tests/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 10:10:31.000000 burrowkv-0.0.4/tests/__init__.py
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1708 2023-04-28 15:07:59.000000 burrowkv-0.0.4/tests/test_burrowkv.py
```

### Comparing `burrowkv-0.0.3/LICENSE` & `burrowkv-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `burrowkv-0.0.3/PKG-INFO` & `burrowkv-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burrowkv
-Version: 0.0.3
+Version: 0.0.4
 Summary: key-value store
 Home-page: https://github.com/iunary/burrowkv
 Author: Yusuf
 Author-email: contact@yusuf.im
 License: MIT
 Keywords: key value store,kv,key-value
 Platform: UNKNOWN
```

### Comparing `burrowkv-0.0.3/README.md` & `burrowkv-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `burrowkv-0.0.3/burrowkv/burrowkv.py` & `burrowkv-0.0.4/burrowkv/burrowkv.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         Set a value for the given key.
 
         Args:
             key (str): The key to set.
             value (str): The value to associate with the key.
 
         Example:
-            >>> store = KeyValueStore()
+            >>> store = Burrowkv()
             >>> store.set('name', 'John')
         """
         with self.__lock:
             self.__store[key] = value
 
     def get(self, key: str) -> Optional[str]:
         """
@@ -42,15 +42,15 @@
             key (str): The key to retrieve.
 
         Returns:
             The value associated with the key, or None
             if the key does not exist.
 
         Example:
-            >>> store = KeyValueStore()
+            >>> store = Burrowkv()
             >>> store.set('name', 'John')
             >>> store.get('name')
             'John'
             >>> store.get('age')
         """
         with self.__lock:
             return self.__store[key]
@@ -72,15 +72,15 @@
         Args:
             key (str): The key to check.
 
         Returns:
             bool: True if the key exists, False otherwise.
 
         Example:
-            >>> store = KeyValueStore()
+            >>> store = Burrowkv()
             >>> store.set('name', 'John')
             >>> store.contains('name')
             True
             >>> store.contains('age')
             False
         """
         return key in self.__store
@@ -89,45 +89,45 @@
         """
         Get a list of all keys in the store.
 
         Returns:
             list: A list of keys.
 
         Example:
-            >>> store = KeyValueStore()
+            >>> store = Burrowkv()
             >>> store.set('name', 'John')
             >>> store.keys()
             ['name']
         """
         return list(self.__store.keys())
 
     def values(self) -> List[str]:
         """
         Get a list of all values in the store.
 
         Returns:
             list: A list of values.
 
         Example:
-            >>> store = KeyValueStore()
+            >>> store = Burrowkv()
             >>> store.set('name', 'John')
             >>> store.values()
             ['John']
         """
         return list(self.__store.values())
 
     def items(self) -> List[Tuple[str, str]]:
         """
         Get a list of all key-value pairs in the store.
 
         Returns:
             list: A list of (key, value) tuples.
 
         Example:
-            >>> store = KeyValueStore()
+            >>> store = Burrowkv()
             >>> store.set('name', 'John')
             >>> store.items()
             [('name', 'John')]
         """
         return list(self.__store.items())
 
     def to_json(self) -> str:
@@ -156,25 +156,22 @@
     @contextmanager
     def transaction(self):
         """
         Create a transaction context for
         performing multiple operations on the store.
 
         Example:
-        >>> store = KeyValueStore()
+        >>> store = Burrowkv()
         >>> with store.transaction():
         ...     store.set('name', 'John')
         ...     store.set('age', 30)
         >>> store.get('name')
         >>> store.get('age')
         """
-        try:
-            yield
-        finally:
-            self.__store.clear()
+        yield
 
     def clear(self):
         """
         Clear the data store
 
         Returns:
             None
@@ -186,7 +183,15 @@
         """
         Return the number of key-value pairs in the store.
 
         Returns:
             int: The number of key-value pairs.
         """
         return len(self.__store)
+
+    def __repr__(self) -> str:
+        """Return the store representation
+
+        Returns:
+            str: JSON respresentation of key-value store
+        """
+        return self.to_json()
```

### Comparing `burrowkv-0.0.3/burrowkv.egg-info/PKG-INFO` & `burrowkv-0.0.4/burrowkv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burrowkv
-Version: 0.0.3
+Version: 0.0.4
 Summary: key-value store
 Home-page: https://github.com/iunary/burrowkv
 Author: Yusuf
 Author-email: contact@yusuf.im
 License: MIT
 Keywords: key value store,kv,key-value
 Platform: UNKNOWN
```

### Comparing `burrowkv-0.0.3/setup.py` & `burrowkv-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="burrowkv",
     version=VERSION,
```

### Comparing `burrowkv-0.0.3/tests/test_burrowkv.py` & `burrowkv-0.0.4/tests/test_burrowkv.py`

 * *Files identical despite different names*

