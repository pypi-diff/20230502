# Comparing `tmp/drb-driver-zarr-1.1.0.tar.gz` & `tmp/drb-driver-zarr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-zarr-1.1.0.tar", last modified: Mon Dec 19 16:00:23 2022, max compression
+gzip compressed data, was "drb-driver-zarr-1.2.0.tar", last modified: Tue May  2 13:16:24 2023, max compression
```

## Comparing `drb-driver-zarr-1.1.0.tar` & `drb-driver-zarr-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.666434 drb-driver-zarr-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1802 2022-12-19 16:00:23.666434 drb-driver-zarr-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1224 2022-12-19 15:13:58.000000 drb-driver-zarr-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.654434 drb-driver-zarr-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.654434 drb-driver-zarr-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.670434 drb-driver-zarr-1.1.0/drb/drivers/zarr/
--rw-rw-rw-   0 root         (0) root         (0)      336 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/drb/drivers/zarr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-19 16:00:23.670434 drb-driver-zarr-1.1.0/drb/drivers/zarr/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6836 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/drb/drivers/zarr/zarr_data_set_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2581 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/drb/drivers/zarr/zarr_node_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.666434 drb-driver-zarr-1.1.0/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       98 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/drb/exceptions/zarr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.654434 drb-driver-zarr-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.666434 drb-driver-zarr-1.1.0/drb/topics/zarr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/drb/topics/zarr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/drb/topics/zarr/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:00:23.666434 drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1802 2022-12-19 16:00:23.000000 drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      520 2022-12-19 16:00:23.000000 drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 16:00:23.000000 drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2022-12-19 16:00:23.000000 drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      101 2022-12-19 16:00:23.000000 drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-19 16:00:23.000000 drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 14:48:21.000000 drb-driver-zarr-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 16:00:23.670434 drb-driver-zarr-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1282 2022-12-19 15:13:58.000000 drb-driver-zarr-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2022-09-28 15:53:28.000000 drb-driver-zarr-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.110252 drb-driver-zarr-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:41:47.000000 drb-driver-zarr-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-19 14:48:21.000000 drb-driver-zarr-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-05-02 13:16:24.110252 drb-driver-zarr-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2022-12-19 15:13:58.000000 drb-driver-zarr-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.090252 drb-driver-zarr-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.090252 drb-driver-zarr-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.114252 drb-driver-zarr-1.2.0/drb/drivers/zarr/
+-rw-rw-rw-   0 root         (0) root         (0)      336 2022-12-19 14:48:21.000000 drb-driver-zarr-1.2.0/drb/drivers/zarr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-02 13:16:24.114252 drb-driver-zarr-1.2.0/drb/drivers/zarr/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5307 2023-04-20 10:02:24.000000 drb-driver-zarr-1.2.0/drb/drivers/zarr/zarr_data_set_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2023-05-02 12:56:31.000000 drb-driver-zarr-1.2.0/drb/drivers/zarr/zarr_node_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.102252 drb-driver-zarr-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2022-12-19 14:48:21.000000 drb-driver-zarr-1.2.0/drb/exceptions/zarr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.090252 drb-driver-zarr-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.102252 drb-driver-zarr-1.2.0/drb/topics/zarr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 14:48:21.000000 drb-driver-zarr-1.2.0/drb/topics/zarr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-02 13:15:21.000000 drb-driver-zarr-1.2.0/drb/topics/zarr/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.106252 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-05-02 13:16:24.000000 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-05-02 13:16:24.000000 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 13:16:24.000000 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-02 13:16:24.000000 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 13:16:23.000000 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-02 13:16:24.000000 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-02 13:16:24.000000 drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-20 13:01:41.000000 drb-driver-zarr-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-20 10:02:24.000000 drb-driver-zarr-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-02 13:16:24.114252 drb-driver-zarr-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-20 10:02:24.000000 drb-driver-zarr-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 13:16:24.110252 drb-driver-zarr-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2832 2022-12-19 14:48:21.000000 drb-driver-zarr-1.2.0/tests/test_drb_zarr_array.py
+-rw-rw-rw-   0 root         (0) root         (0)     5762 2022-12-19 14:48:21.000000 drb-driver-zarr-1.2.0/tests/test_drb_zarr_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3460 2023-04-20 10:02:24.000000 drb-driver-zarr-1.2.0/tests/test_drb_zarr_node_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2023-04-20 10:02:24.000000 drb-driver-zarr-1.2.0/tests/test_drb_zarr_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2022-09-28 15:53:28.000000 drb-driver-zarr-1.2.0/versioneer.py
```

### Comparing `drb-driver-zarr-1.1.0/PKG-INFO` & `drb-driver-zarr-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-zarr
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB Zarr driver
-Home-page: https://gitlab.com/drb-python/impl/zarr
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/zarr
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/zarr
 Project-URL: Source, https://gitlab.com/drb-python/impl/zarr
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # ZarrNode Driver
 
 This drb-driver-zarr module implements access to zarr containers with DRB data model. It is able to navigates among the zarr contents.
 
 ## Zar Factory and Zarr Node
 
