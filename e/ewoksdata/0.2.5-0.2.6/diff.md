# Comparing `tmp/ewoksdata-0.2.5.tar.gz` & `tmp/ewoksdata-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdata-0.2.5.tar", last modified: Tue Apr 25 11:46:26 2023, max compression
+gzip compressed data, was "dist/ewoksdata-0.2.6.tar", last modified: Tue May  2 09:51:58 2023, max compression
```

## Comparing `ewoksdata-0.2.5.tar` & `ewoksdata-0.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-25 11:44:45.000000 ewoksdata-0.2.5/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:46:20.000000 ewoksdata-0.2.5/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8187 2023-04-25 07:40:11.000000 ewoksdata-0.2.5/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6086 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:46:20.000000 ewoksdata-0.2.5/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_data_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-02 08:58:44.000000 ewoksdata-0.2.6/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 09:51:52.000000 ewoksdata-0.2.6/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8413 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 09:51:52.000000 ewoksdata-0.2.6/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.2.5/LICENSE.md` & `ewoksdata-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.5/PKG-INFO` & `ewoksdata-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.5
+Version: 0.2.6
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.5/setup.cfg` & `ewoksdata-0.2.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -48,19 +48,14 @@
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 
-[build_sphinx]
-project = ewoksdata
-version = attr: ewoksdata.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [egg_info]
 tag_build =
```

### Comparing `ewoksdata-0.2.5/src/ewoksdata/data/bliss.py` & `ewoksdata-0.2.6/src/ewoksdata/data/bliss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import logging
 from numbers import Integral, Number
 from typing import Iterator, List, Optional, Tuple, Sequence, Union
 
 import numpy
 import h5py
 import hdf5plugin  # noqa F401
@@ -26,32 +27,37 @@
 logger = logging.getLogger(__name__)
 
 
 def get_data(
     data: Union[str, ArrayLike, Number], **options
 ) -> Union[numpy.ndarray, Number]:
     if isinstance(data, str):
-        filename, h5path, idx = url.h5dataset_url_parse(data)
+        data_url = url.as_dataurl(data)
+        filename, h5path, idx = url.h5dataset_url_parse(data_url)
         if filename.endswith(".h5") or filename.endswith(".nx"):
-            return get_hdf5_data(filename, h5path, idx=idx, **options)
-        else:
-            return silx_get_data(data)
+            return _get_hdf5_data(filename, h5path, idx=idx, **options)
+        if not data_url.scheme():
+            if sys.platform == "win32":
+                data_url = f"fabio:///{data}"
+            else:
+                data_url = f"fabio://{data}"
+        return silx_get_data(data_url)
     elif isinstance(data, (Sequence, Number, numpy.ndarray)):
         return data
     else:
         raise TypeError(type(data))
 
 
 def get_image(*args, **kwargs) -> numpy.ndarray:
     data = get_data(*args, **kwargs)
     return numpy.atleast_2d(numpy.squeeze(data))
 
 
 @h5py_utils.retry()
-def get_hdf5_data(filename: str, h5path: str, idx=None, **options) -> numpy.ndarray:
+def _get_hdf5_data(filename: str, h5path: str, idx=None, **options) -> numpy.ndarray:
     with hdf5.h5context(filename, h5path, **options) as dset:
         if _is_bliss_file(dset):
             if "end_time" not in nexus.get_nxentry(dset):
                 raise retrymod.RetryError
         if idx is None:
             idx = tuple()
         return dset[idx]
```

### Comparing `ewoksdata-0.2.5/src/ewoksdata/data/hdf5/__init__.py` & `ewoksdata-0.2.6/src/ewoksdata/data/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.5/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.2.6/src/ewoksdata/data/hdf5/config.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.5/src/ewoksdata/data/hdf5/dataset_writer.py` & `ewoksdata-0.2.6/src/ewoksdata/data/hdf5/dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.5/src/ewoksdata/data/nexus.py` & `ewoksdata-0.2.6/src/ewoksdata/data/nexus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from contextlib import contextmanager
 from typing import Union, Iterator, Optional, Tuple
 
 import h5py
-from silx.io.url import DataUrl
 from silx.io import h5py_utils
+from .url import DataUrl
+from .url import as_dataurl
 
 
 def ensure_nxclass(group: h5py.Group) -> None:
     if group.attrs.get("NX_class"):
         return
     groups = [s for s in group.name.split("/") if s]
     n = len(groups)
@@ -26,21 +27,21 @@
         if not name:
             continue
         parent.attrs["default"] = name
         parent = parent.parent
 
 
 def create_url(url: str, **open_options) -> DataUrl:
-    url = DataUrl(url)
+    url = as_dataurl(url)
     filename = url.file_path()
     os.makedirs(os.path.dirname(filename), exist_ok=True)
     open_options.setdefault("mode", "a")
     with h5py_utils.open_item(filename, "/", **open_options) as parent:
         h5item, _ = _create_h5group(parent, url.data_path())
-        return DataUrl(f"{filename}::{h5item.name}")
+        return as_dataurl(f"{filename}::{h5item.name}")
 
 
 def get_nxentry(h5item: Union[h5py.Dataset, h5py.Group]):
     parts = [s for s in h5item.name.split("/") if s]
     if parts:
         return h5item.file[parts[0]]
     raise ValueError("HDF5 item must be part of an NXentry")
@@ -53,16 +54,15 @@
     retry_period=None,
     default_levels: Optional[Tuple[str]] = None,
     **open_options,
 ) -> Iterator[Tuple[h5py.Group, bool]]:
     """
     :yields: (h5group, already_existed)
     """
-    if not isinstance(url, DataUrl):
-        url = DataUrl(url)
+    url = as_dataurl(url)
     filename = url.file_path()
     itemname = url.data_path()
     if not itemname:
         itemname = "/"
     if os.path.dirname(filename):
         os.makedirs(os.path.dirname(filename), exist_ok=True)
     open_options.setdefault("mode", "a")
```

### Comparing `ewoksdata-0.2.5/src/ewoksdata/data/utils.py` & `ewoksdata-0.2.6/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.5/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.2.6/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.5/src/ewoksdata/tests/test_dataset_writer.py` & `ewoksdata-0.2.6/src/ewoksdata/tests/test_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.5/src/ewoksdata.egg-info/PKG-INFO` & `ewoksdata-0.2.6/src/ewoksdata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.5
+Version: 0.2.6
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.5/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.2.6/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

