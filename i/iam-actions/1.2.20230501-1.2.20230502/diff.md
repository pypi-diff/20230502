# Comparing `tmp/iam_actions-1.2.20230501.tar.gz` & `tmp/iam_actions-1.2.20230502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230501.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230502.tar", max compression
```

## Comparing `iam_actions-1.2.20230501.tar` & `iam_actions-1.2.20230502.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/README.md
--rw-r--r--   0        0        0      228 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/__init__.py
--rw-r--r--   0        0        0  4240120 2023-05-01 02:29:21.845849 iam_actions-1.2.20230501/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-01 02:27:17.448544 iam_actions-1.2.20230501/iam_actions/generate/services.py
--rw-r--r--   0        0        0   545330 2023-05-01 02:29:21.845849 iam_actions-1.2.20230501/iam_actions/policies.json
--rw-r--r--   0        0        0   193320 2023-05-01 02:29:21.845849 iam_actions-1.2.20230501/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   528875 2023-05-01 02:29:21.845849 iam_actions-1.2.20230501/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-01 02:29:22.633856 iam_actions-1.2.20230501/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230501/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230501/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/README.md
+-rw-r--r--   0        0        0      228 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4242733 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   545585 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/policies.json
+-rw-r--r--   0        0        0   193567 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   529122 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-02 02:27:52.106933 iam_actions-1.2.20230502/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230502/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230502/PKG-INFO
```

### Comparing `iam_actions-1.2.20230501/LICENSE` & `iam_actions-1.2.20230502/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/README.md` & `iam_actions-1.2.20230502/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/iam_actions/actions.json` & `iam_actions-1.2.20230502/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993094329977981%*

 * *Differences: {"'aoss'": "{'DashboardsAccessAll': {'access_level': 'Write', 'description': 'Grants permission to "*

 * *           "Opensearch Serverless Dashboards', 'resources': ['Dashboards']}, 'APIAccessAll': "*

 * *           "{'access_level': 'Write', 'description': 'Grant permission to all the supported "*

 * *           "Opensearch APIs', 'resources': ['Collection']}}",*

 * * "'athena'": "{'ListTagsForResource': {'resources': {insert: [(0, 'capacity-reservation')]}}, "*

 * *             "'TagResource': {'resources': {insert: [(0, 'capaci […]*

```diff
@@ -2926,20 +2926,22 @@
             "resources": [
                 "ThemeResource"
             ]
         }
     },
     "aoss": {
         "APIAccessAll": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "APIAccessAll",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grant permission to all the supported Opensearch APIs",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Collection"
+            ]
         },
         "BatchGetCollection": {
             "access_level": "Read",
             "action": "BatchGetCollection",
             "condition_keys": [],
             "description": "Grants permission to get attributes for one or more collections",
             "orphan": false,
@@ -2993,20 +2995,22 @@
             "action": "CreateVpcEndpoint",
             "condition_keys": [],
             "description": "Grants permission to create an OpenSearch-Serverless-managed interface VPC endpoint",
             "orphan": false,
             "resources": []
         },
         "DashboardsAccessAll": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DashboardsAccessAll",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to Opensearch Serverless Dashboards",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Dashboards"
+            ]
         },
         "DeleteAccessPolicy": {
             "access_level": "Write",
             "action": "DeleteAccessPolicy",
             "condition_keys": [],
             "description": "Grants permission to delete a data access policy",
             "orphan": false,
@@ -7964,28 +7968,35 @@
             "description": "Grants permission to get information about one or more query executions",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
         "CancelCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelCapacityReservation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to cancel a capacity reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "CreateCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCapacityReservation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a capacity reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "CreateDataCatalog": {
             "access_level": "Write",
             "action": "CreateDataCatalog",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -8136,28 +8147,32 @@
             "description": "Grants permission to get a calculation execution status",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
         "GetCapacityAssignmentConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCapacityAssignmentConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get capacity assignment information for a capacity reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "GetCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCapacityReservation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get a capacity reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "GetDataCatalog": {
             "access_level": "Read",
             "action": "GetDataCatalog",
             "condition_keys": [],
             "description": "Grants permission to get a datacatalog",
             "orphan": false,
@@ -8310,18 +8325,18 @@
             "description": "Grants permission to return a list of calculation executions",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
         "ListCapacityReservations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListCapacityReservations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return a list of capacity reservations for the specified AWS account",
             "orphan": false,
             "resources": []
         },
         "ListDataCatalogs": {
             "access_level": "List",
             "action": "ListDataCatalogs",
             "condition_keys": [],
@@ -8428,33 +8443,37 @@
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to return a list of tags for a resource",
             "orphan": false,
             "resources": [
+                "capacity-reservation",
                 "datacatalog",
                 "workgroup"
             ]
         },
         "ListWorkGroups": {
             "access_level": "List",
             "action": "ListWorkGroups",
             "condition_keys": [],
             "description": "Grants permission to return a list of workgroups for the specified AWS account",
             "orphan": false,
             "resources": []
         },
         "PutCapacityAssignmentConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutCapacityAssignmentConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to assign capacity from a capacity reservation to queries",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation",
+                "workgroup"
+            ]
         },
         "StartCalculationExecution": {
             "access_level": "Write",
             "action": "StartCalculationExecution",
             "condition_keys": [],
             "description": "Grants permission to start a calculation execution",
             "orphan": false,
@@ -8508,14 +8527,15 @@
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to add a tag to a resource",
             "orphan": false,
             "resources": [
+                "capacity-reservation",
                 "datacatalog",
                 "workgroup"
             ]
         },
         "TerminateSession": {
             "access_level": "Write",
             "action": "TerminateSession",
@@ -8531,25 +8551,28 @@
             "action": "UntagResource",
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove a tag from a resource",
             "orphan": false,
             "resources": [
+                "capacity-reservation",
                 "datacatalog",
                 "workgroup"
             ]
         },
         "UpdateCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateCapacityReservation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a capacity reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "UpdateDataCatalog": {
             "access_level": "Write",
             "action": "UpdateDataCatalog",
             "condition_keys": [],
             "description": "Grants permission to update a datacatalog",
             "orphan": false,
@@ -13238,86 +13261,150 @@
             "description": "Grants permission to alter a keyspace or table",
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
+        "AlterMultiRegionResource": {
+            "access_level": "Undocumented",
+            "action": "AlterMultiRegionResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Create": {
             "access_level": "Write",
             "action": "Create",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a keyspace or table",
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
+        "CreateMultiRegionResource": {
+            "access_level": "Undocumented",
+            "action": "CreateMultiRegionResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Drop": {
             "access_level": "Write",
             "action": "Drop",
             "condition_keys": [],
             "description": "Grants permission to drop a keyspace or table",
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
+        "DropMultiRegionResource": {
+            "access_level": "Undocumented",
+            "action": "DropMultiRegionResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Modify": {
             "access_level": "Write",
             "action": "Modify",
             "condition_keys": [],
             "description": "Grants permission to INSERT, UPDATE or DELETE data in a table",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
+        "ModifyMultiRegionResource": {
+            "access_level": "Undocumented",
+            "action": "ModifyMultiRegionResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Restore": {
             "access_level": "Write",
             "action": "Restore",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to restore table from a backup",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
+        "RestoreMultiRegionTable": {
+            "access_level": "Undocumented",
+            "action": "RestoreMultiRegionTable",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Select": {
             "access_level": "Read",
             "action": "Select",
             "condition_keys": [],
             "description": "Grants permission to SELECT data from a table",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
+        "SelectMultiRegionResource": {
+            "access_level": "Undocumented",
+            "action": "SelectMultiRegionResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagMultiRegionResource": {
+            "access_level": "Undocumented",
+            "action": "TagMultiRegionResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to tag a keyspace or table",
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
+        "UnTagMultiRegionResource": {
+            "access_level": "Undocumented",
+            "action": "UnTagMultiRegionResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -57685,20 +57772,22 @@
             "description": "Grants permission to view information about domain and node health, the standby Availability Zone, number of nodes per Availability Zone, and shard count per node",
             "orphan": false,
             "resources": [
                 "domain"
             ]
         },
         "DescribeDomainNodes": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeDomainNodes",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view information about nodes configured for the domain and their configurations- the node id, type of node, status of node, Availability Zone, instance type and storage",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domain"
+            ]
         },
         "DescribeDomains": {
             "access_level": "List",
             "action": "DescribeDomains",
             "condition_keys": [],
             "description": "Grants permission to view a description of the domain configuration for up to five specified OpenSearch Service domains",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230501/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230502/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230502/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/iam_actions/generate/generate.py` & `iam_actions-1.2.20230502/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230502/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230502/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/iam_actions/generate/services.py` & `iam_actions-1.2.20230502/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230501/iam_actions/policies.json` & `iam_actions-1.2.20230502/iam_actions/policies.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999947572611934%*

 * *Differences: {"'serviceMap'": "{'Amazon Keyspaces (for Apache Cassandra)': {'Actions': {insert: [(1, "*

 * *                 "'AlterMultiRegionResource'), (3, 'CreateMultiRegionResource'), (5, "*

 * *                 "'DropMultiRegionResource'), (7, 'ModifyMultiRegionResource'), (9, "*

 * *                 "'RestoreMultiRegionTable'), (11, 'SelectMultiRegionResource'), (12, "*

 * *                 "'TagMultiRegionResource'), (14, 'UnTagMultiRegionResource')]}}}"}*

```diff
@@ -14477,20 +14477,28 @@
             ]
         },
         "Amazon Keyspaces (for Apache Cassandra)": {
             "ARNFormat": "arn:aws:cassandra:${Region}:${Account}:/${ResourceType}/${ResourcePath}/",
             "ARNRegex": "^arn:aws:cassandra:.+",
             "Actions": [
                 "Alter",
+                "AlterMultiRegionResource",
                 "Create",
+                "CreateMultiRegionResource",
                 "Drop",
+                "DropMultiRegionResource",
                 "Modify",
+                "ModifyMultiRegionResource",
                 "Restore",
+                "RestoreMultiRegionTable",
                 "Select",
+                "SelectMultiRegionResource",
+                "TagMultiRegionResource",
                 "TagResource",
+                "UnTagMultiRegionResource",
                 "UntagResource",
                 "UpdatePartitioner"
             ],
             "HasResource": true,
             "StringPrefix": "cassandra",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20230501/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230502/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988328664799252%*

 * *Differences: {"'aoss'": "{'Dashboards': OrderedDict([('arn_pattern', 'arn:*:aoss:*:*:dashboards/default'), "*

 * *           "('condition_keys', None)])}",*

 * * "'athena'": "{'capacity-reservation': OrderedDict([('arn_pattern', "*

 * *             "'arn:*:athena:*:*:capacity-reservation/*'), ('condition_keys', "*

 * *             "'aws:ResourceTag/${TagKey}')])}"}*

```diff
@@ -163,14 +163,18 @@
             "condition_keys": "amplifyuibuilder:ThemeResourceAppId"
         }
     },
     "aoss": {
         "Collection": {
             "arn_pattern": "arn:*:aoss:*:*:collection/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "Dashboards": {
+            "arn_pattern": "arn:*:aoss:*:*:dashboards/default",
+            "condition_keys": null
         }
     },
     "apigateway": {
         "AccessLogSettings": {
             "arn_pattern": "arn:*:apigateway:*::/apis/*/stages/*/accesslogsettings",
             "condition_keys": null
         },
@@ -659,14 +663,18 @@
         },
         "report-package": {
             "arn_pattern": "arn:*:artifact:::report-package/*",
             "condition_keys": null
         }
     },
     "athena": {
+        "capacity-reservation": {
+            "arn_pattern": "arn:*:athena:*:*:capacity-reservation/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "datacatalog": {
             "arn_pattern": "arn:*:athena:*:*:datacatalog/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "workgroup": {
             "arn_pattern": "arn:*:athena:*:*:workgroup/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230501/iam_actions/services.json` & `iam_actions-1.2.20230502/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999450760696436%*

 * *Differences: {"'cassandra'": "{'Actions': {insert: [(1, 'AlterMultiRegionResource'), (3, "*

 * *                "'CreateMultiRegionResource'), (5, 'DropMultiRegionResource'), (7, "*

 * *                "'ModifyMultiRegionResource'), (9, 'RestoreMultiRegionTable'), (11, "*

 * *                "'SelectMultiRegionResource'), (12, 'TagMultiRegionResource'), (14, "*

 * *                "'UnTagMultiRegionResource')]}}"}*

```diff
@@ -2165,20 +2165,28 @@
             "arn:aws:cassandra:${Region}:${Account}:/${ResourceType}/${ResourcePath}/"
         ],
         "ARNRegexes": [
             "^arn:aws:cassandra:.+"
         ],
         "Actions": [
             "Alter",
+            "AlterMultiRegionResource",
             "Create",
+            "CreateMultiRegionResource",
             "Drop",
+            "DropMultiRegionResource",
             "Modify",
+            "ModifyMultiRegionResource",
             "Restore",
+            "RestoreMultiRegionTable",
             "Select",
+            "SelectMultiRegionResource",
+            "TagMultiRegionResource",
             "TagResource",
+            "UnTagMultiRegionResource",
             "UntagResource",
             "UpdatePartitioner"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20230501/pyproject.toml` & `iam_actions-1.2.20230502/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230501"
+version = "1.2.20230502"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230501/setup.py` & `iam_actions-1.2.20230502/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230501',
+    'version': '1.2.20230502',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230501/PKG-INFO` & `iam_actions-1.2.20230502/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230501
+Version: 1.2.20230502
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

