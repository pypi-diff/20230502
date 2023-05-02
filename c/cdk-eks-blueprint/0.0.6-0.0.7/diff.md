# Comparing `tmp/cdk-eks-blueprint-0.0.6.tar.gz` & `tmp/cdk-eks-blueprint-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-eks-blueprint-0.0.6.tar", last modified: Tue May  2 01:28:24 2023, max compression
+gzip compressed data, was "cdk-eks-blueprint-0.0.7.tar", last modified: Tue May  2 01:41:41 2023, max compression
```

## Comparing `cdk-eks-blueprint-0.0.6.tar` & `cdk-eks-blueprint-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:28:24.735128 cdk-eks-blueprint-0.0.6/
--rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 01:28:24.735128 cdk-eks-blueprint-0.0.6/PKG-INFO
--rw-r--r--   0 yuriliang  (1000) users      (100)       14 2023-04-29 11:18:46.000000 cdk-eks-blueprint-0.0.6/README.md
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:28:24.735128 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-01 12:20:32.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/__init__.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:28:24.735128 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/addons/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-04-30 10:36:01.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/addons/__init__.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:28:24.735128 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-01 12:20:23.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/__init__.py
--rw-r--r--   0 yuriliang  (1000) users      (100)      625 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/_params_validation.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     5974 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/controller_plane.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     5599 2023-05-02 01:26:25.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/eks_cluster.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     3170 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/managed_node_group.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     2951 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/self_manage_node_group.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:28:24.735128 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint.egg-info/
--rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 01:28:24.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint.egg-info/PKG-INFO
--rw-r--r--   0 yuriliang  (1000) users      (100)      562 2023-05-02 01:28:24.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint.egg-info/SOURCES.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)        1 2023-05-02 01:28:24.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint.egg-info/dependency_links.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       93 2023-05-02 01:28:24.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint.egg-info/requires.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       18 2023-05-02 01:28:24.000000 cdk-eks-blueprint-0.0.6/cdk_eks_blueprint.egg-info/top_level.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       38 2023-05-02 01:28:24.735128 cdk-eks-blueprint-0.0.6/setup.cfg
--r--r--r--   0 yuriliang  (1000) users      (100)      504 2023-05-02 01:27:40.000000 cdk-eks-blueprint-0.0.6/setup.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/
+-rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/PKG-INFO
+-rw-r--r--   0 yuriliang  (1000) users      (100)       14 2023-04-29 11:18:46.000000 cdk-eks-blueprint-0.0.7/README.md
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.806037 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/
+-rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-02 01:38:40.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/__init__.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/addons/
+-rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-04-30 10:36:01.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/addons/__init__.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/
+-rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-02 01:38:52.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/__init__.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)      625 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/_params_validation.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     5933 2023-05-02 01:39:23.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/controller_plane.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     5633 2023-05-02 01:39:57.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/eks_cluster.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     3171 2023-05-02 01:40:03.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/managed_node_group.py
+-rw-r--r--   0 yuriliang  (1000) users      (100)     2952 2023-05-02 01:40:09.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/self_manage_node_group.py
+drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/
+-rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/PKG-INFO
+-rw-r--r--   0 yuriliang  (1000) users      (100)      562 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/SOURCES.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)        1 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/dependency_links.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)       93 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/requires.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)       18 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/top_level.txt
+-rw-r--r--   0 yuriliang  (1000) users      (100)       38 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/setup.cfg
+-r--r--r--   0 yuriliang  (1000) users      (100)      504 2023-05-02 01:41:37.000000 cdk-eks-blueprint-0.0.7/setup.py
```

### Comparing `cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/_params_validation.py` & `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/_params_validation.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/controller_plane.py` & `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/controller_plane.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Union, Dict, Optional, Any
-from semver import VersionInfo  # pyright: reportPrivateImportUsage=false
+from semver import VersionInfo
 from ipaddress import ip_network
 from dataclasses import dataclass, field
-from _params_validation import Validation
+from ._params_validation import Validation
 from aws_cdk import (
     Size,
     aws_eks as eks,
     aws_ec2 as ec2,
     aws_iam as iam,
     aws_lambda as _lambda,
     aws_kms as kms,
@@ -96,15 +96,15 @@
         if value.upper() not in ["EC2", "FARGATE"]:
             raise ValueError("core_dns_compute_type must be one of [EC2, FARGATE]")
         return getattr(eks.CoreDnsComputeType, value)
 
     def validate_alb_controller(
         self, value, **_
     ) -> Union[eks.AlbControllerOptions, None]:
-        if not isinstance(value, str) or not VersionInfo.isvalid(value):
+        if not isinstance(value, str) or not VersionInfo.is_valid(value):
             raise ValueError("alb_controller_version must be valid version string")
         versionNumber = f"V{value.replace('.', '_')}"
         try:
             return eks.AlbControllerOptions(
                 version=getattr(eks.AlbControllerVersion, versionNumber)
             )
         except Exception as e:
```

### Comparing `cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/eks_cluster.py` & `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/eks_cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pyright: reportUndefinedVariable=false, reportGeneralTypeIssues=false
 from typing import List
 from aws_cdk import aws_eks as eks
 from constructs import Construct
-from cluster import ControllerPlane
-from cluster import EKSManagedNodeGroup
-from cluster import SelfManagedNodeGroup
+from .controller_plane import ControllerPlane
+from .managed_node_group import EKSManagedNodeGroup
+from .self_manage_node_group import SelfManagedNodeGroup
 
 
 class EKSCluster(Construct):
     def __init__(
         self,
         scope: Construct,
         id: str,
         *,
         controller_plane: ControllerPlane,
-        eks_managed_node_groups: List[EKSManagedNodeGroup] = None,
-        self_managed_node_group: List[SelfManagedNodeGroup] = None,
+        eks_managed_node_groups: List[EKSManagedNodeGroup] = [],
+        self_managed_node_group: List[SelfManagedNodeGroup] = [],
         **kwargs,
     ):
         super().__init__(scope, id, **kwargs)
         cluster = eks.Cluster(
             self,
             f"{controller_plane.cluster_name}",
             cluster_name=controller_plane.cluster_name,
```

### Comparing `cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/managed_node_group.py` & `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/managed_node_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Dict, List, Any, Union
-from _params_validation import Validation
+from ._params_validation import Validation
 from dataclasses import dataclass, field
 from aws_cdk.aws_autoscaling import (
     BlockDevice,
     GroupMetrics,
     HealthCheck,
     Monitoring,
     Signals,
```

### Comparing `cdk-eks-blueprint-0.0.6/cdk_eks_blueprint/cluster/self_manage_node_group.py` & `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/self_manage_node_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union, List, Dict, Any
 from dataclasses import dataclass, field
-from _params_validation import Validation
+from ._params_validation import Validation
 from aws_cdk import aws_eks as eks, aws_iam as iam, aws_ec2 as ec2
 
 
 @dataclass
 class SelfManagedNodeGroup(Validation):
     nodegroup_name: str
     ami_type: Optional[str] = "AL2_X86_64"
```

### Comparing `cdk-eks-blueprint-0.0.6/cdk_eks_blueprint.egg-info/SOURCES.txt` & `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

