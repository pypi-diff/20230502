# Comparing `tmp/async-polygon-sdk-1.tar.gz` & `tmp/async-polygon-sdk-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-polygon-sdk-1.tar", last modified: Tue May  2 00:29:34 2023, max compression
+gzip compressed data, was "async-polygon-sdk-1.1.tar", last modified: Tue May  2 01:08:29 2023, max compression
```

## Comparing `async-polygon-sdk-1.tar` & `async-polygon-sdk-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 00:29:34.810123 async-polygon-sdk-1/
--rw-rw-rw-   0        0        0      323 2023-05-02 00:29:34.809124 async-polygon-sdk-1/PKG-INFO
--rw-rw-rw-   0        0        0     4028 2023-05-02 00:05:52.000000 async-polygon-sdk-1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 00:29:34.808122 async-polygon-sdk-1/async_polygon_sdk.egg-info/
--rw-rw-rw-   0        0        0      323 2023-05-02 00:29:34.000000 async-polygon-sdk-1/async_polygon_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-02 00:29:34.000000 async-polygon-sdk-1/async_polygon_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 00:29:34.000000 async-polygon-sdk-1/async_polygon_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      408 2023-05-02 00:29:34.000000 async-polygon-sdk-1/async_polygon_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 00:29:34.000000 async-polygon-sdk-1/async_polygon_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 00:29:34.810123 async-polygon-sdk-1/setup.cfg
--rw-rw-rw-   0        0        0      947 2023-05-02 00:26:42.000000 async-polygon-sdk-1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:08:29.550660 async-polygon-sdk-1.1/
+-rw-rw-rw-   0        0        0      325 2023-05-02 01:08:29.550660 async-polygon-sdk-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4028 2023-05-02 00:05:52.000000 async-polygon-sdk-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 01:08:29.549659 async-polygon-sdk-1.1/async_polygon_sdk.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-05-02 01:08:29.000000 async-polygon-sdk-1.1/async_polygon_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-02 01:08:29.000000 async-polygon-sdk-1.1/async_polygon_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 01:08:29.000000 async-polygon-sdk-1.1/async_polygon_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      422 2023-05-02 01:08:29.000000 async-polygon-sdk-1.1/async_polygon_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 01:08:29.000000 async-polygon-sdk-1.1/async_polygon_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 01:08:29.550660 async-polygon-sdk-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-05-02 01:08:16.000000 async-polygon-sdk-1.1/setup.py
```

### Comparing `async-polygon-sdk-1/README.md` & `async-polygon-sdk-1.1/README.md`

 * *Files identical despite different names*

### Comparing `async-polygon-sdk-1/setup.py` & `async-polygon-sdk-1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 name='async-polygon-sdk',
-version='1',
+version='1.1',
 author='chuckdustin12',
 author_email='chuckdustin12@gmail.com',
 description='This package is designed to work with the polygon.io service as an async toolkit for analyzing markets in real time.',
 packages=find_packages(),
 install_requires=[
 'numpy>=1.18',
 'pandas>=1.0',
@@ -20,14 +20,15 @@
 'frozenlist==1.3.3',
 'h11==0.14.0',
 'httpcore==0.17.0',
 'httpx==0.24.0',
 'idna==3.4',
 'multidict==6.0.4',
 'numpy==1.24.3',
+'pandas==2.0.1',
 'polygon==1.1.0',
 'polygon-api-client==1.8.5',
 'requests==2.29.0',
 'scipy==1.10.1',
 'sniffio==1.3.0',
 'urllib3==1.26.15',
 'websocket-client==1.5.1',
```

