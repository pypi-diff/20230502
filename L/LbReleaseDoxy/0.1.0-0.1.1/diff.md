# Comparing `tmp/LbReleaseDoxy-0.1.0.tar.gz` & `tmp/LbReleaseDoxy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbReleaseDoxy-0.1.0.tar", last modified: Tue May  2 13:25:37 2023, max compression
+gzip compressed data, was "LbReleaseDoxy-0.1.1.tar", last modified: Tue May  2 14:06:23 2023, max compression
```

## Comparing `LbReleaseDoxy-0.1.0.tar` & `LbReleaseDoxy-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 13:25:37.016771 LbReleaseDoxy-0.1.0/
-drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 13:25:37.012771 LbReleaseDoxy-0.1.0/LbRelease/
-drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 13:25:37.012771 LbReleaseDoxy-0.1.0/LbRelease/_LHCbDocResources/
--rw-r--r--   0 pnogga    (1000) pnogga    (1000)     2456 2023-05-02 13:18:32.000000 LbReleaseDoxy-0.1.0/LbRelease/_LHCbDocResources/__init__.py
--rw-r--r--   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 13:20:01.000000 LbReleaseDoxy-0.1.0/LbRelease/__init__.py
-drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 13:25:37.012771 LbReleaseDoxy-0.1.0/LbReleaseDoxy.egg-info/
--rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      428 2023-05-02 13:25:37.000000 LbReleaseDoxy-0.1.0/LbReleaseDoxy.egg-info/PKG-INFO
--rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      218 2023-05-02 13:25:37.000000 LbReleaseDoxy-0.1.0/LbReleaseDoxy.egg-info/SOURCES.txt
--rw-rw-r--   0 pnogga    (1000) pnogga    (1000)        1 2023-05-02 13:25:37.000000 LbReleaseDoxy-0.1.0/LbReleaseDoxy.egg-info/dependency_links.txt
--rw-rw-r--   0 pnogga    (1000) pnogga    (1000)       10 2023-05-02 13:25:37.000000 LbReleaseDoxy-0.1.0/LbReleaseDoxy.egg-info/top_level.txt
--rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      428 2023-05-02 13:25:37.016771 LbReleaseDoxy-0.1.0/PKG-INFO
--rw-rw-r--   0 pnogga    (1000) pnogga    (1000)       38 2023-05-02 13:25:37.016771 LbReleaseDoxy-0.1.0/setup.cfg
--rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      627 2023-05-02 13:25:02.000000 LbReleaseDoxy-0.1.0/setup.py
+drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 14:06:23.034750 LbReleaseDoxy-0.1.1/
+drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 14:06:23.030750 LbReleaseDoxy-0.1.1/LbRelease/
+drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 14:06:23.030750 LbReleaseDoxy-0.1.1/LbRelease/_LHCbDocResources/
+-rw-r--r--   0 pnogga    (1000) pnogga    (1000)     2456 2023-05-02 13:18:32.000000 LbReleaseDoxy-0.1.1/LbRelease/_LHCbDocResources/__init__.py
+-rw-r--r--   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 13:20:01.000000 LbReleaseDoxy-0.1.1/LbRelease/__init__.py
+drwxrwxr-x   0 pnogga    (1000) pnogga    (1000)        0 2023-05-02 14:06:23.030750 LbReleaseDoxy-0.1.1/LbReleaseDoxy.egg-info/
+-rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      428 2023-05-02 14:06:23.000000 LbReleaseDoxy-0.1.1/LbReleaseDoxy.egg-info/PKG-INFO
+-rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      218 2023-05-02 14:06:23.000000 LbReleaseDoxy-0.1.1/LbReleaseDoxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 pnogga    (1000) pnogga    (1000)        1 2023-05-02 14:06:23.000000 LbReleaseDoxy-0.1.1/LbReleaseDoxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 pnogga    (1000) pnogga    (1000)       10 2023-05-02 14:06:23.000000 LbReleaseDoxy-0.1.1/LbReleaseDoxy.egg-info/top_level.txt
+-rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      428 2023-05-02 14:06:23.030750 LbReleaseDoxy-0.1.1/PKG-INFO
+-rw-rw-r--   0 pnogga    (1000) pnogga    (1000)       38 2023-05-02 14:06:23.034750 LbReleaseDoxy-0.1.1/setup.cfg
+-rw-rw-r--   0 pnogga    (1000) pnogga    (1000)      928 2023-05-02 14:06:07.000000 LbReleaseDoxy-0.1.1/setup.py
```

### Comparing `LbReleaseDoxy-0.1.0/LbRelease/_LHCbDocResources/__init__.py` & `LbReleaseDoxy-0.1.1/LbRelease/_LHCbDocResources/__init__.py`

 * *Files identical despite different names*

