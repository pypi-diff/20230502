# Comparing `tmp/superset-iris-0.2.0.tar.gz` & `tmp/superset-iris-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superset-iris-0.2.0.tar", last modified: Thu Apr 27 06:46:11 2023, max compression
+gzip compressed data, was "superset-iris-0.3.0.tar", last modified: Tue May  2 13:32:40 2023, max compression
```

## Comparing `superset-iris-0.2.0.tar` & `superset-iris-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 daimor     (501) staff       (20)        0 2023-04-27 06:46:11.837450 superset-iris-0.2.0/
--rw-r--r--   0 daimor     (501) staff       (20)     1075 2023-04-16 14:41:10.000000 superset-iris-0.2.0/LICENSE
--rw-r--r--   0 daimor     (501) staff       (20)     3153 2023-04-27 06:46:11.837537 superset-iris-0.2.0/PKG-INFO
--rw-r--r--   0 daimor     (501) staff       (20)     2209 2023-04-18 09:21:31.000000 superset-iris-0.2.0/README.md
--rw-r--r--   0 daimor     (501) staff       (20)      933 2023-04-27 06:46:11.837854 superset-iris-0.2.0/setup.cfg
--rw-r--r--   0 daimor     (501) staff       (20)      210 2023-04-25 16:03:04.000000 superset-iris-0.2.0/setup.py
-drwxr-xr-x   0 daimor     (501) staff       (20)        0 2023-04-27 06:46:11.836145 superset-iris-0.2.0/superset_iris/
--rw-r--r--   0 daimor     (501) staff       (20)        0 2023-04-16 12:31:18.000000 superset-iris-0.2.0/superset_iris/__init__.py
--rw-r--r--   0 daimor     (501) staff       (20)     3782 2023-04-26 09:34:49.000000 superset-iris-0.2.0/superset_iris/engine.py
-drwxr-xr-x   0 daimor     (501) staff       (20)        0 2023-04-27 06:46:11.837294 superset-iris-0.2.0/superset_iris.egg-info/
--rw-r--r--   0 daimor     (501) staff       (20)     3153 2023-04-27 06:46:11.000000 superset-iris-0.2.0/superset_iris.egg-info/PKG-INFO
--rw-r--r--   0 daimor     (501) staff       (20)      310 2023-04-27 06:46:11.000000 superset-iris-0.2.0/superset_iris.egg-info/SOURCES.txt
--rw-r--r--   0 daimor     (501) staff       (20)        1 2023-04-27 06:46:11.000000 superset-iris-0.2.0/superset_iris.egg-info/dependency_links.txt
--rw-r--r--   0 daimor     (501) staff       (20)       70 2023-04-27 06:46:11.000000 superset-iris-0.2.0/superset_iris.egg-info/entry_points.txt
--rw-r--r--   0 daimor     (501) staff       (20)       23 2023-04-27 06:46:11.000000 superset-iris-0.2.0/superset_iris.egg-info/requires.txt
--rw-r--r--   0 daimor     (501) staff       (20)       14 2023-04-27 06:46:11.000000 superset-iris-0.2.0/superset_iris.egg-info/top_level.txt
+drwxr-xr-x   0 daimor     (501) staff       (20)        0 2023-05-02 13:32:40.463070 superset-iris-0.3.0/
+-rw-r--r--   0 daimor     (501) staff       (20)     1075 2023-04-16 14:41:10.000000 superset-iris-0.3.0/LICENSE
+-rw-r--r--   0 daimor     (501) staff       (20)     3153 2023-05-02 13:32:40.463163 superset-iris-0.3.0/PKG-INFO
+-rw-r--r--   0 daimor     (501) staff       (20)     2209 2023-04-18 09:21:31.000000 superset-iris-0.3.0/README.md
+-rw-r--r--   0 daimor     (501) staff       (20)      933 2023-05-02 13:32:40.463483 superset-iris-0.3.0/setup.cfg
+-rw-r--r--   0 daimor     (501) staff       (20)      211 2023-04-30 18:39:17.000000 superset-iris-0.3.0/setup.py
+drwxr-xr-x   0 daimor     (501) staff       (20)        0 2023-05-02 13:32:40.462030 superset-iris-0.3.0/superset_iris/
+-rw-r--r--   0 daimor     (501) staff       (20)        0 2023-04-16 12:31:18.000000 superset-iris-0.3.0/superset_iris/__init__.py
+-rw-r--r--   0 daimor     (501) staff       (20)     3782 2023-04-26 09:34:49.000000 superset-iris-0.3.0/superset_iris/engine.py
+drwxr-xr-x   0 daimor     (501) staff       (20)        0 2023-05-02 13:32:40.462965 superset-iris-0.3.0/superset_iris.egg-info/
+-rw-r--r--   0 daimor     (501) staff       (20)     3153 2023-05-02 13:32:40.000000 superset-iris-0.3.0/superset_iris.egg-info/PKG-INFO
+-rw-r--r--   0 daimor     (501) staff       (20)      310 2023-05-02 13:32:40.000000 superset-iris-0.3.0/superset_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 daimor     (501) staff       (20)        1 2023-05-02 13:32:40.000000 superset-iris-0.3.0/superset_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 daimor     (501) staff       (20)       70 2023-05-02 13:32:40.000000 superset-iris-0.3.0/superset_iris.egg-info/entry_points.txt
+-rw-r--r--   0 daimor     (501) staff       (20)       24 2023-05-02 13:32:40.000000 superset-iris-0.3.0/superset_iris.egg-info/requires.txt
+-rw-r--r--   0 daimor     (501) staff       (20)       14 2023-05-02 13:32:40.000000 superset-iris-0.3.0/superset_iris.egg-info/top_level.txt
```

### Comparing `superset-iris-0.2.0/LICENSE` & `superset-iris-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `superset-iris-0.2.0/PKG-INFO` & `superset-iris-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superset-iris
-Version: 0.2.0
+Version: 0.3.0
 Summary: InterSystems IRIS Engine for Apache Superset
 Home-page: https://github.com/caretdev/superset-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/superset-iris
 Project-URL: Tracker, https://github.com/caretdev/superset-iris/issues
```

### Comparing `superset-iris-0.2.0/README.md` & `superset-iris-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `superset-iris-0.2.0/setup.cfg` & `superset-iris-0.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = superset-iris
-version = 0.2.0
+version = 0.3.0
 description = InterSystems IRIS Engine for Apache Superset
 long_description = file: README.md
 url = https://github.com/caretdev/superset-iris
 maintainer = CaretDev
 maintainer_email = dmitry@caretdev.com
 license = MIT
 long_description_content_type = text/markdown
```

### Comparing `superset-iris-0.2.0/superset_iris/engine.py` & `superset-iris-0.3.0/superset_iris/engine.py`

 * *Files identical despite different names*

### Comparing `superset-iris-0.2.0/superset_iris.egg-info/PKG-INFO` & `superset-iris-0.3.0/superset_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superset-iris
-Version: 0.2.0
+Version: 0.3.0
 Summary: InterSystems IRIS Engine for Apache Superset
 Home-page: https://github.com/caretdev/superset-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/superset-iris
 Project-URL: Tracker, https://github.com/caretdev/superset-iris/issues
```

