# Comparing `tmp/lazycsv-1.0.3.tar.gz` & `tmp/lazycsv-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycsv-1.0.3.tar", last modified: Fri Apr 21 01:33:16 2023, max compression
+gzip compressed data, was "lazycsv-1.1.0.tar", last modified: Tue May  2 03:26:44 2023, max compression
```

## Comparing `lazycsv-1.0.3.tar` & `lazycsv-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.534634 lazycsv-1.0.3/
--rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.0.3/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     8560 2023-04-21 01:33:16.534634 lazycsv-1.0.3/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     7879 2023-04-18 16:19:33.000000 lazycsv-1.0.3/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-21 01:33:16.534634 lazycsv-1.0.3/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2042 2023-04-21 01:32:31.000000 lazycsv-1.0.3/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.531301 lazycsv-1.0.3/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.531301 lazycsv-1.0.3/src/lazycsv/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.0.3/src/lazycsv/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    35127 2023-04-21 01:31:44.000000 lazycsv-1.0.3/src/lazycsv/lazycsv.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.534634 lazycsv-1.0.3/src/lazycsv.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     8560 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.534634 lazycsv-1.0.3/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    21311 2023-04-20 23:50:41.000000 lazycsv-1.0.3/tests/test_lazycsv.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.0/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     8936 2023-05-02 03:26:44.032390 lazycsv-1.1.0/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     8255 2023-05-01 23:49:17.000000 lazycsv-1.1.0/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-02 03:26:44.032390 lazycsv-1.1.0/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2034 2023-05-02 03:25:32.000000 lazycsv-1.1.0/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/src/lazycsv/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.0/src/lazycsv/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    39297 2023-05-02 02:35:46.000000 lazycsv-1.1.0/src/lazycsv/lazycsv.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/src/lazycsv.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8936 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       67 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    23362 2023-05-01 23:23:30.000000 lazycsv-1.1.0/tests/test_lazycsv.py
```

### Comparing `lazycsv-1.0.3/LICENSE` & `lazycsv-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycsv-1.0.3/PKG-INFO` & `lazycsv-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.0.3
+Version: 1.1.0
 Summary: an OOM csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -88,21 +88,34 @@
 ['1', 'a1', 'b1']
 >>>
 >>> import numpy as np
 >>> np.fromiter(map(int, lazy.sequence(col=0)), dtype=np.int64)
 array([0, 1])
 ```
 
+The `lazy` object also supports indexing operations for expressive iterables.
+The axis for iteration can be passed as a slice object, and the index of the
+iterable can be passed as a integer. Individual coordinate values can also be
+passed as a pair of integers, this call will eagerly return the value at that
+index.
+
+```python
+>>> list(lazy[::-1, 1])
+[b'a1', b'a0']
+>>> lazy[-1, -1]
+b"b1"
+```
+
 Iterators can be materialized at any point by calling the `to_list()` or
 `to_numpy()` methods on the iterator object (to enable optional numpy support,
 see the Numpy section of this document). These methods exhaust the iterator,
 placing the remaining PyBytes values into a PyObject.
 
 ```python
->>> col = lazy.sequence(col=0)
+>>> col = lazy[:, 0]
 >>> next(col)
 b'0'
 >>> col.to_list()
 [b'1']
 >>>
 ```
 
@@ -118,15 +131,15 @@
 >>> lazy.headers
 (b'', b'ALPHA', b'BETA')
 >>> (col := lazy.sequence(col=1))
 <lazycsv_iterator object at 0x7f599fd86b50>
 >>> list(col)
 [b'a0', b'a1']
 >>> lazy = lazycsv.LazyCSV(FPATH, skip_headers=True)
->>> (col := lazy.sequence(col=1))
+>>> (col := lazy[:, 1])
 <lazycsv_iterator object at 0x7f59d1b21890>
 >>> list(col)
 [b'ALPHA', b'a0', b'a1']
 ```
 
 Fields which are double-quoted by default are yielded without quotes. This
 behavior can be disabled by passing `unquoted=False` to the object constructor.
