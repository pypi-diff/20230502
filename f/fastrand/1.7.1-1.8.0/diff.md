# Comparing `tmp/fastrand-1.7.1.tar.gz` & `tmp/fastrand-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastrand-1.7.1.tar", last modified: Tue May  2 18:31:43 2023, max compression
+gzip compressed data, was "fastrand-1.8.0.tar", last modified: Tue May  2 19:27:50 2023, max compression
```

## Comparing `fastrand-1.7.1.tar` & `fastrand-1.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dlemire    (502) staff       (20)        0 2023-05-02 18:31:43.529010 fastrand-1.7.1/
--rw-r--r--   0 dlemire    (502) staff       (20)    11357 2023-02-03 15:08:51.000000 fastrand-1.7.1/LICENSE
--rw-r--r--   0 dlemire    (502) staff       (20)     2671 2023-05-02 18:31:43.528872 fastrand-1.7.1/PKG-INFO
--rw-r--r--   0 dlemire    (502) staff       (20)     2454 2023-05-02 18:22:32.000000 fastrand-1.7.1/README.md
-drwxr-xr-x   0 dlemire    (502) staff       (20)        0 2023-05-02 18:31:43.528708 fastrand-1.7.1/fastrand.egg-info/
--rw-r--r--   0 dlemire    (502) staff       (20)     2671 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/PKG-INFO
--rw-r--r--   0 dlemire    (502) staff       (20)      171 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/SOURCES.txt
--rw-r--r--   0 dlemire    (502) staff       (20)        1 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/dependency_links.txt
--rw-r--r--   0 dlemire    (502) staff       (20)        9 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/top_level.txt
--rw-r--r--   0 dlemire    (502) staff       (20)     4762 2023-02-03 15:08:51.000000 fastrand-1.7.1/fastrandmodule.c
--rw-r--r--   0 dlemire    (502) staff       (20)       38 2023-05-02 18:31:43.529042 fastrand-1.7.1/setup.cfg
--rw-r--r--   0 dlemire    (502) staff       (20)      463 2023-05-02 18:31:04.000000 fastrand-1.7.1/setup.py
+drwxr-xr-x   0 dlemire    (502) staff       (20)        0 2023-05-02 19:27:50.788925 fastrand-1.8.0/
+-rw-r--r--   0 dlemire    (502) staff       (20)    11357 2023-02-03 15:08:51.000000 fastrand-1.8.0/LICENSE
+-rw-r--r--   0 dlemire    (502) staff       (20)     2934 2023-05-02 19:27:50.788786 fastrand-1.8.0/PKG-INFO
+-rw-r--r--   0 dlemire    (502) staff       (20)     2717 2023-05-02 19:27:08.000000 fastrand-1.8.0/README.md
+drwxr-xr-x   0 dlemire    (502) staff       (20)        0 2023-05-02 19:27:50.788612 fastrand-1.8.0/fastrand.egg-info/
+-rw-r--r--   0 dlemire    (502) staff       (20)     2934 2023-05-02 19:27:50.000000 fastrand-1.8.0/fastrand.egg-info/PKG-INFO
+-rw-r--r--   0 dlemire    (502) staff       (20)      171 2023-05-02 19:27:50.000000 fastrand-1.8.0/fastrand.egg-info/SOURCES.txt
+-rw-r--r--   0 dlemire    (502) staff       (20)        1 2023-05-02 19:27:50.000000 fastrand-1.8.0/fastrand.egg-info/dependency_links.txt
+-rw-r--r--   0 dlemire    (502) staff       (20)        9 2023-05-02 19:27:50.000000 fastrand-1.8.0/fastrand.egg-info/top_level.txt
+-rw-r--r--   0 dlemire    (502) staff       (20)     5551 2023-05-02 19:19:17.000000 fastrand-1.8.0/fastrandmodule.c
+-rw-r--r--   0 dlemire    (502) staff       (20)       38 2023-05-02 19:27:50.788961 fastrand-1.8.0/setup.cfg
+-rw-r--r--   0 dlemire    (502) staff       (20)      463 2023-05-02 19:27:23.000000 fastrand-1.8.0/setup.py
```

### Comparing `fastrand-1.7.1/LICENSE` & `fastrand-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastrand-1.7.1/PKG-INFO` & `fastrand-1.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: fastrand
-Version: 1.7.1
-Summary: Fast random number generation in Python
-Author: Daniel Lemire
-Author-email: daniel@lemire.me
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fastrand
 
-Fast random number generation in Python using PCG
+Fast random number generation in Python using PCG: Up to 10x faster than random.randint.
 
