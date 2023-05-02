# Comparing `tmp/apyproxy-0.1.0.tar.gz` & `tmp/apyproxy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apyproxy-0.1.0.tar", max compression
+gzip compressed data, was "apyproxy-0.2.2.tar", max compression
```

## Comparing `apyproxy-0.1.0.tar` & `apyproxy-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1063 2019-11-22 07:51:19.299874 apyproxy-0.1.0/LICENSE
--rw-r--r--   0        0        0     3329 2023-04-14 12:10:43.930234 apyproxy-0.1.0/apyproxy/__init__.py
--rw-r--r--   0        0        0      362 2023-04-14 12:13:45.238158 apyproxy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      629 2023-04-14 15:30:29.365364 apyproxy-0.1.0/setup.py
--rw-r--r--   0        0        0      441 2023-04-14 15:30:29.366133 apyproxy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-02 15:07:20.847494 apyproxy-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3378 2023-05-02 15:07:20.847494 apyproxy-0.2.2/apyproxy/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-02 15:07:20.847494 apyproxy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 apyproxy-0.2.2/PKG-INFO
```

### Comparing `apyproxy-0.1.0/LICENSE` & `apyproxy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apyproxy-0.1.0/apyproxy/__init__.py` & `apyproxy-0.2.2/apyproxy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,7 +107,10 @@
         return self.request("POST", data=data, json=json, **kwargs)
 
     def put(self, data=None, **kwargs):
         return self.request("PUT", data=data, **kwargs)
 
     def __repr__(self):
         return "ApyProxy(%s)" % self._url
+
+    def __str__(self):
+        return self._url
```