@@ -178,17 +191,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.5116381410043687
-parsing cols... time to parse: 1.5931394950021058
-total time: 2.1047776360064745
+indexing lazy... time to index: 0.4978358040098101
+parsing cols... time to parse: 1.8409163669857662
+total time: 2.3387521709955763
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -202,17 +215,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.990824360997067
-parsing cols... time to parse: 19.573407171003055
-total time: 24.56423153200012
+indexing lazy... time to index: 4.978727137990063
+parsing cols... time to parse: 23.64216143201338
+total time: 28.620888570003444
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
```

### Comparing `lazycsv-1.0.3/README.md` & `lazycsv-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,21 +68,34 @@
 ['1', 'a1', 'b1']
 >>>
 >>> import numpy as np
 >>> np.fromiter(map(int, lazy.sequence(col=0)), dtype=np.int64)
 array([0, 1])
 ```
 
+The `lazy` object also supports indexing operations for expressive iterables.
+The axis for iteration can be passed as a slice object, and the index of the
+iterable can be passed as a integer. Individual coordinate values can also be
+passed as a pair of integers, this call will eagerly return the value at that
+index.
+
+```python
+>>> list(lazy[::-1, 1])
+[b'a1', b'a0']
+>>> lazy[-1, -1]
+b"b1"
+```
+
 Iterators can be materialized at any point by calling the `to_list()` or
 `to_numpy()` methods on the iterator object (to enable optional numpy support,
 see the Numpy section of this document). These methods exhaust the iterator,
 placing the remaining PyBytes values into a PyObject.
 
 ```python
->>> col = lazy.sequence(col=0)
+>>> col = lazy[:, 0]
 >>> next(col)
 b'0'
 >>> col.to_list()
 [b'1']
 >>>
 ```
 
@@ -98,15 +111,15 @@
 >>> lazy.headers
 (b'', b'ALPHA', b'BETA')
 >>> (col := lazy.sequence(col=1))
 <lazycsv_iterator object at 0x7f599fd86b50>
 >>> list(col)
 [b'a0', b'a1']
 >>> lazy = lazycsv.LazyCSV(FPATH, skip_headers=True)
->>> (col := lazy.sequence(col=1))
+>>> (col := lazy[:, 1])
 <lazycsv_iterator object at 0x7f59d1b21890>
 >>> list(col)
 [b'ALPHA', b'a0', b'a1']
 ```
 
 Fields which are double-quoted by default are yielded without quotes. This
 behavior can be disabled by passing `unquoted=False` to the object constructor.
@@ -158,17 +171,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.5116381410043687
-parsing cols... time to parse: 1.5931394950021058
-total time: 2.1047776360064745
+indexing lazy... time to index: 0.4978358040098101
+parsing cols... time to parse: 1.8409163669857662
+total time: 2.3387521709955763
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -182,17 +195,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.990824360997067
-parsing cols... time to parse: 19.573407171003055
-total time: 24.56423153200012
+indexing lazy... time to index: 4.978727137990063
+parsing cols... time to parse: 23.64216143201338
+total time: 28.620888570003444
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
```

### Comparing `lazycsv-1.0.3/setup.py` & `lazycsv-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,57 +2,53 @@
 
 from setuptools import Extension, find_packages, setup
 
 LAZYCSV_DEBUG = int(os.environ.get("LAZYCSV_DEBUG", 0))
 LAZYCSV_INDEX_DTYPE = os.environ.get("LAZYCSV_INDEX_DTYPE", "uint16_t")
 
 LAZYCSV_INCLUDE_NUMPY = int(os.environ.get("LAZYCSV_INCLUDE_NUMPY", 0))
-LAZYCSV_INCLUDE_NUMPY_LEGACY = int(
-    os.environ.get("LAZYCSV_INCLUDE_NUMPY_LEGACY", 0)
-)
+LAZYCSV_INCLUDE_NUMPY_LEGACY = int(os.environ.get("LAZYCSV_INCLUDE_NUMPY_LEGACY", 0))
 
 include_dirs = (
     [__import__("numpy").get_include()]
-    if (LAZYCSV_INCLUDE_NUMPY|LAZYCSV_INCLUDE_NUMPY_LEGACY)
+    if (LAZYCSV_INCLUDE_NUMPY | LAZYCSV_INCLUDE_NUMPY_LEGACY)
     else []
 )
 
 if not LAZYCSV_INDEX_DTYPE.startswith(("unsigned", "uint")):
