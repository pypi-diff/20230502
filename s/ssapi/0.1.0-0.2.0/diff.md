# Comparing `tmp/ssapi-0.1.0.tar.gz` & `tmp/ssapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssapi-0.1.0.tar", last modified: Sun Apr 30 12:12:41 2023, max compression
+gzip compressed data, was "ssapi-0.2.0.tar", last modified: Tue May  2 20:12:05 2023, max compression
```

## Comparing `ssapi-0.1.0.tar` & `ssapi-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-04-30 12:12:41.738433 ssapi-0.1.0/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-04-30 12:12:41.738433 ssapi-0.1.0/PKG-INFO
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-04-30 12:12:41.735432 ssapi-0.1.0/scripts/
--rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.1.0/scripts/ssapi-web
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-04-30 12:12:41.739433 ssapi-0.1.0/setup.cfg
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      272 2023-04-29 09:12:22.000000 ssapi-0.1.0/setup.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-04-30 12:12:41.735432 ssapi-0.1.0/src/
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-04-30 12:12:41.737433 ssapi-0.1.0/src/ssapi/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.1.0/src/ssapi/__init__.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)     2596 2023-04-30 11:02:56.000000 ssapi-0.1.0/src/ssapi/db.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      202 2023-04-30 07:47:30.000000 ssapi-0.1.0/src/ssapi/defaults.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      715 2023-04-30 10:33:43.000000 ssapi-0.1.0/src/ssapi/entities.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.1.0/src/ssapi/env.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1309 2023-04-30 10:58:00.000000 ssapi-0.1.0/src/ssapi/relational.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      540 2023-04-30 11:18:15.000000 ssapi-0.1.0/src/ssapi/types.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)     1132 2023-04-30 11:05:05.000000 ssapi-0.1.0/src/ssapi/web.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      927 2023-04-30 10:39:01.000000 ssapi-0.1.0/src/ssapi/web_decorators.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      427 2023-04-30 09:55:14.000000 ssapi-0.1.0/src/ssapi/web_tools.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-04-30 12:12:41.738433 ssapi-0.1.0/src/ssapi.egg-info/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-04-30 12:12:41.000000 ssapi-0.1.0/src/ssapi.egg-info/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      400 2023-04-30 12:12:41.000000 ssapi-0.1.0/src/ssapi.egg-info/SOURCES.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-04-30 12:12:41.000000 ssapi-0.1.0/src/ssapi.egg-info/dependency_links.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-04-30 12:12:41.000000 ssapi-0.1.0/src/ssapi.egg-info/requires.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-04-30 12:12:41.000000 ssapi-0.1.0/src/ssapi.egg-info/top_level.txt
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.477158 ssapi-0.2.0/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-05-02 20:12:05.477158 ssapi-0.2.0/PKG-INFO
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.474158 ssapi-0.2.0/scripts/
+-rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.2.0/scripts/ssapi-web
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-05-02 20:12:05.477158 ssapi-0.2.0/setup.cfg
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      272 2023-05-02 20:11:58.000000 ssapi-0.2.0/setup.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.473158 ssapi-0.2.0/src/
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.476158 ssapi-0.2.0/src/ssapi/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.2.0/src/ssapi/__init__.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)     2596 2023-04-30 11:02:56.000000 ssapi-0.2.0/src/ssapi/db.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      202 2023-04-30 07:47:30.000000 ssapi-0.2.0/src/ssapi/defaults.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      715 2023-04-30 10:33:43.000000 ssapi-0.2.0/src/ssapi/entities.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.2.0/src/ssapi/env.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1309 2023-04-30 10:58:00.000000 ssapi-0.2.0/src/ssapi/relational.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      540 2023-04-30 11:18:15.000000 ssapi-0.2.0/src/ssapi/types.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)     1248 2023-04-30 13:51:41.000000 ssapi-0.2.0/src/ssapi/web.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      927 2023-04-30 10:39:01.000000 ssapi-0.2.0/src/ssapi/web_decorators.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      427 2023-04-30 09:55:14.000000 ssapi-0.2.0/src/ssapi/web_tools.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-05-02 20:12:05.477158 ssapi-0.2.0/src/ssapi.egg-info/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      400 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/requires.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-05-02 20:12:05.000000 ssapi-0.2.0/src/ssapi.egg-info/top_level.txt
```

### Comparing `ssapi-0.1.0/src/ssapi/db.py` & `ssapi-0.2.0/src/ssapi/db.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.1.0/src/ssapi/entities.py` & `ssapi-0.2.0/src/ssapi/entities.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.1.0/src/ssapi/env.py` & `ssapi-0.2.0/src/ssapi/env.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.1.0/src/ssapi/relational.py` & `ssapi-0.2.0/src/ssapi/relational.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.1.0/src/ssapi/types.py` & `ssapi-0.2.0/src/ssapi/types.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.1.0/src/ssapi/web_decorators.py` & `ssapi-0.2.0/src/ssapi/web_decorators.py`

 * *Files identical despite different names*

