# Comparing `tmp/mypy-boto3-ecs-1.26.7.tar.gz` & `tmp/mypy-boto3-ecs-1.26.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.26.7.tar", last modified: Thu Nov 10 20:32:39 2022, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
```

## Comparing `mypy-boto3-ecs-1.26.7.tar` & `mypy-boto3-ecs-1.26.78.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.505201 mypy-boto3-ecs-1.26.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    23619 2022-11-10 20:32:39.505201 mypy-boto3-ecs-1.26.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22200 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.505201 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    47894 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    47821 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14544 2022-11-10 20:32:22.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    14542 2022-11-10 20:32:22.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10402 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10391 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    79860 2022-11-10 20:32:24.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    79769 2022-11-10 20:32:23.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.505201 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23619 2022-11-10 20:32:39.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-10 20:32:39.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-10 20:32:39.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 20:32:39.000000 mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 20:32:39.505201 mypy-boto3-ecs-1.26.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-10 20:32:21.000000 mypy-boto3-ecs-1.26.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24442 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.320421 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-02-23 20:34:25.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-02-23 20:34:25.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85416 2023-02-23 20:34:27.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85315 2023-02-23 20:34:25.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24442 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/setup.py
```

### Comparing `mypy-boto3-ecs-1.26.7/LICENSE` & `mypy-boto3-ecs-1.26.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.7/PKG-INFO` & `mypy-boto3-ecs-1.26.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.26.7
-Summary: Type annotations for boto3.ECS 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.78
+Summary: Type annotations for boto3.ECS 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +284,15 @@
 from mypy_boto3_ecs import ECSClient
 from mypy_boto3_ecs.paginator import (
     ListAccountSettingsPaginator,
     ListAttributesPaginator,
     ListClustersPaginator,
     ListContainerInstancesPaginator,
     ListServicesPaginator,
+    ListServicesByNamespacePaginator,
     ListTaskDefinitionFamiliesPaginator,
     ListTaskDefinitionsPaginator,
     ListTasksPaginator,
 )
 
 client: ECSClient = Session().client("ecs")
 
@@ -301,14 +303,17 @@
 )
 list_attributes_paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_container_instances_paginator: ListContainerInstancesPaginator = client.get_paginator(
     "list_container_instances"
 )
 list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+list_services_by_namespace_paginator: ListServicesByNamespacePaginator = client.get_paginator(
+    "list_services_by_namespace"
+)
 list_task_definition_families_paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator(
     "list_task_definition_families"
 )
 list_task_definitions_paginator: ListTaskDefinitionsPaginator = client.get_paginator(
     "list_task_definitions"
 )
 list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
@@ -347,14 +352,15 @@
 
 `mypy_boto3_ecs.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ecs.literals import (
     AgentUpdateStatusType,
+    ApplicationProtocolType,
     AssignPublicIpType,
     CPUArchitectureType,
     CapacityProviderFieldType,
     CapacityProviderStatusType,
     CapacityProviderUpdateStatusType,
     ClusterFieldType,
     ClusterSettingNameType,
@@ -377,14 +383,15 @@
     InstanceHealthCheckTypeType,
     IpcModeType,
     LaunchTypeType,
     ListAccountSettingsPaginatorName,
     ListAttributesPaginatorName,
     ListClustersPaginatorName,
     ListContainerInstancesPaginatorName,
+    ListServicesByNamespacePaginatorName,
     ListServicesPaginatorName,
     ListTaskDefinitionFamiliesPaginatorName,
     ListTaskDefinitionsPaginatorName,
     ListTasksPaginatorName,
     LogDriverType,
     ManagedAgentNameType,
     ManagedScalingStatusType,
@@ -444,14 +451,16 @@
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
+    ClusterServiceConnectDefaultsRequestTypeDef,
+    ClusterServiceConnectDefaultsTypeDef,
     ClusterSettingTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
     FirelensConfigurationTypeDef,
     HealthCheckTypeDef,
     HostEntryTypeDef,
     MountPointTypeDef,
@@ -476,20 +485,23 @@
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteTaskDefinitionsRequestRequestTypeDef,
+    FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsTypeDef,
     DeploymentCircuitBreakerTypeDef,
+    ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
-    FailureTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
@@ -510,25 +522,27 @@
     KernelCapabilitiesTypeDef,
     TmpfsTypeDef,
     PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
     ListAttributesRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
+    ListServicesByNamespaceRequestRequestTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTasksRequestRequestTypeDef,
     ManagedAgentStateChangeTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
@@ -550,14 +564,15 @@
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
     DeleteAttributesResponseTypeDef,
     DiscoverPollEndpointResponseTypeDef,
     ListAttributesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     PutAttributesResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
@@ -580,41 +595,40 @@
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersTypeDef,
     ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAttributesRequestListAttributesPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     CreateTaskSetRequestRequestTypeDef,
-    DeploymentTypeDef,
     TaskSetTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    UpdateServiceRequestRequestTypeDef,
     ClusterConfigurationTypeDef,
     VolumeTypeDef,
     ContainerDefinitionTypeDef,
+    ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
-    ServiceTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
     TaskTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
@@ -622,31 +636,36 @@
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     RegisterTaskDefinitionRequestRequestTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    DescribeServicesResponseTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    DeploymentTypeDef,
+    UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
+    DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    ServiceTypeDef,
+    CreateServiceResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DescribeServicesResponseTypeDef,
+    UpdateServiceResponseTypeDef,
 )
 
 
 def get_structure() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-ecs-1.26.7/README.md` & `mypy-boto3-ecs-1.26.78/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -252,14 +252,15 @@
 from mypy_boto3_ecs import ECSClient
 from mypy_boto3_ecs.paginator import (
     ListAccountSettingsPaginator,
     ListAttributesPaginator,
     ListClustersPaginator,
     ListContainerInstancesPaginator,
     ListServicesPaginator,
+    ListServicesByNamespacePaginator,
     ListTaskDefinitionFamiliesPaginator,
     ListTaskDefinitionsPaginator,
     ListTasksPaginator,
 )
 
 client: ECSClient = Session().client("ecs")
 
@@ -270,14 +271,17 @@
 )
 list_attributes_paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_container_instances_paginator: ListContainerInstancesPaginator = client.get_paginator(
     "list_container_instances"
 )
 list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+list_services_by_namespace_paginator: ListServicesByNamespacePaginator = client.get_paginator(
+    "list_services_by_namespace"
+)
 list_task_definition_families_paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator(
     "list_task_definition_families"
 )
 list_task_definitions_paginator: ListTaskDefinitionsPaginator = client.get_paginator(
     "list_task_definitions"
 )
 list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
@@ -316,14 +320,15 @@
 
 `mypy_boto3_ecs.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ecs.literals import (
     AgentUpdateStatusType,
+    ApplicationProtocolType,
     AssignPublicIpType,
     CPUArchitectureType,
     CapacityProviderFieldType,
     CapacityProviderStatusType,
     CapacityProviderUpdateStatusType,
     ClusterFieldType,
     ClusterSettingNameType,
@@ -346,14 +351,15 @@
     InstanceHealthCheckTypeType,
     IpcModeType,
     LaunchTypeType,
     ListAccountSettingsPaginatorName,
     ListAttributesPaginatorName,
     ListClustersPaginatorName,
     ListContainerInstancesPaginatorName,
+    ListServicesByNamespacePaginatorName,
     ListServicesPaginatorName,
     ListTaskDefinitionFamiliesPaginatorName,
     ListTaskDefinitionsPaginatorName,
     ListTasksPaginatorName,
     LogDriverType,
     ManagedAgentNameType,
     ManagedScalingStatusType,
@@ -413,14 +419,16 @@
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
+    ClusterServiceConnectDefaultsRequestTypeDef,
+    ClusterServiceConnectDefaultsTypeDef,
     ClusterSettingTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
     FirelensConfigurationTypeDef,
     HealthCheckTypeDef,
     HostEntryTypeDef,
     MountPointTypeDef,
@@ -445,20 +453,23 @@
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteTaskDefinitionsRequestRequestTypeDef,
+    FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsTypeDef,
     DeploymentCircuitBreakerTypeDef,
+    ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
-    FailureTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
@@ -479,25 +490,27 @@
     KernelCapabilitiesTypeDef,
     TmpfsTypeDef,
     PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
     ListAttributesRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
+    ListServicesByNamespaceRequestRequestTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTasksRequestRequestTypeDef,
     ManagedAgentStateChangeTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
@@ -519,14 +532,15 @@
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
     DeleteAttributesResponseTypeDef,
     DiscoverPollEndpointResponseTypeDef,
     ListAttributesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     PutAttributesResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
@@ -549,41 +563,40 @@
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersTypeDef,
     ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAttributesRequestListAttributesPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     CreateTaskSetRequestRequestTypeDef,
-    DeploymentTypeDef,
     TaskSetTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    UpdateServiceRequestRequestTypeDef,
     ClusterConfigurationTypeDef,
     VolumeTypeDef,
     ContainerDefinitionTypeDef,
+    ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
-    ServiceTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
     TaskTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
@@ -591,31 +604,36 @@
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     RegisterTaskDefinitionRequestRequestTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    DescribeServicesResponseTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    DeploymentTypeDef,
+    UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
+    DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    ServiceTypeDef,
+    CreateServiceResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DescribeServicesResponseTypeDef,
+    UpdateServiceResponseTypeDef,
 )
 
 
 def get_structure() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     from mypy_boto3_ecs import (
         Client,
         ECSClient,
         ListAccountSettingsPaginator,
         ListAttributesPaginator,
         ListClustersPaginator,
         ListContainerInstancesPaginator,
+        ListServicesByNamespacePaginator,
         ListServicesPaginator,
         ListTaskDefinitionFamiliesPaginator,
         ListTaskDefinitionsPaginator,
         ListTasksPaginator,
         ServicesInactiveWaiter,
         ServicesStableWaiter,
         TasksRunningWaiter,
@@ -31,25 +32,27 @@
     tasks_stopped_waiter: TasksStoppedWaiter = client.get_waiter("tasks_stopped")
 
     list_account_settings_paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")
     list_attributes_paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_container_instances_paginator: ListContainerInstancesPaginator = client.get_paginator("list_container_instances")
     list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+    list_services_by_namespace_paginator: ListServicesByNamespacePaginator = client.get_paginator("list_services_by_namespace")
     list_task_definition_families_paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator("list_task_definition_families")
     list_task_definitions_paginator: ListTaskDefinitionsPaginator = client.get_paginator("list_task_definitions")
     list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
     ```
 """
 from .client import ECSClient
 from .paginator import (
     ListAccountSettingsPaginator,
     ListAttributesPaginator,
     ListClustersPaginator,
     ListContainerInstancesPaginator,
+    ListServicesByNamespacePaginator,
     ListServicesPaginator,
     ListTaskDefinitionFamiliesPaginator,
     ListTaskDefinitionsPaginator,
     ListTasksPaginator,
 )
 from .waiter import (
     ServicesInactiveWaiter,
@@ -64,14 +67,15 @@
 __all__ = (
     "Client",
     "ECSClient",
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
+    "ListServicesByNamespacePaginator",
     "ListServicesPaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
     "ServicesInactiveWaiter",
     "ServicesStableWaiter",
     "TasksRunningWaiter",
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     from mypy_boto3_ecs import (
         Client,
         ECSClient,
         ListAccountSettingsPaginator,
         ListAttributesPaginator,
         ListClustersPaginator,
         ListContainerInstancesPaginator,
+        ListServicesByNamespacePaginator,
         ListServicesPaginator,
         ListTaskDefinitionFamiliesPaginator,
         ListTaskDefinitionsPaginator,
         ListTasksPaginator,
         ServicesInactiveWaiter,
         ServicesStableWaiter,
         TasksRunningWaiter,
@@ -31,25 +32,27 @@
     tasks_stopped_waiter: TasksStoppedWaiter = client.get_waiter("tasks_stopped")
 
     list_account_settings_paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")
     list_attributes_paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_container_instances_paginator: ListContainerInstancesPaginator = client.get_paginator("list_container_instances")
     list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+    list_services_by_namespace_paginator: ListServicesByNamespacePaginator = client.get_paginator("list_services_by_namespace")
     list_task_definition_families_paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator("list_task_definition_families")
     list_task_definitions_paginator: ListTaskDefinitionsPaginator = client.get_paginator("list_task_definitions")
     list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
     ```
 """
 from .client import ECSClient
 from .paginator import (
     ListAccountSettingsPaginator,
     ListAttributesPaginator,
     ListClustersPaginator,
     ListContainerInstancesPaginator,
+    ListServicesByNamespacePaginator,
     ListServicesPaginator,
     ListTaskDefinitionFamiliesPaginator,
     ListTaskDefinitionsPaginator,
     ListTasksPaginator,
 )
 from .waiter import (
     ServicesInactiveWaiter,
@@ -63,14 +66,15 @@
 __all__ = (
     "Client",
     "ECSClient",
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
+    "ListServicesByNamespacePaginator",
     "ListServicesPaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
     "ServicesInactiveWaiter",
     "ServicesStableWaiter",
     "TasksRunningWaiter",
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.26.7\nVersion:         1.26.7\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.ECS 1.26.78\nVersion:         1.26.78\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.7")
+    print("1.26.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,38 +37,41 @@
     TaskDefinitionStatusType,
 )
 from .paginator import (
     ListAccountSettingsPaginator,
     ListAttributesPaginator,
     ListClustersPaginator,
     ListContainerInstancesPaginator,
+    ListServicesByNamespacePaginator,
     ListServicesPaginator,
     ListTaskDefinitionFamiliesPaginator,
     ListTaskDefinitionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
     AttachmentStateChangeTypeDef,
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
+    ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
     ContainerDefinitionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
+    DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DeploymentConfigurationTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
@@ -82,14 +85,15 @@
     ExecuteCommandResponseTypeDef,
     GetTaskProtectionResponseTypeDef,
     InferenceAcceleratorTypeDef,
     ListAccountSettingsResponseTypeDef,
     ListAttributesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
@@ -105,14 +109,15 @@
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
     ResourceTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
+    ServiceConnectConfigurationTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
@@ -163,14 +168,15 @@
     ClusterContainsContainerInstancesException: Type[BotocoreClientError]
     ClusterContainsServicesException: Type[BotocoreClientError]
     ClusterContainsTasksException: Type[BotocoreClientError]
     ClusterNotFoundException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MissingVersionException: Type[BotocoreClientError]
+    NamespaceNotFoundException: Type[BotocoreClientError]
     NoUpdateAvailableException: Type[BotocoreClientError]
     PlatformTaskDefinitionIncompatibilityException: Type[BotocoreClientError]
     PlatformUnknownException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServerException: Type[BotocoreClientError]
     ServiceNotActiveException: Type[BotocoreClientError]
@@ -233,15 +239,16 @@
         self,
         *,
         clusterName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
         capacityProviders: Sequence[str] = ...,
-        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...
+        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new Amazon ECS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_cluster)
         """
@@ -266,15 +273,16 @@
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
-        enableExecuteCommand: bool = ...
+        enableExecuteCommand: bool = ...,
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
@@ -304,16 +312,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_task_set)
         """
 
     def delete_account_setting(
         self, *, name: SettingNameType, principalArn: str = ...
     ) -> DeleteAccountSettingResponseTypeDef:
         """