-    raise ValueError(
-        "specified LAZYCSV_INDEX_DTYPE must be an unsigned integer type"
-    )
+    raise ValueError("specified LAZYCSV_INDEX_DTYPE must be an unsigned integer type")
 
 extensions = [
     Extension(
         "lazycsv.lazycsv",
         [os.path.join("src", "lazycsv", "lazycsv.c")],
         include_dirs=include_dirs,
         define_macros=[
             ("INDEX_DTYPE", LAZYCSV_INDEX_DTYPE),
             ("INCLUDE_NUMPY", LAZYCSV_INCLUDE_NUMPY),
             ("INCLUDE_NUMPY_LEGACY", LAZYCSV_INCLUDE_NUMPY_LEGACY),
-            ("DEBUG", LAZYCSV_DEBUG)
+            ("DEBUG", LAZYCSV_DEBUG),
         ],
     )
 ]
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lazycsv",
-    version="1.0.3",
+    version="1.1.0",
     author="Michael Green, Chris Perkins",
     author_email="dev@crunch.io",
     description="an OOM csv parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     extras_require={
-        "test": ["pytest"],
+        "test": ["pytest", "numpy"],
         "benchmarks": ["datatable", "pandas", "pyarrow", "polars"],
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `lazycsv-1.0.3/src/lazycsv/lazycsv.c` & `lazycsv-1.1.0/src/lazycsv/lazycsv.c`

 * *Files 5% similar despite different names*

