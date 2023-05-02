# Comparing `tmp/keypact-0.2.1.tar.gz` & `tmp/keypact-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.2.1.tar", last modified: Tue May  2 21:17:17 2023, max compression
+gzip compressed data, was "keypact-0.2.2.tar", last modified: Tue May  2 21:34:01 2023, max compression
```

## Comparing `keypact-0.2.1.tar` & `keypact-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:17:17.574008 keypact-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-02 21:16:59.000000 keypact-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 21:17:17.574008 keypact-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 21:16:59.000000 keypact-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:17:17.574008 keypact-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-02 21:16:59.000000 keypact-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:17:17.570007 keypact-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:17:17.570007 keypact-0.2.1/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 21:16:59.000000 keypact-0.2.1/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-02 21:16:59.000000 keypact-0.2.1/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:17:17.574008 keypact-0.2.1/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 21:17:16.000000 keypact-0.2.1/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-02 21:17:17.000000 keypact-0.2.1/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:17:16.000000 keypact-0.2.1/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 21:17:16.000000 keypact-0.2.1/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:17:16.000000 keypact-0.2.1/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 21:17:16.000000 keypact-0.2.1/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:17:16.000000 keypact-0.2.1/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.680651 keypact-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-02 21:33:49.000000 keypact-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 21:34:01.680651 keypact-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 21:33:49.000000 keypact-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:34:01.680651 keypact-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-02 21:33:49.000000 keypact-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.676651 keypact-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.676651 keypact-0.2.2/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 21:33:49.000000 keypact-0.2.2/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-02 21:33:49.000000 keypact-0.2.2/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:34:01.680651 keypact-0.2.2/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:34:01.000000 keypact-0.2.2/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.2.1/LICENSE` & `keypact-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.2.1/PKG-INFO` & `keypact-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.2.1
+Version: 0.2.2
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```

### Comparing `keypact-0.2.1/README.md` & `keypact-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `keypact-0.2.1/setup.py` & `keypact-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.2.1',
+version='0.2.2',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.2.1/src/keypact/keypact.py` & `keypact-0.2.2/src/keypact/keypact.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,22 +54,26 @@
         return total_result
 
     def get_key(self, key_location: str):
        
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
             raise FileNotFoundError("Key not found")
-
-        with open(os.path.join(self.location, key_location), "rb") as f:
-            result = pickle.load(f)
+        total_result = None
+        while total_result == None:
             try:
-                total_result = result["key"]
-            except TypeError:
-                total_result = False
-            return total_result
+                with open(os.path.join(self.location, key_location), "rb") as f:
+                    result = pickle.load(f)
+                    try:
+                        total_result = result["key"]
+                    except TypeError:
+                        total_result = False
+            except EOFError:
+                pass                        
+        return total_result
 
     def delete(self, key: str):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
         try:
             os.remove(os.path.join(self.location, key_location))
         except OSError:
```

### Comparing `keypact-0.2.1/src/keypact.egg-info/PKG-INFO` & `keypact-0.2.2/src/keypact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.2.1
+Version: 0.2.2
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```

