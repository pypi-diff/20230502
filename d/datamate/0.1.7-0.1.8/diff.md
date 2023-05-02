# Comparing `tmp/datamate-0.1.7.tar.gz` & `tmp/datamate-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamate-0.1.7.tar", last modified: Mon May  1 19:41:33 2023, max compression
+gzip compressed data, was "datamate-0.1.8.tar", last modified: Tue May  2 12:56:34 2023, max compression
```

## Comparing `datamate-0.1.7.tar` & `datamate-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:41:33.163614 datamate-0.1.7/
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-05-01 19:41:33.162851 datamate-0.1.7/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3642 2023-03-06 13:58:32.000000 datamate-0.1.7/README.md
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:41:33.156682 datamate-0.1.7/datamate/
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      647 2023-05-01 19:25:54.000000 datamate-0.1.7/datamate/__init__.py
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    55504 2023-05-01 19:06:32.000000 datamate-0.1.7/datamate/directory.py
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    11921 2023-05-01 17:35:54.000000 datamate-0.1.7/datamate/namespaces.py
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)       20 2023-05-01 19:39:43.000000 datamate-0.1.7/datamate/version.py
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:41:33.159359 datamate-0.1.7/datamate.egg-info/
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3829 2023-05-01 19:41:33.000000 datamate-0.1.7/datamate.egg-info/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      312 2023-05-01 19:41:33.000000 datamate-0.1.7/datamate.egg-info/SOURCES.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        1 2023-05-01 19:41:33.000000 datamate-0.1.7/datamate.egg-info/dependency_links.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      109 2023-05-01 19:41:33.000000 datamate-0.1.7/datamate.egg-info/requires.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        9 2023-05-01 19:41:33.000000 datamate-0.1.7/datamate.egg-info/top_level.txt
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)       38 2023-05-01 19:41:33.163776 datamate-0.1.7/setup.cfg
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)      926 2023-05-01 19:20:47.000000 datamate-0.1.7/setup.py
-drwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)        0 2023-05-01 19:41:33.161561 datamate-0.1.7/tests/
--rwxr-xr-x   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)    28917 2023-05-01 19:06:56.000000 datamate-0.1.7/tests/test_directory.py
--rw-r--r--   0 lappalainenj (1483866292) HHMI\Domain Users (1899195968)     3747 2023-04-04 14:23:09.000000 datamate-0.1.7/tests/test_namespaces.py
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.334211 datamate-0.1.8/
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-02 12:56:34.333460 datamate-0.1.8/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3642 2023-03-06 13:58:32.000000 datamate-0.1.8/README.md
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.329914 datamate-0.1.8/datamate/
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      647 2023-05-01 19:25:54.000000 datamate-0.1.8/datamate/__init__.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968    57284 2023-05-02 12:04:55.000000 datamate-0.1.8/datamate/directory.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968    11921 2023-05-01 17:35:54.000000 datamate-0.1.8/datamate/namespaces.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968       20 2023-05-02 12:54:26.000000 datamate-0.1.8/datamate/version.py
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.332120 datamate-0.1.8/datamate.egg-info/
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      312 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/SOURCES.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968        1 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/dependency_links.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      109 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/requires.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968        9 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/top_level.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968       38 2023-05-02 12:56:34.334360 datamate-0.1.8/setup.cfg
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      926 2023-05-01 19:20:47.000000 datamate-0.1.8/setup.py
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.332949 datamate-0.1.8/tests/
+-rwxr-xr-x   0 lappalainenj (1483866292) 1899195968    30336 2023-05-02 12:36:23.000000 datamate-0.1.8/tests/test_directory.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3747 2023-04-04 14:23:09.000000 datamate-0.1.8/tests/test_namespaces.py
```

### Comparing `datamate-0.1.7/PKG-INFO` & `datamate-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.7
+Version: 0.1.8
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.7/README.md` & `datamate-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `datamate-0.1.7/datamate/__init__.py` & `datamate-0.1.8/datamate/__init__.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.7/datamate/directory.py` & `datamate-0.1.8/datamate/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 # -- Root Directory directory management ----------------------------------------
 
 context = threading.local()
 context.enforce_config_match = True
 context.check_size_on_init = False
 context.verbosity_level = 2
+# context.in_memory = False
 
 
 def set_root_dir(root_dir: Optional[Path]) -> None:
     """
     Set the directory in which to search for Directorys.
     """
     context.root_dir = Path(root_dir) if root_dir is not None else Path(".")
@@ -197,14 +198,25 @@
     try:
         yield
     finally:
         set_root_dir(_root_dir)
         context.within_root_context = False
 
 
+# @contextmanager
+# def in_memory():
+#     """Set in_memory mode within a context and revert after to debug a Directory.
+#     """
+#     _in_memory = getattr(context, "in_memory", False)
+#     context.in_memory = True
+#     try:
+#         yield
+#     finally:
+#         context.in_memory = _in_memory
+
 def enforce_config_match(enforce: bool) -> None:
     """
     Enforce error if configs are not matching.
 
     Defaults to True.
 
     Configs are compared, when initializing a directory
@@ -509,14 +521,17 @@
         (possibly empty) `Directory`s.
 
         Attribute access syntax is also supported, and occurrences of "__" in
         `key` are transformed into ".", to support accessing encoded files as
         attributes (i.e. `Directory['name.ext']` is equivalent to
         `Directory.name__ext`).
         """
+        # if context.in_memory:
+        #     return object.__getattribute__(self, key)
+
         try:
             # to catch cases where key is an index to a reference to an h5 file.
             # this will yield a TypeError because Path / slice does not work.
             path = self.path / key
         except TypeError as e:
             if not self.path.exists():
                 raise (
@@ -549,14 +564,18 @@
         written as subDirectorys.
 
         Attribute access syntax is also supported, and occurrences of "__" in
         `key` are transformed into ".", to support accessing encoded files as
         attributes (i.e. `Directory['name.ext'] = val` is equivalent to
         `Directory.name__ext = val`).
         """
+        # if context.in_memory:
+        #     object.__setattr__(self, key, val)
+        #     return
+
         path = self.path / key
 
         # Copy an existing file or directory.
         if isinstance(val, Path):
             if os.path.isfile(val):
                 _copy_file(path, val)
             elif os.path.isdir(val):
@@ -591,14 +610,17 @@
         Deletes the entry at `self.path/key`
 
         Attribute access syntax is also supported, and occurrences of "__" in
         `key` are transformed into ".", to support accessing encoded files as
         attributes (i.e. `del Directory['name.ext']` is equivalent to
         `del Directory.name__ext`).
         """
+        # if context.in_memory:
+        #     object.__delitem__(self, key)
+        #     return
         path = self.path / key
 
         # Delete an array file.
         if path.with_suffix(".h5").is_file():
             path.with_suffix(".h5").unlink()
 
         # Delete a non-array file.
@@ -616,14 +638,17 @@
         Extending `ArrayFile`s performs concatenation along the first axis,
         extending `Path`s performs byte-level concatenation, and
         extending subDirectorys extends their fields.
 
         Files corresponding to `self[key]` are created if they do not already
         exist.
         """
+        # if context.in_memory:
+        #     self.__setitem__(key, np.append(self.__getitem__(key), val, axis=0))
+
         path = self.path / key
 
         # Append an existing file.
         if isinstance(val, Path):
             assert path.suffix != ""
             _extend_file(path, val)
 
@@ -1379,26 +1404,38 @@
     object.__setattr__(obj, "_config", namespacify(config))
     return cast(Directory, obj)
 
 
 # -- I/O -----------------------------------------------------------------------
 
 
-def _read_h5(path: Path) -> ArrayFile:
+def _read_h5(path: Path, assert_swmr=True) -> ArrayFile:
     try:
         f = h5.File(path, "r", libver="latest", swmr=True)
-        assert f.swmr_mode
+        if assert_swmr:
+            assert f.swmr_mode, "File is not in SWMR mode."
         return f["data"]
     except OSError as e:
         print(e)
-        if "errno = 2" in str(e):  # 2 := File not found.
+        if "errno = 2" in str(e):
             raise e
         sleep(0.1)
         return _read_h5(path)
 
+    # try:
+    #     f = h5.File(path, "r", libver="latest", swmr=True)
+    #     assert f.swmr_mode
+    #     return f["data"]
+    # except OSError as e:
+    #     print(e)
+    #     if "errno = 2" in str(e):  # 2 := File not found.
+    #         raise e
+    #     sleep(0.1)
+    #     return _read_h5(path)
+
 
 def _write_h5(path: Path, val: object) -> None:
     val = np.asarray(val)
     try:
         f = h5.File(path, libver="latest", mode="w")
         if f["data"].dtype != val.dtype:
             raise ValueError()
@@ -1422,14 +1459,29 @@
 
 def _extend_h5(path: Path, val: object, retry: int = 0, max_retries: int = 50) -> None:
     val = np.asarray(val)
     path.parent.mkdir(parents=True, exist_ok=True)
     # mode='a' to read file, create otherwise
     try:
         f = h5.File(path, libver="latest", mode="a")
+        if "data" not in f:
+            dset = f.require_dataset(
+                name="data",
+                shape=None,
+                maxshape=(None, *val.shape[1:]),
+                dtype=val.dtype,
+                data=np.empty((0, *val.shape[1:]), val.dtype),
+                chunks=(
+                    int(np.ceil(2**12 / np.prod(val.shape[1:]))),
+                    *val.shape[1:],
+                ),
+            )
+            f.swmr_mode = True
+        else:
+            dset = f["data"]
     except BlockingIOError as e:
         print(e)
         if "errno = 11" in str(e) or "errno = 35" in str(
             e
         ):  # 11, 35 := Reource temporarily unavailable
             sleep(0.1)
             if retry < max_retries:
@@ -1439,34 +1491,35 @@
                     "maximum retries to extend the dataset"
                     " exceeded, while the resource was unavailable. Because"
                     " the dataset is constantly locked by another thread."
                 )
             return
         else:
             raise e
-    if "data" not in f:
-        dset = f.require_dataset(
-            name="data",
-            shape=None,
-            maxshape=(None, *val.shape[1:]),
-            dtype=val.dtype,
-            data=np.empty((0, *val.shape[1:]), val.dtype),
-            chunks=(
-                int(np.ceil(2**12 / np.prod(val.shape[1:]))),
-                *val.shape[1:],
-            ),
-        )
-        f.swmr_mode = True
-    else:
-        dset = f["data"]
-    if len(val) > 0:
-        dset.resize(dset.len() + len(val), 0)
-        dset[-len(val) :] = val
-        dset.flush()
 
+    def _override_to_chunked(path: Path, val: object) -> None:
+        # override as chunked dataset
+        data = _read_h5(path, assert_swmr=False)[()]
+        path.unlink()
+        _extend_h5(path, data)
+        # call extend again with new value
+        _extend_h5(path, val)
+
+    if len(val) > 0:
+        try:
+            dset.resize(dset.len() + len(val), 0)
+            dset[-len(val) :] = val
+            dset.flush()
+        except TypeError as e:
+            # workaround if dataset was first created as non-chunked
+            # using __setitem__ and then extended using extend
+            if "Only chunked datasets can be resized" in str(e):
+                _override_to_chunked(path, val)
+            else:
+                raise e
 
 def _copy_file(dst: Path, src: Path) -> None:
     # shutil.rmtree(dst, ignore_errors=True)
     dst.parent.mkdir(parents=True, exist_ok=True)
     shutil.copy(src, dst)
```

