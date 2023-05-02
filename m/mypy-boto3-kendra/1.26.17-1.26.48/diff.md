# Comparing `tmp/mypy-boto3-kendra-1.26.17.tar.gz` & `tmp/mypy-boto3-kendra-1.26.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-1.26.17.tar", last modified: Mon Nov 28 04:09:27 2022, max compression
+gzip compressed data, was "mypy-boto3-kendra-1.26.48.tar", last modified: Wed Jan 11 20:26:39 2023, max compression
```

## Comparing `mypy-boto3-kendra-1.26.17.tar` & `mypy-boto3-kendra-1.26.48.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.540745 mypy-boto3-kendra-1.26.17/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    22539 2022-11-28 04:09:27.540745 mypy-boto3-kendra-1.26.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21106 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.536745 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/
--rw-r--r--   0 runner    (1001) docker     (122)      365 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      364 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      904 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43005 2022-11-28 04:08:56.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    42939 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    14307 2022-11-28 04:08:56.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    14305 2022-11-28 04:08:56.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)   100671 2022-11-28 04:08:58.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)   100526 2022-11-28 04:08:57.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.540745 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    22539 2022-11-28 04:09:27.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      598 2022-11-28 04:09:27.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:27.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:27.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-28 04:09:27.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-28 04:09:27.000000 mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 04:09:27.540745 mypy-boto3-kendra-1.26.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2022-11-28 04:08:55.000000 mypy-boto3-kendra-1.26.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43005 2023-01-11 20:26:28.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42939 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-01-11 20:26:28.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-01-11 20:26:28.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   100671 2023-01-11 20:26:31.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100526 2023-01-11 20:26:29.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/setup.py
```

### Comparing `mypy-boto3-kendra-1.26.17/LICENSE` & `mypy-boto3-kendra-1.26.48/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.26.17/PKG-INFO` & `mypy-boto3-kendra-1.26.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.26.17
-Summary: Type annotations for boto3.kendra 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.48
+Summary: Type annotations for boto3.kendra 1.26.48 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.26.48](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kendra-1.26.17/README.md` & `mypy-boto3-kendra-1.26.48/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.26.48](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/__main__.py` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.kendra 1.26.17\nVersion:         1.26.17\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.kendra 1.26.48\nVersion:         1.26.48\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.17")
+    print("1.26.48")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/client.py` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/client.pyi` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/literals.py` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,28 @@
     "SPACE_KEY",
     "SPACE_NAME",
     "URL",
     "VERSION",
 ]
 ConfluenceSpaceFieldNameType = Literal["DISPLAY_URL", "ITEM_TYPE", "SPACE_KEY", "URL"]
 ConfluenceVersionType = Literal["CLOUD", "SERVER"]
-ContentTypeType = Literal["HTML", "MS_WORD", "PDF", "PLAIN_TEXT", "PPT"]
+ContentTypeType = Literal[
+    "CSV",
+    "HTML",
+    "JSON",
+    "MD",
+    "MS_EXCEL",
+    "MS_WORD",
+    "PDF",
+    "PLAIN_TEXT",
+    "PPT",
+    "RTF",
+    "XML",
+    "XSLT",
+]
 DataSourceStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 DataSourceSyncJobStatusType = Literal[
     "ABORTED", "FAILED", "INCOMPLETE", "STOPPING", "SUCCEEDED", "SYNCING", "SYNCING_INDEXING"
 ]
 DataSourceTypeType = Literal[
     "ALFRESCO",
     "BOX",
@@ -272,14 +285,15 @@
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
@@ -303,14 +317,15 @@
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
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
@@ -339,14 +354,15 @@
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
@@ -413,30 +429,33 @@
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
@@ -469,28 +488,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -518,30 +540,34 @@
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
@@ -587,14 +613,15 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
+    "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-west-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
```

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/literals.pyi` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,28 @@
     "SPACE_KEY",
     "SPACE_NAME",
     "URL",
     "VERSION",
 ]
 ConfluenceSpaceFieldNameType = Literal["DISPLAY_URL", "ITEM_TYPE", "SPACE_KEY", "URL"]
 ConfluenceVersionType = Literal["CLOUD", "SERVER"]
-ContentTypeType = Literal["HTML", "MS_WORD", "PDF", "PLAIN_TEXT", "PPT"]
+ContentTypeType = Literal[
+    "CSV",
+    "HTML",
+    "JSON",
+    "MD",
+    "MS_EXCEL",
+    "MS_WORD",
+    "PDF",
+    "PLAIN_TEXT",
+    "PPT",
+    "RTF",
+    "XML",
+    "XSLT",
+]
 DataSourceStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
 DataSourceSyncJobStatusType = Literal[
     "ABORTED", "FAILED", "INCOMPLETE", "STOPPING", "SUCCEEDED", "SYNCING", "SYNCING_INDEXING"
 ]
 DataSourceTypeType = Literal[
     "ALFRESCO",
     "BOX",
@@ -270,14 +283,15 @@
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
@@ -301,14 +315,15 @@
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
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
@@ -337,14 +352,15 @@
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
@@ -411,30 +427,33 @@
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
@@ -467,28 +486,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -516,30 +538,34 @@
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
@@ -585,14 +611,15 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
+    "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-west-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
```

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/type_defs.py` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra/type_defs.pyi` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/PKG-INFO` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.26.17
-Summary: Type annotations for boto3.kendra 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.48
+Summary: Type annotations for boto3.kendra 1.26.48 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.26.48](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kendra-1.26.17/mypy_boto3_kendra.egg-info/SOURCES.txt` & `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.26.17/setup.py` & `mypy-boto3-kendra-1.26.48/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-kendra",
-    version="1.26.17",
+    version="1.26.48",
     packages=["mypy_boto3_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.kendra 1.26.17 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.kendra 1.26.48 service generated with mypy-boto3-builder 7.12.3"
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
     keywords="boto3 kendra type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_kendra": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_kendra": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

