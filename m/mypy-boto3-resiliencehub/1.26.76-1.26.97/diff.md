# Comparing `tmp/mypy-boto3-resiliencehub-1.26.76.tar.gz` & `tmp/mypy-boto3-resiliencehub-1.26.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resiliencehub-1.26.76.tar", last modified: Tue Feb 21 21:33:38 2023, max compression
+gzip compressed data, was "mypy-boto3-resiliencehub-1.26.97.tar", last modified: Wed Mar 22 19:32:31 2023, max compression
```

## Comparing `mypy-boto3-resiliencehub-1.26.76.tar` & `mypy-boto3-resiliencehub-1.26.97.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:33:38.003356 mypy-boto3-resiliencehub-1.26.76/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-02-21 21:33:38.003356 mypy-boto3-resiliencehub-1.26.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:33:38.003356 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39425 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59662 2023-02-21 21:33:13.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59559 2023-02-21 21:33:13.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:33:38.003356 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-02-21 21:33:37.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-21 21:33:37.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:33:37.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:33:37.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-21 21:33:37.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-21 21:33:37.000000 mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 21:33:38.003356 mypy-boto3-resiliencehub-1.26.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-21 21:33:11.000000 mypy-boto3-resiliencehub-1.26.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.373775 mypy-boto3-resiliencehub-1.26.97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-03-22 19:32:31.369775 mypy-boto3-resiliencehub-1.26.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.365775 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39566 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39508 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-03-22 19:32:12.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-03-22 19:32:12.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60670 2023-03-22 19:32:13.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60565 2023-03-22 19:32:12.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.369775 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:32:31.373775 mypy-boto3-resiliencehub-1.26.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/setup.py
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/LICENSE` & `mypy-boto3-resiliencehub-1.26.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.26.76/PKG-INFO` & `mypy-boto3-resiliencehub-1.26.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.26.76
-Summary: Type annotations for boto3.ResilienceHub 1.26.76 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.97
+Summary: Type annotations for boto3.ResilienceHub 1.26.97 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.26.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,14 +328,15 @@
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
+    EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
@@ -351,14 +352,15 @@
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -407,29 +409,29 @@
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
     DeleteAppInputSourceRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    ImportResourcesToDraftAppVersionResponseTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/README.md` & `mypy-boto3-resiliencehub-1.26.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.26.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,14 +296,15 @@
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
+    EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
@@ -319,14 +320,15 @@
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -375,29 +377,29 @@
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
     DeleteAppInputSourceRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    ImportResourcesToDraftAppVersionResponseTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/__main__.py` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResilienceHub 1.26.76\nVersion:         1.26.76\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.ResilienceHub 1.26.97\nVersion:         1.26.97\nBuilder"
+        " version: 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.76")
+    print("1.26.97")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/client.py` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     DescribeAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    EksSourceTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
@@ -159,15 +161,15 @@
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
-        Creates an AWS Resilience Hub application.
+        Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app)
         """
 
     def create_app_version_app_component(
         self,
@@ -176,15 +178,15 @@
         name: str,
         type: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         clientToken: str = ...,
         id: str = ...
     ) -> CreateAppVersionAppComponentResponseTypeDef:
         """
-        Creates a new Application Component in the AWS Resilience Hub application.
+        Creates a new Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_app_component)
         """
 
     def create_app_version_resource(
         self,
@@ -197,15 +199,15 @@
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
-        Adds a resource to the AWS Resilience Hub applicationand assigns it to the
+        Adds a resource to the Resilience Hub application and assigns it to the
         specified Application Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_resource)
         """
 
     def create_recommendation_template(
@@ -217,15 +219,15 @@
         clientToken: str = ...,
         format: TemplateFormatType = ...,
         recommendationIds: Sequence[str] = ...,
         recommendationTypes: Sequence[RenderRecommendationTypeType] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRecommendationTemplateResponseTypeDef:
         """
-        Creates a new recommendation template for the AWS Resilience Hub application.
+        Creates a new recommendation template for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_recommendation_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_recommendation_template)
         """
 
     def create_resiliency_policy(
         self,
@@ -245,51 +247,52 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_resiliency_policy)
         """
 
     def delete_app(
         self, *, appArn: str, clientToken: str = ..., forceDelete: bool = ...
     ) -> DeleteAppResponseTypeDef:
         """
-        Deletes an AWS Resilience Hub application.
+        Deletes an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app)
         """
 
     def delete_app_assessment(
         self, *, assessmentArn: str, clientToken: str = ...
     ) -> DeleteAppAssessmentResponseTypeDef:
         """
-        Deletes an AWS Resilience Hub application assessment.
+        Deletes an Resilience Hub application assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_assessment)
         """
 
     def delete_app_input_source(
         self,
         *,
         appArn: str,
         clientToken: str = ...,
+        eksSourceClusterNamespace: EksSourceClusterNamespaceTypeDef = ...,
         sourceArn: str = ...,
         terraformSource: TerraformSourceTypeDef = ...
     ) -> DeleteAppInputSourceResponseTypeDef:
         """
