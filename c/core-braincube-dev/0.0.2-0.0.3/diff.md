# Comparing `tmp/core-braincube-dev-0.0.2.tar.gz` & `tmp/core-braincube-dev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-braincube-dev-0.0.2.tar", last modified: Tue May  2 11:07:05 2023, max compression
+gzip compressed data, was "core-braincube-dev-0.0.3.tar", last modified: Tue May  2 11:34:58 2023, max compression
```

## Comparing `core-braincube-dev-0.0.2.tar` & `core-braincube-dev-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.687977 core-braincube-dev-0.0.2/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.2/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      643 2023-05-02 11:07:05.687486 core-braincube-dev-0.0.2/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4275 2023-05-02 09:47:16.000000 core-braincube-dev-0.0.2/README.md
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.668061 core-braincube-dev-0.0.2/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.670118 core-braincube-dev-0.0.2/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.672361 core-braincube-dev-0.0.2/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.675272 core-braincube-dev-0.0.2/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.2/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.678242 core-braincube-dev-0.0.2/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.2/core/utils/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:07:05.684795 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      643 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      594 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       24 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:07:05.000000 core-braincube-dev-0.0.2/core_braincube_dev.egg-info/top_level.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:07:05.688129 core-braincube-dev-0.0.2/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      848 2023-05-02 11:02:02.000000 core-braincube-dev-0.0.2/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.080685 core-braincube-dev-0.0.3/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.3/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:34:58.080900 core-braincube-dev-0.0.3/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4275 2023-05-02 09:47:16.000000 core-braincube-dev-0.0.3/README.rst
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.072860 core-braincube-dev-0.0.3/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.074420 core-braincube-dev-0.0.3/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.075515 core-braincube-dev-0.0.3/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.076799 core-braincube-dev-0.0.3/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.3/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.077901 core-braincube-dev-0.0.3/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.3/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 11:34:58.080176 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      903 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      605 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 11:34:58.000000 core-braincube-dev-0.0.3/core_braincube_dev.egg-info/top_level.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      940 2023-05-02 11:34:58.081805 core-braincube-dev-0.0.3/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.3/setup.py
```

### Comparing `core-braincube-dev-0.0.2/LICENSE` & `core-braincube-dev-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/README.md` & `core-braincube-dev-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/dal/data.py` & `core-braincube-dev-0.0.3/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/dal/postgres_connection.py` & `core-braincube-dev-0.0.3/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/dal/postgres_repository.py` & `core-braincube-dev-0.0.3/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/di/data.py` & `core-braincube-dev-0.0.3/core/di/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/di/injector.py` & `core-braincube-dev-0.0.3/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/rest/app_controller.py` & `core-braincube-dev-0.0.3/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/rest/app_module.py` & `core-braincube-dev-0.0.3/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/rest/data.py` & `core-braincube-dev-0.0.3/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/utils/convert.py` & `core-braincube-dev-0.0.3/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.2/core/utils/data.py` & `core-braincube-dev-0.0.3/core/utils/data.py`

 * *Files identical despite different names*