```diff
@@ -107,24 +107,24 @@
     char _newline;
     LazyCSV_Index* _index;
     LazyCSV_File* _data;
     LazyCSV_Cache* _cache;
 } LazyCSV;
 
 
-typedef struct {
+typedef struct lazycsv_iter {
     PyObject_HEAD
     PyObject* lazy;
     size_t row;
     size_t col;
     size_t position;
     size_t stop;
     size_t step;
+    void (*fn)(struct lazycsv_iter*, size_t*, size_t*);
     char reversed;
-    char skip_header;
 } LazyCSV_Iter;
 
 
 static inline void _BufferWrite(int fd, LazyCSV_Buffer *buffer, void *data,
                                 size_t size) {
 
     if (buffer->size + size >= buffer->capacity) {
@@ -224,23 +224,18 @@
 
 
 static inline void LazyCSV_IterCol(LazyCSV_Iter *iter, size_t *offset,
                                    size_t *len) {
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
     if (iter->position < iter->stop) {
-
-        size_t position;
-
-        if (iter->reversed) {
-            position = lazy->rows - 1 - iter->position + !lazy->_skip_headers;
-        }
-        else {
-            position = iter->position + !lazy->_skip_headers;
-        }
+        size_t position =
+            iter->reversed
+                ? lazy->rows - 1 - iter->position + !lazy->_skip_headers
+                : iter->position + !lazy->_skip_headers;
 
         iter->position += iter->step;
 
         char* newlines = lazy->_index->newlines->data;
         char* anchors = lazy->_index->anchors->data;
         char* commas = lazy->_index->commas->data;
 
@@ -261,16 +256,16 @@
 
 
 static inline void LazyCSV_IterRow(LazyCSV_Iter *iter, size_t *offset,
                                    size_t *len) {
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
     if (iter->position < iter->stop) {
-        size_t position = iter->reversed ?
-            lazy->cols - iter->position - 1 : iter->position;
+        size_t position =
+            iter->reversed ? lazy->cols - iter->position - 1 : iter->position;
 
         iter->position += iter->step;
 
         char* newlines = lazy->_index->newlines->data;
         char* anchors = lazy->_index->anchors->data;
         char* commas = lazy->_index->commas->data;
 
@@ -333,27 +328,15 @@
 
 static PyObject* LazyCSV_IterNext(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
     size_t offset = SIZE_MAX, len;
 
-    if (iter->col != SIZE_MAX) {
-        LazyCSV_IterCol(iter, &offset, &len);
-    }
-    else if (iter->row != SIZE_MAX) {
-        LazyCSV_IterRow(iter, &offset, &len);
-    }
-    else {
-        PyErr_SetString(
-            PyExc_RuntimeError,
-            "could not determine axis for materialization"
-        );
-        return NULL;
-    }
+    iter->fn(iter, &offset, &len);
 
     if (offset==SIZE_MAX) {
         PyErr_SetNone(PyExc_StopIteration);
         return NULL;
     }
 
     return PyBytes_FromOffsetAndLen(lazy, offset, len);
@@ -361,38 +344,35 @@
 
 
 static PyObject* LazyCSV_IterAsList(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV* lazy = (LazyCSV*)iter->lazy;
 
     size_t size;
-    void (*IterFn)(LazyCSV_Iter*, size_t*, size_t*);
 
     if (iter->col != SIZE_MAX) {
         size = lazy->rows - iter->position;
-        IterFn = LazyCSV_IterCol;
     }
     else if (iter->row != SIZE_MAX) {
         size = lazy->cols - iter->position;
-        IterFn = LazyCSV_IterRow;
     }
     else {
         PyErr_SetString(
             PyExc_RuntimeError,
             "could not determine axis for materialization"
         );
         return NULL;
     }
 
     PyObject* result = PyList_New(size);
     size_t offset, len;
 
     PyObject* item;
     for (size_t i = 0; i < size; i++) {
-        IterFn(iter, &offset, &len);
+        iter->fn(iter, &offset, &len);
         item = PyBytes_FromOffsetAndLen(lazy, offset, len);
         PyList_SET_ITEM(result, i, item);
     }
 
     return result;
 }
 
@@ -1065,14 +1045,16 @@
 }
 
 
 static PyObject *LazyCSV_Seq(PyObject *self, PyObject *args, PyObject *kwargs) {
 
     size_t row = SIZE_MAX;
     size_t col = SIZE_MAX;
+    size_t stop;
+    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
     char reversed;
 
     static char *kwlist[] = {"row", "col", "reversed", NULL};
 
     char ok = PyArg_ParseTupleAndKeywords(
         args, kwargs, "|nnb", kwlist, &row, &col, &reversed
     );
@@ -1097,55 +1079,65 @@
         PyErr_SetString(
             PyExc_ValueError,
             "cannot specify both row and col"
         );
         return NULL;
     }
 
+    if (col != SIZE_MAX) {
+        fn = LazyCSV_IterCol;
+        stop = ((LazyCSV*)self)->rows;
+    }
+    else if (row != SIZE_MAX) {
+        fn = LazyCSV_IterRow;
+        stop = ((LazyCSV*)self)->cols;
+    }
+    else {
+        PyErr_SetString(
+            PyExc_RuntimeError,
+            "could not determine axis for materialization"
+        );
+        return NULL;
+    }
+
     PyTypeObject* type = &LazyCSV_IterType;
     LazyCSV_Iter* iter = (LazyCSV_Iter*)type->tp_alloc(type, 0);
 
     if (!iter) {
         PyErr_SetString(
             PyExc_MemoryError,
             "unable to allocate memory for iterable"
         );
         return NULL;
     }
 
-    LazyCSV* lazy = (LazyCSV*)self;
-
     iter->row = row;
     iter->col = col;
     iter->reversed = reversed;
     iter->position = 0;
     iter->step = 1;
-    iter->stop = col == SIZE_MAX ? lazy->cols : lazy->rows;
+    iter->stop = stop;
     iter->lazy = self;
+    iter->fn = fn;
 
     Py_INCREF(self);
 
     return (PyObject*)iter;
 }
 
 
 static PyObject* LazyCSV_GetValue(PyObject* self, PyObject* r, PyObject* c) {
 
-    Py_ssize_t row = PyLong_AsSsize_t(r);
-    Py_ssize_t col = PyLong_AsSsize_t(c);
+    Py_ssize_t _row = PyLong_AsSsize_t(r);
+    Py_ssize_t _col = PyLong_AsSsize_t(c);
 
     LazyCSV* lazy = (LazyCSV*)self;
 
-    if (row < 0) {
-        row = lazy->rows + row;
-    }
-
-    if (col < 0) {
-        col = lazy->cols + col;
-    }
+    size_t row = _row < 0 ? lazy->rows + _row : (size_t)_row;
+    size_t col = _col < 0 ? lazy->cols + _col : (size_t)_col;
 
     int row_in_bounds = (
         0 <= row && row < lazy->rows
     );
 
     int col_in_bounds = (
         0 <= col && col < lazy->cols
@@ -1186,32 +1178,172 @@
         PyErr_SetString(
             PyExc_ValueError,
             "index must contain both a row and column value"
         );
         return NULL;
     }
 
-    PyObject *row, *col;
+    PyObject *row_obj, *col_obj;
 
-    if (!PyArg_ParseTuple(key, "OO", &row, &col)) {
+    if (!PyArg_ParseTuple(key, "OO", &row_obj, &col_obj)) {
         PyErr_SetString(
             PyExc_RuntimeError,
             "unable to parse index key"
         );
         return NULL;
     }
 
-    if (PyLong_Check(row) && PyLong_Check(col))
-        return LazyCSV_GetValue(self, row, col);
+    if (PyLong_Check(row_obj) && PyLong_Check(col_obj))
+        return LazyCSV_GetValue(self, row_obj, col_obj);
+
+    int row_is_slice = PySlice_Check(row_obj);
+    int col_is_slice = PySlice_Check(col_obj);
+
+    LazyCSV* lazy = (LazyCSV*)self;
+
+    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
+
+    if (row_is_slice && !col_is_slice) {
+        PySliceObject* row_slice = (PySliceObject*)row_obj;
+
+        Py_ssize_t _col = PyLong_AsSsize_t(col_obj);
+        size_t col = _col < 0 ? lazy->cols + _col : (size_t)_col;
+
+        int col_in_bounds = (
+            0 <= col && col < lazy->cols
+        );
+
+        if (!col_in_bounds) goto boundary_err;
+
+        Py_ssize_t _start = row_slice->start == Py_None
+                                ? (Py_ssize_t)0
+                                : PyLong_AsSsize_t(row_slice->start);
+        Py_ssize_t _stop = row_slice->stop == Py_None
+                               ? (Py_ssize_t)lazy->rows
+                               : PyLong_AsSsize_t(row_slice->stop);
+        Py_ssize_t _step =
+            row_slice->step == Py_None ? 1 : PyLong_AsSsize_t(row_slice->step);
+
+        size_t start = _start < 0 ? lazy->rows + _start : (size_t)_start;
+        size_t stop = _stop < 0 ? lazy->rows + _stop : (size_t)_stop;
+
+        size_t step;
+        char reversed = 0;
+
+        if (_step < 0) {
+            reversed = 1;
+            step = (size_t)(-1 * _step);
+            if (row_slice->start != Py_None) {
+                start = lazy->rows - start - 1;
+            }
+            if (row_slice->stop != Py_None) {
+                stop = lazy->rows - stop - 1;
+            }
+        }
+        else {
+            step = (size_t)_step;
+        }
+
+        PyTypeObject* type = &LazyCSV_IterType;
+        LazyCSV_Iter* iter = (LazyCSV_Iter*)type->tp_alloc(type, 0);
+        if (!iter) goto memory_err;
+
+        iter->row = SIZE_MAX;
+        iter->col = col;
+        iter->reversed = reversed;
+        iter->position = start;
+        iter->step = step;
+        iter->stop = stop;
+        iter->lazy = self;
+        iter->fn = LazyCSV_IterCol;
+        Py_INCREF(self);
+
+        return (PyObject*)iter;
+    }
+
+    if (col_is_slice && !row_is_slice) {
+        PySliceObject* col_slice = (PySliceObject*)col_obj;
+
+        Py_ssize_t _row = PyLong_AsSsize_t(row_obj);
+        size_t row = _row < 0 ? lazy->rows + _row : (size_t)_row;
+
+        int row_in_bounds = (
+            0 <= row && row < lazy->rows
+        );
+
+        if (!row_in_bounds) goto boundary_err;
+
+        Py_ssize_t _start = col_slice->start == Py_None
+                                ? (Py_ssize_t)0
+                                : PyLong_AsSsize_t(col_slice->start);
+        Py_ssize_t _stop = col_slice->stop == Py_None
+                               ? (Py_ssize_t)lazy->cols
+                               : PyLong_AsSsize_t(col_slice->stop);
+        Py_ssize_t _step =
+            col_slice->step == Py_None ? 1 : PyLong_AsSsize_t(col_slice->step);
+
+        size_t start = _start < 0 ? lazy->cols + _start : (size_t)_start;
+        size_t stop = _stop < 0 ? lazy->cols + _stop : (size_t)_stop;
+
+        size_t step;
+        char reversed = 0;
+
+        if (_step < 0) {
+            step = (size_t)(-1 * _step);
+            reversed = 1;
+            if (col_slice->start != Py_None) {
+                start = lazy->cols - start - 1;
+            }
+            if (col_slice->stop != Py_None) {
+                stop = lazy->cols - stop - 1;
+            }
+        }
+        else {
+            step = (size_t)_step;
+        }
+
+        PyTypeObject* type = &LazyCSV_IterType;
+        LazyCSV_Iter* iter = (LazyCSV_Iter*)type->tp_alloc(type, 0);
+        if (!iter) goto memory_err;
+
+        iter->row = row;
+        iter->col = SIZE_MAX;
+        iter->reversed = reversed;
+        iter->position = start;
+        iter->step = step;
+        iter->stop = stop;
+        iter->fn = LazyCSV_IterRow;
+        iter->lazy = self;
+        Py_INCREF(self);
+
+        return (PyObject*)iter;
+    }
+
+    goto schema_err;
 
+schema_err:
     PyErr_SetString(
         PyExc_ValueError,
         "given indexing schema is not supported"
     );
     return NULL;
+
+memory_err:
+    PyErr_SetString(
+        PyExc_MemoryError,
+        "unable to allocate memory for iterable"
+    );
+    return NULL;
+
+boundary_err:
+    PyErr_SetString(
+        PyExc_ValueError,
+        "provided value not in bounds of index"
+    );
+    return NULL;
 }
 
 
 static PyMemberDef LazyCSV_Members[] = {
     {"headers", T_OBJECT, offsetof(LazyCSV, headers), READONLY, "header tuple"},
     {"rows", T_LONG, offsetof(LazyCSV, rows), READONLY, "row length"},
     {"cols", T_LONG, offsetof(LazyCSV, cols), READONLY, "col length"},
```

