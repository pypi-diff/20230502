# Comparing `tmp/xata-0.9.2.tar.gz` & `tmp/xata-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-0.9.2.tar", max compression
+gzip compressed data, was "xata-0.9.3.tar", max compression
```

## Comparing `xata-0.9.2.tar` & `xata-0.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-04-27 12:37:44.650242 xata-0.9.2/LICENSE
--rw-r--r--   0        0        0     1156 2023-04-27 12:37:44.650242 xata-0.9.2/README.md
--rw-r--r--   0        0        0      749 2023-04-27 12:37:44.678241 xata-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      858 2023-04-27 12:37:44.678241 xata-0.9.2/xata/__init__.py
--rw-r--r--   0        0        0    31960 2023-04-27 12:37:44.678241 xata-0.9.2/xata/client.py
--rw-r--r--   0        0        0     1715 2023-04-27 12:37:44.678241 xata-0.9.2/xata/errors.py
--rw-r--r--   0        0        0    11090 2023-04-27 12:37:44.678241 xata-0.9.2/xata/helpers.py
--rw-r--r--   0        0        0     2114 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespace.py
--rw-r--r--   0        0        0      769 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/__init__.py
--rw-r--r--   0        0        0      769 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/__init__.py
--rw-r--r--   0        0        0     2666 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/authentication.py
--rw-r--r--   0        0        0     6182 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/databases.py
--rw-r--r--   0        0        0     6204 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/invites.py
--rw-r--r--   0        0        0     2554 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/users.py
--rw-r--r--   0        0        0     7419 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/core/workspaces.py
--rw-r--r--   0        0        0      769 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/__init__.py
--rw-r--r--   0        0        0    12315 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/branch.py
--rw-r--r--   0        0        0    11721 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/migrations.py
--rw-r--r--   0        0        0    12491 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/records.py
--rw-r--r--   0        0        0    30137 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/search_and_filter.py
--rw-r--r--   0        0        0    12792 2023-04-27 12:37:44.678241 xata-0.9.2/xata/namespaces/workspace/table.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 12:49:08.009065 xata-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1156 2023-04-27 12:49:08.009065 xata-0.9.3/README.md
+-rw-r--r--   0        0        0      749 2023-04-27 12:49:08.033046 xata-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      858 2023-04-27 12:49:08.037043 xata-0.9.3/xata/__init__.py
+-rw-r--r--   0        0        0    31963 2023-04-27 12:49:08.037043 xata-0.9.3/xata/client.py
+-rw-r--r--   0        0        0     1715 2023-04-27 12:49:08.037043 xata-0.9.3/xata/errors.py
+-rw-r--r--   0        0        0    11090 2023-04-27 12:49:08.037043 xata-0.9.3/xata/helpers.py
+-rw-r--r--   0        0        0     2114 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespace.py
+-rw-r--r--   0        0        0      769 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/__init__.py
+-rw-r--r--   0        0        0     2666 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/authentication.py
+-rw-r--r--   0        0        0     6182 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/databases.py
+-rw-r--r--   0        0        0     6204 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/invites.py
+-rw-r--r--   0        0        0     2554 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/users.py
+-rw-r--r--   0        0        0     7419 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/core/workspaces.py
+-rw-r--r--   0        0        0      769 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/__init__.py
+-rw-r--r--   0        0        0    12315 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/branch.py
+-rw-r--r--   0        0        0    11721 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/migrations.py
+-rw-r--r--   0        0        0    12491 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/records.py
+-rw-r--r--   0        0        0    30137 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/search_and_filter.py
+-rw-r--r--   0        0        0    12792 2023-04-27 12:49:08.037043 xata-0.9.3/xata/namespaces/workspace/table.py
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.3/PKG-INFO
```

### Comparing `xata-0.9.2/LICENSE` & `xata-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/README.md` & `xata-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/pyproject.toml` & `xata-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "0.9.2"
+version = "0.9.3"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
```

### Comparing `xata-0.9.2/xata/__init__.py` & `xata-0.9.3/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/client.py` & `xata-0.9.3/xata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .namespaces.workspace.migrations import Migrations
 from .namespaces.workspace.records import Records
 from .namespaces.workspace.search_and_filter import Search_and_filter
 from .namespaces.workspace.table import Table
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
@@ -229,15 +229,15 @@
                 envVals.get("XATA_WORKSPACE_ID"),
                 envVals.get("XATA_REGION", DEFAULT_REGION),
                 "dotenv",
             )
 
         self.ensure_config_read()
         if self.config is not None and self.config.get("databaseURL"):
-            workspaceID, region, _, _ = self._parse_database_url(self.config.get("databaseURL"))
+            workspaceID, region, _, _, _ = self._parse_database_url(self.config.get("databaseURL"))
             return workspaceID, region, "config"
         raise Exception(
             f"No workspace ID found. Searched in `XATA_WORKSPACE_ID` env, "
             f"`{PERSONAL_API_KEY_LOCATION}`, and `{os.path.abspath('.env')}`"
         )
 
     def get_database_name_if_configured(self) -> str:
```

### Comparing `xata-0.9.2/xata/errors.py` & `xata-0.9.3/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/helpers.py` & `xata-0.9.3/xata/helpers.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespace.py` & `xata-0.9.3/xata/namespace.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/__init__.py` & `xata-0.9.3/xata/namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/core/__init__.py` & `xata-0.9.3/xata/namespaces/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/core/authentication.py` & `xata-0.9.3/xata/namespaces/core/authentication.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/core/databases.py` & `xata-0.9.3/xata/namespaces/core/databases.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/core/invites.py` & `xata-0.9.3/xata/namespaces/core/invites.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/core/users.py` & `xata-0.9.3/xata/namespaces/core/users.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/core/workspaces.py` & `xata-0.9.3/xata/namespaces/core/workspaces.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/workspace/__init__.py` & `xata-0.9.3/xata/namespaces/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/workspace/branch.py` & `xata-0.9.3/xata/namespaces/workspace/branch.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/workspace/migrations.py` & `xata-0.9.3/xata/namespaces/workspace/migrations.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/workspace/records.py` & `xata-0.9.3/xata/namespaces/workspace/records.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/workspace/search_and_filter.py` & `xata-0.9.3/xata/namespaces/workspace/search_and_filter.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/xata/namespaces/workspace/table.py` & `xata-0.9.3/xata/namespaces/workspace/table.py`

 * *Files identical despite different names*

### Comparing `xata-0.9.2/PKG-INFO` & `xata-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

