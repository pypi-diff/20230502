# Comparing `tmp/polymatica_api-0.0.2.tar.gz` & `tmp/polymatica_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.0.2.tar", last modified: Tue May  2 07:40:29 2023, max compression
+gzip compressed data, was "polymatica_api-0.0.3.tar", last modified: Tue May  2 08:02:23 2023, max compression
```

## Comparing `polymatica_api-0.0.2.tar` & `polymatica_api-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 07:40:29.277702 polymatica_api-0.0.2/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.2/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)      191 2023-05-02 07:40:29.277512 polymatica_api-0.0.2/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)        0 2023-05-02 01:52:15.000000 polymatica_api-0.0.2/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 07:40:29.276035 polymatica_api-0.0.2/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     1463 2023-05-02 07:39:36.000000 polymatica_api-0.0.2/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.2/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)      838 2023-05-02 07:39:25.000000 polymatica_api-0.0.2/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 07:40:29.276933 polymatica_api-0.0.2/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)      191 2023-05-02 07:40:29.000000 polymatica_api-0.0.2/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      278 2023-05-02 07:40:29.000000 polymatica_api-0.0.2/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-02 07:40:29.000000 polymatica_api-0.0.2/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-02 07:40:29.000000 polymatica_api-0.0.2/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-02 07:40:29.277764 polymatica_api-0.0.2/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      499 2023-05-02 07:40:22.000000 polymatica_api-0.0.2/setup.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 07:40:29.277134 polymatica_api-0.0.2/tests/
--rw-r--r--   0 leggnom    (501) staff       (20)      508 2023-05-02 07:14:02.000000 polymatica_api-0.0.2/tests/test_base.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:02:23.993872 polymatica_api-0.0.3/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.3/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)      191 2023-05-02 08:02:23.993688 polymatica_api-0.0.3/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)        0 2023-05-02 01:52:15.000000 polymatica_api-0.0.3/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:02:23.992154 polymatica_api-0.0.3/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1463 2023-05-02 07:39:36.000000 polymatica_api-0.0.3/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.3/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      838 2023-05-02 07:39:25.000000 polymatica_api-0.0.3/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:02:23.993031 polymatica_api-0.0.3/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)      191 2023-05-02 08:02:23.000000 polymatica_api-0.0.3/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      278 2023-05-02 08:02:23.000000 polymatica_api-0.0.3/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-02 08:02:23.000000 polymatica_api-0.0.3/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-02 08:02:23.000000 polymatica_api-0.0.3/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-02 08:02:23.993931 polymatica_api-0.0.3/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      563 2023-05-02 08:02:13.000000 polymatica_api-0.0.3/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:02:23.993245 polymatica_api-0.0.3/tests/
+-rw-r--r--   0 leggnom    (501) staff       (20)      508 2023-05-02 07:14:02.000000 polymatica_api-0.0.3/tests/test_base.py
```

### Comparing `polymatica_api-0.0.2/LICENSE` & `polymatica_api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.2/polymatica_api/__init__.py` & `polymatica_api-0.0.3/polymatica_api/__init__.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.2/polymatica_api/data_option.py` & `polymatica_api-0.0.3/polymatica_api/data_option.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.2/polymatica_api/types.py` & `polymatica_api-0.0.3/polymatica_api/types.py`

 * *Files identical despite different names*