### Comparing `lazycsv-1.0.3/src/lazycsv.egg-info/PKG-INFO` & `lazycsv-1.1.0/src/lazycsv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.0.3
+Version: 1.1.0
 Summary: an OOM csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -88,21 +88,34 @@
 ['1', 'a1', 'b1']
 >>>
 >>> import numpy as np
 >>> np.fromiter(map(int, lazy.sequence(col=0)), dtype=np.int64)
 array([0, 1])
 ```
 
+The `lazy` object also supports indexing operations for expressive iterables.
+The axis for iteration can be passed as a slice object, and the index of the
+iterable can be passed as a integer. Individual coordinate values can also be
+passed as a pair of integers, this call will eagerly return the value at that
+index.
+
+```python
+>>> list(lazy[::-1, 1])
+[b'a1', b'a0']
+>>> lazy[-1, -1]
+b"b1"
+```
+
 Iterators can be materialized at any point by calling the `to_list()` or
 `to_numpy()` methods on the iterator object (to enable optional numpy support,
 see the Numpy section of this document). These methods exhaust the iterator,
 placing the remaining PyBytes values into a PyObject.
 
 ```python
->>> col = lazy.sequence(col=0)
+>>> col = lazy[:, 0]
 >>> next(col)
 b'0'
 >>> col.to_list()
 [b'1']
 >>>
 ```
 
@@ -118,15 +131,15 @@
 >>> lazy.headers
 (b'', b'ALPHA', b'BETA')
 >>> (col := lazy.sequence(col=1))
 <lazycsv_iterator object at 0x7f599fd86b50>
 >>> list(col)
 [b'a0', b'a1']
 >>> lazy = lazycsv.LazyCSV(FPATH, skip_headers=True)
->>> (col := lazy.sequence(col=1))
+>>> (col := lazy[:, 1])
 <lazycsv_iterator object at 0x7f59d1b21890>
 >>> list(col)
 [b'ALPHA', b'a0', b'a1']
 ```
 
 Fields which are double-quoted by default are yielded without quotes. This
 behavior can be disabled by passing `unquoted=False` to the object constructor.
