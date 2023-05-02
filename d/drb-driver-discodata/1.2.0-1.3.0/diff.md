# Comparing `tmp/drb-driver-discodata-1.2.0.tar.gz` & `tmp/drb-driver-discodata-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-discodata-1.2.0.tar", last modified: Thu Mar 30 09:32:05 2023, max compression
+gzip compressed data, was "drb-driver-discodata-1.3.0.tar", last modified: Tue May  2 11:19:27 2023, max compression
```

## Comparing `drb-driver-discodata-1.2.0.tar` & `drb-driver-discodata-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:32:05.682399 drb-driver-discodata-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 14:58:58.000000 drb-driver-discodata-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-01-10 08:48:04.000000 drb-driver-discodata-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5535 2023-03-30 09:32:05.682399 drb-driver-discodata-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4884 2023-03-08 16:04:20.000000 drb-driver-discodata-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:32:05.650399 drb-driver-discodata-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:32:05.650399 drb-driver-discodata-1.2.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:32:05.686399 drb-driver-discodata-1.2.0/drb/drivers/discodata/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-01-10 10:54:03.000000 drb-driver-discodata-1.2.0/drb/drivers/discodata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-30 09:32:05.686399 drb-driver-discodata-1.2.0/drb/drivers/discodata/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    15287 2023-03-08 16:04:20.000000 drb-driver-discodata-1.2.0/drb/drivers/discodata/discodata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:32:05.650399 drb-driver-discodata-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:32:05.682399 drb-driver-discodata-1.2.0/drb/topics/discodata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 08:48:04.000000 drb-driver-discodata-1.2.0/drb/topics/discodata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-01-10 08:48:04.000000 drb-driver-discodata-1.2.0/drb/topics/discodata/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:32:05.682399 drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5535 2023-03-30 09:32:05.000000 drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-03-30 09:32:05.000000 drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 09:32:05.000000 drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-30 09:32:05.000000 drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-03-30 09:32:05.000000 drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-30 09:32:05.000000 drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-03-08 16:04:20.000000 drb-driver-discodata-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-03-30 09:32:05.686399 drb-driver-discodata-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1378 2023-03-08 16:46:56.000000 drb-driver-discodata-1.2.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2023-01-10 08:48:05.000000 drb-driver-discodata-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.783897 drb-driver-discodata-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 14:58:58.000000 drb-driver-discodata-1.3.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-01-10 08:48:04.000000 drb-driver-discodata-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5419 2023-05-02 11:19:27.783897 drb-driver-discodata-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4858 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.763897 drb-driver-discodata-1.3.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.763897 drb-driver-discodata-1.3.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.783897 drb-driver-discodata-1.3.0/drb/drivers/discodata/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-01-10 10:54:03.000000 drb-driver-discodata-1.3.0/drb/drivers/discodata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-02 11:19:27.783897 drb-driver-discodata-1.3.0/drb/drivers/discodata/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    13199 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/drb/drivers/discodata/discodata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.763897 drb-driver-discodata-1.3.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.775897 drb-driver-discodata-1.3.0/drb/topics/discodata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 08:48:04.000000 drb-driver-discodata-1.3.0/drb/topics/discodata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-02 11:18:24.000000 drb-driver-discodata-1.3.0/drb/topics/discodata/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.779897 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5419 2023-05-02 11:19:27.000000 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      655 2023-05-02 11:19:27.000000 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:19:27.000000 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 11:19:27.000000 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:19:27.000000 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-02 11:19:27.000000 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-02 11:19:27.000000 drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-05-02 11:19:27.783897 drb-driver-discodata-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:19:27.779897 drb-driver-discodata-1.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9072 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/tests/test_discodata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/tests/test_discodata_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1643 2023-04-18 12:11:42.000000 drb-driver-discodata-1.3.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2023-01-10 08:48:05.000000 drb-driver-discodata-1.3.0/versioneer.py
```

### Comparing `drb-driver-discodata-1.2.0/LICENCE.txt` & `drb-driver-discodata-1.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-discodata-1.2.0/PKG-INFO` & `drb-driver-discodata-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: drb-driver-discodata
-Version: 1.2.0
-Summary: DRB DISCODATA Driver
-Home-page: https://gitlab.com/drb-python/impl/discodata
-Author: GAEL Systems
-Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/discodata
-Project-URL: Source, https://gitlab.com/drb-python/impl/discodata
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
 # DISCODATA driver
 
 This drb-driver-discodata module implements DISCODATA databases access with DRB data model. It is able to navigates among the database contents.
 
 For more information about DISCODATA see: https://discodata.eea.europa.eu/Help.html
 
 ## DISOCDATA Factory and DISCODATA Node