-        Disables an account setting for a specified IAM user, IAM role, or the root user
-        for an account.
+        Disables an account setting for a specified user, role, or the root user for an
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_account_setting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_account_setting)
         """
 
     def delete_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
@@ -349,14 +357,24 @@
         """
         Deletes a specified service within a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_service)
         """
 
+    def delete_task_definitions(
+        self, *, taskDefinitions: Sequence[str]
+    ) -> DeleteTaskDefinitionsResponseTypeDef:
+        """
+        Deletes one or more task definitions.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_task_definitions)
+        """
+
     def delete_task_set(
         self, *, cluster: str, service: str, taskSet: str, force: bool = ...
     ) -> DeleteTaskSetResponseTypeDef:
         """
         Deletes a specified task set within a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_set)
@@ -594,14 +612,25 @@
         """
         Returns a list of services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services)
         """
 
+    def list_services_by_namespace(
+        self, *, namespace: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListServicesByNamespaceResponseTypeDef:
+        """
+        This operation lists all of the services that are associated with a Cloud Map
+        namespace.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services_by_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services_by_namespace)
+        """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         List the tags for an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_tags_for_resource)
         """
@@ -667,16 +696,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting)
         """
 
     def put_account_setting_default(
         self, *, name: SettingNameType, value: str
     ) -> PutAccountSettingDefaultResponseTypeDef:
         """
-        Modifies an account setting for all IAM users on an account for whom no
-        individual account setting has been specified.
+        Modifies an account setting for all users on an account for whom no individual
+        account setting has been specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_account_setting_default)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting_default)
         """
 
     def put_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
@@ -891,15 +920,16 @@
         """
 
     def update_cluster(
         self,
         *,
         cluster: str,
         settings: Sequence[ClusterSettingTypeDef] = ...,
-        configuration: ClusterConfigurationTypeDef = ...
+        configuration: ClusterConfigurationTypeDef = ...,
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
     ) -> UpdateClusterResponseTypeDef:
         """
         Updates the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_cluster)
         """
@@ -953,15 +983,16 @@
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
-        serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...
+        serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
@@ -1038,14 +1069,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_services_by_namespace"]
+    ) -> ListServicesByNamespacePaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_task_definition_families"]
     ) -> ListTaskDefinitionFamiliesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,38 +37,41 @@
     TaskDefinitionStatusType,
 )
 from .paginator import (
     ListAccountSettingsPaginator,
     ListAttributesPaginator,
     ListClustersPaginator,
     ListContainerInstancesPaginator,
+    ListServicesByNamespacePaginator,
     ListServicesPaginator,
     ListTaskDefinitionFamiliesPaginator,
     ListTaskDefinitionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
     AttachmentStateChangeTypeDef,
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
+    ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
     ContainerDefinitionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
+    DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DeploymentConfigurationTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
@@ -82,14 +85,15 @@
     ExecuteCommandResponseTypeDef,
     GetTaskProtectionResponseTypeDef,
     InferenceAcceleratorTypeDef,
     ListAccountSettingsResponseTypeDef,
     ListAttributesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
@@ -105,14 +109,15 @@
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
     ResourceTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
+    ServiceConnectConfigurationTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
@@ -160,14 +165,15 @@
     ClusterContainsContainerInstancesException: Type[BotocoreClientError]
     ClusterContainsServicesException: Type[BotocoreClientError]
     ClusterContainsTasksException: Type[BotocoreClientError]
     ClusterNotFoundException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MissingVersionException: Type[BotocoreClientError]
+    NamespaceNotFoundException: Type[BotocoreClientError]
     NoUpdateAvailableException: Type[BotocoreClientError]
     PlatformTaskDefinitionIncompatibilityException: Type[BotocoreClientError]
     PlatformUnknownException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServerException: Type[BotocoreClientError]
     ServiceNotActiveException: Type[BotocoreClientError]
@@ -225,15 +231,16 @@
         self,
         *,
         clusterName: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         settings: Sequence[ClusterSettingTypeDef] = ...,
         configuration: ClusterConfigurationTypeDef = ...,
         capacityProviders: Sequence[str] = ...,
-        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...
+        defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a new Amazon ECS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_cluster)
         """
@@ -257,15 +264,16 @@
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
-        enableExecuteCommand: bool = ...
+        enableExecuteCommand: bool = ...,
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
@@ -293,16 +301,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_task_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_task_set)
         """
     def delete_account_setting(
         self, *, name: SettingNameType, principalArn: str = ...
     ) -> DeleteAccountSettingResponseTypeDef:
         """
-        Disables an account setting for a specified IAM user, IAM role, or the root user
-        for an account.
+        Disables an account setting for a specified user, role, or the root user for an
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_account_setting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_account_setting)
         """
     def delete_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
     ) -> DeleteAttributesResponseTypeDef:
@@ -333,14 +341,23 @@
     ) -> DeleteServiceResponseTypeDef:
         """
         Deletes a specified service within a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_service)
         """
+    def delete_task_definitions(
+        self, *, taskDefinitions: Sequence[str]
+    ) -> DeleteTaskDefinitionsResponseTypeDef:
+        """
+        Deletes one or more task definitions.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#delete_task_definitions)
+        """
     def delete_task_set(
         self, *, cluster: str, service: str, taskSet: str, force: bool = ...
     ) -> DeleteTaskSetResponseTypeDef:
         """
         Deletes a specified task set within a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.delete_task_set)
@@ -559,14 +576,24 @@
     ) -> ListServicesResponseTypeDef:
         """
         Returns a list of services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services)
         """
