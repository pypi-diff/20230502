# Comparing `tmp/charmonium_cache-1.3.0.tar.gz` & `tmp/charmonium_cache-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmonium_cache-1.3.0.tar", max compression
+gzip compressed data, was "charmonium_cache-1.4.0.tar", max compression
```

## Comparing `charmonium_cache-1.3.0.tar` & `charmonium_cache-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1070 2022-04-12 17:37:30.292399 charmonium_cache-1.3.0/LICENSE
--rw-r--r--   0        0        0     6708 2022-04-21 19:07:51.330085 charmonium_cache-1.3.0/README.rst
--rw-r--r--   0        0        0     1195 2023-03-10 06:37:57.298612 charmonium_cache-1.3.0/charmonium/cache/__init__.py
--rw-r--r--   0        0        0     3757 2023-03-10 06:37:57.298612 charmonium_cache-1.3.0/charmonium/cache/helpers.py
--rw-r--r--   0        0        0     4957 2023-03-09 23:49:14.286692 charmonium_cache-1.3.0/charmonium/cache/index.py
--rw-r--r--   0        0        0    28536 2023-03-10 08:49:30.840879 charmonium_cache-1.3.0/charmonium/cache/memoize.py
--rw-r--r--   0        0        0     3136 2023-03-10 06:37:57.298612 charmonium_cache-1.3.0/charmonium/cache/obj_store.py
--rw-r--r--   0        0        0     1424 2023-03-10 06:37:57.298612 charmonium_cache-1.3.0/charmonium/cache/pathlike.py
--rw-r--r--   0        0        0      299 2023-03-09 23:49:13.802689 charmonium_cache-1.3.0/charmonium/cache/pickler.py
--rw-r--r--   0        0        0        0 2021-04-24 04:31:41.136000 charmonium_cache-1.3.0/charmonium/cache/py.typed
--rw-r--r--   0        0        0     3483 2023-03-10 06:37:57.298612 charmonium_cache-1.3.0/charmonium/cache/replacement_policies.py
--rw-r--r--   0        0        0     2161 2023-03-10 06:37:57.298612 charmonium_cache-1.3.0/charmonium/cache/rw_lock.py
--rw-r--r--   0        0        0     4029 2023-03-10 06:37:57.298612 charmonium_cache-1.3.0/charmonium/cache/util.py
--rw-r--r--   0        0        0     3500 2023-03-10 08:49:30.840879 charmonium_cache-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7772 1970-01-01 00:00:00.000000 charmonium_cache-1.3.0/setup.py
--rw-r--r--   0        0        0     8034 1970-01-01 00:00:00.000000 charmonium_cache-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-04-12 17:37:30.292399 charmonium_cache-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6708 2022-04-21 19:07:51.330085 charmonium_cache-1.4.0/README.rst
+-rw-r--r--   0        0        0     1036 2023-05-02 03:56:11.160962 charmonium_cache-1.4.0/charmonium/cache/__init__.py
+-rw-r--r--   0        0        0     3757 2023-03-10 06:37:57.298612 charmonium_cache-1.4.0/charmonium/cache/helpers.py
+-rw-r--r--   0        0        0     5259 2023-04-17 15:48:47.840475 charmonium_cache-1.4.0/charmonium/cache/index.py
+-rw-r--r--   0        0        0    29512 2023-05-02 04:12:37.832131 charmonium_cache-1.4.0/charmonium/cache/memoize.py
+-rw-r--r--   0        0        0     3496 2023-04-17 15:49:19.692444 charmonium_cache-1.4.0/charmonium/cache/obj_store.py
+-rw-r--r--   0        0        0     1424 2023-03-10 06:37:57.298612 charmonium_cache-1.4.0/charmonium/cache/pathlike.py
+-rw-r--r--   0        0        0      299 2023-03-09 23:49:13.802689 charmonium_cache-1.4.0/charmonium/cache/pickler.py
+-rw-r--r--   0        0        0        0 2021-04-24 04:31:41.136000 charmonium_cache-1.4.0/charmonium/cache/py.typed
+-rw-r--r--   0        0        0     3483 2023-03-10 06:37:57.298612 charmonium_cache-1.4.0/charmonium/cache/replacement_policies.py
+-rw-r--r--   0        0        0     2161 2023-03-10 06:37:57.298612 charmonium_cache-1.4.0/charmonium/cache/rw_lock.py
+-rw-r--r--   0        0        0     4029 2023-03-10 06:37:57.298612 charmonium_cache-1.4.0/charmonium/cache/util.py
+-rw-r--r--   0        0        0     3470 2023-05-02 04:12:37.832131 charmonium_cache-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8034 1970-01-01 00:00:00.000000 charmonium_cache-1.4.0/PKG-INFO
```

### Comparing `charmonium_cache-1.3.0/LICENSE` & `charmonium_cache-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `charmonium_cache-1.3.0/README.rst` & `charmonium_cache-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `charmonium_cache-1.3.0/charmonium/cache/helpers.py` & `charmonium_cache-1.4.0/charmonium/cache/helpers.py`

 * *Files identical despite different names*

### Comparing `charmonium_cache-1.3.0/charmonium/cache/index.py` & `charmonium_cache-1.4.0/charmonium/cache/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import enum
-from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar, cast
+from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar, cast, Union
 
 
 class IndexKeyType(enum.IntEnum):
     MATCH = 0
     LOOKUP = 1
 
 
 Key = TypeVar("Key")
 Val = TypeVar("Val")
