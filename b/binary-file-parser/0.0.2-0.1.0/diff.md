# Comparing `tmp/binary-file-parser-0.0.2.tar.gz` & `tmp/binary-file-parser-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary-file-parser-0.0.2.tar", last modified: Thu Dec 15 18:25:51 2022, max compression
+gzip compressed data, was "binary-file-parser-0.1.0.tar", last modified: Tue May  2 06:12:19 2023, max compression
```

## Comparing `binary-file-parser-0.0.2.tar` & `binary-file-parser-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-12-15 18:25:51.467682 binary-file-parser-0.0.2/
--rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary-file-parser-0.0.2/LICENSE
--rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary-file-parser-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3405 2022-12-15 18:25:51.467682 binary-file-parser-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2022-12-15 08:08:32.000000 binary-file-parser-0.0.2/README.md
--rw-rw-rw-   0        0        0      902 2022-12-15 18:25:16.000000 binary-file-parser-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-15 18:25:51.467682 binary-file-parser-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-15 18:25:51.397587 binary-file-parser-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-12-15 18:25:51.406511 binary-file-parser-0.0.2/src/binary_file_parser/
--rw-rw-rw-   0        0        0      214 2022-12-15 07:21:45.000000 binary-file-parser-0.0.2/src/binary_file_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:25:51.432733 binary-file-parser-0.0.2/src/binary_file_parser/errors/
--rw-rw-rw-   0        0        0      118 2022-12-15 18:24:53.000000 binary-file-parser-0.0.2/src/binary_file_parser/errors/CompressionError.py
--rw-rw-rw-   0        0        0       42 2022-12-15 07:13:59.000000 binary-file-parser-0.0.2/src/binary_file_parser/errors/ParsingError.py
--rw-rw-rw-   0        0        0      114 2022-12-15 18:24:20.000000 binary-file-parser-0.0.2/src/binary_file_parser/errors/VersionError.py
--rw-rw-rw-   0        0        0      128 2022-12-15 07:16:50.000000 binary-file-parser-0.0.2/src/binary_file_parser/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:25:51.437732 binary-file-parser-0.0.2/src/binary_file_parser/retrievers/
--rw-rw-rw-   0        0        0     9963 2022-12-15 18:22:22.000000 binary-file-parser-0.0.2/src/binary_file_parser/retrievers/BaseStruct.py
--rw-rw-rw-   0        0        0     2647 2022-11-29 16:43:10.000000 binary-file-parser-0.0.2/src/binary_file_parser/retrievers/MapValidate.py
--rw-rw-rw-   0        0        0    10243 2022-12-15 07:37:11.000000 binary-file-parser-0.0.2/src/binary_file_parser/retrievers/Retriever.py
--rw-rw-rw-   0        0        0      106 2022-12-15 07:16:50.000000 binary-file-parser-0.0.2/src/binary_file_parser/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:25:51.465662 binary-file-parser-0.0.2/src/binary_file_parser/types/
--rw-rw-rw-   0        0        0     6137 2022-12-15 07:41:09.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/Array.py
--rw-rw-rw-   0        0        0      896 2022-12-15 07:41:09.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/Bool.py
--rw-rw-rw-   0        0        0     2796 2022-11-29 16:43:10.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/ByteStream.py
--rw-rw-rw-   0        0        0      815 2022-12-15 07:41:09.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/Bytes.py
--rw-rw-rw-   0        0        0      827 2022-12-15 05:38:48.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/Float.py
--rw-rw-rw-   0        0        0      955 2022-12-15 05:38:49.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/Int.py
--rw-rw-rw-   0        0        0      691 2022-12-15 05:38:48.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/Parseable.py
--rw-rw-rw-   0        0        0     3014 2022-12-15 05:38:48.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/Str.py
--rw-rw-rw-   0        0        0      515 2022-12-15 07:16:50.000000 binary-file-parser-0.0.2/src/binary_file_parser/types/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 18:25:51.427835 binary-file-parser-0.0.2/src/binary_file_parser.egg-info/
--rw-rw-rw-   0        0        0     3405 2022-12-15 18:25:51.000000 binary-file-parser-0.0.2/src/binary_file_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2022-12-15 18:25:51.000000 binary-file-parser-0.0.2/src/binary_file_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-15 18:25:51.000000 binary-file-parser-0.0.2/src/binary_file_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2022-12-15 18:25:51.000000 binary-file-parser-0.0.2/src/binary_file_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-12-15 18:25:51.000000 binary-file-parser-0.0.2/src/binary_file_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.172717 binary-file-parser-0.1.0/
+-rw-rw-rw-   0        0        0     1084 2022-12-14 12:48:09.000000 binary-file-parser-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2022-12-15 05:10:52.000000 binary-file-parser-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3411 2023-05-02 06:12:19.171717 binary-file-parser-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1482 2022-12-18 10:54:12.000000 binary-file-parser-0.1.0/README.md
+-rw-rw-rw-   0        0        0      908 2023-03-21 02:27:40.000000 binary-file-parser-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 06:12:19.172717 binary-file-parser-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 06:12:18.929716 binary-file-parser-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 06:12:18.956715 binary-file-parser-0.1.0/src/binary_file_parser/
+-rw-rw-rw-   0        0        0      290 2023-05-02 04:00:31.000000 binary-file-parser-0.1.0/src/binary_file_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.017718 binary-file-parser-0.1.0/src/binary_file_parser/errors/
+-rw-rw-rw-   0        0        0      118 2022-12-15 18:24:53.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/CompressionError.py
+-rw-rw-rw-   0        0        0       42 2022-12-15 07:13:59.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/ParsingError.py
+-rw-rw-rw-   0        0        0      114 2022-12-15 18:24:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/VersionError.py
+-rw-rw-rw-   0        0        0      128 2022-12-15 07:16:50.000000 binary-file-parser-0.1.0/src/binary_file_parser/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.081718 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/
+-rw-rw-rw-   0        0        0     2647 2023-02-18 09:06:26.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/MapValidate.py
+-rw-rw-rw-   0        0        0     2272 2023-04-24 11:23:48.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/RetreiverCombiner.py
+-rw-rw-rw-   0        0        0     1518 2023-04-24 11:16:38.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/RetreiverRef.py
+-rw-rw-rw-   0        0        0    11222 2023-05-02 03:50:09.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/Retriever.py
+-rw-rw-rw-   0        0        0      199 2023-04-21 01:37:15.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/__init__.py
+-rw-rw-rw-   0        0        0    15418 2023-05-02 04:12:57.000000 binary-file-parser-0.1.0/src/binary_file_parser/retrievers/base_struct.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:12:19.169717 binary-file-parser-0.1.0/src/binary_file_parser/types/
+-rw-rw-rw-   0        0        0     6438 2023-04-21 03:06:40.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Array.py
+-rw-rw-rw-   0        0        0      928 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Bool.py
+-rw-rw-rw-   0        0        0     2796 2022-11-29 16:43:10.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/ByteStream.py
+-rw-rw-rw-   0        0        0      855 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Bytes.py
+-rw-rw-rw-   0        0        0      867 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Float.py
+-rw-rw-rw-   0        0        0      987 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Int.py
+-rw-rw-rw-   0        0        0     1345 2023-04-21 02:01:03.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Parseable.py
+-rw-rw-rw-   0        0        0     2584 2023-04-21 03:37:25.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/RefList.py
+-rw-rw-rw-   0        0        0     3037 2023-04-18 12:21:20.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/Str.py
+-rw-rw-rw-   0        0        0      545 2023-04-21 02:02:51.000000 binary-file-parser-0.1.0/src/binary_file_parser/types/__init__.py
+-rw-rw-rw-   0        0        0      596 2023-05-02 03:35:56.000000 binary-file-parser-0.1.0/src/binary_file_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:12:18.976715 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/
+-rw-rw-rw-   0        0        0     3411 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1209 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-02 06:12:18.000000 binary-file-parser-0.1.0/src/binary_file_parser.egg-info/top_level.txt
```

### Comparing `binary-file-parser-0.0.2/LICENSE` & `binary-file-parser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.0.2/PKG-INFO` & `binary-file-parser-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-file-parser
-Version: 0.0.2
+Version: 0.1.0
 Summary: Read/Write binary files after describing their specifications in code (similar to an ORM table schema)
 Author-email: Divy1211 <divy1211.dc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alian713
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/Divy1211/FileParser
+Project-URL: Homepage, https://github.com/Divy1211/BinaryFileParser
 Keywords: binary,file,parser
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -63,17 +63,17 @@
 
 ```py
 from binary_file_parser import BaseStruct, Retriever
 from binary_file_parser.types import int32, uint64, str32, FixedLenStr
 
 class Spam(BaseStruct):
     file_version: str = Retriever(FixedLenStr[4], default = 0)
-    creator_name: int = Retriever(str32, default = 0)
+    creator_name: str = Retriever(str32, default = 0)
     saved_timestamp: int = Retriever(uint64, default = 0)
-    eggs: str = Retriever(int32, default = 0)
+    eggs: int = Retriever(int32, default = 0)
 
 # read a binary file that has the above format
 file = Spam.from_file("path/to/file")
 
 # modify the creator name
 file.creator_name = "Alian713"
 file.eggs = 20
```