@@ -38,9 +37,7 @@
 ## Using this module
 
 To include this module into your project, the `drb-driver-zarr` module shall be referenced into `requirements.txt` file, or the following pip line can be run:
 
 ```commandline
 pip install drb-driver-zarr
 ```
-
-
```

### Comparing `drb-driver-zarr-1.1.0/README.md` & `drb-driver-zarr-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-zarr-1.1.0/drb/drivers/zarr/zarr_data_set_node.py` & `drb-driver-zarr-1.2.0/drb/drivers/zarr/zarr_data_set_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import enum
 from abc import ABC
 from typing import Any, List, Optional, Union, Dict, Tuple
 
 import drb.topics.resolver as resolver
 import zarr
+from deprecated.classic import deprecated
 
 from drb.core import DrbNode
 from drb.nodes.abstract_node import AbstractNode
 from drb.exceptions.core import DrbNotImplementationException, DrbException
 from drb.core.path import ParsedPath
 
 
@@ -37,100 +38,27 @@
         parent: DrbNode,
         name: str,
         data_set: Union[zarr.hierarchy.Group, zarr.core.Array],
     ):
         super().__init__()
 
         self._data_set = data_set
-        self._parent: DrbNode = parent
-        self._name = name
-        self._path = None
+        self.parent: DrbNode = parent
+        self.name = name
         self._attributes: Dict[Tuple[str, str], Any] = None
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        """
-        Not use in this implementation
-
-        Return:
-            None
-        """
-        return None
-
-    def close(self) -> None:
-        """
-        Not use in this implementation.
-        Do nothing.
-        """
-        pass
-
-    @property
-    def path(self) -> ParsedPath:
-        """
-        Returns the path of the node.
-
-        Returns:
-            ParsedPath: The path of the node.
-        """
-        if self._path is None:
-            self._path = self.parent.path / self.name
-        return self._path
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        """
-        Return the parent of this node if he has one otherwise None.
-
-        Returns:
-            DrbNode: The parent of this node or None.
-        """
-        return self._parent
-
-    @property
-    def name(self) -> str:
-        """
-        Return the name of the node.
-        This name doesn't contain the path of the node.
-
-        Returns:
-            str: the node name
-        """
-        return self._name
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if self._attributes is None:
-            self._attributes = {}
-            for key in self._data_set.attrs.keys():
-                self._attributes[key, None] = self._data_set.attrs[key]
-            self._attributes[
-                DrbZarrAttributeNames.READ_ONLY.value, None
-            ] = self._data_set.read_only
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        key = (name, namespace_uri)
-        if key in self.attributes.keys():
-            return self.attributes[key]
-        raise DrbException(
-            f"Attribute not found name: {name}, " f"namespace: {namespace_uri}"
-        )
-
-    @property
-    def value(self) -> Optional[Any]:
-        """
-        Not use in this implementation.
-
-        Returns:
-            None
-        """
-        return None
-
-    def has_impl(self, impl: type) -> bool:
-        return impl is self._data_set.__class__
+        self._available_impl = [
+            data_set.__class__
+        ]
+        self.__init_attributes()
+
+    def __init_attributes(self):
+        for key in self._data_set.attrs.keys():
+            self @= (key, self._data_set.attrs[key])
+        self @= (DrbZarrAttributeNames.READ_ONLY.value,
+                 self._data_set.read_only)
 
     def get_impl(self, impl: type, **kwargs) -> Any:
         if self.has_impl(impl):
             return self._data_set
         raise DrbNotImplementationException(
             f"no {impl} " f"implementation found"
         )