+_T = TypeVar("_T")
 
 
 class Index(Generic[Key, Val]):
     def __init__(
         self,
         schema: tuple[IndexKeyType, ...],
         deleter: Optional[Callable[[tuple[tuple[Key, ...], Val]], None]] = None,
@@ -117,14 +118,22 @@
         result = self._get_last_level(keys)
         if result:
             last_level, last_key, _ = result
             return last_level[last_key]
         else:
             raise KeyError(keys)
 
+    def get(self, keys: tuple[Key, ...], default: _T) -> Union[Val, _T]:
+        result = self._get_last_level(keys)
+        if result:
+            last_level, last_key, _ = result
+            return last_level.get(last_key, default)
+        else:
+            return default
+
     def __contains__(self, keys: tuple[Key, ...]) -> bool:
         if len(keys) != len(self.schema):
             raise ValueError(
                 f"Keys {keys} should be the same len as schema ({len(self.schema)})"
             )
         result = self._get_last_level(keys)
         if result:
```

### Comparing `charmonium_cache-1.3.0/charmonium/cache/memoize.py` & `charmonium_cache-1.4.0/charmonium/cache/memoize.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Tuple,
     Type,
     Union,
     cast,
 )
 
 import bitmath  # type: ignore
-from charmonium.freeze import freeze, global_config
+from charmonium.freeze import freeze, Config as FreezeConfig, global_config
 
 from .index import Index, IndexKeyType
 from .obj_store import DirObjStore, ObjStore
 from .pickler import Pickler
 from .replacement_policies import REPLACEMENT_POLICIES, Entry, ReplacementPolicy
 from .rw_lock import FileRWLock, Lock, RWLock
 from .util import (
@@ -43,56 +43,44 @@
     GetAttr,
     identity,
     none_tuple,
 )
 
 BYTE_ORDER: str = "big"
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
-freeze_config = copy.deepcopy(global_config)
-freeze_config.use_hash = True
-freeze_config.ignore_classes.update(
+DEFAULT_FREEZE_CONFIG = copy.deepcopy(global_config)
+DEFAULT_FREEZE_CONFIG.use_hash = True
+DEFAULT_FREEZE_CONFIG.ignore_classes.update(
     {
         ("charmonium.cache.memoize", "Memoized"),
         ("charmonium.cache.memoize", "MemoizedGroup"),
     }
 )
-freeze_config.ignore_attributes.update(
+DEFAULT_FREEZE_CONFIG.ignore_attributes.update(
     {
         ("charmonium.cache.memoize", "Memoized", "group"),
         ("charmonium.cache.memoize", "Memoized", "_use_obj_store"),
         ("charmonium.cache.memoize", "Memoized", "_use_metadata_size"),
         ("charmonium.cache.memoize", "Memoized", "_my_pickler"),
         ("charmonium.cache.memoize", "Memoized", "_extra_func_state"),
     }
 )
 
 
 def memoize(
-    *,
-    disable: Union[str, bool, None] = None,
     **kwargs: Any,
 ) -> Callable[[Callable[FuncParams, FuncReturn]], Memoized[FuncParams, FuncReturn]]:
     """See :py:class:`charmonium.cache.Memoized`."""
-    real_disable = (
-        disable
-        if isinstance(disable, bool)
-        else bool(int(os.environ.get("CHARMONIUM_CACHE_DISABLE", "0")))
-    )
-    if real_disable:
-        # TODO: use a multiple dispatch type signature here.
-        # This should just be Callable[FuncParams, FuncReturn]
-        return lambda x: x  # type: ignore
-    else:
-        def actual_memoize(
-            func: Callable[FuncParams, FuncReturn]
-        ) -> Memoized[FuncParams, FuncReturn]:
-            return Memoized[FuncParams, FuncReturn](func, **kwargs)
-        return actual_memoize
+    def actual_memoize(
+        func: Callable[FuncParams, FuncReturn]
+    ) -> Memoized[FuncParams, FuncReturn]:
+        return Memoized[FuncParams, FuncReturn](func, **kwargs)
+    return actual_memoize
 
 
 DEFAULT_LOCK_PATH = ".cache/.lock"
 DEFAULT_OBJ_STORE_PATH = ".cache"
 
 
 ops_logger = logging.getLogger("charmonium.cache.ops")
@@ -104,25 +92,25 @@
 if perf_logger_file:
     perf_logger.setLevel(logging.DEBUG)
     perf_logger.addHandler(logging.FileHandler(perf_logger_file))
     perf_logger.propagate = False
 
 
 @contextlib.contextmanager
-def perf_ctx(event: str, **kwargs: Any) -> Generator[None, None, None]:
+def perf_ctx(event: str, call_id: int) -> Generator[None, None, None]:
     if perf_logger.isEnabledFor(logging.DEBUG):
         start = datetime.datetime.now()
     yield
     if perf_logger.isEnabledFor(logging.DEBUG):
         perf_logger.debug(
             json.dumps(
                 {
                     "event": event,
                     "duration": (datetime.datetime.now() - start).total_seconds(),
-                    **kwargs,
+                    "call_id": call_id,
                 }
             )
         )
 
 
 @dataclasses.dataclass
 class MemoizedGroup:
@@ -164,39 +152,41 @@
                 IndexKeyType.LOOKUP,  # args key
                 IndexKeyType.MATCH,  # args version
             ),
             self._deleter,
         )
         self._version = 0
         self._memory_lock = threading.RLock()