### Comparing `binary-file-parser-0.0.2/README.md` & `binary-file-parser-0.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 ```py
 from binary_file_parser import BaseStruct, Retriever
 from binary_file_parser.types import int32, uint64, str32, FixedLenStr
 
 class Spam(BaseStruct):
     file_version: str = Retriever(FixedLenStr[4], default = 0)
-    creator_name: int = Retriever(str32, default = 0)
+    creator_name: str = Retriever(str32, default = 0)
     saved_timestamp: int = Retriever(uint64, default = 0)
-    eggs: str = Retriever(int32, default = 0)
+    eggs: int = Retriever(int32, default = 0)
 
 # read a binary file that has the above format
 file = Spam.from_file("path/to/file")
 
 # modify the creator name
 file.creator_name = "Alian713"
 file.eggs = 20
```

### Comparing `binary-file-parser-0.0.2/pyproject.toml` & `binary-file-parser-0.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=57.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "binary-file-parser"
-version = "0.0.2"
+version = "0.1.0"
 description = "Read/Write binary files after describing their specifications in code (similar to an ORM table schema)"
 readme = "README.md"
 authors = [{ name = "Divy1211", email = "divy1211.dc@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,8 +23,8 @@
 
 [project.optional-dependencies]
 dev = ["pytest", "pylint"]
 docs = ["mkdocs"]
 depl = ["build", "twine"]
 
 [project.urls]
-Homepage = "https://github.com/Divy1211/FileParser"
+Homepage = "https://github.com/Divy1211/BinaryFileParser"
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/retrievers/BaseStruct.py` & `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/base_struct.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,168 @@
 from __future__ import annotations
 
-from abc import ABCMeta
+from io import StringIO
+from contextlib import suppress
 from typing import TYPE_CHECKING
 
 from alive_progress import alive_it
 
 from binary_file_parser.errors import CompressionError
 from binary_file_parser.errors import ParsingError
 from binary_file_parser.errors import VersionError
-from binary_file_parser.types import ByteStream
+from binary_file_parser.types import ByteStream, RefList
 from binary_file_parser.types import Parseable
+from binary_file_parser.utils import indentify, Version
 
 if TYPE_CHECKING:
     from binary_file_parser.retrievers.Retriever import Retriever
+    from binary_file_parser.retrievers.RetreiverCombiner import RetrieverCombiner
+    from binary_file_parser.retrievers.RetreiverRef import RetrieverRef
 
 
 class BaseStruct(Parseable):
     """
     Base class for defining a file format as a structure
     """
-    __slots__ = "struct_version", "parent"
+    __slots__ = "_struct_ver", "_parent"
 
     _retrievers: list[Retriever] = []
+    _refs: list[RetrieverRef] = []
+    _combiners: list[RetrieverCombiner] = []
 
     @classmethod
-    def add_retriever(cls, retriever: Retriever):
+    def _add_retriever(cls, retriever: Retriever):
         cls._retrievers.append(retriever)
 
-    def __init_subclass__(cls, **kwargs):
-        cls_retrievers = cls._retrievers[:]
-        BaseStruct._retrievers = []
-        cls._retrievers = cls_retrievers
-
     @classmethod
-    def from_default(cls, struct_version: tuple[int, ...] = None, instance: BaseStruct = None) -> BaseStruct:
-        """
-        Create the object representing the file format using default values
-
-        :param struct_version: This is the version of the format that will be created
-        :param instance: Initialise this object from defaults
+    def _add_ref(cls, ref: RetrieverRef):
+        cls._refs.append(ref)
 
-        :return: An instance of a subtype of BaseStruct
-        """
-        instance = instance or cls() if not struct_version else cls(struct_version)
-        for retriever in cls._retrievers:
-            if not retriever.supported(instance.struct_version):
-                continue
-            setattr(instance, retriever.p_name, retriever.from_default(instance))
-        return instance
+    @classmethod
+    def _add_combiner(cls, combiner: RetrieverCombiner):
+        cls._combiners.append(combiner)
 
-    def __init__(self, struct_version: tuple[int, ...] = (0,), parent: BaseStruct = None, initialise_defaults = True):
+    def __init__(
+        self,
+        struct_ver: Version = Version((0,)),
+        parent: BaseStruct = None,
+        idx: int = -1,
+        initialise_defaults: bool = True,
+        **retriever_inits,
+    ):
         """
-        :param struct_version: The struct version to create
+        :param idx:
+        :param struct_ver: The struct version to create
         :param parent: If this struct is nested within another, define the containing struct as parent
         :param initialise_defaults:
             If set to false, skip initialisation of struct values from default. This is only set to false when reading
             a file
+        :param retriever_inits:
+            Use this to provide initial values to retrievers
         """
+        self._struct_ver = struct_ver
+        self._parent = parent
+        self.idx = idx
+
         size = 0
         for retriever in self._retrievers:
-            if not retriever.supported(struct_version):
+            if not retriever.supported(struct_ver):
                 continue
 
-            if type(retriever.dtype) is ABCMeta and issubclass(retriever.dtype, BaseStruct):
-                size += retriever.default.size
-            else:
-                size += retriever.dtype.size
+            if initialise_defaults:
+                init = retriever_inits.get(retriever.p_name, None)
+                if init is None:
+                    init = retriever.from_default(self)
+                setattr(self, retriever.p_name, init)
 
+            size += retriever.default.size if retriever.dtype.is_struct else retriever.dtype.size
         super().__init__(size)
-        self.struct_version = struct_version
-        self.parent = parent
-        if initialise_defaults:
-            self.from_default(instance = self)
+
+    def __init_subclass__(cls, **kwargs):
+        cls._retrievers, BaseStruct._retrievers = cls._retrievers.copy(), []
+        cls._refs, BaseStruct._refs = cls._refs.copy(), []
+        cls._combiners, BaseStruct._combiners = cls._combiners.copy(), []
+
+    @property
+    def is_struct(self) -> bool:
+        return True
+
+    @property
+    def root(self) -> BaseStruct:
+        """
+        The top level object of which this struct is a part of
+        """
+        child = self
+        while child.parent is not None:
+            child = self.parent
+        return child
+
+    def on_struct_ver_change(self, new_struct_ver: Version):
+        """
+        This method is called when a struct's version is changed. Use this to implement any custom logic required to
+        support a version change on a struct. The default method implements a trial and error algorithm where if an
+        unsupported retriever after the version change used to have the same value as its default, then it is discarded
+        without any errors, However, if a value other than the default was assigned to it, an error is raised
+
+        :param new_struct_ver: The new struct version (the self.struct_ver attribute will automatically be updated)
+
+        :raises VersionError: When the version change causes a non default valued retriever to become unsupported
+        """
+        ...
+
+    @property
+    def struct_ver(self):
+        return self._struct_ver
+
+    @struct_ver.setter
+    def struct_ver(self, new_struct_ver: Version):
+        for retriever in self._retrievers:
+            if (
+                not retriever.supported(self.struct_ver)
+                or not (retriever.dtype.is_struct or retriever.dtype.is_iterable)
+                or retriever.is_self_versioned
+            ):
+                continue
+            if (obj := getattr(self, retriever.p_name)) is not None:
+                obj.struct_ver = new_struct_ver
+        self.on_struct_ver_change(new_struct_ver)
+        self._struct_ver = new_struct_ver
+
+    @property
+    def parent(self):
+        return self._parent
+
+    @parent.setter
+    def parent(self, new_parent: BaseStruct):
+        for retriever in self._retrievers:
+            if (
+                not retriever.supported(self.struct_ver)
+                or not (retriever.dtype.is_struct or retriever.dtype.is_iterable)
+            ):
+                continue
+            if (obj := getattr(self, retriever.p_name)) is not None:
+                obj.parent = new_parent
+        self._parent = new_parent
+
+    @property
+    def retriever_name_value_map(self) -> dict[str]:
+        map_ = {}
+        for retriever in self._retrievers:
+            map_[retriever.p_name] = getattr(self, retriever.p_name)
+        return map_
 
     @classmethod
-    def get_version(cls, stream: ByteStream) -> tuple[int, ...]:
+    def get_version(cls, stream: ByteStream, struct_ver: Version = Version((0,)), parent: BaseStruct = None) -> Version:
         """
         If defined, the struct will be versioned and values in the struct which are not supported in the version that is
         read will be skipped
 
         :param stream: The stream to read the struct version from
+        :param struct_ver: The struct version of the parent
+        :param parent:
         :return: A tuple of ints indicating the version eg: v1.47 should return (1, 47)
         :raises VersionError: - When unimplemented
         """
         raise VersionError("Un-versioned File")
 
     @classmethod
     def decompress(cls, bytes_: bytes) -> bytes:
@@ -113,33 +192,31 @@
         raise CompressionError(
             "Unable to write object to file. "
             "A Structure with compressed section needs to implement 'compress' classmethod."
         )
 
     @classmethod
     def from_stream(
-        cls, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,), strict: bool = False,
+        cls, stream: ByteStream, *, struct_ver: Version = Version((0,)), strict: bool = False,
         show_progress: bool = False, parent: BaseStruct = None
     ) -> BaseStruct:
         """
         Create a struct object from a ByteStream
 
         :param stream: The stream to create the struct object from
-        :param struct_version: The version of the structure to create. Overwritten if `get_version` is defined
+        :param struct_ver: The version of the structure to create. Overwritten if `get_version` is defined
         :param strict: Raise an error if struct parsing finishes successfully but the stream has left over bytes
         :param show_progress: When true, display a progress bar
         :param parent: If this struct is nested within another, define the containing struct as parent
         :return: An instance of a subtype of BaseStruct
         """
-        try:
-            struct_version = cls.get_version(stream)
-        except VersionError:
-            pass
+        with suppress(VersionError):
+            struct_ver = cls.get_version(stream, struct_ver, parent)
 
-        instance = cls(struct_version, parent, initialise_defaults = False)
+        instance = cls(struct_ver, parent, initialise_defaults = False)
         retriever_ls = cls._retrievers
         if show_progress:
             retriever_ls = alive_it(
                 retriever_ls,
                 dual_line = True,
                 title = f"         Reading File",
                 stats = False,
@@ -152,43 +229,46 @@
             if retriever.remaining_compressed:
                 stream = ByteStream.from_bytes(cls.decompress(stream.remaining()))
             retriever.from_stream(instance, stream)
 
         file_len = len(stream.content)
 
         if stream.progress != file_len and strict:
-            raise ParsingError(f"{file_len - stream.progress} bytes are left after parsing all retrievers successfully")
+            raise ParsingError(
+                f"{file_len - stream.progress} bytes are left after parsing all retrievers successfully:\n"
+                f"{stream.remaining()}"
+            )
 
         return instance
 
     @classmethod
-    def from_bytes(cls, bytes_: bytes, *, struct_version: tuple[int, ...] = (0,), strict = False) -> BaseStruct:
+    def from_bytes(cls, bytes_: bytes, *, struct_ver: Version = Version((0,)), strict = False) -> BaseStruct:
         """
         Create a struct object from bytes
 
         :param bytes_: The bytes to create the struct object from
-        :param struct_version: The version of the structure to create. Overwritten if `get_version` is defined
+        :param struct_ver: The version of the structure to create. Overwritten if `get_version` is defined
         :param strict: Raise an error if struct parsing finishes successfully but there are unused bytes left over
         :return: An instance of a subtype of BaseStruct
         """
         stream = ByteStream.from_bytes(bytes_)
-        return cls.from_stream(stream, struct_version = struct_version, strict = strict)
+        return cls.from_stream(stream, struct_ver = struct_ver, strict = strict)
 
     @classmethod
-    def from_file(cls, file_name: str, *, file_version: tuple[int, ...] = (0,), strict = False) -> BaseStruct:
+    def from_file(cls, file_name: str, *, file_version: Version = Version((0,)), strict = True) -> BaseStruct:
         """
         Create a struct object from file
 
         :param file_name: The path of the file to create the struct object from
         :param file_version: The version of the structure to create. Overwritten if `get_version` is defined
         :param strict: Raise an error if struct parsing finishes successfully but the stream has left over bytes
         :return: An instance of a subtype of BaseStruct
         """
         stream = ByteStream.from_file(file_name)
-        return cls.from_stream(stream, struct_version = file_version, strict = strict, show_progress = True)
+        return cls.from_stream(stream, struct_ver = file_version, strict = strict, show_progress = True)
 
     @classmethod
     def to_bytes(cls, instance: BaseStruct, *, show_progress = False) -> bytes:
         """
         Convert the struct object to bytes
 
         :param instance: The struct object to convert to bytes
@@ -231,13 +311,76 @@
         Write the bytes of the struct object to a file
 
         :param file_name: The name of the file to write to
         """
         with open(file_name, "wb") as file:
             file.write(self.to_bytes(self, show_progress = True))
 
+    def diff(self, other: BaseStruct) -> list[Retriever]:
+        """
+        Recursively builds a list of retrievers that have different values for the two objects.
+
+        :param other: The object to diff with
+        :return: list of retrievers that have different values for the two objects
+        """
+        if (
+            not isinstance(other, BaseStruct)
+            or type(self) is not type(other)
+        ):
+            raise TypeError(f"Cannot diff '{type(self)}' with an object of type '{type(other)}'")
+        if self.struct_ver != other.struct_ver:
+            raise VersionError(
+                f"Cannot diff structs with different versions '{self.struct_ver}' and '{other.struct_ver}'"
+            )
+
+        diff_retrievers: list[Retriever] = []
+        for retriever in self._retrievers:
+            if not retriever.supported(self.struct_ver):
+                continue
+            if (val1 := getattr(self, retriever.p_name)) == (val2 := getattr(other, retriever.p_name)):
+                continue
+            if retriever.dtype.is_struct and not isinstance(val1, RefList): # todo: implement a diff on reflists
+                diff_retrievers.extend(val1.diff(val2))
+            else:
+                diff_retrievers.append(retriever)
+        return diff_retrievers
+
+    def __repr__(self) -> str:
+        repr_builder = StringIO()
+        repr_builder.write(f"{self.__class__.__name__}(")
+        for retriever in self._retrievers:
+            if not retriever.supported(self.struct_ver):
+                continue
+
+            obj = getattr(self, retriever.p_name)
+            if isinstance(obj, list):
+                sub_obj_repr_str = (
+                    "[\n    "
+                    + ",\n    ".join(map(lambda x: indentify(repr(x)), obj))
+                    + ",\n]"
+                )
+            else:
+                sub_obj_repr_str = f"{obj!r}"
+
+            repr_builder.write(f"\n    {retriever.p_name} = {indentify(sub_obj_repr_str)},")
+        repr_builder.write("\n)")
+        return repr_builder.getvalue()
+
+    def __eq__(self, other: object) -> bool:
+        if (
+            not isinstance(other, BaseStruct)
+            or type(self) is not type(other)
+            or self.struct_ver != other.struct_ver
+        ):
+            return False
+
+        for retriever in self._retrievers:
+            if not retriever.supported(self.struct_ver):
+                continue
+            if getattr(self, retriever.p_name) != getattr(other, retriever.p_name):
+                return False
+        return True
+
     # todo: write val <-> data (names) to file
     # todo: write hex (decompressed) to file
-    # todo: repr, eq, neq
-    # todo: diff
     # todo: file/header/decompressed in both hex/val <-> data
     # todo: to_json
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/retrievers/MapValidate.py` & `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/MapValidate.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/retrievers/Retriever.py` & `binary-file-parser-0.1.0/src/binary_file_parser/retrievers/Retriever.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from __future__ import annotations
 
 
-from abc import ABCMeta
 from copy import copy
+from io import BytesIO
 from typing import Type, Callable, TypeVar
 
 from binary_file_parser.errors import VersionError
 from binary_file_parser.types import ByteStream
 from binary_file_parser.types import Parseable
 
 from binary_file_parser.retrievers.MapValidate import MapValidate
-from binary_file_parser.retrievers.BaseStruct import BaseStruct
-
-
-def ver_str(ver: tuple[int]) -> str:
-    return ".".join(map(str, ver))
-
+from binary_file_parser.retrievers.base_struct import BaseStruct
+from binary_file_parser.types.RefList import RefList
+from binary_file_parser.utils import Version
 
 T = TypeVar("T")
 RetrieverSub = TypeVar("RetrieverSub", bound = "Retriever")
 BaseStructSub = TypeVar("BaseStructSub", bound = BaseStruct)
 
 
 class Retriever(MapValidate):
     """
     Represents a binary object in a struct and the restrictions/dependencies associated with it
     """
-    __slots__ = "dtype", "min_ver", "max_ver", "default", "_repeat", "remaining_compressed", "on_read", "on_write"
+    __slots__ = "atype", "dtype", "min_ver", "max_ver", "default", "_repeat", "remaining_compressed", "on_read", "on_write"
 
     def __init__(
         self,
         dtype: Parseable | Type[Parseable],
-        min_ver: tuple[int] = (-1,),
-        max_ver: tuple[int] = (1000,),
+        min_ver: Version = Version((-1,)),
+        max_ver: Version = Version((1000,)),
         *,
         default: T = None,
         repeat: int = 1,
+        atype: Type[RefList] = RefList,
         remaining_compressed: bool = False,
-        on_read: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,
+        on_read: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,  # todo: add implementations for common on_x operations
         on_write: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,
         mappers: list[Callable[[RetrieverSub, BaseStructSub, T], T]] | None = None,
         validators: list[Callable[[RetrieverSub, BaseStructSub, T], tuple[bool, str]]] | None = None,
         on_get: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,
         on_set: list[Callable[[RetrieverSub, BaseStructSub], None]] | None = None,
     ):
         # todo: default factories and deep copies
@@ -58,14 +56,16 @@
         :param default: A default value for this retriever property
         :param repeat:
             The number of times this value is repeated. Possible values for this parameter include:
                 -1: skips reading value entirely, set property to None
                 0: skips reading value entirely, set property to []
                 1: single value is read and assigned to the property
                 >1: a list of values is read and assigned to the property
+        :param atype:
+            The array like type to use when constructing lists for retrievers with dynamic repeats
         :param remaining_compressed:
             If set to true, the decompress/compress methods are used on the remaining bytes before reading/writing the
             remaining retriever properties
         :param on_read:
             A list of functions that are called when this retriever property is read from bytes for the first time
         :param on_write: A list of functions that are called when this retriever property is written to bytes
         :param mappers: A list of functions that can mutate the value that is assigned to this retriever property
@@ -73,63 +73,77 @@
             A list of functions that can validate the value that is assigned to this retriever property.
             A ValueError is raised if validation from any one of these functions fails
         :param on_get: A list of functions that are called when this retriever property is accessed
         :param on_set: A list of functions that are called when this retriever property is set
         """
         super().__init__(mappers, validators, on_get, on_set)
         self.dtype = dtype
+        self.atype = atype
         self.min_ver = min_ver
         self.max_ver = max_ver
         self.default = default
         self._repeat = repeat
         self.remaining_compressed = remaining_compressed
         self.on_read = on_read or []
         self.on_write = on_write or []
 
         # if self._repeat == 1:
         #     self.validators.append(lambda retriever, instance, x: dtype.is_valid(x))
         # else:
         #     self.validators.append(lambda retriever, instance, iterable: all(map(dtype.is_valid, iterable)))
 
-    def supported(self, ver: tuple[int, ...]) -> bool:
+    @property
+    def is_self_versioned(self) -> bool:
+        """
+        True if the dtype of this retriever is a struct that implements its own versioning.
+        """
+        try:
+            self.dtype.__class__.get_version(stream = ByteStream.from_bytes(b"\x00"*8))
+            return True
+        except EOFError:
+            return True
+        except (VersionError, AttributeError):
+            return False
+
+    def supported(self, ver: Version) -> bool:
         """
         Determine if this retriever property is supported in the specified version
 
         :param ver: The version to check for support in
         :return: true if supported else false
         """
-        return self.min_ver < ver < self.max_ver
+        return self.min_ver <= ver <= self.max_ver
 
     def __set_name__(self, owner: Type[BaseStruct], name: str) -> None:
         super().__set_name__(owner, name)
-        owner.add_retriever(self)
+        owner._add_retriever(self)
 
     def __set__(self, instance: BaseStruct, value: T) -> None:
-        if not self.supported(instance.struct_version):
+        if not self.supported(instance.struct_ver):
             raise VersionError(
-                f"{self.p_name!r} is not supported in your scenario version {ver_str(instance.struct_version)!r}"
+                f"{self.p_name!r} is not supported in your scenario version {instance.struct_ver}"
             )
 
-        def set_parent(obj):
-            if isinstance(obj, BaseStruct):
-                obj.parent = instance
-            elif isinstance(obj, list):
-                for sub_obj in obj:
-                    set_parent(sub_obj)
-
-        set_parent(value)
+        # def set_parent(obj):
+        #     if isinstance(obj, BaseStruct):
+        #         obj.parent = instance
+        #     elif isinstance(obj, list):
+        #         for sub_obj in obj:
+        #             set_parent(sub_obj)
+        #
+        # set_parent(value)
         super().__set__(instance, value)
 
     def __get__(self, instance: BaseStruct, owner: Type[BaseStruct]) -> Retriever | T:
         if instance is None:
             return self
 
-        if not self.supported(instance.struct_version):
+        if not self.supported(instance.struct_ver):
             raise VersionError(
-                f"{self.p_name!r} is not supported in your scenario version {ver_str(instance.struct_version)!r}"
+                f"{self.p_name!r} is not supported in your struct version {instance.struct_ver}"
             )
         try:
             return super().__get__(instance, owner)
         except AttributeError:
             if self.default is None:
                 raise ValueError(f"No default value specified for retriever {self.p_name!r}")
             return self.from_default(instance)
@@ -154,91 +168,97 @@
         :param instance: The struct object to get the repeat value of this retriever property from
         :return: The repeat value
         """
         if (repeat := getattr(instance, self.r_name, None)) is not None:
             return repeat
         return self._repeat
 
-    def from_default(self, instance: BaseStruct) -> None:
+    def from_default(self, instance: BaseStruct):
         """
         Initialise this retriever property from its default value
 
         :param instance: The struct object to initialise the retriever property for
         """
         repeat = self.repeat(instance)
         if repeat == -1:
             return None
 
         val = self.default
-        if type(self.dtype) is ABCMeta and issubclass(self.dtype, BaseStruct):
+        if self.dtype.is_struct:
             val = (
-                val.from_default(val.struct_version) if repeat == 1
-                else [val.from_default(val.struct_version) for _ in range(repeat)]
+                val.__class__(instance.struct_ver, instance) if repeat == 1
+                else [val.__class__(instance.struct_ver, instance) for _ in range(repeat)]
             )
-        elif isinstance(val, list):
+        elif isinstance(val, list): # todo: this should probably be a deepcopy
             val = copy(val) if repeat == 1 else [copy(val) for _ in range(repeat)]
-        elif repeat != 1:
-            val = [val] * repeat
+        elif repeat != 1: # todo: this should probably be a deepcopy too
+            val = [copy(val) for _ in range(repeat)]
+
+        if isinstance(val, list):
+            val = self.atype(val, instance.struct_ver, instance)
 
         return val
 
     def from_stream(self, instance: BaseStruct, stream: ByteStream) -> None:
         """
         Initialise this retriever property from a stream
 
         :param instance: The struct object to initialise the retriever property for
         :param stream: The stream to initialise the retriever property from
         """
-        if not self.supported(instance.struct_version):
+        if not self.supported(instance.struct_ver):
             return
 
         repeat = self.repeat(instance)
         if repeat == -1:
             setattr(instance, self.p_name, None)
             return
 
         def getobj():
-            if type(self.dtype) is ABCMeta and issubclass(self.dtype, BaseStruct):
-                return self.dtype.from_stream(stream, struct_version = instance.struct_version, parent = instance)
-            return self.dtype.from_stream(stream, struct_version = instance.struct_version)
+            if self.dtype.is_struct:
+                self.dtype: BaseStruct  # type: ignore
+                return self.dtype.from_stream(stream, struct_ver = instance.struct_ver, parent = instance)
+            return self.dtype.from_stream(stream, struct_ver = instance.struct_ver)
 
-        if repeat == 1 and not hasattr(instance, self.r_name):
+        is_not_dynamic_repeat = not hasattr(instance, self.r_name)
+        if repeat == 1 and is_not_dynamic_repeat:
             setattr(instance, self.p_name, getobj())
             return
 
         ls: list = [None] * repeat
         for i in range(repeat):
             ls[i] = getobj()
-        setattr(instance, self.p_name, ls)
+        setattr(instance, self.p_name, self.atype(ls, instance.struct_ver, instance))
 
         for func in self.on_read:
             func(self, instance)
 
     def to_bytes(self, instance: BaseStruct) -> bytes:
         """
         Convert this retriever property to bytes
 
         :param instance: The struct object to convert the retriever property from
         :return: The bytes of the retriever property
         """
-        if not self.supported(instance.struct_version):
+        if not self.supported(instance.struct_ver):
             return b""
 
         repeat = self.repeat(instance)
         if repeat == -1:
             return b""
 
         for func in self.on_write:
             func(self, instance)
 
-        if repeat == 1 and not hasattr(instance, self.r_name):
+        is_not_dynamic_repeat = not hasattr(instance, self.r_name)
+        if repeat == 1 and is_not_dynamic_repeat:
             return self.dtype.to_bytes(getattr(instance, self.p_name))
 
         ls: list = getattr(instance, self.p_name)
-        if not len(ls) == repeat:
+        if len(ls) != repeat:
             raise ValueError(f"length of {self.p_name!r} is not the same as {repeat = }")
 
-        bytes_: list[bytes] = [b""] * repeat
-        for j, value in enumerate(getattr(instance, self.p_name)):
-            bytes_[j] = self.dtype.to_bytes(value)
+        bytes_ = BytesIO()
+        for value in getattr(instance, self.p_name):
+            bytes_.write(self.dtype.to_bytes(value))
 
-        return b"".join(bytes_)
+        return bytes_.getvalue()
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/types/Array.py` & `binary-file-parser-0.1.0/src/binary_file_parser/types/Array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 from __future__ import annotations
 
 import struct
 from typing import Type
 
 from binary_file_parser.types.ByteStream import ByteStream
 from binary_file_parser.types.Parseable import Parseable
+from binary_file_parser.types.RefList import RefList
+from binary_file_parser.utils import Version
 
 ParseableType = Type[Parseable] | Parseable
 
 class BaseArray(Parseable):
-    __slots__ = ("dtype", "struct_symbol", "length")
+    __slots__ = ("atype", "dtype", "struct_symbol", "length")
 
-    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str):
+    @property
+    def is_iterable(self) -> bool:
+        return True
+
+    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, atype: Type[RefList] = RefList):
         super().__init__(size)
         self.dtype = dtype