@@ -178,17 +191,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.5116381410043687
-parsing cols... time to parse: 1.5931394950021058
-total time: 2.1047776360064745
+indexing lazy... time to index: 0.4978358040098101
+parsing cols... time to parse: 1.8409163669857662
+total time: 2.3387521709955763
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -202,17 +215,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.990824360997067
-parsing cols... time to parse: 19.573407171003055
-total time: 24.56423153200012
+indexing lazy... time to index: 4.978727137990063
+parsing cols... time to parse: 23.64216143201338
+total time: 28.620888570003444
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
```

### Comparing `lazycsv-1.0.3/tests/test_lazycsv.py` & `lazycsv-1.1.0/tests/test_lazycsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
 import numpy as np
 import pytest
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 FPATH = os.path.join(HERE, "fixtures/file.csv")
 
+INDEX_COLLECTION = [None, *range(-9, 0), *range(1, 10)]
+
+SLICE_INDEXES = [
+    (a, b, c)
+    for a in INDEX_COLLECTION
+    for b in INDEX_COLLECTION
+    for c in INDEX_COLLECTION
+]
+
 
 @pytest.fixture
 def lazy():
     lazy = lazycsv.LazyCSV(FPATH)
     yield lazy
 
 
@@ -87,14 +96,31 @@
         actual = list(lazy.sequence(col=0))
         assert actual == [b"0", b"1"]
         actual = list(lazy.sequence(col=1))
         assert actual == [b"a0", b"a1"]
         actual = list(lazy.sequence(col=2))
         assert actual == [b"b0", b"b1"]
 