-        Deletes the input source and all of its imported resources from the AWS
-        Resilience Hub application.
+        Deletes the input source and all of its imported resources from the Resilience
+        Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_input_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_input_source)
         """
 
     def delete_app_version_app_component(
         self, *, appArn: str, id: str, clientToken: str = ...
     ) -> DeleteAppVersionAppComponentResponseTypeDef:
         """
-        Deletes an Application Component from the AWS Resilience Hub application.
+        Deletes an Application Component from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_version_app_component)
         """
 
     def delete_app_version_resource(
         self,
@@ -299,15 +302,15 @@
         awsRegion: str = ...,
         clientToken: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...
     ) -> DeleteAppVersionResourceResponseTypeDef:
         """
-        Deletes a resource from the AWS Resilience Hub application.
+        Deletes a resource from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_version_resource)
         """
 
     def delete_recommendation_template(
         self, *, recommendationTemplateArn: str, clientToken: str = ...
@@ -327,45 +330,45 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_resiliency_policy)
         """
 
     def describe_app(self, *, appArn: str) -> DescribeAppResponseTypeDef:
         """
-        Describes an AWS Resilience Hub application.
+        Describes an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app)
         """
 
     def describe_app_assessment(
         self, *, assessmentArn: str
     ) -> DescribeAppAssessmentResponseTypeDef:
         """
-        Describes an assessment for an AWS Resilience Hub application.
+        Describes an assessment for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_assessment)
         """
 
     def describe_app_version(
         self, *, appArn: str, appVersion: str
     ) -> DescribeAppVersionResponseTypeDef:
         """
-        Describes the AWS Resilience Hub application version.
+        Describes the Resilience Hub application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version)
         """
 
     def describe_app_version_app_component(
         self, *, appArn: str, appVersion: str, id: str
     ) -> DescribeAppVersionAppComponentResponseTypeDef:
         """
-        Describes an Application Component in the AWS Resilience Hub application.
+        Describes an Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_app_component)
         """
 
     def describe_app_version_resource(
         self,
@@ -375,15 +378,15 @@
         awsAccountId: str = ...,
         awsRegion: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...
     ) -> DescribeAppVersionResourceResponseTypeDef:
         """
-        Describes a resource of the AWS Resilience Hub application.
+        Describes a resource of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_resource)
         """
 
     def describe_app_version_resources_resolution_status(
         self, *, appArn: str, appVersion: str, resolutionId: str = ...
@@ -396,15 +399,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_resources_resolution_status)
         """
 
     def describe_app_version_template(
         self, *, appArn: str, appVersion: str
     ) -> DescribeAppVersionTemplateResponseTypeDef:
         """