@@ -70,15 +52,15 @@
 
 This example shows how to create a `DrbDiscodataServiceNode` then look for the first 3 databases using the attribute of the service:
 
 ```python
 from drb.drivers.discodata import DrbDiscodataServiceNode
 
 service = DrbDiscodataServiceNode(path="https://discodata.eea.europa.eu")
-databases = service.get_attribute("databases")
+databases = service @ "databases"
 for database in databases[:3]:
     print(database)
 ```
 
 Output :
 
 ```
@@ -87,15 +69,15 @@
 CataloguePolicyEvaluations
 ```
 
 Then we can get the list of tables from a specific database:
 
 ```
 database = service["AirQualityDataFlows"]
-tables = database.get_attribute("tables")
+tables = database @ "tables"
 for table in tables:
     print(table)
 ```
 
 Output :
 
 ```
@@ -132,9 +114,7 @@
 2496  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 2497  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 2498  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 2499  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 
 [2500 rows x 39 columns]
 ```
-
-
```

### Comparing `drb-driver-discodata-1.2.0/README.md` & `drb-driver-discodata-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: drb-driver-discodata
+Version: 1.3.0
+Summary: DRB DISCODATA Driver
+Author: GAEL Systems
+Author-email: drb-python@gael.fr
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/discodata
+Project-URL: Source, https://gitlab.com/drb-python/impl/discodata
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 # DISCODATA driver
 
 This drb-driver-discodata module implements DISCODATA databases access with DRB data model. It is able to navigates among the database contents.
 
 For more information about DISCODATA see: https://discodata.eea.europa.eu/Help.html
 
 ## DISOCDATA Factory and DISCODATA Node
@@ -52,15 +68,15 @@
 
 This example shows how to create a `DrbDiscodataServiceNode` then look for the first 3 databases using the attribute of the service:
 
 ```python
 from drb.drivers.discodata import DrbDiscodataServiceNode
 
 service = DrbDiscodataServiceNode(path="https://discodata.eea.europa.eu")
-databases = service.get_attribute("databases")
+databases = service @ "databases"
 for database in databases[:3]:
     print(database)
 ```
 
 Output :
 
 ```
@@ -69,15 +85,15 @@
 CataloguePolicyEvaluations
 ```
 
 Then we can get the list of tables from a specific database:
 
 ```
 database = service["AirQualityDataFlows"]
-tables = database.get_attribute("tables")
+tables = database @ "tables"
 for table in tables:
     print(table)
 ```
 
 Output :
 
 ```
```

### Comparing `drb-driver-discodata-1.2.0/drb/drivers/discodata/discodata.py` & `drb-driver-discodata-1.3.0/drb/drivers/discodata/discodata.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 from typing import Any, Dict, List, Optional, Tuple, Union
 from urllib.request import pathname2url
 
