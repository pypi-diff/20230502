# Comparing `tmp/ds2g-1.0.1.tar.gz` & `tmp/ds2g-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds2g-1.0.1.tar", last modified: Tue Apr 11 10:03:45 2023, max compression
+gzip compressed data, was "ds2g-1.0.2.tar", last modified: Tue May  2 13:41:27 2023, max compression
```

## Comparing `ds2g-1.0.1.tar` & `ds2g-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.880348 ds2g-1.0.1/
--rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.1/LICENSE
--rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.1/MANIFEST.in
--rw-r--r--   0 martinlimberger   (501) staff       (20)      424 2023-04-11 10:03:45.880203 ds2g-1.0.1/PKG-INFO
--rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.1/README.md
--rw-r--r--   0 martinlimberger   (501) staff       (20)      794 2023-04-11 07:18:03.000000 ds2g-1.0.1/pyproject.toml
--rw-r--r--   0 martinlimberger   (501) staff       (20)       38 2023-04-11 10:03:45.880390 ds2g-1.0.1/setup.cfg
--rw-r--r--   0 martinlimberger   (501) staff       (20)       49 2022-11-10 14:16:28.000000 ds2g-1.0.1/setup.py
-drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.877544 ds2g-1.0.1/src/
-drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.878949 ds2g-1.0.1/src/ds2g/
--rw-r--r--   0 martinlimberger   (501) staff       (20)     2598 2023-04-11 09:53:30.000000 ds2g-1.0.1/src/ds2g/TrackingService.py
--rw-r--r--   0 martinlimberger   (501) staff       (20)      115 2023-04-11 09:06:04.000000 ds2g-1.0.1/src/ds2g/__init__.py
--rw-r--r--   0 martinlimberger   (501) staff       (20)       98 2023-04-11 07:51:43.000000 ds2g-1.0.1/src/ds2g/__main__.py
-drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.880001 ds2g-1.0.1/src/ds2g.egg-info/
--rw-r--r--   0 martinlimberger   (501) staff       (20)      424 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/PKG-INFO
--rw-r--r--   0 martinlimberger   (501) staff       (20)      317 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/SOURCES.txt
--rw-r--r--   0 martinlimberger   (501) staff       (20)        1 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/dependency_links.txt
--rw-r--r--   0 martinlimberger   (501) staff       (20)       44 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/entry_points.txt
--rw-r--r--   0 martinlimberger   (501) staff       (20)      107 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/requires.txt
--rw-r--r--   0 martinlimberger   (501) staff       (20)        5 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/top_level.txt
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-05-02 13:41:27.678748 ds2g-1.0.2/
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.2/LICENSE
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.2/MANIFEST.in
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      424 2023-05-02 13:41:27.678611 ds2g-1.0.2/PKG-INFO
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.2/README.md
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      794 2023-05-02 13:38:15.000000 ds2g-1.0.2/pyproject.toml
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       38 2023-05-02 13:41:27.678789 ds2g-1.0.2/setup.cfg
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       49 2022-11-10 14:16:28.000000 ds2g-1.0.2/setup.py
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-05-02 13:41:27.676636 ds2g-1.0.2/src/
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-05-02 13:41:27.677637 ds2g-1.0.2/src/ds2g/
+-rw-r--r--   0 martinlimberger   (501) staff       (20)     2853 2023-05-02 13:36:17.000000 ds2g-1.0.2/src/ds2g/TrackingService.py
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      115 2023-05-02 13:38:14.000000 ds2g-1.0.2/src/ds2g/__init__.py
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       98 2023-04-11 07:51:43.000000 ds2g-1.0.2/src/ds2g/__main__.py
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-05-02 13:41:27.678368 ds2g-1.0.2/src/ds2g.egg-info/
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      424 2023-05-02 13:41:27.000000 ds2g-1.0.2/src/ds2g.egg-info/PKG-INFO
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      317 2023-05-02 13:41:27.000000 ds2g-1.0.2/src/ds2g.egg-info/SOURCES.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        1 2023-05-02 13:41:27.000000 ds2g-1.0.2/src/ds2g.egg-info/dependency_links.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       44 2023-05-02 13:41:27.000000 ds2g-1.0.2/src/ds2g.egg-info/entry_points.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      107 2023-05-02 13:41:27.000000 ds2g-1.0.2/src/ds2g.egg-info/requires.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        5 2023-05-02 13:41:27.000000 ds2g-1.0.2/src/ds2g.egg-info/top_level.txt
```

### Comparing `ds2g-1.0.1/pyproject.toml` & `ds2g-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ds2g"
-version = "1.0.1"
+version = "1.0.2"
 description = "Services of ds2g.io"
 readme = "README.md"
 authors = [{ name = "ds2g", email = "support@ds2g.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `ds2g-1.0.1/src/ds2g/TrackingService.py` & `ds2g-1.0.2/src/ds2g/TrackingService.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,8 +72,17 @@
                 except httpx.HTTPError as error_retry:
                     print(error_retry)
             else:
                 print(error)
 
     def send_many_tracks(self, tracks):
         post_fields_list = list(map(self.__prepData, tracks))
-        asyncio.run(self.__async_send_many_tracks(post_fields_list))
+        loop = None
+        try:
+            loop = asyncio.get_running_loop()
+        except:
+            loop = None
+
+        if loop and loop.is_running():
+            loop.create_task(self.__async_send_many_tracks(post_fields_list))
+        else:
+            asyncio.run(self.__async_send_many_tracks(post_fields_list))
```

