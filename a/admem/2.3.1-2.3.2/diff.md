# Comparing `tmp/admem-2.3.1.tar.gz` & `tmp/admem-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admem-2.3.1.tar", last modified: Tue May  2 15:21:16 2023, max compression
+gzip compressed data, was "admem-2.3.2.tar", last modified: Tue May  2 21:09:52 2023, max compression
```

## Comparing `admem-2.3.1.tar` & `admem-2.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.617513 admem-2.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-05-02 14:46:08.000000 admem-2.3.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 15:21:16.617513 admem-2.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-02 15:21:16.621513 admem-2.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.601512 admem-2.3.1/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.613512 admem-2.3.1/source/admem/
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_backend_manager_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     6684 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_create_django_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     8282 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_django_store.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_inspect_dataclass.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-05-02 15:02:28.000000 admem-2.3.1/source/admem/_path_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_protocols.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_store_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/_util.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:46:09.000000 admem-2.3.1/source/admem/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:21:16.617513 admem-2.3.1/source/admem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:20:57.000000 admem-2.3.1/source/admem.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-02 15:21:16.000000 admem-2.3.1/source/admem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.276428 admem-2.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-05-02 14:46:08.000000 admem-2.3.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 21:09:52.276428 admem-2.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-02 21:09:52.276428 admem-2.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.260427 admem-2.3.2/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.272428 admem-2.3.2/source/admem/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-02 21:02:37.000000 admem-2.3.2/source/admem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_backend_manager_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_create_django_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8282 2023-05-02 21:02:37.000000 admem-2.3.2/source/admem/_django_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_inspect_dataclass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2301 2023-05-02 21:02:37.000000 admem-2.3.2/source/admem/_path_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_protocols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_store_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.276428 admem-2.3.2/source/admem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:09:44.000000 admem-2.3.2/source/admem.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      232 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/top_level.txt
```

### Comparing `admem-2.3.1/LICENSE.txt` & `admem-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/setup.cfg` & `admem-2.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem/__init__.py` & `admem-2.3.2/source/admem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     + _sync_store.__all__
     + _store_setup.__all__
     + _create_django_model.__all__
     + _inspect_dataclass.__all__
 )
 
 
-__version__ = "2.3.1"
+__version__ = "2.3.2"
```

### Comparing `admem-2.3.1/source/admem/_backend_manager_proxy.py` & `admem-2.3.2/source/admem/_backend_manager_proxy.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem/_create_django_model.py` & `admem-2.3.2/source/admem/_create_django_model.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem/_decorator.py` & `admem-2.3.2/source/admem/_decorator.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem/_django_store.py` & `admem-2.3.2/source/admem/_django_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         dj_field = model._meta.get_field(dc_field.name)
         prefix: str | None = None
         if hasattr(dj_field, "upload_to"):
             prefix = getattr(dj_field, "upload_to")
 
         def inner(fieldfile: FieldFile) -> DjangoPath:
             assert fieldfile.name
-            res = DjangoPath.create(fieldfile.name, prefix)
+            res = DjangoPath(fieldfile.name, prefix=prefix)
             return res
 
         return inner
 
     def django_to_dataclass(self, dj_obj: models.Model) -> tp.Any:
         dataclass = BACKEND_LINKER.backend_to_dc[type(dj_obj)]
         obj_kwgs = {}
```

### Comparing `admem-2.3.1/source/admem/_inspect_dataclass.py` & `admem-2.3.2/source/admem/_inspect_dataclass.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem/_path_proxy.py` & `admem-2.3.2/source/admem/_path_proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 # Copyright (c) 2022-2023 Mario S. Könz; License: MIT
 import os
 import typing as tp  # pylint: disable=reimported
 from pathlib import _posix_flavour  # type: ignore
 from pathlib import _windows_flavour  # type: ignore
 from pathlib import Path
+from pathlib import PosixPath
+from pathlib import WindowsPath
 
 from django.core.files.storage import get_storage_class
 
 # 2023-Q1: sphinx has a bug regarding adjusting the signature for attributes,
 # hence I need fully qualified imports for typing and django.db
 
 __all__ = ["DjangoPath"]
 
 
 class DjangoPath(Path):
     _flavour = _windows_flavour if os.name == "nt" else _posix_flavour
+    __slots__ = ("_prefix",)
+
+    def __new__(  # pylint: disable=arguments-differ
+        cls, *args: str, prefix: str | None = None
+    ) -> "DjangoPath":
+        # pylint: disable=no-member,self-cls-assignment
+        cls = DjangoPosixPath
+        if os.name == "nt":
+            cls = DjangoWindowsPath
+        res = super().__new__(cls, *args)
+        res._prefix = prefix  # type: ignore
+        return res
 
     def name_wo_prefix(self) -> str:
         name = self.as_posix()
-        print(f"\033[1;32m========>> {hasattr(self, 'prefix')} {self}\033[0m")
+        # pylint: disable=no-member
 
         if self._prefix:  # type: ignore
             name = name.split(self._prefix + "/", 1)[1]  # type: ignore
         return name
 
-    @classmethod
-    def create(cls, path: Path | str, prefix: str | None) -> "DjangoPath":
-        # pylint: disable=attribute-defined-outside-init
-        res = cls(path)
-        res._prefix = prefix  # type: ignore
-        return res
-
     def __copy__(self) -> "DjangoPath":
-        # pylint: disable=protected-access,no-member,attribute-defined-outside-init
-        res = self.__class__(self)
-        res._prefix = self._prefix  # type: ignore
-        return res
+        # pylint: disable=no-member
+        return self.__class__(self, prefix=self._prefix)  # type: ignore
 
-    def __deepcopy__(self, memo: dict[tp.Any, tp.Any]) -> "DjangoPath":
-        # pylint: disable=protected-access,no-member,attribute-defined-outside-init
-        res = self.__class__(self)
-        res._prefix = self._prefix  # type: ignore
-        return res
+    def __deepcopy__(self, memo: dict[str, tp.Any]) -> "DjangoPath":
+        # pylint: disable=no-member
+        return self.__class__(self, prefix=self._prefix)  # type: ignore
 
     def open(  # type: ignore  # pylint: disable=too-many-arguments
         self,
         mode: str = "r",
         buffering: int = -1,
         encoding: str | None = None,
         errors: str | None = None,
@@ -53,7 +56,15 @@
     ) -> tp.IO[tp.Any]:
         # assert encoding is None
         assert errors is None
         assert newline is None
         assert buffering == -1
         media_storage = get_storage_class()()
         return media_storage.open(self.as_posix(), mode=mode)
+
+
+class DjangoPosixPath(PosixPath, DjangoPath):  # pylint: disable=abstract-method
+    pass
+
+
+class DjangoWindowsPath(WindowsPath, DjangoPath):  # pylint: disable=abstract-method
+    pass
```

### Comparing `admem-2.3.1/source/admem/_protocols.py` & `admem-2.3.2/source/admem/_protocols.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem/_store_setup.py` & `admem-2.3.2/source/admem/_store_setup.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem/_sync_store.py` & `admem-2.3.2/source/admem/_sync_store.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.1/source/admem.egg-info/SOURCES.txt` & `admem-2.3.2/source/admem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

