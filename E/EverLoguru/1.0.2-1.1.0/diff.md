# Comparing `tmp/EverLoguru-1.0.2.tar.gz` & `tmp/EverLoguru-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EverLoguru-1.0.2.tar", last modified: Tue May  2 06:24:45 2023, max compression
+gzip compressed data, was "EverLoguru-1.1.0.tar", last modified: Tue May  2 07:07:23 2023, max compression
```

## Comparing `EverLoguru-1.0.2.tar` & `EverLoguru-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 06:24:45.951694 EverLoguru-1.0.2/
-drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 06:24:45.950694 EverLoguru-1.0.2/EverLoguru.egg-info/
--rw-r--r--   0 cyan      (1000) cyan      (1000)      200 2023-05-02 06:24:45.000000 EverLoguru-1.0.2/EverLoguru.egg-info/PKG-INFO
--rw-r--r--   0 cyan      (1000) cyan      (1000)      247 2023-05-02 06:24:45.000000 EverLoguru-1.0.2/EverLoguru.egg-info/SOURCES.txt
--rw-r--r--   0 cyan      (1000) cyan      (1000)        1 2023-05-02 06:24:45.000000 EverLoguru-1.0.2/EverLoguru.egg-info/dependency_links.txt
--rw-r--r--   0 cyan      (1000) cyan      (1000)       12 2023-05-02 06:24:45.000000 EverLoguru-1.0.2/EverLoguru.egg-info/top_level.txt
--rw-r--r--   0 cyan      (1000) cyan      (1000)      200 2023-05-02 06:24:45.951694 EverLoguru-1.0.2/PKG-INFO
--rw-r--r--   0 cyan      (1000) cyan      (1000)      126 2023-05-02 05:31:52.000000 EverLoguru-1.0.2/README.md
-drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 06:24:45.950694 EverLoguru-1.0.2/ever_loguru/
--rw-r--r--   0 cyan      (1000) cyan      (1000)       46 2023-05-02 05:18:42.000000 EverLoguru-1.0.2/ever_loguru/__init__.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)      916 2023-05-02 05:16:00.000000 EverLoguru-1.0.2/ever_loguru/handler.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)     2066 2023-05-02 06:23:10.000000 EverLoguru-1.0.2/ever_loguru/install.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)      727 2023-05-02 05:28:28.000000 EverLoguru-1.0.2/ever_loguru/wrapper.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)       38 2023-05-02 06:24:45.951694 EverLoguru-1.0.2/setup.cfg
--rw-r--r--   0 cyan      (1000) cyan      (1000)      304 2023-05-02 06:24:01.000000 EverLoguru-1.0.2/setup.py
+drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/
+drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/EverLoguru.egg-info/
+-rw-r--r--   0 cyan      (1000) cyan      (1000)     2002 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/PKG-INFO
+-rw-r--r--   0 cyan      (1000) cyan      (1000)      262 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/SOURCES.txt
+-rw-r--r--   0 cyan      (1000) cyan      (1000)        1 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/dependency_links.txt
+-rw-r--r--   0 cyan      (1000) cyan      (1000)       12 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/top_level.txt
+-rw-r--r--   0 cyan      (1000) cyan      (1000)     2002 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/PKG-INFO
+-rw-r--r--   0 cyan      (1000) cyan      (1000)     1468 2023-05-02 07:01:03.000000 EverLoguru-1.1.0/README.md
+drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/ever_loguru/
+-rw-r--r--   0 cyan      (1000) cyan      (1000)       46 2023-05-02 05:18:42.000000 EverLoguru-1.1.0/ever_loguru/__init__.py
+-rw-r--r--   0 cyan      (1000) cyan      (1000)      916 2023-05-02 05:16:00.000000 EverLoguru-1.1.0/ever_loguru/handler.py
+-rw-r--r--   0 cyan      (1000) cyan      (1000)     2066 2023-05-02 06:23:10.000000 EverLoguru-1.1.0/ever_loguru/install.py
+-rw-r--r--   0 cyan      (1000) cyan      (1000)      727 2023-05-02 05:28:28.000000 EverLoguru-1.1.0/ever_loguru/wrapper.py
+-rw-r--r--   0 cyan      (1000) cyan      (1000)      597 2023-05-02 07:06:19.000000 EverLoguru-1.1.0/pyproject.toml
+-rw-r--r--   0 cyan      (1000) cyan      (1000)       38 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/setup.cfg
+-rw-r--r--   0 cyan      (1000) cyan      (1000)      407 2023-05-02 07:05:12.000000 EverLoguru-1.1.0/setup.py
```

### Comparing `EverLoguru-1.0.2/ever_loguru/handler.py` & `EverLoguru-1.1.0/ever_loguru/handler.py`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.0.2/ever_loguru/install.py` & `EverLoguru-1.1.0/ever_loguru/install.py`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.0.2/ever_loguru/wrapper.py` & `EverLoguru-1.1.0/ever_loguru/wrapper.py`

 * *Files identical despite different names*