+    def list_services_by_namespace(
+        self, *, namespace: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListServicesByNamespaceResponseTypeDef:
+        """
+        This operation lists all of the services that are associated with a Cloud Map
+        namespace.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_services_by_namespace)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_services_by_namespace)
+        """
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         List the tags for an Amazon ECS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#list_tags_for_resource)
         """
@@ -627,16 +654,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_account_setting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting)
         """
     def put_account_setting_default(
         self, *, name: SettingNameType, value: str
     ) -> PutAccountSettingDefaultResponseTypeDef:
         """
-        Modifies an account setting for all IAM users on an account for whom no
-        individual account setting has been specified.
+        Modifies an account setting for all users on an account for whom no individual
+        account setting has been specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.put_account_setting_default)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#put_account_setting_default)
         """
     def put_attributes(
         self, *, attributes: Sequence[AttributeTypeDef], cluster: str = ...
     ) -> PutAttributesResponseTypeDef:
@@ -837,15 +864,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_capacity_provider)
         """
     def update_cluster(
         self,
         *,
         cluster: str,
         settings: Sequence[ClusterSettingTypeDef] = ...,
-        configuration: ClusterConfigurationTypeDef = ...
+        configuration: ClusterConfigurationTypeDef = ...,
+        serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...
     ) -> UpdateClusterResponseTypeDef:
         """
         Updates the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_cluster)
         """
@@ -895,15 +923,16 @@
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
-        serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...
+        serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
@@ -971,14 +1000,22 @@
     def get_paginator(self, operation_name: Literal["list_services"]) -> ListServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_services_by_namespace"]
+    ) -> ListServicesByNamespacePaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_task_definition_families"]
     ) -> ListTaskDefinitionFamiliesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AgentUpdateStatusType",
+    "ApplicationProtocolType",
     "AssignPublicIpType",
     "CPUArchitectureType",
     "CapacityProviderFieldType",
     "CapacityProviderStatusType",
     "CapacityProviderUpdateStatusType",
     "ClusterFieldType",
     "ClusterSettingNameType",
@@ -47,14 +47,15 @@
     "InstanceHealthCheckTypeType",
     "IpcModeType",
     "LaunchTypeType",
     "ListAccountSettingsPaginatorName",
     "ListAttributesPaginatorName",
     "ListClustersPaginatorName",
     "ListContainerInstancesPaginatorName",
+    "ListServicesByNamespacePaginatorName",
     "ListServicesPaginatorName",
     "ListTaskDefinitionFamiliesPaginatorName",
     "ListTaskDefinitionsPaginatorName",
     "ListTasksPaginatorName",
     "LogDriverType",
     "ManagedAgentNameType",
     "ManagedScalingStatusType",
@@ -93,16 +94,16 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgentUpdateStatusType = Literal["FAILED", "PENDING", "STAGED", "STAGING", "UPDATED", "UPDATING"]
+ApplicationProtocolType = Literal["grpc", "http", "http2"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CPUArchitectureType = Literal["ARM64", "X86_64"]
 CapacityProviderFieldType = Literal["TAGS"]
 CapacityProviderStatusType = Literal["ACTIVE", "INACTIVE"]
 CapacityProviderUpdateStatusType = Literal[
     "DELETE_COMPLETE",
     "DELETE_FAILED",
@@ -134,14 +135,15 @@
 InstanceHealthCheckTypeType = Literal["CONTAINER_RUNTIME"]
 IpcModeType = Literal["host", "none", "task"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListAccountSettingsPaginatorName = Literal["list_account_settings"]
 ListAttributesPaginatorName = Literal["list_attributes"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListContainerInstancesPaginatorName = Literal["list_container_instances"]
+ListServicesByNamespacePaginatorName = Literal["list_services_by_namespace"]
 ListServicesPaginatorName = Literal["list_services"]
 ListTaskDefinitionFamiliesPaginatorName = Literal["list_task_definition_families"]
 ListTaskDefinitionsPaginatorName = Literal["list_task_definitions"]
 ListTasksPaginatorName = Literal["list_tasks"]
 LogDriverType = Literal[
     "awsfirelens", "awslogs", "fluentd", "gelf", "journald", "json-file", "splunk", "syslog"
 ]
@@ -181,18 +183,25 @@
 ]
 SortOrderType = Literal["ASC", "DESC"]
 StabilityStatusType = Literal["STABILIZING", "STEADY_STATE"]
 TargetTypeType = Literal["container-instance"]
 TaskDefinitionFamilyStatusType = Literal["ACTIVE", "ALL", "INACTIVE"]
 TaskDefinitionFieldType = Literal["TAGS"]
 TaskDefinitionPlacementConstraintTypeType = Literal["memberOf"]
-TaskDefinitionStatusType = Literal["ACTIVE", "INACTIVE"]
+TaskDefinitionStatusType = Literal["ACTIVE", "DELETE_IN_PROGRESS", "INACTIVE"]
 TaskFieldType = Literal["TAGS"]
 TaskSetFieldType = Literal["TAGS"]
-TaskStopCodeType = Literal["EssentialContainerExited", "TaskFailedToStart", "UserInitiated"]
+TaskStopCodeType = Literal[
+    "EssentialContainerExited",
+    "ServiceSchedulerInitiated",
+    "SpotInterruption",
+    "TaskFailedToStart",
+    "TerminationNotice",
+    "UserInitiated",
+]
 TasksRunningWaiterName = Literal["tasks_running"]
 TasksStoppedWaiterName = Literal["tasks_stopped"]
 TransportProtocolType = Literal["tcp", "udp"]
 UlimitNameType = Literal[
     "core",
     "cpu",
     "data",
@@ -230,14 +239,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -247,27 +257,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -296,14 +310,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -351,14 +366,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -369,30 +385,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -424,28 +443,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -473,52 +496,58 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -546,34 +575,38 @@
 ]
 PaginatorName = Literal[
     "list_account_settings",
     "list_attributes",
     "list_clusters",
     "list_container_instances",
     "list_services",
+    "list_services_by_namespace",
     "list_task_definition_families",
     "list_task_definitions",
     "list_tasks",
 ]
 WaiterName = Literal["services_inactive", "services_stable", "tasks_running", "tasks_stopped"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AgentUpdateStatusType",
+    "ApplicationProtocolType",
     "AssignPublicIpType",
     "CPUArchitectureType",
     "CapacityProviderFieldType",
     "CapacityProviderStatusType",
     "CapacityProviderUpdateStatusType",
     "ClusterFieldType",
     "ClusterSettingNameType",
@@ -46,14 +48,15 @@
     "InstanceHealthCheckTypeType",
     "IpcModeType",
     "LaunchTypeType",
     "ListAccountSettingsPaginatorName",
     "ListAttributesPaginatorName",
     "ListClustersPaginatorName",
     "ListContainerInstancesPaginatorName",
+    "ListServicesByNamespacePaginatorName",
     "ListServicesPaginatorName",
     "ListTaskDefinitionFamiliesPaginatorName",
     "ListTaskDefinitionsPaginatorName",
     "ListTasksPaginatorName",
     "LogDriverType",
     "ManagedAgentNameType",
     "ManagedScalingStatusType",
@@ -92,15 +95,17 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AgentUpdateStatusType = Literal["FAILED", "PENDING", "STAGED", "STAGING", "UPDATED", "UPDATING"]
+ApplicationProtocolType = Literal["grpc", "http", "http2"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CPUArchitectureType = Literal["ARM64", "X86_64"]
 CapacityProviderFieldType = Literal["TAGS"]
 CapacityProviderStatusType = Literal["ACTIVE", "INACTIVE"]
 CapacityProviderUpdateStatusType = Literal[
     "DELETE_COMPLETE",
     "DELETE_FAILED",
@@ -132,14 +137,15 @@
 InstanceHealthCheckTypeType = Literal["CONTAINER_RUNTIME"]
 IpcModeType = Literal["host", "none", "task"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListAccountSettingsPaginatorName = Literal["list_account_settings"]
 ListAttributesPaginatorName = Literal["list_attributes"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListContainerInstancesPaginatorName = Literal["list_container_instances"]
+ListServicesByNamespacePaginatorName = Literal["list_services_by_namespace"]
 ListServicesPaginatorName = Literal["list_services"]
 ListTaskDefinitionFamiliesPaginatorName = Literal["list_task_definition_families"]
 ListTaskDefinitionsPaginatorName = Literal["list_task_definitions"]
 ListTasksPaginatorName = Literal["list_tasks"]
 LogDriverType = Literal[
     "awsfirelens", "awslogs", "fluentd", "gelf", "journald", "json-file", "splunk", "syslog"
 ]
@@ -179,18 +185,25 @@
 ]
 SortOrderType = Literal["ASC", "DESC"]
 StabilityStatusType = Literal["STABILIZING", "STEADY_STATE"]
 TargetTypeType = Literal["container-instance"]
 TaskDefinitionFamilyStatusType = Literal["ACTIVE", "ALL", "INACTIVE"]
 TaskDefinitionFieldType = Literal["TAGS"]
 TaskDefinitionPlacementConstraintTypeType = Literal["memberOf"]
-TaskDefinitionStatusType = Literal["ACTIVE", "INACTIVE"]
+TaskDefinitionStatusType = Literal["ACTIVE", "DELETE_IN_PROGRESS", "INACTIVE"]
 TaskFieldType = Literal["TAGS"]
 TaskSetFieldType = Literal["TAGS"]
-TaskStopCodeType = Literal["EssentialContainerExited", "TaskFailedToStart", "UserInitiated"]
+TaskStopCodeType = Literal[
+    "EssentialContainerExited",
+    "ServiceSchedulerInitiated",
+    "SpotInterruption",
+    "TaskFailedToStart",
+    "TerminationNotice",
+    "UserInitiated",
+]
 TasksRunningWaiterName = Literal["tasks_running"]
 TasksStoppedWaiterName = Literal["tasks_stopped"]
 TransportProtocolType = Literal["tcp", "udp"]
 UlimitNameType = Literal[
     "core",
     "cpu",
     "data",
@@ -228,14 +241,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -245,27 +259,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -294,14 +312,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -349,14 +368,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -367,30 +387,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -422,28 +445,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -471,52 +498,58 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -544,34 +577,38 @@
 ]
 PaginatorName = Literal[
     "list_account_settings",
     "list_attributes",
     "list_clusters",
     "list_container_instances",
     "list_services",
+    "list_services_by_namespace",
     "list_task_definition_families",
     "list_task_definitions",
     "list_tasks",
 ]
 WaiterName = Literal["services_inactive", "services_stable", "tasks_running", "tasks_stopped"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,29 @@
     from mypy_boto3_ecs.client import ECSClient
     from mypy_boto3_ecs.paginator import (
         ListAccountSettingsPaginator,
         ListAttributesPaginator,
         ListClustersPaginator,
         ListContainerInstancesPaginator,
         ListServicesPaginator,
+        ListServicesByNamespacePaginator,
         ListTaskDefinitionFamiliesPaginator,
         ListTaskDefinitionsPaginator,
         ListTasksPaginator,
     )
 
     session = Session()
     client: ECSClient = session.client("ecs")
 
     list_account_settings_paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")
     list_attributes_paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_container_instances_paginator: ListContainerInstancesPaginator = client.get_paginator("list_container_instances")
     list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+    list_services_by_namespace_paginator: ListServicesByNamespacePaginator = client.get_paginator("list_services_by_namespace")
     list_task_definition_families_paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator("list_task_definition_families")
     list_task_definitions_paginator: ListTaskDefinitionsPaginator = client.get_paginator("list_task_definitions")
     list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
     ```
 """
 import sys
 from typing import Generic, Iterator, TypeVar
