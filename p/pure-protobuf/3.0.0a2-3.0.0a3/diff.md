# Comparing `tmp/pure_protobuf-3.0.0a2.tar.gz` & `tmp/pure_protobuf-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_protobuf-3.0.0a2.tar", max compression
+gzip compressed data, was "pure_protobuf-3.0.0a3.tar", max compression
```

## Comparing `pure_protobuf-3.0.0a2.tar` & `pure_protobuf-3.0.0a3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1089 2023-04-25 11:49:12.039312 pure_protobuf-3.0.0a2/LICENSE
--rw-r--r--   0        0        0     3210 2023-04-25 11:49:12.039312 pure_protobuf-3.0.0a2/README.md
--rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/__init__.py
--rw-r--r--   0        0        0     2375 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/_accumulators.py
--rw-r--r--   0        0        0     1679 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/_mergers.py
--rw-r--r--   0        0        0     3239 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/annotations.py
--rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/descriptors/__init__.py
--rw-r--r--   0        0        0     4769 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/descriptors/_field.py
--rw-r--r--   0        0        0     7833 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/descriptors/record.py
--rw-r--r--   0        0        0      685 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/__init__.py
--rw-r--r--   0        0        0      211 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/_dataclasses.py
--rw-r--r--   0        0        0     1085 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/_typing.py
--rw-r--r--   0        0        0      441 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/datetime.py
--rw-r--r--   0        0        0      589 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/io.py
--rw-r--r--   0        0        0      635 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/itertools.py
--rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/__init__.py
--rw-r--r--   0        0        0      935 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_repr.py
--rw-r--r--   0        0        0      620 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_skip.py
--rw-r--r--   0        0        0      522 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_vars.py
--rw-r--r--   0        0        0      716 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/accumulate.py
--rw-r--r--   0        0        0      486 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/merge.py
--rw-r--r--   0        0        0      818 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/read.py
--rw-r--r--   0        0        0      402 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/write.py
--rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/__init__.py
--rw-r--r--   0        0        0     1420 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/bytes_.py
--rw-r--r--   0        0        0      269 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/fixed32.py
--rw-r--r--   0        0        0      250 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/fixed64.py
--rw-r--r--   0        0        0     1112 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/struct_.py
--rw-r--r--   0        0        0     1446 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/tag.py
--rw-r--r--   0        0        0      619 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/url.py
--rw-r--r--   0        0        0     4541 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/varint.py
--rw-r--r--   0        0        0     1204 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/wire_type.py
--rw-r--r--   0        0        0     4976 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/wrappers.py
--rw-r--r--   0        0        0     4576 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/message.py
--rw-r--r--   0        0        0     2376 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/one_of.py
--rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/py.typed
--rw-r--r--   0        0        0     3720 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/well_known.py
--rw-r--r--   0        0        0     3425 2023-04-25 11:49:29.247636 pure_protobuf-3.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 pure_protobuf-3.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-25 14:26:30.317963 pure_protobuf-3.0.0a3/LICENSE
+-rw-r--r--   0        0        0     3210 2023-04-25 14:26:30.317963 pure_protobuf-3.0.0a3/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/__init__.py
+-rw-r--r--   0        0        0     2375 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/_accumulators.py
+-rw-r--r--   0        0        0     1679 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/_mergers.py
+-rw-r--r--   0        0        0     3259 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/annotations.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/descriptors/__init__.py
+-rw-r--r--   0        0        0     4769 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/descriptors/_field.py
+-rw-r--r--   0        0        0     7833 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/descriptors/record.py
+-rw-r--r--   0        0        0      685 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/_dataclasses.py
+-rw-r--r--   0        0        0     1085 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/_typing.py
+-rw-r--r--   0        0        0      441 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/datetime.py
+-rw-r--r--   0        0        0      589 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/io.py
+-rw-r--r--   0        0        0      635 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/helpers/itertools.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/__init__.py
+-rw-r--r--   0        0        0      935 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_repr.py
+-rw-r--r--   0        0        0      620 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_skip.py
+-rw-r--r--   0        0        0      522 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_vars.py
+-rw-r--r--   0        0        0      716 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/accumulate.py
+-rw-r--r--   0        0        0      486 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/merge.py
+-rw-r--r--   0        0        0      818 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/read.py
+-rw-r--r--   0        0        0      402 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/interfaces/write.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/__init__.py
+-rw-r--r--   0        0        0     1420 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/bytes_.py
+-rw-r--r--   0        0        0      269 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/fixed32.py
+-rw-r--r--   0        0        0      250 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/fixed64.py
+-rw-r--r--   0        0        0     1112 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/struct_.py
+-rw-r--r--   0        0        0     1446 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/tag.py
+-rw-r--r--   0        0        0      619 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/url.py
+-rw-r--r--   0        0        0     4541 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/varint.py
+-rw-r--r--   0        0        0     1204 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/wire_type.py
+-rw-r--r--   0        0        0     4976 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/io/wrappers.py
+-rw-r--r--   0        0        0     5180 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/message.py
+-rw-r--r--   0        0        0     2376 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/one_of.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/py.typed
+-rw-r--r--   0        0        0     3720 2023-04-25 14:26:30.321963 pure_protobuf-3.0.0a3/pure_protobuf/well_known.py
+-rw-r--r--   0        0        0     3425 2023-04-25 14:26:48.458065 pure_protobuf-3.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 pure_protobuf-3.0.0a3/PKG-INFO
```

### Comparing `pure_protobuf-3.0.0a2/LICENSE` & `pure_protobuf-3.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/README.md` & `pure_protobuf-3.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/_accumulators.py` & `pure_protobuf-3.0.0a3/pure_protobuf/_accumulators.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/_mergers.py` & `pure_protobuf-3.0.0a3/pure_protobuf/_mergers.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/annotations.py` & `pure_protobuf-3.0.0a3/pure_protobuf/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Field annotations that may be used inside `Annotated`."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from sys import version_info
-from typing import TYPE_CHECKING, Any, NewType, Optional, Union
+from typing import TYPE_CHECKING, Any, ClassVar, NewType, Optional, Union
 
 from pure_protobuf.exceptions import IncorrectAnnotationError
 from pure_protobuf.helpers._dataclasses import SLOTS
 from pure_protobuf.helpers._typing import DEFAULT, Sentinel
 
 if version_info >= (3, 10):
     from dataclasses import KW_ONLY  # type: ignore[attr-defined]