### Comparing `datamate-0.1.7/datamate/namespaces.py` & `datamate-0.1.8/datamate/namespaces.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.7/datamate.egg-info/PKG-INFO` & `datamate-0.1.8/datamate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.7
+Version: 0.1.8
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.7/setup.py` & `datamate-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.7/tests/test_directory.py` & `datamate-0.1.8/tests/test_directory.py`

 * *Files 5% similar despite different names*

```diff
@@ -201,35 +201,57 @@
 
 def test_list_extension(tmp_path: Path) -> None:
     a = Directory(tmp_path)
     a.extend("b", [[7, 8], [9, 10]])
     a.extend("b", [[11, 12]])
     assert_directory_equals(a, {"b": [[7, 8], [9, 10], [11, 12]]})
 
+    b = Directory(tmp_path)
+    b.b = [[7, 8], [9, 10]]
+    b.extend("b", [[11, 12]])
+    assert_directory_equals(a, {"b": [[7, 8], [9, 10], [11, 12]]})
+
 
 def test_array_extension(tmp_path: Path) -> None:
     a = Directory(tmp_path)
     a.extend("b", np.uint16([[7, 8], [9, 10]]))
     a.extend("b", np.uint16([[11, 12]]))
     assert_directory_equals(a, {"b": np.uint16([[7, 8], [9, 10], [11, 12]])})
 