-        Describes details about an AWS Resilience Hub application.
+        Describes details about an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_template)
         """
 
     def describe_draft_app_version_resources_import_status(
         self, *, appArn: str
@@ -416,15 +419,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_draft_app_version_resources_import_status)
         """
 
     def describe_resiliency_policy(
         self, *, policyArn: str
     ) -> DescribeResiliencyPolicyResponseTypeDef:
         """
-        Describes a specified resiliency policy for an AWS Resilience Hub application.
+        Describes a specified resiliency policy for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_resiliency_policy)
         """
 
     def generate_presigned_url(
         self,
@@ -440,31 +443,32 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#generate_presigned_url)
         """
 
     def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
+        eksSources: Sequence[EksSourceTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
-        Imports resources to AWS Resilience Hub application draft version from different
+        Imports resources to Resilience Hub application draft version from different
         input sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.import_resources_to_draft_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#import_resources_to_draft_app_version)
         """
 
     def list_alarm_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAlarmRecommendationsResponseTypeDef:
         """
-        Lists the alarm recommendations for an AWS Resilience Hub application.
+        Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_alarm_recommendations)
         """
 
     def list_app_assessments(
         self,
@@ -475,55 +479,55 @@
         complianceStatus: ComplianceStatusType = ...,
         invoker: AssessmentInvokerType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         reverseOrder: bool = ...
     ) -> ListAppAssessmentsResponseTypeDef:
         """
-        Lists the assessments for an AWS Resilience Hub application.
+        Lists the assessments for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessments)
         """
 
     def list_app_component_compliances(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppComponentCompliancesResponseTypeDef:
         """
-        Lists the compliances for an AWS Resilience Hub Application Component.
+        Lists the compliances for an Resilience Hub Application Component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_component_compliances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_component_compliances)
         """
 
     def list_app_component_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppComponentRecommendationsResponseTypeDef:
         """
-        Lists the recommendations for an AWS Resilience Hub Application Component.
+        Lists the recommendations for an Resilience Hub Application Component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_component_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_component_recommendations)
         """
 
     def list_app_input_sources(
         self, *, appArn: str, appVersion: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppInputSourcesResponseTypeDef:
         """
-        Lists all the input sources of the AWS Resilience Hub application.
+        Lists all the input sources of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_input_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_input_sources)
         """
 
     def list_app_version_app_components(
         self, *, appArn: str, appVersion: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppVersionAppComponentsResponseTypeDef:
         """
-        Lists all the Application Components in the AWS Resilience Hub application.
+        Lists all the Application Components in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_app_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_app_components)
         """
 
     def list_app_version_resource_mappings(
         self, *, appArn: str, appVersion: str, maxResults: int = ..., nextToken: str = ...
@@ -541,35 +545,35 @@
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
         resolutionId: str = ...
     ) -> ListAppVersionResourcesResponseTypeDef:
         """
-        Lists all the resources in an AWS Resilience Hub application.
+        Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_resources)
         """
 
     def list_app_versions(
         self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
-        Lists the different versions for the AWS Resilience Hub applications.
+        Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_versions)
         """
 
     def list_apps(
         self, *, appArn: str = ..., maxResults: int = ..., name: str = ..., nextToken: str = ...
     ) -> ListAppsResponseTypeDef:
         """
-        Lists your AWS Resilience Hub applications.
+        Lists your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_apps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_apps)
         """
 
     def list_recommendation_templates(
         self,
@@ -579,64 +583,64 @@
         name: str = ...,
         nextToken: str = ...,
         recommendationTemplateArn: str = ...,
         reverseOrder: bool = ...,
         status: Sequence[RecommendationTemplateStatusType] = ...
     ) -> ListRecommendationTemplatesResponseTypeDef:
         """
-        Lists the recommendation templates for the AWS Resilience Hub applications.
+        Lists the recommendation templates for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_recommendation_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_recommendation_templates)
         """
 
     def list_resiliency_policies(
         self, *, maxResults: int = ..., nextToken: str = ..., policyName: str = ...
     ) -> ListResiliencyPoliciesResponseTypeDef:
         """
-        Lists the resiliency policies for the AWS Resilience Hub applications.
+        Lists the resiliency policies for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_resiliency_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_resiliency_policies)
         """
 
     def list_sop_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListSopRecommendationsResponseTypeDef:
         """
-        Lists the standard operating procedure (SOP) recommendations for the AWS
-        Resilience Hub applications.
+        Lists the standard operating procedure (SOP) recommendations for the Resilience
+        Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_sop_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_sop_recommendations)
         """
 
     def list_suggested_resiliency_policies(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListSuggestedResiliencyPoliciesResponseTypeDef:
         """
-        Lists the suggested resiliency policies for the AWS Resilience Hub applications.
+        Lists the suggested resiliency policies for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_suggested_resiliency_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_suggested_resiliency_policies)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Lists the tags for your resources in your AWS Resilience Hub applications.
+        Lists the tags for your resources in your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_tags_for_resource)
         """
 
     def list_test_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTestRecommendationsResponseTypeDef:
         """
-        Lists the test recommendations for the AWS Resilience Hub application.
+        Lists the test recommendations for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_test_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_test_recommendations)
         """
 
     def list_unsupported_app_version_resources(
         self,
@@ -644,44 +648,45 @@
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
         resolutionId: str = ...
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
-        Lists the resources that are not currently supported in AWS Resilience Hub.
+        Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_unsupported_app_version_resources)
         """
 
     def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
         """
-        Publishes a new version of a specific AWS Resilience Hub application.
+        Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#publish_app_version)
         """
 
     def put_draft_app_version_template(
         self, *, appArn: str, appTemplateBody: str
     ) -> PutDraftAppVersionTemplateResponseTypeDef:
         """
-        Adds or updates the app template for an AWS Resilience Hub application draft
+        Adds or updates the app template for an Resilience Hub application draft
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.put_draft_app_version_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#put_draft_app_version_template)
         """
 
     def remove_draft_app_version_resource_mappings(
         self,
         *,
         appArn: str,
         appRegistryAppNames: Sequence[str] = ...,
+        eksSourceNames: Sequence[str] = ...,
         logicalStackNames: Sequence[str] = ...,
         resourceGroupNames: Sequence[str] = ...,
         resourceNames: Sequence[str] = ...,
         terraformSourceNames: Sequence[str] = ...
     ) -> RemoveDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Removes resource mappings from a draft application version.
@@ -748,15 +753,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app)
         """
 
     def update_app_version(
         self, *, appArn: str, additionalInfo: Mapping[str, Sequence[str]] = ...
     ) -> UpdateAppVersionResponseTypeDef:
         """