+        self.atype = atype
         self.struct_symbol = struct_symbol
         self.length = -1
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> list:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> list:
         ls = [None] * self.length
         for i in range(self.length):
-            ls[i] = self.dtype.from_stream(stream, struct_version = struct_version)
-        return ls
+            ls[i] = self.dtype.from_stream(stream, struct_ver = struct_ver)
+        return self.atype(ls)
 
-    def from_bytes(self, bytes_: bytes, *, struct_version: tuple[int, ...] = (0,)) -> list:
-        return self.from_stream(ByteStream.from_bytes(bytes_), struct_version = struct_version)
+    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> list:
+        return self.from_stream(ByteStream.from_bytes(bytes_), struct_ver = struct_ver)
 
     def to_bytes(self, value: list) -> bytes:
         ls = [b""]*self.length
         for i, val in enumerate(value):
             ls[i] = self.dtype.to_bytes(val)
         return b"".join(ls)
 
 
 class Array(BaseArray):
     __slots__ = ()
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> list:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> list:
         self.length = struct.unpack(self.struct_symbol, stream.get(self.size))[0]
-        return super().from_stream(stream, struct_version = struct_version)
+        return super().from_stream(stream, struct_ver = struct_ver)
 
     def to_bytes(self, value: list) -> bytes:
         self.length = len(value)
         length_bytes = struct.pack(self.struct_symbol, self.length)
         return length_bytes+super().to_bytes(value)
 
 class Array8(Array):