-        self._index_read()
+        self._index_read(0)
 
     def __init__(
         self,
         *,
         obj_store: Optional[ObjStore] = None,
         replacement_policy: Union[str, ReplacementPolicy] = "gdsize",
         size: Union[int, str, bitmath.Bitmath] = bitmath.KiB(100),
         pickler: Pickler = pickle,
         lock: Optional[RWLock] = None,
         fine_grain_persistence: bool = False,
         fine_grain_eviction: bool = False,
         extra_system_state: Callable[[], Any] = Constant(None),
+        freeze_config: FreezeConfig = DEFAULT_FREEZE_CONFIG,
         temporary: bool = False,
     ) -> None:
         """Construct a memoized group. Use with :py:function:Memoized.
 
         :param obj_store: The object store to use for return values.
         :param replacement_policy: See policies submodule for options. You can pass an object conforming to the ReplacementPolicy protocol or one of REPLACEMENT_POLICIES.
         :param size: The size as an int (in bytes), as a string (e.g. "3 MiB"), or as a `bitmath.Bitmath`_.
         :param pickler: A de/serialization to use on the index, conforming to the Pickler protocol.
         :param lock: A ReadersWriterLock to achieve exclusion. If the lock is wrong but the obj_store is atomic, then the memoization is still *correct*, but it may not be able to borrow values that another machine computed. Defaults to a FileRWLock.
         :param fine_grain_persistence: De/serialize the index at every access. This is useful if you need to update the cache for multiple simultaneous processes, but it compromises performance in the single-process case.
         :param fine_grain_eviction: Maintain the cache's size through eviction at every access (rather than just the de/serialization points). This is useful if the caches size would not otherwise fit in memory, but it compromises performance if not needed.
         :param extra_system_state: A callable that returns "extra" system state. If the system state changes, the cache is dumped.
+        :param freeze_config: A charmonium.freeze.Config object. This config determines how objects and functions get hashed.
         :param temporary: Whether the cache should be cleared at the end of the process; This is useful for tests.
 
         .. _`bitmath.Bitmath`: https://pypi.org/project/bitmath/
 
         """
         self._obj_store = (
             obj_store
@@ -217,52 +207,55 @@
         )
         self._pickler = pickler
         self._index_lock = lock if lock is not None else FileRWLock(DEFAULT_LOCK_PATH)
         self._fine_grain_persistence = fine_grain_persistence
         self._fine_grain_eviction = fine_grain_eviction
         self._extra_system_state = extra_system_state
         self._index_key = 0
+        self._freeze_config = freeze_config
+        assert self._freeze_config.hasher is not None, "Hashing must be enabled in freeze_config"
         self.time_cost = DefaultDict[str, datetime.timedelta](datetime.timedelta)
         self.time_saved = DefaultDict[str, datetime.timedelta](datetime.timedelta)
         self.temporary = temporary
         self.__setstate__({})
         if self.temporary:
             atexit.register(self._obj_store.clear)
             # atexit handlers are run in the opposite order they are registered.
-        atexit.register(self._index_write)
+        atexit.register(self._index_write, 0)
         # TODO: atexit log report
 
     def _deleter(self, item: tuple[Any, Entry]) -> None:
-        # print(f"_deleter {item[0]} {freeze(item[0], freeze_config)}")
         with self._memory_lock:
             key, entry = item
             if entry.obj_store:
-                obj_key = cast(int, freeze(key, freeze_config))
+                obj_key = cast(int, freeze(key, self._freeze_config))
                 del self._obj_store[obj_key]
             else:
                 obj_key = None
             self._replacement_policy.invalidate(key, entry)
         if ops_logger.isEnabledFor(logging.DEBUG):
             ops_logger.debug(
                 json.dumps(
                     {
+                        "pid": os.getpid(),
+                        "tid": threading.get_native_id(),
                         "event": "cascading_delete",
                         "key": key,
                         "obj_key": obj_key,
                     }
                 )
             )
 
-    def _index_read(self) -> None:
+    def _index_read(self, call_id: int) -> None:
         with self._memory_lock, self._index_lock.reader:
-            self._index_read_nolock()
+            self._index_read_nolock(call_id)
 
-    def _index_read_nolock(self) -> None:
+    def _index_read_nolock(self, call_id: int) -> None:
         current_version = self._version