-        Updates the AWS Resilience Hub application version.
+        Updates the Resilience Hub application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version)
         """
 
     def update_app_version_app_component(
         self,
@@ -764,15 +769,15 @@
         appArn: str,
         id: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         name: str = ...,
         type: str = ...
     ) -> UpdateAppVersionAppComponentResponseTypeDef:
         """
-        Updates an existing Application Component in the AWS Resilience Hub application.
+        Updates an existing Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_app_component)
         """
 
     def update_app_version_resource(
         self,
@@ -785,15 +790,15 @@
         excluded: bool = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...,
         resourceType: str = ...
     ) -> UpdateAppVersionResourceResponseTypeDef:
         """
-        Updates the resource details in the AWS Resilience Hub application.
+        Updates the resource details in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_resource)
         """
 
     def update_resiliency_policy(
         self,
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/client.pyi` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     DescribeAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    EksSourceTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
@@ -152,15 +154,15 @@
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
-        Creates an AWS Resilience Hub application.
+        Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app)
         """
     def create_app_version_app_component(
         self,
         *,
@@ -168,15 +170,15 @@
         name: str,
         type: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         clientToken: str = ...,
         id: str = ...
     ) -> CreateAppVersionAppComponentResponseTypeDef:
         """
-        Creates a new Application Component in the AWS Resilience Hub application.
+        Creates a new Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_app_component)
         """
     def create_app_version_resource(
         self,
         *,
@@ -188,15 +190,15 @@
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
         clientToken: str = ...
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
-        Adds a resource to the AWS Resilience Hub applicationand assigns it to the
+        Adds a resource to the Resilience Hub application and assigns it to the
         specified Application Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_resource)
         """
     def create_recommendation_template(
         self,
@@ -207,15 +209,15 @@
         clientToken: str = ...,
         format: TemplateFormatType = ...,
         recommendationIds: Sequence[str] = ...,
         recommendationTypes: Sequence[RenderRecommendationTypeType] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRecommendationTemplateResponseTypeDef:
         """
-        Creates a new recommendation template for the AWS Resilience Hub application.
+        Creates a new recommendation template for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_recommendation_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_recommendation_template)
         """
     def create_resiliency_policy(
         self,
         *,
@@ -233,48 +235,49 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_resiliency_policy)
         """
     def delete_app(
         self, *, appArn: str, clientToken: str = ..., forceDelete: bool = ...
     ) -> DeleteAppResponseTypeDef:
         """
-        Deletes an AWS Resilience Hub application.
+        Deletes an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app)
         """
     def delete_app_assessment(
         self, *, assessmentArn: str, clientToken: str = ...
     ) -> DeleteAppAssessmentResponseTypeDef:
         """
-        Deletes an AWS Resilience Hub application assessment.
+        Deletes an Resilience Hub application assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_assessment)
         """
     def delete_app_input_source(
         self,
         *,
         appArn: str,
         clientToken: str = ...,
+        eksSourceClusterNamespace: EksSourceClusterNamespaceTypeDef = ...,
         sourceArn: str = ...,
         terraformSource: TerraformSourceTypeDef = ...
     ) -> DeleteAppInputSourceResponseTypeDef:
         """
-        Deletes the input source and all of its imported resources from the AWS
-        Resilience Hub application.
+        Deletes the input source and all of its imported resources from the Resilience
+        Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_input_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_input_source)
         """
     def delete_app_version_app_component(
         self, *, appArn: str, id: str, clientToken: str = ...
     ) -> DeleteAppVersionAppComponentResponseTypeDef:
         """
-        Deletes an Application Component from the AWS Resilience Hub application.
+        Deletes an Application Component from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_version_app_component)
         """
     def delete_app_version_resource(
         self,
         *,
@@ -283,15 +286,15 @@
         awsRegion: str = ...,
         clientToken: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...
     ) -> DeleteAppVersionResourceResponseTypeDef:
         """
-        Deletes a resource from the AWS Resilience Hub application.
+        Deletes a resource from the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_app_version_resource)
         """
     def delete_recommendation_template(
         self, *, recommendationTemplateArn: str, clientToken: str = ...
     ) -> DeleteRecommendationTemplateResponseTypeDef:
@@ -308,42 +311,42 @@
         Deletes a resiliency policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.delete_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#delete_resiliency_policy)
         """
     def describe_app(self, *, appArn: str) -> DescribeAppResponseTypeDef:
         """
-        Describes an AWS Resilience Hub application.
+        Describes an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app)
         """
     def describe_app_assessment(
         self, *, assessmentArn: str
     ) -> DescribeAppAssessmentResponseTypeDef:
         """
-        Describes an assessment for an AWS Resilience Hub application.
+        Describes an assessment for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_assessment)
         """
     def describe_app_version(
         self, *, appArn: str, appVersion: str
     ) -> DescribeAppVersionResponseTypeDef:
         """