@@ -69,16 +76,16 @@
     def __class_getitem__(cls, item: ParseableType) -> Array64:
         return cls(8, item, '<Q')
 
 
 class FixedLenArray(BaseArray):
     __slots__ = ()
 
-    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, length: int):
-        super().__init__(size, dtype, struct_symbol)
+    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, length: int, atype: Type[RefList] = RefList):
+        super().__init__(size, dtype, struct_symbol, atype)
         self.length = length
 
     def is_valid(self, value: list) -> tuple[bool, str]:
         if len(value) == self.length:
             return True, ""
         return False, f"%s must have a fixed length of {value}"
 
@@ -91,40 +98,40 @@
     def __class_getitem__(cls, item: tuple[ParseableType, int]) -> FixedLenArray:
         return cls(4, item[0], '<I', item[1])
 
 
 class StackedArrays(BaseArray):
     __slots__ = "num_arrays"
 
-    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, num_arrays: int = -1):
-        super().__init__(size, dtype, struct_symbol)
+    def __init__(self, size: int, dtype: ParseableType, struct_symbol: str, num_arrays: int = -1, atype: Type[RefList] = RefList):
+        super().__init__(size, dtype, struct_symbol, atype)
         self.num_arrays = num_arrays
 
     def is_valid(self, value: list[list]) -> tuple[bool, str]:
         if self.num_arrays == -1:
             return True, ""
 
         num_arrays = len(value)
         if num_arrays == self.num_arrays:
             return True, ""
         return False, f"%s expected {self.num_arrays} but found {num_arrays} stacked arrays"
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> list[list]:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> list[list]:
         num_arrays = self.num_arrays
         if num_arrays == -1:
             num_arrays = struct.unpack(self.struct_symbol, stream.get(self.size))[0]
 
         lengths: list[int] = [struct.unpack(self.struct_symbol, stream.get(self.size))[0] for _ in range(num_arrays)]
         ls: list[list] = [[] for _ in range(num_arrays)]
 
         for i, length in enumerate(lengths):
             self.length = length