+    b = Directory(tmp_path)
+    b.b = np.uint16([[7, 8], [9, 10]])
+    b.extend("b", np.uint16([[11, 12]]))
+    assert_directory_equals(b, {"b": np.uint16([[7, 8], [9, 10], [11, 12]])})
+
 
 def test_path_extension(tmp_path: Path) -> None:
     a = Directory(tmp_path / "a")
     a.extend("b.bin", data_file(tmp_path / "b0.bin"))
     a.extend("b.bin", data_file(tmp_path / "b1.bin"))
     assert_directory_equals(
         a,
         {
             "b.bin": data_file_concat(
                 tmp_path / "b2.bin", [tmp_path / "b0.bin", tmp_path / "b1.bin"]
             )
         },
     )
 
+    b = Directory(tmp_path / "a")
+    b["b.bin"] = data_file(tmp_path / "b0.bin")
+    b.extend("b.bin", data_file(tmp_path / "b1.bin"))
+    assert_directory_equals(
+        b,
+        {
+            "b.bin": data_file_concat(
+                tmp_path / "b2.bin", [tmp_path / "b0.bin", tmp_path / "b1.bin"]
+            )
+        },
+    )
+
 
 def test_dict_extension(tmp_path: Path) -> None:
     a = Directory(tmp_path / "a")
     a.extend(
         "b",
         {
             "c": np.empty((0, 2), dtype="uint16"),
@@ -250,14 +272,40 @@
         {
             "b": {
                 "c": np.uint16([[1, 2], [3, 4]]),
                 "d.bin": data_file_concat(
                     tmp_path / "d2.bin", [tmp_path / "d0.bin", tmp_path / "d1.bin"]
                 ),
                 "e": {"f": [0.1, 0.2, 0.3, 0.4, 0.5]},
+            }
+        },
+    )
+    b = Directory(tmp_path / "b")
+    b.b = {
+            "c": np.empty((0, 2), dtype="uint16"),
+            "d.bin": data_file(tmp_path / "d0.bin"),
+            "e": {"f": [0.1, 0.2]},
+        }
+    b.extend(
+        "b",
+        {
+            "c": np.uint16([[1, 2], [3, 4]]),
+            "d.bin": data_file(tmp_path / "d1.bin"),
+            "e": {"f": [0.3, 0.4, 0.5]},
+        },
+    )
+    assert_directory_equals(
+        b,
+        {
+            "b": {
+                "c": np.uint16([[1, 2], [3, 4]]),
+                "d.bin": data_file_concat(
+                    tmp_path / "d2.bin", [tmp_path / "d0.bin", tmp_path / "d1.bin"]
+                ),
+                "e": {"f": [0.1, 0.2, 0.3, 0.4, 0.5]},
             }
         },
     )
 
 
 def test_directory_extension(tmp_path: Path) -> None:
     a0 = Directory(tmp_path / "a0")
```

### Comparing `datamate-0.1.7/tests/test_namespaces.py` & `datamate-0.1.8/tests/test_namespaces.py`

 * *Files identical despite different names*