-Blog post: [Ranged random-number generation is slow in Python…](https://lemire.me/blog/2016/03/21/ranged-random-number-generation-is-slow-in-python/)
+Blog post: [Ranged random-number generation is slow in Python](https://lemire.me/blog/2016/03/21/ranged-random-number-generation-is-slow-in-python/)
 
 
 
 
 Usage... (don't forget to type the above lines in your shell!)
 
 ```python
 import fastrand
 
 print("generate an integer in [0,1001)")
 fastrand.pcg32bounded(1001) 
+print("generate an integer in [100,1000]")
+fastrand.pcg32randint(100,1000) # requires Python 3.7 or better
 print("Generate a random 32-bit integer.")
 fastrand.pcg32()
 ```
 
 It is nearly an order of magnitude faster than the alternatives:
 
 ```
-python -m timeit -s 'import fastrand' 'fastrand.pcg32bounded(1001)'
-10000000 loops, best of 3: 0.0602 usec per loop
-python -m timeit -s 'import random' 'random.randint(0,1000)'
-1000000 loops, best of 3: 0.698 usec per loop
-python -m timeit -s 'import numpy' 'numpy.random.randint(0, 1000)'
-1000000 loops, best of 3: 0.795 usec per loop
+
+python3 -m timeit -s 'import fastrand' 'fastrand.pcg32bounded(1001)'
+10000000 loops, best of 5: 23.6 nsec per loop
+
+python3 -m timeit -s 'import fastrand' 'fastrand.pcg32randint(100,1000)'
+10000000 loops, best of 5: 24.6 nsec per loop
+
+python3 -m timeit -s 'import random' 'random.randint(0,1000)'
+1000000 loops, best of 5: 216 nsec per loop
+
+python3 -m timeit -s 'import numpy' 'numpy.random.randint(0, 1000)'
+500000 loops, best of 5: 955 nsec per loop
+
 ```
 
 
 If you have Linux, macOS or Windows, you should be able to do just pip install...
 
 ```
 pip install fastrand
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastrand-1.7.1/README.md` & `fastrand-1.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,54 @@
+Metadata-Version: 2.1
+Name: fastrand
+Version: 1.8.0
+Summary: Fast random number generation in Python
+Author: Daniel Lemire
+Author-email: daniel@lemire.me
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # fastrand
 
-Fast random number generation in Python using PCG
+Fast random number generation in Python using PCG: Up to 10x faster than random.randint.
 
-Blog post: [Ranged random-number generation is slow in Python…](https://lemire.me/blog/2016/03/21/ranged-random-number-generation-is-slow-in-python/)
+Blog post: [Ranged random-number generation is slow in Python](https://lemire.me/blog/2016/03/21/ranged-random-number-generation-is-slow-in-python/)
 
 
 
 
 Usage... (don't forget to type the above lines in your shell!)
 
 ```python
 import fastrand
 
 print("generate an integer in [0,1001)")
 fastrand.pcg32bounded(1001) 
+print("generate an integer in [100,1000]")
+fastrand.pcg32randint(100,1000) # requires Python 3.7 or better
 print("Generate a random 32-bit integer.")
 fastrand.pcg32()
 ```
 
 It is nearly an order of magnitude faster than the alternatives:
 
 ```
-python -m timeit -s 'import fastrand' 'fastrand.pcg32bounded(1001)'
-10000000 loops, best of 3: 0.0602 usec per loop
-python -m timeit -s 'import random' 'random.randint(0,1000)'
-1000000 loops, best of 3: 0.698 usec per loop
-python -m timeit -s 'import numpy' 'numpy.random.randint(0, 1000)'
-1000000 loops, best of 3: 0.795 usec per loop
+
+python3 -m timeit -s 'import fastrand' 'fastrand.pcg32bounded(1001)'
+10000000 loops, best of 5: 23.6 nsec per loop
+
+python3 -m timeit -s 'import fastrand' 'fastrand.pcg32randint(100,1000)'
+10000000 loops, best of 5: 24.6 nsec per loop
+
+python3 -m timeit -s 'import random' 'random.randint(0,1000)'
+1000000 loops, best of 5: 216 nsec per loop
+
+python3 -m timeit -s 'import numpy' 'numpy.random.randint(0, 1000)'
+500000 loops, best of 5: 955 nsec per loop
+
 ```
 
 
 If you have Linux, macOS or Windows, you should be able to do just pip install...
 
 ```
 pip install fastrand
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastrand-1.7.1/fastrand.egg-info/PKG-INFO` & `fastrand-1.8.0/fastrand.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: fastrand
-Version: 1.7.1
+Version: 1.8.0
 Summary: Fast random number generation in Python
 Author: Daniel Lemire
 Author-email: daniel@lemire.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastrand
 
-Fast random number generation in Python using PCG
+Fast random number generation in Python using PCG: Up to 10x faster than random.randint.
 
-Blog post: [Ranged random-number generation is slow in Python…](https://lemire.me/blog/2016/03/21/ranged-random-number-generation-is-slow-in-python/)
+Blog post: [Ranged random-number generation is slow in Python](https://lemire.me/blog/2016/03/21/ranged-random-number-generation-is-slow-in-python/)
 
 
 
 
 Usage... (don't forget to type the above lines in your shell!)
 
 ```python
 import fastrand
 
 print("generate an integer in [0,1001)")
 fastrand.pcg32bounded(1001) 
+print("generate an integer in [100,1000]")
+fastrand.pcg32randint(100,1000) # requires Python 3.7 or better
 print("Generate a random 32-bit integer.")
 fastrand.pcg32()
 ```
 
 It is nearly an order of magnitude faster than the alternatives:
 
 ```
-python -m timeit -s 'import fastrand' 'fastrand.pcg32bounded(1001)'
-10000000 loops, best of 3: 0.0602 usec per loop
-python -m timeit -s 'import random' 'random.randint(0,1000)'
-1000000 loops, best of 3: 0.698 usec per loop
-python -m timeit -s 'import numpy' 'numpy.random.randint(0, 1000)'
-1000000 loops, best of 3: 0.795 usec per loop
+
+python3 -m timeit -s 'import fastrand' 'fastrand.pcg32bounded(1001)'
+10000000 loops, best of 5: 23.6 nsec per loop
+
+python3 -m timeit -s 'import fastrand' 'fastrand.pcg32randint(100,1000)'
+10000000 loops, best of 5: 24.6 nsec per loop
+
+python3 -m timeit -s 'import random' 'random.randint(0,1000)'
+1000000 loops, best of 5: 216 nsec per loop
+
+python3 -m timeit -s 'import numpy' 'numpy.random.randint(0, 1000)'
+500000 loops, best of 5: 955 nsec per loop
+
 ```
 
 
 If you have Linux, macOS or Windows, you should be able to do just pip install...
 
 ```
 pip install fastrand
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastrand-1.7.1/fastrandmodule.c` & `fastrand-1.8.0/fastrandmodule.c`

 * *Files 6% similar despite different names*

```diff
@@ -56,28 +56,46 @@
         }
     }
     return multiresult >> 32; // [0, range)
 }
 
 
 #if PY_MAJOR_VERSION >= 3
-#define PyInt_AsLong(x)   PyLong_AsLong(x)
+#define PyInt_AsLong(x)  PyLong_AsLong(x)
 #define PyInt_AsUnsignedLongLongMask(x) PyLong_AsUnsignedLongLongMask(x)
 #endif
 
- static PyObject*
+static PyObject*
 pcg32bounded(PyObject* self, PyObject* args) {
     long n = PyInt_AsLong(args);
     if ((n > 0) && (n <= UINT32_MAX))
       return Py_BuildValue("I", pcg32_random_bounded_divisionless((uint32_t)n));
-    if (!PyErr_Occurred())
+    if (!PyErr_Occurred()) {
       PyErr_SetString(PyExc_ValueError, "no such random number exist");
+    }
     Py_RETURN_NONE;
 }
 
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
+static PyObject*
+pcg32randint(PyObject* self, PyObject *const *args, Py_ssize_t len_args) {
+    long n1 = PyInt_AsLong(args[0]);
+    long n2 = PyInt_AsLong(args[1]);
+    if ((n1 > UINT32_MAX) && (n2 > UINT32_MAX)) {
+        PyErr_SetString(PyExc_ValueError, "the bounds of the interval cannot be greater than 2**32-1");
+        Py_RETURN_NONE;
+    }
+    if(n2 < n1) {
+        PyErr_SetString(PyExc_ValueError, "the second argument must be greater or equal than the first");
+        Py_RETURN_NONE;
+    }
+    return Py_BuildValue("I", n1 + pcg32_random_bounded_divisionless((uint32_t)(n2 - n1 + 1)));
+}
+#endif
+
 static PyObject*
 pcg32inc(PyObject* self, PyObject* args) {
     uint64_t n = PyInt_AsUnsignedLongLongMask(args);
     pcg32_init_inc(n);
     Py_RETURN_NONE;
 }
 
@@ -141,14 +159,17 @@
 
 
 
 
 
 static PyMethodDef FastRandMethods[] =
 {
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 7
+    {"pcg32randint", (PyCFunction)pcg32randint, METH_FASTCALL},
+#endif
      {"xorshift128plus", xorshift, METH_NOARGS, "generate random integer (64 bits)"},
      {"pcg32", pcg32, METH_NOARGS, "generate random integer (32 bits) using PCG"},
      {"pcg32bounded", pcg32bounded, METH_O, "generate random integer in the interval [0,range) using PCG."},
      {"pcg32inc", pcg32inc, METH_O, "change the increment parameter of the pcg32 generator (global, for experts)."},
      {"pcg32_seed", pcg32state, METH_O, "seed the pcg32 generator (global)."},
      {"xorshift128plus_seed1", xorshift128plus_seed1, METH_O, "seed the xorshift128plus generator (global, first 64 bits)."},
      {"xorshift128plus_seed2", xorshift128plus_seed2, METH_O, "seed the xorshift128plus generator (global, second 64 bits)."},
```

