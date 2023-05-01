# Comparing `tmp/neuronx-xlboost-0.1.tar.gz` & `tmp/neuronx-xlboost-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuronx-xlboost-0.1.tar", last modified: Mon May  1 23:42:41 2023, max compression
+gzip compressed data, was "neuronx-xlboost-1.0.tar", last modified: Mon May  1 18:52:34 2023, max compression
```

## Comparing `neuronx-xlboost-0.1.tar` & `neuronx-xlboost-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:42:41.209064 neuronx-xlboost-0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    25646 2020-08-19 00:03:01.000000 neuronx-xlboost-0.1/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      325 2023-05-01 23:42:41.209064 neuronx-xlboost-0.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2519 2023-01-10 16:58:42.000000 neuronx-xlboost-0.1/README
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:42:41.209064 neuronx-xlboost-0.1/neuronx-xlboost_pypi/
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:42:41.209064 neuronx-xlboost-0.1/neuronx-xlboost_pypi/neuronx-xlboost/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      119 2023-05-01 23:42:40.000000 neuronx-xlboost-0.1/neuronx-xlboost_pypi/neuronx-xlboost/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:42:41.209064 neuronx-xlboost-0.1/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      325 2023-05-01 23:42:41.000000 neuronx-xlboost-0.1/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      303 2023-05-01 23:42:41.000000 neuronx-xlboost-0.1/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 23:42:41.000000 neuronx-xlboost-0.1/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-01 23:42:41.000000 neuronx-xlboost-0.1/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 23:42:41.209064 neuronx-xlboost-0.1/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 18:52:34.078038 neuronx-xlboost-1.0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    25646 2020-08-19 00:03:01.000000 neuronx-xlboost-1.0/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      325 2023-05-01 18:52:34.078038 neuronx-xlboost-1.0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2519 2023-01-10 16:58:42.000000 neuronx-xlboost-1.0/README
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 18:52:34.078038 neuronx-xlboost-1.0/neuronx-xlboost_pypi/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 18:52:34.078038 neuronx-xlboost-1.0/neuronx-xlboost_pypi/neuronx-xlboost/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      119 2023-05-01 18:52:33.000000 neuronx-xlboost-1.0/neuronx-xlboost_pypi/neuronx-xlboost/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 18:52:34.078038 neuronx-xlboost-1.0/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      325 2023-05-01 18:52:33.000000 neuronx-xlboost-1.0/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      303 2023-05-01 18:52:34.000000 neuronx-xlboost-1.0/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 18:52:33.000000 neuronx-xlboost-1.0/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-05-01 18:52:33.000000 neuronx-xlboost-1.0/neuronx-xlboost_pypi/neuronx_xlboost.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 18:52:34.078038 neuronx-xlboost-1.0/setup.cfg
```

### Comparing `neuronx-xlboost-0.1/LICENSE` & `neuronx-xlboost-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuronx-xlboost-0.1/README` & `neuronx-xlboost-1.0/README`

 * *Files identical despite different names*