@@ -49,49 +51,47 @@
     TaskDefinitionStatusType,
 )
 from .type_defs import (
     ListAccountSettingsResponseTypeDef,
     ListAttributesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
     "ListServicesPaginator",
+    "ListServicesByNamespacePaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAccountSettingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
     """
 
     def paginate(
@@ -104,15 +104,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
         """
 
-
 class ListAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
     """
 
     def paginate(
@@ -125,30 +124,28 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
         """
 
-
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
         """
 
-
 class ListContainerInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
     """
 
     def paginate(
@@ -160,15 +157,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
         """
 
-
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
     """
 
     def paginate(
@@ -180,14 +176,27 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
         """
 
+class ListServicesByNamespacePaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
+    """
+
+    def paginate(
+        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListServicesByNamespaceResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
+        """
 
 class ListTaskDefinitionFamiliesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
     """
 
@@ -199,15 +208,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
-
 class ListTaskDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
     """
 
     def paginate(
@@ -219,15 +227,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
-
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,29 @@
     from mypy_boto3_ecs.client import ECSClient
     from mypy_boto3_ecs.paginator import (
         ListAccountSettingsPaginator,
         ListAttributesPaginator,
         ListClustersPaginator,
         ListContainerInstancesPaginator,
         ListServicesPaginator,
+        ListServicesByNamespacePaginator,
         ListTaskDefinitionFamiliesPaginator,
         ListTaskDefinitionsPaginator,
         ListTasksPaginator,
     )
 
     session = Session()
     client: ECSClient = session.client("ecs")
 
     list_account_settings_paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")
     list_attributes_paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_container_instances_paginator: ListContainerInstancesPaginator = client.get_paginator("list_container_instances")
     list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+    list_services_by_namespace_paginator: ListServicesByNamespacePaginator = client.get_paginator("list_services_by_namespace")
     list_task_definition_families_paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator("list_task_definition_families")
     list_task_definitions_paginator: ListTaskDefinitionsPaginator = client.get_paginator("list_task_definitions")
     list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
     ```
 """
 import sys
 from typing import Generic, Iterator, TypeVar
@@ -49,45 +51,51 @@
     TaskDefinitionStatusType,
 )
 from .type_defs import (
     ListAccountSettingsResponseTypeDef,
     ListAttributesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListAccountSettingsPaginator",
     "ListAttributesPaginator",
     "ListClustersPaginator",
     "ListContainerInstancesPaginator",
     "ListServicesPaginator",
+    "ListServicesByNamespacePaginator",
     "ListTaskDefinitionFamiliesPaginator",
     "ListTaskDefinitionsPaginator",
     "ListTasksPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAccountSettingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
     """
 
     def paginate(
@@ -100,14 +108,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
         """
 
+
 class ListAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
     """
 
     def paginate(
@@ -120,28 +129,30 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
         """
 
+
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
         """
 
+
 class ListContainerInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
     """
 
     def paginate(
@@ -153,14 +164,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
         """
 
+
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
     """
 
     def paginate(
@@ -172,14 +184,30 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
         """
 
+
+class ListServicesByNamespacePaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
+    """
+
+    def paginate(
+        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListServicesByNamespaceResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
+        """
+
+
 class ListTaskDefinitionFamiliesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
     """
 
     def paginate(
@@ -190,14 +218,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
+
 class ListTaskDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
     """
 
     def paginate(
@@ -209,14 +238,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
+
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     from mypy_boto3_ecs.type_defs import AttachmentStateChangeTypeDef
 
     data: AttachmentStateChangeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AgentUpdateStatusType,
+    ApplicationProtocolType,
     AssignPublicIpType,
     CapacityProviderStatusType,
     CapacityProviderUpdateStatusType,
     ClusterFieldType,
     CompatibilityType,
     ConnectivityType,
     ContainerConditionType,
@@ -66,23 +67,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
+    "ClusterServiceConnectDefaultsRequestTypeDef",
+    "ClusterServiceConnectDefaultsTypeDef",
     "ClusterSettingTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
     "FirelensConfigurationTypeDef",
     "HealthCheckTypeDef",
     "HostEntryTypeDef",
     "MountPointTypeDef",
@@ -107,20 +109,23 @@
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
+    "DeleteTaskDefinitionsRequestRequestTypeDef",
+    "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
+    "DeploymentAlarmsTypeDef",
     "DeploymentCircuitBreakerTypeDef",
+    "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
-    "FailureTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
@@ -141,25 +146,27 @@
     "KernelCapabilitiesTypeDef",
     "TmpfsTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
     "ListAttributesRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
+    "ListServicesByNamespaceRequestRequestTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
     "ListTasksRequestRequestTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
+    "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
@@ -181,14 +188,15 @@
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
     "DeleteAttributesResponseTypeDef",
     "DiscoverPollEndpointResponseTypeDef",
     "ListAttributesResponseTypeDef",
     "ListClustersResponseTypeDef",
     "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTaskDefinitionFamiliesResponseTypeDef",
     "ListTaskDefinitionsResponseTypeDef",
     "ListTasksResponseTypeDef",
     "PutAttributesResponseTypeDef",
     "SubmitAttachmentStateChangesResponseTypeDef",
@@ -211,41 +219,40 @@
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
     "LinuxParametersTypeDef",
     "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
+    "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
-    "DeploymentTypeDef",
     "TaskSetTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
-    "CreateServiceRequestRequestTypeDef",
-    "UpdateServiceRequestRequestTypeDef",
     "ClusterConfigurationTypeDef",
     "VolumeTypeDef",
     "ContainerDefinitionTypeDef",
+    "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
-    "ServiceTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
     "TaskTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
@@ -253,31 +260,36 @@
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "RegisterTaskDefinitionRequestRequestTypeDef",
     "TaskDefinitionTypeDef",
-    "CreateServiceResponseTypeDef",
-    "DeleteServiceResponseTypeDef",
-    "DescribeServicesResponseTypeDef",
-    "UpdateServiceResponseTypeDef",
+    "CreateServiceRequestRequestTypeDef",
+    "DeploymentTypeDef",
+    "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
+    "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
+    "ServiceTypeDef",
+    "CreateServiceResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
+    "DescribeServicesResponseTypeDef",
+    "UpdateServiceResponseTypeDef",
 )
 
 AttachmentStateChangeTypeDef = TypedDict(
     "AttachmentStateChangeTypeDef",
     {
         "attachmentArn": str,
         "status": str,
@@ -305,19 +317,17 @@
         "value": str,
         "targetType": Literal["container-instance"],
         "targetId": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
@@ -337,21 +347,19 @@
     {
         "securityGroups": Sequence[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
-
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -359,30 +367,43 @@
     {
         "weight": int,
         "base": int,
     },
     total=False,
 )
 
-
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+ClusterServiceConnectDefaultsRequestTypeDef = TypedDict(
+    "ClusterServiceConnectDefaultsRequestTypeDef",
+    {
+        "namespace": str,
+    },
+)
+
+ClusterServiceConnectDefaultsTypeDef = TypedDict(
+    "ClusterServiceConnectDefaultsTypeDef",
+    {
+        "namespace": str,
+    },
+    total=False,
+)
+
 ClusterSettingTypeDef = TypedDict(
     "ClusterSettingTypeDef",
     {
         "name": Literal["containerInsights"],
         "value": str,
     },
     total=False,
@@ -414,21 +435,19 @@
     "_OptionalFirelensConfigurationTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
-
 class FirelensConfigurationTypeDef(
     _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
-
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "command": List[str],
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
@@ -438,19 +457,17 @@
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
-
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
-
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
@@ -467,14 +484,17 @@
 
 PortMappingTypeDef = TypedDict(
     "PortMappingTypeDef",
     {
         "containerPort": int,
         "hostPort": int,
         "protocol": TransportProtocolType,
+        "name": str,
+        "appProtocol": ApplicationProtocolType,
+        "containerPortRange": str,
     },
     total=False,
 )
 
 RepositoryCredentialsTypeDef = TypedDict(
     "RepositoryCredentialsTypeDef",
     {
@@ -562,14 +582,16 @@
 NetworkBindingTypeDef = TypedDict(
     "NetworkBindingTypeDef",
     {
         "bindIP": str,
         "containerPort": int,
         "hostPort": int,
         "protocol": TransportProtocolType,
+        "containerPortRange": str,
+        "hostPortRange": str,
     },
     total=False,
 )
 
 ManagedAgentTypeDef = TypedDict(
     "ManagedAgentTypeDef",
     {
@@ -668,22 +690,20 @@
     "_OptionalDeleteAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
-
 class DeleteAccountSettingRequestRequestTypeDef(
     _RequiredDeleteAccountSettingRequestRequestTypeDef,
     _OptionalDeleteAccountSettingRequestRequestTypeDef,
 ):
     pass
 
-
 SettingTypeDef = TypedDict(
     "SettingTypeDef",
     {
         "name": SettingNameType,
         "value": str,
         "principalArn": str,
     },
@@ -715,20 +735,35 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteServiceRequestRequestTypeDef(
     _RequiredDeleteServiceRequestRequestTypeDef, _OptionalDeleteServiceRequestRequestTypeDef
 ):
     pass
 
+DeleteTaskDefinitionsRequestRequestTypeDef = TypedDict(
+    "DeleteTaskDefinitionsRequestRequestTypeDef",
+    {
+        "taskDefinitions": Sequence[str],
+    },
+)
+
+FailureTypeDef = TypedDict(
+    "FailureTypeDef",
+    {
+        "arn": str,
+        "reason": str,
+        "detail": str,
+    },
+    total=False,
+)
 
 _RequiredDeleteTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
@@ -738,29 +773,45 @@
     "_OptionalDeleteTaskSetRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
+DeploymentAlarmsTypeDef = TypedDict(
+    "DeploymentAlarmsTypeDef",
+    {
+        "alarmNames": Sequence[str],
+        "enable": bool,
+        "rollback": bool,
+    },
+)
 
 DeploymentCircuitBreakerTypeDef = TypedDict(
     "DeploymentCircuitBreakerTypeDef",
     {
         "enable": bool,
         "rollback": bool,
     },
 )
 
+ServiceConnectServiceResourceTypeDef = TypedDict(
+    "ServiceConnectServiceResourceTypeDef",
+    {
+        "discoveryName": str,
+        "discoveryArn": str,
+    },
+    total=False,
+)
+
 _RequiredDeregisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterContainerInstanceRequestRequestTypeDef",
     {
         "containerInstance": str,
     },
 )
 _OptionalDeregisterContainerInstanceRequestRequestTypeDef = TypedDict(
@@ -768,22 +819,20 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeregisterContainerInstanceRequestRequestTypeDef(
     _RequiredDeregisterContainerInstanceRequestRequestTypeDef,
     _OptionalDeregisterContainerInstanceRequestRequestTypeDef,
 ):
     pass
 
-
 DeregisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 
@@ -794,24 +843,14 @@
         "include": Sequence[Literal["TAGS"]],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-FailureTypeDef = TypedDict(
-    "FailureTypeDef",
-    {
-        "arn": str,
-        "reason": str,
-        "detail": str,
-    },
-    total=False,
-)
-
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "clusters": Sequence[str],
         "include": Sequence[ClusterFieldType],
     },
     total=False,
@@ -828,22 +867,20 @@
     {
         "cluster": str,
         "include": Sequence[ContainerInstanceFieldType],
     },
     total=False,
 )
 
-
 class DescribeContainerInstancesRequestRequestTypeDef(
     _RequiredDescribeContainerInstancesRequestRequestTypeDef,
     _OptionalDescribeContainerInstancesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeServicesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestRequestTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestRequestTypeDef = TypedDict(
@@ -851,21 +888,19 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeServicesRequestRequestTypeDef(
     _RequiredDescribeServicesRequestRequestTypeDef, _OptionalDescribeServicesRequestRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -881,22 +916,20 @@
     "_OptionalDescribeTaskDefinitionRequestRequestTypeDef",
     {
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTaskDefinitionRequestRequestTypeDef(
     _RequiredDescribeTaskDefinitionRequestRequestTypeDef,
     _OptionalDescribeTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTaskSetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTaskSetsRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
     },
 )
@@ -905,21 +938,19 @@
     {
         "taskSets": Sequence[str],
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTaskSetsRequestRequestTypeDef(
     _RequiredDescribeTaskSetsRequestRequestTypeDef, _OptionalDescribeTaskSetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestRequestTypeDef = TypedDict(
@@ -927,21 +958,19 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
@@ -949,19 +978,17 @@
     {
         "containerPath": str,
         "permissions": List[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
-
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
-
 DiscoverPollEndpointRequestRequestTypeDef = TypedDict(
     "DiscoverPollEndpointRequestRequestTypeDef",
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
@@ -1020,21 +1047,19 @@
     {
         "cluster": str,
         "container": str,
     },
     total=False,
 )
 
-
 class ExecuteCommandRequestRequestTypeDef(
     _RequiredExecuteCommandRequestRequestTypeDef, _OptionalExecuteCommandRequestRequestTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
@@ -1059,21 +1084,19 @@
     "_OptionalGetTaskProtectionRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
     total=False,
 )
 
-
 class GetTaskProtectionRequestRequestTypeDef(
     _RequiredGetTaskProtectionRequestRequestTypeDef, _OptionalGetTaskProtectionRequestRequestTypeDef
 ):
     pass
 
-
 ProtectedTaskTypeDef = TypedDict(
     "ProtectedTaskTypeDef",
     {
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
@@ -1125,19 +1148,17 @@
     "_OptionalTmpfsTypeDef",
     {
         "mountOptions": List[str],
     },
     total=False,
 )
 
-
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1171,21 +1192,19 @@
         "attributeValue": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1199,14 +1218,35 @@
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
+_RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestRequestTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListServicesByNamespaceRequestRequestTypeDef(
+    _RequiredListServicesByNamespaceRequestRequestTypeDef,
+    _OptionalListServicesByNamespaceRequestRequestTypeDef,
+):
+    pass
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
@@ -1273,21 +1313,19 @@
     "_OptionalManagedAgentStateChangeTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
 
-
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
-
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1311,21 +1349,19 @@
     "_OptionalPutAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
-
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
-
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -1336,14 +1372,33 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
+_RequiredServiceConnectClientAliasTypeDef = TypedDict(
+    "_RequiredServiceConnectClientAliasTypeDef",
+    {
+        "port": int,
+    },
+)
+_OptionalServiceConnectClientAliasTypeDef = TypedDict(
+    "_OptionalServiceConnectClientAliasTypeDef",
+    {
+        "dnsName": str,
+    },
+    total=False,
+)
+
+class ServiceConnectClientAliasTypeDef(
+    _RequiredServiceConnectClientAliasTypeDef, _OptionalServiceConnectClientAliasTypeDef
+):
+    pass
+
 ServiceEventTypeDef = TypedDict(
     "ServiceEventTypeDef",
     {
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
@@ -1361,21 +1416,19 @@
     {
         "cluster": str,
         "reason": str,
     },
     total=False,
 )
 
-
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1390,22 +1443,20 @@
     "_OptionalUpdateContainerAgentRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class UpdateContainerAgentRequestRequestTypeDef(
     _RequiredUpdateContainerAgentRequestRequestTypeDef,
     _OptionalUpdateContainerAgentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateContainerInstancesStateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "status": ContainerInstanceStatusType,
     },
 )
@@ -1413,22 +1464,20 @@
     "_OptionalUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class UpdateContainerInstancesStateRequestRequestTypeDef(
     _RequiredUpdateContainerInstancesStateRequestRequestTypeDef,
     _OptionalUpdateContainerInstancesStateRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateServicePrimaryTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "primaryTaskSet": str,
     },
@@ -1446,44 +1495,40 @@
     "_OptionalUpdateTaskProtectionRequestRequestTypeDef",
     {
         "expiresInMinutes": int,
     },
     total=False,
 )
 
-
 class UpdateTaskProtectionRequestRequestTypeDef(
     _RequiredUpdateTaskProtectionRequestRequestTypeDef,
     _OptionalUpdateTaskProtectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "attachments": Sequence[AttachmentStateChangeTypeDef],
     },
 )
 _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_OptionalSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class SubmitAttachmentStateChangesRequestRequestTypeDef(
     _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef,
     _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef,
 ):
     pass
 
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
@@ -1502,63 +1547,57 @@
     {
         "type": Literal["APPMESH"],
         "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
-
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1566,21 +1605,19 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
-
 class AutoScalingGroupProviderTypeDef(
     _RequiredAutoScalingGroupProviderTypeDef, _OptionalAutoScalingGroupProviderTypeDef
 ):
     pass
 
-
 AutoScalingGroupProviderUpdateTypeDef = TypedDict(
     "AutoScalingGroupProviderUpdateTypeDef",
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
@@ -1639,25 +1676,23 @@
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
     "_OptionalLogConfigurationTypeDef",
     {
-        "options": Dict[str, str],
-        "secretOptions": List[SecretTypeDef],
+        "options": Mapping[str, str],
+        "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
-
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
-
 ContainerInstanceHealthStatusTypeDef = TypedDict(
     "ContainerInstanceHealthStatusTypeDef",
     {
         "overallStatus": InstanceHealthCheckStateType,
         "details": List[InstanceHealthCheckResultTypeDef],
     },
     total=False,
@@ -1725,14 +1760,15 @@
 )
 
 DiscoverPollEndpointResponseTypeDef = TypedDict(
     "DiscoverPollEndpointResponseTypeDef",
     {
         "endpoint": str,
         "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributesResponseTypeDef = TypedDict(
     "ListAttributesResponseTypeDef",
     {
@@ -1756,14 +1792,23 @@
     {
         "containerInstanceArns": List[str],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "serviceArns": List[str],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1881,14 +1926,15 @@
 
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
+        "alarms": DeploymentAlarmsTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesInactiveWaitTypeDef",
     {
@@ -1901,22 +1947,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeServicesRequestServicesInactiveWaitTypeDef(
     _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef,
     _OptionalDescribeServicesRequestServicesInactiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesStableWaitTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
@@ -1925,22 +1969,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeServicesRequestServicesStableWaitTypeDef(
     _RequiredDescribeServicesRequestServicesStableWaitTypeDef,
     _OptionalDescribeServicesRequestServicesStableWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksRunningWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
@@ -1949,22 +1991,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTasksRequestTasksRunningWaitTypeDef(
     _RequiredDescribeTasksRequestTasksRunningWaitTypeDef,
     _OptionalDescribeTasksRequestTasksRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksStoppedWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
@@ -1973,22 +2013,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
-
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -1998,21 +2036,19 @@
         "transitEncryption": EFSTransitEncryptionType,
         "transitEncryptionPort": int,
         "authorizationConfig": EFSAuthorizationConfigTypeDef,
     },
     total=False,
 )
 
-
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
-
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2098,22 +2134,20 @@
         "attributeName": str,
         "attributeValue": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAttributesRequestListAttributesPaginateTypeDef(
     _RequiredListAttributesRequestListAttributesPaginateTypeDef,
     _OptionalListAttributesRequestListAttributesPaginateTypeDef,
 ):
     pass
 
-
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2125,14 +2159,34 @@
         "filter": str,
         "status": ContainerInstanceStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "cluster": str,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2188,14 +2242,35 @@
         "attributes": Sequence[AttributeTypeDef],
         "platformDevices": Sequence[PlatformDeviceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredServiceConnectServiceTypeDef = TypedDict(
+    "_RequiredServiceConnectServiceTypeDef",
+    {
+        "portName": str,
+    },
+)
+_OptionalServiceConnectServiceTypeDef = TypedDict(
+    "_OptionalServiceConnectServiceTypeDef",
+    {
+        "discoveryName": str,
+        "clientAliases": Sequence[ServiceConnectClientAliasTypeDef],
+        "ingressPortOverride": int,
+    },
+    total=False,
+)
+
+class ServiceConnectServiceTypeDef(
+    _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
+):
+    pass
+
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2217,22 +2292,20 @@
     "_OptionalCreateCapacityProviderRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCapacityProviderRequestRequestTypeDef(
     _RequiredCreateCapacityProviderRequestRequestTypeDef,
     _OptionalCreateCapacityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateCapacityProviderRequestRequestTypeDef = TypedDict(
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
@@ -2258,44 +2331,19 @@
         "scale": ScaleTypeDef,
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
-
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-    },
-    total=False,
-)
-
 TaskSetTypeDef = TypedDict(
     "TaskSetTypeDef",
     {
         "id": str,
         "taskSetArn": str,
         "serviceArn": str,
         "clusterArn": str,
@@ -2375,91 +2423,14 @@
         "pullStartedAt": Union[datetime, str],
         "pullStoppedAt": Union[datetime, str],
         "executionStoppedAt": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "taskDefinition": str,
-        "loadBalancers": Sequence[LoadBalancerTypeDef],
-        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
-        "desiredCount": int,
-        "clientToken": str,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "role": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
-        "placementConstraints": Sequence[PlacementConstraintTypeDef],
-        "placementStrategy": Sequence[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "healthCheckGracePeriodSeconds": int,
-        "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "enableECSManagedTags": bool,
-        "propagateTags": PropagateTagsType,
-        "enableExecuteCommand": bool,
-    },
-    total=False,
-)
-
-
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
-    {
-        "service": str,
-    },
-)
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "desiredCount": int,
-        "taskDefinition": str,
-        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "placementConstraints": Sequence[PlacementConstraintTypeDef],
-        "placementStrategy": Sequence[PlacementStrategyTypeDef],
-        "platformVersion": str,
-        "forceNewDeployment": bool,
-        "healthCheckGracePeriodSeconds": int,
-        "enableExecuteCommand": bool,
-        "enableECSManagedTags": bool,
-        "loadBalancers": Sequence[LoadBalancerTypeDef],
-        "propagateTags": PropagateTagsType,
-        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
-
-
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
@@ -2518,14 +2489,35 @@
         "systemControls": List[SystemControlTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredServiceConnectConfigurationTypeDef = TypedDict(
+    "_RequiredServiceConnectConfigurationTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalServiceConnectConfigurationTypeDef = TypedDict(
+    "_OptionalServiceConnectConfigurationTypeDef",
+    {
+        "namespace": str,
+        "services": Sequence[ServiceConnectServiceTypeDef],
+        "logConfiguration": LogConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class ServiceConnectConfigurationTypeDef(
+    _RequiredServiceConnectConfigurationTypeDef, _OptionalServiceConnectConfigurationTypeDef
+):
+    pass
+
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2577,52 +2569,14 @@
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServiceTypeDef = TypedDict(
-    "ServiceTypeDef",
-    {
-        "serviceArn": str,
-        "serviceName": str,
-        "clusterArn": str,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "status": str,
-        "desiredCount": int,
-        "runningCount": int,
-        "pendingCount": int,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
-        "taskSets": List[TaskSetTypeDef],
-        "deployments": List[DeploymentTypeDef],
-        "roleArn": str,
-        "events": List[ServiceEventTypeDef],
-        "createdAt": datetime,
-        "placementConstraints": List[PlacementConstraintTypeDef],
-        "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "healthCheckGracePeriodSeconds": int,
-        "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerTypeDef,
-        "tags": List[TagTypeDef],
-        "createdBy": str,
-        "enableECSManagedTags": bool,
-        "propagateTags": PropagateTagsType,
-        "enableExecuteCommand": bool,
-    },
-    total=False,
-)
-
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2660,21 +2614,19 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class RunTaskRequestRequestTypeDef(
     _RequiredRunTaskRequestRequestTypeDef, _OptionalRunTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "taskDefinition": str,
     },
 )
@@ -2691,21 +2643,19 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
-
 TaskTypeDef = TypedDict(
     "TaskTypeDef",
     {
         "attachments": List[AttachmentTypeDef],
         "attributes": List[AttributeTypeDef],
         "availabilityZone": str,
         "capacityProviderName": str,
@@ -2801,27 +2751,29 @@
         "statistics": List[KeyValuePairTypeDef],
         "tags": List[TagTypeDef],
         "settings": List[ClusterSettingTypeDef],
         "capacityProviders": List[str],
         "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "attachments": List[AttachmentTypeDef],
         "attachmentsStatus": str,
+        "serviceConnectDefaults": ClusterServiceConnectDefaultsTypeDef,
     },
     total=False,
 )
 
 CreateClusterRequestRequestTypeDef = TypedDict(
     "CreateClusterRequestRequestTypeDef",
     {
         "clusterName": str,
         "tags": Sequence[TagTypeDef],
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
@@ -2829,25 +2781,24 @@
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateClusterRequestRequestTypeDef",
     {
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
+        "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
-
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "family": str,
         "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
     },
 )
@@ -2869,22 +2820,20 @@
         "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
         "ephemeralStorage": EphemeralStorageTypeDef,
         "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
-
 class RegisterTaskDefinitionRequestRequestTypeDef(
     _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
     _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
         "containerDefinitions": List[ContainerDefinitionTypeDef],
         "family": str,
         "taskRoleArn": str,
@@ -2908,46 +2857,113 @@
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-CreateServiceResponseTypeDef = TypedDict(
-    "CreateServiceResponseTypeDef",
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
     {
-        "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serviceName": str,
     },
 )
-
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
     {
-        "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": str,
+        "taskDefinition": str,
+        "loadBalancers": Sequence[LoadBalancerTypeDef],
+        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
+        "desiredCount": int,
+        "clientToken": str,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "role": str,
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "placementConstraints": Sequence[PlacementConstraintTypeDef],
+        "placementStrategy": Sequence[PlacementStrategyTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "healthCheckGracePeriodSeconds": int,
+        "schedulingStrategy": SchedulingStrategyType,
+        "deploymentController": DeploymentControllerTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "enableECSManagedTags": bool,
+        "propagateTags": PropagateTagsType,
+        "enableExecuteCommand": bool,
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
+    total=False,
 )
 
-DescribeServicesResponseTypeDef = TypedDict(
-    "DescribeServicesResponseTypeDef",
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
+    pass
+
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
     {
-        "services": List[ServiceTypeDef],
-        "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
     },
+    total=False,
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
     {
-        "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "service": str,
     },
 )
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
+    {
+        "cluster": str,
+        "desiredCount": int,
+        "taskDefinition": str,
+        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "placementConstraints": Sequence[PlacementConstraintTypeDef],
+        "placementStrategy": Sequence[PlacementStrategyTypeDef],
+        "platformVersion": str,
+        "forceNewDeployment": bool,
+        "healthCheckGracePeriodSeconds": int,
+        "enableExecuteCommand": bool,
+        "enableECSManagedTags": bool,
+        "loadBalancers": Sequence[LoadBalancerTypeDef],
+        "propagateTags": PropagateTagsType,
+        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
 
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3025,14 +3041,23 @@
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteTaskDefinitionsResponseTypeDef = TypedDict(
+    "DeleteTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitions": List[TaskDefinitionTypeDef],
+        "failures": List[FailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3050,7 +3075,78 @@
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
+    {
+        "serviceArn": str,
+        "serviceName": str,
+        "clusterArn": str,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "status": str,
+        "desiredCount": int,
+        "runningCount": int,
+        "pendingCount": int,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "taskDefinition": str,
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "taskSets": List[TaskSetTypeDef],
+        "deployments": List[DeploymentTypeDef],
+        "roleArn": str,
+        "events": List[ServiceEventTypeDef],
+        "createdAt": datetime,
+        "placementConstraints": List[PlacementConstraintTypeDef],
+        "placementStrategy": List[PlacementStrategyTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "healthCheckGracePeriodSeconds": int,
+        "schedulingStrategy": SchedulingStrategyType,
+        "deploymentController": DeploymentControllerTypeDef,
+        "tags": List[TagTypeDef],
+        "createdBy": str,
+        "enableECSManagedTags": bool,
+        "propagateTags": PropagateTagsType,
+        "enableExecuteCommand": bool,
+    },
+    total=False,
+)
+
+CreateServiceResponseTypeDef = TypedDict(
+    "CreateServiceResponseTypeDef",
+    {
+        "service": ServiceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "service": ServiceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeServicesResponseTypeDef = TypedDict(
+    "DescribeServicesResponseTypeDef",
+    {
+        "services": List[ServiceTypeDef],
+        "failures": List[FailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "service": ServiceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     from mypy_boto3_ecs.type_defs import AttachmentStateChangeTypeDef
 
     data: AttachmentStateChangeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AgentUpdateStatusType,
+    ApplicationProtocolType,
     AssignPublicIpType,
     CapacityProviderStatusType,
     CapacityProviderUpdateStatusType,
     ClusterFieldType,
     CompatibilityType,
     ConnectivityType,
     ContainerConditionType,
@@ -66,22 +67,25 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
+    "ClusterServiceConnectDefaultsRequestTypeDef",
+    "ClusterServiceConnectDefaultsTypeDef",
     "ClusterSettingTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
     "FirelensConfigurationTypeDef",
     "HealthCheckTypeDef",
     "HostEntryTypeDef",
     "MountPointTypeDef",
@@ -106,20 +110,23 @@
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
+    "DeleteTaskDefinitionsRequestRequestTypeDef",
+    "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
+    "DeploymentAlarmsTypeDef",
     "DeploymentCircuitBreakerTypeDef",
+    "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
-    "FailureTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
@@ -140,25 +147,27 @@
     "KernelCapabilitiesTypeDef",
     "TmpfsTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
     "ListAttributesRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
+    "ListServicesByNamespaceRequestRequestTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
     "ListTasksRequestRequestTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
+    "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
@@ -180,14 +189,15 @@
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
     "DeleteAttributesResponseTypeDef",
     "DiscoverPollEndpointResponseTypeDef",
     "ListAttributesResponseTypeDef",
     "ListClustersResponseTypeDef",
     "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTaskDefinitionFamiliesResponseTypeDef",
     "ListTaskDefinitionsResponseTypeDef",
     "ListTasksResponseTypeDef",
     "PutAttributesResponseTypeDef",
     "SubmitAttachmentStateChangesResponseTypeDef",
@@ -210,41 +220,40 @@
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
     "LinuxParametersTypeDef",
     "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
+    "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
-    "DeploymentTypeDef",
     "TaskSetTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
-    "CreateServiceRequestRequestTypeDef",
-    "UpdateServiceRequestRequestTypeDef",
     "ClusterConfigurationTypeDef",
     "VolumeTypeDef",
     "ContainerDefinitionTypeDef",
+    "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
-    "ServiceTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
     "TaskTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
@@ -252,31 +261,36 @@
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "RegisterTaskDefinitionRequestRequestTypeDef",
     "TaskDefinitionTypeDef",
-    "CreateServiceResponseTypeDef",
-    "DeleteServiceResponseTypeDef",
-    "DescribeServicesResponseTypeDef",
-    "UpdateServiceResponseTypeDef",
+    "CreateServiceRequestRequestTypeDef",
+    "DeploymentTypeDef",
+    "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
+    "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
+    "ServiceTypeDef",
+    "CreateServiceResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
+    "DescribeServicesResponseTypeDef",
+    "UpdateServiceResponseTypeDef",
 )
 
 AttachmentStateChangeTypeDef = TypedDict(
     "AttachmentStateChangeTypeDef",
     {
         "attachmentArn": str,
         "status": str,
@@ -304,17 +318,19 @@
         "value": str,
         "targetType": Literal["container-instance"],
         "targetId": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
@@ -334,19 +350,21 @@
     {
         "securityGroups": Sequence[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
+
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -354,28 +372,45 @@
     {
         "weight": int,
         "base": int,
     },
     total=False,
 )
 
+
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+ClusterServiceConnectDefaultsRequestTypeDef = TypedDict(
+    "ClusterServiceConnectDefaultsRequestTypeDef",
+    {
+        "namespace": str,
+    },
+)
+
+ClusterServiceConnectDefaultsTypeDef = TypedDict(
+    "ClusterServiceConnectDefaultsTypeDef",
+    {
+        "namespace": str,
+    },
+    total=False,
+)
+
 ClusterSettingTypeDef = TypedDict(
     "ClusterSettingTypeDef",
     {
         "name": Literal["containerInsights"],
         "value": str,
     },
     total=False,
@@ -407,19 +442,21 @@
     "_OptionalFirelensConfigurationTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
+
 class FirelensConfigurationTypeDef(
     _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
+
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "command": List[str],
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
@@ -429,17 +466,19 @@
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
+
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
+
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
@@ -456,14 +495,17 @@
 
 PortMappingTypeDef = TypedDict(
     "PortMappingTypeDef",
     {
         "containerPort": int,
         "hostPort": int,
         "protocol": TransportProtocolType,
+        "name": str,
+        "appProtocol": ApplicationProtocolType,
+        "containerPortRange": str,
     },
     total=False,
 )
 
 RepositoryCredentialsTypeDef = TypedDict(
     "RepositoryCredentialsTypeDef",
     {
@@ -551,14 +593,16 @@
 NetworkBindingTypeDef = TypedDict(
     "NetworkBindingTypeDef",
     {
         "bindIP": str,
         "containerPort": int,
         "hostPort": int,
         "protocol": TransportProtocolType,
+        "containerPortRange": str,
+        "hostPortRange": str,
     },
     total=False,
 )
 
 ManagedAgentTypeDef = TypedDict(
     "ManagedAgentTypeDef",
     {
@@ -657,20 +701,22 @@
     "_OptionalDeleteAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
+
 class DeleteAccountSettingRequestRequestTypeDef(
     _RequiredDeleteAccountSettingRequestRequestTypeDef,
     _OptionalDeleteAccountSettingRequestRequestTypeDef,
 ):
     pass
 
+
 SettingTypeDef = TypedDict(
     "SettingTypeDef",
     {
         "name": SettingNameType,
         "value": str,
         "principalArn": str,
     },
@@ -702,19 +748,38 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteServiceRequestRequestTypeDef(
     _RequiredDeleteServiceRequestRequestTypeDef, _OptionalDeleteServiceRequestRequestTypeDef
 ):
     pass
 
+
+DeleteTaskDefinitionsRequestRequestTypeDef = TypedDict(
+    "DeleteTaskDefinitionsRequestRequestTypeDef",
+    {
+        "taskDefinitions": Sequence[str],
+    },
+)
+
+FailureTypeDef = TypedDict(
+    "FailureTypeDef",
+    {
+        "arn": str,
+        "reason": str,
+        "detail": str,
+    },
+    total=False,
+)
+
 _RequiredDeleteTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
     },
@@ -723,27 +788,47 @@
     "_OptionalDeleteTaskSetRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
+
+DeploymentAlarmsTypeDef = TypedDict(
+    "DeploymentAlarmsTypeDef",
+    {
+        "alarmNames": Sequence[str],
+        "enable": bool,
+        "rollback": bool,
+    },
+)
+
 DeploymentCircuitBreakerTypeDef = TypedDict(
     "DeploymentCircuitBreakerTypeDef",
     {
         "enable": bool,
         "rollback": bool,
     },
 )
 
+ServiceConnectServiceResourceTypeDef = TypedDict(
+    "ServiceConnectServiceResourceTypeDef",
+    {
+        "discoveryName": str,
+        "discoveryArn": str,
+    },
+    total=False,
+)
+
 _RequiredDeregisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterContainerInstanceRequestRequestTypeDef",
     {
         "containerInstance": str,
     },
 )
 _OptionalDeregisterContainerInstanceRequestRequestTypeDef = TypedDict(
@@ -751,20 +836,22 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeregisterContainerInstanceRequestRequestTypeDef(
     _RequiredDeregisterContainerInstanceRequestRequestTypeDef,
     _OptionalDeregisterContainerInstanceRequestRequestTypeDef,
 ):
     pass
 
+
 DeregisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 
@@ -775,24 +862,14 @@
         "include": Sequence[Literal["TAGS"]],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-FailureTypeDef = TypedDict(
-    "FailureTypeDef",
-    {
-        "arn": str,
-        "reason": str,
-        "detail": str,
-    },
-    total=False,
-)
-
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "clusters": Sequence[str],
         "include": Sequence[ClusterFieldType],
     },
     total=False,
@@ -809,20 +886,22 @@
     {
         "cluster": str,
         "include": Sequence[ContainerInstanceFieldType],
     },
     total=False,
 )
 
+
 class DescribeContainerInstancesRequestRequestTypeDef(
     _RequiredDescribeContainerInstancesRequestRequestTypeDef,
     _OptionalDescribeContainerInstancesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeServicesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestRequestTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestRequestTypeDef = TypedDict(
@@ -830,19 +909,21 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeServicesRequestRequestTypeDef(
     _RequiredDescribeServicesRequestRequestTypeDef, _OptionalDescribeServicesRequestRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -858,20 +939,22 @@
     "_OptionalDescribeTaskDefinitionRequestRequestTypeDef",
     {
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTaskDefinitionRequestRequestTypeDef(
     _RequiredDescribeTaskDefinitionRequestRequestTypeDef,
     _OptionalDescribeTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTaskSetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTaskSetsRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
     },
 )
@@ -880,19 +963,21 @@
     {
         "taskSets": Sequence[str],
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTaskSetsRequestRequestTypeDef(
     _RequiredDescribeTaskSetsRequestRequestTypeDef, _OptionalDescribeTaskSetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestRequestTypeDef = TypedDict(
@@ -900,19 +985,21 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
@@ -920,17 +1007,19 @@
     {
         "containerPath": str,
         "permissions": List[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
+
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
+
 DiscoverPollEndpointRequestRequestTypeDef = TypedDict(
     "DiscoverPollEndpointRequestRequestTypeDef",
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
@@ -989,19 +1078,21 @@
     {
         "cluster": str,
         "container": str,
     },
     total=False,
 )
 
+
 class ExecuteCommandRequestRequestTypeDef(
     _RequiredExecuteCommandRequestRequestTypeDef, _OptionalExecuteCommandRequestRequestTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
@@ -1026,19 +1117,21 @@
     "_OptionalGetTaskProtectionRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
     total=False,
 )
 
+
 class GetTaskProtectionRequestRequestTypeDef(
     _RequiredGetTaskProtectionRequestRequestTypeDef, _OptionalGetTaskProtectionRequestRequestTypeDef
 ):
     pass
 
+
 ProtectedTaskTypeDef = TypedDict(
     "ProtectedTaskTypeDef",
     {
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
@@ -1090,17 +1183,19 @@
     "_OptionalTmpfsTypeDef",
     {
         "mountOptions": List[str],
     },
     total=False,
 )
 
+
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1134,19 +1229,21 @@
         "attributeValue": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1160,14 +1257,37 @@
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
+_RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestRequestTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListServicesByNamespaceRequestRequestTypeDef(
+    _RequiredListServicesByNamespaceRequestRequestTypeDef,
+    _OptionalListServicesByNamespaceRequestRequestTypeDef,
+):
+    pass
+
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
@@ -1234,19 +1354,21 @@
     "_OptionalManagedAgentStateChangeTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
 
+
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
+
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1270,19 +1392,21 @@
     "_OptionalPutAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
+
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
+
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -1293,14 +1417,35 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
+_RequiredServiceConnectClientAliasTypeDef = TypedDict(
+    "_RequiredServiceConnectClientAliasTypeDef",
+    {
+        "port": int,
+    },
+)
+_OptionalServiceConnectClientAliasTypeDef = TypedDict(
+    "_OptionalServiceConnectClientAliasTypeDef",
+    {
+        "dnsName": str,
+    },
+    total=False,
+)
+
+
+class ServiceConnectClientAliasTypeDef(
+    _RequiredServiceConnectClientAliasTypeDef, _OptionalServiceConnectClientAliasTypeDef
+):
+    pass
+
+
 ServiceEventTypeDef = TypedDict(
     "ServiceEventTypeDef",
     {
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
@@ -1318,19 +1463,21 @@
     {
         "cluster": str,
         "reason": str,
     },
     total=False,
 )
 
+
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1345,20 +1492,22 @@
     "_OptionalUpdateContainerAgentRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class UpdateContainerAgentRequestRequestTypeDef(
     _RequiredUpdateContainerAgentRequestRequestTypeDef,
     _OptionalUpdateContainerAgentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateContainerInstancesStateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "status": ContainerInstanceStatusType,
     },
 )
@@ -1366,20 +1515,22 @@
     "_OptionalUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class UpdateContainerInstancesStateRequestRequestTypeDef(
     _RequiredUpdateContainerInstancesStateRequestRequestTypeDef,
     _OptionalUpdateContainerInstancesStateRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateServicePrimaryTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "primaryTaskSet": str,
     },
@@ -1397,40 +1548,44 @@
     "_OptionalUpdateTaskProtectionRequestRequestTypeDef",
     {
         "expiresInMinutes": int,
     },
     total=False,
 )
 
+
 class UpdateTaskProtectionRequestRequestTypeDef(
     _RequiredUpdateTaskProtectionRequestRequestTypeDef,
     _OptionalUpdateTaskProtectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "attachments": Sequence[AttachmentStateChangeTypeDef],
     },
 )
 _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_OptionalSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class SubmitAttachmentStateChangesRequestRequestTypeDef(
     _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef,
     _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef,
 ):
     pass
 
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
@@ -1449,57 +1604,63 @@
     {
         "type": Literal["APPMESH"],
         "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
+
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
+
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1507,19 +1668,21 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
+
 class AutoScalingGroupProviderTypeDef(
     _RequiredAutoScalingGroupProviderTypeDef, _OptionalAutoScalingGroupProviderTypeDef
 ):
     pass
 
+
 AutoScalingGroupProviderUpdateTypeDef = TypedDict(
     "AutoScalingGroupProviderUpdateTypeDef",
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
@@ -1578,23 +1741,25 @@
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
     "_OptionalLogConfigurationTypeDef",
     {
-        "options": Dict[str, str],
-        "secretOptions": List[SecretTypeDef],
+        "options": Mapping[str, str],
+        "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
+
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
+
 ContainerInstanceHealthStatusTypeDef = TypedDict(
     "ContainerInstanceHealthStatusTypeDef",
     {
         "overallStatus": InstanceHealthCheckStateType,
         "details": List[InstanceHealthCheckResultTypeDef],
     },
     total=False,
@@ -1662,14 +1827,15 @@
 )
 
 DiscoverPollEndpointResponseTypeDef = TypedDict(
     "DiscoverPollEndpointResponseTypeDef",
     {
         "endpoint": str,
         "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributesResponseTypeDef = TypedDict(
     "ListAttributesResponseTypeDef",
     {
@@ -1693,14 +1859,23 @@
     {
         "containerInstanceArns": List[str],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "serviceArns": List[str],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1818,14 +1993,15 @@
 
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
+        "alarms": DeploymentAlarmsTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesInactiveWaitTypeDef",
     {
@@ -1838,20 +2014,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeServicesRequestServicesInactiveWaitTypeDef(
     _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef,
     _OptionalDescribeServicesRequestServicesInactiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesStableWaitTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
@@ -1860,20 +2038,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeServicesRequestServicesStableWaitTypeDef(
     _RequiredDescribeServicesRequestServicesStableWaitTypeDef,
     _OptionalDescribeServicesRequestServicesStableWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksRunningWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
@@ -1882,20 +2062,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTasksRequestTasksRunningWaitTypeDef(
     _RequiredDescribeTasksRequestTasksRunningWaitTypeDef,
     _OptionalDescribeTasksRequestTasksRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksStoppedWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
@@ -1904,20 +2086,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
+
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -1927,19 +2111,21 @@
         "transitEncryption": EFSTransitEncryptionType,
         "transitEncryptionPort": int,
         "authorizationConfig": EFSAuthorizationConfigTypeDef,
     },
     total=False,
 )
 
+
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
+
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2025,20 +2211,22 @@
         "attributeName": str,
         "attributeValue": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAttributesRequestListAttributesPaginateTypeDef(
     _RequiredListAttributesRequestListAttributesPaginateTypeDef,
     _OptionalListAttributesRequestListAttributesPaginateTypeDef,
 ):
     pass
 
+
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2050,14 +2238,36 @@
         "filter": str,
         "status": ContainerInstanceStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
+
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "cluster": str,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2113,14 +2323,37 @@
         "attributes": Sequence[AttributeTypeDef],
         "platformDevices": Sequence[PlatformDeviceTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredServiceConnectServiceTypeDef = TypedDict(
+    "_RequiredServiceConnectServiceTypeDef",
+    {
+        "portName": str,
+    },
+)
+_OptionalServiceConnectServiceTypeDef = TypedDict(
+    "_OptionalServiceConnectServiceTypeDef",
+    {
+        "discoveryName": str,
+        "clientAliases": Sequence[ServiceConnectClientAliasTypeDef],
+        "ingressPortOverride": int,
+    },
+    total=False,
+)
+
+
+class ServiceConnectServiceTypeDef(
+    _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
+):
+    pass
+
+
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2142,20 +2375,22 @@
     "_OptionalCreateCapacityProviderRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCapacityProviderRequestRequestTypeDef(
     _RequiredCreateCapacityProviderRequestRequestTypeDef,
     _OptionalCreateCapacityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateCapacityProviderRequestRequestTypeDef = TypedDict(
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
@@ -2181,41 +2416,20 @@
         "scale": ScaleTypeDef,
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-    },
-    total=False,
-)
 
 TaskSetTypeDef = TypedDict(
     "TaskSetTypeDef",
     {
         "id": str,
         "taskSetArn": str,
         "serviceArn": str,
@@ -2296,87 +2510,14 @@
         "pullStartedAt": Union[datetime, str],
         "pullStoppedAt": Union[datetime, str],
         "executionStoppedAt": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "taskDefinition": str,
-        "loadBalancers": Sequence[LoadBalancerTypeDef],
-        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
-        "desiredCount": int,
-        "clientToken": str,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "role": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
-        "placementConstraints": Sequence[PlacementConstraintTypeDef],
-        "placementStrategy": Sequence[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "healthCheckGracePeriodSeconds": int,
-        "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "enableECSManagedTags": bool,
-        "propagateTags": PropagateTagsType,
-        "enableExecuteCommand": bool,
-    },
-    total=False,
-)
-
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
-    {
-        "service": str,
-    },
-)
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "desiredCount": int,
-        "taskDefinition": str,
-        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "placementConstraints": Sequence[PlacementConstraintTypeDef],
-        "placementStrategy": Sequence[PlacementStrategyTypeDef],
-        "platformVersion": str,
-        "forceNewDeployment": bool,
-        "healthCheckGracePeriodSeconds": int,
-        "enableExecuteCommand": bool,
-        "enableECSManagedTags": bool,
-        "loadBalancers": Sequence[LoadBalancerTypeDef],
-        "propagateTags": PropagateTagsType,
-        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
-    },
-    total=False,
-)
-
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
-
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
@@ -2435,14 +2576,37 @@
         "systemControls": List[SystemControlTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredServiceConnectConfigurationTypeDef = TypedDict(
+    "_RequiredServiceConnectConfigurationTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalServiceConnectConfigurationTypeDef = TypedDict(
+    "_OptionalServiceConnectConfigurationTypeDef",
+    {
+        "namespace": str,
+        "services": Sequence[ServiceConnectServiceTypeDef],
+        "logConfiguration": LogConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class ServiceConnectConfigurationTypeDef(
+    _RequiredServiceConnectConfigurationTypeDef, _OptionalServiceConnectConfigurationTypeDef
+):
+    pass
+
+
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2494,52 +2658,14 @@
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServiceTypeDef = TypedDict(
-    "ServiceTypeDef",
-    {
-        "serviceArn": str,
-        "serviceName": str,
-        "clusterArn": str,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "status": str,
-        "desiredCount": int,
-        "runningCount": int,
-        "pendingCount": int,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationTypeDef,
-        "taskSets": List[TaskSetTypeDef],
-        "deployments": List[DeploymentTypeDef],
-        "roleArn": str,
-        "events": List[ServiceEventTypeDef],
-        "createdAt": datetime,
-        "placementConstraints": List[PlacementConstraintTypeDef],
-        "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "healthCheckGracePeriodSeconds": int,
-        "schedulingStrategy": SchedulingStrategyType,
-        "deploymentController": DeploymentControllerTypeDef,
-        "tags": List[TagTypeDef],
-        "createdBy": str,
-        "enableECSManagedTags": bool,
-        "propagateTags": PropagateTagsType,
-        "enableExecuteCommand": bool,
-    },
-    total=False,
-)
-
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2577,19 +2703,21 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class RunTaskRequestRequestTypeDef(
     _RequiredRunTaskRequestRequestTypeDef, _OptionalRunTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "taskDefinition": str,
     },
 )
@@ -2606,19 +2734,21 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
+
 TaskTypeDef = TypedDict(
     "TaskTypeDef",
     {
         "attachments": List[AttachmentTypeDef],
         "attributes": List[AttributeTypeDef],
         "availabilityZone": str,
         "capacityProviderName": str,
@@ -2714,27 +2844,29 @@
         "statistics": List[KeyValuePairTypeDef],
         "tags": List[TagTypeDef],
         "settings": List[ClusterSettingTypeDef],
         "capacityProviders": List[str],
         "defaultCapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "attachments": List[AttachmentTypeDef],
         "attachmentsStatus": str,
+        "serviceConnectDefaults": ClusterServiceConnectDefaultsTypeDef,
     },
     total=False,
 )
 
 CreateClusterRequestRequestTypeDef = TypedDict(
     "CreateClusterRequestRequestTypeDef",
     {
         "clusterName": str,
         "tags": Sequence[TagTypeDef],
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
@@ -2742,23 +2874,26 @@
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateClusterRequestRequestTypeDef",
     {
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
+        "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
+
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
     {
         "family": str,
         "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
     },
 )
@@ -2780,20 +2915,22 @@
         "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
         "ephemeralStorage": EphemeralStorageTypeDef,
         "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
+
 class RegisterTaskDefinitionRequestRequestTypeDef(
     _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
     _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
         "containerDefinitions": List[ContainerDefinitionTypeDef],
         "family": str,
         "taskRoleArn": str,
@@ -2817,47 +2954,118 @@
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-CreateServiceResponseTypeDef = TypedDict(
-    "CreateServiceResponseTypeDef",
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
     {
-        "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serviceName": str,
     },
 )
-
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
     {
-        "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": str,
+        "taskDefinition": str,
+        "loadBalancers": Sequence[LoadBalancerTypeDef],
+        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
+        "desiredCount": int,
+        "clientToken": str,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "role": str,
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "placementConstraints": Sequence[PlacementConstraintTypeDef],
+        "placementStrategy": Sequence[PlacementStrategyTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "healthCheckGracePeriodSeconds": int,
+        "schedulingStrategy": SchedulingStrategyType,
+        "deploymentController": DeploymentControllerTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "enableECSManagedTags": bool,
+        "propagateTags": PropagateTagsType,
+        "enableExecuteCommand": bool,
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
+    total=False,
 )
 
-DescribeServicesResponseTypeDef = TypedDict(
-    "DescribeServicesResponseTypeDef",
+
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
+    pass
+
+
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
     {
-        "services": List[ServiceTypeDef],
-        "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
     },
+    total=False,
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
     {
-        "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "service": str,
+    },
+)
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
+    {
+        "cluster": str,
+        "desiredCount": int,
+        "taskDefinition": str,
+        "capacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "placementConstraints": Sequence[PlacementConstraintTypeDef],
+        "placementStrategy": Sequence[PlacementStrategyTypeDef],
+        "platformVersion": str,
+        "forceNewDeployment": bool,
+        "healthCheckGracePeriodSeconds": int,
+        "enableExecuteCommand": bool,
+        "enableECSManagedTags": bool,
+        "loadBalancers": Sequence[LoadBalancerTypeDef],
+        "propagateTags": PropagateTagsType,
+        "serviceRegistries": Sequence[ServiceRegistryTypeDef],
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
+    total=False,
 )
 
+
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
+
+
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2934,14 +3142,23 @@
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteTaskDefinitionsResponseTypeDef = TypedDict(
+    "DeleteTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitions": List[TaskDefinitionTypeDef],
+        "failures": List[FailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2959,7 +3176,78 @@
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
+    {
+        "serviceArn": str,
+        "serviceName": str,
+        "clusterArn": str,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "status": str,
+        "desiredCount": int,
+        "runningCount": int,
+        "pendingCount": int,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "taskDefinition": str,
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
+        "taskSets": List[TaskSetTypeDef],
+        "deployments": List[DeploymentTypeDef],
+        "roleArn": str,
+        "events": List[ServiceEventTypeDef],
+        "createdAt": datetime,
+        "placementConstraints": List[PlacementConstraintTypeDef],
+        "placementStrategy": List[PlacementStrategyTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "healthCheckGracePeriodSeconds": int,
+        "schedulingStrategy": SchedulingStrategyType,
+        "deploymentController": DeploymentControllerTypeDef,
+        "tags": List[TagTypeDef],
+        "createdBy": str,
+        "enableECSManagedTags": bool,
+        "propagateTags": PropagateTagsType,
+        "enableExecuteCommand": bool,
+    },
+    total=False,
+)
+
+CreateServiceResponseTypeDef = TypedDict(
+    "CreateServiceResponseTypeDef",
+    {
+        "service": ServiceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "service": ServiceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeServicesResponseTypeDef = TypedDict(
+    "DescribeServicesResponseTypeDef",
+    {
+        "services": List[ServiceTypeDef],
+        "failures": List[FailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "service": ServiceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/PKG-INFO` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.26.7
-Summary: Type annotations for boto3.ECS 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.78
+Summary: Type annotations for boto3.ECS 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +284,15 @@
 from mypy_boto3_ecs import ECSClient
 from mypy_boto3_ecs.paginator import (
     ListAccountSettingsPaginator,
     ListAttributesPaginator,
     ListClustersPaginator,
     ListContainerInstancesPaginator,
     ListServicesPaginator,
+    ListServicesByNamespacePaginator,
     ListTaskDefinitionFamiliesPaginator,
     ListTaskDefinitionsPaginator,
     ListTasksPaginator,
 )
 
 client: ECSClient = Session().client("ecs")
 
@@ -301,14 +303,17 @@
 )
 list_attributes_paginator: ListAttributesPaginator = client.get_paginator("list_attributes")
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_container_instances_paginator: ListContainerInstancesPaginator = client.get_paginator(
     "list_container_instances"
 )
 list_services_paginator: ListServicesPaginator = client.get_paginator("list_services")
+list_services_by_namespace_paginator: ListServicesByNamespacePaginator = client.get_paginator(
+    "list_services_by_namespace"
+)
 list_task_definition_families_paginator: ListTaskDefinitionFamiliesPaginator = client.get_paginator(
     "list_task_definition_families"
 )
 list_task_definitions_paginator: ListTaskDefinitionsPaginator = client.get_paginator(
     "list_task_definitions"
 )
 list_tasks_paginator: ListTasksPaginator = client.get_paginator("list_tasks")
@@ -347,14 +352,15 @@
 
 `mypy_boto3_ecs.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ecs.literals import (
     AgentUpdateStatusType,
+    ApplicationProtocolType,
     AssignPublicIpType,
     CPUArchitectureType,
     CapacityProviderFieldType,
     CapacityProviderStatusType,
     CapacityProviderUpdateStatusType,
     ClusterFieldType,
     ClusterSettingNameType,
@@ -377,14 +383,15 @@
     InstanceHealthCheckTypeType,
     IpcModeType,
     LaunchTypeType,
     ListAccountSettingsPaginatorName,
     ListAttributesPaginatorName,
     ListClustersPaginatorName,
     ListContainerInstancesPaginatorName,
+    ListServicesByNamespacePaginatorName,
     ListServicesPaginatorName,
     ListTaskDefinitionFamiliesPaginatorName,
     ListTaskDefinitionsPaginatorName,
     ListTasksPaginatorName,
     LogDriverType,
     ManagedAgentNameType,
     ManagedScalingStatusType,
@@ -444,14 +451,16 @@
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
+    ClusterServiceConnectDefaultsRequestTypeDef,
+    ClusterServiceConnectDefaultsTypeDef,
     ClusterSettingTypeDef,
     ContainerDependencyTypeDef,
     EnvironmentFileTypeDef,
     FirelensConfigurationTypeDef,
     HealthCheckTypeDef,
     HostEntryTypeDef,
     MountPointTypeDef,
@@ -476,20 +485,23 @@
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
     SettingTypeDef,
     DeleteCapacityProviderRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
+    DeleteTaskDefinitionsRequestRequestTypeDef,
+    FailureTypeDef,
     DeleteTaskSetRequestRequestTypeDef,
+    DeploymentAlarmsTypeDef,
     DeploymentCircuitBreakerTypeDef,
+    ServiceConnectServiceResourceTypeDef,
     DeregisterContainerInstanceRequestRequestTypeDef,
     DeregisterTaskDefinitionRequestRequestTypeDef,
     DescribeCapacityProvidersRequestRequestTypeDef,
-    FailureTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeContainerInstancesRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
@@ -510,25 +522,27 @@
     KernelCapabilitiesTypeDef,
     TmpfsTypeDef,
     PaginatorConfigTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
     ListAttributesRequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
+    ListServicesByNamespaceRequestRequestTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTasksRequestRequestTypeDef,
     ManagedAgentStateChangeTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
@@ -550,14 +564,15 @@
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
     DeleteAttributesResponseTypeDef,
     DiscoverPollEndpointResponseTypeDef,
     ListAttributesResponseTypeDef,
     ListClustersResponseTypeDef,
     ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     PutAttributesResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
@@ -580,41 +595,40 @@
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersTypeDef,
     ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAttributesRequestListAttributesPaginateTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
+    ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     CreateTaskSetRequestRequestTypeDef,
-    DeploymentTypeDef,
     TaskSetTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
-    CreateServiceRequestRequestTypeDef,
-    UpdateServiceRequestRequestTypeDef,
     ClusterConfigurationTypeDef,
     VolumeTypeDef,
     ContainerDefinitionTypeDef,
+    ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
-    ServiceTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
     TaskTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
@@ -622,31 +636,36 @@
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     RegisterTaskDefinitionRequestRequestTypeDef,
     TaskDefinitionTypeDef,
-    CreateServiceResponseTypeDef,
-    DeleteServiceResponseTypeDef,
-    DescribeServicesResponseTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    DeploymentTypeDef,
+    UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
+    DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    ServiceTypeDef,
+    CreateServiceResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DescribeServicesResponseTypeDef,
+    UpdateServiceResponseTypeDef,
 )
 
 
 def get_structure() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-ecs-1.26.7/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.7/setup.py` & `mypy-boto3-ecs-1.26.78/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.26.7",
+    version="1.26.78",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECS 1.26.7 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ECS 1.26.78 service generated with mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 ecs type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_ecs": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_ecs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

