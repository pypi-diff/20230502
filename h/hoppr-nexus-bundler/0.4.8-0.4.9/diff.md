# Comparing `tmp/hoppr_nexus_bundler-0.4.8.tar.gz` & `tmp/hoppr_nexus_bundler-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_nexus_bundler-0.4.8.tar", max compression
+gzip compressed data, was "hoppr_nexus_bundler-0.4.9.tar", max compression
```

## Comparing `hoppr_nexus_bundler-0.4.8.tar` & `hoppr_nexus_bundler-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1084 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/LICENSE
--rw-r--r--   0        0        0     1694 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/README.md
--rw-r--r--   0        0        0       89 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/__init__.py
--rw-r--r--   0        0        0     7034 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/bundler.py
--rw-r--r--   0        0        0     1998 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/nexus_instance.py
--rw-r--r--   0        0        0        0 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/__init__.py
--rw-r--r--   0        0        0     4373 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/apt_publisher.py
--rw-r--r--   0        0        0     9569 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/base_publisher.py
--rw-r--r--   0        0        0     6265 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/docker_publisher.py
--rw-r--r--   0        0        0     2278 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/git_publisher.py
--rw-r--r--   0        0        0      833 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/helm_publisher.py
--rw-r--r--   0        0        0     1873 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/maven_publisher.py
--rw-r--r--   0        0        0        0 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/py.typed
--rw-r--r--   0        0        0      832 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/pypi_publisher.py
--rw-r--r--   0        0        0     1861 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/raw_publisher.py
--rw-r--r--   0        0        0     5741 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/yum_publisher.py
--rw-r--r--   0        0        0        0 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/nexus_bundler/py.typed
--rw-r--r--   0        0        0     1164 2023-04-26 16:10:05.000000 hoppr_nexus_bundler-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1694 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/README.md
+-rw-r--r--   0        0        0       89 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/__init__.py
+-rw-r--r--   0        0        0     7034 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/bundler.py
+-rw-r--r--   0        0        0     1998 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/nexus_instance.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/__init__.py
+-rw-r--r--   0        0        0     4373 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/apt_publisher.py
+-rw-r--r--   0        0        0     9569 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/base_publisher.py
+-rw-r--r--   0        0        0     6265 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/docker_publisher.py
+-rw-r--r--   0        0        0     2278 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/git_publisher.py
+-rw-r--r--   0        0        0      833 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/helm_publisher.py
+-rw-r--r--   0        0        0     1873 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/maven_publisher.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/py.typed
+-rw-r--r--   0        0        0      832 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/pypi_publisher.py
+-rw-r--r--   0        0        0     1861 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/raw_publisher.py
+-rw-r--r--   0        0        0     5741 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/yum_publisher.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.4.9/PKG-INFO
```

### Comparing `hoppr_nexus_bundler-0.4.8/LICENSE` & `hoppr_nexus_bundler-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/README.md` & `hoppr_nexus_bundler-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/bundler.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/bundler.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/nexus_instance.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/nexus_instance.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/apt_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/apt_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/base_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/base_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/docker_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/docker_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/git_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/git_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/helm_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/helm_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/maven_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/maven_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/pypi_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/pypi_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/raw_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/raw_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/nexus_bundler/publishers/yum_publisher.py` & `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/yum_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.8/pyproject.toml` & `hoppr_nexus_bundler-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr_nexus_bundler"
-version = "0.4.8"
+version = "0.4.9"
 description = "Plug-in for Hoppr to bundle artifacts into a Nexus Repository"
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev/"
 repository = "https://gitlab.com/-/ide/project/lmco/hoppr/plugins/hoppr-nexus-bundler"
```

### Comparing `hoppr_nexus_bundler-0.4.8/PKG-INFO` & `hoppr_nexus_bundler-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-nexus-bundler
-Version: 0.4.8
+Version: 0.4.9
 Summary: Plug-in for Hoppr to bundle artifacts into a Nexus Repository
 Home-page: https://hoppr.dev/
 License: MIT
 Keywords: hoppr,plugin,nexus
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

