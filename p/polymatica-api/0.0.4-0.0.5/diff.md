# Comparing `tmp/polymatica_api-0.0.4.tar.gz` & `tmp/polymatica_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.0.4.tar", last modified: Tue May  2 08:04:15 2023, max compression
+gzip compressed data, was "polymatica_api-0.0.5.tar", last modified: Tue May  2 10:57:30 2023, max compression
```

## Comparing `polymatica_api-0.0.4.tar` & `polymatica_api-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:04:15.287929 polymatica_api-0.0.4/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.4/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)      191 2023-05-02 08:04:15.287752 polymatica_api-0.0.4/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)        0 2023-05-02 01:52:15.000000 polymatica_api-0.0.4/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:04:15.286026 polymatica_api-0.0.4/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     1463 2023-05-02 07:39:36.000000 polymatica_api-0.0.4/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.4/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)      838 2023-05-02 07:39:25.000000 polymatica_api-0.0.4/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:04:15.287098 polymatica_api-0.0.4/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)      191 2023-05-02 08:04:15.000000 polymatica_api-0.0.4/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      315 2023-05-02 08:04:15.000000 polymatica_api-0.0.4/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-02 08:04:15.000000 polymatica_api-0.0.4/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-02 08:04:15.000000 polymatica_api-0.0.4/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-02 08:04:15.000000 polymatica_api-0.0.4/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-02 08:04:15.287984 polymatica_api-0.0.4/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-02 08:04:06.000000 polymatica_api-0.0.4/setup.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 08:04:15.287285 polymatica_api-0.0.4/tests/
--rw-r--r--   0 leggnom    (501) staff       (20)      508 2023-05-02 07:14:02.000000 polymatica_api-0.0.4/tests/test_base.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.856598 polymatica_api-0.0.5/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.5/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)      731 2023-05-02 10:57:30.856471 polymatica_api-0.0.5/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      538 2023-05-02 10:56:35.000000 polymatica_api-0.0.5/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.855290 polymatica_api-0.0.5/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1463 2023-05-02 07:39:36.000000 polymatica_api-0.0.5/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.5/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      838 2023-05-02 07:39:25.000000 polymatica_api-0.0.5/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.856049 polymatica_api-0.0.5/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)      731 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      315 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-02 10:57:30.856634 polymatica_api-0.0.5/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-02 10:57:24.000000 polymatica_api-0.0.5/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.856164 polymatica_api-0.0.5/tests/
+-rw-r--r--   0 leggnom    (501) staff       (20)      508 2023-05-02 07:14:02.000000 polymatica_api-0.0.5/tests/test_base.py
```

### Comparing `polymatica_api-0.0.4/LICENSE` & `polymatica_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.4/polymatica_api/__init__.py` & `polymatica_api-0.0.5/polymatica_api/__init__.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.4/polymatica_api/data_option.py` & `polymatica_api-0.0.5/polymatica_api/data_option.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.4/polymatica_api/types.py` & `polymatica_api-0.0.5/polymatica_api/types.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.4/setup.py` & `polymatica_api-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.0.4",
+    version="0.0.5",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

