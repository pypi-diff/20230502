# Comparing `tmp/neuron-xlboost-0.1.tar.gz` & `tmp/neuron-xlboost-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuron-xlboost-0.1.tar", last modified: Mon May  1 23:40:58 2023, max compression
+gzip compressed data, was "neuron-xlboost-1.0.tar", last modified: Mon May  1 23:32:03 2023, max compression
```

## Comparing `neuron-xlboost-0.1.tar` & `neuron-xlboost-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:40:58.977578 neuron-xlboost-0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    25646 2020-08-19 00:03:01.000000 neuron-xlboost-0.1/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      324 2023-05-01 23:40:58.977578 neuron-xlboost-0.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2519 2023-01-10 16:58:42.000000 neuron-xlboost-0.1/README
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:40:58.977578 neuron-xlboost-0.1/neuron-xlboost_pypi/
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:40:58.977578 neuron-xlboost-0.1/neuron-xlboost_pypi/neuron-xlboost/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      119 2023-05-01 23:40:58.000000 neuron-xlboost-0.1/neuron-xlboost_pypi/neuron-xlboost/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:40:58.977578 neuron-xlboost-0.1/neuron-xlboost_pypi/neuron_xlboost.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      324 2023-05-01 23:40:58.000000 neuron-xlboost-0.1/neuron-xlboost_pypi/neuron_xlboost.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      293 2023-05-01 23:40:58.000000 neuron-xlboost-0.1/neuron-xlboost_pypi/neuron_xlboost.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 23:40:58.000000 neuron-xlboost-0.1/neuron-xlboost_pypi/neuron_xlboost.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       15 2023-05-01 23:40:58.000000 neuron-xlboost-0.1/neuron-xlboost_pypi/neuron_xlboost.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 23:40:58.977578 neuron-xlboost-0.1/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:32:03.464322 neuron-xlboost-1.0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    25646 2020-08-19 00:03:01.000000 neuron-xlboost-1.0/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      324 2023-05-01 23:32:03.464322 neuron-xlboost-1.0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2519 2023-01-10 16:58:42.000000 neuron-xlboost-1.0/README
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:32:03.464322 neuron-xlboost-1.0/neuron-xlboost_pypi/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:32:03.464322 neuron-xlboost-1.0/neuron-xlboost_pypi/neuron-xlboost/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      119 2023-05-01 23:32:03.000000 neuron-xlboost-1.0/neuron-xlboost_pypi/neuron-xlboost/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-01 23:32:03.464322 neuron-xlboost-1.0/neuron-xlboost_pypi/neuron_xlboost.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      324 2023-05-01 23:32:03.000000 neuron-xlboost-1.0/neuron-xlboost_pypi/neuron_xlboost.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      293 2023-05-01 23:32:03.000000 neuron-xlboost-1.0/neuron-xlboost_pypi/neuron_xlboost.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-01 23:32:03.000000 neuron-xlboost-1.0/neuron-xlboost_pypi/neuron_xlboost.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       15 2023-05-01 23:32:03.000000 neuron-xlboost-1.0/neuron-xlboost_pypi/neuron_xlboost.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-01 23:32:03.464322 neuron-xlboost-1.0/setup.cfg
```

### Comparing `neuron-xlboost-0.1/LICENSE` & `neuron-xlboost-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuron-xlboost-0.1/README` & `neuron-xlboost-1.0/README`

 * *Files identical despite different names*