+    def test_get_column_slice(self, lazy):
+        actual = list(lazy[:, 1])
+        assert actual == [b"a0", b"a1"]
+        with pytest.raises(ValueError) as err:
+            _ = list(lazy[:, -5])
+        assert err.value.args == ("provided value not in bounds of index",)
+
+    def test_get_col_slice_variety(self, lazy):
+        actual = b"INDEX\n0\n1\n2\n3\n4\n5\n6\n7\n8\n9\n"
+        with prepped_file(actual) as tempf:
+            lazy = lazycsv.LazyCSV(tempf.name)
+            for indexes in SLICE_INDEXES:
+                _slice = slice(*indexes)
+                expected = list(range(10))[_slice]
+                actual = list(map(int, lazy[_slice, 0]))
+                assert actual == expected
+
     def test_get_actual_col(self):
         actual = b"INDEX,ATTR\n0,a\n1,b\n2,c\n3,d\n"
         with prepped_file(actual) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name)
             assert list(lazy.sequence(col=0)) == [b"0", b"1", b"2", b"3"]
             assert list(lazy.sequence(col=1)) == [b"a", b"b", b"c", b"d"]
             assert lazy.headers == (b"INDEX", b"ATTR")
@@ -121,14 +147,41 @@
 
     def test_get_row(self, lazy):
         row_0 = list(lazy.sequence(row=0))
         assert row_0 == [b"0", b"a0", b"b0"]
         row_1 = list(lazy.sequence(row=1))
         assert row_1 == [b"1", b"a1", b"b1"]
 
