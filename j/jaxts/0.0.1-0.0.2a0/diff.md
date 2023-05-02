# Comparing `tmp/jaxts-0.0.1.tar.gz` & `tmp/jaxts-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxts-0.0.1.tar", max compression
+gzip compressed data, was "jaxts-0.0.2a0.tar", max compression
```

## Comparing `jaxts-0.0.1.tar` & `jaxts-0.0.2a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-01 01:04:12.513180 jaxts-0.0.1/LICENSE
--rw-r--r--   0        0        0       52 2023-05-01 01:16:53.903782 jaxts-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-01 01:30:05.651265 jaxts-0.0.1/jaxts/SSM/__init__.py
--rw-r--r--   0        0        0      227 2023-05-01 01:32:23.772050 jaxts-0.0.1/jaxts/SSM/base.py
--rw-r--r--   0        0        0      307 2023-05-01 01:37:19.170396 jaxts-0.0.1/jaxts/SSM/dglm.py
--rw-r--r--   0        0        0      318 2023-05-01 01:37:19.167020 jaxts-0.0.1/jaxts/SSM/dlm.py
--rw-r--r--   0        0        0        0 2023-05-01 01:27:55.664006 jaxts-0.0.1/jaxts/__init__.py
--rw-r--r--   0        0        0      454 2023-05-02 00:40:24.134034 jaxts-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 jaxts-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-01 01:04:12.513180 jaxts-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0       52 2023-05-01 01:16:53.903782 jaxts-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 01:30:05.651265 jaxts-0.0.2a0/jaxts/SSM/__init__.py
+-rw-r--r--   0        0        0      227 2023-05-01 01:32:23.772050 jaxts-0.0.2a0/jaxts/SSM/base.py
+-rw-r--r--   0        0        0      307 2023-05-01 01:37:19.170396 jaxts-0.0.2a0/jaxts/SSM/dglm.py
+-rw-r--r--   0        0        0      318 2023-05-01 01:37:19.167020 jaxts-0.0.2a0/jaxts/SSM/dlm.py
+-rw-r--r--   0        0        0        0 2023-05-01 01:27:55.664006 jaxts-0.0.2a0/jaxts/__init__.py
+-rw-r--r--   0        0        0      456 2023-05-02 01:00:33.338113 jaxts-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 jaxts-0.0.2a0/PKG-INFO
```

### Comparing `jaxts-0.0.1/LICENSE` & `jaxts-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxts-0.0.1/PKG-INFO` & `jaxts-0.0.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxts
-Version: 0.0.1
+Version: 0.0.2a0
 Summary: A Jax based python package for time series
 Home-page: https://github.com/michaelellis003/JaxTS
 License: MIT
 Keywords: Time Series,State Space Models,Dynamic Linear Models
 Author: Michael Ellis
 Author-email: michael@mlellis.com
 Requires-Python: >=3.11,<4.0
```