+from deprecated.classic import deprecated
 from drb.core import DrbFactory, DrbNode, ParsedPath
 from drb.drivers.http import DrbHttpNode
 from drb.drivers.json import JsonBaseNode
 from drb.exceptions.core import (
     DrbException,
     DrbFactoryException,
     DrbNotImplementationException,
@@ -155,82 +156,45 @@
     in this table.
     Its children is a list of DrbDiscodataRowList that can be browsed
     only by its index or slice in the table.
 
     Parameters:
         parent(DrbNode): The parent of the node.
     """
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    def close(self) -> None:
-        pass
-
     def __init__(self, parent: DrbNode, table_node: DrbNode):
         super().__init__()
 
         self._table_node = table_node
 
-        self._name = table_node["name"].value
-        self._parent: DrbNode = parent
+        self.name = table_node["name"].value
+        self.parent: DrbNode = parent
         self._id = table_node["id"].value
-        self._attributes = {}
         self._table_node = table_node
         self._children: List[DrbNode] = None
-        self._path = None
         self._df_impl = None
+        self._available_impl = [pd.DataFrame, xr.Dataset]
+        self.__init_attributes()
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def path(self) -> ParsedPath:
-        return self._parent.path / self._name
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if not self._attributes:
-            for col in self._table_node["Columns", :]:
-                dict_col = {}
-                for child_col in col:
-                    dict_col[child_col.name] = child_col.value
-                self._attributes[col["name"].value, None] = dict_col
-            columns = [c["name"].value for c in self._table_node["Columns", :]]
-            self._attributes[("columns", None)] = columns
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if namespace_uri is None and (name, None) in self.attributes.keys():
-            return self.attributes[(name, None)]
-        raise DrbException(
-            f"Attribute not found name: {name}, " f"namespace: {namespace_uri}"
-        )
+    def __init_attributes(self):
+        for col in self._table_node["Columns", :]:
+            dict_col = {}
+            for child_col in col:
+                dict_col[child_col.name] = child_col.value
+            self @= (col["name"].value, dict_col)
+        columns = [c["name"].value for c in self._table_node["Columns", :]]
+        self @= ("columns", columns)
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = DrbDiscodataRowList(self)
         return self._children
 
-    def has_impl(self, impl: type) -> bool:
-        if impl in [pd.DataFrame, xr.Dataset]:
-            return True
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         if not self.has_impl(impl):
             raise DrbNotImplementationException(
                 f"no {impl} " f"implementation found"
             )
         if self._df_impl is None:
             recs = []
@@ -243,15 +207,15 @@
             return self._df_impl.to_xarray()
 
     def get_id(self):
         return self._id
 
     def get_elts(self, page_number):
         parent = self.parent
-        table_name = self._name
+        table_name = self.name
         database_name_version = None
         while parent is not None and not isinstance(
             parent, DrbDiscodataServiceNode
         ):
             if isinstance(parent, DrbDiscodataDataBaseNode):
                 database_name_version = parent.get_database_name_version()
             parent = parent.parent
@@ -261,199 +225,148 @@
         ):
             return parent.get_elts(
                 table_name, database_name_version, page_number
             )
 
         return None
 
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
+
 
 class DrbDiscodataDataBaseNode(AbstractNode):
     """
     The DrbDiscodataDataBaseNode is used to represent a database of discodata
 
     Its attribute "tables" contain the list of the data available
     in this database.
     Its children is a list of DrbDiscodataTableNode that can be browsed
     by table name.
     Parameters:
         parent(DrbNode): The parent of the node.
     """
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    def close(self) -> None:
-        pass
-
     def __init__(self, parent: DrbNode, database_node: DrbNode):
         super().__init__()
 
         self._database_node = database_node
         self._version = ""
-        self._name = database_node["database"].value
-        self._parent: DrbNode = parent
-        self._attributes = {}
+        self.name = database_node["database"].value
+        self.parent: DrbNode = parent
         self._children: List[DrbNode] = None
-        self._path = None
         node_schemas = self._database_node["Schemas", :]
         latest = [n for n in node_schemas if n["schema"].value == "latest"]
         # there should be only one 'latest' version
         if len(latest) == 1:
             self._latest_node = latest[0]
             self._latest_node = self._database_node["Schemas", -1]
         # if not, we take the last one, hoping they'll stay sorted
         else:
             self._latest_node = self._database_node["Schemas", -1]
         self._version = self._latest_node["schema"].value
+        self._available_impl.clear()
+        self.__init_attributes()
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def path(self) -> ParsedPath:
-        return self._parent.path / self._name
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if not self._attributes:
+    def __init_attributes(self):
+        if self._latest_node.has_child("Tables"):
             tables = [t["name"].value for t in self._latest_node["Tables", :]]
-            self._attributes[("tables", None)] = tables
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if namespace_uri is None and (name, None) in self.attributes.keys():
-            return self.attributes[(name, None)]
-        raise DrbException(
-            f"Attribute not found name: {name}, " f"namespace: {namespace_uri}"
-        )
+            self @= ("tables", tables)
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the bracket is recommended')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
             if self._database_node.has_child("Schemas"):
                 try:
                     tables = self._latest_node["Tables", :]
                     for child_node in tables:
                         self._children.append(
                             DrbDiscodataTableNode(self, child_node)
                         )
                 except Exception:
                     pass
         return self._children
 
-    def has_impl(self, impl: type) -> bool:
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         raise DrbNotImplementationException(
             f"no {impl} " f"implementation found"
         )
 
     def get_database_name_version(self):
-        return f"[{self._name}].[{self._version}]"
+        return f"[{self.name}].[{self._version}]"
+
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
 
 
 class DrbDiscodataServiceNode(AbstractNode):
     """
     Represent a node for browsing Discodata data.
 
     Its attribute "databases" contain the list of all the available
     databases in the discodata service.
     Its children is a list of DrbDiscodataDataBaseNode
     This node has no implementations.
     """
-
     def __init__(
         self,
         path="https://discodata.eea.europa.eu",
         auth: Union[AuthBase, str] = None,
     ):
         super().__init__()
         path = path.replace("+discodata", "") if "+discodata" in path else path
 
         self._children = None
-        self._attributes = {}
+        # self._attributes = {}
+        self.name = "DISCODATA"
         if path.endswith("/"):
             path = path[:-1]
         self._path = path
         self._auth = auth
         self._path_map = path.replace("discodata", "discomap")
         md_node = DrbHttpNode(self._path + "/md")
         self._metadata = create(md_node)
+        self._available_impl.clear()
+        self.__init_attributes()
 
-    @property
-    def name(self) -> str:
-        return "DISCODATA"
+    def __init_attributes(self):
+        if self._metadata.has_child("md"):
+            databases = [
+                c.value["database"] for c in self._metadata["md"].children
+            ]
 
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if not self._attributes:
-            databases = []
-            if self._metadata.has_child("md"):
-                databases = [
-                    c.value["database"] for c in self._metadata["md"].children
-                ]
-                self._attributes[("databases", None)] = databases
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if namespace_uri is None and (name, None) in self.attributes.keys():
-            return self.attributes[(name, None)]
-        raise DrbException(f"Attribute not found: ({name}, {namespace_uri})")
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return None
+            self @= ("databases", databases)
 
     @property
     def path(self) -> ParsedPath:
         return ParsedPath(self._path)
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
-            # node = DrbHttpNode(self._path + "/md")
-            # json_node = create(node)
 
-            if self._metadata.has_child("md"):
-                for database in self._metadata["md"].children:
-                    dt_child = DrbDiscodataDataBaseNode(self, database)
-                    self._children.append(dt_child)
+            for database in self._metadata["md"]:
+                dt_child = DrbDiscodataDataBaseNode(self, database)
+                self._children.append(dt_child)
 
         return self._children
 
-    def has_impl(self, impl: type) -> bool:
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         raise DrbException(f"Do not support implementation: {impl}")
 
-    def close(self) -> None:
-        pass
-
     def get_elts(self, table_name, database_name_version, page_number):
         json = {
             "Page": page_number,
             "SortBy": "",
             "SortAscending": True,
             "RequestFilter": {},
         }
@@ -462,14 +375,20 @@
             self._path_map + f"/App/DiscodataViewer/data?fqn="
             f"{database_name_version}.[{table_name}]",
             data=json,
         )
 
         return JsonBaseNode(node_ret, node_ret.get_impl(io.BufferedIOBase))
 
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
+
 
 class DiscodataFactory(DrbFactory):
     def _create(self, node: DrbNode) -> DrbNode:
         if isinstance(node, DrbDiscodataServiceNode):
             return node
         if isinstance(node, DrbHttpNode):
             node_discodata_service = DrbDiscodataServiceNode(
```

### Comparing `drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/PKG-INFO` & `drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: drb-driver-discodata
-Version: 1.2.0
+Version: 1.3.0
 Summary: DRB DISCODATA Driver
-Home-page: https://gitlab.com/drb-python/impl/discodata
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/discodata
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/discodata
 Project-URL: Source, https://gitlab.com/drb-python/impl/discodata
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # DISCODATA driver
 
 This drb-driver-discodata module implements DISCODATA databases access with DRB data model. It is able to navigates among the database contents.
@@ -70,15 +68,15 @@
 
 This example shows how to create a `DrbDiscodataServiceNode` then look for the first 3 databases using the attribute of the service:
 
 ```python
 from drb.drivers.discodata import DrbDiscodataServiceNode
 
 service = DrbDiscodataServiceNode(path="https://discodata.eea.europa.eu")
-databases = service.get_attribute("databases")
+databases = service @ "databases"
 for database in databases[:3]:
     print(database)
 ```
 
 Output :
 
 ```
@@ -87,15 +85,15 @@
 CataloguePolicyEvaluations
 ```
 
 Then we can get the list of tables from a specific database:
 
 ```
 database = service["AirQualityDataFlows"]
-tables = database.get_attribute("tables")
+tables = database @ "tables"
 for table in tables:
     print(table)
 ```
 
 Output :
 
 ```
@@ -132,9 +130,7 @@
 2496  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 2497  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 2498  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 2499  Slovenia  SI             SI.ARSO.AQ  ...  Vojkova 1b, LJUBLJANA, 1000  http://cdr.eionet.europa.eu/si/eu/aqd/e1b/envy...  2021-11-20T19:08:05.693
 
 [2500 rows x 39 columns]
 ```
-
-
```

### Comparing `drb-driver-discodata-1.2.0/drb_driver_discodata.egg-info/SOURCES.txt` & `drb-driver-discodata-1.3.0/drb_driver_discodata.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 LICENCE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 drb/drivers/discodata/__init__.py
 drb/drivers/discodata/_version.py
 drb/drivers/discodata/discodata.py
 drb/topics/discodata/__init__.py
 drb/topics/discodata/cortex.yml
 drb_driver_discodata.egg-info/PKG-INFO
 drb_driver_discodata.egg-info/SOURCES.txt
 drb_driver_discodata.egg-info/dependency_links.txt
 drb_driver_discodata.egg-info/entry_points.txt
+drb_driver_discodata.egg-info/not-zip-safe
 drb_driver_discodata.egg-info/requires.txt
-drb_driver_discodata.egg-info/top_level.txt
+drb_driver_discodata.egg-info/top_level.txt
+tests/test_discodata.py
+tests/test_discodata_factory.py
+tests/test_signature.py
```

### Comparing `drb-driver-discodata-1.2.0/versioneer.py` & `drb-driver-discodata-1.3.0/versioneer.py`

 * *Files identical despite different names*

