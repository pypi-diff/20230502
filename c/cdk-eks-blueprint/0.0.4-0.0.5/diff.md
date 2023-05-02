# Comparing `tmp/cdk-eks-blueprint-0.0.4.tar.gz` & `tmp/cdk-eks-blueprint-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-eks-blueprint-0.0.4.tar", last modified: Mon May  1 12:21:20 2023, max compression
+gzip compressed data, was "cdk-eks-blueprint-0.0.5.tar", last modified: Tue May  2 00:56:35 2023, max compression
```

## Comparing `cdk-eks-blueprint-0.0.4.tar` & `cdk-eks-blueprint-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-01 12:21:20.769876 cdk-eks-blueprint-0.0.4/
--rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-01 12:21:20.769876 cdk-eks-blueprint-0.0.4/PKG-INFO
--rw-r--r--   0 yuriliang  (1000) users      (100)       14 2023-04-29 11:18:46.000000 cdk-eks-blueprint-0.0.4/README.md
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-01 12:21:20.769876 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-01 12:20:32.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/__init__.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-01 12:21:20.769876 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/addons/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-04-30 10:36:01.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/addons/__init__.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-01 12:21:20.769876 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-01 12:20:23.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/__init__.py
--rw-r--r--   0 yuriliang  (1000) users      (100)      625 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/_params_validation.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     5974 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/controller_plane.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     5634 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/eks_cluster.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     3170 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/managed_node_group.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     2951 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/self_manage_node_group.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-01 12:21:20.769876 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint.egg-info/
--rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-01 12:21:20.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint.egg-info/PKG-INFO
--rw-r--r--   0 yuriliang  (1000) users      (100)      562 2023-05-01 12:21:20.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint.egg-info/SOURCES.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)        1 2023-05-01 12:21:20.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint.egg-info/dependency_links.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       93 2023-05-01 12:21:20.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint.egg-info/requires.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       18 2023-05-01 12:21:20.000000 cdk-eks-blueprint-0.0.4/cdk_eks_blueprint.egg-info/top_level.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       38 2023-05-01 12:21:20.769876 cdk-eks-blueprint-0.0.4/setup.cfg
--r--r--r--   0 yuriliang  (1000) users      (100)      504 2023-05-01 12:20:57.000000 cdk-eks-blueprint-0.0.4/setup.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 00:56:35.814981 cdk-eks-blueprint-0.0.5/
+-rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 00:56:35.814981 cdk-eks-blueprint-0.0.5/PKG-INFO
+-rw-r--r--   0 yuriliang  (1000) users      (100)       14 2023-04-29 11:18:46.000000 cdk-eks-blueprint-0.0.5/README.md
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 00:56:35.814981 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/
+-rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-01 12:20:32.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/__init__.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 00:56:35.814981 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/addons/
+-rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-04-30 10:36:01.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/addons/__init__.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 00:56:35.814981 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/
+-rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-01 12:20:23.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/__init__.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)      625 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/_params_validation.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     5974 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/controller_plane.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     5581 2023-05-02 00:55:41.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/eks_cluster.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     3170 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/managed_node_group.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     2951 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/self_manage_node_group.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 00:56:35.814981 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint.egg-info/
+-rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 00:56:35.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint.egg-info/PKG-INFO
+-rw-r--r--   0 yuriliang  (1000) users      (100)      562 2023-05-02 00:56:35.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint.egg-info/SOURCES.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)        1 2023-05-02 00:56:35.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint.egg-info/dependency_links.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)       93 2023-05-02 00:56:35.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint.egg-info/requires.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)       18 2023-05-02 00:56:35.000000 cdk-eks-blueprint-0.0.5/cdk_eks_blueprint.egg-info/top_level.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)       38 2023-05-02 00:56:35.814981 cdk-eks-blueprint-0.0.5/setup.cfg
+-r--r--r--   0 yuriliang  (1000) users      (100)      504 2023-05-02 00:56:24.000000 cdk-eks-blueprint-0.0.5/setup.py
```

### Comparing `cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/_params_validation.py` & `cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/_params_validation.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/controller_plane.py` & `cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/controller_plane.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/eks_cluster.py` & `cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/eks_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyright: reportUndefinedVariable=false, reportGeneralTypeIssues=false
 from typing import List
 from aws_cdk import aws_eks as eks
 from constructs import Construct
-from controller_plane import ControllerPlane
-from managed_node_group import EKSManagedNodeGroup
-from self_manage_node_group import SelfManagedNodeGroup
+from . import ControllerPlane
+from . import EKSManagedNodeGroup
+from . import SelfManagedNodeGroup
 
 
 class EKSCluster(Construct):
     def __init__(
         self,
         scope: Construct,
         id: str,
```

### Comparing `cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/managed_node_group.py` & `cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/managed_node_group.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.4/cdk_eks_blueprint/cluster/self_manage_node_group.py` & `cdk-eks-blueprint-0.0.5/cdk_eks_blueprint/cluster/self_manage_node_group.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.4/cdk_eks_blueprint.egg-info/SOURCES.txt` & `cdk-eks-blueprint-0.0.5/cdk_eks_blueprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

