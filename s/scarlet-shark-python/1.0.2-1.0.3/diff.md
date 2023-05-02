# Comparing `tmp/scarlet-shark-python-1.0.2.tar.gz` & `tmp/scarlet-shark-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarlet-shark-python-1.0.2.tar", last modified: Tue May  2 10:03:42 2023, max compression
+gzip compressed data, was "scarlet-shark-python-1.0.3.tar", last modified: Tue May  2 10:54:45 2023, max compression
```

## Comparing `scarlet-shark-python-1.0.2.tar` & `scarlet-shark-python-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.281817 scarlet-shark-python-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-02 10:03:42.281817 scarlet-shark-python-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.277817 scarlet-shark-python-1.0.2/scarlet_shark_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.277817 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/v04_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.277817 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:03:42.281817 scarlet-shark-python-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:54:45.238271 scarlet-shark-python-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-02 10:54:45.238271 scarlet-shark-python-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:54:45.238271 scarlet-shark-python-1.0.3/scarlet_shark_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/scarlet_shark_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/scarlet_shark_python/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:54:45.238271 scarlet-shark-python-1.0.3/scarlet_shark_python/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/scarlet_shark_python/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/scarlet_shark_python/clients/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/scarlet_shark_python/clients/v04_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:54:45.238271 scarlet-shark-python-1.0.3/scarlet_shark_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-02 10:54:45.000000 scarlet-shark-python-1.0.3/scarlet_shark_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 10:54:45.000000 scarlet-shark-python-1.0.3/scarlet_shark_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:54:45.000000 scarlet-shark-python-1.0.3/scarlet_shark_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 10:54:45.000000 scarlet-shark-python-1.0.3/scarlet_shark_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 10:54:45.000000 scarlet-shark-python-1.0.3/scarlet_shark_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:54:45.238271 scarlet-shark-python-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 10:54:35.000000 scarlet-shark-python-1.0.3/setup.py
```

### Comparing `scarlet-shark-python-1.0.2/LICENSE.txt` & `scarlet-shark-python-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.2/PKG-INFO` & `scarlet-shark-python-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: scarlet-shark-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Scarlet Shark REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/scarlet-shark-python
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # scarlet-shark-python
         Scarlet Shark REST API Python client.
         
+        ## Installation
+        ```
+        pip install scarlet-shark-python
+        ```
+        
         ## Usage example
         ```python
         from scarlet_shark_python.client import ClientFactory
         
         client = ClientFactory.get_client('<your API key>', api_version='v0.4', print_json=True)
         result = client.search_domain(domain='scarletshark.com')
         ```
```

### Comparing `scarlet-shark-python-1.0.2/README.md` & `scarlet-shark-python-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # scarlet-shark-python
 Scarlet Shark REST API Python client.
 
+## Installation
+```
+pip install scarlet-shark-python
+```
+
 ## Usage example
 ```python
 from scarlet_shark_python.client import ClientFactory
 
 client = ClientFactory.get_client('<your API key>', api_version='v0.4', print_json=True)
 result = client.search_domain(domain='scarletshark.com')
 ```
```

### Comparing `scarlet-shark-python-1.0.2/scarlet_shark_python/client.py` & `scarlet-shark-python-1.0.3/scarlet_shark_python/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,7 +8,11 @@
 
 class ClientFactory:
     @staticmethod
     def get_client(api_key: str, api_version: str = 'v0.4', print_json=False) -> ScarletSharkClient:
         if api_version not in API_CLIENTS:
             raise Exception(f'No Scarlet Shark client is available for the given version {api_version}')
         return API_CLIENTS[api_version](api_key, print_json)
+
+    @staticmethod
+    def get_supported_versions():
+        return list(API_CLIENTS.keys())
```

### Comparing `scarlet-shark-python-1.0.2/scarlet_shark_python/clients/abstract.py` & `scarlet-shark-python-1.0.3/scarlet_shark_python/clients/abstract.py`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.2/scarlet_shark_python/clients/v04_client.py` & `scarlet-shark-python-1.0.3/scarlet_shark_python/clients/v04_client.py`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/PKG-INFO` & `scarlet-shark-python-1.0.3/scarlet_shark_python.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: scarlet-shark-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: Scarlet Shark REST API Python client
 Home-page: https://github.com/PiRogueToolSuite/scarlet-shark-python
 Author: U+039b
 Author-email: esther@pts-project.org
 License: UNKNOWN
 Description: # scarlet-shark-python
         Scarlet Shark REST API Python client.
         
+        ## Installation
+        ```
+        pip install scarlet-shark-python
+        ```
+        
         ## Usage example
         ```python
         from scarlet_shark_python.client import ClientFactory
         
         client = ClientFactory.get_client('<your API key>', api_version='v0.4', print_json=True)
         result = client.search_domain(domain='scarletshark.com')
         ```
```

### Comparing `scarlet-shark-python-1.0.2/setup.py` & `scarlet-shark-python-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (pwd / "README.md").read_text()
 
 install_requires = [
     'requests==2.29.0'
 ]
 
 setup(name='scarlet-shark-python',
-      version='1.0.2',
+      version='1.0.3',
       description='Scarlet Shark REST API Python client',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='U+039b',
       author_email='esther@pts-project.org',
       url='https://github.com/PiRogueToolSuite/scarlet-shark-python',
       packages=find_packages(exclude=['*.tests', '*.tests.*', 'test*', 'tests']),
```