@@ -144,14 +72,20 @@
             name = "."
         if isinstance(data_set, zarr.hierarchy.Group):
             node = DrbZarrGroupNode(parent, name, data_set)
         else:
             node = DrbZarrArrayNode(parent, name, data_set)
         return node
 
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
+
 
 class DrbZarrGroupNode(DrbZarrDataSetNode):
     """
     This node is used to organize the data in a zarr architecture,
     he contains a group of zarr array in his children
     or another DrbZarrGroupNode.
 
@@ -170,14 +104,15 @@
         name: str,
         data_set: Union[zarr.hierarchy.Group, zarr.core.Array],
     ):
         super().__init__(parent, name, data_set)
         self._children: List[DrbNode] = None
 
     @property
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     @resolver.resolve_children
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
             self._data_set.visitvalues(self.add_data_set_children)
         return self._children
 
@@ -231,12 +166,10 @@
         parent: DrbNode,
         name: str,
         data_set: Union[zarr.hierarchy.Group, zarr.core.Array],
     ):
         super().__init__(parent, name, data_set)
 
     @property
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def children(self) -> List[DrbNode]:
         return []
-
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        return False
```

### Comparing `drb-driver-zarr-1.1.0/drb/drivers/zarr/zarr_node_factory.py` & `drb-driver-zarr-1.2.0/drb/drivers/zarr/zarr_node_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, List, Dict, Tuple, Optional
 
+from deprecated.classic import deprecated
 from drb.core import DrbNode
 from drb.nodes.abstract_node import AbstractNode
 from drb.core.factory import DrbFactory
 from drb.core.path import ParsedPath
 import zarr
 
 from drb.exceptions.zarr import DrbZarrNodeException
@@ -42,21 +43,27 @@
         return self.base_node.namespace_uri
 
     @property
     def value(self) -> Optional[Any]:
         return self.base_node.value
 
     @property
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def attributes(self) -> Dict[Tuple[str, str], Any]:
         return self.base_node.attributes
 
+    def impl_capabilities(self) -> List[type]:
+        return self.base_node.impl_capabilities()
+
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
         return self.base_node.get_attribute(name, namespace_uri)
 
     @property
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def children(self) -> List[DrbNode]:
         if self._children is None:
             try:
                 root_data_set = zarr.open(self.base_node.path.name)
                 root_node = DrbZarrDataSetNode.create_node_from_data_set(
                     self, root_data_set
                 )
@@ -77,13 +84,19 @@
 
     def get_impl(self, impl: type, **kwargs) -> Any:
         return self.base_node.get_impl(impl)
 
     def close(self):
         self.base_node.close()
 
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
+
 
 class DrbZarrFactory(DrbFactory):
     def _create(self, node: DrbNode) -> DrbNode:
         if isinstance(node, DrbZarrNode):
             return node
         return DrbZarrNode(base_node=node)
```

### Comparing `drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/PKG-INFO` & `drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-zarr
-Version: 1.1.0
+Version: 1.2.0
 Summary: DRB Zarr driver
-Home-page: https://gitlab.com/drb-python/impl/zarr
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/zarr
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/zarr
 Project-URL: Source, https://gitlab.com/drb-python/impl/zarr
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # ZarrNode Driver
 
 This drb-driver-zarr module implements access to zarr containers with DRB data model. It is able to navigates among the zarr contents.
 
 ## Zar Factory and Zarr Node
 
@@ -38,9 +37,7 @@
 ## Using this module
 
 To include this module into your project, the `drb-driver-zarr` module shall be referenced into `requirements.txt` file, or the following pip line can be run:
 
 ```commandline
 pip install drb-driver-zarr
 ```
-
-
```

### Comparing `drb-driver-zarr-1.1.0/drb_driver_zarr.egg-info/SOURCES.txt` & `drb-driver-zarr-1.2.0/drb_driver_zarr.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENCE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 drb/drivers/zarr/__init__.py
 drb/drivers/zarr/_version.py
 drb/drivers/zarr/zarr_data_set_node.py
@@ -11,9 +13,14 @@
 drb/exceptions/zarr.py
 drb/topics/zarr/__init__.py
 drb/topics/zarr/cortex.yml
 drb_driver_zarr.egg-info/PKG-INFO
 drb_driver_zarr.egg-info/SOURCES.txt
 drb_driver_zarr.egg-info/dependency_links.txt
 drb_driver_zarr.egg-info/entry_points.txt
+drb_driver_zarr.egg-info/not-zip-safe
 drb_driver_zarr.egg-info/requires.txt
-drb_driver_zarr.egg-info/top_level.txt
+drb_driver_zarr.egg-info/top_level.txt
+tests/test_drb_zarr_array.py
+tests/test_drb_zarr_group.py
+tests/test_drb_zarr_node_factory.py
+tests/test_drb_zarr_signature.py
```

### Comparing `drb-driver-zarr-1.1.0/versioneer.py` & `drb-driver-zarr-1.2.0/versioneer.py`

 * *Files identical despite different names*

