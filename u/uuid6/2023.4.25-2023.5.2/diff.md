# Comparing `tmp/uuid6-2023.4.25.tar.gz` & `tmp/uuid6-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuid6-2023.4.25.tar", last modified: Tue Apr 25 10:03:57 2023, max compression
+gzip compressed data, was "uuid6-2023.5.2.tar", last modified: Tue May  2 09:34:22 2023, max compression
```

## Comparing `uuid6-2023.4.25.tar` & `uuid6-2023.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-25 10:03:43.000000 uuid6-2023.4.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-25 10:03:57.554544 uuid6-2023.4.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-25 10:03:43.000000 uuid6-2023.4.25/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 10:03:43.000000 uuid6-2023.4.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:03:57.554544 uuid6-2023.4.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-25 10:03:43.000000 uuid6-2023.4.25/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.550544 uuid6-2023.4.25/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/src/uuid6/
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-25 10:03:43.000000 uuid6-2023.4.25/src/uuid6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:43.000000 uuid6-2023.4.25/src/uuid6/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/src/uuid6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-25 10:03:43.000000 uuid6-2023.4.25/test/test_uuid6.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-25 10:03:43.000000 uuid6-2023.4.25/test/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:34:21.995131 uuid6-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 09:34:10.000000 uuid6-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-02 09:34:21.995131 uuid6-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-05-02 09:34:10.000000 uuid6-2023.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 09:34:10.000000 uuid6-2023.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:34:21.995131 uuid6-2023.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-02 09:34:10.000000 uuid6-2023.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:34:21.995131 uuid6-2023.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:34:21.995131 uuid6-2023.5.2/src/uuid6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-02 09:34:10.000000 uuid6-2023.5.2/src/uuid6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:34:10.000000 uuid6-2023.5.2/src/uuid6/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:34:21.995131 uuid6-2023.5.2/src/uuid6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-02 09:34:21.000000 uuid6-2023.5.2/src/uuid6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 09:34:21.000000 uuid6-2023.5.2/src/uuid6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:34:21.000000 uuid6-2023.5.2/src/uuid6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:34:21.000000 uuid6-2023.5.2/src/uuid6.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 09:34:21.000000 uuid6-2023.5.2/src/uuid6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:34:21.995131 uuid6-2023.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-02 09:34:10.000000 uuid6-2023.5.2/test/test_uuid6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-02 09:34:10.000000 uuid6-2023.5.2/test/test_vectors.py
```

### Comparing `uuid6-2023.4.25/LICENSE` & `uuid6-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uuid6-2023.4.25/PKG-INFO` & `uuid6-2023.5.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: uuid6
-Version: 2023.4.25
-Summary: New time-based UUID formats which are suited for use as a database key
-Home-page: https://github.com/oittaa/uuid6-python
-Author: Oittaa
-Author-email: 
-Keywords: uuid,uuid6,uuid7,uuid8,uuidv6,uuidv7,uuidv8
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # uuid6
 New time-based UUID formats which are suited for use as a database key.
 
 [![CI](https://github.com/oittaa/uuid6-python/actions/workflows/main.yml/badge.svg)](https://github.com/oittaa/uuid6-python/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/oittaa/uuid6-python/branch/main/graph/badge.svg?token=O59DZ6UWQV)](https://codecov.io/gh/oittaa/uuid6-python)
 [![PyPI status](https://badge.fury.io/py/uuid6.svg)](https://pypi.org/project/uuid6/)
 [![Python versions supported](https://img.shields.io/pypi/pyversions/uuid6.svg?logo=python)](https://pypi.org/project/uuid6/)
@@ -36,54 +14,85 @@
 ```shell
 pip install uuid6
 ```
 
 ## Usage
 
 ```python
-from uuid6 import uuid6, uuid7, uuid8
+import uuid6
 
-my_uuid = uuid6()
+my_uuid = uuid6.uuid6()
 print(my_uuid)
-assert my_uuid < uuid6()
+assert my_uuid < uuid6.uuid6()
 
-my_uuid = uuid7()
+my_uuid = uuid6.uuid7()
 print(my_uuid)
-assert my_uuid < uuid7()
+assert my_uuid < uuid6.uuid7()
 
-my_uuid = uuid8()
+my_uuid = uuid6.uuid8()
 print(my_uuid)
-assert my_uuid < uuid8()
+assert my_uuid < uuid6.uuid8()
+
+import uuid
+
+my_uuid = uuid.UUID(hex="C232AB00-9414-11EC-B3C8-9E6BDECED846")
+assert uuid6.uuid1_to_uuid6(my_uuid) == uuid.UUID(hex="1EC9414C-232A-6B00-B3C8-9E6BDECED846")
 ```
 
 ## Which UUID version should I use?
 
 > Implementations SHOULD utilize UUID version 7 over UUID version 1 and 6 if possible.
 
 UUID version 7 features a time-ordered value field derived from the widely implemented and well known Unix Epoch timestamp source, the number of milliseconds since midnight 1 Jan 1970 UTC, leap seconds excluded. As well as improved entropy characteristics over versions 1 or 6.
 
 If your use case requires greater granularity than UUID version 7 can provide, you might consider UUID version 8. UUID version 8 doesn't provide as good entropy characteristics as UUID version 7, but it utilizes timestamp with nanosecond level of precision.
 
-## UUIDv6 Field and Bit Layout
+## Functions
+
+### uuid6.uuid1_to_uuid6(*uuid1*)
+
+Generate a UUID version 6 object from a UUID version 1 object.
+
+### uuid6.uuid6(*node=None*, *clock_seq=None*)
+
+Generate a UUID from a host ID, sequence number, and the current time. If *node* is not given, a random 48-bit number is chosen. If *clock_seq* is given, it is used as the sequence number; otherwise a random 14-bit sequence number is chosen.
+
+### uuid6.uuid7()
+
+Generate a UUID from a random number, and the current time.
+
+### uuid6.uuid8()
+
+Generate a UUID from a random number, and the current time.
+
+## UUID Version 6
+
+UUID version 6 is a field-compatible version of UUIDv1, reordered for improved DB locality. It is expected that UUIDv6 will primarily be used in contexts where there are existing v1 UUIDs. Systems that do not involve legacy UUIDv1 **SHOULD** use UUIDv7 instead.
+
+### UUIDv6 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           time_high                           |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-        |           time_mid            |      time_low_and_version     |
+        |           time_mid            |  ver  |       time_low        |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-        |clk_seq_hi_res |  clk_seq_low  |         node (0-1)            |
+        |var|         clock_seq         |             node              |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-        |                         node (2-5)                            |
+        |                              node                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
-## UUIDv7 Field and Bit Layout
+## UUID Version 7
+
+UUID version 7 features a time-ordered value field derived from the widely implemented and well known Unix Epoch timestamp source, the number of milliseconds seconds since midnight 1 Jan 1970 UTC, leap seconds excluded. UUID version 7 also has improved entropy characteristics over versions 1 or 6.
+
+### UUIDv7 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
@@ -91,15 +100,21 @@
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |var|                        rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                            rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
-## UUIDv8 Field and Bit Layout
+## UUID Version 8
+
+UUID version 8 provides an RFC-compatible format for experimental or vendor-specific use cases.
+
+This implementation of `uuid8()` sacrifices some entropy for granularity compared to `uuid7()`, while being otherwise compatible.
+
+### UUIDv8 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
```

### Comparing `uuid6-2023.4.25/setup.py` & `uuid6-2023.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `uuid6-2023.4.25/src/uuid6/__init__.py` & `uuid6-2023.5.2/src/uuid6/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,45 +74,58 @@
     return -(-value * 10**6 // 2**20)
 
 
 def _subsec_encode(value: int) -> int:
     return value * 2**20 // 10**6
 
 
+def uuid1_to_uuid6(uuid1: uuid.UUID) -> UUID:
+    r"""Generate a UUID version 6 object from a UUID version 1 object."""
+    if uuid1.version != 1:
+        raise ValueError("given UUID's version number must be 1")
+    h = uuid1.hex
+    h = h[13:16] + h[8:12] + h[0:5] + "6" + h[5:8] + h[16:]
+    return UUID(hex=h, is_safe=uuid1.is_safe)
+
+
 _last_v6_timestamp = None
 _last_v7_timestamp = None
 _last_v8_timestamp = None
 
 
-def uuid6(clock_seq: Optional[int] = None) -> UUID:
+def uuid6(node: Optional[int] = None, clock_seq: Optional[int] = None) -> UUID:
     r"""UUID version 6 is a field-compatible version of UUIDv1, reordered for
     improved DB locality. It is expected that UUIDv6 will primarily be
     used in contexts where there are existing v1 UUIDs. Systems that do
     not involve legacy UUIDv1 SHOULD consider using UUIDv7 instead.
 
+    If 'node' is not given, a random 48-bit number is chosen.
+
     If 'clock_seq' is given, it is used as the sequence number;
     otherwise a random 14-bit sequence number is chosen."""
 
     global _last_v6_timestamp
 
     nanoseconds = time.time_ns()
     # 0x01b21dd213814000 is the number of 100-ns intervals between the
     # UUID epoch 1582-10-15 00:00:00 and the Unix epoch 1970-01-01 00:00:00.
     timestamp = nanoseconds // 100 + 0x01B21DD213814000
     if _last_v6_timestamp is not None and timestamp <= _last_v6_timestamp:
         timestamp = _last_v6_timestamp + 1
     _last_v6_timestamp = timestamp
     if clock_seq is None:
         clock_seq = secrets.randbits(14)  # instead of stable storage
+    if node is None:
+        node = secrets.randbits(48)
     time_high_and_time_mid = (timestamp >> 12) & 0xFFFFFFFFFFFF
     time_low_and_version = timestamp & 0x0FFF
     uuid_int = time_high_and_time_mid << 80
     uuid_int |= time_low_and_version << 64
     uuid_int |= (clock_seq & 0x3FFF) << 48
-    uuid_int |= secrets.randbits(48)
+    uuid_int |= node & 0xFFFFFFFFFFFF
     return UUID(int=uuid_int, version=6)
 
 
 def uuid7() -> UUID:
     r"""UUID version 7 features a time-ordered value field derived from the
     widely implemented and well known Unix Epoch timestamp source, the
     number of milliseconds since midnight 1 Jan 1970 UTC, leap seconds
```

### Comparing `uuid6-2023.4.25/src/uuid6.egg-info/PKG-INFO` & `uuid6-2023.5.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uuid6
-Version: 2023.4.25
+Version: 2023.5.2
 Summary: New time-based UUID formats which are suited for use as a database key
 Home-page: https://github.com/oittaa/uuid6-python
 Author: Oittaa
 Author-email: 
 Keywords: uuid,uuid6,uuid7,uuid8,uuidv6,uuidv7,uuidv8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -36,54 +36,85 @@
 ```shell
 pip install uuid6
 ```
 
 ## Usage
 
 ```python
-from uuid6 import uuid6, uuid7, uuid8
+import uuid6
 
-my_uuid = uuid6()
+my_uuid = uuid6.uuid6()
 print(my_uuid)
-assert my_uuid < uuid6()
+assert my_uuid < uuid6.uuid6()
 
-my_uuid = uuid7()
+my_uuid = uuid6.uuid7()
 print(my_uuid)
-assert my_uuid < uuid7()
+assert my_uuid < uuid6.uuid7()
 
-my_uuid = uuid8()
+my_uuid = uuid6.uuid8()
 print(my_uuid)
-assert my_uuid < uuid8()
+assert my_uuid < uuid6.uuid8()
+
+import uuid
+
+my_uuid = uuid.UUID(hex="C232AB00-9414-11EC-B3C8-9E6BDECED846")
+assert uuid6.uuid1_to_uuid6(my_uuid) == uuid.UUID(hex="1EC9414C-232A-6B00-B3C8-9E6BDECED846")
 ```
 
 ## Which UUID version should I use?
 
 > Implementations SHOULD utilize UUID version 7 over UUID version 1 and 6 if possible.
 
 UUID version 7 features a time-ordered value field derived from the widely implemented and well known Unix Epoch timestamp source, the number of milliseconds since midnight 1 Jan 1970 UTC, leap seconds excluded. As well as improved entropy characteristics over versions 1 or 6.
 
 If your use case requires greater granularity than UUID version 7 can provide, you might consider UUID version 8. UUID version 8 doesn't provide as good entropy characteristics as UUID version 7, but it utilizes timestamp with nanosecond level of precision.
 
-## UUIDv6 Field and Bit Layout
+## Functions
+
+### uuid6.uuid1_to_uuid6(*uuid1*)
+
+Generate a UUID version 6 object from a UUID version 1 object.
+
+### uuid6.uuid6(*node=None*, *clock_seq=None*)
+
+Generate a UUID from a host ID, sequence number, and the current time. If *node* is not given, a random 48-bit number is chosen. If *clock_seq* is given, it is used as the sequence number; otherwise a random 14-bit sequence number is chosen.
+
+### uuid6.uuid7()
+
+Generate a UUID from a random number, and the current time.
+
+### uuid6.uuid8()
+
+Generate a UUID from a random number, and the current time.
+
+## UUID Version 6
+
+UUID version 6 is a field-compatible version of UUIDv1, reordered for improved DB locality. It is expected that UUIDv6 will primarily be used in contexts where there are existing v1 UUIDs. Systems that do not involve legacy UUIDv1 **SHOULD** use UUIDv7 instead.
+
+### UUIDv6 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           time_high                           |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-        |           time_mid            |      time_low_and_version     |
+        |           time_mid            |  ver  |       time_low        |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-        |clk_seq_hi_res |  clk_seq_low  |         node (0-1)            |
+        |var|         clock_seq         |             node              |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
-        |                         node (2-5)                            |
+        |                              node                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
-## UUIDv7 Field and Bit Layout
+## UUID Version 7
+
+UUID version 7 features a time-ordered value field derived from the widely implemented and well known Unix Epoch timestamp source, the number of milliseconds seconds since midnight 1 Jan 1970 UTC, leap seconds excluded. UUID version 7 also has improved entropy characteristics over versions 1 or 6.
+
+### UUIDv7 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
@@ -91,15 +122,21 @@
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |var|                        rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                            rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
-## UUIDv8 Field and Bit Layout
+## UUID Version 8
+
+UUID version 8 provides an RFC-compatible format for experimental or vendor-specific use cases.
+
+This implementation of `uuid8()` sacrifices some entropy for granularity compared to `uuid7()`, while being otherwise compatible.
+
+### UUIDv8 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
```

### Comparing `uuid6-2023.4.25/test/test_uuid6.py` & `uuid6-2023.5.2/test/test_uuid6.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from time import time_ns
 from unittest.mock import patch
 from uuid import uuid1
 
-from uuid6 import UUID, uuid6, uuid7, uuid8
+from uuid6 import UUID, uuid6, uuid7, uuid8, uuid1_to_uuid6
 
 REGEX_UUID6 = r"^[0-9a-f]{8}-[0-9a-f]{4}-6[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}$"
 REGEX_UUID7 = r"^[0-9a-f]{8}-[0-9a-f]{4}-7[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}$"
 REGEX_UUID8 = r"^[0-9a-f]{8}-[0-9a-f]{4}-8[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}$"
 YEAR_IN_NS = 3600 * 24 * 36525 * 10**7
 
 
@@ -35,14 +35,27 @@
         self.assertEqual(uuid8_1.version, 8)
         for _ in range(1000):
             self.assertRegex(str(uuid8_1), REGEX_UUID8)
             uuid8_2 = uuid8()
             self.assertLess(uuid8_1, uuid8_2)
             uuid8_1 = uuid8_2
 
+    def test_uuid1_to_uuid6_generation(self):
+        uuid6_1 = None
+        for _ in range(1000):
+            uuid_1 = uuid1()
+            uuid6_2 = uuid1_to_uuid6(uuid_1)
+            self.assertEqual(uuid6_2.version, 6)
+            self.assertEqual(uuid6_2.node, uuid_1.node)
+            self.assertEqual(uuid6_2.clock_seq, uuid_1.clock_seq)
+            self.assertEqual(uuid6_2.time, uuid_1.time)
+            if uuid6_1 is not None:
+                self.assertLess(uuid6_1, uuid6_2)
+            uuid6_1 = uuid6_2
+
     def test_invalid_int(self):
         with self.assertRaises(ValueError):
             _ = UUID(int=-1)
         with self.assertRaises(ValueError):
             _ = UUID(int=1 << 128)
 
     def test_valid_int(self):
@@ -151,10 +164,14 @@
         uuid_8 = UUID(hex="ffffffff-ffff-8fff-bfff-ffffffffffff")
         self.assertEqual(uuid_8.time, 281474976710656000000)
 
     def test_multiple_arguments(self):
         with self.assertRaises(TypeError):
             _ = UUID(int=0, hex="061d0edc-bea0-75cc-9892-f6295fd7d295")
 
+    def test_convert_invalid_version(self):
+        with self.assertRaises(ValueError):
+            _ = uuid1_to_uuid6(uuid7())
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `uuid6-2023.4.25/test/test_vectors.py` & `uuid6-2023.5.2/test/test_vectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Unix_64_bit_ns = 0x16D6320C3D4DCC00 or 1645557742000000000
 """
 
 
 import unittest
 from unittest.mock import patch
 
-from uuid6 import UUID, uuid6, uuid7, uuid8
+from uuid6 import UUID, uuid6, uuid7, uuid8, uuid1_to_uuid6
 
 
 class TestVectors6(unittest.TestCase):
     """
     -------------------------------------------
     field       bits value
     -------------------------------------------
@@ -40,26 +40,30 @@
             | 0x3C8 << 48
             | 0x9E6BDECED846
         )
         uuid_6 = UUID(int=uuid_int, version=6)
         self.assertEqual(str(uuid_6), "1ec9414c-232a-6b00-b3c8-9e6bdeced846")
 
     @patch("uuid6._last_v6_timestamp", 1)
-    @patch("secrets.randbits", return_value=0x9E6BDECED846)
     @patch("time.time_ns", return_value=0x16D6320C3D4DCC00)
-    def test_uuid6_hex_from_time(self, mocktime, mockrand):
-        uuid_6 = uuid6(0x3C8 | int("11", 2) << 12)
+    def test_uuid6_hex_from_time(self, mocktime):
+        uuid_6 = uuid6(node=0x9E6BDECED846, clock_seq=0x3C8 | int("11", 2) << 12)
         self.assertEqual(str(uuid_6), "1ec9414c-232a-6b00-b3c8-9e6bdeced846")
 
     def test_uuid6_time_from_hex(self):
         uuid_6 = UUID(hex="1EC9414C-232A-6B00-B3C8-9E6BDECED846")
         self.assertEqual(uuid_6.time, 138648505420000000)
         uuid_1 = UUID(hex="C232AB00-9414-11EC-B3C8-9E6BDECED846")
         self.assertEqual(uuid_6.time, uuid_1.time)
 
+    def test_uuid1_to_uuid6(self):
+        uuid_1 = UUID(hex="C232AB00-9414-11EC-B3C8-9E6BDECED846")
+        uuid_6 = uuid1_to_uuid6(uuid_1)
+        self.assertEqual(str(uuid_6), "1ec9414c-232a-6b00-b3c8-9e6bdeced846")
+
 
 class TestVectors7(unittest.TestCase):
     """
     -------------------------------------------
     field       bits value
     -------------------------------------------
     unix_ts_ms  48   0x17F22E279B0
```