@@ -26,15 +26,15 @@
     Specifies the field's number.
 
     See also:
         - https://developers.google.com/protocol-buffers/docs/proto3#assigning_field_numbers
     """
 
     if version_info >= (3, 10):
-        _: KW_ONLY
+        _: ClassVar[KW_ONLY]
 
     packed: Union[bool, Sentinel] = DEFAULT
     """Specifies whether the field should be packed in its serialized representation."""
 
     one_of: Optional[OneOf] = None
     """Specifies a one-of group for this field."""
```

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/descriptors/_field.py` & `pure_protobuf-3.0.0a3/pure_protobuf/descriptors/_field.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/descriptors/record.py` & `pure_protobuf-3.0.0a3/pure_protobuf/descriptors/record.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/exceptions.py` & `pure_protobuf-3.0.0a3/pure_protobuf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/helpers/_typing.py` & `pure_protobuf-3.0.0a3/pure_protobuf/helpers/_typing.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/helpers/io.py` & `pure_protobuf-3.0.0a3/pure_protobuf/helpers/io.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/helpers/itertools.py` & `pure_protobuf-3.0.0a3/pure_protobuf/helpers/itertools.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_repr.py` & `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_repr.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_skip.py` & `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_skip.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_vars.py` & `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/_vars.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/accumulate.py` & `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/accumulate.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/read.py` & `pure_protobuf-3.0.0a3/pure_protobuf/interfaces/read.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/io/bytes_.py` & `pure_protobuf-3.0.0a3/pure_protobuf/io/bytes_.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/io/struct_.py` & `pure_protobuf-3.0.0a3/pure_protobuf/io/struct_.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/io/tag.py` & `pure_protobuf-3.0.0a3/pure_protobuf/io/tag.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/io/url.py` & `pure_protobuf-3.0.0a3/pure_protobuf/io/url.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/io/varint.py` & `pure_protobuf-3.0.0a3/pure_protobuf/io/varint.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/io/wire_type.py` & `pure_protobuf-3.0.0a3/pure_protobuf/io/wire_type.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/io/wrappers.py` & `pure_protobuf-3.0.0a3/pure_protobuf/io/wrappers.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/message.py` & `pure_protobuf-3.0.0a3/pure_protobuf/message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from abc import ABC
+from io import BytesIO
 from typing import IO, Any, ClassVar, Dict, Tuple
 
 from typing_extensions import Self
 
 try:
     from inspect import get_annotations  # type: ignore[attr-defined]
 except ImportError:
@@ -88,23 +89,44 @@
                 # Possibly update the one-of field.
                 one_of = descriptor.one_of
                 if one_of is not None:
                     one_of._keep_values(values, descriptor.number)
 
         return cls(**values)
 
+    @classmethod
+    def loads(cls, buffer: bytes) -> Self:
+        """
+        Read a message from the buffer.
+
+        This is functionally the same as calling `read_from(BytesIO(buffer))`.
+        """
+        return cls.read_from(BytesIO(buffer))
+
     def write_to(self, io: IO[bytes]) -> None:
         """Write the message to the file."""
         for _, (name, descriptor) in self.__PROTOBUF_FIELDS_BY_NUMBER__.items():
             descriptor.write(getattr(self, name), io)
 
     def __bytes__(self) -> bytes:
-        """Convert the message to a bytestring."""
+        """
+        Convert the message to a bytestring.
+
+        This is functionally the same as calling `dumps()` or `write_to(BytesIO(…))`.
+        """
         return to_bytes(BaseMessage.write_to, self)
 
+    def dumps(self) -> bytes:
+        """
+        Convert the message to a bytestring.
+
+        This is functionally the same as calling `bytes(message)` or `write_to(BytesIO(…))`.
+        """
+        return bytes(self)
+
     def __setattr__(self, name: str, value: Any) -> None:  # noqa: D105
         super().__setattr__(name, value)
         descriptor = self.__PROTOBUF_FIELDS_BY_NAME__[name]
         one_of = descriptor.one_of
         if one_of is not None:
             one_of._keep_attribute(self, descriptor.number)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/one_of.py` & `pure_protobuf-3.0.0a3/pure_protobuf/one_of.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pure_protobuf/well_known.py` & `pure_protobuf-3.0.0a3/pure_protobuf/well_known.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a2/pyproject.toml` & `pure_protobuf-3.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "Protocol Buffers using Python type annotations"
 keywords = ["protobuf", "protocol-buffers"]
 license = "MIT"
 name = "pure-protobuf"
 readme = "README.md"
 repository = "https://github.com/eigenein/protobuf"
-version = "3.0.0a2"
+version = "3.0.0a3"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `pure_protobuf-3.0.0a2/PKG-INFO` & `pure_protobuf-3.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-protobuf
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: Protocol Buffers using Python type annotations
 Home-page: https://github.com/eigenein/protobuf
 License: MIT
 Keywords: protobuf,protocol-buffers
 Author: Pavel Perestoronin
 Author-email: eigenein@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
```