-        Describes the AWS Resilience Hub application version.
+        Describes the Resilience Hub application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version)
         """
     def describe_app_version_app_component(
         self, *, appArn: str, appVersion: str, id: str
     ) -> DescribeAppVersionAppComponentResponseTypeDef:
         """
-        Describes an Application Component in the AWS Resilience Hub application.
+        Describes an Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_app_component)
         """
     def describe_app_version_resource(
         self,
         *,
@@ -352,15 +355,15 @@
         awsAccountId: str = ...,
         awsRegion: str = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...
     ) -> DescribeAppVersionResourceResponseTypeDef:
         """
-        Describes a resource of the AWS Resilience Hub application.
+        Describes a resource of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_resource)
         """
     def describe_app_version_resources_resolution_status(
         self, *, appArn: str, appVersion: str, resolutionId: str = ...
     ) -> DescribeAppVersionResourcesResolutionStatusResponseTypeDef:
@@ -371,15 +374,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_resources_resolution_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_resources_resolution_status)
         """
     def describe_app_version_template(
         self, *, appArn: str, appVersion: str
     ) -> DescribeAppVersionTemplateResponseTypeDef:
         """
-        Describes details about an AWS Resilience Hub application.
+        Describes details about an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_app_version_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_app_version_template)
         """
     def describe_draft_app_version_resources_import_status(
         self, *, appArn: str
     ) -> DescribeDraftAppVersionResourcesImportStatusResponseTypeDef:
@@ -389,15 +392,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_draft_app_version_resources_import_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_draft_app_version_resources_import_status)
         """
     def describe_resiliency_policy(
         self, *, policyArn: str
     ) -> DescribeResiliencyPolicyResponseTypeDef:
         """
-        Describes a specified resiliency policy for an AWS Resilience Hub application.
+        Describes a specified resiliency policy for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.describe_resiliency_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#describe_resiliency_policy)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -411,30 +414,31 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#generate_presigned_url)
         """
     def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
+        eksSources: Sequence[EksSourceTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
-        Imports resources to AWS Resilience Hub application draft version from different
+        Imports resources to Resilience Hub application draft version from different
         input sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.import_resources_to_draft_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#import_resources_to_draft_app_version)
         """
     def list_alarm_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAlarmRecommendationsResponseTypeDef:
         """
-        Lists the alarm recommendations for an AWS Resilience Hub application.
+        Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_alarm_recommendations)
         """
     def list_app_assessments(
         self,
         *,
@@ -444,51 +448,51 @@
         complianceStatus: ComplianceStatusType = ...,
         invoker: AssessmentInvokerType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         reverseOrder: bool = ...
     ) -> ListAppAssessmentsResponseTypeDef:
         """
-        Lists the assessments for an AWS Resilience Hub application.
+        Lists the assessments for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessments)
         """
     def list_app_component_compliances(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppComponentCompliancesResponseTypeDef:
         """
-        Lists the compliances for an AWS Resilience Hub Application Component.
+        Lists the compliances for an Resilience Hub Application Component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_component_compliances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_component_compliances)
         """
     def list_app_component_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppComponentRecommendationsResponseTypeDef:
         """
-        Lists the recommendations for an AWS Resilience Hub Application Component.
+        Lists the recommendations for an Resilience Hub Application Component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_component_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_component_recommendations)
         """
     def list_app_input_sources(
         self, *, appArn: str, appVersion: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppInputSourcesResponseTypeDef:
         """
-        Lists all the input sources of the AWS Resilience Hub application.
+        Lists all the input sources of the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_input_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_input_sources)
         """
     def list_app_version_app_components(
         self, *, appArn: str, appVersion: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppVersionAppComponentsResponseTypeDef:
         """
-        Lists all the Application Components in the AWS Resilience Hub application.
+        Lists all the Application Components in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_app_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_app_components)
         """
     def list_app_version_resource_mappings(
         self, *, appArn: str, appVersion: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppVersionResourceMappingsResponseTypeDef:
@@ -504,33 +508,33 @@
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
         resolutionId: str = ...
     ) -> ListAppVersionResourcesResponseTypeDef:
         """
-        Lists all the resources in an AWS Resilience Hub application.
+        Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_resources)
         """
     def list_app_versions(
         self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
-        Lists the different versions for the AWS Resilience Hub applications.
+        Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_versions)
         """
     def list_apps(
         self, *, appArn: str = ..., maxResults: int = ..., name: str = ..., nextToken: str = ...
     ) -> ListAppsResponseTypeDef:
         """
-        Lists your AWS Resilience Hub applications.
+        Lists your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_apps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_apps)
         """
     def list_recommendation_templates(
         self,
         *,
@@ -539,100 +543,101 @@
         name: str = ...,
         nextToken: str = ...,
         recommendationTemplateArn: str = ...,
         reverseOrder: bool = ...,
         status: Sequence[RecommendationTemplateStatusType] = ...
     ) -> ListRecommendationTemplatesResponseTypeDef:
         """
-        Lists the recommendation templates for the AWS Resilience Hub applications.
+        Lists the recommendation templates for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_recommendation_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_recommendation_templates)
         """
     def list_resiliency_policies(
         self, *, maxResults: int = ..., nextToken: str = ..., policyName: str = ...
     ) -> ListResiliencyPoliciesResponseTypeDef:
         """
-        Lists the resiliency policies for the AWS Resilience Hub applications.
+        Lists the resiliency policies for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_resiliency_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_resiliency_policies)
         """
     def list_sop_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListSopRecommendationsResponseTypeDef:
         """