-            ls[i] = super().from_stream(stream, struct_version = struct_version)
+            ls[i] = super().from_stream(stream, struct_ver = struct_ver)
 
-        return ls
+        return self.atype(ls)
 
     def to_bytes(self, value: list[list]) -> bytes:
         valid, msg = self.is_valid(value)
         if not valid:
             raise TypeError(msg)
 
         length_bytes = b""
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/types/Bool.py` & `binary-file-parser-0.1.0/src/binary_file_parser/types/Bytes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import struct
+from __future__ import annotations
 
 from binary_file_parser.types.ByteStream import ByteStream
 from binary_file_parser.types.Parseable import Parseable
+from binary_file_parser.utils import Version
 
 
-class Bool(Parseable):
-    __slots__ = "struct_symbol"
+class Bytes(Parseable):
+    __slots__ = ()
 
-    def __init__(self, size: int, struct_symbol: str):
-        super().__init__(size)
-        self.struct_symbol = struct_symbol
-
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> bool:
-        return self.from_bytes(stream.get(self.size), struct_version = struct_version)
-
-    def from_bytes(self, bytes_: bytes, *, struct_version: tuple[int, ...] = (0,)) -> bool:
-        return not not struct.unpack(self.struct_symbol, bytes_)[0]
-
-    def to_bytes(self, value: bool) -> bytes:
-        return struct.pack(self.struct_symbol, 1 if value else 0)
-
-bool8 = Bool(1, "<B")
-bool16 = Bool(2, "<H")
-bool32 = Bool(4, "<I")
-bool64 = Bool(8, "<Q")
+    def is_valid(self, value: bytes) -> tuple[bool, str]:
+        if len(value) == self.size:
+            return True, ""
+        return False, f"number of bytes in %s must equal {self.size}"
+
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> bytes:
+        return stream.get(self.size)
+
+    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> bytes:
+        return bytes_
+
+    def to_bytes(self, value: bytes) -> bytes:
+        return value
+
+    def __class_getitem__(cls, item: int) -> Bytes:
+        return cls(item)
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/types/ByteStream.py` & `binary-file-parser-0.1.0/src/binary_file_parser/types/ByteStream.py`

 * *Files identical despite different names*

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/types/Bytes.py` & `binary-file-parser-0.1.0/src/binary_file_parser/types/Int.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-from __future__ import annotations
+import struct
 
 from binary_file_parser.types.ByteStream import ByteStream
 from binary_file_parser.types.Parseable import Parseable
+from binary_file_parser.utils import Version
 
 
-class Bytes(Parseable):
-    __slots__ = ()
+class Int(Parseable):
+    __slots__ = "struct_symbol"
 
-    def is_valid(self, value: bytes) -> tuple[bool, str]:
-        if len(value) == self.size:
-            return True, ""
-        return False, f"number of bytes in %s must equal {self.size}"
+    def __init__(self, size: int, struct_symbol: str):
+        super().__init__(size)
+        self.struct_symbol = struct_symbol
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> bytes:
-        return stream.get(self.size)
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> int:
+        return self.from_bytes(stream.get(self.size), struct_ver = struct_ver)
 
-    def from_bytes(self, bytes_: bytes, *, struct_version: tuple[int, ...] = (0,)) -> bytes:
-        return bytes_
+    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> int:
+        return struct.unpack(self.struct_symbol, bytes_)[0]
 
-    def to_bytes(self, value: bytes) -> bytes:
-        return value
+    def to_bytes(self, value: int) -> bytes:
+        return struct.pack(self.struct_symbol, value)
 
-    def __class_getitem__(cls, item: int) -> Bytes:
-        return cls(item)
+int8 = Int(1, "<b")
+int16 = Int(2, "<h")
+int32 = Int(4, "<i")
+int64 = Int(8, "<q")
+uint8 = Int(1, "<B")
+uint16 = Int(2, "<H")
+uint32 = Int(4, "<I")
+uint64 = Int(8, "<Q")
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/types/Float.py` & `binary-file-parser-0.1.0/src/binary_file_parser/types/Float.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import struct
 
 from binary_file_parser.types.ByteStream import ByteStream
 from binary_file_parser.types.Parseable import Parseable
+from binary_file_parser.utils import Version
 
 
 class Float(Parseable):
     __slots__ = "struct_symbol"
 
     def __init__(self, size: int, struct_symbol: str):
         super().__init__(size)
         self.struct_symbol = struct_symbol
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> float:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> float:
         return self.from_bytes(stream.get(self.size))
 
-    def from_bytes(self, bytes_: bytes, *, struct_version: tuple[int, ...] = (0,)) -> float:
+    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> float:
         return struct.unpack(self.struct_symbol, bytes_)[0]
 
     def to_bytes(self, value: float) -> bytes:
         return struct.pack(self.struct_symbol, value)
 
 float16 = Float(2, "e")
 float32 = Float(4, "f")
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/types/Str.py` & `binary-file-parser-0.1.0/src/binary_file_parser/types/Str.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import struct
 from abc import ABC
 
 from binary_file_parser.types.ByteStream import ByteStream
 from binary_file_parser.types.Parseable import Parseable
+from binary_file_parser.utils import Version
 
 
 class BaseStr(Parseable, ABC):
     __slots__ = ()
 
-    def from_bytes(self, bytes_: bytes, *, struct_version: tuple[int, ...] = (0,)) -> str:
+    def from_bytes(self, bytes_: bytes, *, struct_ver: Version = Version((0,))) -> str:
         try:
             return bytes_.decode("utf-8")
         except UnicodeDecodeError:
             return bytes_.decode("latin-1")
 
     def to_bytes(self, value: str) -> bytes:
         # TODO: plain bytes
@@ -25,15 +26,15 @@
 
         return bytes_
 
 
 class CStr(BaseStr):
     __slots__ = ()
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> str:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> str:
         bytes_ = b""
         while (byte := stream.get(1)) != b"\x00":
             bytes_ += byte
         return self.from_bytes(bytes_)
 
     def to_bytes(self, value: str) -> bytes:
         if not value.endswith("\x00"):
@@ -44,29 +45,29 @@
 class Str(BaseStr):
     __slots__ = "struct_symbol"
 
     def __init__(self, size: int, struct_symbol: str):
         super().__init__(size)
         self.struct_symbol = struct_symbol
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> str:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> str:
         length: int = struct.unpack(self.struct_symbol, stream.get(self.size))[0]
         return self.from_bytes(stream.get(length))
 
     def to_bytes(self, value: str) -> bytes:
         bytes_ = super().to_bytes(value)
         length = struct.pack(self.struct_symbol, len(bytes_))
         return length+bytes_
 
 
 class NullTermStr(Str):
     __slots__ = ()
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> str:
-        return super().from_stream(stream, struct_version = struct_version)[:-1]
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> str:
+        return super().from_stream(stream, struct_ver = struct_ver)[:-1]
 
     def to_bytes(self, value: str) -> bytes:
         if not value.endswith("\x00"):
             value += "\x00"
         return super().to_bytes(value)
 
 
@@ -78,15 +79,15 @@
         self.length = length
 
     def is_valid(self, value: str) -> tuple[bool, str]:
         if len(value) == self.length:
             return True, ""
         return False, f"%s must have a fixed length of {value}"
 
-    def from_stream(self, stream: ByteStream, *, struct_version: tuple[int, ...] = (0,)) -> str:
+    def from_stream(self, stream: ByteStream, *, struct_ver: Version = Version((0,))) -> str:
         return self.from_bytes(stream.get(self.length))
 
     def __class_getitem__(cls, item: int) -> FixedLenStr:
         return cls(4, item)
 
 c_str = CStr(4)
 str8 = Str(1, "<B")
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser/types/__init__.py` & `binary-file-parser-0.1.0/src/binary_file_parser/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,8 +3,9 @@
 )
 from .Bool import bool8, bool16, bool32, bool64
 from .Bytes import Bytes
 from .ByteStream import ByteStream
 from .Float import float16, float32, float64
 from .Int import int8, int16, int32, int64, uint8, uint16, uint32, uint64
 from .Parseable import Parseable
+from .RefList import RefList
 from .Str import c_str, str8, str16, str32, str64, nt_str8, nt_str16, nt_str32, nt_str64, FixedLenStr
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser.egg-info/PKG-INFO` & `binary-file-parser-0.1.0/src/binary_file_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-file-parser
-Version: 0.0.2
+Version: 0.1.0
 Summary: Read/Write binary files after describing their specifications in code (similar to an ORM table schema)
 Author-email: Divy1211 <divy1211.dc@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alian713
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/Divy1211/FileParser
+Project-URL: Homepage, https://github.com/Divy1211/BinaryFileParser
 Keywords: binary,file,parser
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -63,17 +63,17 @@
 
 ```py
 from binary_file_parser import BaseStruct, Retriever
 from binary_file_parser.types import int32, uint64, str32, FixedLenStr
 
 class Spam(BaseStruct):
     file_version: str = Retriever(FixedLenStr[4], default = 0)
