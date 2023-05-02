# Comparing `tmp/HACNet-1.3.3.tar.gz` & `tmp/HACNet-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HACNet-1.3.3.tar", last modified: Sat Apr 15 15:42:41 2023, max compression
+gzip compressed data, was "HACNet-1.4.0.tar", last modified: Tue May  2 17:14:20 2023, max compression
```

## Comparing `HACNet-1.3.3.tar` & `HACNet-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 15:42:41.355286 HACNet-1.3.3/
-drwxrwxrwx   0        0        0        0 2023-04-15 15:42:41.324045 HACNet-1.3.3/HACNet/
--rw-rw-rw-   0        0        0    14950 2023-04-15 15:42:21.000000 HACNet-1.3.3/HACNet/CNN.py
--rw-rw-rw-   0        0        0    15340 2023-04-15 15:42:22.000000 HACNet-1.3.3/HACNet/GCN.py
--rw-rw-rw-   0        0        0     8898 2023-04-15 15:42:22.000000 HACNet-1.3.3/HACNet/MLP.py
--rw-rw-rw-   0        0        0        2 2023-04-15 15:42:22.000000 HACNet-1.3.3/HACNet/__init__.py
--rw-rw-rw-   0        0        0    16922 2023-04-15 15:42:22.000000 HACNet-1.3.3/HACNet/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-15 15:42:41.355286 HACNet-1.3.3/HACNet.egg-info/
--rw-rw-rw-   0        0        0      319 2023-04-15 15:42:41.000000 HACNet-1.3.3/HACNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-15 15:42:41.000000 HACNet-1.3.3/HACNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 15:42:41.000000 HACNet-1.3.3/HACNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 15:42:41.000000 HACNet-1.3.3/HACNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2023-04-15 15:42:23.000000 HACNet-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      319 2023-04-15 15:42:41.355286 HACNet-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3536 2023-04-15 15:42:23.000000 HACNet-1.3.3/README.md
--rw-rw-rw-   0        0        0       86 2023-04-15 15:42:41.355286 HACNet-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      444 2023-04-15 15:42:23.000000 HACNet-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:14:20.035785 HACNet-1.4.0/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:14:19.946026 HACNet-1.4.0/HACNet/
+-rw-rw-rw-   0        0        0    14950 2023-05-02 17:13:22.000000 HACNet-1.4.0/HACNet/CNN.py
+-rw-rw-rw-   0        0        0    15340 2023-05-02 17:13:22.000000 HACNet-1.4.0/HACNet/GCN.py
+-rw-rw-rw-   0        0        0     8898 2023-05-02 17:13:22.000000 HACNet-1.4.0/HACNet/MLP.py
+-rw-rw-rw-   0        0        0        2 2023-05-02 17:13:22.000000 HACNet-1.4.0/HACNet/__init__.py
+-rw-rw-rw-   0        0        0    55425 2023-05-02 17:13:22.000000 HACNet-1.4.0/HACNet/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:14:20.033790 HACNet-1.4.0/HACNet.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-05-02 17:14:18.000000 HACNet-1.4.0/HACNet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-02 17:14:18.000000 HACNet-1.4.0/HACNet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:14:18.000000 HACNet-1.4.0/HACNet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 17:14:18.000000 HACNet-1.4.0/HACNet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2023-05-02 17:13:23.000000 HACNet-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      373 2023-05-02 17:14:20.036782 HACNet-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3536 2023-05-02 17:13:23.000000 HACNet-1.4.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-02 17:14:20.039774 HACNet-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-05-02 17:13:23.000000 HACNet-1.4.0/setup.py
```

### Comparing `HACNet-1.3.3/HACNet/CNN.py` & `HACNet-1.4.0/HACNet/CNN.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.3.3/HACNet/GCN.py` & `HACNet-1.4.0/HACNet/GCN.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.3.3/HACNet/MLP.py` & `HACNet-1.4.0/HACNet/MLP.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.3.3/LICENSE` & `HACNet-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HACNet-1.3.3/README.md` & `HACNet-1.4.0/README.md`

 * *Files identical despite different names*