-        Lists the standard operating procedure (SOP) recommendations for the AWS
-        Resilience Hub applications.
+        Lists the standard operating procedure (SOP) recommendations for the Resilience
+        Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_sop_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_sop_recommendations)
         """
     def list_suggested_resiliency_policies(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListSuggestedResiliencyPoliciesResponseTypeDef:
         """
-        Lists the suggested resiliency policies for the AWS Resilience Hub applications.
+        Lists the suggested resiliency policies for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_suggested_resiliency_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_suggested_resiliency_policies)
         """
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Lists the tags for your resources in your AWS Resilience Hub applications.
+        Lists the tags for your resources in your Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_tags_for_resource)
         """
     def list_test_recommendations(
         self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTestRecommendationsResponseTypeDef:
         """
-        Lists the test recommendations for the AWS Resilience Hub application.
+        Lists the test recommendations for the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_test_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_test_recommendations)
         """
     def list_unsupported_app_version_resources(
         self,
         *,
         appArn: str,
         appVersion: str,
         maxResults: int = ...,
         nextToken: str = ...,
         resolutionId: str = ...
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
-        Lists the resources that are not currently supported in AWS Resilience Hub.
+        Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_unsupported_app_version_resources)
         """
     def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
         """
-        Publishes a new version of a specific AWS Resilience Hub application.
+        Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#publish_app_version)
         """
     def put_draft_app_version_template(
         self, *, appArn: str, appTemplateBody: str
     ) -> PutDraftAppVersionTemplateResponseTypeDef:
         """
-        Adds or updates the app template for an AWS Resilience Hub application draft
+        Adds or updates the app template for an Resilience Hub application draft
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.put_draft_app_version_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#put_draft_app_version_template)
         """
     def remove_draft_app_version_resource_mappings(
         self,
         *,
         appArn: str,
         appRegistryAppNames: Sequence[str] = ...,
+        eksSourceNames: Sequence[str] = ...,
         logicalStackNames: Sequence[str] = ...,
         resourceGroupNames: Sequence[str] = ...,
         resourceNames: Sequence[str] = ...,
         terraformSourceNames: Sequence[str] = ...
     ) -> RemoveDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Removes resource mappings from a draft application version.
@@ -693,30 +698,30 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app)
         """
     def update_app_version(
         self, *, appArn: str, additionalInfo: Mapping[str, Sequence[str]] = ...
     ) -> UpdateAppVersionResponseTypeDef:
         """
-        Updates the AWS Resilience Hub application version.
+        Updates the Resilience Hub application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version)
         """
     def update_app_version_app_component(
         self,
         *,
         appArn: str,
         id: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         name: str = ...,
         type: str = ...
     ) -> UpdateAppVersionAppComponentResponseTypeDef:
         """
-        Updates an existing Application Component in the AWS Resilience Hub application.
+        Updates an existing Application Component in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_app_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_app_component)
         """
     def update_app_version_resource(
         self,
         *,
@@ -728,15 +733,15 @@
         excluded: bool = ...,
         logicalResourceId: LogicalResourceIdTypeDef = ...,
         physicalResourceId: str = ...,
         resourceName: str = ...,
         resourceType: str = ...
     ) -> UpdateAppVersionResourceResponseTypeDef:
         """
-        Updates the resource details in the AWS Resilience Hub application.
+        Updates the resource details in the Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app_version_resource)
         """
     def update_resiliency_policy(
         self,
         *,
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/literals.py` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
     "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
-    "AppRegistryApp", "CfnStack", "Resource", "ResourceGroup", "Terraform"
+    "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 SopServiceTypeType = Literal["SSM"]
 TemplateFormatType = Literal["CfnJson", "CfnYaml"]
 TestRiskType = Literal["High", "Medium", "Small"]
 TestTypeType = Literal["AZ", "Hardware", "Region", "Software"]
 ResilienceHubServiceName = Literal["resiliencehub"]
@@ -241,14 +241,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/literals.pyi` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
     "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
-    "AppRegistryApp", "CfnStack", "Resource", "ResourceGroup", "Terraform"
+    "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 SopServiceTypeType = Literal["SSM"]
 TemplateFormatType = Literal["CfnJson", "CfnYaml"]
 TestRiskType = Literal["High", "Medium", "Small"]
 TestTypeType = Literal["AZ", "Hardware", "Region", "Software"]
 ResilienceHubServiceName = Literal["resiliencehub"]
@@ -239,14 +239,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/type_defs.py` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 __all__ = (
     "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
+    "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
     "AppTypeDef",
     "AppVersionSummaryTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
@@ -79,14 +80,15 @@
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
@@ -135,29 +137,29 @@
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionResponseTypeDef",
     "ListAppsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "ImportResourcesToDraftAppVersionResponseTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
@@ -274,14 +276,22 @@
 )
 
 
 class AppComponentTypeDef(_RequiredAppComponentTypeDef, _OptionalAppComponentTypeDef):
     pass
 
 
+EksSourceClusterNamespaceTypeDef = TypedDict(
+    "EksSourceClusterNamespaceTypeDef",
+    {
+        "eksClusterArn": str,
+        "namespace": str,
+    },
+)
+
 TerraformSourceTypeDef = TypedDict(
     "TerraformSourceTypeDef",
     {
         "s3StateFileUrl": str,
     },
 )
 
@@ -427,14 +437,15 @@
     {
         "identifier": str,
     },
 )
 _OptionalLogicalResourceIdTypeDef = TypedDict(
     "_OptionalLogicalResourceIdTypeDef",
     {
+        "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
@@ -664,14 +675,22 @@
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 
+EksSourceTypeDef = TypedDict(
+    "EksSourceTypeDef",
+    {
+        "eksClusterArn": str,
+        "namespaces": Sequence[str],
+    },
+)
+
 _RequiredListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlarmRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1059,14 +1078,15 @@
         "appArn": str,
     },
 )
 _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     {
         "appRegistryAppNames": Sequence[str],
+        "eksSourceNames": Sequence[str],
         "logicalStackNames": Sequence[str],
         "resourceGroupNames": Sequence[str],
         "resourceNames": Sequence[str],
         "terraformSourceNames": Sequence[str],
     },
     total=False,
 )
@@ -1526,14 +1546,15 @@
     {
         "importType": ResourceMappingTypeType,
     },
 )
 _OptionalAppInputSourceTypeDef = TypedDict(
     "_OptionalAppInputSourceTypeDef",
     {
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
         "resourceCount": int,
         "sourceArn": str,
         "sourceName": str,
         "terraformSource": TerraformSourceTypeDef,
     },
     total=False,
 )
@@ -1549,64 +1570,29 @@
         "appArn": str,
     },
 )
 _OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
     {
         "clientToken": str,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
         "sourceArn": str,
         "terraformSource": TerraformSourceTypeDef,
     },
     total=False,
 )
 
 
 class DeleteAppInputSourceRequestRequestTypeDef(
     _RequiredDeleteAppInputSourceRequestRequestTypeDef,
     _OptionalDeleteAppInputSourceRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
-
-ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
-    "ImportResourcesToDraftAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "sourceArns": List[str],
-        "status": ResourceImportStatusTypeType,
-        "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1855,14 +1841,52 @@
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
+
+ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
+    "ImportResourcesToDraftAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "eksSources": List[EksSourceTypeDef],
+        "sourceArns": List[str],
+        "status": ResourceImportStatusTypeType,
+        "terraformSources": List[TerraformSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -1890,35 +1914,50 @@
         "physicalResourceId": PhysicalResourceIdTypeDef,
     },
 )
 _OptionalResourceMappingTypeDef = TypedDict(
     "_OptionalResourceMappingTypeDef",
     {
         "appRegistryAppName": str,
+        "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "resourceName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
 
 class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
     pass
 
 
-UnsupportedResourceTypeDef = TypedDict(
-    "UnsupportedResourceTypeDef",
+_RequiredUnsupportedResourceTypeDef = TypedDict(
+    "_RequiredUnsupportedResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
 )
+_OptionalUnsupportedResourceTypeDef = TypedDict(
+    "_OptionalUnsupportedResourceTypeDef",
+    {
+        "unsupportedResourceStatus": str,
+    },
+    total=False,
+)
+
+
+class UnsupportedResourceTypeDef(
+    _RequiredUnsupportedResourceTypeDef, _OptionalUnsupportedResourceTypeDef
+):
+    pass
+
 
 _RequiredRecommendationTemplateTypeDef = TypedDict(
     "_RequiredRecommendationTemplateTypeDef",
     {
         "assessmentArn": str,
         "format": TemplateFormatType,
         "name": str,
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub/type_defs.pyi` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 __all__ = (
     "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
+    "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
     "AppTypeDef",
     "AppVersionSummaryTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
@@ -78,14 +79,15 @@
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
@@ -134,29 +136,29 @@
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionResponseTypeDef",
     "ListAppsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "ImportResourcesToDraftAppVersionResponseTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
@@ -269,14 +271,22 @@
     },
     total=False,
 )
 
 class AppComponentTypeDef(_RequiredAppComponentTypeDef, _OptionalAppComponentTypeDef):
     pass
 
+EksSourceClusterNamespaceTypeDef = TypedDict(
+    "EksSourceClusterNamespaceTypeDef",
+    {
+        "eksClusterArn": str,
+        "namespace": str,
+    },
+)
+
 TerraformSourceTypeDef = TypedDict(
     "TerraformSourceTypeDef",
     {
         "s3StateFileUrl": str,
     },
 )
 
@@ -412,14 +422,15 @@
     {
         "identifier": str,
     },
 )
 _OptionalLogicalResourceIdTypeDef = TypedDict(
     "_OptionalLogicalResourceIdTypeDef",
     {
+        "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
@@ -633,14 +644,22 @@
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 
+EksSourceTypeDef = TypedDict(
+    "EksSourceTypeDef",
+    {
+        "eksClusterArn": str,
+        "namespaces": Sequence[str],
+    },
+)
+
 _RequiredListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlarmRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1002,14 +1021,15 @@
         "appArn": str,
     },
 )
 _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     {
         "appRegistryAppNames": Sequence[str],
+        "eksSourceNames": Sequence[str],
         "logicalStackNames": Sequence[str],
         "resourceGroupNames": Sequence[str],
         "resourceNames": Sequence[str],
         "terraformSourceNames": Sequence[str],
     },
     total=False,
 )