+    def test_get_row_getitem(self, lazy):
+        row_0 = list(lazy[0, :])
+        assert row_0 == [b"0", b"a0", b"b0"]
+        with pytest.raises(ValueError) as err:
+            _ = list(lazy[-5, :])
+        assert err.value.args == ("provided value not in bounds of index",)
+
+    def test_get_row_slice_variety(self):
+        actual = b"A,B,C,D,E,F,G,H,I,J\n0,1,2,3,4,5,6,7,8,9\n"
+        with prepped_file(actual) as tempf:
+            lazy = lazycsv.LazyCSV(tempf.name)
+            for indexes in SLICE_INDEXES:
+                _slice = slice(*indexes)
+                expected = list(range(10))[_slice]
+                actual = list(map(int, lazy[0, _slice]))
+                assert actual == expected
+
+    def test_get_row_slice_skipped_headers(self):
+        actual = b"A,B,C,D,E,F,G,H,I,J\n0,1,2,3,4,5,6,7,8,9\n"
+        with prepped_file(actual) as tempf:
+            lazy = lazycsv.LazyCSV(tempf.name, skip_headers=True)
+            for indexes in SLICE_INDEXES:
+                _slice = slice(*indexes)
+                expected = list(range(10))[_slice]
+                actual = list(map(int, lazy[1, _slice]))
+                assert actual == expected
+
     def test_empty_csv(self):
         lazy = lazycsv.LazyCSV("fixtures/file_empty.csv")
         actual = [list(lazy.sequence(col=i)) for i in range(lazy.cols)]
         assert actual == [[b"", b""], [b"", b""], [b"", b""]]
 
     def test_headless_empty_csv(self):
         actual = b",\n,\n,\n"
@@ -155,15 +208,15 @@
         with prepped_file(data) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name)
             assert lazy[0, 0] == lazy[-3, -3] == b"0x0"
             assert lazy[1, 1] == lazy[-2, -2] == b"1x1"
             assert lazy[2, 2] == lazy[-1, -1] == b"2x2"
             with pytest.raises(ValueError) as err:
                 lazy[3, 3]
-            assert ('provided value not in bounds of index',) == err.value.args
+            assert ("provided value not in bounds of index",) == err.value.args
 
     def test_getitem_empty(self, lazy):
         data = b",,\n0x0,0x1,0x2\n1x0,,1x2\n2x0,2x1,2x2\n"
         with prepped_file(data) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name)
             assert lazy[1, 1] == b""
 
@@ -172,15 +225,15 @@
         with prepped_file(data) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name, skip_headers=True)
             assert lazy[0, 0] == lazy[-3, -3] == b"0x0"
             assert lazy[1, 1] == lazy[-2, -2] == b"1x1"
             assert lazy[2, 2] == lazy[-1, -1] == b"2x2"
             with pytest.raises(ValueError) as err:
                 lazy[3, 3]
-            assert ('provided value not in bounds of index',) == err.value.args
+            assert ("provided value not in bounds of index",) == err.value.args
 
 
 class TestLazyCSVIter:
     def test_to_list(self, lazy):
         _iter = lazy.sequence(col=0)
         assert _iter.to_list() == [b"0", b"1"]
 
@@ -311,15 +364,15 @@
 class TestBigFiles:
     def test_bigger_file(self, file_1000r_1000c):
         lazy = lazycsv.LazyCSV(file_1000r_1000c.name)
         actual = list(lazy.sequence(col=0))
         assert len(actual) == 1000
 
     def test_variable_buffer_size(self, file_1000r_1000c):
-        lazy = lazycsv.LazyCSV(file_1000r_1000c.name, buffer_size=10 ** 7)
+        lazy = lazycsv.LazyCSV(file_1000r_1000c.name, buffer_size=10**7)
         actual = list(lazy.sequence(col=0))
         assert len(actual) == 1000
 
     def test_big_sparse(self):
         tempf = tempfile.NamedTemporaryFile()
         cols, rows = 200, 200
         headers = ",".join(f"col_{i}" for i in range(cols)) + "\n"
```

