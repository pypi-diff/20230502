# Comparing `tmp/np_tools-0.1.4.tar.gz` & `tmp/np_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_tools-0.1.4.tar", last modified: Thu Apr 20 00:00:12 2023, max compression
+gzip compressed data, was "np_tools-0.1.6.tar", last modified: Tue May  2 16:22:57 2023, max compression
```

## Comparing `np_tools-0.1.4.tar` & `np_tools-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.4/README.md
--rw-r--r--   0        0        0     2417 2023-04-20 00:00:12.394667 np_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.4/src/np_tools/__init__.py
--rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.4/src/np_tools/config.py
--rw-r--r--   0        0        0     8517 2023-04-19 23:59:55.459560 np_tools-0.1.4/src/np_tools/openephys.py
--rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.4/src/np_tools/remote.py
--rw-r--r--   0        0        0     2754 2023-04-19 22:12:49.593247 np_tools-0.1.4/src/np_tools/tools.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 np_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.6/README.md
+-rw-r--r--   0        0        0     2407 2023-05-02 16:22:57.834073 np_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-19 20:41:36.127176 np_tools-0.1.6/src/np_tools/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.6/src/np_tools/config.py
+-rw-r--r--   0        0        0     8517 2023-04-19 23:59:55.459560 np_tools-0.1.6/src/np_tools/openephys.py
+-rw-r--r--   0        0        0     4196 2023-04-19 20:13:12.296840 np_tools-0.1.6/src/np_tools/remote.py
+-rw-r--r--   0        0        0     4056 2023-04-25 20:24:36.073231 np_tools-0.1.6/src/np_tools/tools.py
+-rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 np_tools-0.1.6/PKG-INFO
```

### Comparing `np_tools-0.1.4/pyproject.toml` & `np_tools-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -71,24 +71,24 @@
 ]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "np_tools"
-version = "0.1.4"
+version = "0.1.6"
 description = "General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
-    "fabric>=3.0.0",
+    "fabric",
+    "invoke<2.1",
     "np-config>=0.4.17",
     "np-logging>=0.5.1",
-    "black>=22.1.0",
 ]
 requires-python = ">=3.7,<4"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `np_tools-0.1.4/src/np_tools/openephys.py` & `np_tools-0.1.6/src/np_tools/openephys.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.4/src/np_tools/remote.py` & `np_tools-0.1.6/src/np_tools/remote.py`

 * *Files identical despite different names*

### Comparing `np_tools-0.1.4/src/np_tools/tools.py` & `np_tools-0.1.6/src/np_tools/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 Tools for working with Open Ephys raw data files.
 """
 from __future__ import annotations
 import contextlib
+import datetime
 import hashlib
 import pathlib
 import shutil
 import subprocess
 import sys
-from typing import Iterable
+import time
+from typing import Iterable, Optional
+
+import np_config
 import np_logging
 
 
 logger = np_logging.get_logger(__name__)
 
 
 def checksum(path: str | pathlib.Path) -> str:
@@ -81,7 +85,37 @@
     dir_size = 0
     dir_size += sum(
         f.stat().st_size
         for f in pathlib.Path(path).rglob('*')
         if pathlib.Path(f).is_file()
     )
     return dir_size
+
+
+def free_gb(path: str | bytes | pathlib.Path) -> float:
+    "Return free space at `path`, to .1 GB. Raises FileNotFoundError if `path` not accessible."
+    path = pathlib.Path(path)
+    path = np_config.unc_to_local(path)
+    return round(shutil.disk_usage(path).free / 1e9, 1)
+
+
+def get_files_created_between(
+    path: str | bytes | pathlib.Path,
+    glob: str = "*",
+    start: float | datetime.datetime = 0,
+    end: Optional[float | datetime.datetime] = None,
+    reverse: bool = False,
+) -> tuple[pathlib.Path, ...]:
+    """Recusively get search for files in subfolders of `path` created between `start` and `end`.
+    
+    Sequence is sorted by ascending creation time (oldest first). `reverse` reverses this order.
+    """
+    path = pathlib.Path(path)
+    if not path.is_dir():
+        raise ValueError(f'{path} is not a directory, cannot glob for files')
+    if not end:
+        end = time.time()
+    start = start.timestamp() if isinstance(start, datetime.datetime) else start
+    end = end.timestamp() if isinstance(end, datetime.datetime) else end
+    ctime = lambda x: x.stat().st_ctime
+    files = (file for file in path.rglob(glob) if int(start) <= ctime(file) <= end)
+    return tuple(sorted(files, key=ctime, reverse=reverse))
```

### Comparing `np_tools-0.1.4/PKG-INFO` & `np_tools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-tools
-Version: 0.1.4
+Version: 0.1.6
 Summary: General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows.
 Author-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Repository, https://github.com/AllenInstitute/np_tools
 Project-URL: Bug tracker, https://github.com/AllenInstitute/np_tools/issues
 Requires-Python: <4,>=3.7
-Requires-Dist: fabric>=3.0.0
+Requires-Dist: fabric
+Requires-Dist: invoke<2.1
 Requires-Dist: np-config>=0.4.17
 Requires-Dist: np-logging>=0.5.1
-Requires-Dist: black>=22.1.0
 Requires-Dist: blue>=0.9.1; extra == "dev"
 Requires-Dist: pytest>=7.2.2; extra == "dev"
 Requires-Dist: mypy>=1.1.1; extra == "dev"
 Requires-Dist: coverage[toml]>=7.2.2; extra == "dev"
 Requires-Dist: pdm>=2.4.9; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: bump>=1.3.2; extra == "dev"
```