@@ -1451,14 +1471,15 @@
     {
         "importType": ResourceMappingTypeType,
     },
 )
 _OptionalAppInputSourceTypeDef = TypedDict(
     "_OptionalAppInputSourceTypeDef",
     {
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
         "resourceCount": int,
         "sourceArn": str,
         "sourceName": str,
         "terraformSource": TerraformSourceTypeDef,
     },
     total=False,
 )
@@ -1472,60 +1493,27 @@
         "appArn": str,
     },
 )
 _OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
     {
         "clientToken": str,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
         "sourceArn": str,
         "terraformSource": TerraformSourceTypeDef,
     },
     total=False,
 )
 
 class DeleteAppInputSourceRequestRequestTypeDef(
     _RequiredDeleteAppInputSourceRequestRequestTypeDef,
     _OptionalDeleteAppInputSourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
-ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
-    "ImportResourcesToDraftAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "sourceArns": List[str],
-        "status": ResourceImportStatusTypeType,
-        "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1760,14 +1748,50 @@
 
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
+    },
+    total=False,
+)
+
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
+ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
+    "ImportResourcesToDraftAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "eksSources": List[EksSourceTypeDef],
+        "sourceArns": List[str],
+        "status": ResourceImportStatusTypeType,
+        "terraformSources": List[TerraformSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -1793,33 +1817,46 @@
         "physicalResourceId": PhysicalResourceIdTypeDef,
     },
 )
 _OptionalResourceMappingTypeDef = TypedDict(
     "_OptionalResourceMappingTypeDef",
     {
         "appRegistryAppName": str,
+        "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "resourceName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
 class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
     pass
 
-UnsupportedResourceTypeDef = TypedDict(
-    "UnsupportedResourceTypeDef",
+_RequiredUnsupportedResourceTypeDef = TypedDict(
+    "_RequiredUnsupportedResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
 )
+_OptionalUnsupportedResourceTypeDef = TypedDict(
+    "_OptionalUnsupportedResourceTypeDef",
+    {
+        "unsupportedResourceStatus": str,
+    },
+    total=False,
+)
+
+class UnsupportedResourceTypeDef(
+    _RequiredUnsupportedResourceTypeDef, _OptionalUnsupportedResourceTypeDef
+):
+    pass
 
 _RequiredRecommendationTemplateTypeDef = TypedDict(
     "_RequiredRecommendationTemplateTypeDef",
     {
         "assessmentArn": str,
         "format": TemplateFormatType,
         "name": str,
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/PKG-INFO` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.26.76
-Summary: Type annotations for boto3.ResilienceHub 1.26.76 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.97
+Summary: Type annotations for boto3.ResilienceHub 1.26.97 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.26.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,14 +328,15 @@
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
+    EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
@@ -351,14 +352,15 @@
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -407,29 +409,29 @@
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
     DeleteAppInputSourceRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    ImportResourcesToDraftAppVersionResponseTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.26.76/mypy_boto3_resiliencehub.egg-info/SOURCES.txt` & `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.26.76/setup.py` & `mypy-boto3-resiliencehub-1.26.97/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-resiliencehub",
-    version="1.26.76",
+    version="1.26.97",
     packages=["mypy_boto3_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResilienceHub 1.26.76 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.ResilienceHub 1.26.97 service generated with mypy-boto3-builder"
+        " 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

