# Comparing `tmp/lampo_py-0.0.1a2.tar.gz` & `tmp/lampo_py-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampo_py-0.0.1a2.tar", max compression
+gzip compressed data, was "lampo_py-0.0.1a3.tar", max compression
```

## Comparing `lampo_py-0.0.1a2.tar` & `lampo_py-0.0.1a3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      143 2023-05-02 03:39:48.602048 lampo_py-0.0.1a2/README.md
--rw-r--r--   0        0        0       31 2023-05-02 01:32:52.791915 lampo_py-0.0.1a2/lampo_py/__init__.py
--rw-r--r--   0        0        0     1946 2023-05-02 03:12:02.898733 lampo_py-0.0.1a2/lampo_py/lampo.py
--rw-r--r--   0        0        0      432 2023-05-02 03:45:07.760904 lampo_py-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 lampo_py-0.0.1a2/setup.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-02 04:25:55.140684 lampo_py-0.0.1a3/README.md
+-rw-r--r--   0        0        0       31 2023-05-02 04:25:55.140684 lampo_py-0.0.1a3/lampo_py/__init__.py
+-rw-r--r--   0        0        0     1955 2023-05-02 05:31:45.809387 lampo_py-0.0.1a3/lampo_py/lampo.py
+-rw-r--r--   0        0        0      432 2023-05-02 05:33:21.333143 lampo_py-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 lampo_py-0.0.1a3/setup.py
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 lampo_py-0.0.1a3/PKG-INFO
```

### Comparing `lampo_py-0.0.1a2/lampo_py/lampo.py` & `lampo_py-0.0.1a3/lampo_py/lampo.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Run The lightning node!
         """
         lampod.add_jsonrpc_on_unixsocket(self.__inner)
         lampod.lampo_listen(self.__inner)
 
     def call(self, method: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         """ " Perform a call to the lightning node"""
-        result = lampod.lampod_call(self.__inner, bytes(method), b"{}")
+        result = lampod.lampod_call(self.__inner, bytes(method, "utf-8"), b"{}")
         logging.debug(f"raw data {result}")
         result = ffi.string(result).decode("utf-8")
         assert result is not None
         result = json.loads(result)
 
         logging.debug(f"call to `{method}` return {result}")
         return result
```

### Comparing `lampo_py-0.0.1a2/setup.py` & `lampo_py-0.0.1a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cffi>=1.15.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'lampo-py',
-    'version': '0.0.1a2',
+    'version': '0.0.1a3',
     'description': '',
     'long_description': '# Python Language Binding for Lampo\n\n## What is lampo?\n\nlampo (lightning in Italian) is a experimental implementation of a tiny lightning node\n',
     'author': 'Vincenzo Palazzo',
     'author_email': 'vincenzopalazzodev@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lampo_py-0.0.1a2/PKG-INFO` & `lampo_py-0.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lampo-py
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: 
 Author: Vincenzo Palazzo
 Author-email: vincenzopalazzodev@gmail.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

