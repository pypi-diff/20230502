# Comparing `tmp/easy_reed-0.1.5.tar.gz` & `tmp/easy_reed-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_reed-0.1.5.tar", last modified: Fri Apr  7 20:31:50 2023, max compression
+gzip compressed data, was "easy_reed-0.9.0.tar", last modified: Tue May  2 03:39:43 2023, max compression
```

## Comparing `easy_reed-0.1.5.tar` & `easy_reed-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-04-07 20:31:50.430915 easy_reed-0.1.5/
--rw-r--r--   0 reed      (1000) reed      (1000)    35128 2023-04-05 22:29:50.000000 easy_reed-0.1.5/LICENSE.txt
--rw-r--r--   0 reed      (1000) reed      (1000)      253 2023-04-07 20:31:50.430915 easy_reed-0.1.5/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)       90 2023-04-05 22:12:15.000000 easy_reed-0.1.5/README.md
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-04-07 20:31:50.430915 easy_reed-0.1.5/easy_reed/
--rw-r--r--   0 reed      (1000) reed      (1000)       17 2023-04-05 22:12:15.000000 easy_reed-0.1.5/easy_reed/__init__.py
--rw-r--r--   0 reed      (1000) reed      (1000)       21 2023-04-05 23:48:11.000000 easy_reed-0.1.5/easy_reed/_builder.py
--rw-r--r--   0 reed      (1000) reed      (1000)      694 2023-04-06 00:03:47.000000 easy_reed-0.1.5/easy_reed/config.py
--rw-r--r--   0 reed      (1000) reed      (1000)      277 2023-04-07 20:04:23.000000 easy_reed-0.1.5/easy_reed/namespace.py
-drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-04-07 20:31:50.430915 easy_reed-0.1.5/easy_reed.egg-info/
--rw-r--r--   0 reed      (1000) reed      (1000)      253 2023-04-07 20:31:50.000000 easy_reed-0.1.5/easy_reed.egg-info/PKG-INFO
--rw-r--r--   0 reed      (1000) reed      (1000)      264 2023-04-07 20:31:50.000000 easy_reed-0.1.5/easy_reed.egg-info/SOURCES.txt
--rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-04-07 20:31:50.000000 easy_reed-0.1.5/easy_reed.egg-info/dependency_links.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       10 2023-04-07 20:31:50.000000 easy_reed-0.1.5/easy_reed.egg-info/top_level.txt
--rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-04-05 22:12:15.000000 easy_reed-0.1.5/pyproject.toml
--rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-04-07 20:31:50.430915 easy_reed-0.1.5/setup.cfg
--rw-r--r--   0 reed      (1000) reed      (1000)      484 2023-04-07 20:31:36.000000 easy_reed-0.1.5/setup.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 03:39:43.819616 easy_reed-0.9.0/
+-rw-r--r--   0 reed      (1000) reed      (1000)    35128 2023-04-05 22:29:50.000000 easy_reed-0.9.0/LICENSE.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)      253 2023-05-02 03:39:43.819616 easy_reed-0.9.0/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)       90 2023-04-05 22:12:15.000000 easy_reed-0.9.0/README.md
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 03:39:43.809616 easy_reed-0.9.0/easy_reed/
+-rw-r--r--   0 reed      (1000) reed      (1000)      781 2023-05-02 03:26:11.000000 easy_reed-0.9.0/easy_reed/__init__.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     1502 2023-05-02 03:26:49.000000 easy_reed-0.9.0/easy_reed/_logger.py
+-rw-r--r--   0 reed      (1000) reed      (1000)    12104 2023-05-01 22:27:00.000000 easy_reed-0.9.0/easy_reed/config_object.py
+-rw-r--r--   0 reed      (1000) reed      (1000)    11131 2023-04-26 19:15:42.000000 easy_reed-0.9.0/easy_reed/config_reader.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     5381 2023-05-02 03:25:44.000000 easy_reed-0.9.0/easy_reed/environment.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     7915 2023-04-28 16:17:58.000000 easy_reed-0.9.0/easy_reed/namespace.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 03:39:43.809616 easy_reed-0.9.0/easy_reed.egg-info/
+-rw-r--r--   0 reed      (1000) reed      (1000)      253 2023-05-02 03:39:43.000000 easy_reed-0.9.0/easy_reed.egg-info/PKG-INFO
+-rw-r--r--   0 reed      (1000) reed      (1000)      417 2023-05-02 03:39:43.000000 easy_reed-0.9.0/easy_reed.egg-info/SOURCES.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)        1 2023-05-02 03:39:43.000000 easy_reed-0.9.0/easy_reed.egg-info/dependency_links.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       10 2023-05-02 03:39:43.000000 easy_reed-0.9.0/easy_reed.egg-info/top_level.txt
+-rw-r--r--   0 reed      (1000) reed      (1000)       80 2023-04-05 22:12:15.000000 easy_reed-0.9.0/pyproject.toml
+-rw-r--r--   0 reed      (1000) reed      (1000)       38 2023-05-02 03:39:43.819616 easy_reed-0.9.0/setup.cfg
+-rw-r--r--   0 reed      (1000) reed      (1000)      484 2023-05-02 03:39:27.000000 easy_reed-0.9.0/setup.py
+drwxr-xr-x   0 reed      (1000) reed      (1000)        0 2023-05-02 03:39:43.809616 easy_reed-0.9.0/test/
+-rw-r--r--   0 reed      (1000) reed      (1000)     2258 2023-05-01 23:51:02.000000 easy_reed-0.9.0/test/test_config.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     6135 2023-04-28 19:29:10.000000 easy_reed-0.9.0/test/test_config_reader.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     3289 2023-04-16 19:59:10.000000 easy_reed-0.9.0/test/test_environment.py
+-rw-r--r--   0 reed      (1000) reed      (1000)     2270 2023-04-28 16:17:14.000000 easy_reed-0.9.0/test/test_namespace.py
```

### Comparing `easy_reed-0.1.5/LICENSE.txt` & `easy_reed-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