-        with perf_ctx("index_read"):
+        with perf_ctx("index_read", call_id):
             if self._index_key in self._obj_store:
                 other_version, other_index, other_rp, other_tc, other_ts = cast(
                     Tuple[
                         int,
                         Index[Any, Entry],
                         ReplacementPolicy,
                         DefaultDict[str, datetime.timedelta],
@@ -276,24 +269,27 @@
                     self._replacement_policy.update(other_rp)
                     self.time_cost = other_tc
                     self.time_saved = other_ts
         if ops_logger.isEnabledFor(logging.DEBUG):
             ops_logger.debug(
                 json.dumps(
                     {
+                        "pid": os.getpid(),
+                        "tid": threading.get_native_id(),
                         "event": "index_read",
                         "old_version": current_version,
                         "self._version": self._version,
+                        "call_id": call_id,
                     }
                 )
             )
 
-    def _index_write(self) -> None:
-        with perf_ctx("index_write"), self._memory_lock, self._index_lock.writer:
-            self._index_read_nolock()
+    def _index_write(self, call_id: int) -> None:
+        with perf_ctx("index_write", call_id), self._memory_lock, self._index_lock.writer:
+            self._index_read_nolock(call_id)
             self._evict()
             self._version += 1
             self._obj_store[self._index_key] = self._pickler.dumps(
                 (
                     self._version,
                     self._index,
                     self._replacement_policy,
@@ -301,16 +297,19 @@
                     self.time_saved,
                 )
             )
         if ops_logger.isEnabledFor(logging.DEBUG):
             ops_logger.debug(
                 json.dumps(
                     {
+                        "pid": os.getpid(),
+                        "tid": threading.get_native_id(),
                         "event": "index_write",
                         "self._version": self._version,
+                        "call_id": call_id,
                     }
                 )
             )
 
     def _system_state(self) -> Any:
         """Functions are deterministic with (global state, function-specific state, args key, args version).
 
@@ -328,26 +327,28 @@
             for key, entry in self._index.items():
                 # heapq.heappush(heap, (self._eval_func(entry), key, entry))
                 total_size += entry.data_size
 
             while total_size > self._size:
                 key, entry = self._replacement_policy.evict()
                 if entry.obj_store:
-                    obj_key = cast(int, freeze(key, freeze_config))
+                    obj_key = cast(int, freeze(key, self._freeze_config))
                     assert (
                         obj_key in self._obj_store
                     ), "Replacement policy tried to evict something that wasn't there"
                     del self._obj_store[obj_key]
                 else:
                     obj_key = None
                 total_size -= entry.data_size
                 if ops_logger.isEnabledFor(logging.DEBUG):
                     ops_logger.debug(
                         json.dumps(
                             {
+                                "pid": os.getpid(),
+                                "tid": threading.get_native_id(),
                                 "event": "evict",
                                 "key": key,
                                 "obj_key": obj_key,
                                 "entry.data_size": entry.data_size.bytes,
                                 "new_total_size": (total_size - entry.data_size).bytes,
                             }
                         )
@@ -375,14 +376,16 @@
             }
             for obj_key in self._obj_store:
                 if obj_key not in found_obj_keys:
                     if ops_logger.isEnabledFor(logging.DEBUG):
                         ops_logger.debug(
                             json.dumps(
                                 {
+                                    "pid": os.getpid(),
+                                    "tid": threading.get_native_id(),
                                     "event": "remove_orphan",
                                     "obj_key": obj_key,
                                 }
                             )
                         )
                     del self._obj_store[obj_key]
 
@@ -549,15 +552,15 @@
 
         if self._use_obj_store:
             stored_value = None
             value_ser = self._pickler.dumps(value)
             data_size = bitmath.Byte(len(value_ser))
             # Group is a "friend class", hence pylint disable
 
-            with perf_ctx("obj_store", call_id=call_id):
+            with perf_ctx("obj_store", call_id):
                 self.group._obj_store[  # pylint: disable=protected-access
                     obj_key
                 ] = value_ser
         else:
             stored_value = value
             data_size = bitmath.Byte(0)
 
@@ -596,86 +599,85 @@
             value,
             # Returning value in addition to Entry elides the redundant `loads(dumps(...))` when obj_store is True.
         )
 
     def __getfrozenstate__(self) -> Callable[..., Any]:
         return self.func
 
+    def _try_unpickle(self, value_ser: bytes, call_id: int) -> Tuple[bool, Optional[FuncReturn]]:
+        with perf_ctx("deserialize", call_id):
+            try:
+                value = cast(FuncReturn, self._pickler.loads(value_ser))
+            except (EOFError, pickling.UnpicklingError):
+                return False, None
+            else:
+                return True, value
+
     def __call__(
         self, *args: FuncParams.args, **kwargs: FuncParams.kwargs
     ) -> FuncReturn:
         call_start = datetime.datetime.now()
-
         call_id = random.randint(0, 2**64 - 1)
 
-        would_hit, key, obj_key = self._would_hit(call_id, *args, **kwargs)
+        key, entry, obj_key, value_ser = self._would_hit(call_id, *args, **kwargs)
+
+        hit, value = False, None
+        if entry is not None:
+            if entry.obj_store:
+                if value_ser is not None:
+                    hit, value = self._try_unpickle(value_ser, call_id)
+            else:
+                hit, value = True, cast(FuncReturn, entry.value)
 
         if ops_logger.isEnabledFor(logging.DEBUG):
             ops_logger.debug(
                 json.dumps(
                     {
-                        "event": "hit" if would_hit else "miss",
+                        "pid": os.getpid(),
+                        "tid": threading.get_native_id(),
+                        "event": "hit" if hit else "miss",
                         "call_id": call_id,
                         "name": self.name,
                         "key": key,
                         "obj_key": obj_key,
                         # "args_kwargs": ellipsize(str(args) + " " + str(kwargs), 60),
                     }
                 )
             )
 
-        if would_hit:
-
-            # Do the lookup
-            with self.group._memory_lock:
-                entry = self.group._index[key]
-                with perf_ctx("obj_load", call_id=call_id):
-                    value_ser = (
-                        self.group._obj_store[obj_key] if entry.obj_store else None
-                    )
-
-            # Deserialize
-            if entry.obj_store:
-                assert value_ser is not None
-                with perf_ctx("deserialize", call_id=call_id):
-                    value = cast(FuncReturn, self._pickler.loads(value_ser))
-            else:
-                value = cast(FuncReturn, entry.value)
-
-            # Update time_saved
-            with self.group._memory_lock:
-                self.group.time_saved[self.name] += entry.function_time
-                self.group._replacement_policy.access(key, entry)
-        else:
-
+        if not hit:
             # Do the recompute
             entry, value = self._recompute(call_id, obj_key, *args, **kwargs)
 
-            # Do the store
-            with self.group._memory_lock:
+        with self.group._memory_lock:
+            if hit:
+                # Update time_saved
+                self.group.time_saved[self.name] += entry.function_time
+                self.group._replacement_policy.access(key, entry)
+            else:
+                # Do the store
                 if self._use_metadata_size:
                     if not self._use_obj_store:
                         entry.data_size += bitmath.Byte(
                             len(self.group._pickler.dumps(entry))
                         )
                     entry.data_size += bitmath.Byte(len(self.group._pickler.dumps(key)))
                 self.group._index[key] = entry
                 self.group._replacement_policy.add(key, entry)
 
-        # Update time_cost
-        with self.group._memory_lock:
+            # Update time_cost
             if self.group._fine_grain_eviction:
                 self.group._evict()
 
             if self.group._fine_grain_persistence:
-                self.group._index_write()
+                self.group._index_write(call_id)
 
             call_stop = datetime.datetime.now()
             time_cost_inevitable = (
-                datetime.timedelta(seconds=0) if would_hit else entry.function_time
+                datetime.timedelta(seconds=0) if hit else entry.function_time
             )
             # time-cost is the overhead of caching, so  it should exclud ethe overhead of the function.
             self.group.time_cost[self.name] += (
                 call_stop - call_start - time_cost_inevitable
             )
 
             tc = self.group.time_cost[self.name]
@@ -686,73 +688,75 @@
                 json.dumps(
                     {
                         "name": self.name,
                         "event": "outer_function",
                         "call_id": call_id,
                         "hit": would_hit,
                         "duration": (call_stop - call_start).total_seconds(),
-                        "obj_key": obj_key,
                     }
                 )
             )
 
         if ts < tc and tc.total_seconds() > 5:
             warnings.warn(
                 f"Caching {self.func.__qualname__} cost {tc.total_seconds():.1f}s but only saved {ts.total_seconds():.1f}s",
                 CacheThrashingWarning,
             )
 
         return value
 
     def would_hit(self, *args: FuncParams.args, **kwargs: FuncParams.kwargs) -> bool:
         call_id = random.randint(0, 2**64 - 1)
-        would_hit, key, obj_key = self._would_hit(call_id, *args, **kwargs)
+        key, entry, obj_key, value_ser = self._would_hit(call_id, *args, **kwargs)
+        would_hit = entry is not None and (not entry.obj_store or value_ser is not None)
         if ops_logger.isEnabledFor(logging.DEBUG):
             ops_logger.debug(
                 json.dumps(
                     {
-                        "event": "hit" if would_hit else "miss",
+                        "pid": os.getpid(),
+                        "tid": threading.get_native_id(),
+                        "event": "hit" if hit else "miss",
                         "call_id": call_id,
                         "name": self.name,
                         "key": key,
                         "obj_key": obj_key,
                         # "args_kwargs": ellipsize(str(args) + " " + str(kwargs), 60),
                     }
                 )
             )
         return would_hit
 
     def _would_hit(
         self, call_id: int, *args: FuncParams.args, **kwargs: FuncParams.kwargs
-    ) -> Tuple[bool, Tuple[Any, ...], int]:
+    ) -> Tuple[Tuple[Any, ...], Optional[Entry], int, Optional[bytes]]:
         # pylint: disable=protected-access
 
-        with perf_ctx("hash", call_id=call_id):
+        with perf_ctx("hash", call_id):
             # Note that the system state and name or so small already, it isn't worth hashing them.
             # They are also used by other Memoized functions in the same MemoizedGroup.
             # We will only hash the potentially large key items that are used exclusively by this Memoized function.
             key = (
                 # Group is a friend class, hence type ignore
                 freeze(
-                    self.group._system_state(), freeze_config
+                    self.group._system_state(), self.group._freeze_config
                 ),  # pylint: disable=protected-access
-                freeze(self.name, freeze_config),
-                freeze(self._func_state(), freeze_config),
-                freeze(self._args2key(*args, **kwargs), freeze_config),
-                freeze(self._args2ver(*args, **kwargs), freeze_config),
+                freeze(self.name, self.group._freeze_config),
+                freeze(self._func_state(), self.group._freeze_config),
+                freeze(self._args2key(*args, **kwargs), self.group._freeze_config),
+                freeze(self._args2ver(*args, **kwargs), self.group._freeze_config),
             )
-            obj_key = cast(int, freeze(key, freeze_config))
+            obj_key = cast(int, freeze(key, self.group._freeze_config))
         with self.group._memory_lock:
             if self.group._fine_grain_persistence:
-                self.group._index_read()
+                self.group._index_read(call_id)
             return (
-                key in self.group._index
-                and (not self._use_obj_store or obj_key in self.group._obj_store),
                 key,
+                self.group._index.get(key, None),
                 obj_key,
+                self.group._obj_store.get(obj_key, None) if self._use_obj_store else None,
             )
 
     def __get__(self, instance: Any, instancetype: Type[Any]) -> BoundMemoized[FuncParams, FuncReturn]:
         """Implement the descriptor protocol to make decorating instance
         method possible.
 
         """
```

### Comparing `charmonium_cache-1.3.0/charmonium/cache/obj_store.py` & `charmonium_cache-1.4.0/charmonium/cache/obj_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import dataclasses
 import shutil
-from typing import TYPE_CHECKING, Any, Iterator, Union
+from typing import TYPE_CHECKING, Any, Iterator, Union, TypeVar
 from pathlib import Path
 
 if TYPE_CHECKING:
     from typing import Protocol
 else:
     Protocol = object
 
 
+_T = TypeVar("_T")
+
+
 class ObjStore(Protocol):
     """An `object-store`_ is a persistent mapping from int to bytes.
 
     .. _`object-store`: https://en.wikipedia.org/wiki/Object_storage
 
     """
 
@@ -23,14 +26,17 @@
 
     def __getitem__(self, key: int) -> bytes:
         ...
 
     def __delitem__(self, key: int) -> None:
         ...
 
+    def get(self, key: int, default: _T) -> Union[bytes | _T]:
+        ...
+
     def __contains__(self, key: int) -> bool:
         """The implementation is often slow, so it will be called rarely."""
 
     def __iter__(self) -> Iterator[int]:
         # pylint: disable=non-iterator-returned
         ...
 
@@ -56,15 +62,15 @@
 
     def __init__(self, path: Union[Path, str], key_bytes: int = 16) -> None:
         """
         :param path: the directory of the object store.
         :param key_bytes: the number of bytes to use as keys
         """
         super().__init__()
-        self.path = Path(path)
+        self.path = path if isinstance(path, Path) else Path(path)
         self.key_bytes = key_bytes
 
         if self.path.exists():
             if any(
                 not self._is_key(path) and not path.name.startswith(".")
                 for path in self.path.iterdir()
             ):
@@ -92,14 +98,21 @@
             return path.read_bytes()
 
     def __delitem__(self, key: int) -> None:
         if key in self:
             # print(f"delitem {key}")
             (self.path / self._int2str(key)).unlink()
 
+    def get(self, key: int, default: _T) -> Union[bytes | _T]:
+        path = self.path / self._int2str(key)
+        if not path.exists():
+            return default
+        else:
+            return path.read_bytes()
+
     def __contains__(self, key: int) -> bool:
         return (self.path / self._int2str(key)).exists()
 
     def __iter__(self) -> Iterator[int]:
         yield from (
             int(path.name, base=16)
             for path in self.path.iterdir()
```

### Comparing `charmonium_cache-1.3.0/charmonium/cache/pathlike.py` & `charmonium_cache-1.4.0/charmonium/cache/pathlike.py`

 * *Files identical despite different names*

### Comparing `charmonium_cache-1.3.0/charmonium/cache/replacement_policies.py` & `charmonium_cache-1.4.0/charmonium/cache/replacement_policies.py`

 * *Files identical despite different names*

### Comparing `charmonium_cache-1.3.0/charmonium/cache/rw_lock.py` & `charmonium_cache-1.4.0/charmonium/cache/rw_lock.py`

 * *Files identical despite different names*

### Comparing `charmonium_cache-1.3.0/charmonium/cache/util.py` & `charmonium_cache-1.4.0/charmonium/cache/util.py`

 * *Files identical despite different names*

### Comparing `charmonium_cache-1.3.0/pyproject.toml` & `charmonium_cache-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charmonium.cache"
-version = "1.3.0"
+version = "1.4.0"
 description = "Provides a decorator for caching a function between subsequent processes."
 authors = ["Samuel Grayson <sam+dev@samgrayson.me>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/charmoniumQ/charmonium.cache"
 packages = [
     { include = "charmonium" },
@@ -20,14 +20,15 @@
 	"Intended Audience :: Science/Research",
 	"Intended Audience :: Developers",
 	"Topic :: Scientific/Engineering",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 ]
 [tool.poetry.group.dev.dependencies]
 deptry = "^0.8.0"
+cryptography = "40.0.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
@@ -69,15 +70,15 @@
 strict = true
 pretty = true
 error_summary = true
 color_output = true
 #mypy_path = stubs
 
 [tool.bump2version]
-current_version = "1.3.0"
+current_version = "1.4.0"
 commit = true
 tag = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py{38,39,310}
@@ -114,17 +115,14 @@
 proselint = "^0.13.0"
 rstcheck = "^3.3.1"
 bump2version = "^1.0.1"
 "charmonium.async-subprocess" = "^0.1.7"
 typer = "^0.4.0"
 termcolor = "^1.1.0"
 typing-extensions = "^4.1.1"
-ipython = "^8.10"
-ipdb = "^0.13.9"
-codecov = "^2.1.4"
 sphinx = "^4.5.0"
 pytest-assume = "^2.4.2"
 sphinx-autodoc-typehints = "^1.12.0"
 sphinxcontrib-spelling = "^7.1.0"
 cloudpickle = "^1.6.0"
 dask = {extras = ["bag"], version = "^2021.4.1"}
 gitchangelog = "^3.0.4"
```

### Comparing `charmonium_cache-1.3.0/setup.py` & `charmonium_cache-1.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,192 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: charmonium-cache
+Version: 1.4.0
+Summary: Provides a decorator for caching a function between subsequent processes.
+Home-page: https://github.com/charmoniumQ/charmonium.cache
+License: MIT
+Keywords: cache,memoize,decorator
+Author: Samuel Grayson
+Author-email: sam+dev@samgrayson.me
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: bitmath (>=1.3,<2.0)
+Requires-Dist: charmonium.freeze (>=0.8.1,<2)
+Requires-Dist: fasteners (>=0.16,<2)
+Project-URL: Documentation, https://charmoniumq.github.io/charmonium.cache/
+Project-URL: Repository, https://github.com/charmoniumQ/charmonium.cache
+Description-Content-Type: text/x-rst
+
+==========================
+charmonium.cache
+==========================
+
+.. image:: https://img.shields.io/pypi/v/charmonium.cache
+   :alt: PyPI Package
+   :target: https://pypi.org/project/charmonium.cache
+.. image:: https://img.shields.io/pypi/dm/charmonium.cache
+   :alt: PyPI Downloads
+   :target: https://pypi.org/project/charmonium.cache
+.. image:: https://img.shields.io/pypi/l/charmonium.cache
+   :alt: PyPI License
+   :target: https://github.com/charmoniumQ/charmonium.cache/blob/main/LICENSE
+.. image:: https://img.shields.io/pypi/pyversions/charmonium.cache
+   :alt: Python Versions
+   :target: https://pypi.org/project/charmonium.cache
+.. image:: https://img.shields.io/github/stars/charmoniumQ/charmonium.cache?style=social
+   :alt: GitHub stars
+   :target: https://github.com/charmoniumQ/charmonium.cache
+.. image:: https://github.com/charmoniumQ/charmonium.cache/actions/workflows/main.yaml/badge.svg
+   :alt: CI status
+   :target: https://github.com/charmoniumQ/charmonium.cache/actions/workflows/main.yaml
+.. image:: https://codecov.io/gh/charmoniumQ/charmonium.cache/branch/main/graph/badge.svg?token=JTL4SNMWTP
+   :alt: Code Coverage
+   :target: https://codecov.io/gh/charmoniumQ/charmonium.cache
+.. image:: https://img.shields.io/github/last-commit/charmoniumQ/charmonium.cache
+   :alt: GitHub last commit
+   :target: https://github.com/charmoniumQ/charmonium.cache/commits
+.. image:: https://img.shields.io/librariesio/sourcerank/pypi/charmonium.cache
+   :alt: libraries.io sourcerank
+   :target: https://libraries.io/pypi/charmonium.cache
+.. image:: https://img.shields.io/badge/docs-yes-success
+   :alt: Documentation link
+   :target: https://charmoniumq.github.io/charmonium.cache/
+.. image:: http://www.mypy-lang.org/static/mypy_badge.svg
+   :target: https://mypy.readthedocs.io/en/stable/
+   :alt: Checked with Mypy
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+
+Provides a decorator for caching a function between subsequent processes.
+
+Whenever the function is called with the same arguments, the result is
+loaded from the cache instead of computed. This cache is **persistent
+across runs**. If the arguments, source code, or enclosing environment
+have changed, the cache recomputes the data transparently (**no need
+for manual invalidation**).
+
+The use case is meant for iterative development, especially on scientific
+experiments. Many times a developer will tweak some of the code but not
+all. Often, reusing intermediate results saves a significant amount of time
+every run.
+
+See full documentation `here`_.
+
+.. _`here`: https://charmoniumq.github.io/charmonium.cache/
+
+
+Quickstart
+----------
+
+If you don't have ``pip`` installed, see the `pip install
+guide`_.
+
+.. _`pip install guide`: https://pip.pypa.io/en/latest/installing/
+
+.. code-block:: console
+
+    $ pip install charmonium.cache
+
+>>> from charmonium.cache import memoize
+>>> i = 0
+>>> @memoize()
+... def square(x):
+...     print("recomputing")
+...     # Imagine a more expensive computation here.
+...     return x**2 + i
+...
+>>> square(4)
+recomputing
+16
+>>> square(4) # no need to recompute
+16
+>>> i = 1
+>>> square(4) # global i changed; must recompute
+recomputing
+17
+
+Advantages
+----------
+
+While there are other libraries and techniques for memoization, I believe this
+one is unique because it is:
+
+1. **Correct with respect to source-code changes:** The cache detects if you
+   edit the source code or change a file which the program reads (provided they
+   use this library's right file abstraction). Users never need to manually
+   invalidate the cache, so long as the functions are pure (unlike
+   `joblib.Memory`_, `Klepto`_).
+
+   It is precise enough that it will ignore changes in unrelated functions in
+   the file, but it will detect changes in relevant functions in other files. It
+   even detects changes in global variables (as in the example above). See
+   `Detecting Changes in Functions`_ for details.
+
+2. **Useful between runs and across machines:** The cache can persist on the
+   disk (unlike `functools.lru_cache`_). Moreover, a cache can be shared on the
+   network, so that if *any* machine has computed the function for the same
+   source-source and arguments, this value can be reused by *any other* machine,
+   provided your datatype is de/serializable on those platforms.
+
+3. **Easy to adopt:** Only requires adding one line (`decorator`_) to
+   the function definition.
+
+4. **Bounded in size:** The cache won't take up too much space. This
+   space is partitioned across all memoized functions according to the
+   heuristic.
+
+5. **Supports smart heuristics:** By default, the library uses state-of-the-art
+   cache policies that can take into account time-to-recompute and storage-size
+   in addition to recency, more advanced than simple `LRU`_.
+
+6. **Overhead aware:** The library measures the time saved versus overhead. It
+   warns the user if the overhead of caching is not worth it.
+
+.. _`Detecting Changes in Functions`: https://charmoniumq.github.io/charmonium.cache/tutorial.html#detecting-changes-in-functions
+.. _`Klepto`: https://klepto.readthedocs.io/en/latest/
+.. _`joblib.Memory`: https://joblib.readthedocs.io/en/latest/memory.html
+.. _`functools.lru_cache`: https://docs.python.org/3/library/functools.html#functools.lru_cache
+.. _`decorator`: https://docs.python.org/3/glossary.html#term-decorator
+.. _`LRU`: https://en.wikipedia.org/wiki/Cache_replacement_policies#Least_recently_used_(LRU)
+
+Memoize CLI
+-----------
+
+Make is good for compiling code, but falls short for data science. To get
+correct results, you have to incorporate *every* variable your result depends on
+into a file or part of the filename. If you put it in a file, you only have one
+version cached at a time; if you put it in the filename, you have to squeeze the
+variable into a short string. In either case, stale results will accumulate
+unboundedly, until you run ``make clean`` which also purges the fresh
+results. Finally, it is a significant effor to rewrite shell scripts in make.
+
+``memoize`` makes it easy to memoize steps in shell scripts, correctly. Just add
+``memoize`` to the start of the line. If the command, its arguments,
+or its input files change, then ``command arg1 arg2 ...`` will be
+rerun. Otherwise, the output files (including stderr and stdout) will be
+produced from a prior run. ``memoize`` uses ptrace to automatically determine
+what inputs you depend on and what outputs you produce.
+
+::
+
+   memoize command arg1 arg2
+   # or
+   memoize --key=$(date +%Y-%m-%d) -- command arg1 arg2
 
-packages = \
-['charmonium', 'charmonium.cache']
+See `CLI`_ for more details.
 
-package_data = \
-{'': ['*']}
+.. _`CLI`: https://charmoniumq.github.io/charmonium.cache/cli.html
 
-install_requires = \
-['bitmath>=1.3,<2.0', 'charmonium.freeze>=0.8.1,<2', 'fasteners>=0.16,<2']
-
-entry_points = \
-{'console_scripts': ['cache = charmonium.cache._cli:main']}
-
-setup_kwargs = {
-    'name': 'charmonium-cache',
-    'version': '1.3.0',
-    'description': 'Provides a decorator for caching a function between subsequent processes.',
-    'long_description': '==========================\ncharmonium.cache\n==========================\n\n.. image:: https://img.shields.io/pypi/v/charmonium.cache\n   :alt: PyPI Package\n   :target: https://pypi.org/project/charmonium.cache\n.. image:: https://img.shields.io/pypi/dm/charmonium.cache\n   :alt: PyPI Downloads\n   :target: https://pypi.org/project/charmonium.cache\n.. image:: https://img.shields.io/pypi/l/charmonium.cache\n   :alt: PyPI License\n   :target: https://github.com/charmoniumQ/charmonium.cache/blob/main/LICENSE\n.. image:: https://img.shields.io/pypi/pyversions/charmonium.cache\n   :alt: Python Versions\n   :target: https://pypi.org/project/charmonium.cache\n.. image:: https://img.shields.io/github/stars/charmoniumQ/charmonium.cache?style=social\n   :alt: GitHub stars\n   :target: https://github.com/charmoniumQ/charmonium.cache\n.. image:: https://github.com/charmoniumQ/charmonium.cache/actions/workflows/main.yaml/badge.svg\n   :alt: CI status\n   :target: https://github.com/charmoniumQ/charmonium.cache/actions/workflows/main.yaml\n.. image:: https://codecov.io/gh/charmoniumQ/charmonium.cache/branch/main/graph/badge.svg?token=JTL4SNMWTP\n   :alt: Code Coverage\n   :target: https://codecov.io/gh/charmoniumQ/charmonium.cache\n.. image:: https://img.shields.io/github/last-commit/charmoniumQ/charmonium.cache\n   :alt: GitHub last commit\n   :target: https://github.com/charmoniumQ/charmonium.cache/commits\n.. image:: https://img.shields.io/librariesio/sourcerank/pypi/charmonium.cache\n   :alt: libraries.io sourcerank\n   :target: https://libraries.io/pypi/charmonium.cache\n.. image:: https://img.shields.io/badge/docs-yes-success\n   :alt: Documentation link\n   :target: https://charmoniumq.github.io/charmonium.cache/\n.. image:: http://www.mypy-lang.org/static/mypy_badge.svg\n   :target: https://mypy.readthedocs.io/en/stable/\n   :alt: Checked with Mypy\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Code style: black\n\nProvides a decorator for caching a function between subsequent processes.\n\nWhenever the function is called with the same arguments, the result is\nloaded from the cache instead of computed. This cache is **persistent\nacross runs**. If the arguments, source code, or enclosing environment\nhave changed, the cache recomputes the data transparently (**no need\nfor manual invalidation**).\n\nThe use case is meant for iterative development, especially on scientific\nexperiments. Many times a developer will tweak some of the code but not\nall. Often, reusing intermediate results saves a significant amount of time\nevery run.\n\nSee full documentation `here`_.\n\n.. _`here`: https://charmoniumq.github.io/charmonium.cache/\n\n\nQuickstart\n----------\n\nIf you don\'t have ``pip`` installed, see the `pip install\nguide`_.\n\n.. _`pip install guide`: https://pip.pypa.io/en/latest/installing/\n\n.. code-block:: console\n\n    $ pip install charmonium.cache\n\n>>> from charmonium.cache import memoize\n>>> i = 0\n>>> @memoize()\n... def square(x):\n...     print("recomputing")\n...     # Imagine a more expensive computation here.\n...     return x**2 + i\n...\n>>> square(4)\nrecomputing\n16\n>>> square(4) # no need to recompute\n16\n>>> i = 1\n>>> square(4) # global i changed; must recompute\nrecomputing\n17\n\nAdvantages\n----------\n\nWhile there are other libraries and techniques for memoization, I believe this\none is unique because it is:\n\n1. **Correct with respect to source-code changes:** The cache detects if you\n   edit the source code or change a file which the program reads (provided they\n   use this library\'s right file abstraction). Users never need to manually\n   invalidate the cache, so long as the functions are pure (unlike\n   `joblib.Memory`_, `Klepto`_).\n\n   It is precise enough that it will ignore changes in unrelated functions in\n   the file, but it will detect changes in relevant functions in other files. It\n   even detects changes in global variables (as in the example above). See\n   `Detecting Changes in Functions`_ for details.\n\n2. **Useful between runs and across machines:** The cache can persist on the\n   disk (unlike `functools.lru_cache`_). Moreover, a cache can be shared on the\n   network, so that if *any* machine has computed the function for the same\n   source-source and arguments, this value can be reused by *any other* machine,\n   provided your datatype is de/serializable on those platforms.\n\n3. **Easy to adopt:** Only requires adding one line (`decorator`_) to\n   the function definition.\n\n4. **Bounded in size:** The cache won\'t take up too much space. This\n   space is partitioned across all memoized functions according to the\n   heuristic.\n\n5. **Supports smart heuristics:** By default, the library uses state-of-the-art\n   cache policies that can take into account time-to-recompute and storage-size\n   in addition to recency, more advanced than simple `LRU`_.\n\n6. **Overhead aware:** The library measures the time saved versus overhead. It\n   warns the user if the overhead of caching is not worth it.\n\n.. _`Detecting Changes in Functions`: https://charmoniumq.github.io/charmonium.cache/tutorial.html#detecting-changes-in-functions\n.. _`Klepto`: https://klepto.readthedocs.io/en/latest/\n.. _`joblib.Memory`: https://joblib.readthedocs.io/en/latest/memory.html\n.. _`functools.lru_cache`: https://docs.python.org/3/library/functools.html#functools.lru_cache\n.. _`decorator`: https://docs.python.org/3/glossary.html#term-decorator\n.. _`LRU`: https://en.wikipedia.org/wiki/Cache_replacement_policies#Least_recently_used_(LRU)\n\nMemoize CLI\n-----------\n\nMake is good for compiling code, but falls short for data science. To get\ncorrect results, you have to incorporate *every* variable your result depends on\ninto a file or part of the filename. If you put it in a file, you only have one\nversion cached at a time; if you put it in the filename, you have to squeeze the\nvariable into a short string. In either case, stale results will accumulate\nunboundedly, until you run ``make clean`` which also purges the fresh\nresults. Finally, it is a significant effor to rewrite shell scripts in make.\n\n``memoize`` makes it easy to memoize steps in shell scripts, correctly. Just add\n``memoize`` to the start of the line. If the command, its arguments,\nor its input files change, then ``command arg1 arg2 ...`` will be\nrerun. Otherwise, the output files (including stderr and stdout) will be\nproduced from a prior run. ``memoize`` uses ptrace to automatically determine\nwhat inputs you depend on and what outputs you produce.\n\n::\n\n   memoize command arg1 arg2\n   # or\n   memoize --key=$(date +%Y-%m-%d) -- command arg1 arg2\n\nSee `CLI`_ for more details.\n\n.. _`CLI`: https://charmoniumq.github.io/charmonium.cache/cli.html\n',
-    'author': 'Samuel Grayson',
-    'author_email': 'sam+dev@samgrayson.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/charmoniumQ/charmonium.cache',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

