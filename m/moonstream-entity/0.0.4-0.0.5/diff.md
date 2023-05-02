# Comparing `tmp/moonstream-entity-0.0.4.tar.gz` & `tmp/moonstream-entity-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstream-entity-0.0.4.tar", last modified: Thu Apr 27 17:42:25 2023, max compression
+gzip compressed data, was "moonstream-entity-0.0.5.tar", last modified: Tue May  2 14:57:28 2023, max compression
```

## Comparing `moonstream-entity-0.0.4.tar` & `moonstream-entity-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/entity/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9659 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/moonstream_entity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:57:28.452477 moonstream-entity-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-05-02 14:57:28.452477 moonstream-entity-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:57:28.452477 moonstream-entity-0.0.5/entity/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9659 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/entity/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10198 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/entity/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/entity/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/entity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/entity/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/entity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:57:28.452477 moonstream-entity-0.0.5/moonstream_entity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-05-02 14:57:28.000000 moonstream-entity-0.0.5/moonstream_entity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-05-02 14:57:28.000000 moonstream-entity-0.0.5/moonstream_entity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 14:57:28.000000 moonstream-entity-0.0.5/moonstream_entity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-02 14:57:28.000000 moonstream-entity-0.0.5/moonstream_entity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-02 14:57:28.000000 moonstream-entity-0.0.5/moonstream_entity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-02 14:57:28.000000 moonstream-entity-0.0.5/moonstream_entity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 14:57:28.452477 moonstream-entity-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-02 14:57:05.000000 moonstream-entity-0.0.5/setup.py
```

### Comparing `moonstream-entity-0.0.4/PKG-INFO` & `moonstream-entity-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstream-entity
-Version: 0.0.4
+Version: 0.0.5
 Summary: Moonstream entity API client library
 Home-page: https://github.com/bugout-dev/entity
 Author: Moonstream
 Author-email: engineering@moonstream.to
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `moonstream-entity-0.0.4/README.md` & `moonstream-entity-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `moonstream-entity-0.0.4/entity/cli.py` & `moonstream-entity-0.0.5/entity/cli.py`

 * *Files identical despite different names*

### Comparing `moonstream-entity-0.0.4/entity/client.py` & `moonstream-entity-0.0.5/entity/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,10 +309,11 @@
             params["filters"] = filters
 
         result = self._call(
             method=data.Method.GET,
             url=f"{self.api.endpoints[ENDPOINT_COLLECTIONS]}/{str(collection_id)}{ENDPOINT_SEARCH}",
             headers=headers,
             timeout=timeout,
+            params=params,
         )
 
         return data.EntitySearchResponse(**result)
```

### Comparing `moonstream-entity-0.0.4/entity/data.py` & `moonstream-entity-0.0.5/entity/data.py`

 * *Files identical despite different names*

### Comparing `moonstream-entity-0.0.4/moonstream_entity.egg-info/PKG-INFO` & `moonstream-entity-0.0.5/moonstream_entity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstream-entity
-Version: 0.0.4
+Version: 0.0.5
 Summary: Moonstream entity API client library
 Home-page: https://github.com/bugout-dev/entity
 Author: Moonstream
 Author-email: engineering@moonstream.to
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `moonstream-entity-0.0.4/setup.py` & `moonstream-entity-0.0.5/setup.py`

 * *Files identical despite different names*