-    creator_name: int = Retriever(str32, default = 0)
+    creator_name: str = Retriever(str32, default = 0)
     saved_timestamp: int = Retriever(uint64, default = 0)
-    eggs: str = Retriever(int32, default = 0)
+    eggs: int = Retriever(int32, default = 0)
 
 # read a binary file that has the above format
 file = Spam.from_file("path/to/file")
 
 # modify the creator name
 file.creator_name = "Alian713"
 file.eggs = 20
```

### Comparing `binary-file-parser-0.0.2/src/binary_file_parser.egg-info/SOURCES.txt` & `binary-file-parser-0.1.0/src/binary_file_parser.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/binary_file_parser/__init__.py
+src/binary_file_parser/utils.py
 src/binary_file_parser.egg-info/PKG-INFO
 src/binary_file_parser.egg-info/SOURCES.txt
 src/binary_file_parser.egg-info/dependency_links.txt
 src/binary_file_parser.egg-info/requires.txt
 src/binary_file_parser.egg-info/top_level.txt
 src/binary_file_parser/errors/CompressionError.py
 src/binary_file_parser/errors/ParsingError.py
 src/binary_file_parser/errors/VersionError.py
 src/binary_file_parser/errors/__init__.py
-src/binary_file_parser/retrievers/BaseStruct.py
 src/binary_file_parser/retrievers/MapValidate.py
+src/binary_file_parser/retrievers/RetreiverCombiner.py
+src/binary_file_parser/retrievers/RetreiverRef.py
 src/binary_file_parser/retrievers/Retriever.py
 src/binary_file_parser/retrievers/__init__.py
+src/binary_file_parser/retrievers/base_struct.py
 src/binary_file_parser/types/Array.py
 src/binary_file_parser/types/Bool.py
 src/binary_file_parser/types/ByteStream.py
 src/binary_file_parser/types/Bytes.py
 src/binary_file_parser/types/Float.py
 src/binary_file_parser/types/Int.py
 src/binary_file_parser/types/Parseable.py
+src/binary_file_parser/types/RefList.py
 src/binary_file_parser/types/Str.py
 src/binary_file_parser/types/__init__.py
```

