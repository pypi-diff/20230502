# Comparing `tmp/psycopg-c-3.1.7.tar.gz` & `tmp/psycopg-c-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg-c-3.1.7.tar", last modified: Tue Dec 20 15:37:13 2022, max compression
+gzip compressed data, was "psycopg-c-3.1.8.tar", last modified: Mon Jan 16 22:56:57 2023, max compression
```

## Comparing `psycopg-c-3.1.7.tar` & `psycopg-c-3.1.8.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:37:13.319693 psycopg-c-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2022-12-20 15:37:13.319693 psycopg-c-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:37:13.315693 psycopg-c-3.1.7/psycopg_c/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:37:13.319693 psycopg-c-3.1.7/psycopg_c/_psycopg/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/_psycopg/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/_psycopg/endian.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/_psycopg/oids.pxd
--rw-r--r--   0 runner    (1001) docker     (123)  4422537 2022-12-20 15:37:12.000000 psycopg-c-3.1.7/psycopg_c/_psycopg.c
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/_psycopg.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:37:13.319693 psycopg-c-3.1.7/psycopg_c/pq/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/pq/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/pq/libpq.pxd
--rw-r--r--   0 runner    (1001) docker     (123)  1639015 2022-12-20 15:37:13.000000 psycopg-c-3.1.7/psycopg_c/pq.c
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/pq.pxd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:37:13.319693 psycopg-c-3.1.7/psycopg_c/types/
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/types/numutils.c
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/psycopg_c/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:37:13.319693 psycopg-c-3.1.7/psycopg_c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2022-12-20 15:37:09.000000 psycopg-c-3.1.7/psycopg_c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-20 15:37:13.000000 psycopg-c-3.1.7/psycopg_c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:37:09.000000 psycopg-c-3.1.7/psycopg_c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:37:09.000000 psycopg-c-3.1.7/psycopg_c.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-20 15:37:09.000000 psycopg-c-3.1.7/psycopg_c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2022-12-20 15:37:13.319693 psycopg-c-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2022-12-20 15:37:05.000000 psycopg-c-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:57.838401 psycopg-c-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-16 22:56:57.838401 psycopg-c-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:57.830401 psycopg-c-3.1.8/build_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/build_backend/cython_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:57.834401 psycopg-c-3.1.8/psycopg_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:57.838401 psycopg-c-3.1.8/psycopg_c/_psycopg/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/_psycopg/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/_psycopg/endian.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/_psycopg/oids.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)  4422416 2023-01-16 22:56:56.000000 psycopg-c-3.1.8/psycopg_c/_psycopg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/_psycopg.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:57.838401 psycopg-c-3.1.8/psycopg_c/pq/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/pq/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/pq/libpq.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)  1657509 2023-01-16 22:56:57.000000 psycopg-c-3.1.8/psycopg_c/pq.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/pq.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:57.838401 psycopg-c-3.1.8/psycopg_c/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/types/numutils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/psycopg_c/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 22:56:57.838401 psycopg-c-3.1.8/psycopg_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-16 22:56:54.000000 psycopg-c-3.1.8/psycopg_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-16 22:56:57.000000 psycopg-c-3.1.8/psycopg_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 22:56:54.000000 psycopg-c-3.1.8/psycopg_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 22:56:54.000000 psycopg-c-3.1.8/psycopg_c.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-16 22:56:54.000000 psycopg-c-3.1.8/psycopg_c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-01-16 22:56:57.838401 psycopg-c-3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-01-16 22:56:42.000000 psycopg-c-3.1.8/setup.py
```

### Comparing `psycopg-c-3.1.7/LICENSE.txt` & `psycopg-c-3.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/PKG-INFO` & `psycopg-c-3.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: psycopg-c
-Version: 3.1.7
+Version: 3.1.8
 Summary: PostgreSQL database adapter for Python -- C optimisation distribution
 Home-page: https://psycopg.org/psycopg3/
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://psycopg.org/
+Project-URL: Documentation, https://psycopg.org/psycopg3/docs/
+Project-URL: Changes, https://psycopg.org/psycopg3/docs/news.html
 Project-URL: Code, https://github.com/psycopg/psycopg
 Project-URL: Issue Tracker, https://github.com/psycopg/psycopg/issues
 Project-URL: Download, https://pypi.org/project/psycopg-c/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -60,9 +61,7 @@
 more details.
 
 .. __: https://github.com/psycopg/psycopg#readme
 .. __: https://www.psycopg.org/psycopg3/docs/basic/install.html
 
 
 Copyright (C) 2020 The Psycopg Team
-
-
```

### Comparing `psycopg-c-3.1.7/README.rst` & `psycopg-c-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/psycopg_c/_psycopg/endian.pxd` & `psycopg-c-3.1.8/psycopg_c/_psycopg/endian.pxd`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/psycopg_c/_psycopg/oids.pxd` & `psycopg-c-3.1.8/psycopg_c/_psycopg/oids.pxd`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/psycopg_c/_psycopg.c` & `psycopg-c-3.1.8/psycopg_c/_psycopg.c`

 * *Files 0% similar despite different names*

```diff
@@ -1103,14 +1103,20 @@
 #define PQexitPipelineMode(conn) 1
 #define PQpipelineSync(conn) 0
 #define PQsendFlushRequest(conn) 0
 #define PQsetTraceFlags(conn, stream) do {} while (0)
 #endif
 
 
+/* Include this early to avoid a warning about redefined ARRAYSIZE in winnt.h */
+#ifdef MS_WINDOWS
+#define WIN32_LEAN_AND_MEAN
+#include <winsock2.h>
+#endif
+
 #ifndef ARRAYSIZE
 #define ARRAYSIZE(a) ((sizeof(a) / sizeof(*(a))))
 #endif
     
 #include <string.h>
 #include <stdio.h>
 #include <stdint.h>
@@ -1349,20 +1355,17 @@
     }
 
     Py_BEGIN_ALLOW_THREADS
     errno = 0;
     select_rv = poll(&input_fd, 1, timeout_ms);
     Py_END_ALLOW_THREADS
 
+    if (select_rv < 0) { goto error; }
     if (PyErr_CheckSignals()) { goto finally; }
 
-    if (select_rv < 0) {
-        goto error;
-    }
-
     if (input_fd.events & POLLIN) { rv |= SELECT_EV_READ; }
     if (input_fd.events & POLLOUT) { rv |= SELECT_EV_WRITE; }
 
 #else
 
     fd_set ifds;
     fd_set ofds;
@@ -1397,20 +1400,17 @@
     }
 
     Py_BEGIN_ALLOW_THREADS
     errno = 0;
     select_rv = select(fileno + 1, &ifds, &ofds, &efds, tvptr);
     Py_END_ALLOW_THREADS
 
+    if (select_rv < 0) { goto error; }
     if (PyErr_CheckSignals()) { goto finally; }
 
-    if (select_rv < 0) {
-        goto error;
-    }
-
     if (FD_ISSET(fileno, &ifds)) { rv |= SELECT_EV_READ; }
     if (FD_ISSET(fileno, &ofds)) { rv |= SELECT_EV_WRITE; }
 
 #endif  /* HAVE_POLL */
 
     return rv;
 
@@ -1748,21 +1748,21 @@
   "psycopg_c/_psycopg/waiting.pyx",
   "psycopg_c/types/datetime.pyx",
   "psycopg_c/types/string.pyx",
   "psycopg_c/_psycopg/copy.pyx",
   "psycopg_c/_psycopg/generators.pyx",
   "psycopg_c/types/array.pyx",
   "psycopg_c/types/bool.pyx",
-  ".eggs/Cython-3.0.0a11-py3.9-linux-x86_64.egg/Cython/Includes/cpython/contextvars.pxd",
-  ".eggs/Cython-3.0.0a11-py3.9-linux-x86_64.egg/Cython/Includes/cpython/datetime.pxd",
+  "contextvars.pxd",
+  "datetime.pxd",
   "psycopg_c/_psycopg.pyx",
   "psycopg_c/pq.pxd",
-  ".eggs/Cython-3.0.0a11-py3.9-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
-  ".eggs/Cython-3.0.0a11-py3.9-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd",
-  ".eggs/Cython-3.0.0a11-py3.9-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd",
+  "type.pxd",
+  "bool.pxd",
+  "complex.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
@@ -29318,15 +29318,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/_psycopg/waiting.pyx":160
+/* "psycopg_c/_psycopg/waiting.pyx":154
  * 
  * 
  * def wait_c(gen: PQGen[RV], int fileno, timeout = None) -> RV:             # <<<<<<<<<<<<<<
  *     """
  *     Wait for a generator using poll or select.
  */
 
@@ -29380,52 +29380,52 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_gen)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 160, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 154, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fileno)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 160, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 154, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("wait_c", 0, 2, 3, 1); __PYX_ERR(4, 160, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("wait_c", 0, 2, 3, 1); __PYX_ERR(4, 154, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_timeout);
           if (value) { values[2] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 160, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 154, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "wait_c") < 0)) __PYX_ERR(4, 160, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "wait_c") < 0)) __PYX_ERR(4, 154, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_gen = values[0];
-    __pyx_v_fileno = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_fileno == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 160, __pyx_L3_error)
+    __pyx_v_fileno = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_fileno == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 154, __pyx_L3_error)
     __pyx_v_timeout = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("wait_c", 0, 2, 3, __pyx_nargs); __PYX_ERR(4, 160, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("wait_c", 0, 2, 3, __pyx_nargs); __PYX_ERR(4, 154, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c._psycopg.wait_c", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9psycopg_c_8_psycopg_26wait_c(__pyx_self, __pyx_v_gen, __pyx_v_fileno, __pyx_v_timeout);
 
@@ -29465,97 +29465,97 @@
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wait_c", 0);
 
-  /* "psycopg_c/_psycopg/waiting.pyx":168
+  /* "psycopg_c/_psycopg/waiting.pyx":162
  *     cdef PyObject *pyready
  * 
  *     if timeout is None:             # <<<<<<<<<<<<<<
  *         ctimeout = -1.0
  *     else:
  */
   __pyx_t_1 = (__pyx_v_timeout == Py_None);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/_psycopg/waiting.pyx":169
+    /* "psycopg_c/_psycopg/waiting.pyx":163
  * 
  *     if timeout is None:
  *         ctimeout = -1.0             # <<<<<<<<<<<<<<
  *     else:
- *         ctimeout = float(timeout)
+ *         ctimeout = <float>float(timeout)
  */
     __pyx_v_ctimeout = -1.0;
 
-    /* "psycopg_c/_psycopg/waiting.pyx":168
+    /* "psycopg_c/_psycopg/waiting.pyx":162
  *     cdef PyObject *pyready
  * 
  *     if timeout is None:             # <<<<<<<<<<<<<<
  *         ctimeout = -1.0
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "psycopg_c/_psycopg/waiting.pyx":171
+  /* "psycopg_c/_psycopg/waiting.pyx":165
  *         ctimeout = -1.0
  *     else:
- *         ctimeout = float(timeout)             # <<<<<<<<<<<<<<
+ *         ctimeout = <float>float(timeout)             # <<<<<<<<<<<<<<
  *         if ctimeout < 0.0:
  *             ctimeout = -1.0
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_AsDouble(__pyx_v_timeout); if (unlikely(__pyx_t_2 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(4, 171, __pyx_L1_error)
-    __pyx_v_ctimeout = __pyx_t_2;
+    __pyx_t_2 = __Pyx_PyObject_AsDouble(__pyx_v_timeout); if (unlikely(__pyx_t_2 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(4, 165, __pyx_L1_error)
+    __pyx_v_ctimeout = ((float)__pyx_t_2);
 
-    /* "psycopg_c/_psycopg/waiting.pyx":172
+    /* "psycopg_c/_psycopg/waiting.pyx":166
  *     else:
- *         ctimeout = float(timeout)
+ *         ctimeout = <float>float(timeout)
  *         if ctimeout < 0.0:             # <<<<<<<<<<<<<<
  *             ctimeout = -1.0
  * 
  */
     __pyx_t_1 = (__pyx_v_ctimeout < 0.0);
     if (__pyx_t_1) {
 
-      /* "psycopg_c/_psycopg/waiting.pyx":173
- *         ctimeout = float(timeout)
+      /* "psycopg_c/_psycopg/waiting.pyx":167
+ *         ctimeout = <float>float(timeout)
  *         if ctimeout < 0.0:
  *             ctimeout = -1.0             # <<<<<<<<<<<<<<
  * 
  *     send = gen.send
  */
       __pyx_v_ctimeout = -1.0;
 
-      /* "psycopg_c/_psycopg/waiting.pyx":172
+      /* "psycopg_c/_psycopg/waiting.pyx":166
  *     else:
- *         ctimeout = float(timeout)
+ *         ctimeout = <float>float(timeout)
  *         if ctimeout < 0.0:             # <<<<<<<<<<<<<<
  *             ctimeout = -1.0
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "psycopg_c/_psycopg/waiting.pyx":175
+  /* "psycopg_c/_psycopg/waiting.pyx":169
  *             ctimeout = -1.0
  * 
  *     send = gen.send             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gen, __pyx_n_s_send); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 175, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_gen, __pyx_n_s_send); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_send = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "psycopg_c/_psycopg/waiting.pyx":177
+  /* "psycopg_c/_psycopg/waiting.pyx":171
  *     send = gen.send
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         wait = next(gen)
  * 
  */
   {
@@ -29563,199 +29563,199 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_6);
     /*try:*/ {
 
-      /* "psycopg_c/_psycopg/waiting.pyx":178
+      /* "psycopg_c/_psycopg/waiting.pyx":172
  * 
  *     try:
  *         wait = next(gen)             # <<<<<<<<<<<<<<
  * 
  *         while True:
  */
-      __pyx_t_3 = __Pyx_PyIter_Next(__pyx_v_gen); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 178, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyIter_Next(__pyx_v_gen); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 172, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 178, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 172, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_v_wait = __pyx_t_7;
 
-      /* "psycopg_c/_psycopg/waiting.pyx":180
+      /* "psycopg_c/_psycopg/waiting.pyx":174
  *         wait = next(gen)
  * 
  *         while True:             # <<<<<<<<<<<<<<
  *             ready = wait_c_impl(fileno, wait, ctimeout)
  *             if ready == 0:
  */
       while (1) {
 
-        /* "psycopg_c/_psycopg/waiting.pyx":181
+        /* "psycopg_c/_psycopg/waiting.pyx":175
  * 
  *         while True:
  *             ready = wait_c_impl(fileno, wait, ctimeout)             # <<<<<<<<<<<<<<
  *             if ready == 0:
  *                 continue
  */
-        __pyx_t_7 = wait_c_impl(__pyx_v_fileno, __pyx_v_wait, __pyx_v_ctimeout); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(4, 181, __pyx_L5_error)
+        __pyx_t_7 = wait_c_impl(__pyx_v_fileno, __pyx_v_wait, __pyx_v_ctimeout); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(4, 175, __pyx_L5_error)
         __pyx_v_ready = __pyx_t_7;
 
-        /* "psycopg_c/_psycopg/waiting.pyx":182
+        /* "psycopg_c/_psycopg/waiting.pyx":176
  *         while True:
  *             ready = wait_c_impl(fileno, wait, ctimeout)
  *             if ready == 0:             # <<<<<<<<<<<<<<
  *                 continue
  *             elif ready == READY_R:
  */
         __pyx_t_1 = (__pyx_v_ready == 0);
         if (__pyx_t_1) {
 
-          /* "psycopg_c/_psycopg/waiting.pyx":183
+          /* "psycopg_c/_psycopg/waiting.pyx":177
  *             ready = wait_c_impl(fileno, wait, ctimeout)
  *             if ready == 0:
  *                 continue             # <<<<<<<<<<<<<<
  *             elif ready == READY_R:
  *                 pyready = <PyObject *>PY_READY_R
  */
           goto __pyx_L11_continue;
 
-          /* "psycopg_c/_psycopg/waiting.pyx":182
+          /* "psycopg_c/_psycopg/waiting.pyx":176
  *         while True:
  *             ready = wait_c_impl(fileno, wait, ctimeout)
  *             if ready == 0:             # <<<<<<<<<<<<<<
  *                 continue
  *             elif ready == READY_R:
  */
         }
 
-        /* "psycopg_c/_psycopg/waiting.pyx":184
+        /* "psycopg_c/_psycopg/waiting.pyx":178
  *             if ready == 0:
  *                 continue
  *             elif ready == READY_R:             # <<<<<<<<<<<<<<
  *                 pyready = <PyObject *>PY_READY_R
  *             elif ready == READY_RW:
  */
         __pyx_t_1 = (__pyx_v_ready == __pyx_v_9psycopg_c_8_psycopg_READY_R);
         if (__pyx_t_1) {
 
-          /* "psycopg_c/_psycopg/waiting.pyx":185
+          /* "psycopg_c/_psycopg/waiting.pyx":179
  *                 continue
  *             elif ready == READY_R:
  *                 pyready = <PyObject *>PY_READY_R             # <<<<<<<<<<<<<<
  *             elif ready == READY_RW:
  *                 pyready = <PyObject *>PY_READY_RW
  */
           __pyx_v_pyready = ((PyObject *)__pyx_v_9psycopg_c_8_psycopg_PY_READY_R);
 
-          /* "psycopg_c/_psycopg/waiting.pyx":184
+          /* "psycopg_c/_psycopg/waiting.pyx":178
  *             if ready == 0:
  *                 continue
  *             elif ready == READY_R:             # <<<<<<<<<<<<<<
  *                 pyready = <PyObject *>PY_READY_R
  *             elif ready == READY_RW:
  */
           goto __pyx_L13;
         }
 
-        /* "psycopg_c/_psycopg/waiting.pyx":186
+        /* "psycopg_c/_psycopg/waiting.pyx":180
  *             elif ready == READY_R:
  *                 pyready = <PyObject *>PY_READY_R
  *             elif ready == READY_RW:             # <<<<<<<<<<<<<<
  *                 pyready = <PyObject *>PY_READY_RW
  *             elif ready == READY_W:
  */
         __pyx_t_1 = (__pyx_v_ready == __pyx_v_9psycopg_c_8_psycopg_READY_RW);
         if (__pyx_t_1) {
 
-          /* "psycopg_c/_psycopg/waiting.pyx":187
+          /* "psycopg_c/_psycopg/waiting.pyx":181
  *                 pyready = <PyObject *>PY_READY_R
  *             elif ready == READY_RW:
  *                 pyready = <PyObject *>PY_READY_RW             # <<<<<<<<<<<<<<
  *             elif ready == READY_W:
  *                 pyready = <PyObject *>PY_READY_W
  */
           __pyx_v_pyready = ((PyObject *)__pyx_v_9psycopg_c_8_psycopg_PY_READY_RW);
 
-          /* "psycopg_c/_psycopg/waiting.pyx":186
+          /* "psycopg_c/_psycopg/waiting.pyx":180
  *             elif ready == READY_R:
  *                 pyready = <PyObject *>PY_READY_R
  *             elif ready == READY_RW:             # <<<<<<<<<<<<<<
  *                 pyready = <PyObject *>PY_READY_RW
  *             elif ready == READY_W:
  */
           goto __pyx_L13;
         }
 
-        /* "psycopg_c/_psycopg/waiting.pyx":188
+        /* "psycopg_c/_psycopg/waiting.pyx":182
  *             elif ready == READY_RW:
  *                 pyready = <PyObject *>PY_READY_RW
  *             elif ready == READY_W:             # <<<<<<<<<<<<<<
  *                 pyready = <PyObject *>PY_READY_W
  *             else:
  */
         __pyx_t_1 = (__pyx_v_ready == __pyx_v_9psycopg_c_8_psycopg_READY_W);
         if (likely(__pyx_t_1)) {
 
-          /* "psycopg_c/_psycopg/waiting.pyx":189
+          /* "psycopg_c/_psycopg/waiting.pyx":183
  *                 pyready = <PyObject *>PY_READY_RW
  *             elif ready == READY_W:
  *                 pyready = <PyObject *>PY_READY_W             # <<<<<<<<<<<<<<
  *             else:
  *                 raise AssertionError(f"unexpected ready value: {ready}")
  */
           __pyx_v_pyready = ((PyObject *)__pyx_v_9psycopg_c_8_psycopg_PY_READY_W);
 
-          /* "psycopg_c/_psycopg/waiting.pyx":188
+          /* "psycopg_c/_psycopg/waiting.pyx":182
  *             elif ready == READY_RW:
  *                 pyready = <PyObject *>PY_READY_RW
  *             elif ready == READY_W:             # <<<<<<<<<<<<<<
  *                 pyready = <PyObject *>PY_READY_W
  *             else:
  */
           goto __pyx_L13;
         }
 
-        /* "psycopg_c/_psycopg/waiting.pyx":191
+        /* "psycopg_c/_psycopg/waiting.pyx":185
  *                 pyready = <PyObject *>PY_READY_W
  *             else:
  *                 raise AssertionError(f"unexpected ready value: {ready}")             # <<<<<<<<<<<<<<
  * 
  *             wait = PyObject_CallFunctionObjArgs(send, pyready, NULL)
  */
         /*else*/ {
-          __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_ready, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 191, __pyx_L5_error)
+          __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_ready, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 185, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_kp_u_unexpected_ready_value, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 191, __pyx_L5_error)
+          __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_kp_u_unexpected_ready_value, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 185, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AssertionError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 191, __pyx_L5_error)
+          __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AssertionError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 185, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_Raise(__pyx_t_3, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __PYX_ERR(4, 191, __pyx_L5_error)
+          __PYX_ERR(4, 185, __pyx_L5_error)
         }
         __pyx_L13:;
 
-        /* "psycopg_c/_psycopg/waiting.pyx":193
+        /* "psycopg_c/_psycopg/waiting.pyx":187
  *                 raise AssertionError(f"unexpected ready value: {ready}")
  * 
  *             wait = PyObject_CallFunctionObjArgs(send, pyready, NULL)             # <<<<<<<<<<<<<<
  * 
  *     except StopIteration as ex:
  */
-        __pyx_t_3 = PyObject_CallFunctionObjArgs(__pyx_v_send, __pyx_v_pyready, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 193, __pyx_L5_error)
+        __pyx_t_3 = PyObject_CallFunctionObjArgs(__pyx_v_send, __pyx_v_pyready, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 187, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 193, __pyx_L5_error)
+        __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 187, __pyx_L5_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_v_wait = __pyx_t_7;
         __pyx_L11_continue:;
       }
 
-      /* "psycopg_c/_psycopg/waiting.pyx":177
+      /* "psycopg_c/_psycopg/waiting.pyx":171
  *     send = gen.send
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         wait = next(gen)
  * 
  */
     }
@@ -29763,72 +29763,72 @@
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     goto __pyx_L10_try_end;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "psycopg_c/_psycopg/waiting.pyx":195
+    /* "psycopg_c/_psycopg/waiting.pyx":189
  *             wait = PyObject_CallFunctionObjArgs(send, pyready, NULL)
  * 
  *     except StopIteration as ex:             # <<<<<<<<<<<<<<
  *         rv: RV = ex.args[0] if ex.args else None
  *         return rv
  */
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
     if (__pyx_t_7) {
       __Pyx_AddTraceback("psycopg_c._psycopg.wait_c", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_8, &__pyx_t_9) < 0) __PYX_ERR(4, 195, __pyx_L7_except_error)
+      if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_8, &__pyx_t_9) < 0) __PYX_ERR(4, 189, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_8);
       __pyx_v_ex = __pyx_t_8;
       /*try:*/ {
 
-        /* "psycopg_c/_psycopg/waiting.pyx":196
+        /* "psycopg_c/_psycopg/waiting.pyx":190
  * 
  *     except StopIteration as ex:
  *         rv: RV = ex.args[0] if ex.args else None             # <<<<<<<<<<<<<<
  *         return rv
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ex, __pyx_n_s_args); if (unlikely(!__pyx_t_11)) __PYX_ERR(4, 196, __pyx_L19_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ex, __pyx_n_s_args); if (unlikely(!__pyx_t_11)) __PYX_ERR(4, 190, __pyx_L19_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(4, 196, __pyx_L19_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(4, 190, __pyx_L19_error)
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         if (__pyx_t_1) {
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ex, __pyx_n_s_args); if (unlikely(!__pyx_t_11)) __PYX_ERR(4, 196, __pyx_L19_error)
+          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_ex, __pyx_n_s_args); if (unlikely(!__pyx_t_11)) __PYX_ERR(4, 190, __pyx_L19_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_12 = __Pyx_GetItemInt(__pyx_t_11, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(4, 196, __pyx_L19_error)
+          __pyx_t_12 = __Pyx_GetItemInt(__pyx_t_11, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(4, 190, __pyx_L19_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __pyx_t_10 = __pyx_t_12;
           __pyx_t_12 = 0;
         } else {
           __Pyx_INCREF(Py_None);
           __pyx_t_10 = Py_None;
         }
         __pyx_v_rv = __pyx_t_10;
         __pyx_t_10 = 0;
 
-        /* "psycopg_c/_psycopg/waiting.pyx":197
+        /* "psycopg_c/_psycopg/waiting.pyx":191
  *     except StopIteration as ex:
  *         rv: RV = ex.args[0] if ex.args else None
  *         return rv             # <<<<<<<<<<<<<<
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_v_rv);
         __pyx_r = __pyx_v_rv;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L18_return;
       }
 
-      /* "psycopg_c/_psycopg/waiting.pyx":195
+      /* "psycopg_c/_psycopg/waiting.pyx":189
  *             wait = PyObject_CallFunctionObjArgs(send, pyready, NULL)
  * 
  *     except StopIteration as ex:             # <<<<<<<<<<<<<<
  *         rv: RV = ex.args[0] if ex.args else None
  *         return rv
  */
       /*finally:*/ {
@@ -29875,15 +29875,15 @@
           goto __pyx_L8_except_return;
         }
       }
     }
     goto __pyx_L7_except_error;
     __pyx_L7_except_error:;
 
-    /* "psycopg_c/_psycopg/waiting.pyx":177
+    /* "psycopg_c/_psycopg/waiting.pyx":171
  *     send = gen.send
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         wait = next(gen)
  * 
  */
     __Pyx_XGIVEREF(__pyx_t_4);
@@ -29896,15 +29896,15 @@
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
     goto __pyx_L0;
     __pyx_L10_try_end:;
   }
 
-  /* "psycopg_c/_psycopg/waiting.pyx":160
+  /* "psycopg_c/_psycopg/waiting.pyx":154
  * 
  * 
  * def wait_c(gen: PQGen[RV], int fileno, timeout = None) -> RV:             # <<<<<<<<<<<<<<
  *     """
  *     Wait for a generator using poll or select.
  */
 
@@ -31036,15 +31036,15 @@
 static PyObject *__pyx_f_9psycopg_c_8_psycopg__parse_token(char const **__pyx_v_bufptr, char const *__pyx_v_bufend, char __pyx_v_cdelim, char **__pyx_v_scratch, size_t *__pyx_v_sclen, struct __pyx_obj_9psycopg_c_8_psycopg_CLoader *__pyx_v_cloader, PyObject *__pyx_v_load) {
   char const *__pyx_v_start;
   int __pyx_v_has_quotes;
   int __pyx_v_quoted;
   int __pyx_v_num_escapes;
   int __pyx_v_escaped;
   char const *__pyx_v_end;
-  int __pyx_v_length;
+  Py_ssize_t __pyx_v_length;
   char const *__pyx_v_src;
   char *__pyx_v_tgt;
   size_t __pyx_v_unesclen;
   PyObject *__pyx_v_b = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -31371,15 +31371,15 @@
 if (__pyx_t_1) {
 
   /* "psycopg_c/types/array.pyx":165
  *     bufptr[0] = end
  *     if has_quotes:
  *         end -= 1             # <<<<<<<<<<<<<<
  * 
- *     cdef int length = (end - start)
+ *     cdef Py_ssize_t length = (end - start)
  */
   __pyx_v_end = (__pyx_v_end - 1);
 
   /* "psycopg_c/types/array.pyx":164
  *     # Return the new position for the buffer
  *     bufptr[0] = end
  *     if has_quotes:             # <<<<<<<<<<<<<<
@@ -31387,36 +31387,36 @@
  * 
  */
 }
 
 /* "psycopg_c/types/array.pyx":167
  *         end -= 1
  * 
- *     cdef int length = (end - start)             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = (end - start)             # <<<<<<<<<<<<<<
  *     if length == 4 and not has_quotes \
  *             and start[0] == b'N' and start[1] == b'U' \
  */
 __pyx_v_length = (__pyx_v_end - __pyx_v_start);
 
 /* "psycopg_c/types/array.pyx":168
  * 
- *     cdef int length = (end - start)
+ *     cdef Py_ssize_t length = (end - start)
  *     if length == 4 and not has_quotes \             # <<<<<<<<<<<<<<
  *             and start[0] == b'N' and start[1] == b'U' \
  *             and start[2] == b'L' and start[3] == b'L':
  */
 __pyx_t_2 = (__pyx_v_length == 4);
 if (__pyx_t_2) {
 } else {
   __pyx_t_1 = __pyx_t_2;
   goto __pyx_L16_bool_binop_done;
 }
 
 /* "psycopg_c/types/array.pyx":169
- *     cdef int length = (end - start)
+ *     cdef Py_ssize_t length = (end - start)
  *     if length == 4 and not has_quotes \
  *             and start[0] == b'N' and start[1] == b'U' \             # <<<<<<<<<<<<<<
  *             and start[2] == b'L' and start[3] == b'L':
  *         return None
  */
 __pyx_t_2 = (!(__pyx_v_has_quotes != 0));
 if (__pyx_t_2) {
@@ -31452,15 +31452,15 @@
 }
 __pyx_t_2 = ((__pyx_v_start[3]) == 'L');
 __pyx_t_1 = __pyx_t_2;
 __pyx_L16_bool_binop_done:;
 
 /* "psycopg_c/types/array.pyx":168
  * 
- *     cdef int length = (end - start)
+ *     cdef Py_ssize_t length = (end - start)
  *     if length == 4 and not has_quotes \             # <<<<<<<<<<<<<<
  *             and start[0] == b'N' and start[1] == b'U' \
  *             and start[2] == b'L' and start[3] == b'L':
  */
 if (__pyx_t_1) {
 
   /* "psycopg_c/types/array.pyx":171
@@ -31472,15 +31472,15 @@
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
   /* "psycopg_c/types/array.pyx":168
  * 
- *     cdef int length = (end - start)
+ *     cdef Py_ssize_t length = (end - start)
  *     if length == 4 and not has_quotes \             # <<<<<<<<<<<<<<
  *             and start[0] == b'N' and start[1] == b'U' \
  *             and start[2] == b'L' and start[3] == b'L':
  */
 }
 
 /* "psycopg_c/types/array.pyx":177
@@ -78259,16 +78259,16 @@
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 447, __pyx_L1_error)
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(1, 59, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(3, 278, __pyx_L1_error)
   __pyx_builtin_format = __Pyx_GetBuiltinName(__pyx_n_s_format); if (!__pyx_builtin_format) __PYX_ERR(3, 597, __pyx_L1_error)
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(4, 191, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(4, 195, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(4, 185, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(4, 189, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(5, 61, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(5, 638, __pyx_L1_error)
   __pyx_builtin_OverflowError = __Pyx_GetBuiltinName(__pyx_n_s_OverflowError); if (!__pyx_builtin_OverflowError) __PYX_ERR(5, 676, __pyx_L1_error)
   __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(5, 1101, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(6, 208, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(12, 308, __pyx_L1_error)
   return 0;
@@ -78775,26 +78775,26 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(2, 3, __pyx_L1_error)
 
-  /* "psycopg_c/_psycopg/waiting.pyx":160
+  /* "psycopg_c/_psycopg/waiting.pyx":154
  * 
  * 
  * def wait_c(gen: PQGen[RV], int fileno, timeout = None) -> RV:             # <<<<<<<<<<<<<<
  *     """
  *     Wait for a generator using poll or select.
  */
-  __pyx_tuple__90 = PyTuple_Pack(10, __pyx_n_s_gen, __pyx_n_s_fileno, __pyx_n_s_timeout, __pyx_n_s_ctimeout, __pyx_n_s_wait, __pyx_n_s_ready, __pyx_n_s_pyready, __pyx_n_s_send, __pyx_n_s_ex, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__90)) __PYX_ERR(4, 160, __pyx_L1_error)
+  __pyx_tuple__90 = PyTuple_Pack(10, __pyx_n_s_gen, __pyx_n_s_fileno, __pyx_n_s_timeout, __pyx_n_s_ctimeout, __pyx_n_s_wait, __pyx_n_s_ready, __pyx_n_s_pyready, __pyx_n_s_send, __pyx_n_s_ex, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__90)) __PYX_ERR(4, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__90);
   __Pyx_GIVEREF(__pyx_tuple__90);
-  __pyx_codeobj__91 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__90, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c__psycopg_waiting_pyx, __pyx_n_s_wait_c, 160, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__91)) __PYX_ERR(4, 160, __pyx_L1_error)
-  __pyx_tuple__92 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__92)) __PYX_ERR(4, 160, __pyx_L1_error)
+  __pyx_codeobj__91 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__90, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c__psycopg_waiting_pyx, __pyx_n_s_wait_c, 154, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__91)) __PYX_ERR(4, 154, __pyx_L1_error)
+  __pyx_tuple__92 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__92)) __PYX_ERR(4, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__92);
   __Pyx_GIVEREF(__pyx_tuple__92);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -85934,31 +85934,31 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_8_psycopg_11Transformer_27__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Transformer___setstate_cython, NULL, __pyx_n_s_psycopg_c__psycopg, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(2, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "psycopg_c/_psycopg/waiting.pyx":160
+  /* "psycopg_c/_psycopg/waiting.pyx":154
  * 
  * 
  * def wait_c(gen: PQGen[RV], int fileno, timeout = None) -> RV:             # <<<<<<<<<<<<<<
  *     """
  *     Wait for a generator using poll or select.
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(4, 160, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(4, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_gen, __pyx_kp_s_PQGen_RV) < 0) __PYX_ERR(4, 160, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_RV) < 0) __PYX_ERR(4, 160, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_8_psycopg_27wait_c, 0, __pyx_n_s_wait_c, NULL, __pyx_n_s_psycopg_c__psycopg, __pyx_d, ((PyObject *)__pyx_codeobj__91)); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 160, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_gen, __pyx_kp_s_PQGen_RV) < 0) __PYX_ERR(4, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_RV) < 0) __PYX_ERR(4, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_8_psycopg_27wait_c, 0, __pyx_n_s_wait_c, NULL, __pyx_n_s_psycopg_c__psycopg, __pyx_d, ((PyObject *)__pyx_codeobj__91)); if (unlikely(!__pyx_t_3)) __PYX_ERR(4, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__92);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_wait_c, __pyx_t_3) < 0) __PYX_ERR(4, 160, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_wait_c, __pyx_t_3) < 0) __PYX_ERR(4, 154, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "psycopg_c/types/array.pyx":21
  * from psycopg_c._psycopg cimport endian
  * 
  * from psycopg import errors as e             # <<<<<<<<<<<<<<
  *
```

### Comparing `psycopg-c-3.1.7/psycopg_c/_psycopg.pyi` & `psycopg-c-3.1.8/psycopg_c/_psycopg.pyi`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/psycopg_c/pq/libpq.pxd` & `psycopg-c-3.1.8/psycopg_c/pq/libpq.pxd`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/psycopg_c/pq.c` & `psycopg-c-3.1.8/psycopg_c/pq.c`

 * *Files 1% similar despite different names*

```diff
@@ -1322,15 +1322,15 @@
   "<stringsource>",
   "psycopg_c/pq.pyx",
   "psycopg_c/pq/pgresult.pyx",
   "psycopg_c/pq/pgcancel.pyx",
   "psycopg_c/pq/conninfo.pyx",
   "psycopg_c/pq/escaping.pyx",
   "psycopg_c/pq/pqbuffer.pyx",
-  ".eggs/Cython-3.0.0a11-py3.9-linux-x86_64.egg/Cython/Includes/cpython/type.pxd",
+  "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
@@ -1369,15 +1369,15 @@
  * ctypedef char *(*conn_bytes_f) (const libpq.PGconn *)
  * ctypedef int(*conn_int_f) (const libpq.PGconn *)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 typedef int (*__pyx_t_9psycopg_c_2pq_conn_int_f)(PGconn const *);
 
-/* "psycopg_c/pq/pgconn.pyx":665
+/* "psycopg_c/pq/pgconn.pyx":671
  * 
  * 
  * cdef (Py_ssize_t, libpq.Oid *, char * const*, int *, int *) _query_params_args(             # <<<<<<<<<<<<<<
  *     list param_values: Optional[Sequence[Optional[bytes]]],
  *     param_types: Optional[Sequence[int]],
  */
 struct __pyx_ctuple_9512b6__Py_ssize_t__and_Oid__ptr__and_char__ptrconst__ptr__and_int__ptr__and_int__ptr__etc {
@@ -2500,21 +2500,21 @@
 static const char __pyx_k_x[] = "x";
 static const char __pyx_k__2[] = "<";
 static const char __pyx_k__3[] = " ";
 static const char __pyx_k__4[] = ">";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_rv[] = "rv";
-static const char __pyx_k__12[] = "";
-static const char __pyx_k__14[] = " [";
-static const char __pyx_k__17[] = " (";
-static const char __pyx_k__18[] = ")>";
-static const char __pyx_k__19[] = "(";
-static const char __pyx_k__20[] = ")";
-static const char __pyx_k__22[] = "*";
+static const char __pyx_k__11[] = "";
+static const char __pyx_k__13[] = " [";
+static const char __pyx_k__16[] = " (";
+static const char __pyx_k__17[] = ")>";
+static const char __pyx_k__18[] = "(";
+static const char __pyx_k__19[] = ")";
+static const char __pyx_k__21[] = "*";
 static const char __pyx_k_buf[] = "buf";
 static const char __pyx_k_cls[] = "cls";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_exc[] = "exc";
 static const char __pyx_k_got[] = "got ";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_new[] = "__new__";
@@ -2523,15 +2523,15 @@
 static const char __pyx_k_ptr[] = "ptr";
 static const char __pyx_k_res[] = "res";
 static const char __pyx_k_ssl[] = "ssl";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_val[] = "val";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_TEXT[] = "TEXT";
-static const char __pyx_k__135[] = "?";
+static const char __pyx_k__134[] = "?";
 static const char __pyx_k_ccol[] = "ccol";
 static const char __pyx_k_cerr[] = "cerr";
 static const char __pyx_k_conn[] = "conn";
 static const char __pyx_k_crow[] = "crow";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_exec[] = "exec_";
@@ -2795,14 +2795,16 @@
 static const char __pyx_k_escape_literal_failed[] = "escape_literal failed: ";
 static const char __pyx_k_pyx_unpickle_Escaping[] = "__pyx_unpickle_Escaping";
 static const char __pyx_k_Escaping_escape_string[] = "Escaping.escape_string";
 static const char __pyx_k_PGconn___reduce_cython[] = "PGconn.__reduce_cython__";
 static const char __pyx_k_PGconn_describe_portal[] = "PGconn.describe_portal";
 static const char __pyx_k_PGconn_set_trace_flags[] = "PGconn.set_trace_flags";
 static const char __pyx_k_consuming_input_failed[] = "consuming input failed: ";
+static const char __pyx_k_executing_query_failed[] = "executing query failed: ";
+static const char __pyx_k_preparing_query_failed[] = "preparing query failed: ";
 static const char __pyx_k_send_describe_prepared[] = "send_describe_prepared";
 static const char __pyx_k_the_connection_is_lost[] = "the connection is lost";
 static const char __pyx_k_Escaping_escape_literal[] = "Escaping.escape_literal";
 static const char __pyx_k_Escaping_unescape_bytea[] = "Escaping.unescape_bytea";
 static const char __pyx_k_Optional_Sequence_bytes[] = "Optional[Sequence[bytes]]";
 static const char __pyx_k_PGconn_encrypt_password[] = "PGconn.encrypt_password";
 static const char __pyx_k_PGconn_parameter_status[] = "PGconn.parameter_status";
@@ -2816,14 +2818,15 @@
 static const char __pyx_k_PGconn___setstate_cython[] = "PGconn.__setstate_cython__";
 static const char __pyx_k_PGconn_describe_prepared[] = "PGconn.describe_prepared";
 static const char __pyx_k_PGconn_make_empty_result[] = "PGconn.make_empty_result";
 static const char __pyx_k_PGconn_send_query_params[] = "PGconn.send_query_params";
 static const char __pyx_k_PGresult___reduce_cython[] = "PGresult.__reduce_cython__";
 static const char __pyx_k_PQBuffer___reduce_cython[] = "PQBuffer.__reduce_cython__";
 static const char __pyx_k_couldn_t_allocate_PGconn[] = "couldn't allocate PGconn";
+static const char __pyx_k_describe_prepared_failed[] = "describe prepared failed: ";
 static const char __pyx_k_escape_identifier_failed[] = "escape_identifier failed: ";
 static const char __pyx_k_sending_copy_data_failed[] = "sending copy data failed: ";
 static const char __pyx_k_the_connection_is_closed[] = "the connection is closed";
 static const char __pyx_k_PGconn_exit_pipeline_mode[] = "PGconn.exit_pipeline_mode";
 static const char __pyx_k_PGconn_send_flush_request[] = "PGconn.send_flush_request";
 static const char __pyx_k_couldn_t_reset_connection[] = "couldn't reset connection";
 static const char __pyx_k_psycopg_c_pq_conninfo_pyx[] = "psycopg_c/pq/conninfo.pyx";
@@ -2835,28 +2838,28 @@
 static const char __pyx_k_PGcancel___setstate_cython[] = "PGcancel.__setstate_cython__";
 static const char __pyx_k_PGconn_enter_pipeline_mode[] = "PGconn.enter_pipeline_mode";
 static const char __pyx_k_PGconn_send_query_prepared[] = "PGconn.send_query_prepared";
 static const char __pyx_k_PGconn_set_single_row_mode[] = "PGconn.set_single_row_mode";
 static const char __pyx_k_PGresult___setstate_cython[] = "PGresult.__setstate_cython__";
 static const char __pyx_k_PQBuffer___setstate_cython[] = "PQBuffer.__setstate_cython__";
 static const char __pyx_k_ViewBuffer___reduce_cython[] = "ViewBuffer.__reduce_cython__";
-static const char __pyx_k_couldn_t_allocate_PGresult[] = "couldn't allocate PGresult";
 static const char __pyx_k_error_in_notice_receiver_s[] = "error in notice receiver: %s";
 static const char __pyx_k_password_encryption_failed[] = "password encryption failed: ";
 static const char __pyx_k_receiving_copy_data_failed[] = "receiving copy data failed: ";
 static const char __pyx_k_setting_nonblocking_failed[] = "setting nonblocking failed: ";
 static const char __pyx_k_PGconn_send_describe_portal[] = "PGconn.send_describe_portal";
 static const char __pyx_k_ViewBuffer___setstate_cython[] = "ViewBuffer.__setstate_cython__";
 static const char __pyx_k_bytes_or_buffer_expected_got[] = "bytes or buffer expected, got ";
 static const char __pyx_k_PGconn_send_describe_prepared[] = "PGconn.send_describe_prepared";
 static const char __pyx_k_couldn_t_create_cancel_object[] = "couldn't create cancel object";
 static const char __pyx_k_failed_to_enter_pipeline_mode[] = "failed to enter pipeline mode";
 static const char __pyx_k_sending_prepared_query_failed[] = "sending prepared query failed: ";
 static const char __pyx_k_setting_single_row_mode_failed[] = "setting single row mode failed";
 static const char __pyx_k_connection_not_in_pipeline_mode[] = "connection not in pipeline mode";
+static const char __pyx_k_executing_prepared_query_failed[] = "executing prepared query failed: ";
 static const char __pyx_k_libpq_Python_wrapper_using_cyth[] = "\nlibpq Python wrapper using cython bindings.\n";
 static const char __pyx_k_sending_query_and_params_failed[] = "sending query and params failed: ";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x0804127, 0x3908a35, 0x0c1d0e2) = (conn))";
 static const char __pyx_k_Optional_Sequence_Optional_bytes[] = "Optional[Sequence[Optional[bytes]]]";
 static const char __pyx_k_PQencryptPasswordConn_requires_l[] = "PQencryptPasswordConn requires libpq from PostgreSQL 10, ";
 static const char __pyx_k_PQenterPipelineMode_requires_lib[] = "PQenterPipelineMode requires libpq from PostgreSQL 14, ";
 static const char __pyx_k_PQexitPipelineMode_requires_libp[] = "PQexitPipelineMode requires libpq from PostgreSQL 14, ";
@@ -2988,23 +2991,23 @@
 static PyObject *__pyx_n_s_Trace;
 static PyObject *__pyx_kp_s_Tuple_int_memoryview;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_ViewBuffer;
 static PyObject *__pyx_n_s_ViewBuffer___reduce_cython;
 static PyObject *__pyx_n_s_ViewBuffer___setstate_cython;
-static PyObject *__pyx_kp_b__12;
-static PyObject *__pyx_n_s__135;
-static PyObject *__pyx_kp_u__14;
+static PyObject *__pyx_kp_b__11;
+static PyObject *__pyx_kp_u__13;
+static PyObject *__pyx_n_s__134;
+static PyObject *__pyx_kp_u__16;
 static PyObject *__pyx_kp_u__17;
 static PyObject *__pyx_kp_u__18;
 static PyObject *__pyx_kp_u__19;
 static PyObject *__pyx_kp_u__2;
-static PyObject *__pyx_kp_u__20;
-static PyObject *__pyx_n_s__22;
+static PyObject *__pyx_n_s__21;
 static PyObject *__pyx_kp_u__3;
 static PyObject *__pyx_kp_u__4;
 static PyObject *__pyx_n_s_algorithm;
 static PyObject *__pyx_n_u_ascii;
 static PyObject *__pyx_n_s_async;
 static PyObject *__pyx_n_s_asyncio_coroutines;
 static PyObject *__pyx_kp_u_at_0x;
@@ -3044,15 +3047,14 @@
 static PyObject *__pyx_n_s_connect_start;
 static PyObject *__pyx_kp_u_connection_not_in_pipeline_mode;
 static PyObject *__pyx_n_s_connection_summary;
 static PyObject *__pyx_n_s_conninfo;
 static PyObject *__pyx_n_s_consume_input;
 static PyObject *__pyx_kp_u_consuming_input_failed;
 static PyObject *__pyx_kp_u_couldn_t_allocate_PGconn;
-static PyObject *__pyx_kp_u_couldn_t_allocate_PGresult;
 static PyObject *__pyx_kp_u_couldn_t_allocate_connection_def;
 static PyObject *__pyx_kp_u_couldn_t_allocate_connection_inf;
 static PyObject *__pyx_kp_u_couldn_t_allocate_empty_PGresult;
 static PyObject *__pyx_kp_u_couldn_t_allocate_for_escape_byt;
 static PyObject *__pyx_kp_u_couldn_t_allocate_for_unescape_b;
 static PyObject *__pyx_kp_u_couldn_t_allocate_on_conninfo_pa;
 static PyObject *__pyx_kp_u_couldn_t_create_cancel_object;
@@ -3063,14 +3065,15 @@
 static PyObject *__pyx_n_s_cvalues;
 static PyObject *__pyx_n_u_d;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_descr;
 static PyObject *__pyx_n_s_describe_portal;
 static PyObject *__pyx_n_s_describe_prepared;
+static PyObject *__pyx_kp_u_describe_prepared_failed;
 static PyObject *__pyx_n_s_descriptions;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_dict_2;
 static PyObject *__pyx_kp_u_disable;
 static PyObject *__pyx_n_s_dispchar;
 static PyObject *__pyx_n_s_dispsize;
 static PyObject *__pyx_n_s_doc;
@@ -3096,14 +3099,16 @@
 static PyObject *__pyx_kp_u_escape_string_failed;
 static PyObject *__pyx_n_s_exc;
 static PyObject *__pyx_n_s_exception;
 static PyObject *__pyx_n_s_exec;
 static PyObject *__pyx_n_s_exec_params;
 static PyObject *__pyx_n_s_exec_prepared;
 static PyObject *__pyx_n_s_exec_status;
+static PyObject *__pyx_kp_u_executing_prepared_query_failed;
+static PyObject *__pyx_kp_u_executing_query_failed;
 static PyObject *__pyx_n_s_exit_pipeline_mode;
 static PyObject *__pyx_kp_u_failed_to_enter_pipeline_mode;
 static PyObject *__pyx_kp_u_failed_to_sync_pipeline;
 static PyObject *__pyx_n_s_fformat;
 static PyObject *__pyx_n_s_fieldcode;
 static PyObject *__pyx_n_s_fileno;
 static PyObject *__pyx_n_s_finish;
@@ -3175,14 +3180,15 @@
 static PyObject *__pyx_n_s_pgresult;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_ping;
 static PyObject *__pyx_n_s_pipeline_sync;
 static PyObject *__pyx_n_s_platform;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_prepare_2;
+static PyObject *__pyx_kp_u_preparing_query_failed;
 static PyObject *__pyx_n_s_psycopg;
 static PyObject *__pyx_n_u_psycopg;
 static PyObject *__pyx_n_s_psycopg_c_pq;
 static PyObject *__pyx_kp_s_psycopg_c_pq_conninfo_pyx;
 static PyObject *__pyx_kp_s_psycopg_c_pq_escaping_pyx;
 static PyObject *__pyx_kp_s_psycopg_c_pq_pgcancel_pyx;
 static PyObject *__pyx_kp_s_psycopg_c_pq_pgconn_pyx;
@@ -3405,137 +3411,136 @@
 static PyObject *__pyx_tp_new_9psycopg_c_2pq_ViewBuffer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 #if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_int_8405287;
 static PyObject *__pyx_int_12701922;
 static PyObject *__pyx_int_59804213;
 #endif
 #if !CYTHON_USE_MODULE_STATE
+static int __pyx_k__7;
 static int __pyx_k__8;
 static int __pyx_k__9;
 static int __pyx_k__10;
-static int __pyx_k__11;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__12;
+static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__21;
-static PyObject *__pyx_tuple__23;
-static PyObject *__pyx_tuple__25;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_tuple__36;
-static PyObject *__pyx_tuple__38;
-static PyObject *__pyx_tuple__40;
-static PyObject *__pyx_tuple__42;
-static PyObject *__pyx_tuple__44;
-static PyObject *__pyx_tuple__46;
+static PyObject *__pyx_tuple__20;
+static PyObject *__pyx_tuple__22;
+static PyObject *__pyx_tuple__24;
+static PyObject *__pyx_tuple__27;
+static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__45;
+static PyObject *__pyx_tuple__47;
 static PyObject *__pyx_tuple__48;
-static PyObject *__pyx_tuple__49;
-static PyObject *__pyx_tuple__57;
-static PyObject *__pyx_tuple__60;
-static PyObject *__pyx_tuple__64;
-static PyObject *__pyx_tuple__67;
-static PyObject *__pyx_tuple__69;
-static PyObject *__pyx_tuple__71;
-static PyObject *__pyx_tuple__73;
-static PyObject *__pyx_tuple__75;
-static PyObject *__pyx_tuple__78;
-static PyObject *__pyx_tuple__80;
-static PyObject *__pyx_tuple__87;
-static PyObject *__pyx_tuple__90;
-static PyObject *__pyx_tuple__92;
-static PyObject *__pyx_tuple__94;
-static PyObject *__pyx_tuple__101;
-static PyObject *__pyx_tuple__103;
-static PyObject *__pyx_tuple__105;
-static PyObject *__pyx_tuple__110;
-static PyObject *__pyx_tuple__114;
-static PyObject *__pyx_tuple__116;
-static PyObject *__pyx_tuple__119;
-static PyObject *__pyx_tuple__124;
-static PyObject *__pyx_tuple__126;
-static PyObject *__pyx_tuple__133;
-static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_tuple__56;
+static PyObject *__pyx_tuple__59;
+static PyObject *__pyx_tuple__63;
+static PyObject *__pyx_tuple__66;
+static PyObject *__pyx_tuple__68;
+static PyObject *__pyx_tuple__70;
+static PyObject *__pyx_tuple__72;
+static PyObject *__pyx_tuple__74;
+static PyObject *__pyx_tuple__77;
+static PyObject *__pyx_tuple__79;
+static PyObject *__pyx_tuple__86;
+static PyObject *__pyx_tuple__89;
+static PyObject *__pyx_tuple__91;
+static PyObject *__pyx_tuple__93;
+static PyObject *__pyx_tuple__100;
+static PyObject *__pyx_tuple__102;
+static PyObject *__pyx_tuple__104;
+static PyObject *__pyx_tuple__109;
+static PyObject *__pyx_tuple__113;
+static PyObject *__pyx_tuple__115;
+static PyObject *__pyx_tuple__118;
+static PyObject *__pyx_tuple__123;
+static PyObject *__pyx_tuple__125;
+static PyObject *__pyx_tuple__132;
+static PyObject *__pyx_codeobj__23;
+static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__26;
-static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_codeobj__28;
 static PyObject *__pyx_codeobj__29;
 static PyObject *__pyx_codeobj__30;
 static PyObject *__pyx_codeobj__31;
 static PyObject *__pyx_codeobj__32;
-static PyObject *__pyx_codeobj__33;
-static PyObject *__pyx_codeobj__35;
-static PyObject *__pyx_codeobj__37;
-static PyObject *__pyx_codeobj__39;
-static PyObject *__pyx_codeobj__41;
-static PyObject *__pyx_codeobj__43;
-static PyObject *__pyx_codeobj__45;
-static PyObject *__pyx_codeobj__47;
+static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__40;
+static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_codeobj__44;
+static PyObject *__pyx_codeobj__46;
+static PyObject *__pyx_codeobj__49;
 static PyObject *__pyx_codeobj__50;
 static PyObject *__pyx_codeobj__51;
 static PyObject *__pyx_codeobj__52;
 static PyObject *__pyx_codeobj__53;
 static PyObject *__pyx_codeobj__54;
 static PyObject *__pyx_codeobj__55;
-static PyObject *__pyx_codeobj__56;
+static PyObject *__pyx_codeobj__57;
 static PyObject *__pyx_codeobj__58;
-static PyObject *__pyx_codeobj__59;
+static PyObject *__pyx_codeobj__60;
 static PyObject *__pyx_codeobj__61;
 static PyObject *__pyx_codeobj__62;
-static PyObject *__pyx_codeobj__63;
+static PyObject *__pyx_codeobj__64;
 static PyObject *__pyx_codeobj__65;
-static PyObject *__pyx_codeobj__66;
-static PyObject *__pyx_codeobj__68;
-static PyObject *__pyx_codeobj__70;
-static PyObject *__pyx_codeobj__72;
-static PyObject *__pyx_codeobj__74;
+static PyObject *__pyx_codeobj__67;
+static PyObject *__pyx_codeobj__69;
+static PyObject *__pyx_codeobj__71;
+static PyObject *__pyx_codeobj__73;
+static PyObject *__pyx_codeobj__75;
 static PyObject *__pyx_codeobj__76;
-static PyObject *__pyx_codeobj__77;
-static PyObject *__pyx_codeobj__79;
+static PyObject *__pyx_codeobj__78;
+static PyObject *__pyx_codeobj__80;
 static PyObject *__pyx_codeobj__81;
 static PyObject *__pyx_codeobj__82;
 static PyObject *__pyx_codeobj__83;
 static PyObject *__pyx_codeobj__84;
 static PyObject *__pyx_codeobj__85;
-static PyObject *__pyx_codeobj__86;
+static PyObject *__pyx_codeobj__87;
 static PyObject *__pyx_codeobj__88;
-static PyObject *__pyx_codeobj__89;
-static PyObject *__pyx_codeobj__91;
-static PyObject *__pyx_codeobj__93;
+static PyObject *__pyx_codeobj__90;
+static PyObject *__pyx_codeobj__92;
+static PyObject *__pyx_codeobj__94;
 static PyObject *__pyx_codeobj__95;
 static PyObject *__pyx_codeobj__96;
 static PyObject *__pyx_codeobj__97;
 static PyObject *__pyx_codeobj__98;
 static PyObject *__pyx_codeobj__99;
-static PyObject *__pyx_codeobj__100;
-static PyObject *__pyx_codeobj__102;
-static PyObject *__pyx_codeobj__104;
+static PyObject *__pyx_codeobj__101;
+static PyObject *__pyx_codeobj__103;
+static PyObject *__pyx_codeobj__105;
 static PyObject *__pyx_codeobj__106;
 static PyObject *__pyx_codeobj__107;
 static PyObject *__pyx_codeobj__108;
-static PyObject *__pyx_codeobj__109;
+static PyObject *__pyx_codeobj__110;
 static PyObject *__pyx_codeobj__111;
 static PyObject *__pyx_codeobj__112;
-static PyObject *__pyx_codeobj__113;
-static PyObject *__pyx_codeobj__115;
+static PyObject *__pyx_codeobj__114;
+static PyObject *__pyx_codeobj__116;
 static PyObject *__pyx_codeobj__117;
-static PyObject *__pyx_codeobj__118;
+static PyObject *__pyx_codeobj__119;
 static PyObject *__pyx_codeobj__120;
 static PyObject *__pyx_codeobj__121;
 static PyObject *__pyx_codeobj__122;
-static PyObject *__pyx_codeobj__123;
-static PyObject *__pyx_codeobj__125;
+static PyObject *__pyx_codeobj__124;
+static PyObject *__pyx_codeobj__126;
 static PyObject *__pyx_codeobj__127;
 static PyObject *__pyx_codeobj__128;
 static PyObject *__pyx_codeobj__129;
 static PyObject *__pyx_codeobj__130;
 static PyObject *__pyx_codeobj__131;
-static PyObject *__pyx_codeobj__132;
-static PyObject *__pyx_codeobj__134;
+static PyObject *__pyx_codeobj__133;
 #endif
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 #if CYTHON_USE_MODULE_STATE
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
@@ -3673,23 +3678,23 @@
   PyObject *__pyx_n_s_Trace;
   PyObject *__pyx_kp_s_Tuple_int_memoryview;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_ViewBuffer;
   PyObject *__pyx_n_s_ViewBuffer___reduce_cython;
   PyObject *__pyx_n_s_ViewBuffer___setstate_cython;
-  PyObject *__pyx_kp_b__12;
-  PyObject *__pyx_n_s__135;
-  PyObject *__pyx_kp_u__14;
+  PyObject *__pyx_kp_b__11;
+  PyObject *__pyx_kp_u__13;
+  PyObject *__pyx_n_s__134;
+  PyObject *__pyx_kp_u__16;
   PyObject *__pyx_kp_u__17;
   PyObject *__pyx_kp_u__18;
   PyObject *__pyx_kp_u__19;
   PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_kp_u__20;
-  PyObject *__pyx_n_s__22;
+  PyObject *__pyx_n_s__21;
   PyObject *__pyx_kp_u__3;
   PyObject *__pyx_kp_u__4;
   PyObject *__pyx_n_s_algorithm;
   PyObject *__pyx_n_u_ascii;
   PyObject *__pyx_n_s_async;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_kp_u_at_0x;
@@ -3729,15 +3734,14 @@
   PyObject *__pyx_n_s_connect_start;
   PyObject *__pyx_kp_u_connection_not_in_pipeline_mode;
   PyObject *__pyx_n_s_connection_summary;
   PyObject *__pyx_n_s_conninfo;
   PyObject *__pyx_n_s_consume_input;
   PyObject *__pyx_kp_u_consuming_input_failed;
   PyObject *__pyx_kp_u_couldn_t_allocate_PGconn;
-  PyObject *__pyx_kp_u_couldn_t_allocate_PGresult;
   PyObject *__pyx_kp_u_couldn_t_allocate_connection_def;
   PyObject *__pyx_kp_u_couldn_t_allocate_connection_inf;
   PyObject *__pyx_kp_u_couldn_t_allocate_empty_PGresult;
   PyObject *__pyx_kp_u_couldn_t_allocate_for_escape_byt;
   PyObject *__pyx_kp_u_couldn_t_allocate_for_unescape_b;
   PyObject *__pyx_kp_u_couldn_t_allocate_on_conninfo_pa;
   PyObject *__pyx_kp_u_couldn_t_create_cancel_object;
@@ -3748,14 +3752,15 @@
   PyObject *__pyx_n_s_cvalues;
   PyObject *__pyx_n_u_d;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_decode;
   PyObject *__pyx_n_s_descr;
   PyObject *__pyx_n_s_describe_portal;
   PyObject *__pyx_n_s_describe_prepared;
+  PyObject *__pyx_kp_u_describe_prepared_failed;
   PyObject *__pyx_n_s_descriptions;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dict_2;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_s_dispchar;
   PyObject *__pyx_n_s_dispsize;
   PyObject *__pyx_n_s_doc;
@@ -3781,14 +3786,16 @@
   PyObject *__pyx_kp_u_escape_string_failed;
   PyObject *__pyx_n_s_exc;
   PyObject *__pyx_n_s_exception;
   PyObject *__pyx_n_s_exec;
   PyObject *__pyx_n_s_exec_params;
   PyObject *__pyx_n_s_exec_prepared;
   PyObject *__pyx_n_s_exec_status;
+  PyObject *__pyx_kp_u_executing_prepared_query_failed;
+  PyObject *__pyx_kp_u_executing_query_failed;
   PyObject *__pyx_n_s_exit_pipeline_mode;
   PyObject *__pyx_kp_u_failed_to_enter_pipeline_mode;
   PyObject *__pyx_kp_u_failed_to_sync_pipeline;
   PyObject *__pyx_n_s_fformat;
   PyObject *__pyx_n_s_fieldcode;
   PyObject *__pyx_n_s_fileno;
   PyObject *__pyx_n_s_finish;
@@ -3860,14 +3867,15 @@
   PyObject *__pyx_n_s_pgresult;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_ping;
   PyObject *__pyx_n_s_pipeline_sync;
   PyObject *__pyx_n_s_platform;
   PyObject *__pyx_n_s_prepare;
   PyObject *__pyx_n_s_prepare_2;
+  PyObject *__pyx_kp_u_preparing_query_failed;
   PyObject *__pyx_n_s_psycopg;
   PyObject *__pyx_n_u_psycopg;
   PyObject *__pyx_n_s_psycopg_c_pq;
   PyObject *__pyx_kp_s_psycopg_c_pq_conninfo_pyx;
   PyObject *__pyx_kp_s_psycopg_c_pq_escaping_pyx;
   PyObject *__pyx_kp_s_psycopg_c_pq_pgcancel_pyx;
   PyObject *__pyx_kp_s_psycopg_c_pq_pgconn_pyx;
@@ -3946,137 +3954,136 @@
   PyObject *__pyx_n_s_v;
   PyObject *__pyx_n_s_val;
   PyObject *__pyx_n_s_version;
   PyObject *__pyx_n_u_x;
   PyObject *__pyx_int_8405287;
   PyObject *__pyx_int_12701922;
   PyObject *__pyx_int_59804213;
+  int __pyx_k__7;
   int __pyx_k__8;
   int __pyx_k__9;
   int __pyx_k__10;
-  int __pyx_k__11;
   PyObject *__pyx_tuple__5;
   PyObject *__pyx_tuple__6;
-  PyObject *__pyx_tuple__7;
-  PyObject *__pyx_tuple__13;
+  PyObject *__pyx_tuple__12;
+  PyObject *__pyx_tuple__14;
   PyObject *__pyx_tuple__15;
-  PyObject *__pyx_tuple__16;
-  PyObject *__pyx_tuple__21;
-  PyObject *__pyx_tuple__23;
-  PyObject *__pyx_tuple__25;
-  PyObject *__pyx_tuple__28;
-  PyObject *__pyx_tuple__34;
-  PyObject *__pyx_tuple__36;
-  PyObject *__pyx_tuple__38;
-  PyObject *__pyx_tuple__40;
-  PyObject *__pyx_tuple__42;
-  PyObject *__pyx_tuple__44;
-  PyObject *__pyx_tuple__46;
+  PyObject *__pyx_tuple__20;
+  PyObject *__pyx_tuple__22;
+  PyObject *__pyx_tuple__24;
+  PyObject *__pyx_tuple__27;
+  PyObject *__pyx_tuple__33;
+  PyObject *__pyx_tuple__35;
+  PyObject *__pyx_tuple__37;
+  PyObject *__pyx_tuple__39;
+  PyObject *__pyx_tuple__41;
+  PyObject *__pyx_tuple__43;
+  PyObject *__pyx_tuple__45;
+  PyObject *__pyx_tuple__47;
   PyObject *__pyx_tuple__48;
-  PyObject *__pyx_tuple__49;
-  PyObject *__pyx_tuple__57;
-  PyObject *__pyx_tuple__60;
-  PyObject *__pyx_tuple__64;
-  PyObject *__pyx_tuple__67;
-  PyObject *__pyx_tuple__69;
-  PyObject *__pyx_tuple__71;
-  PyObject *__pyx_tuple__73;
-  PyObject *__pyx_tuple__75;
-  PyObject *__pyx_tuple__78;
-  PyObject *__pyx_tuple__80;
-  PyObject *__pyx_tuple__87;
-  PyObject *__pyx_tuple__90;
-  PyObject *__pyx_tuple__92;
-  PyObject *__pyx_tuple__94;
-  PyObject *__pyx_tuple__101;
-  PyObject *__pyx_tuple__103;
-  PyObject *__pyx_tuple__105;
-  PyObject *__pyx_tuple__110;
-  PyObject *__pyx_tuple__114;
-  PyObject *__pyx_tuple__116;
-  PyObject *__pyx_tuple__119;
-  PyObject *__pyx_tuple__124;
-  PyObject *__pyx_tuple__126;
-  PyObject *__pyx_tuple__133;
-  PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_tuple__56;
+  PyObject *__pyx_tuple__59;
+  PyObject *__pyx_tuple__63;
+  PyObject *__pyx_tuple__66;
+  PyObject *__pyx_tuple__68;
+  PyObject *__pyx_tuple__70;
+  PyObject *__pyx_tuple__72;
+  PyObject *__pyx_tuple__74;
+  PyObject *__pyx_tuple__77;
+  PyObject *__pyx_tuple__79;
+  PyObject *__pyx_tuple__86;
+  PyObject *__pyx_tuple__89;
+  PyObject *__pyx_tuple__91;
+  PyObject *__pyx_tuple__93;
+  PyObject *__pyx_tuple__100;
+  PyObject *__pyx_tuple__102;
+  PyObject *__pyx_tuple__104;
+  PyObject *__pyx_tuple__109;
+  PyObject *__pyx_tuple__113;
+  PyObject *__pyx_tuple__115;
+  PyObject *__pyx_tuple__118;
+  PyObject *__pyx_tuple__123;
+  PyObject *__pyx_tuple__125;
+  PyObject *__pyx_tuple__132;
+  PyObject *__pyx_codeobj__23;
+  PyObject *__pyx_codeobj__25;
   PyObject *__pyx_codeobj__26;
-  PyObject *__pyx_codeobj__27;
+  PyObject *__pyx_codeobj__28;
   PyObject *__pyx_codeobj__29;
   PyObject *__pyx_codeobj__30;
   PyObject *__pyx_codeobj__31;
   PyObject *__pyx_codeobj__32;
-  PyObject *__pyx_codeobj__33;
-  PyObject *__pyx_codeobj__35;
-  PyObject *__pyx_codeobj__37;
-  PyObject *__pyx_codeobj__39;
-  PyObject *__pyx_codeobj__41;
-  PyObject *__pyx_codeobj__43;
-  PyObject *__pyx_codeobj__45;
-  PyObject *__pyx_codeobj__47;
+  PyObject *__pyx_codeobj__34;
+  PyObject *__pyx_codeobj__36;
+  PyObject *__pyx_codeobj__38;
+  PyObject *__pyx_codeobj__40;
+  PyObject *__pyx_codeobj__42;
+  PyObject *__pyx_codeobj__44;
+  PyObject *__pyx_codeobj__46;
+  PyObject *__pyx_codeobj__49;
   PyObject *__pyx_codeobj__50;
   PyObject *__pyx_codeobj__51;
   PyObject *__pyx_codeobj__52;
   PyObject *__pyx_codeobj__53;
   PyObject *__pyx_codeobj__54;
   PyObject *__pyx_codeobj__55;
-  PyObject *__pyx_codeobj__56;
+  PyObject *__pyx_codeobj__57;
   PyObject *__pyx_codeobj__58;
-  PyObject *__pyx_codeobj__59;
+  PyObject *__pyx_codeobj__60;
   PyObject *__pyx_codeobj__61;
   PyObject *__pyx_codeobj__62;
-  PyObject *__pyx_codeobj__63;
+  PyObject *__pyx_codeobj__64;
   PyObject *__pyx_codeobj__65;
-  PyObject *__pyx_codeobj__66;
-  PyObject *__pyx_codeobj__68;
-  PyObject *__pyx_codeobj__70;
-  PyObject *__pyx_codeobj__72;
-  PyObject *__pyx_codeobj__74;
+  PyObject *__pyx_codeobj__67;
+  PyObject *__pyx_codeobj__69;
+  PyObject *__pyx_codeobj__71;
+  PyObject *__pyx_codeobj__73;
+  PyObject *__pyx_codeobj__75;
   PyObject *__pyx_codeobj__76;
-  PyObject *__pyx_codeobj__77;
-  PyObject *__pyx_codeobj__79;
+  PyObject *__pyx_codeobj__78;
+  PyObject *__pyx_codeobj__80;
   PyObject *__pyx_codeobj__81;
   PyObject *__pyx_codeobj__82;
   PyObject *__pyx_codeobj__83;
   PyObject *__pyx_codeobj__84;
   PyObject *__pyx_codeobj__85;
-  PyObject *__pyx_codeobj__86;
+  PyObject *__pyx_codeobj__87;
   PyObject *__pyx_codeobj__88;
-  PyObject *__pyx_codeobj__89;
-  PyObject *__pyx_codeobj__91;
-  PyObject *__pyx_codeobj__93;
+  PyObject *__pyx_codeobj__90;
+  PyObject *__pyx_codeobj__92;
+  PyObject *__pyx_codeobj__94;
   PyObject *__pyx_codeobj__95;
   PyObject *__pyx_codeobj__96;
   PyObject *__pyx_codeobj__97;
   PyObject *__pyx_codeobj__98;
   PyObject *__pyx_codeobj__99;
-  PyObject *__pyx_codeobj__100;
-  PyObject *__pyx_codeobj__102;
-  PyObject *__pyx_codeobj__104;
+  PyObject *__pyx_codeobj__101;
+  PyObject *__pyx_codeobj__103;
+  PyObject *__pyx_codeobj__105;
   PyObject *__pyx_codeobj__106;
   PyObject *__pyx_codeobj__107;
   PyObject *__pyx_codeobj__108;
-  PyObject *__pyx_codeobj__109;
+  PyObject *__pyx_codeobj__110;
   PyObject *__pyx_codeobj__111;
   PyObject *__pyx_codeobj__112;
-  PyObject *__pyx_codeobj__113;
-  PyObject *__pyx_codeobj__115;
+  PyObject *__pyx_codeobj__114;
+  PyObject *__pyx_codeobj__116;
   PyObject *__pyx_codeobj__117;
-  PyObject *__pyx_codeobj__118;
+  PyObject *__pyx_codeobj__119;
   PyObject *__pyx_codeobj__120;
   PyObject *__pyx_codeobj__121;
   PyObject *__pyx_codeobj__122;
-  PyObject *__pyx_codeobj__123;
-  PyObject *__pyx_codeobj__125;
+  PyObject *__pyx_codeobj__124;
+  PyObject *__pyx_codeobj__126;
   PyObject *__pyx_codeobj__127;
   PyObject *__pyx_codeobj__128;
   PyObject *__pyx_codeobj__129;
   PyObject *__pyx_codeobj__130;
   PyObject *__pyx_codeobj__131;
-  PyObject *__pyx_codeobj__132;
-  PyObject *__pyx_codeobj__134;
+  PyObject *__pyx_codeobj__133;
 } __pyx_mstate;
 
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
 #else
@@ -4230,23 +4237,23 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Trace);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Tuple_int_memoryview);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ViewBuffer);
   Py_CLEAR(clear_module_state->__pyx_n_s_ViewBuffer___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_ViewBuffer___setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_kp_b__12);
-  Py_CLEAR(clear_module_state->__pyx_n_s__135);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__14);
+  Py_CLEAR(clear_module_state->__pyx_kp_b__11);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__13);
+  Py_CLEAR(clear_module_state->__pyx_n_s__134);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__16);
   Py_CLEAR(clear_module_state->__pyx_kp_u__17);
   Py_CLEAR(clear_module_state->__pyx_kp_u__18);
   Py_CLEAR(clear_module_state->__pyx_kp_u__19);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__20);
-  Py_CLEAR(clear_module_state->__pyx_n_s__22);
+  Py_CLEAR(clear_module_state->__pyx_n_s__21);
   Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_kp_u__4);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithm);
   Py_CLEAR(clear_module_state->__pyx_n_u_ascii);
   Py_CLEAR(clear_module_state->__pyx_n_s_async);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_kp_u_at_0x);
@@ -4286,15 +4293,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_connect_start);
   Py_CLEAR(clear_module_state->__pyx_kp_u_connection_not_in_pipeline_mode);
   Py_CLEAR(clear_module_state->__pyx_n_s_connection_summary);
   Py_CLEAR(clear_module_state->__pyx_n_s_conninfo);
   Py_CLEAR(clear_module_state->__pyx_n_s_consume_input);
   Py_CLEAR(clear_module_state->__pyx_kp_u_consuming_input_failed);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_PGconn);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_PGresult);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_connection_def);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_connection_inf);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_empty_PGresult);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_for_escape_byt);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_for_unescape_b);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_allocate_on_conninfo_pa);
   Py_CLEAR(clear_module_state->__pyx_kp_u_couldn_t_create_cancel_object);
@@ -4305,14 +4311,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_cvalues);
   Py_CLEAR(clear_module_state->__pyx_n_u_d);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_descr);
   Py_CLEAR(clear_module_state->__pyx_n_s_describe_portal);
   Py_CLEAR(clear_module_state->__pyx_n_s_describe_prepared);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_describe_prepared_failed);
   Py_CLEAR(clear_module_state->__pyx_n_s_descriptions);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_s_dispchar);
   Py_CLEAR(clear_module_state->__pyx_n_s_dispsize);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
@@ -4338,14 +4345,16 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_escape_string_failed);
   Py_CLEAR(clear_module_state->__pyx_n_s_exc);
   Py_CLEAR(clear_module_state->__pyx_n_s_exception);
   Py_CLEAR(clear_module_state->__pyx_n_s_exec);
   Py_CLEAR(clear_module_state->__pyx_n_s_exec_params);
   Py_CLEAR(clear_module_state->__pyx_n_s_exec_prepared);
   Py_CLEAR(clear_module_state->__pyx_n_s_exec_status);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_executing_prepared_query_failed);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_executing_query_failed);
   Py_CLEAR(clear_module_state->__pyx_n_s_exit_pipeline_mode);
   Py_CLEAR(clear_module_state->__pyx_kp_u_failed_to_enter_pipeline_mode);
   Py_CLEAR(clear_module_state->__pyx_kp_u_failed_to_sync_pipeline);
   Py_CLEAR(clear_module_state->__pyx_n_s_fformat);
   Py_CLEAR(clear_module_state->__pyx_n_s_fieldcode);
   Py_CLEAR(clear_module_state->__pyx_n_s_fileno);
   Py_CLEAR(clear_module_state->__pyx_n_s_finish);
@@ -4417,14 +4426,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_pgresult);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_ping);
   Py_CLEAR(clear_module_state->__pyx_n_s_pipeline_sync);
   Py_CLEAR(clear_module_state->__pyx_n_s_platform);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare_2);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_preparing_query_failed);
   Py_CLEAR(clear_module_state->__pyx_n_s_psycopg);
   Py_CLEAR(clear_module_state->__pyx_n_u_psycopg);
   Py_CLEAR(clear_module_state->__pyx_n_s_psycopg_c_pq);
   Py_CLEAR(clear_module_state->__pyx_kp_s_psycopg_c_pq_conninfo_pyx);
   Py_CLEAR(clear_module_state->__pyx_kp_s_psycopg_c_pq_escaping_pyx);
   Py_CLEAR(clear_module_state->__pyx_kp_s_psycopg_c_pq_pgcancel_pyx);
   Py_CLEAR(clear_module_state->__pyx_kp_s_psycopg_c_pq_pgconn_pyx);
@@ -4503,137 +4513,136 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_v);
   Py_CLEAR(clear_module_state->__pyx_n_s_val);
   Py_CLEAR(clear_module_state->__pyx_n_s_version);
   Py_CLEAR(clear_module_state->__pyx_n_u_x);
   Py_CLEAR(clear_module_state->__pyx_int_8405287);
   Py_CLEAR(clear_module_state->__pyx_int_12701922);
   Py_CLEAR(clear_module_state->__pyx_int_59804213);
+  Py_CLEAR(clear_module_state->__pyx_k__7);
   Py_CLEAR(clear_module_state->__pyx_k__8);
   Py_CLEAR(clear_module_state->__pyx_k__9);
   Py_CLEAR(clear_module_state->__pyx_k__10);
-  Py_CLEAR(clear_module_state->__pyx_k__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
-  Py_CLEAR(clear_module_state->__pyx_tuple__7);
-  Py_CLEAR(clear_module_state->__pyx_tuple__13);
+  Py_CLEAR(clear_module_state->__pyx_tuple__12);
+  Py_CLEAR(clear_module_state->__pyx_tuple__14);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
-  Py_CLEAR(clear_module_state->__pyx_tuple__16);
-  Py_CLEAR(clear_module_state->__pyx_tuple__21);
-  Py_CLEAR(clear_module_state->__pyx_tuple__23);
-  Py_CLEAR(clear_module_state->__pyx_tuple__25);
-  Py_CLEAR(clear_module_state->__pyx_tuple__28);
-  Py_CLEAR(clear_module_state->__pyx_tuple__34);
-  Py_CLEAR(clear_module_state->__pyx_tuple__36);
-  Py_CLEAR(clear_module_state->__pyx_tuple__38);
-  Py_CLEAR(clear_module_state->__pyx_tuple__40);
-  Py_CLEAR(clear_module_state->__pyx_tuple__42);
-  Py_CLEAR(clear_module_state->__pyx_tuple__44);
-  Py_CLEAR(clear_module_state->__pyx_tuple__46);
+  Py_CLEAR(clear_module_state->__pyx_tuple__20);
+  Py_CLEAR(clear_module_state->__pyx_tuple__22);
+  Py_CLEAR(clear_module_state->__pyx_tuple__24);
+  Py_CLEAR(clear_module_state->__pyx_tuple__27);
+  Py_CLEAR(clear_module_state->__pyx_tuple__33);
+  Py_CLEAR(clear_module_state->__pyx_tuple__35);
+  Py_CLEAR(clear_module_state->__pyx_tuple__37);
+  Py_CLEAR(clear_module_state->__pyx_tuple__39);
+  Py_CLEAR(clear_module_state->__pyx_tuple__41);
+  Py_CLEAR(clear_module_state->__pyx_tuple__43);
+  Py_CLEAR(clear_module_state->__pyx_tuple__45);
+  Py_CLEAR(clear_module_state->__pyx_tuple__47);
   Py_CLEAR(clear_module_state->__pyx_tuple__48);
-  Py_CLEAR(clear_module_state->__pyx_tuple__49);
-  Py_CLEAR(clear_module_state->__pyx_tuple__57);
-  Py_CLEAR(clear_module_state->__pyx_tuple__60);
-  Py_CLEAR(clear_module_state->__pyx_tuple__64);
-  Py_CLEAR(clear_module_state->__pyx_tuple__67);
-  Py_CLEAR(clear_module_state->__pyx_tuple__69);
-  Py_CLEAR(clear_module_state->__pyx_tuple__71);
-  Py_CLEAR(clear_module_state->__pyx_tuple__73);
-  Py_CLEAR(clear_module_state->__pyx_tuple__75);
-  Py_CLEAR(clear_module_state->__pyx_tuple__78);
-  Py_CLEAR(clear_module_state->__pyx_tuple__80);
-  Py_CLEAR(clear_module_state->__pyx_tuple__87);
-  Py_CLEAR(clear_module_state->__pyx_tuple__90);
-  Py_CLEAR(clear_module_state->__pyx_tuple__92);
-  Py_CLEAR(clear_module_state->__pyx_tuple__94);
-  Py_CLEAR(clear_module_state->__pyx_tuple__101);
-  Py_CLEAR(clear_module_state->__pyx_tuple__103);
-  Py_CLEAR(clear_module_state->__pyx_tuple__105);
-  Py_CLEAR(clear_module_state->__pyx_tuple__110);
-  Py_CLEAR(clear_module_state->__pyx_tuple__114);
-  Py_CLEAR(clear_module_state->__pyx_tuple__116);
-  Py_CLEAR(clear_module_state->__pyx_tuple__119);
-  Py_CLEAR(clear_module_state->__pyx_tuple__124);
-  Py_CLEAR(clear_module_state->__pyx_tuple__126);
-  Py_CLEAR(clear_module_state->__pyx_tuple__133);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_tuple__56);
+  Py_CLEAR(clear_module_state->__pyx_tuple__59);
+  Py_CLEAR(clear_module_state->__pyx_tuple__63);
+  Py_CLEAR(clear_module_state->__pyx_tuple__66);
+  Py_CLEAR(clear_module_state->__pyx_tuple__68);
+  Py_CLEAR(clear_module_state->__pyx_tuple__70);
+  Py_CLEAR(clear_module_state->__pyx_tuple__72);
+  Py_CLEAR(clear_module_state->__pyx_tuple__74);
+  Py_CLEAR(clear_module_state->__pyx_tuple__77);
+  Py_CLEAR(clear_module_state->__pyx_tuple__79);
+  Py_CLEAR(clear_module_state->__pyx_tuple__86);
+  Py_CLEAR(clear_module_state->__pyx_tuple__89);
+  Py_CLEAR(clear_module_state->__pyx_tuple__91);
+  Py_CLEAR(clear_module_state->__pyx_tuple__93);
+  Py_CLEAR(clear_module_state->__pyx_tuple__100);
+  Py_CLEAR(clear_module_state->__pyx_tuple__102);
+  Py_CLEAR(clear_module_state->__pyx_tuple__104);
+  Py_CLEAR(clear_module_state->__pyx_tuple__109);
+  Py_CLEAR(clear_module_state->__pyx_tuple__113);
+  Py_CLEAR(clear_module_state->__pyx_tuple__115);
+  Py_CLEAR(clear_module_state->__pyx_tuple__118);
+  Py_CLEAR(clear_module_state->__pyx_tuple__123);
+  Py_CLEAR(clear_module_state->__pyx_tuple__125);
+  Py_CLEAR(clear_module_state->__pyx_tuple__132);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
   Py_CLEAR(clear_module_state->__pyx_codeobj__26);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__28);
   Py_CLEAR(clear_module_state->__pyx_codeobj__29);
   Py_CLEAR(clear_module_state->__pyx_codeobj__30);
   Py_CLEAR(clear_module_state->__pyx_codeobj__31);
   Py_CLEAR(clear_module_state->__pyx_codeobj__32);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__33);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__35);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__37);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__39);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__41);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__43);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__45);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__47);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__34);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__36);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__38);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__40);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__42);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__44);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__46);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__49);
   Py_CLEAR(clear_module_state->__pyx_codeobj__50);
   Py_CLEAR(clear_module_state->__pyx_codeobj__51);
   Py_CLEAR(clear_module_state->__pyx_codeobj__52);
   Py_CLEAR(clear_module_state->__pyx_codeobj__53);
   Py_CLEAR(clear_module_state->__pyx_codeobj__54);
   Py_CLEAR(clear_module_state->__pyx_codeobj__55);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__56);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__57);
   Py_CLEAR(clear_module_state->__pyx_codeobj__58);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__59);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__60);
   Py_CLEAR(clear_module_state->__pyx_codeobj__61);
   Py_CLEAR(clear_module_state->__pyx_codeobj__62);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__63);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__64);
   Py_CLEAR(clear_module_state->__pyx_codeobj__65);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__66);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__68);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__70);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__72);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__74);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__67);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__69);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__71);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__73);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__75);
   Py_CLEAR(clear_module_state->__pyx_codeobj__76);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__77);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__79);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__78);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__80);
   Py_CLEAR(clear_module_state->__pyx_codeobj__81);
   Py_CLEAR(clear_module_state->__pyx_codeobj__82);
   Py_CLEAR(clear_module_state->__pyx_codeobj__83);
   Py_CLEAR(clear_module_state->__pyx_codeobj__84);
   Py_CLEAR(clear_module_state->__pyx_codeobj__85);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__86);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__87);
   Py_CLEAR(clear_module_state->__pyx_codeobj__88);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__89);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__91);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__93);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__90);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__92);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__94);
   Py_CLEAR(clear_module_state->__pyx_codeobj__95);
   Py_CLEAR(clear_module_state->__pyx_codeobj__96);
   Py_CLEAR(clear_module_state->__pyx_codeobj__97);
   Py_CLEAR(clear_module_state->__pyx_codeobj__98);
   Py_CLEAR(clear_module_state->__pyx_codeobj__99);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__100);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__102);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__104);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__101);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__103);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__105);
   Py_CLEAR(clear_module_state->__pyx_codeobj__106);
   Py_CLEAR(clear_module_state->__pyx_codeobj__107);
   Py_CLEAR(clear_module_state->__pyx_codeobj__108);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__109);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__110);
   Py_CLEAR(clear_module_state->__pyx_codeobj__111);
   Py_CLEAR(clear_module_state->__pyx_codeobj__112);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__113);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__115);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__114);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__116);
   Py_CLEAR(clear_module_state->__pyx_codeobj__117);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__118);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__119);
   Py_CLEAR(clear_module_state->__pyx_codeobj__120);
   Py_CLEAR(clear_module_state->__pyx_codeobj__121);
   Py_CLEAR(clear_module_state->__pyx_codeobj__122);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__123);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__125);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__124);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__126);
   Py_CLEAR(clear_module_state->__pyx_codeobj__127);
   Py_CLEAR(clear_module_state->__pyx_codeobj__128);
   Py_CLEAR(clear_module_state->__pyx_codeobj__129);
   Py_CLEAR(clear_module_state->__pyx_codeobj__130);
   Py_CLEAR(clear_module_state->__pyx_codeobj__131);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__132);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__134);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__133);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -4774,23 +4783,23 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Trace);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Tuple_int_memoryview);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ViewBuffer);
   Py_VISIT(traverse_module_state->__pyx_n_s_ViewBuffer___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_ViewBuffer___setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_kp_b__12);
-  Py_VISIT(traverse_module_state->__pyx_n_s__135);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__14);
+  Py_VISIT(traverse_module_state->__pyx_kp_b__11);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__13);
+  Py_VISIT(traverse_module_state->__pyx_n_s__134);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__16);
   Py_VISIT(traverse_module_state->__pyx_kp_u__17);
   Py_VISIT(traverse_module_state->__pyx_kp_u__18);
   Py_VISIT(traverse_module_state->__pyx_kp_u__19);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__20);
-  Py_VISIT(traverse_module_state->__pyx_n_s__22);
+  Py_VISIT(traverse_module_state->__pyx_n_s__21);
   Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_kp_u__4);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithm);
   Py_VISIT(traverse_module_state->__pyx_n_u_ascii);
   Py_VISIT(traverse_module_state->__pyx_n_s_async);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_kp_u_at_0x);
@@ -4830,15 +4839,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_connect_start);
   Py_VISIT(traverse_module_state->__pyx_kp_u_connection_not_in_pipeline_mode);
   Py_VISIT(traverse_module_state->__pyx_n_s_connection_summary);
   Py_VISIT(traverse_module_state->__pyx_n_s_conninfo);
   Py_VISIT(traverse_module_state->__pyx_n_s_consume_input);
   Py_VISIT(traverse_module_state->__pyx_kp_u_consuming_input_failed);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_PGconn);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_PGresult);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_connection_def);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_connection_inf);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_empty_PGresult);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_for_escape_byt);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_for_unescape_b);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_allocate_on_conninfo_pa);
   Py_VISIT(traverse_module_state->__pyx_kp_u_couldn_t_create_cancel_object);
@@ -4849,14 +4857,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_cvalues);
   Py_VISIT(traverse_module_state->__pyx_n_u_d);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_descr);
   Py_VISIT(traverse_module_state->__pyx_n_s_describe_portal);
   Py_VISIT(traverse_module_state->__pyx_n_s_describe_prepared);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_describe_prepared_failed);
   Py_VISIT(traverse_module_state->__pyx_n_s_descriptions);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_s_dispchar);
   Py_VISIT(traverse_module_state->__pyx_n_s_dispsize);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
@@ -4882,14 +4891,16 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_escape_string_failed);
   Py_VISIT(traverse_module_state->__pyx_n_s_exc);
   Py_VISIT(traverse_module_state->__pyx_n_s_exception);
   Py_VISIT(traverse_module_state->__pyx_n_s_exec);
   Py_VISIT(traverse_module_state->__pyx_n_s_exec_params);
   Py_VISIT(traverse_module_state->__pyx_n_s_exec_prepared);
   Py_VISIT(traverse_module_state->__pyx_n_s_exec_status);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_executing_prepared_query_failed);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_executing_query_failed);
   Py_VISIT(traverse_module_state->__pyx_n_s_exit_pipeline_mode);
   Py_VISIT(traverse_module_state->__pyx_kp_u_failed_to_enter_pipeline_mode);
   Py_VISIT(traverse_module_state->__pyx_kp_u_failed_to_sync_pipeline);
   Py_VISIT(traverse_module_state->__pyx_n_s_fformat);
   Py_VISIT(traverse_module_state->__pyx_n_s_fieldcode);
   Py_VISIT(traverse_module_state->__pyx_n_s_fileno);
   Py_VISIT(traverse_module_state->__pyx_n_s_finish);
@@ -4961,14 +4972,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_pgresult);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_ping);
   Py_VISIT(traverse_module_state->__pyx_n_s_pipeline_sync);
   Py_VISIT(traverse_module_state->__pyx_n_s_platform);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare_2);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_preparing_query_failed);
   Py_VISIT(traverse_module_state->__pyx_n_s_psycopg);
   Py_VISIT(traverse_module_state->__pyx_n_u_psycopg);
   Py_VISIT(traverse_module_state->__pyx_n_s_psycopg_c_pq);
   Py_VISIT(traverse_module_state->__pyx_kp_s_psycopg_c_pq_conninfo_pyx);
   Py_VISIT(traverse_module_state->__pyx_kp_s_psycopg_c_pq_escaping_pyx);
   Py_VISIT(traverse_module_state->__pyx_kp_s_psycopg_c_pq_pgcancel_pyx);
   Py_VISIT(traverse_module_state->__pyx_kp_s_psycopg_c_pq_pgconn_pyx);
@@ -5047,137 +5059,136 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_v);
   Py_VISIT(traverse_module_state->__pyx_n_s_val);
   Py_VISIT(traverse_module_state->__pyx_n_s_version);
   Py_VISIT(traverse_module_state->__pyx_n_u_x);
   Py_VISIT(traverse_module_state->__pyx_int_8405287);
   Py_VISIT(traverse_module_state->__pyx_int_12701922);
   Py_VISIT(traverse_module_state->__pyx_int_59804213);
+  Py_VISIT(traverse_module_state->__pyx_k__7);
   Py_VISIT(traverse_module_state->__pyx_k__8);
   Py_VISIT(traverse_module_state->__pyx_k__9);
   Py_VISIT(traverse_module_state->__pyx_k__10);
-  Py_VISIT(traverse_module_state->__pyx_k__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
-  Py_VISIT(traverse_module_state->__pyx_tuple__7);
-  Py_VISIT(traverse_module_state->__pyx_tuple__13);
+  Py_VISIT(traverse_module_state->__pyx_tuple__12);
+  Py_VISIT(traverse_module_state->__pyx_tuple__14);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
-  Py_VISIT(traverse_module_state->__pyx_tuple__16);
-  Py_VISIT(traverse_module_state->__pyx_tuple__21);
-  Py_VISIT(traverse_module_state->__pyx_tuple__23);
-  Py_VISIT(traverse_module_state->__pyx_tuple__25);
-  Py_VISIT(traverse_module_state->__pyx_tuple__28);
-  Py_VISIT(traverse_module_state->__pyx_tuple__34);
-  Py_VISIT(traverse_module_state->__pyx_tuple__36);
-  Py_VISIT(traverse_module_state->__pyx_tuple__38);
-  Py_VISIT(traverse_module_state->__pyx_tuple__40);
-  Py_VISIT(traverse_module_state->__pyx_tuple__42);
-  Py_VISIT(traverse_module_state->__pyx_tuple__44);
-  Py_VISIT(traverse_module_state->__pyx_tuple__46);
+  Py_VISIT(traverse_module_state->__pyx_tuple__20);
+  Py_VISIT(traverse_module_state->__pyx_tuple__22);
+  Py_VISIT(traverse_module_state->__pyx_tuple__24);
+  Py_VISIT(traverse_module_state->__pyx_tuple__27);
+  Py_VISIT(traverse_module_state->__pyx_tuple__33);
+  Py_VISIT(traverse_module_state->__pyx_tuple__35);
+  Py_VISIT(traverse_module_state->__pyx_tuple__37);
+  Py_VISIT(traverse_module_state->__pyx_tuple__39);
+  Py_VISIT(traverse_module_state->__pyx_tuple__41);
+  Py_VISIT(traverse_module_state->__pyx_tuple__43);
+  Py_VISIT(traverse_module_state->__pyx_tuple__45);
+  Py_VISIT(traverse_module_state->__pyx_tuple__47);
   Py_VISIT(traverse_module_state->__pyx_tuple__48);
-  Py_VISIT(traverse_module_state->__pyx_tuple__49);
-  Py_VISIT(traverse_module_state->__pyx_tuple__57);
-  Py_VISIT(traverse_module_state->__pyx_tuple__60);
-  Py_VISIT(traverse_module_state->__pyx_tuple__64);
-  Py_VISIT(traverse_module_state->__pyx_tuple__67);
-  Py_VISIT(traverse_module_state->__pyx_tuple__69);
-  Py_VISIT(traverse_module_state->__pyx_tuple__71);
-  Py_VISIT(traverse_module_state->__pyx_tuple__73);
-  Py_VISIT(traverse_module_state->__pyx_tuple__75);
-  Py_VISIT(traverse_module_state->__pyx_tuple__78);
-  Py_VISIT(traverse_module_state->__pyx_tuple__80);
-  Py_VISIT(traverse_module_state->__pyx_tuple__87);
-  Py_VISIT(traverse_module_state->__pyx_tuple__90);
-  Py_VISIT(traverse_module_state->__pyx_tuple__92);
-  Py_VISIT(traverse_module_state->__pyx_tuple__94);
-  Py_VISIT(traverse_module_state->__pyx_tuple__101);
-  Py_VISIT(traverse_module_state->__pyx_tuple__103);
-  Py_VISIT(traverse_module_state->__pyx_tuple__105);
-  Py_VISIT(traverse_module_state->__pyx_tuple__110);
-  Py_VISIT(traverse_module_state->__pyx_tuple__114);
-  Py_VISIT(traverse_module_state->__pyx_tuple__116);
-  Py_VISIT(traverse_module_state->__pyx_tuple__119);
-  Py_VISIT(traverse_module_state->__pyx_tuple__124);
-  Py_VISIT(traverse_module_state->__pyx_tuple__126);
-  Py_VISIT(traverse_module_state->__pyx_tuple__133);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_tuple__56);
+  Py_VISIT(traverse_module_state->__pyx_tuple__59);
+  Py_VISIT(traverse_module_state->__pyx_tuple__63);
+  Py_VISIT(traverse_module_state->__pyx_tuple__66);
+  Py_VISIT(traverse_module_state->__pyx_tuple__68);
+  Py_VISIT(traverse_module_state->__pyx_tuple__70);
+  Py_VISIT(traverse_module_state->__pyx_tuple__72);
+  Py_VISIT(traverse_module_state->__pyx_tuple__74);
+  Py_VISIT(traverse_module_state->__pyx_tuple__77);
+  Py_VISIT(traverse_module_state->__pyx_tuple__79);
+  Py_VISIT(traverse_module_state->__pyx_tuple__86);
+  Py_VISIT(traverse_module_state->__pyx_tuple__89);
+  Py_VISIT(traverse_module_state->__pyx_tuple__91);
+  Py_VISIT(traverse_module_state->__pyx_tuple__93);
+  Py_VISIT(traverse_module_state->__pyx_tuple__100);
+  Py_VISIT(traverse_module_state->__pyx_tuple__102);
+  Py_VISIT(traverse_module_state->__pyx_tuple__104);
+  Py_VISIT(traverse_module_state->__pyx_tuple__109);
+  Py_VISIT(traverse_module_state->__pyx_tuple__113);
+  Py_VISIT(traverse_module_state->__pyx_tuple__115);
+  Py_VISIT(traverse_module_state->__pyx_tuple__118);
+  Py_VISIT(traverse_module_state->__pyx_tuple__123);
+  Py_VISIT(traverse_module_state->__pyx_tuple__125);
+  Py_VISIT(traverse_module_state->__pyx_tuple__132);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
   Py_VISIT(traverse_module_state->__pyx_codeobj__26);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__28);
   Py_VISIT(traverse_module_state->__pyx_codeobj__29);
   Py_VISIT(traverse_module_state->__pyx_codeobj__30);
   Py_VISIT(traverse_module_state->__pyx_codeobj__31);
   Py_VISIT(traverse_module_state->__pyx_codeobj__32);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__33);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__35);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__37);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__39);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__41);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__43);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__45);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__47);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__34);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__36);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__38);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__40);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__42);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__44);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__46);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__49);
   Py_VISIT(traverse_module_state->__pyx_codeobj__50);
   Py_VISIT(traverse_module_state->__pyx_codeobj__51);
   Py_VISIT(traverse_module_state->__pyx_codeobj__52);
   Py_VISIT(traverse_module_state->__pyx_codeobj__53);
   Py_VISIT(traverse_module_state->__pyx_codeobj__54);
   Py_VISIT(traverse_module_state->__pyx_codeobj__55);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__56);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__57);
   Py_VISIT(traverse_module_state->__pyx_codeobj__58);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__59);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__60);
   Py_VISIT(traverse_module_state->__pyx_codeobj__61);
   Py_VISIT(traverse_module_state->__pyx_codeobj__62);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__63);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__64);
   Py_VISIT(traverse_module_state->__pyx_codeobj__65);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__66);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__68);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__70);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__72);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__74);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__67);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__69);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__71);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__73);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__75);
   Py_VISIT(traverse_module_state->__pyx_codeobj__76);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__77);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__79);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__78);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__80);
   Py_VISIT(traverse_module_state->__pyx_codeobj__81);
   Py_VISIT(traverse_module_state->__pyx_codeobj__82);
   Py_VISIT(traverse_module_state->__pyx_codeobj__83);
   Py_VISIT(traverse_module_state->__pyx_codeobj__84);
   Py_VISIT(traverse_module_state->__pyx_codeobj__85);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__86);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__87);
   Py_VISIT(traverse_module_state->__pyx_codeobj__88);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__89);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__91);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__93);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__90);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__92);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__94);
   Py_VISIT(traverse_module_state->__pyx_codeobj__95);
   Py_VISIT(traverse_module_state->__pyx_codeobj__96);
   Py_VISIT(traverse_module_state->__pyx_codeobj__97);
   Py_VISIT(traverse_module_state->__pyx_codeobj__98);
   Py_VISIT(traverse_module_state->__pyx_codeobj__99);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__100);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__102);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__104);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__101);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__103);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__105);
   Py_VISIT(traverse_module_state->__pyx_codeobj__106);
   Py_VISIT(traverse_module_state->__pyx_codeobj__107);
   Py_VISIT(traverse_module_state->__pyx_codeobj__108);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__109);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__110);
   Py_VISIT(traverse_module_state->__pyx_codeobj__111);
   Py_VISIT(traverse_module_state->__pyx_codeobj__112);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__113);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__115);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__114);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__116);
   Py_VISIT(traverse_module_state->__pyx_codeobj__117);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__118);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__119);
   Py_VISIT(traverse_module_state->__pyx_codeobj__120);
   Py_VISIT(traverse_module_state->__pyx_codeobj__121);
   Py_VISIT(traverse_module_state->__pyx_codeobj__122);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__123);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__125);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__124);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__126);
   Py_VISIT(traverse_module_state->__pyx_codeobj__127);
   Py_VISIT(traverse_module_state->__pyx_codeobj__128);
   Py_VISIT(traverse_module_state->__pyx_codeobj__129);
   Py_VISIT(traverse_module_state->__pyx_codeobj__130);
   Py_VISIT(traverse_module_state->__pyx_codeobj__131);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__132);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__134);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__133);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
@@ -5315,23 +5326,23 @@
 #define __pyx_n_s_Trace __pyx_mstate_global->__pyx_n_s_Trace
 #define __pyx_kp_s_Tuple_int_memoryview __pyx_mstate_global->__pyx_kp_s_Tuple_int_memoryview
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_ViewBuffer __pyx_mstate_global->__pyx_n_s_ViewBuffer
 #define __pyx_n_s_ViewBuffer___reduce_cython __pyx_mstate_global->__pyx_n_s_ViewBuffer___reduce_cython
 #define __pyx_n_s_ViewBuffer___setstate_cython __pyx_mstate_global->__pyx_n_s_ViewBuffer___setstate_cython
-#define __pyx_kp_b__12 __pyx_mstate_global->__pyx_kp_b__12
-#define __pyx_n_s__135 __pyx_mstate_global->__pyx_n_s__135
-#define __pyx_kp_u__14 __pyx_mstate_global->__pyx_kp_u__14
+#define __pyx_kp_b__11 __pyx_mstate_global->__pyx_kp_b__11
+#define __pyx_kp_u__13 __pyx_mstate_global->__pyx_kp_u__13
+#define __pyx_n_s__134 __pyx_mstate_global->__pyx_n_s__134
+#define __pyx_kp_u__16 __pyx_mstate_global->__pyx_kp_u__16
 #define __pyx_kp_u__17 __pyx_mstate_global->__pyx_kp_u__17
 #define __pyx_kp_u__18 __pyx_mstate_global->__pyx_kp_u__18
 #define __pyx_kp_u__19 __pyx_mstate_global->__pyx_kp_u__19
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_kp_u__20 __pyx_mstate_global->__pyx_kp_u__20
-#define __pyx_n_s__22 __pyx_mstate_global->__pyx_n_s__22
+#define __pyx_n_s__21 __pyx_mstate_global->__pyx_n_s__21
 #define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
 #define __pyx_n_s_algorithm __pyx_mstate_global->__pyx_n_s_algorithm
 #define __pyx_n_u_ascii __pyx_mstate_global->__pyx_n_u_ascii
 #define __pyx_n_s_async __pyx_mstate_global->__pyx_n_s_async
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_kp_u_at_0x __pyx_mstate_global->__pyx_kp_u_at_0x
@@ -5371,15 +5382,14 @@
 #define __pyx_n_s_connect_start __pyx_mstate_global->__pyx_n_s_connect_start
 #define __pyx_kp_u_connection_not_in_pipeline_mode __pyx_mstate_global->__pyx_kp_u_connection_not_in_pipeline_mode
 #define __pyx_n_s_connection_summary __pyx_mstate_global->__pyx_n_s_connection_summary
 #define __pyx_n_s_conninfo __pyx_mstate_global->__pyx_n_s_conninfo
 #define __pyx_n_s_consume_input __pyx_mstate_global->__pyx_n_s_consume_input
 #define __pyx_kp_u_consuming_input_failed __pyx_mstate_global->__pyx_kp_u_consuming_input_failed
 #define __pyx_kp_u_couldn_t_allocate_PGconn __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_PGconn
-#define __pyx_kp_u_couldn_t_allocate_PGresult __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_PGresult
 #define __pyx_kp_u_couldn_t_allocate_connection_def __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_connection_def
 #define __pyx_kp_u_couldn_t_allocate_connection_inf __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_connection_inf
 #define __pyx_kp_u_couldn_t_allocate_empty_PGresult __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_empty_PGresult
 #define __pyx_kp_u_couldn_t_allocate_for_escape_byt __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_for_escape_byt
 #define __pyx_kp_u_couldn_t_allocate_for_unescape_b __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_for_unescape_b
 #define __pyx_kp_u_couldn_t_allocate_on_conninfo_pa __pyx_mstate_global->__pyx_kp_u_couldn_t_allocate_on_conninfo_pa
 #define __pyx_kp_u_couldn_t_create_cancel_object __pyx_mstate_global->__pyx_kp_u_couldn_t_create_cancel_object
@@ -5390,14 +5400,15 @@
 #define __pyx_n_s_cvalues __pyx_mstate_global->__pyx_n_s_cvalues
 #define __pyx_n_u_d __pyx_mstate_global->__pyx_n_u_d
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_decode __pyx_mstate_global->__pyx_n_s_decode
 #define __pyx_n_s_descr __pyx_mstate_global->__pyx_n_s_descr
 #define __pyx_n_s_describe_portal __pyx_mstate_global->__pyx_n_s_describe_portal
 #define __pyx_n_s_describe_prepared __pyx_mstate_global->__pyx_n_s_describe_prepared
+#define __pyx_kp_u_describe_prepared_failed __pyx_mstate_global->__pyx_kp_u_describe_prepared_failed
 #define __pyx_n_s_descriptions __pyx_mstate_global->__pyx_n_s_descriptions
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_s_dispchar __pyx_mstate_global->__pyx_n_s_dispchar
 #define __pyx_n_s_dispsize __pyx_mstate_global->__pyx_n_s_dispsize
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
@@ -5423,14 +5434,16 @@
 #define __pyx_kp_u_escape_string_failed __pyx_mstate_global->__pyx_kp_u_escape_string_failed
 #define __pyx_n_s_exc __pyx_mstate_global->__pyx_n_s_exc
 #define __pyx_n_s_exception __pyx_mstate_global->__pyx_n_s_exception
 #define __pyx_n_s_exec __pyx_mstate_global->__pyx_n_s_exec
 #define __pyx_n_s_exec_params __pyx_mstate_global->__pyx_n_s_exec_params
 #define __pyx_n_s_exec_prepared __pyx_mstate_global->__pyx_n_s_exec_prepared
 #define __pyx_n_s_exec_status __pyx_mstate_global->__pyx_n_s_exec_status
+#define __pyx_kp_u_executing_prepared_query_failed __pyx_mstate_global->__pyx_kp_u_executing_prepared_query_failed
+#define __pyx_kp_u_executing_query_failed __pyx_mstate_global->__pyx_kp_u_executing_query_failed
 #define __pyx_n_s_exit_pipeline_mode __pyx_mstate_global->__pyx_n_s_exit_pipeline_mode
 #define __pyx_kp_u_failed_to_enter_pipeline_mode __pyx_mstate_global->__pyx_kp_u_failed_to_enter_pipeline_mode
 #define __pyx_kp_u_failed_to_sync_pipeline __pyx_mstate_global->__pyx_kp_u_failed_to_sync_pipeline
 #define __pyx_n_s_fformat __pyx_mstate_global->__pyx_n_s_fformat
 #define __pyx_n_s_fieldcode __pyx_mstate_global->__pyx_n_s_fieldcode
 #define __pyx_n_s_fileno __pyx_mstate_global->__pyx_n_s_fileno
 #define __pyx_n_s_finish __pyx_mstate_global->__pyx_n_s_finish
@@ -5502,14 +5515,15 @@
 #define __pyx_n_s_pgresult __pyx_mstate_global->__pyx_n_s_pgresult
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_ping __pyx_mstate_global->__pyx_n_s_ping
 #define __pyx_n_s_pipeline_sync __pyx_mstate_global->__pyx_n_s_pipeline_sync
 #define __pyx_n_s_platform __pyx_mstate_global->__pyx_n_s_platform
 #define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
 #define __pyx_n_s_prepare_2 __pyx_mstate_global->__pyx_n_s_prepare_2
+#define __pyx_kp_u_preparing_query_failed __pyx_mstate_global->__pyx_kp_u_preparing_query_failed
 #define __pyx_n_s_psycopg __pyx_mstate_global->__pyx_n_s_psycopg
 #define __pyx_n_u_psycopg __pyx_mstate_global->__pyx_n_u_psycopg
 #define __pyx_n_s_psycopg_c_pq __pyx_mstate_global->__pyx_n_s_psycopg_c_pq
 #define __pyx_kp_s_psycopg_c_pq_conninfo_pyx __pyx_mstate_global->__pyx_kp_s_psycopg_c_pq_conninfo_pyx
 #define __pyx_kp_s_psycopg_c_pq_escaping_pyx __pyx_mstate_global->__pyx_kp_s_psycopg_c_pq_escaping_pyx
 #define __pyx_kp_s_psycopg_c_pq_pgcancel_pyx __pyx_mstate_global->__pyx_kp_s_psycopg_c_pq_pgcancel_pyx
 #define __pyx_kp_s_psycopg_c_pq_pgconn_pyx __pyx_mstate_global->__pyx_kp_s_psycopg_c_pq_pgconn_pyx
@@ -5588,137 +5602,136 @@
 #define __pyx_n_s_v __pyx_mstate_global->__pyx_n_s_v
 #define __pyx_n_s_val __pyx_mstate_global->__pyx_n_s_val
 #define __pyx_n_s_version __pyx_mstate_global->__pyx_n_s_version
 #define __pyx_n_u_x __pyx_mstate_global->__pyx_n_u_x
 #define __pyx_int_8405287 __pyx_mstate_global->__pyx_int_8405287
 #define __pyx_int_12701922 __pyx_mstate_global->__pyx_int_12701922
 #define __pyx_int_59804213 __pyx_mstate_global->__pyx_int_59804213
+#define __pyx_k__7 __pyx_mstate_global->__pyx_k__7
 #define __pyx_k__8 __pyx_mstate_global->__pyx_k__8
 #define __pyx_k__9 __pyx_mstate_global->__pyx_k__9
 #define __pyx_k__10 __pyx_mstate_global->__pyx_k__10
-#define __pyx_k__11 __pyx_mstate_global->__pyx_k__11
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
-#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
-#define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
+#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
+#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
-#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
-#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
-#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
-#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
-#define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
-#define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
-#define __pyx_tuple__36 __pyx_mstate_global->__pyx_tuple__36
-#define __pyx_tuple__38 __pyx_mstate_global->__pyx_tuple__38
-#define __pyx_tuple__40 __pyx_mstate_global->__pyx_tuple__40
-#define __pyx_tuple__42 __pyx_mstate_global->__pyx_tuple__42
-#define __pyx_tuple__44 __pyx_mstate_global->__pyx_tuple__44
-#define __pyx_tuple__46 __pyx_mstate_global->__pyx_tuple__46
+#define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
+#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
+#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
+#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
+#define __pyx_tuple__33 __pyx_mstate_global->__pyx_tuple__33
+#define __pyx_tuple__35 __pyx_mstate_global->__pyx_tuple__35
+#define __pyx_tuple__37 __pyx_mstate_global->__pyx_tuple__37
+#define __pyx_tuple__39 __pyx_mstate_global->__pyx_tuple__39
+#define __pyx_tuple__41 __pyx_mstate_global->__pyx_tuple__41
+#define __pyx_tuple__43 __pyx_mstate_global->__pyx_tuple__43
+#define __pyx_tuple__45 __pyx_mstate_global->__pyx_tuple__45
+#define __pyx_tuple__47 __pyx_mstate_global->__pyx_tuple__47
 #define __pyx_tuple__48 __pyx_mstate_global->__pyx_tuple__48
-#define __pyx_tuple__49 __pyx_mstate_global->__pyx_tuple__49
-#define __pyx_tuple__57 __pyx_mstate_global->__pyx_tuple__57
-#define __pyx_tuple__60 __pyx_mstate_global->__pyx_tuple__60
-#define __pyx_tuple__64 __pyx_mstate_global->__pyx_tuple__64
-#define __pyx_tuple__67 __pyx_mstate_global->__pyx_tuple__67
-#define __pyx_tuple__69 __pyx_mstate_global->__pyx_tuple__69
-#define __pyx_tuple__71 __pyx_mstate_global->__pyx_tuple__71
-#define __pyx_tuple__73 __pyx_mstate_global->__pyx_tuple__73
-#define __pyx_tuple__75 __pyx_mstate_global->__pyx_tuple__75
-#define __pyx_tuple__78 __pyx_mstate_global->__pyx_tuple__78
-#define __pyx_tuple__80 __pyx_mstate_global->__pyx_tuple__80
-#define __pyx_tuple__87 __pyx_mstate_global->__pyx_tuple__87
-#define __pyx_tuple__90 __pyx_mstate_global->__pyx_tuple__90
-#define __pyx_tuple__92 __pyx_mstate_global->__pyx_tuple__92
-#define __pyx_tuple__94 __pyx_mstate_global->__pyx_tuple__94
-#define __pyx_tuple__101 __pyx_mstate_global->__pyx_tuple__101
-#define __pyx_tuple__103 __pyx_mstate_global->__pyx_tuple__103
-#define __pyx_tuple__105 __pyx_mstate_global->__pyx_tuple__105
-#define __pyx_tuple__110 __pyx_mstate_global->__pyx_tuple__110
-#define __pyx_tuple__114 __pyx_mstate_global->__pyx_tuple__114
-#define __pyx_tuple__116 __pyx_mstate_global->__pyx_tuple__116
-#define __pyx_tuple__119 __pyx_mstate_global->__pyx_tuple__119
-#define __pyx_tuple__124 __pyx_mstate_global->__pyx_tuple__124
-#define __pyx_tuple__126 __pyx_mstate_global->__pyx_tuple__126
-#define __pyx_tuple__133 __pyx_mstate_global->__pyx_tuple__133
-#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_tuple__56 __pyx_mstate_global->__pyx_tuple__56
+#define __pyx_tuple__59 __pyx_mstate_global->__pyx_tuple__59
+#define __pyx_tuple__63 __pyx_mstate_global->__pyx_tuple__63
+#define __pyx_tuple__66 __pyx_mstate_global->__pyx_tuple__66
+#define __pyx_tuple__68 __pyx_mstate_global->__pyx_tuple__68
+#define __pyx_tuple__70 __pyx_mstate_global->__pyx_tuple__70
+#define __pyx_tuple__72 __pyx_mstate_global->__pyx_tuple__72
+#define __pyx_tuple__74 __pyx_mstate_global->__pyx_tuple__74
+#define __pyx_tuple__77 __pyx_mstate_global->__pyx_tuple__77
+#define __pyx_tuple__79 __pyx_mstate_global->__pyx_tuple__79
+#define __pyx_tuple__86 __pyx_mstate_global->__pyx_tuple__86
+#define __pyx_tuple__89 __pyx_mstate_global->__pyx_tuple__89
+#define __pyx_tuple__91 __pyx_mstate_global->__pyx_tuple__91
+#define __pyx_tuple__93 __pyx_mstate_global->__pyx_tuple__93
+#define __pyx_tuple__100 __pyx_mstate_global->__pyx_tuple__100
+#define __pyx_tuple__102 __pyx_mstate_global->__pyx_tuple__102
+#define __pyx_tuple__104 __pyx_mstate_global->__pyx_tuple__104
+#define __pyx_tuple__109 __pyx_mstate_global->__pyx_tuple__109
+#define __pyx_tuple__113 __pyx_mstate_global->__pyx_tuple__113
+#define __pyx_tuple__115 __pyx_mstate_global->__pyx_tuple__115
+#define __pyx_tuple__118 __pyx_mstate_global->__pyx_tuple__118
+#define __pyx_tuple__123 __pyx_mstate_global->__pyx_tuple__123
+#define __pyx_tuple__125 __pyx_mstate_global->__pyx_tuple__125
+#define __pyx_tuple__132 __pyx_mstate_global->__pyx_tuple__132
+#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
+#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
-#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
+#define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
 #define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
 #define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
-#define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
-#define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
-#define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
-#define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
-#define __pyx_codeobj__41 __pyx_mstate_global->__pyx_codeobj__41
-#define __pyx_codeobj__43 __pyx_mstate_global->__pyx_codeobj__43
-#define __pyx_codeobj__45 __pyx_mstate_global->__pyx_codeobj__45
-#define __pyx_codeobj__47 __pyx_mstate_global->__pyx_codeobj__47
+#define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
+#define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
+#define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
+#define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
+#define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
+#define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
+#define __pyx_codeobj__46 __pyx_mstate_global->__pyx_codeobj__46
+#define __pyx_codeobj__49 __pyx_mstate_global->__pyx_codeobj__49
 #define __pyx_codeobj__50 __pyx_mstate_global->__pyx_codeobj__50
 #define __pyx_codeobj__51 __pyx_mstate_global->__pyx_codeobj__51
 #define __pyx_codeobj__52 __pyx_mstate_global->__pyx_codeobj__52
 #define __pyx_codeobj__53 __pyx_mstate_global->__pyx_codeobj__53
 #define __pyx_codeobj__54 __pyx_mstate_global->__pyx_codeobj__54
 #define __pyx_codeobj__55 __pyx_mstate_global->__pyx_codeobj__55
-#define __pyx_codeobj__56 __pyx_mstate_global->__pyx_codeobj__56
+#define __pyx_codeobj__57 __pyx_mstate_global->__pyx_codeobj__57
 #define __pyx_codeobj__58 __pyx_mstate_global->__pyx_codeobj__58
-#define __pyx_codeobj__59 __pyx_mstate_global->__pyx_codeobj__59
+#define __pyx_codeobj__60 __pyx_mstate_global->__pyx_codeobj__60
 #define __pyx_codeobj__61 __pyx_mstate_global->__pyx_codeobj__61
 #define __pyx_codeobj__62 __pyx_mstate_global->__pyx_codeobj__62
-#define __pyx_codeobj__63 __pyx_mstate_global->__pyx_codeobj__63
+#define __pyx_codeobj__64 __pyx_mstate_global->__pyx_codeobj__64
 #define __pyx_codeobj__65 __pyx_mstate_global->__pyx_codeobj__65
-#define __pyx_codeobj__66 __pyx_mstate_global->__pyx_codeobj__66
-#define __pyx_codeobj__68 __pyx_mstate_global->__pyx_codeobj__68
-#define __pyx_codeobj__70 __pyx_mstate_global->__pyx_codeobj__70
-#define __pyx_codeobj__72 __pyx_mstate_global->__pyx_codeobj__72
-#define __pyx_codeobj__74 __pyx_mstate_global->__pyx_codeobj__74
+#define __pyx_codeobj__67 __pyx_mstate_global->__pyx_codeobj__67
+#define __pyx_codeobj__69 __pyx_mstate_global->__pyx_codeobj__69
+#define __pyx_codeobj__71 __pyx_mstate_global->__pyx_codeobj__71
+#define __pyx_codeobj__73 __pyx_mstate_global->__pyx_codeobj__73
+#define __pyx_codeobj__75 __pyx_mstate_global->__pyx_codeobj__75
 #define __pyx_codeobj__76 __pyx_mstate_global->__pyx_codeobj__76
-#define __pyx_codeobj__77 __pyx_mstate_global->__pyx_codeobj__77
-#define __pyx_codeobj__79 __pyx_mstate_global->__pyx_codeobj__79
+#define __pyx_codeobj__78 __pyx_mstate_global->__pyx_codeobj__78
+#define __pyx_codeobj__80 __pyx_mstate_global->__pyx_codeobj__80
 #define __pyx_codeobj__81 __pyx_mstate_global->__pyx_codeobj__81
 #define __pyx_codeobj__82 __pyx_mstate_global->__pyx_codeobj__82
 #define __pyx_codeobj__83 __pyx_mstate_global->__pyx_codeobj__83
 #define __pyx_codeobj__84 __pyx_mstate_global->__pyx_codeobj__84
 #define __pyx_codeobj__85 __pyx_mstate_global->__pyx_codeobj__85
-#define __pyx_codeobj__86 __pyx_mstate_global->__pyx_codeobj__86
+#define __pyx_codeobj__87 __pyx_mstate_global->__pyx_codeobj__87
 #define __pyx_codeobj__88 __pyx_mstate_global->__pyx_codeobj__88
-#define __pyx_codeobj__89 __pyx_mstate_global->__pyx_codeobj__89
-#define __pyx_codeobj__91 __pyx_mstate_global->__pyx_codeobj__91
-#define __pyx_codeobj__93 __pyx_mstate_global->__pyx_codeobj__93
+#define __pyx_codeobj__90 __pyx_mstate_global->__pyx_codeobj__90
+#define __pyx_codeobj__92 __pyx_mstate_global->__pyx_codeobj__92
+#define __pyx_codeobj__94 __pyx_mstate_global->__pyx_codeobj__94
 #define __pyx_codeobj__95 __pyx_mstate_global->__pyx_codeobj__95
 #define __pyx_codeobj__96 __pyx_mstate_global->__pyx_codeobj__96
 #define __pyx_codeobj__97 __pyx_mstate_global->__pyx_codeobj__97
 #define __pyx_codeobj__98 __pyx_mstate_global->__pyx_codeobj__98
 #define __pyx_codeobj__99 __pyx_mstate_global->__pyx_codeobj__99
-#define __pyx_codeobj__100 __pyx_mstate_global->__pyx_codeobj__100
-#define __pyx_codeobj__102 __pyx_mstate_global->__pyx_codeobj__102
-#define __pyx_codeobj__104 __pyx_mstate_global->__pyx_codeobj__104
+#define __pyx_codeobj__101 __pyx_mstate_global->__pyx_codeobj__101
+#define __pyx_codeobj__103 __pyx_mstate_global->__pyx_codeobj__103
+#define __pyx_codeobj__105 __pyx_mstate_global->__pyx_codeobj__105
 #define __pyx_codeobj__106 __pyx_mstate_global->__pyx_codeobj__106
 #define __pyx_codeobj__107 __pyx_mstate_global->__pyx_codeobj__107
 #define __pyx_codeobj__108 __pyx_mstate_global->__pyx_codeobj__108
-#define __pyx_codeobj__109 __pyx_mstate_global->__pyx_codeobj__109
+#define __pyx_codeobj__110 __pyx_mstate_global->__pyx_codeobj__110
 #define __pyx_codeobj__111 __pyx_mstate_global->__pyx_codeobj__111
 #define __pyx_codeobj__112 __pyx_mstate_global->__pyx_codeobj__112
-#define __pyx_codeobj__113 __pyx_mstate_global->__pyx_codeobj__113
-#define __pyx_codeobj__115 __pyx_mstate_global->__pyx_codeobj__115
+#define __pyx_codeobj__114 __pyx_mstate_global->__pyx_codeobj__114
+#define __pyx_codeobj__116 __pyx_mstate_global->__pyx_codeobj__116
 #define __pyx_codeobj__117 __pyx_mstate_global->__pyx_codeobj__117
-#define __pyx_codeobj__118 __pyx_mstate_global->__pyx_codeobj__118
+#define __pyx_codeobj__119 __pyx_mstate_global->__pyx_codeobj__119
 #define __pyx_codeobj__120 __pyx_mstate_global->__pyx_codeobj__120
 #define __pyx_codeobj__121 __pyx_mstate_global->__pyx_codeobj__121
 #define __pyx_codeobj__122 __pyx_mstate_global->__pyx_codeobj__122
-#define __pyx_codeobj__123 __pyx_mstate_global->__pyx_codeobj__123
-#define __pyx_codeobj__125 __pyx_mstate_global->__pyx_codeobj__125
+#define __pyx_codeobj__124 __pyx_mstate_global->__pyx_codeobj__124
+#define __pyx_codeobj__126 __pyx_mstate_global->__pyx_codeobj__126
 #define __pyx_codeobj__127 __pyx_mstate_global->__pyx_codeobj__127
 #define __pyx_codeobj__128 __pyx_mstate_global->__pyx_codeobj__128
 #define __pyx_codeobj__129 __pyx_mstate_global->__pyx_codeobj__129
 #define __pyx_codeobj__130 __pyx_mstate_global->__pyx_codeobj__130
 #define __pyx_codeobj__131 __pyx_mstate_global->__pyx_codeobj__131
-#define __pyx_codeobj__132 __pyx_mstate_global->__pyx_codeobj__132
-#define __pyx_codeobj__134 __pyx_mstate_global->__pyx_codeobj__134
+#define __pyx_codeobj__133 __pyx_mstate_global->__pyx_codeobj__133
 #endif
 /* #### Code section: module_code ### */
 
 /* "psycopg_c/pq.pyx":21
  * 
  * 
  * def version():             # <<<<<<<<<<<<<<
@@ -8761,14 +8774,18 @@
 static struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_pf_9psycopg_c_2pq_6PGconn_24exec_(struct __pyx_obj_9psycopg_c_2pq_PGconn *__pyx_v_self, char const *__pyx_v_command) {
   PGresult *__pyx_v_pgresult;
   struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exec_", 0);
 
   /* "psycopg_c/pq/pgconn.pyx":205
  * 
@@ -8796,15 +8813,15 @@
       /*try:*/ {
 
         /* "psycopg_c/pq/pgconn.pyx":208
  *         cdef libpq.PGresult *pgresult
  *         with nogil:
  *             pgresult = libpq.PQexec(self._pgconn_ptr, command)             # <<<<<<<<<<<<<<
  *         if pgresult is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  */
         __pyx_v_pgresult = PQexec(__pyx_v_self->_pgconn_ptr, __pyx_v_command);
       }
 
       /* "psycopg_c/pq/pgconn.pyx":207
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *pgresult
@@ -8824,44 +8841,96 @@
       }
   }
 
   /* "psycopg_c/pq/pgconn.pyx":209
  *         with nogil:
  *             pgresult = libpq.PQexec(self._pgconn_ptr, command)
  *         if pgresult is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  * 
  */
   __pyx_t_2 = (__pyx_v_pgresult == NULL);
   if (unlikely(__pyx_t_2)) {
 
     /* "psycopg_c/pq/pgconn.pyx":210
  *             pgresult = libpq.PQexec(self._pgconn_ptr, command)
  *         if pgresult is NULL:
- *             raise MemoryError("couldn't allocate PGresult")             # <<<<<<<<<<<<<<
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  * 
  *         return PGresult._from_ptr(pgresult)
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_executing_query_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
+      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(0, 210, __pyx_L1_error)
 
     /* "psycopg_c/pq/pgconn.pyx":209
  *         with nogil:
  *             pgresult = libpq.PQexec(self._pgconn_ptr, command)
  *         if pgresult is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  * 
  */
   }
 
   /* "psycopg_c/pq/pgconn.pyx":212
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  * 
  *         return PGresult._from_ptr(pgresult)             # <<<<<<<<<<<<<<
  * 
  *     def send_query(self, const char *command) -> None:
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_3 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_pgresult)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
@@ -8877,14 +8946,18 @@
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *pgresult
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.exec_", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9240,15 +9313,15 @@
     __pyx_v_command = __Pyx_PyObject_AsString(values[0]); if (unlikely((!__pyx_v_command) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L3_error)
     __pyx_v_param_values = values[1];
     __pyx_v_param_types = values[2];
     __pyx_v_param_formats = values[3];
     if (values[4]) {
       __pyx_v_result_format = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_result_format == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L3_error)
     } else {
-      __pyx_v_result_format = __pyx_k__8;
+      __pyx_v_result_format = __pyx_k__7;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("exec_params", 0, 2, 5, __pyx_nargs); __PYX_ERR(0, 222, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.exec_params", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -9284,14 +9357,18 @@
   Py_ssize_t __pyx_t_3;
   Oid *__pyx_t_4;
   char *const *__pyx_t_5;
   int *__pyx_t_6;
   int *__pyx_t_7;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exec_params", 0);
 
   /* "psycopg_c/pq/pgconn.pyx":230
  *         int result_format = PqFormat.TEXT,
@@ -9377,53 +9454,105 @@
   }
 
   /* "psycopg_c/pq/pgconn.pyx":245
  *                 self._pgconn_ptr, command, <int>cnparams, ctypes,
  *                 <const char *const *>cvalues, clengths, cformats, result_format)
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)             # <<<<<<<<<<<<<<
  *         if pgresult is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  */
   __pyx_f_9psycopg_c_2pq__clear_query_params(__pyx_v_ctypes, __pyx_v_cvalues, __pyx_v_clengths, __pyx_v_cformats);
 
   /* "psycopg_c/pq/pgconn.pyx":246
  *                 <const char *const *>cvalues, clengths, cformats, result_format)
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)
  *         if pgresult is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  *         return PGresult._from_ptr(pgresult)
  */
   __pyx_t_8 = (__pyx_v_pgresult == NULL);
   if (unlikely(__pyx_t_8)) {
 
     /* "psycopg_c/pq/pgconn.pyx":247
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)
  *         if pgresult is NULL:
- *             raise MemoryError("couldn't allocate PGresult")             # <<<<<<<<<<<<<<
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  *         return PGresult._from_ptr(pgresult)
  * 
  */
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 247, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_e); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_error_message); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_13 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+      __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
+      if (likely(__pyx_t_13)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+        __Pyx_INCREF(__pyx_t_13);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_12, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_13, ((PyObject *)__pyx_v_self)};
+      __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 247, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    }
+    __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_t_10, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_executing_query_failed, __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_12 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
+      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
+      if (likely(__pyx_t_12)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+        __Pyx_INCREF(__pyx_t_12);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_11, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_10};
+      __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 247, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    }
     __Pyx_Raise(__pyx_t_9, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __PYX_ERR(0, 247, __pyx_L1_error)
 
     /* "psycopg_c/pq/pgconn.pyx":246
  *                 <const char *const *>cvalues, clengths, cformats, result_format)
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)
  *         if pgresult is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  *         return PGresult._from_ptr(pgresult)
  */
   }
 
   /* "psycopg_c/pq/pgconn.pyx":248
  *         if pgresult is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"executing query failed: {error_message(self)}")
  *         return PGresult._from_ptr(pgresult)             # <<<<<<<<<<<<<<
  * 
  *     def send_query_params(
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_9 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_pgresult)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
@@ -9438,14 +9567,18 @@
  *         self,
  *         const char *command,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.exec_params", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9586,15 +9719,15 @@
     __pyx_v_command = __Pyx_PyObject_AsString(values[0]); if (unlikely((!__pyx_v_command) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L3_error)
     __pyx_v_param_values = values[1];
     __pyx_v_param_types = values[2];
     __pyx_v_param_formats = values[3];
     if (values[4]) {
       __pyx_v_result_format = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_result_format == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 256, __pyx_L3_error)
     } else {
-      __pyx_v_result_format = __pyx_k__9;
+      __pyx_v_result_format = __pyx_k__8;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("send_query_params", 0, 2, 5, __pyx_nargs); __PYX_ERR(0, 250, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.send_query_params", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -10374,15 +10507,15 @@
     }
     __pyx_v_name = __Pyx_PyObject_AsString(values[0]); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 308, __pyx_L3_error)
     __pyx_v_param_values = values[1];
     __pyx_v_param_formats = values[2];
     if (values[3]) {
       __pyx_v_result_format = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_result_format == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L3_error)
     } else {
-      __pyx_v_result_format = __pyx_k__10;
+      __pyx_v_result_format = __pyx_k__9;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("send_query_prepared", 0, 2, 4, __pyx_nargs); __PYX_ERR(0, 306, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.send_query_prepared", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -10776,14 +10909,18 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   Oid __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("prepare", 0);
 
   /* "psycopg_c/pq/pgconn.pyx":340
  *         param_types: Optional[Sequence[int]] = None,
@@ -10919,53 +11056,105 @@
   }
 
   /* "psycopg_c/pq/pgconn.pyx":354
  *             rv = libpq.PQprepare(
  *                 self._pgconn_ptr, name, command, <int>nparams, atypes)
  *         PyMem_Free(atypes)             # <<<<<<<<<<<<<<
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"preparing query failed: {error_message(self)}")
  */
   PyMem_Free(__pyx_v_atypes);
 
   /* "psycopg_c/pq/pgconn.pyx":355
  *                 self._pgconn_ptr, name, command, <int>nparams, atypes)
  *         PyMem_Free(atypes)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"preparing query failed: {error_message(self)}")
  *         return PGresult._from_ptr(rv)
  */
   __pyx_t_3 = (__pyx_v_rv == NULL);
   if (unlikely(__pyx_t_3)) {
 
     /* "psycopg_c/pq/pgconn.pyx":356
  *         PyMem_Free(atypes)
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")             # <<<<<<<<<<<<<<
+ *             raise e.OperationalError(f"preparing query failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  *         return PGresult._from_ptr(rv)
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_e); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 356, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 356, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_error_message); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 356, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_10 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+      if (likely(__pyx_t_10)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        __Pyx_INCREF(__pyx_t_10);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_9, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_10, ((PyObject *)__pyx_v_self)};
+      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 356, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    }
+    __pyx_t_9 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 356, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_preparing_query_failed, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 356, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_9 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_9);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_7};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    }
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __PYX_ERR(0, 356, __pyx_L1_error)
 
     /* "psycopg_c/pq/pgconn.pyx":355
  *                 self._pgconn_ptr, name, command, <int>nparams, atypes)
  *         PyMem_Free(atypes)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"preparing query failed: {error_message(self)}")
  *         return PGresult._from_ptr(rv)
  */
   }
 
   /* "psycopg_c/pq/pgconn.pyx":357
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(f"preparing query failed: {error_message(self)}")
  *         return PGresult._from_ptr(rv)             # <<<<<<<<<<<<<<
  * 
  *     def exec_prepared(
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_5 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -10980,14 +11169,18 @@
  *         self,
  *         const char *name,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.prepare", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -11106,15 +11299,15 @@
     }
     __pyx_v_name = __Pyx_PyObject_AsString(values[0]); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L3_error)
     __pyx_v_param_values = values[1];
     __pyx_v_param_formats = values[2];
     if (values[3]) {
       __pyx_v_result_format = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_result_format == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 364, __pyx_L3_error)
     } else {
-      __pyx_v_result_format = __pyx_k__11;
+      __pyx_v_result_format = __pyx_k__10;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("exec_prepared", 0, 2, 4, __pyx_nargs); __PYX_ERR(0, 359, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.exec_prepared", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -11150,14 +11343,18 @@
   Py_ssize_t __pyx_t_3;
   Oid *__pyx_t_4;
   char *const *__pyx_t_5;
   int *__pyx_t_6;
   int *__pyx_t_7;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exec_prepared", 0);
 
   /* "psycopg_c/pq/pgconn.pyx":366
  *         int result_format = PqFormat.TEXT,
@@ -11243,59 +11440,119 @@
   }
 
   /* "psycopg_c/pq/pgconn.pyx":383
  *                 clengths, cformats, result_format)
  * 
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)             # <<<<<<<<<<<<<<
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(
  */
   __pyx_f_9psycopg_c_2pq__clear_query_params(__pyx_v_ctypes, __pyx_v_cvalues, __pyx_v_clengths, __pyx_v_cformats);
 
   /* "psycopg_c/pq/pgconn.pyx":384
  * 
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
- *         return PGresult._from_ptr(rv)
+ *             raise e.OperationalError(
+ *                 f"executing prepared query failed: {error_message(self)}"
  */
   __pyx_t_8 = (__pyx_v_rv == NULL);
   if (unlikely(__pyx_t_8)) {
 
     /* "psycopg_c/pq/pgconn.pyx":385
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")             # <<<<<<<<<<<<<<
+ *             raise e.OperationalError(             # <<<<<<<<<<<<<<
+ *                 f"executing prepared query failed: {error_message(self)}"
+ *             )
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_e); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+
+    /* "psycopg_c/pq/pgconn.pyx":386
+ *         if rv is NULL:
+ *             raise e.OperationalError(
+ *                 f"executing prepared query failed: {error_message(self)}"             # <<<<<<<<<<<<<<
+ *             )
  *         return PGresult._from_ptr(rv)
- * 
  */
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 385, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_error_message); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_13 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+      __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
+      if (likely(__pyx_t_13)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+        __Pyx_INCREF(__pyx_t_13);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_12, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_13, ((PyObject *)__pyx_v_self)};
+      __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 386, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    }
+    __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_t_10, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_executing_prepared_query_failed, __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_12 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
+      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
+      if (likely(__pyx_t_12)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+        __Pyx_INCREF(__pyx_t_12);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_11, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_10};
+      __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 385, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    }
     __Pyx_Raise(__pyx_t_9, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __PYX_ERR(0, 385, __pyx_L1_error)
 
     /* "psycopg_c/pq/pgconn.pyx":384
  * 
  *         _clear_query_params(ctypes, cvalues, clengths, cformats)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
- *         return PGresult._from_ptr(rv)
+ *             raise e.OperationalError(
+ *                 f"executing prepared query failed: {error_message(self)}"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":386
- *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+  /* "psycopg_c/pq/pgconn.pyx":388
+ *                 f"executing prepared query failed: {error_message(self)}"
+ *             )
  *         return PGresult._from_ptr(rv)             # <<<<<<<<<<<<<<
  * 
  *     def describe_prepared(self, const char *name) -> PGresult:
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_9 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_9 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_r = ((struct __pyx_obj_9psycopg_c_2pq_PGresult *)__pyx_t_9);
   __pyx_t_9 = 0;
   goto __pyx_L0;
 
   /* "psycopg_c/pq/pgconn.pyx":359
  *         return PGresult._from_ptr(rv)
@@ -11304,23 +11561,27 @@
  *         self,
  *         const char *name,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.exec_prepared", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":388
+/* "psycopg_c/pq/pgconn.pyx":390
  *         return PGresult._from_ptr(rv)
  * 
  *     def describe_prepared(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  */
 
@@ -11333,15 +11594,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("describe_prepared (wrapper)", 0);
   assert(__pyx_arg_name); {
-    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 388, __pyx_L3_error)
+    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.describe_prepared", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -11355,103 +11616,171 @@
 static struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_pf_9psycopg_c_2pq_6PGconn_40describe_prepared(struct __pyx_obj_9psycopg_c_2pq_PGconn *__pyx_v_self, char const *__pyx_v_name) {
   PGresult *__pyx_v_rv;
   struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("describe_prepared", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":389
+  /* "psycopg_c/pq/pgconn.pyx":391
  * 
  *     def describe_prepared(self, const char *name) -> PGresult:
  *         _ensure_pgconn(self)             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  *         if rv is NULL:
  */
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 391, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":390
+  /* "psycopg_c/pq/pgconn.pyx":392
  *     def describe_prepared(self, const char *name) -> PGresult:
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)             # <<<<<<<<<<<<<<
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(
  */
   __pyx_v_rv = PQdescribePrepared(__pyx_v_self->_pgconn_ptr, __pyx_v_name);
 
-  /* "psycopg_c/pq/pgconn.pyx":391
+  /* "psycopg_c/pq/pgconn.pyx":393
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
- *         return PGresult._from_ptr(rv)
+ *             raise e.OperationalError(
+ *                 f"describe prepared failed: {error_message(self)}"
  */
   __pyx_t_2 = (__pyx_v_rv == NULL);
   if (unlikely(__pyx_t_2)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":392
+    /* "psycopg_c/pq/pgconn.pyx":394
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")             # <<<<<<<<<<<<<<
+ *             raise e.OperationalError(             # <<<<<<<<<<<<<<
+ *                 f"describe prepared failed: {error_message(self)}"
+ *             )
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "psycopg_c/pq/pgconn.pyx":395
+ *         if rv is NULL:
+ *             raise e.OperationalError(
+ *                 f"describe prepared failed: {error_message(self)}"             # <<<<<<<<<<<<<<
+ *             )
  *         return PGresult._from_ptr(rv)
- * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 395, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 395, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 395, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_describe_prepared_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 395, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
+      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 394, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 392, __pyx_L1_error)
+    __PYX_ERR(0, 394, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":391
+    /* "psycopg_c/pq/pgconn.pyx":393
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
- *         return PGresult._from_ptr(rv)
+ *             raise e.OperationalError(
+ *                 f"describe prepared failed: {error_message(self)}"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":393
- *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+  /* "psycopg_c/pq/pgconn.pyx":397
+ *                 f"describe prepared failed: {error_message(self)}"
+ *             )
  *         return PGresult._from_ptr(rv)             # <<<<<<<<<<<<<<
  * 
  *     def send_describe_prepared(self, const char *name) -> None:
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_3 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_3 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = ((struct __pyx_obj_9psycopg_c_2pq_PGresult *)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":388
+  /* "psycopg_c/pq/pgconn.pyx":390
  *         return PGresult._from_ptr(rv)
  * 
  *     def describe_prepared(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.describe_prepared", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":395
+/* "psycopg_c/pq/pgconn.pyx":399
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_prepared(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  */
 
@@ -11464,15 +11793,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("send_describe_prepared (wrapper)", 0);
   assert(__pyx_arg_name); {
-    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 395, __pyx_L3_error)
+    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 399, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.send_describe_prepared", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -11495,63 +11824,63 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_describe_prepared", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":396
+  /* "psycopg_c/pq/pgconn.pyx":400
  * 
  *     def send_describe_prepared(self, const char *name) -> None:
  *         _ensure_pgconn(self)             # <<<<<<<<<<<<<<
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  *         if not rv:
  */
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 400, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":397
+  /* "psycopg_c/pq/pgconn.pyx":401
  *     def send_describe_prepared(self, const char *name) -> None:
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)             # <<<<<<<<<<<<<<
  *         if not rv:
  *             raise e.OperationalError(
  */
   __pyx_v_rv = PQsendDescribePrepared(__pyx_v_self->_pgconn_ptr, __pyx_v_name);
 
-  /* "psycopg_c/pq/pgconn.pyx":398
+  /* "psycopg_c/pq/pgconn.pyx":402
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  *         if not rv:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(
  *                 f"sending describe prepared failed: {error_message(self)}"
  */
   __pyx_t_2 = (!(__pyx_v_rv != 0));
   if (unlikely(__pyx_t_2)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":399
+    /* "psycopg_c/pq/pgconn.pyx":403
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  *         if not rv:
  *             raise e.OperationalError(             # <<<<<<<<<<<<<<
  *                 f"sending describe prepared failed: {error_message(self)}"
  *             )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 399, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 399, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":400
+    /* "psycopg_c/pq/pgconn.pyx":404
  *         if not rv:
  *             raise e.OperationalError(
  *                 f"sending describe prepared failed: {error_message(self)}"             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_1 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -11561,22 +11890,22 @@
         __pyx_t_1 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 404, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_describe_prepared_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_describe_prepared_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_1 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
@@ -11588,32 +11917,32 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 399, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 399, __pyx_L1_error)
+    __PYX_ERR(0, 403, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":398
+    /* "psycopg_c/pq/pgconn.pyx":402
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  *         if not rv:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(
  *                 f"sending describe prepared failed: {error_message(self)}"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":395
+  /* "psycopg_c/pq/pgconn.pyx":399
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_prepared(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  */
 
@@ -11630,15 +11959,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":403
+/* "psycopg_c/pq/pgconn.pyx":407
  *             )
  * 
  *     def describe_portal(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  */
 
@@ -11651,15 +11980,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("describe_portal (wrapper)", 0);
   assert(__pyx_arg_name); {
-    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 403, __pyx_L3_error)
+    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.describe_portal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -11673,103 +12002,171 @@
 static struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_pf_9psycopg_c_2pq_6PGconn_44describe_portal(struct __pyx_obj_9psycopg_c_2pq_PGconn *__pyx_v_self, char const *__pyx_v_name) {
   PGresult *__pyx_v_rv;
   struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("describe_portal", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":404
+  /* "psycopg_c/pq/pgconn.pyx":408
  * 
  *     def describe_portal(self, const char *name) -> PGresult:
  *         _ensure_pgconn(self)             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  *         if rv is NULL:
  */
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 408, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":405
+  /* "psycopg_c/pq/pgconn.pyx":409
  *     def describe_portal(self, const char *name) -> PGresult:
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)             # <<<<<<<<<<<<<<
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+ *             raise e.OperationalError(
  */
   __pyx_v_rv = PQdescribePortal(__pyx_v_self->_pgconn_ptr, __pyx_v_name);
 
-  /* "psycopg_c/pq/pgconn.pyx":406
+  /* "psycopg_c/pq/pgconn.pyx":410
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
- *         return PGresult._from_ptr(rv)
+ *             raise e.OperationalError(
+ *                 f"describe prepared failed: {error_message(self)}"
  */
   __pyx_t_2 = (__pyx_v_rv == NULL);
   if (unlikely(__pyx_t_2)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":407
+    /* "psycopg_c/pq/pgconn.pyx":411
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")             # <<<<<<<<<<<<<<
+ *             raise e.OperationalError(             # <<<<<<<<<<<<<<
+ *                 f"describe prepared failed: {error_message(self)}"
+ *             )
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "psycopg_c/pq/pgconn.pyx":412
+ *         if rv is NULL:
+ *             raise e.OperationalError(
+ *                 f"describe prepared failed: {error_message(self)}"             # <<<<<<<<<<<<<<
+ *             )
  *         return PGresult._from_ptr(rv)
- * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_describe_prepared_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
+      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 407, __pyx_L1_error)
+    __PYX_ERR(0, 411, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":406
+    /* "psycopg_c/pq/pgconn.pyx":410
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  *         if rv is NULL:             # <<<<<<<<<<<<<<
- *             raise MemoryError("couldn't allocate PGresult")
- *         return PGresult._from_ptr(rv)
+ *             raise e.OperationalError(
+ *                 f"describe prepared failed: {error_message(self)}"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":408
- *         if rv is NULL:
- *             raise MemoryError("couldn't allocate PGresult")
+  /* "psycopg_c/pq/pgconn.pyx":414
+ *                 f"describe prepared failed: {error_message(self)}"
+ *             )
  *         return PGresult._from_ptr(rv)             # <<<<<<<<<<<<<<
  * 
  *     def send_describe_portal(self, const char *name) -> None:
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_3 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_3 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = ((struct __pyx_obj_9psycopg_c_2pq_PGresult *)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":403
+  /* "psycopg_c/pq/pgconn.pyx":407
  *             )
  * 
  *     def describe_portal(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.describe_portal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":410
+/* "psycopg_c/pq/pgconn.pyx":416
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_portal(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  */
 
@@ -11782,15 +12179,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("send_describe_portal (wrapper)", 0);
   assert(__pyx_arg_name); {
-    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 410, __pyx_L3_error)
+    __pyx_v_name = __Pyx_PyObject_AsString(__pyx_arg_name); if (unlikely((!__pyx_v_name) && PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.send_describe_portal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -11813,63 +12210,63 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_describe_portal", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":411
+  /* "psycopg_c/pq/pgconn.pyx":417
  * 
  *     def send_describe_portal(self, const char *name) -> None:
  *         _ensure_pgconn(self)             # <<<<<<<<<<<<<<
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  *         if not rv:
  */
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 417, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":412
+  /* "psycopg_c/pq/pgconn.pyx":418
  *     def send_describe_portal(self, const char *name) -> None:
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)             # <<<<<<<<<<<<<<
  *         if not rv:
  *             raise e.OperationalError(
  */
   __pyx_v_rv = PQsendDescribePortal(__pyx_v_self->_pgconn_ptr, __pyx_v_name);
 
-  /* "psycopg_c/pq/pgconn.pyx":413
+  /* "psycopg_c/pq/pgconn.pyx":419
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  *         if not rv:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(
  *                 f"sending describe prepared failed: {error_message(self)}"
  */
   __pyx_t_2 = (!(__pyx_v_rv != 0));
   if (unlikely(__pyx_t_2)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":414
+    /* "psycopg_c/pq/pgconn.pyx":420
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  *         if not rv:
  *             raise e.OperationalError(             # <<<<<<<<<<<<<<
  *                 f"sending describe prepared failed: {error_message(self)}"
  *             )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":415
+    /* "psycopg_c/pq/pgconn.pyx":421
  *         if not rv:
  *             raise e.OperationalError(
  *                 f"sending describe prepared failed: {error_message(self)}"             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_1 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -11879,22 +12276,22 @@
         __pyx_t_1 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 415, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_describe_prepared_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_describe_prepared_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_1 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
@@ -11906,32 +12303,32 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 414, __pyx_L1_error)
+    __PYX_ERR(0, 420, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":413
+    /* "psycopg_c/pq/pgconn.pyx":419
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  *         if not rv:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(
  *                 f"sending describe prepared failed: {error_message(self)}"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":410
+  /* "psycopg_c/pq/pgconn.pyx":416
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_portal(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  */
 
@@ -11948,15 +12345,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":418
+/* "psycopg_c/pq/pgconn.pyx":424
  *             )
  * 
  *     def get_result(self) -> Optional["PGresult"]:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)
  *         if pgresult is NULL:
  */
 
@@ -11982,68 +12379,68 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_result", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":419
+  /* "psycopg_c/pq/pgconn.pyx":425
  * 
  *     def get_result(self) -> Optional["PGresult"]:
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         if pgresult is NULL:
  *             return None
  */
   __pyx_v_pgresult = PQgetResult(__pyx_v_self->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":420
+  /* "psycopg_c/pq/pgconn.pyx":426
  *     def get_result(self) -> Optional["PGresult"]:
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)
  *         if pgresult is NULL:             # <<<<<<<<<<<<<<
  *             return None
  *         return PGresult._from_ptr(pgresult)
  */
   __pyx_t_1 = (__pyx_v_pgresult == NULL);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":421
+    /* "psycopg_c/pq/pgconn.pyx":427
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)
  *         if pgresult is NULL:
  *             return None             # <<<<<<<<<<<<<<
  *         return PGresult._from_ptr(pgresult)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":420
+    /* "psycopg_c/pq/pgconn.pyx":426
  *     def get_result(self) -> Optional["PGresult"]:
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)
  *         if pgresult is NULL:             # <<<<<<<<<<<<<<
  *             return None
  *         return PGresult._from_ptr(pgresult)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":422
+  /* "psycopg_c/pq/pgconn.pyx":428
  *         if pgresult is NULL:
  *             return None
  *         return PGresult._from_ptr(pgresult)             # <<<<<<<<<<<<<<
  * 
  *     def consume_input(self) -> None:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_pgresult)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_pgresult)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":418
+  /* "psycopg_c/pq/pgconn.pyx":424
  *             )
  * 
  *     def get_result(self) -> Optional["PGresult"]:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)
  *         if pgresult is NULL:
  */
 
@@ -12054,15 +12451,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":424
+/* "psycopg_c/pq/pgconn.pyx":430
  *         return PGresult._from_ptr(pgresult)
  * 
  *     def consume_input(self) -> None:             # <<<<<<<<<<<<<<
  *         if 1 != libpq.PQconsumeInput(self._pgconn_ptr):
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  */
 
@@ -12092,37 +12489,37 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("consume_input", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":425
+  /* "psycopg_c/pq/pgconn.pyx":431
  * 
  *     def consume_input(self) -> None:
  *         if 1 != libpq.PQconsumeInput(self._pgconn_ptr):             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  * 
  */
   __pyx_t_1 = (1 != PQconsumeInput(__pyx_v_self->_pgconn_ptr));
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":426
+    /* "psycopg_c/pq/pgconn.pyx":432
  *     def consume_input(self) -> None:
  *         if 1 != libpq.PQconsumeInput(self._pgconn_ptr):
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  * 
  *     def is_busy(self) -> int:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_error_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 426, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_error_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -12132,22 +12529,22 @@
         __pyx_t_7 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, ((PyObject *)__pyx_v_self)};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 426, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_consuming_input_failed, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_consuming_input_failed, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -12159,32 +12556,32 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 426, __pyx_L1_error)
+    __PYX_ERR(0, 432, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":425
+    /* "psycopg_c/pq/pgconn.pyx":431
  * 
  *     def consume_input(self) -> None:
  *         if 1 != libpq.PQconsumeInput(self._pgconn_ptr):             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":424
+  /* "psycopg_c/pq/pgconn.pyx":430
  *         return PGresult._from_ptr(pgresult)
  * 
  *     def consume_input(self) -> None:             # <<<<<<<<<<<<<<
  *         if 1 != libpq.PQconsumeInput(self._pgconn_ptr):
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  */
 
@@ -12201,15 +12598,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":428
+/* "psycopg_c/pq/pgconn.pyx":434
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  * 
  *     def is_busy(self) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         with nogil:
  */
 
@@ -12234,15 +12631,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_busy", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":430
+  /* "psycopg_c/pq/pgconn.pyx":436
  *     def is_busy(self) -> int:
  *         cdef int rv
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rv = libpq.PQisBusy(self._pgconn_ptr)
  *         return rv
  */
   {
@@ -12250,25 +12647,25 @@
       PyThreadState *_save;
       _save = NULL;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "psycopg_c/pq/pgconn.pyx":431
+        /* "psycopg_c/pq/pgconn.pyx":437
  *         cdef int rv
  *         with nogil:
  *             rv = libpq.PQisBusy(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         return rv
  * 
  */
         __pyx_v_rv = PQisBusy(__pyx_v_self->_pgconn_ptr);
       }
 
-      /* "psycopg_c/pq/pgconn.pyx":430
+      /* "psycopg_c/pq/pgconn.pyx":436
  *     def is_busy(self) -> int:
  *         cdef int rv
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rv = libpq.PQisBusy(self._pgconn_ptr)
  *         return rv
  */
       /*finally:*/ {
@@ -12279,30 +12676,30 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":432
+  /* "psycopg_c/pq/pgconn.pyx":438
  *         with nogil:
  *             rv = libpq.PQisBusy(self._pgconn_ptr)
  *         return rv             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_rv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_rv); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyInt_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 432, __pyx_L1_error)
+  if (!(likely(PyInt_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 438, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":428
+  /* "psycopg_c/pq/pgconn.pyx":434
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  * 
  *     def is_busy(self) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         with nogil:
  */
 
@@ -12313,15 +12710,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":434
+/* "psycopg_c/pq/pgconn.pyx":440
  *         return rv
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def nonblocking(self) -> int:
  *         return libpq.PQisnonblocking(self._pgconn_ptr)
  */
 
@@ -12344,29 +12741,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":436
+  /* "psycopg_c/pq/pgconn.pyx":442
  *     @property
  *     def nonblocking(self) -> int:
  *         return libpq.PQisnonblocking(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  * 
  *     @nonblocking.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(PQisnonblocking(__pyx_v_self->_pgconn_ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(PQisnonblocking(__pyx_v_self->_pgconn_ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":434
+  /* "psycopg_c/pq/pgconn.pyx":440
  *         return rv
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def nonblocking(self) -> int:
  *         return libpq.PQisnonblocking(self._pgconn_ptr)
  */
 
@@ -12377,15 +12774,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":438
+/* "psycopg_c/pq/pgconn.pyx":444
  *         return libpq.PQisnonblocking(self._pgconn_ptr)
  * 
  *     @nonblocking.setter             # <<<<<<<<<<<<<<
  *     def nonblocking(self, int arg) -> None:
  *         if 0 > libpq.PQsetnonblocking(self._pgconn_ptr, arg):
  */
 
@@ -12397,15 +12794,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_arg); {
-    __pyx_v_arg = __Pyx_PyInt_As_int(__pyx_arg_arg); if (unlikely((__pyx_v_arg == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 439, __pyx_L3_error)
+    __pyx_v_arg = __Pyx_PyInt_As_int(__pyx_arg_arg); if (unlikely((__pyx_v_arg == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.nonblocking.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -12427,37 +12824,37 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":440
+  /* "psycopg_c/pq/pgconn.pyx":446
  *     @nonblocking.setter
  *     def nonblocking(self, int arg) -> None:
  *         if 0 > libpq.PQsetnonblocking(self._pgconn_ptr, arg):             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"setting nonblocking failed: {error_message(self)}")
  * 
  */
   __pyx_t_1 = (0 > PQsetnonblocking(__pyx_v_self->_pgconn_ptr, __pyx_v_arg));
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":441
+    /* "psycopg_c/pq/pgconn.pyx":447
  *     def nonblocking(self, int arg) -> None:
  *         if 0 > libpq.PQsetnonblocking(self._pgconn_ptr, arg):
  *             raise e.OperationalError(f"setting nonblocking failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  * 
  *     cpdef int flush(self) except -1:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_error_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_error_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -12467,22 +12864,22 @@
         __pyx_t_7 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, ((PyObject *)__pyx_v_self)};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_setting_nonblocking_failed, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_setting_nonblocking_failed, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -12494,32 +12891,32 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 441, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 441, __pyx_L1_error)
+    __PYX_ERR(0, 447, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":440
+    /* "psycopg_c/pq/pgconn.pyx":446
  *     @nonblocking.setter
  *     def nonblocking(self, int arg) -> None:
  *         if 0 > libpq.PQsetnonblocking(self._pgconn_ptr, arg):             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"setting nonblocking failed: {error_message(self)}")
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":438
+  /* "psycopg_c/pq/pgconn.pyx":444
  *         return libpq.PQisnonblocking(self._pgconn_ptr)
  * 
  *     @nonblocking.setter             # <<<<<<<<<<<<<<
  *     def nonblocking(self, int arg) -> None:
  *         if 0 > libpq.PQsetnonblocking(self._pgconn_ptr, arg):
  */
 
@@ -12535,15 +12932,15 @@
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.nonblocking.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":443
+/* "psycopg_c/pq/pgconn.pyx":449
  *             raise e.OperationalError(f"setting nonblocking failed: {error_message(self)}")
  * 
  *     cpdef int flush(self) except -1:             # <<<<<<<<<<<<<<
  *         if self._pgconn_ptr == NULL:
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  */
 
@@ -12568,15 +12965,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_flush); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_flush); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 449, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_9psycopg_c_2pq_6PGconn_55flush)) {
@@ -12593,19 +12990,19 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_4, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 449, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 443, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -12616,34 +13013,34 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":444
+  /* "psycopg_c/pq/pgconn.pyx":450
  * 
  *     cpdef int flush(self) except -1:
  *         if self._pgconn_ptr == NULL:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  *         cdef int rv = libpq.PQflush(self._pgconn_ptr)
  */
   __pyx_t_6 = (__pyx_v_self->_pgconn_ptr == NULL);
   if (unlikely(__pyx_t_6)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":445
+    /* "psycopg_c/pq/pgconn.pyx":451
  *     cpdef int flush(self) except -1:
  *         if self._pgconn_ptr == NULL:
  *             raise e.OperationalError(f"flushing failed: the connection is closed")             # <<<<<<<<<<<<<<
  *         cdef int rv = libpq.PQflush(self._pgconn_ptr)
  *         if rv < 0:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_e); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_e); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
@@ -12654,63 +13051,63 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_u_flushing_failed_the_connection_i};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 445, __pyx_L1_error)
+    __PYX_ERR(0, 451, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":444
+    /* "psycopg_c/pq/pgconn.pyx":450
  * 
  *     cpdef int flush(self) except -1:
  *         if self._pgconn_ptr == NULL:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  *         cdef int rv = libpq.PQflush(self._pgconn_ptr)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":446
+  /* "psycopg_c/pq/pgconn.pyx":452
  *         if self._pgconn_ptr == NULL:
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  *         cdef int rv = libpq.PQflush(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         if rv < 0:
  *             raise e.OperationalError(f"flushing failed: {error_message(self)}")
  */
   __pyx_v_rv = PQflush(__pyx_v_self->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":447
+  /* "psycopg_c/pq/pgconn.pyx":453
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  *         cdef int rv = libpq.PQflush(self._pgconn_ptr)
  *         if rv < 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"flushing failed: {error_message(self)}")
  *         return rv
  */
   __pyx_t_6 = (__pyx_v_rv < 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":448
+    /* "psycopg_c/pq/pgconn.pyx":454
  *         cdef int rv = libpq.PQflush(self._pgconn_ptr)
  *         if rv < 0:
  *             raise e.OperationalError(f"flushing failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  *         return rv
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 448, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_error_message); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_error_message); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -12720,22 +13117,22 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_flushing_failed, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_flushing_failed, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
@@ -12747,42 +13144,42 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 448, __pyx_L1_error)
+    __PYX_ERR(0, 454, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":447
+    /* "psycopg_c/pq/pgconn.pyx":453
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  *         cdef int rv = libpq.PQflush(self._pgconn_ptr)
  *         if rv < 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"flushing failed: {error_message(self)}")
  *         return rv
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":449
+  /* "psycopg_c/pq/pgconn.pyx":455
  *         if rv < 0:
  *             raise e.OperationalError(f"flushing failed: {error_message(self)}")
  *         return rv             # <<<<<<<<<<<<<<
  * 
  *     def set_single_row_mode(self) -> None:
  */
   __pyx_r = __pyx_v_rv;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":443
+  /* "psycopg_c/pq/pgconn.pyx":449
  *             raise e.OperationalError(f"setting nonblocking failed: {error_message(self)}")
  * 
  *     cpdef int flush(self) except -1:             # <<<<<<<<<<<<<<
  *         if self._pgconn_ptr == NULL:
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  */
 
@@ -12821,16 +13218,16 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("flush", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq_6PGconn_flush(__pyx_v_self, 1); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 443, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq_6PGconn_flush(__pyx_v_self, 1); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12839,15 +13236,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":451
+/* "psycopg_c/pq/pgconn.pyx":457
  *         return rv
  * 
  *     def set_single_row_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         if not libpq.PQsetSingleRowMode(self._pgconn_ptr):
  *             raise e.OperationalError("setting single row mode failed")
  */
 
@@ -12875,34 +13272,34 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_single_row_mode", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":452
+  /* "psycopg_c/pq/pgconn.pyx":458
  * 
  *     def set_single_row_mode(self) -> None:
  *         if not libpq.PQsetSingleRowMode(self._pgconn_ptr):             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("setting single row mode failed")
  * 
  */
   __pyx_t_1 = (!(PQsetSingleRowMode(__pyx_v_self->_pgconn_ptr) != 0));
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":453
+    /* "psycopg_c/pq/pgconn.pyx":459
  *     def set_single_row_mode(self) -> None:
  *         if not libpq.PQsetSingleRowMode(self._pgconn_ptr):
  *             raise e.OperationalError("setting single row mode failed")             # <<<<<<<<<<<<<<
  * 
  *     def get_cancel(self) -> PGcancel:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -12913,32 +13310,32 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_setting_single_row_mode_failed};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 453, __pyx_L1_error)
+    __PYX_ERR(0, 459, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":452
+    /* "psycopg_c/pq/pgconn.pyx":458
  * 
  *     def set_single_row_mode(self) -> None:
  *         if not libpq.PQsetSingleRowMode(self._pgconn_ptr):             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("setting single row mode failed")
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":451
+  /* "psycopg_c/pq/pgconn.pyx":457
  *         return rv
  * 
  *     def set_single_row_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         if not libpq.PQsetSingleRowMode(self._pgconn_ptr):
  *             raise e.OperationalError("setting single row mode failed")
  */
 
@@ -12953,15 +13350,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":455
+/* "psycopg_c/pq/pgconn.pyx":461
  *             raise e.OperationalError("setting single row mode failed")
  * 
  *     def get_cancel(self) -> PGcancel:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)
  *         if not ptr:
  */
 
@@ -12990,43 +13387,43 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cancel", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":456
+  /* "psycopg_c/pq/pgconn.pyx":462
  * 
  *     def get_cancel(self) -> PGcancel:
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         if not ptr:
  *             raise e.OperationalError("couldn't create cancel object")
  */
   __pyx_v_ptr = PQgetCancel(__pyx_v_self->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":457
+  /* "psycopg_c/pq/pgconn.pyx":463
  *     def get_cancel(self) -> PGcancel:
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)
  *         if not ptr:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("couldn't create cancel object")
  *         return PGcancel._from_ptr(ptr)
  */
   __pyx_t_1 = (!(__pyx_v_ptr != 0));
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":458
+    /* "psycopg_c/pq/pgconn.pyx":464
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)
  *         if not ptr:
  *             raise e.OperationalError("couldn't create cancel object")             # <<<<<<<<<<<<<<
  *         return PGcancel._from_ptr(ptr)
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 458, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -13037,46 +13434,46 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_couldn_t_create_cancel_object};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 458, __pyx_L1_error)
+    __PYX_ERR(0, 464, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":457
+    /* "psycopg_c/pq/pgconn.pyx":463
  *     def get_cancel(self) -> PGcancel:
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)
  *         if not ptr:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("couldn't create cancel object")
  *         return PGcancel._from_ptr(ptr)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":459
+  /* "psycopg_c/pq/pgconn.pyx":465
  *         if not ptr:
  *             raise e.OperationalError("couldn't create cancel object")
  *         return PGcancel._from_ptr(ptr)             # <<<<<<<<<<<<<<
  * 
  *     cpdef object notifies(self):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGcancel__from_ptr(__pyx_v_ptr)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGcancel__from_ptr(__pyx_v_ptr)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = ((struct __pyx_obj_9psycopg_c_2pq_PGcancel *)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":455
+  /* "psycopg_c/pq/pgconn.pyx":461
  *             raise e.OperationalError("setting single row mode failed")
  * 
  *     def get_cancel(self) -> PGcancel:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)
  *         if not ptr:
  */
 
@@ -13089,15 +13486,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":461
+/* "psycopg_c/pq/pgconn.pyx":467
  *         return PGcancel._from_ptr(ptr)
  * 
  *     cpdef object notifies(self):             # <<<<<<<<<<<<<<
  *         cdef libpq.PGnotify *ptr
  *         with nogil:
  */
 
@@ -13124,15 +13521,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_notifies); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_notifies); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_9psycopg_c_2pq_6PGconn_61notifies)) {
@@ -13150,15 +13547,15 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_4, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -13172,15 +13569,15 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":463
+  /* "psycopg_c/pq/pgconn.pyx":469
  *     cpdef object notifies(self):
  *         cdef libpq.PGnotify *ptr
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ptr = libpq.PQnotifies(self._pgconn_ptr)
  *         if ptr:
  */
   {
@@ -13188,25 +13585,25 @@
       PyThreadState *_save;
       _save = NULL;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "psycopg_c/pq/pgconn.pyx":464
+        /* "psycopg_c/pq/pgconn.pyx":470
  *         cdef libpq.PGnotify *ptr
  *         with nogil:
  *             ptr = libpq.PQnotifies(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         if ptr:
  *             ret = PGnotify(ptr.relname, ptr.be_pid, ptr.extra)
  */
         __pyx_v_ptr = PQnotifies(__pyx_v_self->_pgconn_ptr);
       }
 
-      /* "psycopg_c/pq/pgconn.pyx":463
+      /* "psycopg_c/pq/pgconn.pyx":469
  *     cpdef object notifies(self):
  *         cdef libpq.PGnotify *ptr
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ptr = libpq.PQnotifies(self._pgconn_ptr)
  *         if ptr:
  */
       /*finally:*/ {
@@ -13217,38 +13614,38 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":465
+  /* "psycopg_c/pq/pgconn.pyx":471
  *         with nogil:
  *             ptr = libpq.PQnotifies(self._pgconn_ptr)
  *         if ptr:             # <<<<<<<<<<<<<<
  *             ret = PGnotify(ptr.relname, ptr.be_pid, ptr.extra)
  *             libpq.PQfreemem(ptr)
  */
   __pyx_t_6 = (__pyx_v_ptr != 0);
   if (__pyx_t_6) {
 
-    /* "psycopg_c/pq/pgconn.pyx":466
+    /* "psycopg_c/pq/pgconn.pyx":472
  *             ptr = libpq.PQnotifies(self._pgconn_ptr)
  *         if ptr:
  *             ret = PGnotify(ptr.relname, ptr.be_pid, ptr.extra)             # <<<<<<<<<<<<<<
  *             libpq.PQfreemem(ptr)
  *             return ret
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PGnotify); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PGnotify); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_ptr->relname); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_ptr->relname); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_ptr->be_pid); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 466, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_ptr->be_pid); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyBytes_FromString(__pyx_v_ptr->extra); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 466, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyBytes_FromString(__pyx_v_ptr->extra); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -13261,65 +13658,65 @@
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_8, __pyx_t_3, __pyx_t_4, __pyx_t_7};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 3+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_v_ret = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":467
+    /* "psycopg_c/pq/pgconn.pyx":473
  *         if ptr:
  *             ret = PGnotify(ptr.relname, ptr.be_pid, ptr.extra)
  *             libpq.PQfreemem(ptr)             # <<<<<<<<<<<<<<
  *             return ret
  *         else:
  */
     PQfreemem(__pyx_v_ptr);
 
-    /* "psycopg_c/pq/pgconn.pyx":468
+    /* "psycopg_c/pq/pgconn.pyx":474
  *             ret = PGnotify(ptr.relname, ptr.be_pid, ptr.extra)
  *             libpq.PQfreemem(ptr)
  *             return ret             # <<<<<<<<<<<<<<
  *         else:
  *             return None
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_ret);
     __pyx_r = __pyx_v_ret;
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":465
+    /* "psycopg_c/pq/pgconn.pyx":471
  *         with nogil:
  *             ptr = libpq.PQnotifies(self._pgconn_ptr)
  *         if ptr:             # <<<<<<<<<<<<<<
  *             ret = PGnotify(ptr.relname, ptr.be_pid, ptr.extra)
  *             libpq.PQfreemem(ptr)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":470
+  /* "psycopg_c/pq/pgconn.pyx":476
  *             return ret
  *         else:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *     def put_copy_data(self, buffer) -> int:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":461
+  /* "psycopg_c/pq/pgconn.pyx":467
  *         return PGcancel._from_ptr(ptr)
  * 
  *     cpdef object notifies(self):             # <<<<<<<<<<<<<<
  *         cdef libpq.PGnotify *ptr
  *         with nogil:
  */
 
@@ -13360,15 +13757,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("notifies", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq_6PGconn_notifies(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq_6PGconn_notifies(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13377,15 +13774,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":472
+/* "psycopg_c/pq/pgconn.pyx":478
  *             return None
  * 
  *     def put_copy_data(self, buffer) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef char *cbuffer
  */
 
@@ -13418,55 +13815,55 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("put_copy_data", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":477
+  /* "psycopg_c/pq/pgconn.pyx":483
  *         cdef Py_ssize_t length
  * 
  *         _buffer_as_string_and_size(buffer, &cbuffer, &length)             # <<<<<<<<<<<<<<
  *         rv = libpq.PQputCopyData(self._pgconn_ptr, cbuffer, <int>length)
  *         if rv < 0:
  */
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__buffer_as_string_and_size(__pyx_v_buffer, (&__pyx_v_cbuffer), (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 477, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__buffer_as_string_and_size(__pyx_v_buffer, (&__pyx_v_cbuffer), (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 483, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":478
+  /* "psycopg_c/pq/pgconn.pyx":484
  * 
  *         _buffer_as_string_and_size(buffer, &cbuffer, &length)
  *         rv = libpq.PQputCopyData(self._pgconn_ptr, cbuffer, <int>length)             # <<<<<<<<<<<<<<
  *         if rv < 0:
  *             raise e.OperationalError(f"sending copy data failed: {error_message(self)}")
  */
   __pyx_v_rv = PQputCopyData(__pyx_v_self->_pgconn_ptr, __pyx_v_cbuffer, ((int)__pyx_v_length));
 
-  /* "psycopg_c/pq/pgconn.pyx":479
+  /* "psycopg_c/pq/pgconn.pyx":485
  *         _buffer_as_string_and_size(buffer, &cbuffer, &length)
  *         rv = libpq.PQputCopyData(self._pgconn_ptr, cbuffer, <int>length)
  *         if rv < 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"sending copy data failed: {error_message(self)}")
  *         return rv
  */
   __pyx_t_2 = (__pyx_v_rv < 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":480
+    /* "psycopg_c/pq/pgconn.pyx":486
  *         rv = libpq.PQputCopyData(self._pgconn_ptr, cbuffer, <int>length)
  *         if rv < 0:
  *             raise e.OperationalError(f"sending copy data failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  *         return rv
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_1 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -13476,22 +13873,22 @@
         __pyx_t_1 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_copy_data_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_copy_data_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_1 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
@@ -13503,47 +13900,47 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 486, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 480, __pyx_L1_error)
+    __PYX_ERR(0, 486, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":479
+    /* "psycopg_c/pq/pgconn.pyx":485
  *         _buffer_as_string_and_size(buffer, &cbuffer, &length)
  *         rv = libpq.PQputCopyData(self._pgconn_ptr, cbuffer, <int>length)
  *         if rv < 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"sending copy data failed: {error_message(self)}")
  *         return rv
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":481
+  /* "psycopg_c/pq/pgconn.pyx":487
  *         if rv < 0:
  *             raise e.OperationalError(f"sending copy data failed: {error_message(self)}")
  *         return rv             # <<<<<<<<<<<<<<
  * 
  *     def put_copy_end(self, error: Optional[bytes] = None) -> int:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_rv); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_rv); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(PyInt_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (!(likely(PyInt_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 487, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":472
+  /* "psycopg_c/pq/pgconn.pyx":478
  *             return None
  * 
  *     def put_copy_data(self, buffer) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef char *cbuffer
  */
 
@@ -13558,15 +13955,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":483
+/* "psycopg_c/pq/pgconn.pyx":489
  *         return rv
  * 
  *     def put_copy_end(self, error: Optional[bytes] = None) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef const char *cerr = NULL
  */
 
@@ -13615,34 +14012,34 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_error);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 489, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "put_copy_end") < 0)) __PYX_ERR(0, 483, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "put_copy_end") < 0)) __PYX_ERR(0, 489, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_error = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("put_copy_end", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 483, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("put_copy_end", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 489, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.put_copy_end", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9psycopg_c_2pq_6PGconn_64put_copy_end(((struct __pyx_obj_9psycopg_c_2pq_PGconn *)__pyx_v_self), __pyx_v_error);
 
@@ -13665,84 +14062,84 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("put_copy_end", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":485
+  /* "psycopg_c/pq/pgconn.pyx":491
  *     def put_copy_end(self, error: Optional[bytes] = None) -> int:
  *         cdef int rv
  *         cdef const char *cerr = NULL             # <<<<<<<<<<<<<<
  *         if error is not None:
  *             cerr = PyBytes_AsString(error)
  */
   __pyx_v_cerr = NULL;
 
-  /* "psycopg_c/pq/pgconn.pyx":486
+  /* "psycopg_c/pq/pgconn.pyx":492
  *         cdef int rv
  *         cdef const char *cerr = NULL
  *         if error is not None:             # <<<<<<<<<<<<<<
  *             cerr = PyBytes_AsString(error)
  *         rv = libpq.PQputCopyEnd(self._pgconn_ptr, cerr)
  */
   __pyx_t_1 = (__pyx_v_error != Py_None);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":487
+    /* "psycopg_c/pq/pgconn.pyx":493
  *         cdef const char *cerr = NULL
  *         if error is not None:
  *             cerr = PyBytes_AsString(error)             # <<<<<<<<<<<<<<
  *         rv = libpq.PQputCopyEnd(self._pgconn_ptr, cerr)
  *         if rv < 0:
  */
-    __pyx_t_2 = PyBytes_AsString(__pyx_v_error); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(0, 487, __pyx_L1_error)
+    __pyx_t_2 = PyBytes_AsString(__pyx_v_error); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(0, 493, __pyx_L1_error)
     __pyx_v_cerr = __pyx_t_2;
 
-    /* "psycopg_c/pq/pgconn.pyx":486
+    /* "psycopg_c/pq/pgconn.pyx":492
  *         cdef int rv
  *         cdef const char *cerr = NULL
  *         if error is not None:             # <<<<<<<<<<<<<<
  *             cerr = PyBytes_AsString(error)
  *         rv = libpq.PQputCopyEnd(self._pgconn_ptr, cerr)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":488
+  /* "psycopg_c/pq/pgconn.pyx":494
  *         if error is not None:
  *             cerr = PyBytes_AsString(error)
  *         rv = libpq.PQputCopyEnd(self._pgconn_ptr, cerr)             # <<<<<<<<<<<<<<
  *         if rv < 0:
  *             raise e.OperationalError(f"sending copy end failed: {error_message(self)}")
  */
   __pyx_v_rv = PQputCopyEnd(__pyx_v_self->_pgconn_ptr, __pyx_v_cerr);
 
-  /* "psycopg_c/pq/pgconn.pyx":489
+  /* "psycopg_c/pq/pgconn.pyx":495
  *             cerr = PyBytes_AsString(error)
  *         rv = libpq.PQputCopyEnd(self._pgconn_ptr, cerr)
  *         if rv < 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"sending copy end failed: {error_message(self)}")
  *         return rv
  */
   __pyx_t_1 = (__pyx_v_rv < 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":490
+    /* "psycopg_c/pq/pgconn.pyx":496
  *         rv = libpq.PQputCopyEnd(self._pgconn_ptr, cerr)
  *         if rv < 0:
  *             raise e.OperationalError(f"sending copy end failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  *         return rv
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_error_message); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -13752,22 +14149,22 @@
         __pyx_t_8 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_self)};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 490, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_copy_end_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_sending_copy_end_failed, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
@@ -13779,47 +14176,47 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 490, __pyx_L1_error)
+    __PYX_ERR(0, 496, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":489
+    /* "psycopg_c/pq/pgconn.pyx":495
  *             cerr = PyBytes_AsString(error)
  *         rv = libpq.PQputCopyEnd(self._pgconn_ptr, cerr)
  *         if rv < 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"sending copy end failed: {error_message(self)}")
  *         return rv
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":491
+  /* "psycopg_c/pq/pgconn.pyx":497
  *         if rv < 0:
  *             raise e.OperationalError(f"sending copy end failed: {error_message(self)}")
  *         return rv             # <<<<<<<<<<<<<<
  * 
  *     def get_copy_data(self, int async_) -> Tuple[int, memoryview]:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_rv); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_rv); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(PyInt_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 491, __pyx_L1_error)
+  if (!(likely(PyInt_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 497, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":483
+  /* "psycopg_c/pq/pgconn.pyx":489
  *         return rv
  * 
  *     def put_copy_end(self, error: Optional[bytes] = None) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef const char *cerr = NULL
  */
 
@@ -13834,15 +14231,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":493
+/* "psycopg_c/pq/pgconn.pyx":499
  *         return rv
  * 
  *     def get_copy_data(self, int async_) -> Tuple[int, memoryview]:             # <<<<<<<<<<<<<<
  *         cdef char *buffer_ptr = NULL
  *         cdef int nbytes
  */
 
@@ -13855,15 +14252,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_copy_data (wrapper)", 0);
   assert(__pyx_arg_async_); {
-    __pyx_v_async_ = __Pyx_PyInt_As_int(__pyx_arg_async_); if (unlikely((__pyx_v_async_ == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 493, __pyx_L3_error)
+    __pyx_v_async_ = __Pyx_PyInt_As_int(__pyx_arg_async_); if (unlikely((__pyx_v_async_ == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 499, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.get_copy_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -13888,55 +14285,55 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_copy_data", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":494
+  /* "psycopg_c/pq/pgconn.pyx":500
  * 
  *     def get_copy_data(self, int async_) -> Tuple[int, memoryview]:
  *         cdef char *buffer_ptr = NULL             # <<<<<<<<<<<<<<
  *         cdef int nbytes
  *         nbytes = libpq.PQgetCopyData(self._pgconn_ptr, &buffer_ptr, async_)
  */
   __pyx_v_buffer_ptr = NULL;
 
-  /* "psycopg_c/pq/pgconn.pyx":496
+  /* "psycopg_c/pq/pgconn.pyx":502
  *         cdef char *buffer_ptr = NULL
  *         cdef int nbytes
  *         nbytes = libpq.PQgetCopyData(self._pgconn_ptr, &buffer_ptr, async_)             # <<<<<<<<<<<<<<
  *         if nbytes == -2:
  *             raise e.OperationalError(f"receiving copy data failed: {error_message(self)}")
  */
   __pyx_v_nbytes = PQgetCopyData(__pyx_v_self->_pgconn_ptr, (&__pyx_v_buffer_ptr), __pyx_v_async_);
 
-  /* "psycopg_c/pq/pgconn.pyx":497
+  /* "psycopg_c/pq/pgconn.pyx":503
  *         cdef int nbytes
  *         nbytes = libpq.PQgetCopyData(self._pgconn_ptr, &buffer_ptr, async_)
  *         if nbytes == -2:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"receiving copy data failed: {error_message(self)}")
  *         if buffer_ptr is not NULL:
  */
   __pyx_t_1 = (__pyx_v_nbytes == -2L);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":498
+    /* "psycopg_c/pq/pgconn.pyx":504
  *         nbytes = libpq.PQgetCopyData(self._pgconn_ptr, &buffer_ptr, async_)
  *         if nbytes == -2:
  *             raise e.OperationalError(f"receiving copy data failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  *         if buffer_ptr is not NULL:
  *             data = PyMemoryView_FromObject(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_error_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_error_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -13946,22 +14343,22 @@
         __pyx_t_7 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, ((PyObject *)__pyx_v_self)};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 504, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_3, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_receiving_copy_data_failed, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_receiving_copy_data_failed, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -13973,120 +14370,120 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 504, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 498, __pyx_L1_error)
+    __PYX_ERR(0, 504, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":497
+    /* "psycopg_c/pq/pgconn.pyx":503
  *         cdef int nbytes
  *         nbytes = libpq.PQgetCopyData(self._pgconn_ptr, &buffer_ptr, async_)
  *         if nbytes == -2:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"receiving copy data failed: {error_message(self)}")
  *         if buffer_ptr is not NULL:
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":499
+  /* "psycopg_c/pq/pgconn.pyx":505
  *         if nbytes == -2:
  *             raise e.OperationalError(f"receiving copy data failed: {error_message(self)}")
  *         if buffer_ptr is not NULL:             # <<<<<<<<<<<<<<
  *             data = PyMemoryView_FromObject(
  *                 PQBuffer._from_buffer(<unsigned char *>buffer_ptr, nbytes))
  */
   __pyx_t_1 = (__pyx_v_buffer_ptr != NULL);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":501
+    /* "psycopg_c/pq/pgconn.pyx":507
  *         if buffer_ptr is not NULL:
  *             data = PyMemoryView_FromObject(
  *                 PQBuffer._from_buffer(<unsigned char *>buffer_ptr, nbytes))             # <<<<<<<<<<<<<<
  *             return nbytes, data
  *         else:
  */
-    __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PQBuffer__from_buffer(((unsigned char *)__pyx_v_buffer_ptr), __pyx_v_nbytes)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 501, __pyx_L1_error)
+    __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PQBuffer__from_buffer(((unsigned char *)__pyx_v_buffer_ptr), __pyx_v_nbytes)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 507, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "psycopg_c/pq/pgconn.pyx":500
+    /* "psycopg_c/pq/pgconn.pyx":506
  *             raise e.OperationalError(f"receiving copy data failed: {error_message(self)}")
  *         if buffer_ptr is not NULL:
  *             data = PyMemoryView_FromObject(             # <<<<<<<<<<<<<<
  *                 PQBuffer._from_buffer(<unsigned char *>buffer_ptr, nbytes))
  *             return nbytes, data
  */
-    __pyx_t_4 = PyMemoryView_FromObject(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 500, __pyx_L1_error)
+    __pyx_t_4 = PyMemoryView_FromObject(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_data = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":502
+    /* "psycopg_c/pq/pgconn.pyx":508
  *             data = PyMemoryView_FromObject(
  *                 PQBuffer._from_buffer(<unsigned char *>buffer_ptr, nbytes))
  *             return nbytes, data             # <<<<<<<<<<<<<<
  *         else:
  *             return nbytes, b""  # won't parse it, doesn't really be memoryview
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nbytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 502, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nbytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_data);
     __pyx_t_4 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":499
+    /* "psycopg_c/pq/pgconn.pyx":505
  *         if nbytes == -2:
  *             raise e.OperationalError(f"receiving copy data failed: {error_message(self)}")
  *         if buffer_ptr is not NULL:             # <<<<<<<<<<<<<<
  *             data = PyMemoryView_FromObject(
  *                 PQBuffer._from_buffer(<unsigned char *>buffer_ptr, nbytes))
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":504
+  /* "psycopg_c/pq/pgconn.pyx":510
  *             return nbytes, data
  *         else:
  *             return nbytes, b""  # won't parse it, doesn't really be memoryview             # <<<<<<<<<<<<<<
  * 
  *     def trace(self, fileno: int) -> None:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_nbytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 504, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_nbytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 504, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
-    __Pyx_INCREF(__pyx_kp_b__12);
-    __Pyx_GIVEREF(__pyx_kp_b__12);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_b__12);
+    __Pyx_INCREF(__pyx_kp_b__11);
+    __Pyx_GIVEREF(__pyx_kp_b__11);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_b__11);
     __pyx_t_2 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":493
+  /* "psycopg_c/pq/pgconn.pyx":499
  *         return rv
  * 
  *     def get_copy_data(self, int async_) -> Tuple[int, memoryview]:             # <<<<<<<<<<<<<<
  *         cdef char *buffer_ptr = NULL
  *         cdef int nbytes
  */
 
@@ -14102,15 +14499,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":506
+/* "psycopg_c/pq/pgconn.pyx":512
  *             return nbytes, b""  # won't parse it, doesn't really be memoryview
  * 
  *     def trace(self, fileno: int) -> None:             # <<<<<<<<<<<<<<
  *         if sys.platform != "linux":
  *             raise e.NotSupportedError("currently only supported on Linux")
  */
 
@@ -14121,15 +14518,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("trace (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fileno), (&PyInt_Type), 0, "fileno", 1))) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fileno), (&PyInt_Type), 0, "fileno", 1))) __PYX_ERR(0, 512, __pyx_L1_error)
   __pyx_r = __pyx_pf_9psycopg_c_2pq_6PGconn_68trace(((struct __pyx_obj_9psycopg_c_2pq_PGconn *)__pyx_v_self), ((PyObject*)__pyx_v_fileno));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -14147,40 +14544,40 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("trace", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":507
+  /* "psycopg_c/pq/pgconn.pyx":513
  * 
  *     def trace(self, fileno: int) -> None:
  *         if sys.platform != "linux":             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError("currently only supported on Linux")
  *         stream = fdopen(fileno, b"w")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_sys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_sys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_linux, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_linux, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":508
+    /* "psycopg_c/pq/pgconn.pyx":514
  *     def trace(self, fileno: int) -> None:
  *         if sys.platform != "linux":
  *             raise e.NotSupportedError("currently only supported on Linux")             # <<<<<<<<<<<<<<
  *         stream = fdopen(fileno, b"w")
  *         libpq.PQtrace(self._pgconn_ptr, stream)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_e); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 508, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_e); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_1)) {
@@ -14191,51 +14588,51 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_kp_u_currently_only_supported_on_Linu};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 508, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 508, __pyx_L1_error)
+    __PYX_ERR(0, 514, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":507
+    /* "psycopg_c/pq/pgconn.pyx":513
  * 
  *     def trace(self, fileno: int) -> None:
  *         if sys.platform != "linux":             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError("currently only supported on Linux")
  *         stream = fdopen(fileno, b"w")
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":509
+  /* "psycopg_c/pq/pgconn.pyx":515
  *         if sys.platform != "linux":
  *             raise e.NotSupportedError("currently only supported on Linux")
  *         stream = fdopen(fileno, b"w")             # <<<<<<<<<<<<<<
  *         libpq.PQtrace(self._pgconn_ptr, stream)
  * 
  */
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_fileno); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_fileno); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 515, __pyx_L1_error)
   __pyx_v_stream = fdopen(__pyx_t_5, ((char const *)"w"));
 
-  /* "psycopg_c/pq/pgconn.pyx":510
+  /* "psycopg_c/pq/pgconn.pyx":516
  *             raise e.NotSupportedError("currently only supported on Linux")
  *         stream = fdopen(fileno, b"w")
  *         libpq.PQtrace(self._pgconn_ptr, stream)             # <<<<<<<<<<<<<<
  * 
  *     def set_trace_flags(self, flags: Trace) -> None:
  */
   PQtrace(__pyx_v_self->_pgconn_ptr, __pyx_v_stream);
 
-  /* "psycopg_c/pq/pgconn.pyx":506
+  /* "psycopg_c/pq/pgconn.pyx":512
  *             return nbytes, b""  # won't parse it, doesn't really be memoryview
  * 
  *     def trace(self, fileno: int) -> None:             # <<<<<<<<<<<<<<
  *         if sys.platform != "linux":
  *             raise e.NotSupportedError("currently only supported on Linux")
  */
 
@@ -14250,15 +14647,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":512
+/* "psycopg_c/pq/pgconn.pyx":518
  *         libpq.PQtrace(self._pgconn_ptr, stream)
  * 
  *     def set_trace_flags(self, flags: Trace) -> None:             # <<<<<<<<<<<<<<
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  */
 
@@ -14289,79 +14686,79 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_trace_flags", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":513
+  /* "psycopg_c/pq/pgconn.pyx":519
  * 
  *     def set_trace_flags(self, flags: Trace) -> None:
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQsetTraceFlags requires libpq from PostgreSQL 14,"
  */
   __pyx_t_1 = (PG_VERSION_NUM < 0x222E0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":514
+    /* "psycopg_c/pq/pgconn.pyx":520
  *     def set_trace_flags(self, flags: Trace) -> None:
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(             # <<<<<<<<<<<<<<
  *                 f"PQsetTraceFlags requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 520, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 520, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":515
+    /* "psycopg_c/pq/pgconn.pyx":521
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQsetTraceFlags requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 515, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_PQsetTraceFlags_requires_libpq_f);
     __pyx_t_5 += 51;
     __Pyx_GIVEREF(__pyx_kp_u_PQsetTraceFlags_requires_libpq_f);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_PQsetTraceFlags_requires_libpq_f);
 
-    /* "psycopg_c/pq/pgconn.pyx":516
+    /* "psycopg_c/pq/pgconn.pyx":522
  *             raise e.NotSupportedError(
  *                 f"PQsetTraceFlags requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"             # <<<<<<<<<<<<<<
  *             )
  *         libpq.PQsetTraceFlags(self._pgconn_ptr, flags)
  */
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 516, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_available_instead);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_available_instead);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_available_instead);
 
-    /* "psycopg_c/pq/pgconn.pyx":515
+    /* "psycopg_c/pq/pgconn.pyx":521
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQsetTraceFlags requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 515, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -14373,42 +14770,42 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_7};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 514, __pyx_L1_error)
+    __PYX_ERR(0, 520, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":513
+    /* "psycopg_c/pq/pgconn.pyx":519
  * 
  *     def set_trace_flags(self, flags: Trace) -> None:
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQsetTraceFlags requires libpq from PostgreSQL 14,"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":518
+  /* "psycopg_c/pq/pgconn.pyx":524
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  *         libpq.PQsetTraceFlags(self._pgconn_ptr, flags)             # <<<<<<<<<<<<<<
  * 
  *     def untrace(self) -> None:
  */
-  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_flags); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_flags); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 524, __pyx_L1_error)
   PQsetTraceFlags(__pyx_v_self->_pgconn_ptr, __pyx_t_8);
 
-  /* "psycopg_c/pq/pgconn.pyx":512
+  /* "psycopg_c/pq/pgconn.pyx":518
  *         libpq.PQtrace(self._pgconn_ptr, stream)
  * 
  *     def set_trace_flags(self, flags: Trace) -> None:             # <<<<<<<<<<<<<<
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  */
 
@@ -14424,15 +14821,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":520
+/* "psycopg_c/pq/pgconn.pyx":526
  *         libpq.PQsetTraceFlags(self._pgconn_ptr, flags)
  * 
  *     def untrace(self) -> None:             # <<<<<<<<<<<<<<
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  */
 
@@ -14452,39 +14849,39 @@
 }
 
 static PyObject *__pyx_pf_9psycopg_c_2pq_6PGconn_72untrace(struct __pyx_obj_9psycopg_c_2pq_PGconn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("untrace", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":521
+  /* "psycopg_c/pq/pgconn.pyx":527
  * 
  *     def untrace(self) -> None:
  *         libpq.PQuntrace(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  * 
  *     def encrypt_password(
  */
   PQuntrace(__pyx_v_self->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":520
+  /* "psycopg_c/pq/pgconn.pyx":526
  *         libpq.PQsetTraceFlags(self._pgconn_ptr, flags)
  * 
  *     def untrace(self) -> None:             # <<<<<<<<<<<<<<
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":523
+/* "psycopg_c/pq/pgconn.pyx":529
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  *     def encrypt_password(             # <<<<<<<<<<<<<<
  *         self, const char *passwd, const char *user, algorithm = None
  *     ) -> bytes:
  */
 
@@ -14521,15 +14918,15 @@
     #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_passwd,&__pyx_n_s_user,&__pyx_n_s_algorithm,0};
     #else
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_passwd,&__pyx_n_s_user,&__pyx_n_s_algorithm,0};
     #endif
     PyObject* values[3] = {0,0,0};
 
-    /* "psycopg_c/pq/pgconn.pyx":524
+    /* "psycopg_c/pq/pgconn.pyx":530
  * 
  *     def encrypt_password(
  *         self, const char *passwd, const char *user, algorithm = None             # <<<<<<<<<<<<<<
  *     ) -> bytes:
  *         if libpq.PG_VERSION_NUM < 100000:
  */
     values[2] = ((PyObject *)Py_None);
@@ -14545,60 +14942,60 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_passwd)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 523, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_user)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 523, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("encrypt_password", 0, 2, 3, 1); __PYX_ERR(0, 523, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encrypt_password", 0, 2, 3, 1); __PYX_ERR(0, 529, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_algorithm);
           if (value) { values[2] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 523, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encrypt_password") < 0)) __PYX_ERR(0, 523, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encrypt_password") < 0)) __PYX_ERR(0, 529, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_passwd = __Pyx_PyObject_AsString(values[0]); if (unlikely((!__pyx_v_passwd) && PyErr_Occurred())) __PYX_ERR(0, 524, __pyx_L3_error)
-    __pyx_v_user = __Pyx_PyObject_AsString(values[1]); if (unlikely((!__pyx_v_user) && PyErr_Occurred())) __PYX_ERR(0, 524, __pyx_L3_error)
+    __pyx_v_passwd = __Pyx_PyObject_AsString(values[0]); if (unlikely((!__pyx_v_passwd) && PyErr_Occurred())) __PYX_ERR(0, 530, __pyx_L3_error)
+    __pyx_v_user = __Pyx_PyObject_AsString(values[1]); if (unlikely((!__pyx_v_user) && PyErr_Occurred())) __PYX_ERR(0, 530, __pyx_L3_error)
     __pyx_v_algorithm = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encrypt_password", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 523, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encrypt_password", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 529, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.encrypt_password", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9psycopg_c_2pq_6PGconn_74encrypt_password(((struct __pyx_obj_9psycopg_c_2pq_PGconn *)__pyx_v_self), __pyx_v_passwd, __pyx_v_user, __pyx_v_algorithm);
 
-  /* "psycopg_c/pq/pgconn.pyx":523
+  /* "psycopg_c/pq/pgconn.pyx":529
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  *     def encrypt_password(             # <<<<<<<<<<<<<<
  *         self, const char *passwd, const char *user, algorithm = None
  *     ) -> bytes:
  */
 
@@ -14624,79 +15021,79 @@
   char const *__pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encrypt_password", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":526
+  /* "psycopg_c/pq/pgconn.pyx":532
  *         self, const char *passwd, const char *user, algorithm = None
  *     ) -> bytes:
  *         if libpq.PG_VERSION_NUM < 100000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQencryptPasswordConn requires libpq from PostgreSQL 10,"
  */
   __pyx_t_1 = (PG_VERSION_NUM < 0x186A0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":527
+    /* "psycopg_c/pq/pgconn.pyx":533
  *     ) -> bytes:
  *         if libpq.PG_VERSION_NUM < 100000:
  *             raise e.NotSupportedError(             # <<<<<<<<<<<<<<
  *                 f"PQencryptPasswordConn requires libpq from PostgreSQL 10,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 527, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 533, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 527, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 533, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":528
+    /* "psycopg_c/pq/pgconn.pyx":534
  *         if libpq.PG_VERSION_NUM < 100000:
  *             raise e.NotSupportedError(
  *                 f"PQencryptPasswordConn requires libpq from PostgreSQL 10,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 528, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 534, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_PQencryptPasswordConn_requires_l);
     __pyx_t_5 += 57;
     __Pyx_GIVEREF(__pyx_kp_u_PQencryptPasswordConn_requires_l);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_PQencryptPasswordConn_requires_l);
 
-    /* "psycopg_c/pq/pgconn.pyx":529
+    /* "psycopg_c/pq/pgconn.pyx":535
  *             raise e.NotSupportedError(
  *                 f"PQencryptPasswordConn requires libpq from PostgreSQL 10,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 535, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_available_instead);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_available_instead);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_available_instead);
 
-    /* "psycopg_c/pq/pgconn.pyx":528
+    /* "psycopg_c/pq/pgconn.pyx":534
  *         if libpq.PG_VERSION_NUM < 100000:
  *             raise e.NotSupportedError(
  *                 f"PQencryptPasswordConn requires libpq from PostgreSQL 10,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 528, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 534, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -14708,109 +15105,109 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_7};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 527, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 533, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 527, __pyx_L1_error)
+    __PYX_ERR(0, 533, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":526
+    /* "psycopg_c/pq/pgconn.pyx":532
  *         self, const char *passwd, const char *user, algorithm = None
  *     ) -> bytes:
  *         if libpq.PG_VERSION_NUM < 100000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQencryptPasswordConn requires libpq from PostgreSQL 10,"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":533
+  /* "psycopg_c/pq/pgconn.pyx":539
  * 
  *         cdef char *out
  *         cdef const char *calgo = NULL             # <<<<<<<<<<<<<<
  *         if algorithm:
  *             calgo = algorithm
  */
   __pyx_v_calgo = NULL;
 
-  /* "psycopg_c/pq/pgconn.pyx":534
+  /* "psycopg_c/pq/pgconn.pyx":540
  *         cdef char *out
  *         cdef const char *calgo = NULL
  *         if algorithm:             # <<<<<<<<<<<<<<
  *             calgo = algorithm
  *         out = libpq.PQencryptPasswordConn(self._pgconn_ptr, passwd, user, calgo)
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_algorithm); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_algorithm); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 540, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":535
+    /* "psycopg_c/pq/pgconn.pyx":541
  *         cdef const char *calgo = NULL
  *         if algorithm:
  *             calgo = algorithm             # <<<<<<<<<<<<<<
  *         out = libpq.PQencryptPasswordConn(self._pgconn_ptr, passwd, user, calgo)
  *         if not out:
  */
-    __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_algorithm); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 535, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_algorithm); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 541, __pyx_L1_error)
     __pyx_v_calgo = __pyx_t_9;
 
-    /* "psycopg_c/pq/pgconn.pyx":534
+    /* "psycopg_c/pq/pgconn.pyx":540
  *         cdef char *out
  *         cdef const char *calgo = NULL
  *         if algorithm:             # <<<<<<<<<<<<<<
  *             calgo = algorithm
  *         out = libpq.PQencryptPasswordConn(self._pgconn_ptr, passwd, user, calgo)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":536
+  /* "psycopg_c/pq/pgconn.pyx":542
  *         if algorithm:
  *             calgo = algorithm
  *         out = libpq.PQencryptPasswordConn(self._pgconn_ptr, passwd, user, calgo)             # <<<<<<<<<<<<<<
  *         if not out:
  *             raise e.OperationalError(
  */
   __pyx_v_out = PQencryptPasswordConn(__pyx_v_self->_pgconn_ptr, __pyx_v_passwd, __pyx_v_user, __pyx_v_calgo);
 
-  /* "psycopg_c/pq/pgconn.pyx":537
+  /* "psycopg_c/pq/pgconn.pyx":543
  *             calgo = algorithm
  *         out = libpq.PQencryptPasswordConn(self._pgconn_ptr, passwd, user, calgo)
  *         if not out:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(
  *                 f"password encryption failed: {error_message(self)}"
  */
   __pyx_t_1 = (!(__pyx_v_out != 0));
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":538
+    /* "psycopg_c/pq/pgconn.pyx":544
  *         out = libpq.PQencryptPasswordConn(self._pgconn_ptr, passwd, user, calgo)
  *         if not out:
  *             raise e.OperationalError(             # <<<<<<<<<<<<<<
  *                 f"password encryption failed: {error_message(self)}"
  *             )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":539
+    /* "psycopg_c/pq/pgconn.pyx":545
  *         if not out:
  *             raise e.OperationalError(
  *                 f"password encryption failed: {error_message(self)}"             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_error_message); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 539, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_error_message); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_10 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -14820,22 +15217,22 @@
         __pyx_t_8 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, ((PyObject *)__pyx_v_self)};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 539, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 545, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 539, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_password_encryption_failed, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 539, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_password_encryption_failed, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_3)) {
@@ -14847,68 +15244,68 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 538, __pyx_L1_error)
+    __PYX_ERR(0, 544, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":537
+    /* "psycopg_c/pq/pgconn.pyx":543
  *             calgo = algorithm
  *         out = libpq.PQencryptPasswordConn(self._pgconn_ptr, passwd, user, calgo)
  *         if not out:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(
  *                 f"password encryption failed: {error_message(self)}"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":542
+  /* "psycopg_c/pq/pgconn.pyx":548
  *             )
  * 
  *         rv = bytes(out)             # <<<<<<<<<<<<<<
  *         libpq.PQfreemem(out)
  *         return rv
  */
-  __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_out); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_out); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_rv = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "psycopg_c/pq/pgconn.pyx":543
+  /* "psycopg_c/pq/pgconn.pyx":549
  * 
  *         rv = bytes(out)
  *         libpq.PQfreemem(out)             # <<<<<<<<<<<<<<
  *         return rv
  * 
  */
   PQfreemem(__pyx_v_out);
 
-  /* "psycopg_c/pq/pgconn.pyx":544
+  /* "psycopg_c/pq/pgconn.pyx":550
  *         rv = bytes(out)
  *         libpq.PQfreemem(out)
  *         return rv             # <<<<<<<<<<<<<<
  * 
  *     def make_empty_result(self, int exec_status) -> PGresult:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_rv);
   __pyx_r = __pyx_v_rv;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":523
+  /* "psycopg_c/pq/pgconn.pyx":529
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  *     def encrypt_password(             # <<<<<<<<<<<<<<
  *         self, const char *passwd, const char *user, algorithm = None
  *     ) -> bytes:
  */
 
@@ -14924,15 +15321,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_rv);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":546
+/* "psycopg_c/pq/pgconn.pyx":552
  *         return rv
  * 
  *     def make_empty_result(self, int exec_status) -> PGresult:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *rv = libpq.PQmakeEmptyPGresult(
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  */
 
@@ -14945,15 +15342,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   struct __pyx_obj_9psycopg_c_2pq_PGresult *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("make_empty_result (wrapper)", 0);
   assert(__pyx_arg_exec_status); {
-    __pyx_v_exec_status = __Pyx_PyInt_As_int(__pyx_arg_exec_status); if (unlikely((__pyx_v_exec_status == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 546, __pyx_L3_error)
+    __pyx_v_exec_status = __Pyx_PyInt_As_int(__pyx_arg_exec_status); if (unlikely((__pyx_v_exec_status == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 552, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.make_empty_result", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -14971,70 +15368,70 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_empty_result", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":547
+  /* "psycopg_c/pq/pgconn.pyx":553
  * 
  *     def make_empty_result(self, int exec_status) -> PGresult:
  *         cdef libpq.PGresult *rv = libpq.PQmakeEmptyPGresult(             # <<<<<<<<<<<<<<
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  *         if not rv:
  */
   __pyx_v_rv = PQmakeEmptyPGresult(__pyx_v_self->_pgconn_ptr, ((ExecStatusType)__pyx_v_exec_status));
 
-  /* "psycopg_c/pq/pgconn.pyx":549
+  /* "psycopg_c/pq/pgconn.pyx":555
  *         cdef libpq.PGresult *rv = libpq.PQmakeEmptyPGresult(
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  *         if not rv:             # <<<<<<<<<<<<<<
  *             raise MemoryError("couldn't allocate empty PGresult")
  *         return PGresult._from_ptr(rv)
  */
   __pyx_t_1 = (!(__pyx_v_rv != 0));
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":550
+    /* "psycopg_c/pq/pgconn.pyx":556
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  *         if not rv:
  *             raise MemoryError("couldn't allocate empty PGresult")             # <<<<<<<<<<<<<<
  *         return PGresult._from_ptr(rv)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 556, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 550, __pyx_L1_error)
+    __PYX_ERR(0, 556, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":549
+    /* "psycopg_c/pq/pgconn.pyx":555
  *         cdef libpq.PGresult *rv = libpq.PQmakeEmptyPGresult(
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  *         if not rv:             # <<<<<<<<<<<<<<
  *             raise MemoryError("couldn't allocate empty PGresult")
  *         return PGresult._from_ptr(rv)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":551
+  /* "psycopg_c/pq/pgconn.pyx":557
  *         if not rv:
  *             raise MemoryError("couldn't allocate empty PGresult")
  *         return PGresult._from_ptr(rv)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(__pyx_v_rv)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = ((struct __pyx_obj_9psycopg_c_2pq_PGresult *)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":546
+  /* "psycopg_c/pq/pgconn.pyx":552
  *         return rv
  * 
  *     def make_empty_result(self, int exec_status) -> PGresult:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *rv = libpq.PQmakeEmptyPGresult(
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  */
 
@@ -15045,15 +15442,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":553
+/* "psycopg_c/pq/pgconn.pyx":559
  *         return PGresult._from_ptr(rv)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def pipeline_status(self) -> int:
  *         """The current pipeline mode status.
  */
 
@@ -15078,71 +15475,71 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":559
+  /* "psycopg_c/pq/pgconn.pyx":565
  *         For libpq < 14.0, always return 0 (PQ_PIPELINE_OFF).
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             return libpq.PQ_PIPELINE_OFF
  *         cdef int status = libpq.PQpipelineStatus(self._pgconn_ptr)
  */
   __pyx_t_1 = (PG_VERSION_NUM < 0x222E0);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":560
+    /* "psycopg_c/pq/pgconn.pyx":566
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:
  *             return libpq.PQ_PIPELINE_OFF             # <<<<<<<<<<<<<<
  *         cdef int status = libpq.PQpipelineStatus(self._pgconn_ptr)
  *         return status
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_PGpipelineStatus(PQ_PIPELINE_OFF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_PGpipelineStatus(PQ_PIPELINE_OFF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":559
+    /* "psycopg_c/pq/pgconn.pyx":565
  *         For libpq < 14.0, always return 0 (PQ_PIPELINE_OFF).
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             return libpq.PQ_PIPELINE_OFF
  *         cdef int status = libpq.PQpipelineStatus(self._pgconn_ptr)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":561
+  /* "psycopg_c/pq/pgconn.pyx":567
  *         if libpq.PG_VERSION_NUM < 140000:
  *             return libpq.PQ_PIPELINE_OFF
  *         cdef int status = libpq.PQpipelineStatus(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         return status
  * 
  */
   __pyx_v_status = PQpipelineStatus(__pyx_v_self->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":562
+  /* "psycopg_c/pq/pgconn.pyx":568
  *             return libpq.PQ_PIPELINE_OFF
  *         cdef int status = libpq.PQpipelineStatus(self._pgconn_ptr)
  *         return status             # <<<<<<<<<<<<<<
  * 
  *     def enter_pipeline_mode(self) -> None:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":553
+  /* "psycopg_c/pq/pgconn.pyx":559
  *         return PGresult._from_ptr(rv)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def pipeline_status(self) -> int:
  *         """The current pipeline mode status.
  */
 
@@ -15153,15 +15550,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":564
+/* "psycopg_c/pq/pgconn.pyx":570
  *         return status
  * 
  *     def enter_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Enter pipeline mode.
  * 
  */
 
@@ -15193,79 +15590,79 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("enter_pipeline_mode", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":570
+  /* "psycopg_c/pq/pgconn.pyx":576
  *             mode.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQenterPipelineMode requires libpq from PostgreSQL 14,"
  */
   __pyx_t_1 = (PG_VERSION_NUM < 0x222E0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":571
+    /* "psycopg_c/pq/pgconn.pyx":577
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(             # <<<<<<<<<<<<<<
  *                 f"PQenterPipelineMode requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 571, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 571, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":572
+    /* "psycopg_c/pq/pgconn.pyx":578
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQenterPipelineMode requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 572, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_PQenterPipelineMode_requires_lib);
     __pyx_t_5 += 55;
     __Pyx_GIVEREF(__pyx_kp_u_PQenterPipelineMode_requires_lib);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_PQenterPipelineMode_requires_lib);
 
-    /* "psycopg_c/pq/pgconn.pyx":573
+    /* "psycopg_c/pq/pgconn.pyx":579
  *             raise e.NotSupportedError(
  *                 f"PQenterPipelineMode requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"             # <<<<<<<<<<<<<<
  *             )
  *         if libpq.PQenterPipelineMode(self._pgconn_ptr) != 1:
  */
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 573, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_available_instead);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_available_instead);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_available_instead);
 
-    /* "psycopg_c/pq/pgconn.pyx":572
+    /* "psycopg_c/pq/pgconn.pyx":578
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQenterPipelineMode requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 572, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -15277,51 +15674,51 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_7};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 571, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 571, __pyx_L1_error)
+    __PYX_ERR(0, 577, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":570
+    /* "psycopg_c/pq/pgconn.pyx":576
  *             mode.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQenterPipelineMode requires libpq from PostgreSQL 14,"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":575
+  /* "psycopg_c/pq/pgconn.pyx":581
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  *         if libpq.PQenterPipelineMode(self._pgconn_ptr) != 1:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("failed to enter pipeline mode")
  * 
  */
   __pyx_t_1 = (PQenterPipelineMode(__pyx_v_self->_pgconn_ptr) != 1);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":576
+    /* "psycopg_c/pq/pgconn.pyx":582
  *             )
  *         if libpq.PQenterPipelineMode(self._pgconn_ptr) != 1:
  *             raise e.OperationalError("failed to enter pipeline mode")             # <<<<<<<<<<<<<<
  * 
  *     def exit_pipeline_mode(self) -> None:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 576, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 582, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 576, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 582, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_4)) {
@@ -15332,32 +15729,32 @@
         __pyx_t_8 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_failed_to_enter_pipeline_mode};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 576, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 576, __pyx_L1_error)
+    __PYX_ERR(0, 582, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":575
+    /* "psycopg_c/pq/pgconn.pyx":581
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  *         if libpq.PQenterPipelineMode(self._pgconn_ptr) != 1:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("failed to enter pipeline mode")
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":564
+  /* "psycopg_c/pq/pgconn.pyx":570
  *         return status
  * 
  *     def enter_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Enter pipeline mode.
  * 
  */
 
@@ -15373,15 +15770,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":578
+/* "psycopg_c/pq/pgconn.pyx":584
  *             raise e.OperationalError("failed to enter pipeline mode")
  * 
  *     def exit_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Exit pipeline mode.
  * 
  */
 
@@ -15414,79 +15811,79 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exit_pipeline_mode", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":584
+  /* "psycopg_c/pq/pgconn.pyx":590
  *             mode.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQexitPipelineMode requires libpq from PostgreSQL 14,"
  */
   __pyx_t_1 = (PG_VERSION_NUM < 0x222E0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":585
+    /* "psycopg_c/pq/pgconn.pyx":591
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(             # <<<<<<<<<<<<<<
  *                 f"PQexitPipelineMode requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 585, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 585, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":586
+    /* "psycopg_c/pq/pgconn.pyx":592
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQexitPipelineMode requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_PQexitPipelineMode_requires_libp);
     __pyx_t_5 += 54;
     __Pyx_GIVEREF(__pyx_kp_u_PQexitPipelineMode_requires_libp);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_PQexitPipelineMode_requires_libp);
 
-    /* "psycopg_c/pq/pgconn.pyx":587
+    /* "psycopg_c/pq/pgconn.pyx":593
  *             raise e.NotSupportedError(
  *                 f"PQexitPipelineMode requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"             # <<<<<<<<<<<<<<
  *             )
  *         if libpq.PQexitPipelineMode(self._pgconn_ptr) != 1:
  */
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_available_instead);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_available_instead);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_available_instead);
 
-    /* "psycopg_c/pq/pgconn.pyx":586
+    /* "psycopg_c/pq/pgconn.pyx":592
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQexitPipelineMode requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 586, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -15498,54 +15895,54 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_7};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 585, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 585, __pyx_L1_error)
+    __PYX_ERR(0, 591, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":584
+    /* "psycopg_c/pq/pgconn.pyx":590
  *             mode.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQexitPipelineMode requires libpq from PostgreSQL 14,"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":589
+  /* "psycopg_c/pq/pgconn.pyx":595
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  *         if libpq.PQexitPipelineMode(self._pgconn_ptr) != 1:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(error_message(self))
  * 
  */
   __pyx_t_1 = (PQexitPipelineMode(__pyx_v_self->_pgconn_ptr) != 1);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":590
+    /* "psycopg_c/pq/pgconn.pyx":596
  *             )
  *         if libpq.PQexitPipelineMode(self._pgconn_ptr) != 1:
  *             raise e.OperationalError(error_message(self))             # <<<<<<<<<<<<<<
  * 
  *     def pipeline_sync(self) -> None:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 590, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 590, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 596, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_error_message); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 590, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_error_message); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_9 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -15555,15 +15952,15 @@
         __pyx_t_8 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, ((PyObject *)__pyx_v_self)};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 590, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
@@ -15576,32 +15973,32 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 596, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 590, __pyx_L1_error)
+    __PYX_ERR(0, 596, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":589
+    /* "psycopg_c/pq/pgconn.pyx":595
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  *         if libpq.PQexitPipelineMode(self._pgconn_ptr) != 1:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(error_message(self))
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":578
+  /* "psycopg_c/pq/pgconn.pyx":584
  *             raise e.OperationalError("failed to enter pipeline mode")
  * 
  *     def exit_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Exit pipeline mode.
  * 
  */
 
@@ -15618,15 +16015,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":592
+/* "psycopg_c/pq/pgconn.pyx":598
  *             raise e.OperationalError(error_message(self))
  * 
  *     def pipeline_sync(self) -> None:             # <<<<<<<<<<<<<<
  *         """Mark a synchronization point in a pipeline.
  * 
  */
 
@@ -15659,79 +16056,79 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pipeline_sync", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":598
+  /* "psycopg_c/pq/pgconn.pyx":604
  *             or if sync failed.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQpipelineSync requires libpq from PostgreSQL 14,"
  */
   __pyx_t_1 = (PG_VERSION_NUM < 0x222E0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":599
+    /* "psycopg_c/pq/pgconn.pyx":605
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(             # <<<<<<<<<<<<<<
  *                 f"PQpipelineSync requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 599, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":600
+    /* "psycopg_c/pq/pgconn.pyx":606
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQpipelineSync requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_PQpipelineSync_requires_libpq_fr);
     __pyx_t_5 += 50;
     __Pyx_GIVEREF(__pyx_kp_u_PQpipelineSync_requires_libpq_fr);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_PQpipelineSync_requires_libpq_fr);
 
-    /* "psycopg_c/pq/pgconn.pyx":601
+    /* "psycopg_c/pq/pgconn.pyx":607
  *             raise e.NotSupportedError(
  *                 f"PQpipelineSync requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"             # <<<<<<<<<<<<<<
  *             )
  *         rv = libpq.PQpipelineSync(self._pgconn_ptr)
  */
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 601, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 607, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_available_instead);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_available_instead);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_available_instead);
 
-    /* "psycopg_c/pq/pgconn.pyx":600
+    /* "psycopg_c/pq/pgconn.pyx":606
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQpipelineSync requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -15743,60 +16140,60 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_7};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 599, __pyx_L1_error)
+    __PYX_ERR(0, 605, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":598
+    /* "psycopg_c/pq/pgconn.pyx":604
  *             or if sync failed.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQpipelineSync requires libpq from PostgreSQL 14,"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":603
+  /* "psycopg_c/pq/pgconn.pyx":609
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  *         rv = libpq.PQpipelineSync(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         if rv == 0:
  *             raise e.OperationalError("connection not in pipeline mode")
  */
   __pyx_v_rv = PQpipelineSync(__pyx_v_self->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":604
+  /* "psycopg_c/pq/pgconn.pyx":610
  *             )
  *         rv = libpq.PQpipelineSync(self._pgconn_ptr)
  *         if rv == 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("connection not in pipeline mode")
  *         if rv != 1:
  */
   __pyx_t_1 = (__pyx_v_rv == 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":605
+    /* "psycopg_c/pq/pgconn.pyx":611
  *         rv = libpq.PQpipelineSync(self._pgconn_ptr)
  *         if rv == 0:
  *             raise e.OperationalError("connection not in pipeline mode")             # <<<<<<<<<<<<<<
  *         if rv != 1:
  *             raise e.OperationalError("failed to sync pipeline")
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_4)) {
@@ -15807,51 +16204,51 @@
         __pyx_t_8 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_connection_not_in_pipeline_mode};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 611, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 605, __pyx_L1_error)
+    __PYX_ERR(0, 611, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":604
+    /* "psycopg_c/pq/pgconn.pyx":610
  *             )
  *         rv = libpq.PQpipelineSync(self._pgconn_ptr)
  *         if rv == 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("connection not in pipeline mode")
  *         if rv != 1:
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":606
+  /* "psycopg_c/pq/pgconn.pyx":612
  *         if rv == 0:
  *             raise e.OperationalError("connection not in pipeline mode")
  *         if rv != 1:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("failed to sync pipeline")
  * 
  */
   __pyx_t_1 = (__pyx_v_rv != 1);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":607
+    /* "psycopg_c/pq/pgconn.pyx":613
  *             raise e.OperationalError("connection not in pipeline mode")
  *         if rv != 1:
  *             raise e.OperationalError("failed to sync pipeline")             # <<<<<<<<<<<<<<
  * 
  *     def send_flush_request(self) -> None:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_e); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_e); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
@@ -15862,32 +16259,32 @@
         __pyx_t_8 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_u_failed_to_sync_pipeline};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 607, __pyx_L1_error)
+    __PYX_ERR(0, 613, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":606
+    /* "psycopg_c/pq/pgconn.pyx":612
  *         if rv == 0:
  *             raise e.OperationalError("connection not in pipeline mode")
  *         if rv != 1:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError("failed to sync pipeline")
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":592
+  /* "psycopg_c/pq/pgconn.pyx":598
  *             raise e.OperationalError(error_message(self))
  * 
  *     def pipeline_sync(self) -> None:             # <<<<<<<<<<<<<<
  *         """Mark a synchronization point in a pipeline.
  * 
  */
 
@@ -15903,15 +16300,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":609
+/* "psycopg_c/pq/pgconn.pyx":615
  *             raise e.OperationalError("failed to sync pipeline")
  * 
  *     def send_flush_request(self) -> None:             # <<<<<<<<<<<<<<
  *         """Sends a request for the server to flush its output buffer.
  * 
  */
 
@@ -15945,79 +16342,79 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_flush_request", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":614
+  /* "psycopg_c/pq/pgconn.pyx":620
  *         :raises ~e.OperationalError: if the flush request failed.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQsendFlushRequest requires libpq from PostgreSQL 14,"
  */
   __pyx_t_1 = (PG_VERSION_NUM < 0x222E0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":615
+    /* "psycopg_c/pq/pgconn.pyx":621
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(             # <<<<<<<<<<<<<<
  *                 f"PQsendFlushRequest requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 615, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_NotSupportedError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":616
+    /* "psycopg_c/pq/pgconn.pyx":622
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQsendFlushRequest requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 622, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_PQsendFlushRequest_requires_libp);
     __pyx_t_5 += 54;
     __Pyx_GIVEREF(__pyx_kp_u_PQsendFlushRequest_requires_libp);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_PQsendFlushRequest_requires_libp);
 
-    /* "psycopg_c/pq/pgconn.pyx":617
+    /* "psycopg_c/pq/pgconn.pyx":623
  *             raise e.NotSupportedError(
  *                 f"PQsendFlushRequest requires libpq from PostgreSQL 14,"
  *                 f" {libpq.PG_VERSION_NUM} available instead"             # <<<<<<<<<<<<<<
  *             )
  *         cdef int rv = libpq.PQsendFlushRequest(self._pgconn_ptr)
  */
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 617, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(PG_VERSION_NUM, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 623, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_available_instead);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_available_instead);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_available_instead);
 
-    /* "psycopg_c/pq/pgconn.pyx":616
+    /* "psycopg_c/pq/pgconn.pyx":622
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  *                 f"PQsendFlushRequest requires libpq from PostgreSQL 14,"             # <<<<<<<<<<<<<<
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 622, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -16029,63 +16426,63 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_7};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 615, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 615, __pyx_L1_error)
+    __PYX_ERR(0, 621, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":614
+    /* "psycopg_c/pq/pgconn.pyx":620
  *         :raises ~e.OperationalError: if the flush request failed.
  *         """
  *         if libpq.PG_VERSION_NUM < 140000:             # <<<<<<<<<<<<<<
  *             raise e.NotSupportedError(
  *                 f"PQsendFlushRequest requires libpq from PostgreSQL 14,"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":619
+  /* "psycopg_c/pq/pgconn.pyx":625
  *                 f" {libpq.PG_VERSION_NUM} available instead"
  *             )
  *         cdef int rv = libpq.PQsendFlushRequest(self._pgconn_ptr)             # <<<<<<<<<<<<<<
  *         if rv == 0:
  *             raise e.OperationalError(f"flush request failed: {error_message(self)}")
  */
   __pyx_v_rv = PQsendFlushRequest(__pyx_v_self->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":620
+  /* "psycopg_c/pq/pgconn.pyx":626
  *             )
  *         cdef int rv = libpq.PQsendFlushRequest(self._pgconn_ptr)
  *         if rv == 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"flush request failed: {error_message(self)}")
  * 
  */
   __pyx_t_1 = (__pyx_v_rv == 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":621
+    /* "psycopg_c/pq/pgconn.pyx":627
  *         cdef int rv = libpq.PQsendFlushRequest(self._pgconn_ptr)
  *         if rv == 0:
  *             raise e.OperationalError(f"flush request failed: {error_message(self)}")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_e); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_error_message); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_error_message); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_9 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -16095,22 +16492,22 @@
         __pyx_t_8 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, ((PyObject *)__pyx_v_self)};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_flush_request_failed, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_kp_u_flush_request_failed, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 627, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_3)) {
@@ -16122,32 +16519,32 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 621, __pyx_L1_error)
+    __PYX_ERR(0, 627, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":620
+    /* "psycopg_c/pq/pgconn.pyx":626
  *             )
  *         cdef int rv = libpq.PQsendFlushRequest(self._pgconn_ptr)
  *         if rv == 0:             # <<<<<<<<<<<<<<
  *             raise e.OperationalError(f"flush request failed: {error_message(self)}")
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":609
+  /* "psycopg_c/pq/pgconn.pyx":615
  *             raise e.OperationalError("failed to sync pipeline")
  * 
  *     def send_flush_request(self) -> None:             # <<<<<<<<<<<<<<
  *         """Sends a request for the server to flush its output buffer.
  * 
  */
 
@@ -16467,15 +16864,15 @@
   __Pyx_AddTraceback("psycopg_c.pq.PGconn.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":624
+/* "psycopg_c/pq/pgconn.pyx":630
  * 
  * 
  * cdef int _ensure_pgconn(PGconn pgconn) except 0:             # <<<<<<<<<<<<<<
  *     if pgconn._pgconn_ptr is not NULL:
  *         return 1
  */
 
@@ -16488,53 +16885,53 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_ensure_pgconn", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":625
+  /* "psycopg_c/pq/pgconn.pyx":631
  * 
  * cdef int _ensure_pgconn(PGconn pgconn) except 0:
  *     if pgconn._pgconn_ptr is not NULL:             # <<<<<<<<<<<<<<
  *         return 1
  * 
  */
   __pyx_t_1 = (__pyx_v_pgconn->_pgconn_ptr != NULL);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":626
+    /* "psycopg_c/pq/pgconn.pyx":632
  * cdef int _ensure_pgconn(PGconn pgconn) except 0:
  *     if pgconn._pgconn_ptr is not NULL:
  *         return 1             # <<<<<<<<<<<<<<
  * 
  *     raise e.OperationalError("the connection is closed")
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":625
+    /* "psycopg_c/pq/pgconn.pyx":631
  * 
  * cdef int _ensure_pgconn(PGconn pgconn) except 0:
  *     if pgconn._pgconn_ptr is not NULL:             # <<<<<<<<<<<<<<
  *         return 1
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":628
+  /* "psycopg_c/pq/pgconn.pyx":634
  *         return 1
  * 
  *     raise e.OperationalError("the connection is closed")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_OperationalError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
@@ -16545,23 +16942,23 @@
       __pyx_t_5 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_the_connection_is_closed};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_Raise(__pyx_t_2, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __PYX_ERR(0, 628, __pyx_L1_error)
+  __PYX_ERR(0, 634, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":624
+  /* "psycopg_c/pq/pgconn.pyx":630
  * 
  * 
  * cdef int _ensure_pgconn(PGconn pgconn) except 0:             # <<<<<<<<<<<<<<
  *     if pgconn._pgconn_ptr is not NULL:
  *         return 1
  */
 
@@ -16573,15 +16970,15 @@
   __Pyx_AddTraceback("psycopg_c.pq._ensure_pgconn", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":631
+/* "psycopg_c/pq/pgconn.pyx":637
  * 
  * 
  * cdef char *_call_bytes(PGconn pgconn, conn_bytes_f func) except NULL:             # <<<<<<<<<<<<<<
  *     """
  *     Call one of the pgconn libpq functions returning a bytes pointer.
  */
 
@@ -16592,83 +16989,83 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_call_bytes", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":635
+  /* "psycopg_c/pq/pgconn.pyx":641
  *     Call one of the pgconn libpq functions returning a bytes pointer.
  *     """
  *     if not _ensure_pgconn(pgconn):             # <<<<<<<<<<<<<<
  *         return NULL
  *     cdef char *rv = func(pgconn._pgconn_ptr)
  */
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_pgconn); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_pgconn); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 641, __pyx_L1_error)
   __pyx_t_2 = (!(__pyx_t_1 != 0));
   if (__pyx_t_2) {
 
-    /* "psycopg_c/pq/pgconn.pyx":636
+    /* "psycopg_c/pq/pgconn.pyx":642
  *     """
  *     if not _ensure_pgconn(pgconn):
  *         return NULL             # <<<<<<<<<<<<<<
  *     cdef char *rv = func(pgconn._pgconn_ptr)
  *     assert rv is not NULL
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":635
+    /* "psycopg_c/pq/pgconn.pyx":641
  *     Call one of the pgconn libpq functions returning a bytes pointer.
  *     """
  *     if not _ensure_pgconn(pgconn):             # <<<<<<<<<<<<<<
  *         return NULL
  *     cdef char *rv = func(pgconn._pgconn_ptr)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":637
+  /* "psycopg_c/pq/pgconn.pyx":643
  *     if not _ensure_pgconn(pgconn):
  *         return NULL
  *     cdef char *rv = func(pgconn._pgconn_ptr)             # <<<<<<<<<<<<<<
  *     assert rv is not NULL
  *     return rv
  */
   __pyx_v_rv = __pyx_v_func(__pyx_v_pgconn->_pgconn_ptr);
 
-  /* "psycopg_c/pq/pgconn.pyx":638
+  /* "psycopg_c/pq/pgconn.pyx":644
  *         return NULL
  *     cdef char *rv = func(pgconn._pgconn_ptr)
  *     assert rv is not NULL             # <<<<<<<<<<<<<<
  *     return rv
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     __pyx_t_2 = (__pyx_v_rv != NULL);
     if (unlikely(!__pyx_t_2)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 638, __pyx_L1_error)
+      __PYX_ERR(0, 644, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 638, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 644, __pyx_L1_error)
   #endif
 
-  /* "psycopg_c/pq/pgconn.pyx":639
+  /* "psycopg_c/pq/pgconn.pyx":645
  *     cdef char *rv = func(pgconn._pgconn_ptr)
  *     assert rv is not NULL
  *     return rv             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_rv;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":631
+  /* "psycopg_c/pq/pgconn.pyx":637
  * 
  * 
  * cdef char *_call_bytes(PGconn pgconn, conn_bytes_f func) except NULL:             # <<<<<<<<<<<<<<
  *     """
  *     Call one of the pgconn libpq functions returning a bytes pointer.
  */
 
@@ -16677,15 +17074,15 @@
   __Pyx_AddTraceback("psycopg_c.pq._call_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":642
+/* "psycopg_c/pq/pgconn.pyx":648
  * 
  * 
  * cdef int _call_int(PGconn pgconn, conn_int_f func) except -2:             # <<<<<<<<<<<<<<
  *     """
  *     Call one of the pgconn libpq functions returning an int.
  */
 
@@ -16695,55 +17092,55 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_call_int", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":646
+  /* "psycopg_c/pq/pgconn.pyx":652
  *     Call one of the pgconn libpq functions returning an int.
  *     """
  *     if not _ensure_pgconn(pgconn):             # <<<<<<<<<<<<<<
  *         return -2
  *     return func(pgconn._pgconn_ptr)
  */
-  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_pgconn); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9psycopg_c_2pq__ensure_pgconn(__pyx_v_pgconn); if (unlikely(__pyx_t_1 == ((int)0))) __PYX_ERR(0, 652, __pyx_L1_error)
   __pyx_t_2 = (!(__pyx_t_1 != 0));
   if (__pyx_t_2) {
 
-    /* "psycopg_c/pq/pgconn.pyx":647
+    /* "psycopg_c/pq/pgconn.pyx":653
  *     """
  *     if not _ensure_pgconn(pgconn):
  *         return -2             # <<<<<<<<<<<<<<
  *     return func(pgconn._pgconn_ptr)
  * 
  */
     __pyx_r = -2;
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":646
+    /* "psycopg_c/pq/pgconn.pyx":652
  *     Call one of the pgconn libpq functions returning an int.
  *     """
  *     if not _ensure_pgconn(pgconn):             # <<<<<<<<<<<<<<
  *         return -2
  *     return func(pgconn._pgconn_ptr)
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":648
+  /* "psycopg_c/pq/pgconn.pyx":654
  *     if not _ensure_pgconn(pgconn):
  *         return -2
  *     return func(pgconn._pgconn_ptr)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_func(__pyx_v_pgconn->_pgconn_ptr);
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":642
+  /* "psycopg_c/pq/pgconn.pyx":648
  * 
  * 
  * cdef int _call_int(PGconn pgconn, conn_int_f func) except -2:             # <<<<<<<<<<<<<<
  *     """
  *     Call one of the pgconn libpq functions returning an int.
  */
 
@@ -16752,15 +17149,15 @@
   __Pyx_AddTraceback("psycopg_c.pq._call_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -2;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":651
+/* "psycopg_c/pq/pgconn.pyx":657
  * 
  * 
  * cdef void notice_receiver(void *arg, const libpq.PGresult *res_ptr) with gil:             # <<<<<<<<<<<<<<
  *     cdef PGconn pgconn = <object>arg
  *     if pgconn.notice_handler is None:
  */
 
@@ -16793,68 +17190,68 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("notice_receiver", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":652
+  /* "psycopg_c/pq/pgconn.pyx":658
  * 
  * cdef void notice_receiver(void *arg, const libpq.PGresult *res_ptr) with gil:
  *     cdef PGconn pgconn = <object>arg             # <<<<<<<<<<<<<<
  *     if pgconn.notice_handler is None:
  *         return
  */
-  if (!(likely(((((PyObject *)__pyx_v_arg)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_arg), __pyx_ptype_9psycopg_c_2pq_PGconn))))) __PYX_ERR(0, 652, __pyx_L1_error)
+  if (!(likely(((((PyObject *)__pyx_v_arg)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_arg), __pyx_ptype_9psycopg_c_2pq_PGconn))))) __PYX_ERR(0, 658, __pyx_L1_error)
   __pyx_t_1 = ((PyObject *)__pyx_v_arg);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_pgconn = ((struct __pyx_obj_9psycopg_c_2pq_PGconn *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "psycopg_c/pq/pgconn.pyx":653
+  /* "psycopg_c/pq/pgconn.pyx":659
  * cdef void notice_receiver(void *arg, const libpq.PGresult *res_ptr) with gil:
  *     cdef PGconn pgconn = <object>arg
  *     if pgconn.notice_handler is None:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_2 = (__pyx_v_pgconn->notice_handler == Py_None);
   if (__pyx_t_2) {
 
-    /* "psycopg_c/pq/pgconn.pyx":654
+    /* "psycopg_c/pq/pgconn.pyx":660
  *     cdef PGconn pgconn = <object>arg
  *     if pgconn.notice_handler is None:
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef PGresult res = PGresult._from_ptr(<libpq.PGresult *>res_ptr)
  */
     goto __pyx_L0;
 
-    /* "psycopg_c/pq/pgconn.pyx":653
+    /* "psycopg_c/pq/pgconn.pyx":659
  * cdef void notice_receiver(void *arg, const libpq.PGresult *res_ptr) with gil:
  *     cdef PGconn pgconn = <object>arg
  *     if pgconn.notice_handler is None:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":656
+  /* "psycopg_c/pq/pgconn.pyx":662
  *         return
  * 
  *     cdef PGresult res = PGresult._from_ptr(<libpq.PGresult *>res_ptr)             # <<<<<<<<<<<<<<
  *     try:
  *         pgconn.notice_handler(res)
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(((PGresult *)__pyx_v_res_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_9psycopg_c_2pq_8PGresult__from_ptr(((PGresult *)__pyx_v_res_ptr))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_res = ((struct __pyx_obj_9psycopg_c_2pq_PGresult *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "psycopg_c/pq/pgconn.pyx":657
+  /* "psycopg_c/pq/pgconn.pyx":663
  * 
  *     cdef PGresult res = PGresult._from_ptr(<libpq.PGresult *>res_ptr)
  *     try:             # <<<<<<<<<<<<<<
  *         pgconn.notice_handler(res)
  *     except Exception as e:
  */
   /*try:*/ {
@@ -16863,15 +17260,15 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "psycopg_c/pq/pgconn.pyx":658
+        /* "psycopg_c/pq/pgconn.pyx":664
  *     cdef PGresult res = PGresult._from_ptr(<libpq.PGresult *>res_ptr)
  *     try:
  *         pgconn.notice_handler(res)             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         logger.exception("error in notice receiver: %s", e)
  */
         __Pyx_INCREF(__pyx_v_pgconn->notice_handler);
@@ -16887,21 +17284,21 @@
             __pyx_t_8 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_7, ((PyObject *)__pyx_v_res)};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 658, __pyx_L7_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 664, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "psycopg_c/pq/pgconn.pyx":657
+        /* "psycopg_c/pq/pgconn.pyx":663
  * 
  *     cdef PGresult res = PGresult._from_ptr(<libpq.PGresult *>res_ptr)
  *     try:             # <<<<<<<<<<<<<<
  *         pgconn.notice_handler(res)
  *     except Exception as e:
  */
       }
@@ -16910,42 +17307,42 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L12_try_end;
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "psycopg_c/pq/pgconn.pyx":659
+      /* "psycopg_c/pq/pgconn.pyx":665
  *     try:
  *         pgconn.notice_handler(res)
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         logger.exception("error in notice receiver: %s", e)
  *     finally:
  */
       __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_8) {
         __Pyx_AddTraceback("psycopg_c.pq.notice_receiver", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 659, __pyx_L9_except_error)
+        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 665, __pyx_L9_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_6);
         __pyx_v_e = __pyx_t_6;
         /*try:*/ {
 
-          /* "psycopg_c/pq/pgconn.pyx":660
+          /* "psycopg_c/pq/pgconn.pyx":666
  *         pgconn.notice_handler(res)
  *     except Exception as e:
  *         logger.exception("error in notice receiver: %s", e)             # <<<<<<<<<<<<<<
  *     finally:
  *         res._pgresult_ptr = NULL  # avoid destroying the pgresult_ptr
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_logger); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 660, __pyx_L18_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_logger); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 666, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_exception); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 660, __pyx_L18_error)
+          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_exception); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 666, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __pyx_t_10 = NULL;
           __pyx_t_8 = 0;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
             __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
             if (likely(__pyx_t_10)) {
@@ -16956,22 +17353,22 @@
               __pyx_t_8 = 1;
             }
           }
           {
             PyObject *__pyx_callargs[3] = {__pyx_t_10, __pyx_kp_u_error_in_notice_receiver_s, __pyx_v_e};
             __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_8, 2+__pyx_t_8);
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 660, __pyx_L18_error)
+            if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 666, __pyx_L18_error)
             __Pyx_GOTREF(__pyx_t_9);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           }
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
 
-        /* "psycopg_c/pq/pgconn.pyx":659
+        /* "psycopg_c/pq/pgconn.pyx":665
  *     try:
  *         pgconn.notice_handler(res)
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         logger.exception("error in notice receiver: %s", e)
  *     finally:
  */
         /*finally:*/ {
@@ -17019,15 +17416,15 @@
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L8_exception_handled;
       }
       goto __pyx_L9_except_error;
       __pyx_L9_except_error:;
 
-      /* "psycopg_c/pq/pgconn.pyx":657
+      /* "psycopg_c/pq/pgconn.pyx":663
  * 
  *     cdef PGresult res = PGresult._from_ptr(<libpq.PGresult *>res_ptr)
  *     try:             # <<<<<<<<<<<<<<
  *         pgconn.notice_handler(res)
  *     except Exception as e:
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -17040,15 +17437,15 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       __pyx_L12_try_end:;
     }
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":662
+  /* "psycopg_c/pq/pgconn.pyx":668
  *         logger.exception("error in notice receiver: %s", e)
  *     finally:
  *         res._pgresult_ptr = NULL  # avoid destroying the pgresult_ptr             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*finally:*/ {
@@ -17092,15 +17489,15 @@
       __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_3 = 0; __pyx_t_19 = 0; __pyx_t_18 = 0; __pyx_t_17 = 0;
       __pyx_lineno = __pyx_t_12; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_20;
       goto __pyx_L1_error;
     }
     __pyx_L6:;
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":651
+  /* "psycopg_c/pq/pgconn.pyx":657
  * 
  * 
  * cdef void notice_receiver(void *arg, const libpq.PGresult *res_ptr) with gil:             # <<<<<<<<<<<<<<
  *     cdef PGconn pgconn = <object>arg
  *     if pgconn.notice_handler is None:
  */
 
@@ -17120,15 +17517,15 @@
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "psycopg_c/pq/pgconn.pyx":665
+/* "psycopg_c/pq/pgconn.pyx":671
  * 
  * 
  * cdef (Py_ssize_t, libpq.Oid *, char * const*, int *, int *) _query_params_args(             # <<<<<<<<<<<<<<
  *     list param_values: Optional[Sequence[Optional[bytes]]],
  *     param_types: Optional[Sequence[int]],
  */
 
@@ -17158,15 +17555,15 @@
   Oid __pyx_t_11;
   __pyx_ctuple_9512b6__Py_ssize_t__and_Oid__ptr__and_char__ptrconst__ptr__and_int__ptr__and_int__ptr__etc __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_query_params_args", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":675
+  /* "psycopg_c/pq/pgconn.pyx":681
  *     # is most often no-op
  *     cdef tuple tparam_types
  *     if param_types is not None and not isinstance(param_types, tuple):             # <<<<<<<<<<<<<<
  *         tparam_types = tuple(param_types)
  *     else:
  */
   __pyx_t_2 = (__pyx_v_param_types != Py_None);
@@ -17177,586 +17574,586 @@
   }
   __pyx_t_2 = PyTuple_Check(__pyx_v_param_types); 
   __pyx_t_3 = (!__pyx_t_2);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":676
+    /* "psycopg_c/pq/pgconn.pyx":682
  *     cdef tuple tparam_types
  *     if param_types is not None and not isinstance(param_types, tuple):
  *         tparam_types = tuple(param_types)             # <<<<<<<<<<<<<<
  *     else:
  *         tparam_types = param_types
  */
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_param_types); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 676, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_param_types); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 682, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_tparam_types = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":675
+    /* "psycopg_c/pq/pgconn.pyx":681
  *     # is most often no-op
  *     cdef tuple tparam_types
  *     if param_types is not None and not isinstance(param_types, tuple):             # <<<<<<<<<<<<<<
  *         tparam_types = tuple(param_types)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":678
+  /* "psycopg_c/pq/pgconn.pyx":684
  *         tparam_types = tuple(param_types)
  *     else:
  *         tparam_types = param_types             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t nparams = len(param_values) if param_values else 0
  */
   /*else*/ {
-    if (!(likely(PyTuple_CheckExact(__pyx_v_param_types))||((__pyx_v_param_types) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v_param_types))) __PYX_ERR(0, 678, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v_param_types))||((__pyx_v_param_types) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v_param_types))) __PYX_ERR(0, 684, __pyx_L1_error)
     __pyx_t_4 = __pyx_v_param_types;
     __Pyx_INCREF(__pyx_t_4);
     __pyx_v_tparam_types = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "psycopg_c/pq/pgconn.pyx":680
+  /* "psycopg_c/pq/pgconn.pyx":686
  *         tparam_types = param_types
  * 
  *     cdef Py_ssize_t nparams = len(param_values) if param_values else 0             # <<<<<<<<<<<<<<
  *     if tparam_types is not None and len(tparam_types) != nparams:
  *         raise ValueError(
  */
   __pyx_t_1 = (__pyx_v_param_values != Py_None)&&(PyList_GET_SIZE(__pyx_v_param_values) != 0);
   if (__pyx_t_1) {
     if (unlikely(__pyx_v_param_values == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 680, __pyx_L1_error)
+      __PYX_ERR(0, 686, __pyx_L1_error)
     }
-    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_param_values); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 680, __pyx_L1_error)
+    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_param_values); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 686, __pyx_L1_error)
     __pyx_t_5 = __pyx_t_6;
   } else {
     __pyx_t_5 = 0;
   }
   __pyx_v_nparams = __pyx_t_5;
 
-  /* "psycopg_c/pq/pgconn.pyx":681
+  /* "psycopg_c/pq/pgconn.pyx":687
  * 
  *     cdef Py_ssize_t nparams = len(param_values) if param_values else 0
  *     if tparam_types is not None and len(tparam_types) != nparams:             # <<<<<<<<<<<<<<
  *         raise ValueError(
  *             "got %d param_values but %d param_types"
  */
   __pyx_t_3 = (__pyx_v_tparam_types != ((PyObject*)Py_None));
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L7_bool_binop_done;
   }
   if (unlikely(__pyx_v_tparam_types == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 681, __pyx_L1_error)
+    __PYX_ERR(0, 687, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(__pyx_v_tparam_types); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(__pyx_v_tparam_types); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 687, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_5 != __pyx_v_nparams);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":683
+    /* "psycopg_c/pq/pgconn.pyx":689
  *     if tparam_types is not None and len(tparam_types) != nparams:
  *         raise ValueError(
  *             "got %d param_values but %d param_types"             # <<<<<<<<<<<<<<
  *             % (nparams, len(tparam_types))
  *         )
  */
-    __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 683, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 689, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_got);
     __pyx_t_5 += 4;
     __Pyx_GIVEREF(__pyx_kp_u_got);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_got);
 
-    /* "psycopg_c/pq/pgconn.pyx":684
+    /* "psycopg_c/pq/pgconn.pyx":690
  *         raise ValueError(
  *             "got %d param_values but %d param_types"
  *             % (nparams, len(tparam_types))             # <<<<<<<<<<<<<<
  *         )
  *     if param_formats is not None and len(param_formats) != nparams:
  */
-    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_nparams, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 684, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_nparams, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_param_values_but);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_param_values_but);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u_param_values_but);
     if (unlikely(__pyx_v_tparam_types == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 684, __pyx_L1_error)
+      __PYX_ERR(0, 690, __pyx_L1_error)
     }
-    __pyx_t_6 = PyTuple_GET_SIZE(__pyx_v_tparam_types); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 684, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_6, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 684, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_GET_SIZE(__pyx_v_tparam_types); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 690, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_6, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_param_types_2);
     __pyx_t_5 += 12;
     __Pyx_GIVEREF(__pyx_kp_u_param_types_2);
     PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u_param_types_2);
 
-    /* "psycopg_c/pq/pgconn.pyx":683
+    /* "psycopg_c/pq/pgconn.pyx":689
  *     if tparam_types is not None and len(tparam_types) != nparams:
  *         raise ValueError(
  *             "got %d param_values but %d param_types"             # <<<<<<<<<<<<<<
  *             % (nparams, len(tparam_types))
  *         )
  */
-    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 683, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 689, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":682
+    /* "psycopg_c/pq/pgconn.pyx":688
  *     cdef Py_ssize_t nparams = len(param_values) if param_values else 0
  *     if tparam_types is not None and len(tparam_types) != nparams:
  *         raise ValueError(             # <<<<<<<<<<<<<<
  *             "got %d param_values but %d param_types"
  *             % (nparams, len(tparam_types))
  */
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 682, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 688, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 682, __pyx_L1_error)
+    __PYX_ERR(0, 688, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":681
+    /* "psycopg_c/pq/pgconn.pyx":687
  * 
  *     cdef Py_ssize_t nparams = len(param_values) if param_values else 0
  *     if tparam_types is not None and len(tparam_types) != nparams:             # <<<<<<<<<<<<<<
  *         raise ValueError(
  *             "got %d param_values but %d param_types"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":686
+  /* "psycopg_c/pq/pgconn.pyx":692
  *             % (nparams, len(tparam_types))
  *         )
  *     if param_formats is not None and len(param_formats) != nparams:             # <<<<<<<<<<<<<<
  *         raise ValueError(
  *             "got %d param_values but %d param_formats"
  */
   __pyx_t_3 = (__pyx_v_param_formats != ((PyObject*)Py_None));
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L10_bool_binop_done;
   }
   if (unlikely(__pyx_v_param_formats == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 686, __pyx_L1_error)
+    __PYX_ERR(0, 692, __pyx_L1_error)
   }
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_param_formats); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_param_formats); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 692, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_5 != __pyx_v_nparams);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L10_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "psycopg_c/pq/pgconn.pyx":688
+    /* "psycopg_c/pq/pgconn.pyx":694
  *     if param_formats is not None and len(param_formats) != nparams:
  *         raise ValueError(
  *             "got %d param_values but %d param_formats"             # <<<<<<<<<<<<<<
  *             % (nparams, len(param_formats))
  *         )
  */
-    __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 688, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 694, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_got);
     __pyx_t_5 += 4;
     __Pyx_GIVEREF(__pyx_kp_u_got);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_got);
 
-    /* "psycopg_c/pq/pgconn.pyx":689
+    /* "psycopg_c/pq/pgconn.pyx":695
  *         raise ValueError(
  *             "got %d param_values but %d param_formats"
  *             % (nparams, len(param_formats))             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_nparams, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 689, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_nparams, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 695, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_param_values_but);
     __pyx_t_5 += 18;
     __Pyx_GIVEREF(__pyx_kp_u_param_values_but);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u_param_values_but);
     if (unlikely(__pyx_v_param_formats == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 689, __pyx_L1_error)
+      __PYX_ERR(0, 695, __pyx_L1_error)
     }
-    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_param_formats); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 689, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_6, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 689, __pyx_L1_error)
+    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_param_formats); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 695, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_6, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 695, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_param_formats_2);
     __pyx_t_5 += 14;
     __Pyx_GIVEREF(__pyx_kp_u_param_formats_2);
     PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u_param_formats_2);
 
-    /* "psycopg_c/pq/pgconn.pyx":688
+    /* "psycopg_c/pq/pgconn.pyx":694
  *     if param_formats is not None and len(param_formats) != nparams:
  *         raise ValueError(
  *             "got %d param_values but %d param_formats"             # <<<<<<<<<<<<<<
  *             % (nparams, len(param_formats))
  *         )
  */
-    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 688, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 694, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "psycopg_c/pq/pgconn.pyx":687
+    /* "psycopg_c/pq/pgconn.pyx":693
  *         )
  *     if param_formats is not None and len(param_formats) != nparams:
  *         raise ValueError(             # <<<<<<<<<<<<<<
  *             "got %d param_values but %d param_formats"
  *             % (nparams, len(param_formats))
  */
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 687, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 693, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 687, __pyx_L1_error)
+    __PYX_ERR(0, 693, __pyx_L1_error)
 
-    /* "psycopg_c/pq/pgconn.pyx":686
+    /* "psycopg_c/pq/pgconn.pyx":692
  *             % (nparams, len(tparam_types))
  *         )
  *     if param_formats is not None and len(param_formats) != nparams:             # <<<<<<<<<<<<<<
  *         raise ValueError(
  *             "got %d param_values but %d param_formats"
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":692
+  /* "psycopg_c/pq/pgconn.pyx":698
  *         )
  * 
  *     cdef char **aparams = NULL             # <<<<<<<<<<<<<<
  *     cdef int *alenghts = NULL
  *     cdef char *ptr
  */
   __pyx_v_aparams = NULL;
 
-  /* "psycopg_c/pq/pgconn.pyx":693
+  /* "psycopg_c/pq/pgconn.pyx":699
  * 
  *     cdef char **aparams = NULL
  *     cdef int *alenghts = NULL             # <<<<<<<<<<<<<<
  *     cdef char *ptr
  *     cdef Py_ssize_t length
  */
   __pyx_v_alenghts = NULL;
 
-  /* "psycopg_c/pq/pgconn.pyx":697
+  /* "psycopg_c/pq/pgconn.pyx":703
  *     cdef Py_ssize_t length
  * 
  *     if nparams:             # <<<<<<<<<<<<<<
  *         aparams = <char **>PyMem_Malloc(nparams * sizeof(char *))
  *         alenghts = <int *>PyMem_Malloc(nparams * sizeof(int))
  */
   __pyx_t_1 = (__pyx_v_nparams != 0);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":698
+    /* "psycopg_c/pq/pgconn.pyx":704
  * 
  *     if nparams:
  *         aparams = <char **>PyMem_Malloc(nparams * sizeof(char *))             # <<<<<<<<<<<<<<
  *         alenghts = <int *>PyMem_Malloc(nparams * sizeof(int))
  *         for i in range(nparams):
  */
     __pyx_v_aparams = ((char **)PyMem_Malloc((__pyx_v_nparams * (sizeof(char *)))));
 
-    /* "psycopg_c/pq/pgconn.pyx":699
+    /* "psycopg_c/pq/pgconn.pyx":705
  *     if nparams:
  *         aparams = <char **>PyMem_Malloc(nparams * sizeof(char *))
  *         alenghts = <int *>PyMem_Malloc(nparams * sizeof(int))             # <<<<<<<<<<<<<<
  *         for i in range(nparams):
  *             obj = param_values[i]
  */
     __pyx_v_alenghts = ((int *)PyMem_Malloc((__pyx_v_nparams * (sizeof(int)))));
 
-    /* "psycopg_c/pq/pgconn.pyx":700
+    /* "psycopg_c/pq/pgconn.pyx":706
  *         aparams = <char **>PyMem_Malloc(nparams * sizeof(char *))
  *         alenghts = <int *>PyMem_Malloc(nparams * sizeof(int))
  *         for i in range(nparams):             # <<<<<<<<<<<<<<
  *             obj = param_values[i]
  *             if obj is None:
  */
     __pyx_t_5 = __pyx_v_nparams;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_6; __pyx_t_9+=1) {
       __pyx_v_i = __pyx_t_9;
 
-      /* "psycopg_c/pq/pgconn.pyx":701
+      /* "psycopg_c/pq/pgconn.pyx":707
  *         alenghts = <int *>PyMem_Malloc(nparams * sizeof(int))
  *         for i in range(nparams):
  *             obj = param_values[i]             # <<<<<<<<<<<<<<
  *             if obj is None:
  *                 aparams[i] = NULL
  */
       if (unlikely(__pyx_v_param_values == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 701, __pyx_L1_error)
+        __PYX_ERR(0, 707, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_param_values, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 701, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_param_values, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 707, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_obj, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "psycopg_c/pq/pgconn.pyx":702
+      /* "psycopg_c/pq/pgconn.pyx":708
  *         for i in range(nparams):
  *             obj = param_values[i]
  *             if obj is None:             # <<<<<<<<<<<<<<
  *                 aparams[i] = NULL
  *                 alenghts[i] = 0
  */
       __pyx_t_1 = (__pyx_v_obj == Py_None);
       if (__pyx_t_1) {
 
-        /* "psycopg_c/pq/pgconn.pyx":703
+        /* "psycopg_c/pq/pgconn.pyx":709
  *             obj = param_values[i]
  *             if obj is None:
  *                 aparams[i] = NULL             # <<<<<<<<<<<<<<
  *                 alenghts[i] = 0
  *             else:
  */
         (__pyx_v_aparams[__pyx_v_i]) = NULL;
 
-        /* "psycopg_c/pq/pgconn.pyx":704
+        /* "psycopg_c/pq/pgconn.pyx":710
  *             if obj is None:
  *                 aparams[i] = NULL
  *                 alenghts[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 # TODO: it is a leak if this fails (but it should only fail
  */
         (__pyx_v_alenghts[__pyx_v_i]) = 0;
 
-        /* "psycopg_c/pq/pgconn.pyx":702
+        /* "psycopg_c/pq/pgconn.pyx":708
  *         for i in range(nparams):
  *             obj = param_values[i]
  *             if obj is None:             # <<<<<<<<<<<<<<
  *                 aparams[i] = NULL
  *                 alenghts[i] = 0
  */
         goto __pyx_L15;
       }
 
-      /* "psycopg_c/pq/pgconn.pyx":708
+      /* "psycopg_c/pq/pgconn.pyx":714
  *                 # TODO: it is a leak if this fails (but it should only fail
  *                 # on internal error, e.g. if obj is not a buffer)
  *                 _buffer_as_string_and_size(obj, &ptr, &length)             # <<<<<<<<<<<<<<
  *                 aparams[i] = ptr
  *                 alenghts[i] = <int>length
  */
       /*else*/ {
-        __pyx_t_10 = __pyx_f_9psycopg_c_2pq__buffer_as_string_and_size(__pyx_v_obj, (&__pyx_v_ptr), (&__pyx_v_length)); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 708, __pyx_L1_error)
+        __pyx_t_10 = __pyx_f_9psycopg_c_2pq__buffer_as_string_and_size(__pyx_v_obj, (&__pyx_v_ptr), (&__pyx_v_length)); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 714, __pyx_L1_error)
 
-        /* "psycopg_c/pq/pgconn.pyx":709
+        /* "psycopg_c/pq/pgconn.pyx":715
  *                 # on internal error, e.g. if obj is not a buffer)
  *                 _buffer_as_string_and_size(obj, &ptr, &length)
  *                 aparams[i] = ptr             # <<<<<<<<<<<<<<
  *                 alenghts[i] = <int>length
  * 
  */
         (__pyx_v_aparams[__pyx_v_i]) = __pyx_v_ptr;
 
-        /* "psycopg_c/pq/pgconn.pyx":710
+        /* "psycopg_c/pq/pgconn.pyx":716
  *                 _buffer_as_string_and_size(obj, &ptr, &length)
  *                 aparams[i] = ptr
  *                 alenghts[i] = <int>length             # <<<<<<<<<<<<<<
  * 
  *     cdef libpq.Oid *atypes = NULL
  */
         (__pyx_v_alenghts[__pyx_v_i]) = ((int)__pyx_v_length);
       }
       __pyx_L15:;
     }
 
-    /* "psycopg_c/pq/pgconn.pyx":697
+    /* "psycopg_c/pq/pgconn.pyx":703
  *     cdef Py_ssize_t length
  * 
  *     if nparams:             # <<<<<<<<<<<<<<
  *         aparams = <char **>PyMem_Malloc(nparams * sizeof(char *))
  *         alenghts = <int *>PyMem_Malloc(nparams * sizeof(int))
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":712
+  /* "psycopg_c/pq/pgconn.pyx":718
  *                 alenghts[i] = <int>length
  * 
  *     cdef libpq.Oid *atypes = NULL             # <<<<<<<<<<<<<<
  *     if tparam_types:
  *         atypes = <libpq.Oid *>PyMem_Malloc(nparams * sizeof(libpq.Oid))
  */
   __pyx_v_atypes = NULL;
 
-  /* "psycopg_c/pq/pgconn.pyx":713
+  /* "psycopg_c/pq/pgconn.pyx":719
  * 
  *     cdef libpq.Oid *atypes = NULL
  *     if tparam_types:             # <<<<<<<<<<<<<<
  *         atypes = <libpq.Oid *>PyMem_Malloc(nparams * sizeof(libpq.Oid))
  *         for i in range(nparams):
  */
   __pyx_t_1 = (__pyx_v_tparam_types != Py_None)&&(PyTuple_GET_SIZE(__pyx_v_tparam_types) != 0);
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":714
+    /* "psycopg_c/pq/pgconn.pyx":720
  *     cdef libpq.Oid *atypes = NULL
  *     if tparam_types:
  *         atypes = <libpq.Oid *>PyMem_Malloc(nparams * sizeof(libpq.Oid))             # <<<<<<<<<<<<<<
  *         for i in range(nparams):
  *             atypes[i] = tparam_types[i]
  */
     __pyx_v_atypes = ((Oid *)PyMem_Malloc((__pyx_v_nparams * (sizeof(Oid)))));
 
-    /* "psycopg_c/pq/pgconn.pyx":715
+    /* "psycopg_c/pq/pgconn.pyx":721
  *     if tparam_types:
  *         atypes = <libpq.Oid *>PyMem_Malloc(nparams * sizeof(libpq.Oid))
  *         for i in range(nparams):             # <<<<<<<<<<<<<<
  *             atypes[i] = tparam_types[i]
  * 
  */
     __pyx_t_5 = __pyx_v_nparams;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_6; __pyx_t_9+=1) {
       __pyx_v_i = __pyx_t_9;
 
-      /* "psycopg_c/pq/pgconn.pyx":716
+      /* "psycopg_c/pq/pgconn.pyx":722
  *         atypes = <libpq.Oid *>PyMem_Malloc(nparams * sizeof(libpq.Oid))
  *         for i in range(nparams):
  *             atypes[i] = tparam_types[i]             # <<<<<<<<<<<<<<
  * 
  *     cdef int *aformats = NULL
  */
       if (unlikely(__pyx_v_tparam_types == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 716, __pyx_L1_error)
+        __PYX_ERR(0, 722, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_GetItemInt_Tuple(__pyx_v_tparam_types, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 716, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt_Tuple(__pyx_v_tparam_types, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 722, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_11 = __Pyx_PyInt_As_Oid(__pyx_t_4); if (unlikely((__pyx_t_11 == ((Oid)-1)) && PyErr_Occurred())) __PYX_ERR(0, 716, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_Oid(__pyx_t_4); if (unlikely((__pyx_t_11 == ((Oid)-1)) && PyErr_Occurred())) __PYX_ERR(0, 722, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       (__pyx_v_atypes[__pyx_v_i]) = __pyx_t_11;
     }
 
-    /* "psycopg_c/pq/pgconn.pyx":713
+    /* "psycopg_c/pq/pgconn.pyx":719
  * 
  *     cdef libpq.Oid *atypes = NULL
  *     if tparam_types:             # <<<<<<<<<<<<<<
  *         atypes = <libpq.Oid *>PyMem_Malloc(nparams * sizeof(libpq.Oid))
  *         for i in range(nparams):
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":718
+  /* "psycopg_c/pq/pgconn.pyx":724
  *             atypes[i] = tparam_types[i]
  * 
  *     cdef int *aformats = NULL             # <<<<<<<<<<<<<<
  *     if param_formats is not None:
  *         aformats = <int *>PyMem_Malloc(nparams * sizeof(int *))
  */
   __pyx_v_aformats = NULL;
 
-  /* "psycopg_c/pq/pgconn.pyx":719
+  /* "psycopg_c/pq/pgconn.pyx":725
  * 
  *     cdef int *aformats = NULL
  *     if param_formats is not None:             # <<<<<<<<<<<<<<
  *         aformats = <int *>PyMem_Malloc(nparams * sizeof(int *))
  *         for i in range(nparams):
  */
   __pyx_t_1 = (__pyx_v_param_formats != ((PyObject*)Py_None));
   if (__pyx_t_1) {
 
-    /* "psycopg_c/pq/pgconn.pyx":720
+    /* "psycopg_c/pq/pgconn.pyx":726
  *     cdef int *aformats = NULL
  *     if param_formats is not None:
  *         aformats = <int *>PyMem_Malloc(nparams * sizeof(int *))             # <<<<<<<<<<<<<<
  *         for i in range(nparams):
  *             aformats[i] = param_formats[i]
  */
     __pyx_v_aformats = ((int *)PyMem_Malloc((__pyx_v_nparams * (sizeof(int *)))));
 
-    /* "psycopg_c/pq/pgconn.pyx":721
+    /* "psycopg_c/pq/pgconn.pyx":727
  *     if param_formats is not None:
  *         aformats = <int *>PyMem_Malloc(nparams * sizeof(int *))
  *         for i in range(nparams):             # <<<<<<<<<<<<<<
  *             aformats[i] = param_formats[i]
  * 
  */
     __pyx_t_5 = __pyx_v_nparams;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_6; __pyx_t_9+=1) {
       __pyx_v_i = __pyx_t_9;
 
-      /* "psycopg_c/pq/pgconn.pyx":722
+      /* "psycopg_c/pq/pgconn.pyx":728
  *         aformats = <int *>PyMem_Malloc(nparams * sizeof(int *))
  *         for i in range(nparams):
  *             aformats[i] = param_formats[i]             # <<<<<<<<<<<<<<
  * 
  *     return (nparams, atypes, aparams, alenghts, aformats)
  */
       if (unlikely(__pyx_v_param_formats == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 722, __pyx_L1_error)
+        __PYX_ERR(0, 728, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_param_formats, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 722, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_param_formats, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 728, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 722, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 728, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       (__pyx_v_aformats[__pyx_v_i]) = __pyx_t_10;
     }
 
-    /* "psycopg_c/pq/pgconn.pyx":719
+    /* "psycopg_c/pq/pgconn.pyx":725
  * 
  *     cdef int *aformats = NULL
  *     if param_formats is not None:             # <<<<<<<<<<<<<<
  *         aformats = <int *>PyMem_Malloc(nparams * sizeof(int *))
  *         for i in range(nparams):
  */
   }
 
-  /* "psycopg_c/pq/pgconn.pyx":724
+  /* "psycopg_c/pq/pgconn.pyx":730
  *             aformats[i] = param_formats[i]
  * 
  *     return (nparams, atypes, aparams, alenghts, aformats)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_12.f0 = __pyx_v_nparams;
   __pyx_t_12.f1 = __pyx_v_atypes;
   __pyx_t_12.f2 = __pyx_v_aparams;
   __pyx_t_12.f3 = __pyx_v_alenghts;
   __pyx_t_12.f4 = __pyx_v_aformats;
   __pyx_r = __pyx_t_12;
   goto __pyx_L0;
 
-  /* "psycopg_c/pq/pgconn.pyx":665
+  /* "psycopg_c/pq/pgconn.pyx":671
  * 
  * 
  * cdef (Py_ssize_t, libpq.Oid *, char * const*, int *, int *) _query_params_args(             # <<<<<<<<<<<<<<
  *     list param_values: Optional[Sequence[Optional[bytes]]],
  *     param_types: Optional[Sequence[int]],
  */
 
@@ -17769,60 +18166,60 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_tparam_types);
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "psycopg_c/pq/pgconn.pyx":727
+/* "psycopg_c/pq/pgconn.pyx":733
  * 
  * 
  * cdef void _clear_query_params(             # <<<<<<<<<<<<<<
  *     libpq.Oid *ctypes, char *const *cvalues, int *clenghst, int *cformats
  * ):
  */
 
 static void __pyx_f_9psycopg_c_2pq__clear_query_params(Oid *__pyx_v_ctypes, char *const *__pyx_v_cvalues, int *__pyx_v_clenghst, int *__pyx_v_cformats) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_clear_query_params", 0);
 
-  /* "psycopg_c/pq/pgconn.pyx":730
+  /* "psycopg_c/pq/pgconn.pyx":736
  *     libpq.Oid *ctypes, char *const *cvalues, int *clenghst, int *cformats
  * ):
  *     PyMem_Free(ctypes)             # <<<<<<<<<<<<<<
  *     PyMem_Free(<char **>cvalues)
  *     PyMem_Free(clenghst)
  */
   PyMem_Free(__pyx_v_ctypes);
 
-  /* "psycopg_c/pq/pgconn.pyx":731
+  /* "psycopg_c/pq/pgconn.pyx":737
  * ):
  *     PyMem_Free(ctypes)
  *     PyMem_Free(<char **>cvalues)             # <<<<<<<<<<<<<<
  *     PyMem_Free(clenghst)
  *     PyMem_Free(cformats)
  */
   PyMem_Free(((char **)__pyx_v_cvalues));
 
-  /* "psycopg_c/pq/pgconn.pyx":732
+  /* "psycopg_c/pq/pgconn.pyx":738
  *     PyMem_Free(ctypes)
  *     PyMem_Free(<char **>cvalues)
  *     PyMem_Free(clenghst)             # <<<<<<<<<<<<<<
  *     PyMem_Free(cformats)
  */
   PyMem_Free(__pyx_v_clenghst);
 
-  /* "psycopg_c/pq/pgconn.pyx":733
+  /* "psycopg_c/pq/pgconn.pyx":739
  *     PyMem_Free(<char **>cvalues)
  *     PyMem_Free(clenghst)
  *     PyMem_Free(cformats)             # <<<<<<<<<<<<<<
  */
   PyMem_Free(__pyx_v_cformats);
 
-  /* "psycopg_c/pq/pgconn.pyx":727
+  /* "psycopg_c/pq/pgconn.pyx":733
  * 
  * 
  * cdef void _clear_query_params(             # <<<<<<<<<<<<<<
  *     libpq.Oid *ctypes, char *const *cvalues, int *clenghst, int *cformats
  * ):
  */
 
@@ -18174,18 +18571,18 @@
   __Pyx_GIVEREF(__pyx_kp_u__2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__2);
   __Pyx_INCREF(__pyx_v_cls);
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_cls) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_cls) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_cls);
   __Pyx_GIVEREF(__pyx_v_cls);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_cls);
-  __Pyx_INCREF(__pyx_kp_u__14);
+  __Pyx_INCREF(__pyx_kp_u__13);
   __pyx_t_2 += 2;
-  __Pyx_GIVEREF(__pyx_kp_u__14);
-  PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u__14);
+  __Pyx_GIVEREF(__pyx_kp_u__13);
+  PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u__13);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_status, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_1, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
@@ -19669,16 +20066,16 @@
  *             else:
  *                 return b""             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
-      __Pyx_INCREF(__pyx_kp_b__12);
-      __pyx_r = __pyx_kp_b__12;
+      __Pyx_INCREF(__pyx_kp_b__11);
+      __pyx_r = __pyx_kp_b__11;
       goto __pyx_L0;
     }
   }
 
   /* "psycopg_c/pq/pgresult.pyx":97
  *         return libpq.PQbinaryTuples(self._pgresult_ptr)
  * 
@@ -21113,15 +21510,15 @@
     /* "psycopg_c/pq/conninfo.pyx":15
  *         cdef libpq.PQconninfoOption *opts = libpq.PQconndefaults()
  *         if opts is NULL :
  *             raise MemoryError("couldn't allocate connection defaults")             # <<<<<<<<<<<<<<
  *         rv = _options_from_array(opts)
  *         libpq.PQconninfoFree(opts)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 15, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(5, 15, __pyx_L1_error)
 
     /* "psycopg_c/pq/conninfo.pyx":14
  *     def get_defaults(cls) -> List[ConninfoOption]:
@@ -21339,15 +21736,15 @@
       /* "psycopg_c/pq/conninfo.pyx":26
  *         if opts is NULL:
  *             if errmsg is NULL:
  *                 raise MemoryError("couldn't allocate on conninfo parse")             # <<<<<<<<<<<<<<
  *             else:
  *                 exc = e.OperationalError(errmsg.decode("utf8", "replace"))
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 26, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 26, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __PYX_ERR(5, 26, __pyx_L1_error)
 
       /* "psycopg_c/pq/conninfo.pyx":25
  *         cdef libpq.PQconninfoOption *opts = libpq.PQconninfoParse(conninfo, &errmsg)
@@ -21543,18 +21940,18 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
   __pyx_t_5 = 0;
-  __Pyx_INCREF(__pyx_kp_u__17);
+  __Pyx_INCREF(__pyx_kp_u__16);
   __pyx_t_2 += 2;
-  __Pyx_GIVEREF(__pyx_kp_u__17);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__17);
+  __Pyx_GIVEREF(__pyx_kp_u__16);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__16);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_keyword); if (unlikely(!__pyx_t_4)) __PYX_ERR(5, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
@@ -21580,18 +21977,18 @@
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_6);
   __pyx_t_6 = 0;
-  __Pyx_INCREF(__pyx_kp_u__18);
+  __Pyx_INCREF(__pyx_kp_u__17);
   __pyx_t_2 += 2;
-  __Pyx_GIVEREF(__pyx_kp_u__18);
-  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__18);
+  __Pyx_GIVEREF(__pyx_kp_u__17);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__17);
   __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
@@ -24516,18 +24913,18 @@
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_INCREF(__pyx_kp_u__19);
+  __Pyx_INCREF(__pyx_kp_u__18);
   __pyx_t_2 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__19);
-  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__19);
+  __Pyx_GIVEREF(__pyx_kp_u__18);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__18);
 
   /* "psycopg_c/pq/pqbuffer.pyx":36
  *         return (
  *             f"{self.__class__.__module__}.{self.__class__.__qualname__}"
  *             f"({bytes(self)})"             # <<<<<<<<<<<<<<
  *         )
  * 
@@ -24538,18 +24935,18 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
   __pyx_t_5 = 0;
-  __Pyx_INCREF(__pyx_kp_u__20);
+  __Pyx_INCREF(__pyx_kp_u__19);
   __pyx_t_2 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__20);
-  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_kp_u__20);
+  __Pyx_GIVEREF(__pyx_kp_u__19);
+  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_kp_u__19);
 
   /* "psycopg_c/pq/pqbuffer.pyx":35
  *     def __repr__(self):
  *         return (
  *             f"{self.__class__.__module__}.{self.__class__.__qualname__}"             # <<<<<<<<<<<<<<
  *             f"({bytes(self)})"
  *         )
@@ -25112,18 +25509,18 @@
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_INCREF(__pyx_kp_u__19);
+  __Pyx_INCREF(__pyx_kp_u__18);
   __pyx_t_2 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__19);
-  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__19);
+  __Pyx_GIVEREF(__pyx_kp_u__18);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__18);
 
   /* "psycopg_c/pq/pqbuffer.pyx":78
  *         return (
  *             f"{self.__class__.__module__}.{self.__class__.__qualname__}"
  *             f"({bytes(self)})"             # <<<<<<<<<<<<<<
  *         )
  * 
@@ -25134,18 +25531,18 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
   __pyx_t_5 = 0;
-  __Pyx_INCREF(__pyx_kp_u__20);
+  __Pyx_INCREF(__pyx_kp_u__19);
   __pyx_t_2 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__20);
-  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_kp_u__20);
+  __Pyx_GIVEREF(__pyx_kp_u__19);
+  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_kp_u__19);
 
   /* "psycopg_c/pq/pqbuffer.pyx":77
  *     def __repr__(self):
  *         return (
  *             f"{self.__class__.__module__}.{self.__class__.__qualname__}"             # <<<<<<<<<<<<<<
  *             f"({bytes(self)})"
  *         )
@@ -25745,15 +26142,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x0804127, 0x3908a35, 0x0c1d0e2):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x0804127, 0x3908a35, 0x0c1d0e2) = (conn))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__21, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__20, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x0804127, 0x3908a35, 0x0c1d0e2):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -27478,23 +27875,23 @@
   {0, __pyx_k_Trace, sizeof(__pyx_k_Trace), 0, 0, 1, 1},
   {0, __pyx_k_Tuple_int_memoryview, sizeof(__pyx_k_Tuple_int_memoryview), 0, 0, 1, 0},
   {0, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {0, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {0, __pyx_k_ViewBuffer, sizeof(__pyx_k_ViewBuffer), 0, 0, 1, 1},
   {0, __pyx_k_ViewBuffer___reduce_cython, sizeof(__pyx_k_ViewBuffer___reduce_cython), 0, 0, 1, 1},
   {0, __pyx_k_ViewBuffer___setstate_cython, sizeof(__pyx_k_ViewBuffer___setstate_cython), 0, 0, 1, 1},
-  {0, __pyx_k__12, sizeof(__pyx_k__12), 0, 0, 0, 0},
-  {0, __pyx_k__135, sizeof(__pyx_k__135), 0, 0, 1, 1},
-  {0, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 0},
+  {0, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 0, 0},
+  {0, __pyx_k__13, sizeof(__pyx_k__13), 0, 1, 0, 0},
+  {0, __pyx_k__134, sizeof(__pyx_k__134), 0, 0, 1, 1},
+  {0, __pyx_k__16, sizeof(__pyx_k__16), 0, 1, 0, 0},
   {0, __pyx_k__17, sizeof(__pyx_k__17), 0, 1, 0, 0},
   {0, __pyx_k__18, sizeof(__pyx_k__18), 0, 1, 0, 0},
   {0, __pyx_k__19, sizeof(__pyx_k__19), 0, 1, 0, 0},
   {0, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-  {0, __pyx_k__20, sizeof(__pyx_k__20), 0, 1, 0, 0},
-  {0, __pyx_k__22, sizeof(__pyx_k__22), 0, 0, 1, 1},
+  {0, __pyx_k__21, sizeof(__pyx_k__21), 0, 0, 1, 1},
   {0, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {0, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
   {0, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
   {0, __pyx_k_ascii, sizeof(__pyx_k_ascii), 0, 1, 0, 1},
   {0, __pyx_k_async, sizeof(__pyx_k_async), 0, 0, 1, 1},
   {0, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
   {0, __pyx_k_at_0x, sizeof(__pyx_k_at_0x), 0, 1, 0, 0},
@@ -27534,15 +27931,14 @@
   {0, __pyx_k_connect_start, sizeof(__pyx_k_connect_start), 0, 0, 1, 1},
   {0, __pyx_k_connection_not_in_pipeline_mode, sizeof(__pyx_k_connection_not_in_pipeline_mode), 0, 1, 0, 0},
   {0, __pyx_k_connection_summary, sizeof(__pyx_k_connection_summary), 0, 0, 1, 1},
   {0, __pyx_k_conninfo, sizeof(__pyx_k_conninfo), 0, 0, 1, 1},
   {0, __pyx_k_consume_input, sizeof(__pyx_k_consume_input), 0, 0, 1, 1},
   {0, __pyx_k_consuming_input_failed, sizeof(__pyx_k_consuming_input_failed), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_allocate_PGconn, sizeof(__pyx_k_couldn_t_allocate_PGconn), 0, 1, 0, 0},
-  {0, __pyx_k_couldn_t_allocate_PGresult, sizeof(__pyx_k_couldn_t_allocate_PGresult), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_allocate_connection_def, sizeof(__pyx_k_couldn_t_allocate_connection_def), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_allocate_connection_inf, sizeof(__pyx_k_couldn_t_allocate_connection_inf), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_allocate_empty_PGresult, sizeof(__pyx_k_couldn_t_allocate_empty_PGresult), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_allocate_for_escape_byt, sizeof(__pyx_k_couldn_t_allocate_for_escape_byt), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_allocate_for_unescape_b, sizeof(__pyx_k_couldn_t_allocate_for_unescape_b), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_allocate_on_conninfo_pa, sizeof(__pyx_k_couldn_t_allocate_on_conninfo_pa), 0, 1, 0, 0},
   {0, __pyx_k_couldn_t_create_cancel_object, sizeof(__pyx_k_couldn_t_create_cancel_object), 0, 1, 0, 0},
@@ -27553,14 +27949,15 @@
   {0, __pyx_k_cvalues, sizeof(__pyx_k_cvalues), 0, 0, 1, 1},
   {0, __pyx_k_d, sizeof(__pyx_k_d), 0, 1, 0, 1},
   {0, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {0, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {0, __pyx_k_descr, sizeof(__pyx_k_descr), 0, 0, 1, 1},
   {0, __pyx_k_describe_portal, sizeof(__pyx_k_describe_portal), 0, 0, 1, 1},
   {0, __pyx_k_describe_prepared, sizeof(__pyx_k_describe_prepared), 0, 0, 1, 1},
+  {0, __pyx_k_describe_prepared_failed, sizeof(__pyx_k_describe_prepared_failed), 0, 1, 0, 0},
   {0, __pyx_k_descriptions, sizeof(__pyx_k_descriptions), 0, 0, 1, 1},
   {0, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {0, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
   {0, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
   {0, __pyx_k_dispchar, sizeof(__pyx_k_dispchar), 0, 0, 1, 1},
   {0, __pyx_k_dispsize, sizeof(__pyx_k_dispsize), 0, 0, 1, 1},
   {0, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
@@ -27586,14 +27983,16 @@
   {0, __pyx_k_escape_string_failed, sizeof(__pyx_k_escape_string_failed), 0, 1, 0, 0},
   {0, __pyx_k_exc, sizeof(__pyx_k_exc), 0, 0, 1, 1},
   {0, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {0, __pyx_k_exec, sizeof(__pyx_k_exec), 0, 0, 1, 1},
   {0, __pyx_k_exec_params, sizeof(__pyx_k_exec_params), 0, 0, 1, 1},
   {0, __pyx_k_exec_prepared, sizeof(__pyx_k_exec_prepared), 0, 0, 1, 1},
   {0, __pyx_k_exec_status, sizeof(__pyx_k_exec_status), 0, 0, 1, 1},
+  {0, __pyx_k_executing_prepared_query_failed, sizeof(__pyx_k_executing_prepared_query_failed), 0, 1, 0, 0},
+  {0, __pyx_k_executing_query_failed, sizeof(__pyx_k_executing_query_failed), 0, 1, 0, 0},
   {0, __pyx_k_exit_pipeline_mode, sizeof(__pyx_k_exit_pipeline_mode), 0, 0, 1, 1},
   {0, __pyx_k_failed_to_enter_pipeline_mode, sizeof(__pyx_k_failed_to_enter_pipeline_mode), 0, 1, 0, 0},
   {0, __pyx_k_failed_to_sync_pipeline, sizeof(__pyx_k_failed_to_sync_pipeline), 0, 1, 0, 0},
   {0, __pyx_k_fformat, sizeof(__pyx_k_fformat), 0, 0, 1, 1},
   {0, __pyx_k_fieldcode, sizeof(__pyx_k_fieldcode), 0, 0, 1, 1},
   {0, __pyx_k_fileno, sizeof(__pyx_k_fileno), 0, 0, 1, 1},
   {0, __pyx_k_finish, sizeof(__pyx_k_finish), 0, 0, 1, 1},
@@ -27665,14 +28064,15 @@
   {0, __pyx_k_pgresult, sizeof(__pyx_k_pgresult), 0, 0, 1, 1},
   {0, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {0, __pyx_k_ping, sizeof(__pyx_k_ping), 0, 0, 1, 1},
   {0, __pyx_k_pipeline_sync, sizeof(__pyx_k_pipeline_sync), 0, 0, 1, 1},
   {0, __pyx_k_platform, sizeof(__pyx_k_platform), 0, 0, 1, 1},
   {0, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {0, __pyx_k_prepare_2, sizeof(__pyx_k_prepare_2), 0, 0, 1, 1},
+  {0, __pyx_k_preparing_query_failed, sizeof(__pyx_k_preparing_query_failed), 0, 1, 0, 0},
   {0, __pyx_k_psycopg, sizeof(__pyx_k_psycopg), 0, 0, 1, 1},
   {0, __pyx_k_psycopg, sizeof(__pyx_k_psycopg), 0, 1, 0, 1},
   {0, __pyx_k_psycopg_c_pq, sizeof(__pyx_k_psycopg_c_pq), 0, 0, 1, 1},
   {0, __pyx_k_psycopg_c_pq_conninfo_pyx, sizeof(__pyx_k_psycopg_c_pq_conninfo_pyx), 0, 0, 1, 0},
   {0, __pyx_k_psycopg_c_pq_escaping_pyx, sizeof(__pyx_k_psycopg_c_pq_escaping_pyx), 0, 0, 1, 0},
   {0, __pyx_k_psycopg_c_pq_pgcancel_pyx, sizeof(__pyx_k_psycopg_c_pq_pgcancel_pyx), 0, 0, 1, 0},
   {0, __pyx_k_psycopg_c_pq_pgconn_pyx, sizeof(__pyx_k_psycopg_c_pq_pgconn_pyx), 0, 0, 1, 0},
@@ -27864,23 +28264,23 @@
   {&__pyx_n_s_Trace, __pyx_k_Trace, sizeof(__pyx_k_Trace), 0, 0, 1, 1},
   {&__pyx_kp_s_Tuple_int_memoryview, __pyx_k_Tuple_int_memoryview, sizeof(__pyx_k_Tuple_int_memoryview), 0, 0, 1, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_ViewBuffer, __pyx_k_ViewBuffer, sizeof(__pyx_k_ViewBuffer), 0, 0, 1, 1},
   {&__pyx_n_s_ViewBuffer___reduce_cython, __pyx_k_ViewBuffer___reduce_cython, sizeof(__pyx_k_ViewBuffer___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_ViewBuffer___setstate_cython, __pyx_k_ViewBuffer___setstate_cython, sizeof(__pyx_k_ViewBuffer___setstate_cython), 0, 0, 1, 1},
-  {&__pyx_kp_b__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 0, 0, 0},
-  {&__pyx_n_s__135, __pyx_k__135, sizeof(__pyx_k__135), 0, 0, 1, 1},
-  {&__pyx_kp_u__14, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 0},
+  {&__pyx_kp_b__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 0, 0},
+  {&__pyx_kp_u__13, __pyx_k__13, sizeof(__pyx_k__13), 0, 1, 0, 0},
+  {&__pyx_n_s__134, __pyx_k__134, sizeof(__pyx_k__134), 0, 0, 1, 1},
+  {&__pyx_kp_u__16, __pyx_k__16, sizeof(__pyx_k__16), 0, 1, 0, 0},
   {&__pyx_kp_u__17, __pyx_k__17, sizeof(__pyx_k__17), 0, 1, 0, 0},
   {&__pyx_kp_u__18, __pyx_k__18, sizeof(__pyx_k__18), 0, 1, 0, 0},
   {&__pyx_kp_u__19, __pyx_k__19, sizeof(__pyx_k__19), 0, 1, 0, 0},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-  {&__pyx_kp_u__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 1, 0, 0},
-  {&__pyx_n_s__22, __pyx_k__22, sizeof(__pyx_k__22), 0, 0, 1, 1},
+  {&__pyx_n_s__21, __pyx_k__21, sizeof(__pyx_k__21), 0, 0, 1, 1},
   {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
   {&__pyx_n_s_algorithm, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
   {&__pyx_n_u_ascii, __pyx_k_ascii, sizeof(__pyx_k_ascii), 0, 1, 0, 1},
   {&__pyx_n_s_async, __pyx_k_async, sizeof(__pyx_k_async), 0, 0, 1, 1},
   {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
   {&__pyx_kp_u_at_0x, __pyx_k_at_0x, sizeof(__pyx_k_at_0x), 0, 1, 0, 0},
@@ -27920,15 +28320,14 @@
   {&__pyx_n_s_connect_start, __pyx_k_connect_start, sizeof(__pyx_k_connect_start), 0, 0, 1, 1},
   {&__pyx_kp_u_connection_not_in_pipeline_mode, __pyx_k_connection_not_in_pipeline_mode, sizeof(__pyx_k_connection_not_in_pipeline_mode), 0, 1, 0, 0},
   {&__pyx_n_s_connection_summary, __pyx_k_connection_summary, sizeof(__pyx_k_connection_summary), 0, 0, 1, 1},
   {&__pyx_n_s_conninfo, __pyx_k_conninfo, sizeof(__pyx_k_conninfo), 0, 0, 1, 1},
   {&__pyx_n_s_consume_input, __pyx_k_consume_input, sizeof(__pyx_k_consume_input), 0, 0, 1, 1},
   {&__pyx_kp_u_consuming_input_failed, __pyx_k_consuming_input_failed, sizeof(__pyx_k_consuming_input_failed), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_allocate_PGconn, __pyx_k_couldn_t_allocate_PGconn, sizeof(__pyx_k_couldn_t_allocate_PGconn), 0, 1, 0, 0},
-  {&__pyx_kp_u_couldn_t_allocate_PGresult, __pyx_k_couldn_t_allocate_PGresult, sizeof(__pyx_k_couldn_t_allocate_PGresult), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_allocate_connection_def, __pyx_k_couldn_t_allocate_connection_def, sizeof(__pyx_k_couldn_t_allocate_connection_def), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_allocate_connection_inf, __pyx_k_couldn_t_allocate_connection_inf, sizeof(__pyx_k_couldn_t_allocate_connection_inf), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_allocate_empty_PGresult, __pyx_k_couldn_t_allocate_empty_PGresult, sizeof(__pyx_k_couldn_t_allocate_empty_PGresult), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_allocate_for_escape_byt, __pyx_k_couldn_t_allocate_for_escape_byt, sizeof(__pyx_k_couldn_t_allocate_for_escape_byt), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_allocate_for_unescape_b, __pyx_k_couldn_t_allocate_for_unescape_b, sizeof(__pyx_k_couldn_t_allocate_for_unescape_b), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_allocate_on_conninfo_pa, __pyx_k_couldn_t_allocate_on_conninfo_pa, sizeof(__pyx_k_couldn_t_allocate_on_conninfo_pa), 0, 1, 0, 0},
   {&__pyx_kp_u_couldn_t_create_cancel_object, __pyx_k_couldn_t_create_cancel_object, sizeof(__pyx_k_couldn_t_create_cancel_object), 0, 1, 0, 0},
@@ -27939,14 +28338,15 @@
   {&__pyx_n_s_cvalues, __pyx_k_cvalues, sizeof(__pyx_k_cvalues), 0, 0, 1, 1},
   {&__pyx_n_u_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 1, 0, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_descr, __pyx_k_descr, sizeof(__pyx_k_descr), 0, 0, 1, 1},
   {&__pyx_n_s_describe_portal, __pyx_k_describe_portal, sizeof(__pyx_k_describe_portal), 0, 0, 1, 1},
   {&__pyx_n_s_describe_prepared, __pyx_k_describe_prepared, sizeof(__pyx_k_describe_prepared), 0, 0, 1, 1},
+  {&__pyx_kp_u_describe_prepared_failed, __pyx_k_describe_prepared_failed, sizeof(__pyx_k_describe_prepared_failed), 0, 1, 0, 0},
   {&__pyx_n_s_descriptions, __pyx_k_descriptions, sizeof(__pyx_k_descriptions), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
   {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
   {&__pyx_n_s_dispchar, __pyx_k_dispchar, sizeof(__pyx_k_dispchar), 0, 0, 1, 1},
   {&__pyx_n_s_dispsize, __pyx_k_dispsize, sizeof(__pyx_k_dispsize), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
@@ -27972,14 +28372,16 @@
   {&__pyx_kp_u_escape_string_failed, __pyx_k_escape_string_failed, sizeof(__pyx_k_escape_string_failed), 0, 1, 0, 0},
   {&__pyx_n_s_exc, __pyx_k_exc, sizeof(__pyx_k_exc), 0, 0, 1, 1},
   {&__pyx_n_s_exception, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {&__pyx_n_s_exec, __pyx_k_exec, sizeof(__pyx_k_exec), 0, 0, 1, 1},
   {&__pyx_n_s_exec_params, __pyx_k_exec_params, sizeof(__pyx_k_exec_params), 0, 0, 1, 1},
   {&__pyx_n_s_exec_prepared, __pyx_k_exec_prepared, sizeof(__pyx_k_exec_prepared), 0, 0, 1, 1},
   {&__pyx_n_s_exec_status, __pyx_k_exec_status, sizeof(__pyx_k_exec_status), 0, 0, 1, 1},
+  {&__pyx_kp_u_executing_prepared_query_failed, __pyx_k_executing_prepared_query_failed, sizeof(__pyx_k_executing_prepared_query_failed), 0, 1, 0, 0},
+  {&__pyx_kp_u_executing_query_failed, __pyx_k_executing_query_failed, sizeof(__pyx_k_executing_query_failed), 0, 1, 0, 0},
   {&__pyx_n_s_exit_pipeline_mode, __pyx_k_exit_pipeline_mode, sizeof(__pyx_k_exit_pipeline_mode), 0, 0, 1, 1},
   {&__pyx_kp_u_failed_to_enter_pipeline_mode, __pyx_k_failed_to_enter_pipeline_mode, sizeof(__pyx_k_failed_to_enter_pipeline_mode), 0, 1, 0, 0},
   {&__pyx_kp_u_failed_to_sync_pipeline, __pyx_k_failed_to_sync_pipeline, sizeof(__pyx_k_failed_to_sync_pipeline), 0, 1, 0, 0},
   {&__pyx_n_s_fformat, __pyx_k_fformat, sizeof(__pyx_k_fformat), 0, 0, 1, 1},
   {&__pyx_n_s_fieldcode, __pyx_k_fieldcode, sizeof(__pyx_k_fieldcode), 0, 0, 1, 1},
   {&__pyx_n_s_fileno, __pyx_k_fileno, sizeof(__pyx_k_fileno), 0, 0, 1, 1},
   {&__pyx_n_s_finish, __pyx_k_finish, sizeof(__pyx_k_finish), 0, 0, 1, 1},
@@ -28051,14 +28453,15 @@
   {&__pyx_n_s_pgresult, __pyx_k_pgresult, sizeof(__pyx_k_pgresult), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_ping, __pyx_k_ping, sizeof(__pyx_k_ping), 0, 0, 1, 1},
   {&__pyx_n_s_pipeline_sync, __pyx_k_pipeline_sync, sizeof(__pyx_k_pipeline_sync), 0, 0, 1, 1},
   {&__pyx_n_s_platform, __pyx_k_platform, sizeof(__pyx_k_platform), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_prepare_2, __pyx_k_prepare_2, sizeof(__pyx_k_prepare_2), 0, 0, 1, 1},
+  {&__pyx_kp_u_preparing_query_failed, __pyx_k_preparing_query_failed, sizeof(__pyx_k_preparing_query_failed), 0, 1, 0, 0},
   {&__pyx_n_s_psycopg, __pyx_k_psycopg, sizeof(__pyx_k_psycopg), 0, 0, 1, 1},
   {&__pyx_n_u_psycopg, __pyx_k_psycopg, sizeof(__pyx_k_psycopg), 0, 1, 0, 1},
   {&__pyx_n_s_psycopg_c_pq, __pyx_k_psycopg_c_pq, sizeof(__pyx_k_psycopg_c_pq), 0, 0, 1, 1},
   {&__pyx_kp_s_psycopg_c_pq_conninfo_pyx, __pyx_k_psycopg_c_pq_conninfo_pyx, sizeof(__pyx_k_psycopg_c_pq_conninfo_pyx), 0, 0, 1, 0},
   {&__pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_k_psycopg_c_pq_escaping_pyx, sizeof(__pyx_k_psycopg_c_pq_escaping_pyx), 0, 0, 1, 0},
   {&__pyx_kp_s_psycopg_c_pq_pgcancel_pyx, __pyx_k_psycopg_c_pq_pgcancel_pyx, sizeof(__pyx_k_psycopg_c_pq_pgcancel_pyx), 0, 0, 1, 0},
   {&__pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_k_psycopg_c_pq_pgconn_pyx, sizeof(__pyx_k_psycopg_c_pq_pgconn_pyx), 0, 0, 1, 0},
@@ -28144,15 +28547,15 @@
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(0, 54, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 60, __pyx_L1_error)
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 138, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 292, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 688, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -28177,848 +28580,837 @@
  *         rv = _options_from_array(opts)
  *         libpq.PQconninfoFree(opts)
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_connection_inf); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "psycopg_c/pq/pgconn.pyx":210
- *             pgresult = libpq.PQexec(self._pgconn_ptr, command)
- *         if pgresult is NULL:
- *             raise MemoryError("couldn't allocate PGresult")             # <<<<<<<<<<<<<<
- * 
- *         return PGresult._from_ptr(pgresult)
- */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_PGresult); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-
-  /* "psycopg_c/pq/pgconn.pyx":550
+  /* "psycopg_c/pq/pgconn.pyx":556
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  *         if not rv:
  *             raise MemoryError("couldn't allocate empty PGresult")             # <<<<<<<<<<<<<<
  *         return PGresult._from_ptr(rv)
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_empty_PGresult); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 550, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_empty_PGresult); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 556, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "psycopg_c/pq/conninfo.pyx":15
  *         cdef libpq.PQconninfoOption *opts = libpq.PQconndefaults()
  *         if opts is NULL :
  *             raise MemoryError("couldn't allocate connection defaults")             # <<<<<<<<<<<<<<
  *         rv = _options_from_array(opts)
  *         libpq.PQconninfoFree(opts)
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_connection_def); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(5, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_connection_def); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(5, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "psycopg_c/pq/conninfo.pyx":26
  *         if opts is NULL:
  *             if errmsg is NULL:
  *                 raise MemoryError("couldn't allocate on conninfo parse")             # <<<<<<<<<<<<<<
  *             else:
  *                 exc = e.OperationalError(errmsg.decode("utf8", "replace"))
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_on_conninfo_pa); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(5, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_couldn_t_allocate_on_conninfo_pa); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(5, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x0804127, 0x3908a35, 0x0c1d0e2):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x0804127, 0x3908a35, 0x0c1d0e2) = (conn))" % __pyx_checksum
  */
-  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_8405287, __pyx_int_59804213, __pyx_int_12701922); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_int_8405287, __pyx_int_59804213, __pyx_int_12701922); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "psycopg_c/pq.pyx":15
  * from psycopg.pq.misc import error_message
  * 
  * logger = logging.getLogger("psycopg")             # <<<<<<<<<<<<<<
  * 
  * __impl__ = 'c'
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_n_u_psycopg); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_n_u_psycopg); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "psycopg_c/pq.pyx":21
  * 
  * 
  * def version():             # <<<<<<<<<<<<<<
  *     return libpq.PQlibVersion()
  * 
  */
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pyx, __pyx_n_s_version, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(2, 21, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pyx, __pyx_n_s_version, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(2, 21, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":56
  *         return f"<{cls} {info} at 0x{id(self):x}>"
  * 
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def connect(cls, const char *conninfo) -> PGconn:
  *         cdef libpq.PGconn* pgconn = libpq.PQconnectdb(conninfo)
  */
-  __pyx_tuple__25 = PyTuple_Pack(4, __pyx_n_s_cls, __pyx_n_s_conninfo, __pyx_n_s_conninfo, __pyx_n_s_pgconn); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_connect, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(4, __pyx_n_s_cls, __pyx_n_s_conninfo, __pyx_n_s_conninfo, __pyx_n_s_pgconn); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_connect, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 56, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":64
  *         return PGconn._from_ptr(pgconn)
  * 
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def connect_start(cls, const char *conninfo) -> PGconn:
  *         cdef libpq.PGconn* pgconn = libpq.PQconnectStart(conninfo)
  */
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_connect_start, 64, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_connect_start, 64, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 64, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":72
  *         return PGconn._from_ptr(pgconn)
  * 
  *     def connect_poll(self) -> int:             # <<<<<<<<<<<<<<
  *         return _call_int(self, <conn_int_f>libpq.PQconnectPoll)
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_connect_poll, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_connect_poll, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 72, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":75
  *         return _call_int(self, <conn_int_f>libpq.PQconnectPoll)
  * 
  *     def finish(self) -> None:             # <<<<<<<<<<<<<<
  *         if self._pgconn_ptr is not NULL:
  *             libpq.PQfinish(self._pgconn_ptr)
  */
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_finish, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_finish, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 75, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":97
  *         return rv
  * 
  *     def reset(self) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         libpq.PQreset(self._pgconn_ptr)
  */
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_reset, 97, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_reset, 97, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 97, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":101
  *         libpq.PQreset(self._pgconn_ptr)
  * 
  *     def reset_start(self) -> None:             # <<<<<<<<<<<<<<
  *         if not libpq.PQresetStart(self._pgconn_ptr):
  *             raise e.OperationalError("couldn't reset connection")
  */
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_reset_start, 101, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_reset_start, 101, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 101, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":105
  *             raise e.OperationalError("couldn't reset connection")
  * 
  *     def reset_poll(self) -> int:             # <<<<<<<<<<<<<<
  *         return _call_int(self, <conn_int_f>libpq.PQresetPoll)
  * 
  */
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_reset_poll, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_reset_poll, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 105, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":108
  *         return _call_int(self, <conn_int_f>libpq.PQresetPoll)
  * 
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def ping(self, const char *conninfo) -> int:
  *         return libpq.PQping(conninfo)
  */
-  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_conninfo, __pyx_n_s_conninfo); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_ping, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_conninfo, __pyx_n_s_conninfo); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_ping, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 108, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":161
  *         return libpq.PQtransactionStatus(self._pgconn_ptr)
  * 
  *     def parameter_status(self, const char *name) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef const char *rv = libpq.PQparameterStatus(self._pgconn_ptr, name)
  */
-  __pyx_tuple__36 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_name, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_parameter_status, 161, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_name, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_parameter_status, 161, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 161, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":204
  *         return bool(_call_int(self, <conn_int_f>libpq.PQsslInUse))
  * 
  *     def exec_(self, const char *command) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *pgresult
  */
-  __pyx_tuple__38 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_command, __pyx_n_s_pgresult); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exec, 204, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_command, __pyx_n_s_pgresult); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exec, 204, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 204, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":214
  *         return PGresult._from_ptr(pgresult)
  * 
  *     def send_query(self, const char *command) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv
  */
-  __pyx_tuple__40 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_command, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 214, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_query, 214, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_command, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_query, 214, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 214, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":222
  *             raise e.OperationalError(f"sending query failed: {error_message(self)}")
  * 
  *     def exec_params(             # <<<<<<<<<<<<<<
  *         self,
  *         const char *command,
  */
-  __pyx_tuple__42 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_param_values, __pyx_n_s_param_types, __pyx_n_s_param_formats, __pyx_n_s_result_format, __pyx_n_s_cnparams, __pyx_n_s_ctypes, __pyx_n_s_cvalues, __pyx_n_s_clengths, __pyx_n_s_cformats, __pyx_n_s_pgresult); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 222, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__42);
-  __Pyx_GIVEREF(__pyx_tuple__42);
-  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exec_params, 222, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_param_values, __pyx_n_s_param_types, __pyx_n_s_param_formats, __pyx_n_s_result_format, __pyx_n_s_cnparams, __pyx_n_s_ctypes, __pyx_n_s_cvalues, __pyx_n_s_clengths, __pyx_n_s_cformats, __pyx_n_s_pgresult); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exec_params, 222, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 222, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":250
  *         return PGresult._from_ptr(pgresult)
  * 
  *     def send_query_params(             # <<<<<<<<<<<<<<
  *         self,
  *         const char *command,
  */
-  __pyx_tuple__44 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_param_values, __pyx_n_s_param_types, __pyx_n_s_param_formats, __pyx_n_s_result_format, __pyx_n_s_cnparams, __pyx_n_s_ctypes, __pyx_n_s_cvalues, __pyx_n_s_clengths, __pyx_n_s_cformats, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_query_params, 250, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_command, __pyx_n_s_param_values, __pyx_n_s_param_types, __pyx_n_s_param_formats, __pyx_n_s_result_format, __pyx_n_s_cnparams, __pyx_n_s_ctypes, __pyx_n_s_cvalues, __pyx_n_s_clengths, __pyx_n_s_cformats, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_query_params, 250, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 250, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":279
  *             )
  * 
  *     def send_prepare(             # <<<<<<<<<<<<<<
  *         self,
  *         const char *name,
  */
-  __pyx_tuple__46 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_command, __pyx_n_s_param_types, __pyx_n_s_i, __pyx_n_s_nparams, __pyx_n_s_atypes, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 279, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__46);
-  __Pyx_GIVEREF(__pyx_tuple__46);
-  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_prepare, 279, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 279, __pyx_L1_error)
-  __pyx_tuple__48 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 279, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_tuple__45 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_command, __pyx_n_s_param_types, __pyx_n_s_i, __pyx_n_s_nparams, __pyx_n_s_atypes, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_prepare, 279, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
 
   /* "psycopg_c/pq/pgconn.pyx":306
  *             )
  * 
  *     def send_query_prepared(             # <<<<<<<<<<<<<<
  *         self,
  *         const char *name,
  */
-  __pyx_tuple__49 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_param_values, __pyx_n_s_param_formats, __pyx_n_s_result_format, __pyx_n_s_cnparams, __pyx_n_s_ctypes, __pyx_n_s_cvalues, __pyx_n_s_clengths, __pyx_n_s_cformats, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__49);
-  __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_query_prepared, 306, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_param_values, __pyx_n_s_param_formats, __pyx_n_s_result_format, __pyx_n_s_cnparams, __pyx_n_s_ctypes, __pyx_n_s_cvalues, __pyx_n_s_clengths, __pyx_n_s_cformats, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_query_prepared, 306, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 306, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":334
  *             )
  * 
  *     def prepare(             # <<<<<<<<<<<<<<
  *         self,
  *         const char *name,
  */
-  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_prepare, 334, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_prepare, 334, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 334, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgconn.pyx":359
  *         return PGresult._from_ptr(rv)
  * 
  *     def exec_prepared(             # <<<<<<<<<<<<<<
  *         self,
  *         const char *name,
  */
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exec_prepared, 359, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exec_prepared, 359, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 359, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":388
+  /* "psycopg_c/pq/pgconn.pyx":390
  *         return PGresult._from_ptr(rv)
  * 
  *     def describe_prepared(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  */
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_describe_prepared, 388, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_describe_prepared, 390, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 390, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":395
+  /* "psycopg_c/pq/pgconn.pyx":399
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_prepared(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  */
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_describe_prepared, 395, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 395, __pyx_L1_error)
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_describe_prepared, 399, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 399, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":403
+  /* "psycopg_c/pq/pgconn.pyx":407
  *             )
  * 
  *     def describe_portal(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  */
-  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_describe_portal, 403, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_describe_portal, 407, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 407, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":410
+  /* "psycopg_c/pq/pgconn.pyx":416
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_portal(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  */
-  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_describe_portal, 410, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_describe_portal, 416, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 416, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":418
+  /* "psycopg_c/pq/pgconn.pyx":424
  *             )
  * 
  *     def get_result(self) -> Optional["PGresult"]:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)
  *         if pgresult is NULL:
  */
-  __pyx_tuple__57 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pgresult); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 418, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__57);
-  __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_get_result, 418, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pgresult); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_get_result, 424, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 424, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":424
+  /* "psycopg_c/pq/pgconn.pyx":430
  *         return PGresult._from_ptr(pgresult)
  * 
  *     def consume_input(self) -> None:             # <<<<<<<<<<<<<<
  *         if 1 != libpq.PQconsumeInput(self._pgconn_ptr):
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  */
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_consume_input, 424, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_consume_input, 430, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 430, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":428
+  /* "psycopg_c/pq/pgconn.pyx":434
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  * 
  *     def is_busy(self) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         with nogil:
  */
-  __pyx_tuple__60 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 428, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__60);
-  __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_is_busy, 428, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_tuple__59 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 434, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__59);
+  __Pyx_GIVEREF(__pyx_tuple__59);
+  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_is_busy, 434, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 434, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":443
+  /* "psycopg_c/pq/pgconn.pyx":449
  *             raise e.OperationalError(f"setting nonblocking failed: {error_message(self)}")
  * 
  *     cpdef int flush(self) except -1:             # <<<<<<<<<<<<<<
  *         if self._pgconn_ptr == NULL:
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  */
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_flush, 443, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 443, __pyx_L1_error)
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_flush, 449, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 449, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":451
+  /* "psycopg_c/pq/pgconn.pyx":457
  *         return rv
  * 
  *     def set_single_row_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         if not libpq.PQsetSingleRowMode(self._pgconn_ptr):
  *             raise e.OperationalError("setting single row mode failed")
  */
-  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_set_single_row_mode, 451, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_set_single_row_mode, 457, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 457, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":455
+  /* "psycopg_c/pq/pgconn.pyx":461
  *             raise e.OperationalError("setting single row mode failed")
  * 
  *     def get_cancel(self) -> PGcancel:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)
  *         if not ptr:
  */
-  __pyx_tuple__64 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_ptr); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 455, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__64);
-  __Pyx_GIVEREF(__pyx_tuple__64);
-  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_get_cancel, 455, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_ptr); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__63);
+  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_get_cancel, 461, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 461, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":461
+  /* "psycopg_c/pq/pgconn.pyx":467
  *         return PGcancel._from_ptr(ptr)
  * 
  *     cpdef object notifies(self):             # <<<<<<<<<<<<<<
  *         cdef libpq.PGnotify *ptr
  *         with nogil:
  */
-  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_notifies, 461, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_notifies, 467, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 467, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":472
+  /* "psycopg_c/pq/pgconn.pyx":478
  *             return None
  * 
  *     def put_copy_data(self, buffer) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef char *cbuffer
  */
-  __pyx_tuple__67 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_buffer, __pyx_n_s_rv, __pyx_n_s_cbuffer, __pyx_n_s_length); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 472, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
-  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_put_copy_data, 472, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_tuple__66 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_buffer, __pyx_n_s_rv, __pyx_n_s_cbuffer, __pyx_n_s_length); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__66);
+  __Pyx_GIVEREF(__pyx_tuple__66);
+  __pyx_codeobj__67 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_put_copy_data, 478, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__67)) __PYX_ERR(0, 478, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":483
+  /* "psycopg_c/pq/pgconn.pyx":489
  *         return rv
  * 
  *     def put_copy_end(self, error: Optional[bytes] = None) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef const char *cerr = NULL
  */
-  __pyx_tuple__69 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_error, __pyx_n_s_rv, __pyx_n_s_cerr); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 483, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__69);
-  __Pyx_GIVEREF(__pyx_tuple__69);
-  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_put_copy_end, 483, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_tuple__68 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_error, __pyx_n_s_rv, __pyx_n_s_cerr); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__68);
+  __Pyx_GIVEREF(__pyx_tuple__68);
+  __pyx_codeobj__69 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_put_copy_end, 489, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__69)) __PYX_ERR(0, 489, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":493
+  /* "psycopg_c/pq/pgconn.pyx":499
  *         return rv
  * 
  *     def get_copy_data(self, int async_) -> Tuple[int, memoryview]:             # <<<<<<<<<<<<<<
  *         cdef char *buffer_ptr = NULL
  *         cdef int nbytes
  */
-  __pyx_tuple__71 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_async, __pyx_n_s_async, __pyx_n_s_buffer_ptr, __pyx_n_s_nbytes, __pyx_n_s_data); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(0, 493, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__71);
-  __Pyx_GIVEREF(__pyx_tuple__71);
-  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__71, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_get_copy_data, 493, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_tuple__70 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_async, __pyx_n_s_async, __pyx_n_s_buffer_ptr, __pyx_n_s_nbytes, __pyx_n_s_data); if (unlikely(!__pyx_tuple__70)) __PYX_ERR(0, 499, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__70);
+  __Pyx_GIVEREF(__pyx_tuple__70);
+  __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__70, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_get_copy_data, 499, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(0, 499, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":506
+  /* "psycopg_c/pq/pgconn.pyx":512
  *             return nbytes, b""  # won't parse it, doesn't really be memoryview
  * 
  *     def trace(self, fileno: int) -> None:             # <<<<<<<<<<<<<<
  *         if sys.platform != "linux":
  *             raise e.NotSupportedError("currently only supported on Linux")
  */
-  __pyx_tuple__73 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_fileno, __pyx_n_s_stream); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(0, 506, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__73);
-  __Pyx_GIVEREF(__pyx_tuple__73);
-  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__73, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_trace, 506, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_tuple__72 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_fileno, __pyx_n_s_stream); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__72);
+  __Pyx_GIVEREF(__pyx_tuple__72);
+  __pyx_codeobj__73 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__72, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_trace, 512, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__73)) __PYX_ERR(0, 512, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":512
+  /* "psycopg_c/pq/pgconn.pyx":518
  *         libpq.PQtrace(self._pgconn_ptr, stream)
  * 
  *     def set_trace_flags(self, flags: Trace) -> None:             # <<<<<<<<<<<<<<
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  */
-  __pyx_tuple__75 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(0, 512, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__75);
-  __Pyx_GIVEREF(__pyx_tuple__75);
-  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__75, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_set_trace_flags, 512, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_tuple__74 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__74);
+  __Pyx_GIVEREF(__pyx_tuple__74);
+  __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__74, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_set_trace_flags, 518, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(0, 518, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":520
+  /* "psycopg_c/pq/pgconn.pyx":526
  *         libpq.PQsetTraceFlags(self._pgconn_ptr, flags)
  * 
  *     def untrace(self) -> None:             # <<<<<<<<<<<<<<
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  */
-  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_untrace, 520, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_untrace, 526, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 526, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":523
+  /* "psycopg_c/pq/pgconn.pyx":529
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  *     def encrypt_password(             # <<<<<<<<<<<<<<
  *         self, const char *passwd, const char *user, algorithm = None
  *     ) -> bytes:
  */
-  __pyx_tuple__78 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_passwd, __pyx_n_s_user, __pyx_n_s_algorithm, __pyx_n_s_out, __pyx_n_s_calgo, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(0, 523, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__78);
-  __Pyx_GIVEREF(__pyx_tuple__78);
-  __pyx_codeobj__79 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__78, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_encrypt_password, 523, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__79)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_tuple__77 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_passwd, __pyx_n_s_user, __pyx_n_s_algorithm, __pyx_n_s_out, __pyx_n_s_calgo, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__77)) __PYX_ERR(0, 529, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__77);
+  __Pyx_GIVEREF(__pyx_tuple__77);
+  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__77, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_encrypt_password, 529, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(0, 529, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":546
+  /* "psycopg_c/pq/pgconn.pyx":552
  *         return rv
  * 
  *     def make_empty_result(self, int exec_status) -> PGresult:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *rv = libpq.PQmakeEmptyPGresult(
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  */
-  __pyx_tuple__80 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_exec_status, __pyx_n_s_exec_status, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__80)) __PYX_ERR(0, 546, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__80);
-  __Pyx_GIVEREF(__pyx_tuple__80);
-  __pyx_codeobj__81 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_make_empty_result, 546, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__81)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_tuple__79 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_exec_status, __pyx_n_s_exec_status, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__79);
+  __Pyx_GIVEREF(__pyx_tuple__79);
+  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_make_empty_result, 552, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(0, 552, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":564
+  /* "psycopg_c/pq/pgconn.pyx":570
  *         return status
  * 
  *     def enter_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Enter pipeline mode.
  * 
  */
-  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_enter_pipeline_mode, 564, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __pyx_codeobj__81 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_enter_pipeline_mode, 570, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__81)) __PYX_ERR(0, 570, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":578
+  /* "psycopg_c/pq/pgconn.pyx":584
  *             raise e.OperationalError("failed to enter pipeline mode")
  * 
  *     def exit_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Exit pipeline mode.
  * 
  */
-  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exit_pipeline_mode, 578, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 578, __pyx_L1_error)
+  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_exit_pipeline_mode, 584, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 584, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":592
+  /* "psycopg_c/pq/pgconn.pyx":598
  *             raise e.OperationalError(error_message(self))
  * 
  *     def pipeline_sync(self) -> None:             # <<<<<<<<<<<<<<
  *         """Mark a synchronization point in a pipeline.
  * 
  */
-  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_pipeline_sync, 592, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_pipeline_sync, 598, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 598, __pyx_L1_error)
 
-  /* "psycopg_c/pq/pgconn.pyx":609
+  /* "psycopg_c/pq/pgconn.pyx":615
  *             raise e.OperationalError("failed to sync pipeline")
  * 
  *     def send_flush_request(self) -> None:             # <<<<<<<<<<<<<<
  *         """Sends a request for the server to flush its output buffer.
  * 
  */
-  __pyx_codeobj__85 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_flush_request, 609, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__85)) __PYX_ERR(0, 609, __pyx_L1_error)
+  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgconn_pyx, __pyx_n_s_send_flush_request, 615, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 615, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__85 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__85)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_tuple__87 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__87)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__87);
-  __Pyx_GIVEREF(__pyx_tuple__87);
-  __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_tuple__86 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__86)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__86);
+  __Pyx_GIVEREF(__pyx_tuple__86);
+  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(1, 3, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":33
  *         return f"<{cls} [{status.name}] at 0x{id(self):x}>"
  * 
  *     def clear(self) -> None:             # <<<<<<<<<<<<<<
  *         if self._pgresult_ptr is not NULL:
  *             libpq.PQclear(self._pgresult_ptr)
  */
-  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_clear, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_clear, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(3, 33, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":53
  *         return libpq.PQresultErrorMessage(self._pgresult_ptr)
  * 
  *     def error_field(self, int fieldcode) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         cdef char * rv = libpq.PQresultErrorField(self._pgresult_ptr, fieldcode)
  *         if rv is not NULL:
  */
-  __pyx_tuple__90 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_fieldcode, __pyx_n_s_fieldcode, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__90)) __PYX_ERR(3, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__90);
-  __Pyx_GIVEREF(__pyx_tuple__90);
-  __pyx_codeobj__91 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__90, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_error_field, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__91)) __PYX_ERR(3, 53, __pyx_L1_error)
+  __pyx_tuple__89 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_fieldcode, __pyx_n_s_fieldcode, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__89)) __PYX_ERR(3, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__89);
+  __Pyx_GIVEREF(__pyx_tuple__89);
+  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__89, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_error_field, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(3, 53, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":68
  *         return libpq.PQnfields(self._pgresult_ptr)
  * 
  *     def fname(self, int column_number) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         cdef char *rv = libpq.PQfname(self._pgresult_ptr, column_number)
  *         if rv is not NULL:
  */
-  __pyx_tuple__92 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_column_number, __pyx_n_s_column_number, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__92)) __PYX_ERR(3, 68, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__92);
-  __Pyx_GIVEREF(__pyx_tuple__92);
-  __pyx_codeobj__93 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__92, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fname, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__93)) __PYX_ERR(3, 68, __pyx_L1_error)
+  __pyx_tuple__91 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_column_number, __pyx_n_s_column_number, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__91)) __PYX_ERR(3, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__91);
+  __Pyx_GIVEREF(__pyx_tuple__91);
+  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fname, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(3, 68, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":75
  *             return None
  * 
  *     def ftable(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQftable(self._pgresult_ptr, column_number)
  * 
  */
-  __pyx_tuple__94 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_column_number, __pyx_n_s_column_number); if (unlikely(!__pyx_tuple__94)) __PYX_ERR(3, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__94);
-  __Pyx_GIVEREF(__pyx_tuple__94);
-  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_ftable, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(3, 75, __pyx_L1_error)
+  __pyx_tuple__93 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_column_number, __pyx_n_s_column_number); if (unlikely(!__pyx_tuple__93)) __PYX_ERR(3, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__93);
+  __Pyx_GIVEREF(__pyx_tuple__93);
+  __pyx_codeobj__94 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_ftable, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__94)) __PYX_ERR(3, 75, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":78
  *         return libpq.PQftable(self._pgresult_ptr, column_number)
  * 
  *     def ftablecol(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQftablecol(self._pgresult_ptr, column_number)
  * 
  */
-  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_ftablecol, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(3, 78, __pyx_L1_error)
+  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_ftablecol, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(3, 78, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":81
  *         return libpq.PQftablecol(self._pgresult_ptr, column_number)
  * 
  *     def fformat(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQfformat(self._pgresult_ptr, column_number)
  * 
  */
-  __pyx_codeobj__97 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fformat, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__97)) __PYX_ERR(3, 81, __pyx_L1_error)
+  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fformat, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(3, 81, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":84
  *         return libpq.PQfformat(self._pgresult_ptr, column_number)
  * 
  *     def ftype(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQftype(self._pgresult_ptr, column_number)
  * 
  */
-  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_ftype, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(3, 84, __pyx_L1_error)
+  __pyx_codeobj__97 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_ftype, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__97)) __PYX_ERR(3, 84, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":87
  *         return libpq.PQftype(self._pgresult_ptr, column_number)
  * 
  *     def fmod(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQfmod(self._pgresult_ptr, column_number)
  * 
  */
-  __pyx_codeobj__99 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fmod, 87, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__99)) __PYX_ERR(3, 87, __pyx_L1_error)
+  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fmod, 87, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(3, 87, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":90
  *         return libpq.PQfmod(self._pgresult_ptr, column_number)
  * 
  *     def fsize(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQfsize(self._pgresult_ptr, column_number)
  * 
  */
-  __pyx_codeobj__100 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fsize, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__100)) __PYX_ERR(3, 90, __pyx_L1_error)
+  __pyx_codeobj__99 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__93, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_fsize, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__99)) __PYX_ERR(3, 90, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":97
  *         return libpq.PQbinaryTuples(self._pgresult_ptr)
  * 
  *     def get_value(self, int row_number, int column_number) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         cdef int crow = row_number
  *         cdef int ccol = column_number
  */
-  __pyx_tuple__101 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_row_number, __pyx_n_s_column_number, __pyx_n_s_crow, __pyx_n_s_ccol, __pyx_n_s_length, __pyx_n_s_v); if (unlikely(!__pyx_tuple__101)) __PYX_ERR(3, 97, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__101);
-  __Pyx_GIVEREF(__pyx_tuple__101);
-  __pyx_codeobj__102 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__101, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_get_value, 97, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__102)) __PYX_ERR(3, 97, __pyx_L1_error)
+  __pyx_tuple__100 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_row_number, __pyx_n_s_column_number, __pyx_n_s_crow, __pyx_n_s_ccol, __pyx_n_s_length, __pyx_n_s_v); if (unlikely(!__pyx_tuple__100)) __PYX_ERR(3, 97, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__100);
+  __Pyx_GIVEREF(__pyx_tuple__100);
+  __pyx_codeobj__101 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__100, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_get_value, 97, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__101)) __PYX_ERR(3, 97, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":116
  *         return libpq.PQnparams(self._pgresult_ptr)
  * 
  *     def param_type(self, int param_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQparamtype(self._pgresult_ptr, param_number)
  * 
  */
-  __pyx_tuple__103 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_param_number, __pyx_n_s_param_number); if (unlikely(!__pyx_tuple__103)) __PYX_ERR(3, 116, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__103);
-  __Pyx_GIVEREF(__pyx_tuple__103);
-  __pyx_codeobj__104 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__103, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_param_type, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__104)) __PYX_ERR(3, 116, __pyx_L1_error)
+  __pyx_tuple__102 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_param_number, __pyx_n_s_param_number); if (unlikely(!__pyx_tuple__102)) __PYX_ERR(3, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__102);
+  __Pyx_GIVEREF(__pyx_tuple__102);
+  __pyx_codeobj__103 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__102, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_param_type, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__103)) __PYX_ERR(3, 116, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgresult.pyx":139
  *         return libpq.PQoidValue(self._pgresult_ptr)
  * 
  *     def set_attributes(self, descriptions: List[PGresAttDesc]):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t num = len(descriptions)
  *         cdef libpq.PGresAttDesc *attrs = <libpq.PGresAttDesc *>PyMem_Malloc(
  */
-  __pyx_tuple__105 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_descriptions, __pyx_n_s_num, __pyx_n_s_attrs, __pyx_n_s_i, __pyx_n_s_descr, __pyx_n_s_res); if (unlikely(!__pyx_tuple__105)) __PYX_ERR(3, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__105);
-  __Pyx_GIVEREF(__pyx_tuple__105);
-  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__105, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_set_attributes, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(3, 139, __pyx_L1_error)
+  __pyx_tuple__104 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_descriptions, __pyx_n_s_num, __pyx_n_s_attrs, __pyx_n_s_i, __pyx_n_s_descr, __pyx_n_s_res); if (unlikely(!__pyx_tuple__104)) __PYX_ERR(3, 139, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__104);
+  __Pyx_GIVEREF(__pyx_tuple__104);
+  __pyx_codeobj__105 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__104, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgresult_pyx, __pyx_n_s_set_attributes, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__105)) __PYX_ERR(3, 139, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__107 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__107)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_codeobj__107 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__107)) __PYX_ERR(1, 3, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgcancel.pyx":21
  *         self.free()
  * 
  *     def free(self) -> None:             # <<<<<<<<<<<<<<
  *         if self.pgcancel_ptr is not NULL:
  *             libpq.PQfreeCancel(self.pgcancel_ptr)
  */
-  __pyx_codeobj__109 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgcancel_pyx, __pyx_n_s_free, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__109)) __PYX_ERR(4, 21, __pyx_L1_error)
+  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgcancel_pyx, __pyx_n_s_free, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(4, 21, __pyx_L1_error)
 
   /* "psycopg_c/pq/pgcancel.pyx":26
  *             self.pgcancel_ptr = NULL
  * 
  *     def cancel(self) -> None:             # <<<<<<<<<<<<<<
  *         cdef char buf[256]
  *         cdef int res = libpq.PQcancel(self.pgcancel_ptr, buf, sizeof(buf))
  */
-  __pyx_tuple__110 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_buf, __pyx_n_s_res); if (unlikely(!__pyx_tuple__110)) __PYX_ERR(4, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__110);
-  __Pyx_GIVEREF(__pyx_tuple__110);
-  __pyx_codeobj__111 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__110, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgcancel_pyx, __pyx_n_s_cancel, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__111)) __PYX_ERR(4, 26, __pyx_L1_error)
+  __pyx_tuple__109 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_buf, __pyx_n_s_res); if (unlikely(!__pyx_tuple__109)) __PYX_ERR(4, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__109);
+  __Pyx_GIVEREF(__pyx_tuple__109);
+  __pyx_codeobj__110 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__109, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_pgcancel_pyx, __pyx_n_s_cancel, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__110)) __PYX_ERR(4, 26, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__112 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__112)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__111 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__111)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__113 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__113)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_codeobj__112 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__112)) __PYX_ERR(1, 3, __pyx_L1_error)
 
   /* "psycopg_c/pq/conninfo.pyx":11
  * 
  * class Conninfo:
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def get_defaults(cls) -> List[ConninfoOption]:
  *         cdef libpq.PQconninfoOption *opts = libpq.PQconndefaults()
  */
-  __pyx_tuple__114 = PyTuple_Pack(3, __pyx_n_s_cls, __pyx_n_s_opts, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__114)) __PYX_ERR(5, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__114);
-  __Pyx_GIVEREF(__pyx_tuple__114);
-  __pyx_codeobj__115 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__114, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_conninfo_pyx, __pyx_n_s_get_defaults, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__115)) __PYX_ERR(5, 11, __pyx_L1_error)
+  __pyx_tuple__113 = PyTuple_Pack(3, __pyx_n_s_cls, __pyx_n_s_opts, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__113)) __PYX_ERR(5, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__113);
+  __Pyx_GIVEREF(__pyx_tuple__113);
+  __pyx_codeobj__114 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__113, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_conninfo_pyx, __pyx_n_s_get_defaults, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__114)) __PYX_ERR(5, 11, __pyx_L1_error)
 
   /* "psycopg_c/pq/conninfo.pyx":20
  *         return rv
  * 
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def parse(cls, const char *conninfo) -> List[ConninfoOption]:
  *         cdef char *errmsg = NULL
  */
-  __pyx_tuple__116 = PyTuple_Pack(6, __pyx_n_s_cls, __pyx_n_s_conninfo, __pyx_n_s_errmsg, __pyx_n_s_opts, __pyx_n_s_exc, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__116)) __PYX_ERR(5, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__116);
-  __Pyx_GIVEREF(__pyx_tuple__116);
-  __pyx_codeobj__117 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__116, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_conninfo_pyx, __pyx_n_s_parse, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__117)) __PYX_ERR(5, 20, __pyx_L1_error)
+  __pyx_tuple__115 = PyTuple_Pack(6, __pyx_n_s_cls, __pyx_n_s_conninfo, __pyx_n_s_errmsg, __pyx_n_s_opts, __pyx_n_s_exc, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__115)) __PYX_ERR(5, 20, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__115);
+  __Pyx_GIVEREF(__pyx_tuple__115);
+  __pyx_codeobj__116 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__115, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_conninfo_pyx, __pyx_n_s_parse, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__116)) __PYX_ERR(5, 20, __pyx_L1_error)
 
   /* "psycopg_c/pq/conninfo.pyx":36
  *         return rv
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"<{type(self).__name__} ({self.keyword.decode('ascii')})>"
  * 
  */
-  __pyx_codeobj__118 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_conninfo_pyx, __pyx_n_s_repr, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__118)) __PYX_ERR(5, 36, __pyx_L1_error)
+  __pyx_codeobj__117 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_conninfo_pyx, __pyx_n_s_repr, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__117)) __PYX_ERR(5, 36, __pyx_L1_error)
 
   /* "psycopg_c/pq/escaping.pyx":15
  *         self.conn = conn
  * 
  *     cpdef escape_literal(self, data):             # <<<<<<<<<<<<<<
  *         cdef char *out
  *         cdef char *ptr
  */
-  __pyx_tuple__119 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_data); if (unlikely(!__pyx_tuple__119)) __PYX_ERR(6, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__119);
-  __Pyx_GIVEREF(__pyx_tuple__119);
-  __pyx_codeobj__120 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__119, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_literal, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__120)) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_tuple__118 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_data); if (unlikely(!__pyx_tuple__118)) __PYX_ERR(6, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__118);
+  __Pyx_GIVEREF(__pyx_tuple__118);
+  __pyx_codeobj__119 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_literal, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__119)) __PYX_ERR(6, 15, __pyx_L1_error)
 
   /* "psycopg_c/pq/escaping.pyx":37
  *         return rv
  * 
  *     cpdef escape_identifier(self, data):             # <<<<<<<<<<<<<<
  *         cdef char *out
  *         cdef char *ptr
  */
-  __pyx_codeobj__121 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__119, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_identifier, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__121)) __PYX_ERR(6, 37, __pyx_L1_error)
+  __pyx_codeobj__120 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_identifier, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__120)) __PYX_ERR(6, 37, __pyx_L1_error)
 
   /* "psycopg_c/pq/escaping.pyx":59
  *         return rv
  * 
  *     cpdef escape_string(self, data):             # <<<<<<<<<<<<<<
  *         cdef int error
  *         cdef size_t len_out
  */
-  __pyx_codeobj__122 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__119, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_string, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__122)) __PYX_ERR(6, 59, __pyx_L1_error)
+  __pyx_codeobj__121 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_string, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__121)) __PYX_ERR(6, 59, __pyx_L1_error)
 
   /* "psycopg_c/pq/escaping.pyx":90
  *         return rv
  * 
  *     cpdef escape_bytea(self, data):             # <<<<<<<<<<<<<<
  *         cdef size_t len_out
  *         cdef unsigned char *out
  */
-  __pyx_codeobj__123 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__119, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_bytea, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__123)) __PYX_ERR(6, 90, __pyx_L1_error)
+  __pyx_codeobj__122 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_escape_bytea, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__122)) __PYX_ERR(6, 90, __pyx_L1_error)
 
   /* "psycopg_c/pq/escaping.pyx":116
  *         return rv
  * 
  *     cpdef unescape_bytea(self, const unsigned char *data):             # <<<<<<<<<<<<<<
  *         # not needed, but let's keep it symmetric with the escaping:
  *         # if a connection is passed in, it must be valid.
  */
-  __pyx_tuple__124 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_data); if (unlikely(!__pyx_tuple__124)) __PYX_ERR(6, 116, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__124);
-  __Pyx_GIVEREF(__pyx_tuple__124);
-  __pyx_codeobj__125 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__124, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_unescape_bytea, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__125)) __PYX_ERR(6, 116, __pyx_L1_error)
+  __pyx_tuple__123 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_data); if (unlikely(!__pyx_tuple__123)) __PYX_ERR(6, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__123);
+  __Pyx_GIVEREF(__pyx_tuple__123);
+  __pyx_codeobj__124 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__123, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_psycopg_c_pq_escaping_pyx, __pyx_n_s_unescape_bytea, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__124)) __PYX_ERR(6, 116, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_tuple__126 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__126)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__126);
-  __Pyx_GIVEREF(__pyx_tuple__126);
-  __pyx_codeobj__127 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__126, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__127)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__125 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__125)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__125);
+  __Pyx_GIVEREF(__pyx_tuple__125);
+  __pyx_codeobj__126 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__125, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__126)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Escaping, (type(self), 0x0804127, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Escaping__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__128 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__128)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_codeobj__127 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__127)) __PYX_ERR(1, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__129 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__129)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__128 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__128)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__130 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__130)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_codeobj__129 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__129)) __PYX_ERR(1, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__131 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__131)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__130 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__130)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__132 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__87, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__132)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_codeobj__131 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__131)) __PYX_ERR(1, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Escaping(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__133 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__133)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__133);
-  __Pyx_GIVEREF(__pyx_tuple__133);
-  __pyx_codeobj__134 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__133, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Escaping, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__134)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__132 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__132)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__132);
+  __Pyx_GIVEREF(__pyx_tuple__132);
+  __pyx_codeobj__133 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__132, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Escaping, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__133)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -29136,23 +29528,23 @@
   if (__Pyx_InitString(__pyx_string_tab[108], &__pyx_n_s_Trace) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[109], &__pyx_kp_s_Tuple_int_memoryview) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[110], &__pyx_n_s_TypeError) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[111], &__pyx_n_s_ValueError) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[112], &__pyx_n_s_ViewBuffer) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[113], &__pyx_n_s_ViewBuffer___reduce_cython) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[114], &__pyx_n_s_ViewBuffer___setstate_cython) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[115], &__pyx_kp_b__12) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[116], &__pyx_n_s__135) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[117], &__pyx_kp_u__14) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[118], &__pyx_kp_u__17) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[119], &__pyx_kp_u__18) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[120], &__pyx_kp_u__19) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[121], &__pyx_kp_u__2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[122], &__pyx_kp_u__20) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[123], &__pyx_n_s__22) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[115], &__pyx_kp_b__11) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[116], &__pyx_kp_u__13) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[117], &__pyx_n_s__134) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[118], &__pyx_kp_u__16) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[119], &__pyx_kp_u__17) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[120], &__pyx_kp_u__18) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[121], &__pyx_kp_u__19) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[122], &__pyx_kp_u__2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[123], &__pyx_n_s__21) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[124], &__pyx_kp_u__3) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[125], &__pyx_kp_u__4) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[126], &__pyx_n_s_algorithm) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[127], &__pyx_n_u_ascii) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[128], &__pyx_n_s_async) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[129], &__pyx_n_s_asyncio_coroutines) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[130], &__pyx_kp_u_at_0x) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
@@ -29192,33 +29584,33 @@
   if (__Pyx_InitString(__pyx_string_tab[164], &__pyx_n_s_connect_start) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[165], &__pyx_kp_u_connection_not_in_pipeline_mode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[166], &__pyx_n_s_connection_summary) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[167], &__pyx_n_s_conninfo) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[168], &__pyx_n_s_consume_input) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[169], &__pyx_kp_u_consuming_input_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[170], &__pyx_kp_u_couldn_t_allocate_PGconn) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[171], &__pyx_kp_u_couldn_t_allocate_PGresult) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[172], &__pyx_kp_u_couldn_t_allocate_connection_def) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[173], &__pyx_kp_u_couldn_t_allocate_connection_inf) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[174], &__pyx_kp_u_couldn_t_allocate_empty_PGresult) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[175], &__pyx_kp_u_couldn_t_allocate_for_escape_byt) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[176], &__pyx_kp_u_couldn_t_allocate_for_unescape_b) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[177], &__pyx_kp_u_couldn_t_allocate_on_conninfo_pa) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[178], &__pyx_kp_u_couldn_t_create_cancel_object) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[179], &__pyx_kp_u_couldn_t_reset_connection) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[180], &__pyx_n_s_crow) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[181], &__pyx_n_s_ctypes) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[182], &__pyx_kp_u_currently_only_supported_on_Linu) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[183], &__pyx_n_s_cvalues) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[184], &__pyx_n_u_d) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[185], &__pyx_n_s_data) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[186], &__pyx_n_s_decode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[187], &__pyx_n_s_descr) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[188], &__pyx_n_s_describe_portal) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[189], &__pyx_n_s_describe_prepared) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[171], &__pyx_kp_u_couldn_t_allocate_connection_def) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[172], &__pyx_kp_u_couldn_t_allocate_connection_inf) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[173], &__pyx_kp_u_couldn_t_allocate_empty_PGresult) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[174], &__pyx_kp_u_couldn_t_allocate_for_escape_byt) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[175], &__pyx_kp_u_couldn_t_allocate_for_unescape_b) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[176], &__pyx_kp_u_couldn_t_allocate_on_conninfo_pa) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[177], &__pyx_kp_u_couldn_t_create_cancel_object) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[178], &__pyx_kp_u_couldn_t_reset_connection) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[179], &__pyx_n_s_crow) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[180], &__pyx_n_s_ctypes) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[181], &__pyx_kp_u_currently_only_supported_on_Linu) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[182], &__pyx_n_s_cvalues) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[183], &__pyx_n_u_d) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[184], &__pyx_n_s_data) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[185], &__pyx_n_s_decode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[186], &__pyx_n_s_descr) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[187], &__pyx_n_s_describe_portal) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[188], &__pyx_n_s_describe_prepared) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[189], &__pyx_kp_u_describe_prepared_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[190], &__pyx_n_s_descriptions) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[191], &__pyx_n_s_dict) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[192], &__pyx_n_s_dict_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[193], &__pyx_kp_u_disable) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[194], &__pyx_n_s_dispchar) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[195], &__pyx_n_s_dispsize) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[196], &__pyx_n_s_doc) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
@@ -29244,176 +29636,179 @@
   if (__Pyx_InitString(__pyx_string_tab[216], &__pyx_kp_u_escape_string_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[217], &__pyx_n_s_exc) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[218], &__pyx_n_s_exception) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[219], &__pyx_n_s_exec) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[220], &__pyx_n_s_exec_params) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[221], &__pyx_n_s_exec_prepared) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[222], &__pyx_n_s_exec_status) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[223], &__pyx_n_s_exit_pipeline_mode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[224], &__pyx_kp_u_failed_to_enter_pipeline_mode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[225], &__pyx_kp_u_failed_to_sync_pipeline) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[226], &__pyx_n_s_fformat) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[227], &__pyx_n_s_fieldcode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[228], &__pyx_n_s_fileno) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[229], &__pyx_n_s_finish) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[230], &__pyx_n_s_flags) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[231], &__pyx_n_s_flush) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[232], &__pyx_kp_u_flush_request_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[233], &__pyx_kp_u_flushing_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[234], &__pyx_kp_u_flushing_failed_the_connection_i) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[235], &__pyx_n_s_fmod) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[236], &__pyx_n_s_fname) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[237], &__pyx_n_s_format) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[238], &__pyx_n_s_free) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[239], &__pyx_n_s_fsize) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[240], &__pyx_n_s_ftable) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[241], &__pyx_n_s_ftablecol) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[242], &__pyx_n_s_ftype) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[243], &__pyx_kp_u_gc) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[244], &__pyx_n_s_getLogger) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[245], &__pyx_n_s_get_cancel) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[246], &__pyx_n_s_get_copy_data) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[247], &__pyx_n_s_get_defaults) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[248], &__pyx_n_s_get_result) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[249], &__pyx_n_s_get_value) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[250], &__pyx_n_s_getstate) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[251], &__pyx_kp_u_got) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[252], &__pyx_n_s_i) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[253], &__pyx_n_s_id) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[254], &__pyx_n_s_impl) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[255], &__pyx_n_s_import) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[256], &__pyx_n_s_init_subclass) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[257], &__pyx_n_s_initializing) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[258], &__pyx_n_s_int) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[259], &__pyx_n_s_is_busy) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[260], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[261], &__pyx_kp_u_isenabled) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[262], &__pyx_n_s_keyword) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[263], &__pyx_n_s_label) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[264], &__pyx_n_s_length) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[265], &__pyx_n_u_linux) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[266], &__pyx_n_s_logger) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[267], &__pyx_n_s_logging) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[268], &__pyx_n_s_main) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[269], &__pyx_n_s_make_empty_result) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[270], &__pyx_n_s_metaclass) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[271], &__pyx_n_s_module) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[272], &__pyx_n_s_name) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[273], &__pyx_n_s_name_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[274], &__pyx_n_s_nbytes) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[275], &__pyx_n_s_new) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[276], &__pyx_kp_s_no_default___reduce___due_to_non) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[277], &__pyx_n_s_notifies) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[278], &__pyx_n_s_nparams) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[279], &__pyx_n_s_num) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[280], &__pyx_n_s_opts) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[281], &__pyx_n_s_out) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[282], &__pyx_n_s_param_formats) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[283], &__pyx_kp_u_param_formats_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[284], &__pyx_n_s_param_number) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[285], &__pyx_n_s_param_type) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[286], &__pyx_n_s_param_types) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[287], &__pyx_kp_u_param_types_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[288], &__pyx_n_s_param_values) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[289], &__pyx_kp_u_param_values_but) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[290], &__pyx_n_s_parameter_status) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[291], &__pyx_n_s_parse) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[292], &__pyx_n_s_passwd) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[293], &__pyx_kp_u_password_encryption_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[294], &__pyx_n_s_pgconn) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[295], &__pyx_n_s_pgresult) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[296], &__pyx_n_s_pickle) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[297], &__pyx_n_s_ping) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[298], &__pyx_n_s_pipeline_sync) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[299], &__pyx_n_s_platform) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[300], &__pyx_n_s_prepare) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[301], &__pyx_n_s_prepare_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[302], &__pyx_n_s_psycopg) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[303], &__pyx_n_u_psycopg) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[304], &__pyx_n_s_psycopg_c_pq) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[305], &__pyx_kp_s_psycopg_c_pq_conninfo_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[306], &__pyx_kp_s_psycopg_c_pq_escaping_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[307], &__pyx_kp_s_psycopg_c_pq_pgcancel_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[308], &__pyx_kp_s_psycopg_c_pq_pgconn_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[309], &__pyx_kp_s_psycopg_c_pq_pgresult_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[310], &__pyx_kp_s_psycopg_c_pq_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[311], &__pyx_n_s_psycopg_pq) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[312], &__pyx_n_s_psycopg_pq__enums) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[313], &__pyx_n_s_psycopg_pq_misc) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[314], &__pyx_n_s_ptr) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[315], &__pyx_n_s_put_copy_data) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[316], &__pyx_n_s_put_copy_end) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[317], &__pyx_n_s_pyx_PickleError) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[318], &__pyx_n_s_pyx_checksum) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[319], &__pyx_n_s_pyx_result) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[320], &__pyx_n_s_pyx_state) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[321], &__pyx_n_s_pyx_type) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[322], &__pyx_n_s_pyx_unpickle_Escaping) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[323], &__pyx_n_s_pyx_vtable) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[324], &__pyx_n_s_qualname) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[325], &__pyx_n_s_range) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[326], &__pyx_kp_u_receiving_copy_data_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[327], &__pyx_n_s_reduce) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[328], &__pyx_n_s_reduce_cython) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[329], &__pyx_n_s_reduce_ex) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[330], &__pyx_n_s_repr) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[331], &__pyx_n_s_res) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[332], &__pyx_n_s_reset) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[333], &__pyx_n_s_reset_poll) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[334], &__pyx_n_s_reset_start) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[335], &__pyx_n_s_result_format) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[336], &__pyx_n_s_return) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[337], &__pyx_n_s_row_number) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[338], &__pyx_n_s_rv) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[339], &__pyx_n_s_self) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[340], &__pyx_n_s_send_describe_portal) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[341], &__pyx_n_s_send_describe_prepared) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[342], &__pyx_n_s_send_flush_request) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[343], &__pyx_n_s_send_prepare) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[344], &__pyx_n_s_send_query) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[345], &__pyx_n_s_send_query_params) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[346], &__pyx_n_s_send_query_prepared) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[347], &__pyx_kp_u_sending_copy_data_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[348], &__pyx_kp_u_sending_copy_end_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[349], &__pyx_kp_u_sending_describe_prepared_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[350], &__pyx_kp_u_sending_prepared_query_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[351], &__pyx_kp_u_sending_query_and_params_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[352], &__pyx_kp_u_sending_query_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[353], &__pyx_n_s_set_attributes) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[354], &__pyx_n_s_set_name) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[355], &__pyx_n_s_set_single_row_mode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[356], &__pyx_n_s_set_trace_flags) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[357], &__pyx_n_s_setstate) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[358], &__pyx_n_s_setstate_cython) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[359], &__pyx_kp_u_setting_nonblocking_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[360], &__pyx_kp_u_setting_single_row_mode_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[361], &__pyx_n_s_spec) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[362], &__pyx_n_s_ssl) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[363], &__pyx_n_s_state) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[364], &__pyx_n_s_status) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[365], &__pyx_n_s_stream) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[366], &__pyx_kp_s_stringsource) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[367], &__pyx_n_s_super) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[368], &__pyx_n_s_sys) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[369], &__pyx_n_s_tableid) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[370], &__pyx_n_s_test) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[371], &__pyx_kp_u_the_connection_is_closed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[372], &__pyx_kp_u_the_connection_is_lost) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[373], &__pyx_n_s_trace) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[374], &__pyx_n_s_typid) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[375], &__pyx_n_s_typlen) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[376], &__pyx_n_s_unescape_bytea) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[377], &__pyx_n_s_untrace) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[378], &__pyx_n_s_update) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[379], &__pyx_n_s_use_setstate) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[380], &__pyx_n_s_user) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[381], &__pyx_n_s_v) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[382], &__pyx_n_s_val) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[383], &__pyx_n_s_version) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[384], &__pyx_n_u_x) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[223], &__pyx_kp_u_executing_prepared_query_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[224], &__pyx_kp_u_executing_query_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[225], &__pyx_n_s_exit_pipeline_mode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[226], &__pyx_kp_u_failed_to_enter_pipeline_mode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[227], &__pyx_kp_u_failed_to_sync_pipeline) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[228], &__pyx_n_s_fformat) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[229], &__pyx_n_s_fieldcode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[230], &__pyx_n_s_fileno) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[231], &__pyx_n_s_finish) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[232], &__pyx_n_s_flags) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[233], &__pyx_n_s_flush) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[234], &__pyx_kp_u_flush_request_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[235], &__pyx_kp_u_flushing_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[236], &__pyx_kp_u_flushing_failed_the_connection_i) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[237], &__pyx_n_s_fmod) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[238], &__pyx_n_s_fname) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[239], &__pyx_n_s_format) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[240], &__pyx_n_s_free) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[241], &__pyx_n_s_fsize) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[242], &__pyx_n_s_ftable) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[243], &__pyx_n_s_ftablecol) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[244], &__pyx_n_s_ftype) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[245], &__pyx_kp_u_gc) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[246], &__pyx_n_s_getLogger) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[247], &__pyx_n_s_get_cancel) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[248], &__pyx_n_s_get_copy_data) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[249], &__pyx_n_s_get_defaults) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[250], &__pyx_n_s_get_result) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[251], &__pyx_n_s_get_value) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[252], &__pyx_n_s_getstate) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[253], &__pyx_kp_u_got) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[254], &__pyx_n_s_i) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[255], &__pyx_n_s_id) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[256], &__pyx_n_s_impl) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[257], &__pyx_n_s_import) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[258], &__pyx_n_s_init_subclass) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[259], &__pyx_n_s_initializing) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[260], &__pyx_n_s_int) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[261], &__pyx_n_s_is_busy) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[262], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[263], &__pyx_kp_u_isenabled) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[264], &__pyx_n_s_keyword) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[265], &__pyx_n_s_label) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[266], &__pyx_n_s_length) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[267], &__pyx_n_u_linux) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[268], &__pyx_n_s_logger) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[269], &__pyx_n_s_logging) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[270], &__pyx_n_s_main) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[271], &__pyx_n_s_make_empty_result) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[272], &__pyx_n_s_metaclass) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[273], &__pyx_n_s_module) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[274], &__pyx_n_s_name) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[275], &__pyx_n_s_name_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[276], &__pyx_n_s_nbytes) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[277], &__pyx_n_s_new) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[278], &__pyx_kp_s_no_default___reduce___due_to_non) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[279], &__pyx_n_s_notifies) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[280], &__pyx_n_s_nparams) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[281], &__pyx_n_s_num) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[282], &__pyx_n_s_opts) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[283], &__pyx_n_s_out) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[284], &__pyx_n_s_param_formats) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[285], &__pyx_kp_u_param_formats_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[286], &__pyx_n_s_param_number) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[287], &__pyx_n_s_param_type) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[288], &__pyx_n_s_param_types) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[289], &__pyx_kp_u_param_types_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[290], &__pyx_n_s_param_values) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[291], &__pyx_kp_u_param_values_but) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[292], &__pyx_n_s_parameter_status) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[293], &__pyx_n_s_parse) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[294], &__pyx_n_s_passwd) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[295], &__pyx_kp_u_password_encryption_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[296], &__pyx_n_s_pgconn) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[297], &__pyx_n_s_pgresult) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[298], &__pyx_n_s_pickle) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[299], &__pyx_n_s_ping) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[300], &__pyx_n_s_pipeline_sync) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[301], &__pyx_n_s_platform) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[302], &__pyx_n_s_prepare) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[303], &__pyx_n_s_prepare_2) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[304], &__pyx_kp_u_preparing_query_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[305], &__pyx_n_s_psycopg) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[306], &__pyx_n_u_psycopg) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[307], &__pyx_n_s_psycopg_c_pq) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[308], &__pyx_kp_s_psycopg_c_pq_conninfo_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[309], &__pyx_kp_s_psycopg_c_pq_escaping_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[310], &__pyx_kp_s_psycopg_c_pq_pgcancel_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[311], &__pyx_kp_s_psycopg_c_pq_pgconn_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[312], &__pyx_kp_s_psycopg_c_pq_pgresult_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[313], &__pyx_kp_s_psycopg_c_pq_pyx) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[314], &__pyx_n_s_psycopg_pq) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[315], &__pyx_n_s_psycopg_pq__enums) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[316], &__pyx_n_s_psycopg_pq_misc) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[317], &__pyx_n_s_ptr) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[318], &__pyx_n_s_put_copy_data) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[319], &__pyx_n_s_put_copy_end) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[320], &__pyx_n_s_pyx_PickleError) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[321], &__pyx_n_s_pyx_checksum) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[322], &__pyx_n_s_pyx_result) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[323], &__pyx_n_s_pyx_state) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[324], &__pyx_n_s_pyx_type) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[325], &__pyx_n_s_pyx_unpickle_Escaping) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[326], &__pyx_n_s_pyx_vtable) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[327], &__pyx_n_s_qualname) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[328], &__pyx_n_s_range) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[329], &__pyx_kp_u_receiving_copy_data_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[330], &__pyx_n_s_reduce) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[331], &__pyx_n_s_reduce_cython) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[332], &__pyx_n_s_reduce_ex) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[333], &__pyx_n_s_repr) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[334], &__pyx_n_s_res) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[335], &__pyx_n_s_reset) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[336], &__pyx_n_s_reset_poll) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[337], &__pyx_n_s_reset_start) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[338], &__pyx_n_s_result_format) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[339], &__pyx_n_s_return) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[340], &__pyx_n_s_row_number) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[341], &__pyx_n_s_rv) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[342], &__pyx_n_s_self) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[343], &__pyx_n_s_send_describe_portal) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[344], &__pyx_n_s_send_describe_prepared) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[345], &__pyx_n_s_send_flush_request) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[346], &__pyx_n_s_send_prepare) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[347], &__pyx_n_s_send_query) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[348], &__pyx_n_s_send_query_params) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[349], &__pyx_n_s_send_query_prepared) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[350], &__pyx_kp_u_sending_copy_data_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[351], &__pyx_kp_u_sending_copy_end_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[352], &__pyx_kp_u_sending_describe_prepared_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[353], &__pyx_kp_u_sending_prepared_query_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[354], &__pyx_kp_u_sending_query_and_params_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[355], &__pyx_kp_u_sending_query_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[356], &__pyx_n_s_set_attributes) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[357], &__pyx_n_s_set_name) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[358], &__pyx_n_s_set_single_row_mode) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[359], &__pyx_n_s_set_trace_flags) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[360], &__pyx_n_s_setstate) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[361], &__pyx_n_s_setstate_cython) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[362], &__pyx_kp_u_setting_nonblocking_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[363], &__pyx_kp_u_setting_single_row_mode_failed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[364], &__pyx_n_s_spec) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[365], &__pyx_n_s_ssl) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[366], &__pyx_n_s_state) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[367], &__pyx_n_s_status) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[368], &__pyx_n_s_stream) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[369], &__pyx_kp_s_stringsource) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[370], &__pyx_n_s_super) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[371], &__pyx_n_s_sys) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[372], &__pyx_n_s_tableid) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[373], &__pyx_n_s_test) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[374], &__pyx_kp_u_the_connection_is_closed) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[375], &__pyx_kp_u_the_connection_is_lost) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[376], &__pyx_n_s_trace) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[377], &__pyx_n_s_typid) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[378], &__pyx_n_s_typlen) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[379], &__pyx_n_s_unescape_bytea) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[380], &__pyx_n_s_untrace) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[381], &__pyx_n_s_update) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[382], &__pyx_n_s_use_setstate) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[383], &__pyx_n_s_user) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[384], &__pyx_n_s_v) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[385], &__pyx_n_s_val) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[386], &__pyx_n_s_version) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[387], &__pyx_n_u_x) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   #endif
   #if !CYTHON_USE_MODULE_STATE
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(2, 1, __pyx_L1_error);
   #endif
   __pyx_int_8405287 = PyInt_FromLong(8405287L); if (unlikely(!__pyx_int_8405287)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_int_12701922 = PyInt_FromLong(12701922L); if (unlikely(!__pyx_int_12701922)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_int_59804213 = PyInt_FromLong(59804213L); if (unlikely(!__pyx_int_59804213)) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -30083,15 +30478,15 @@
  * __impl__ = 'c'
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 15, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_3) < 0) __PYX_ERR(2, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "psycopg_c/pq.pyx":17
  * logger = logging.getLogger("psycopg")
@@ -30117,15 +30512,15 @@
   /* "psycopg_c/pq.pyx":21
  * 
  * 
  * def version():             # <<<<<<<<<<<<<<
  *     return libpq.PQlibVersion()
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_1version, 0, __pyx_n_s_version, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 21, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_1version, 0, __pyx_n_s_version, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_t_3) < 0) __PYX_ERR(2, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "psycopg_c/pq/pgconn.pyx":25
  * from cpython.memoryview cimport PyMemoryView_FromObject
  * 
@@ -30200,15 +30595,15 @@
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def connect(cls, const char *conninfo) -> PGconn:
  *         cdef libpq.PGconn* pgconn = libpq.PQconnectdb(conninfo)
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_PGconn) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_7connect, __Pyx_CYFUNCTION_CLASSMETHOD | __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_connect, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_7connect, __Pyx_CYFUNCTION_CLASSMETHOD | __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_connect, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_connect, __pyx_t_2) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
   __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn, __pyx_n_s_connect); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
@@ -30226,15 +30621,15 @@
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def connect_start(cls, const char *conninfo) -> PGconn:
  *         cdef libpq.PGconn* pgconn = libpq.PQconnectStart(conninfo)
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_PGconn) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_9connect_start, __Pyx_CYFUNCTION_CLASSMETHOD | __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_connect_start, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_9connect_start, __Pyx_CYFUNCTION_CLASSMETHOD | __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_connect_start, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_connect_start, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
   __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn, __pyx_n_s_connect_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
@@ -30252,15 +30647,15 @@
  *     def connect_poll(self) -> int:             # <<<<<<<<<<<<<<
  *         return _call_int(self, <conn_int_f>libpq.PQconnectPoll)
  * 
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_11connect_poll, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_connect_poll, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_11connect_poll, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_connect_poll, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_connect_poll, __pyx_t_2) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30270,15 +30665,15 @@
  *     def finish(self) -> None:             # <<<<<<<<<<<<<<
  *         if self._pgconn_ptr is not NULL:
  *             libpq.PQfinish(self._pgconn_ptr)
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_13finish, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_finish, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_13finish, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_finish, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_finish, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30288,15 +30683,15 @@
  *     def reset(self) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         libpq.PQreset(self._pgconn_ptr)
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_15reset, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_reset, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_15reset, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_reset, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_reset, __pyx_t_2) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30306,15 +30701,15 @@
  *     def reset_start(self) -> None:             # <<<<<<<<<<<<<<
  *         if not libpq.PQresetStart(self._pgconn_ptr):
  *             raise e.OperationalError("couldn't reset connection")
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_17reset_start, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_reset_start, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_17reset_start, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_reset_start, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_reset_start, __pyx_t_3) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30324,15 +30719,15 @@
  *     def reset_poll(self) -> int:             # <<<<<<<<<<<<<<
  *         return _call_int(self, <conn_int_f>libpq.PQresetPoll)
  * 
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_19reset_poll, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_reset_poll, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_19reset_poll, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_reset_poll, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_reset_poll, __pyx_t_2) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30342,15 +30737,15 @@
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def ping(self, const char *conninfo) -> int:
  *         return libpq.PQping(conninfo)
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_21ping, __Pyx_CYFUNCTION_CLASSMETHOD | __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_ping, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_21ping, __Pyx_CYFUNCTION_CLASSMETHOD | __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_ping, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_ping, __pyx_t_3) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
   __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn, __pyx_n_s_ping); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
@@ -30368,15 +30763,15 @@
  *     def parameter_status(self, const char *name) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef const char *rv = libpq.PQparameterStatus(self._pgconn_ptr, name)
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_Optional_bytes) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_23parameter_status, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_parameter_status, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_23parameter_status, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_parameter_status, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_parameter_status, __pyx_t_3) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30386,15 +30781,15 @@
  *     def exec_(self, const char *command) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *pgresult
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_25exec_, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exec, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_25exec_, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exec, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_exec, __pyx_t_2) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30404,15 +30799,15 @@
  *     def send_query(self, const char *command) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_27send_query, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_query, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_27send_query, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_query, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_query, __pyx_t_3) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
@@ -30426,15 +30821,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PqFormat); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_k__8 = __pyx_t_4;
+  __pyx_k__7 = __pyx_t_4;
 
   /* "psycopg_c/pq/pgconn.pyx":227
  *         param_values: Optional[Sequence[Optional[bytes]]],
  *         param_types: Optional[Sequence[int]] = None,
  *         param_formats: Optional[Sequence[int]] = None,             # <<<<<<<<<<<<<<
  *         int result_format = PqFormat.TEXT,
  *     ) -> PGresult:
@@ -30477,15 +30872,15 @@
   __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_param_values, __pyx_kp_s_Optional_Sequence_Optional_bytes) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_param_types, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_param_formats, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_29exec_params, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exec_params, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_29exec_params, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exec_params, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_exec_params, __pyx_t_5) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
@@ -30501,15 +30896,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_PqFormat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_k__9 = __pyx_t_4;
+  __pyx_k__8 = __pyx_t_4;
 
   /* "psycopg_c/pq/pgconn.pyx":255
  *         param_values: Optional[Sequence[Optional[bytes]]],
  *         param_types: Optional[Sequence[int]] = None,
  *         param_formats: Optional[Sequence[int]] = None,             # <<<<<<<<<<<<<<
  *         int result_format = PqFormat.TEXT,
  *     ) -> None:
@@ -30552,15 +30947,15 @@
   __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_param_values, __pyx_kp_s_Optional_Sequence_Optional_bytes) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_param_types, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_param_formats, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_31send_query_params, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_query_params, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_31send_query_params, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_query_params, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_query_params, __pyx_t_2) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -30573,17 +30968,17 @@
  *         self,
  *         const char *name,
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_param_types, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_33send_prepare, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_prepare, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_33send_prepare, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_prepare, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__48);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__47);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_prepare, __pyx_t_5) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
   /* "psycopg_c/pq/pgconn.pyx":311
@@ -30596,15 +30991,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_PqFormat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_k__10 = __pyx_t_4;
+  __pyx_k__9 = __pyx_t_4;
 
   /* "psycopg_c/pq/pgconn.pyx":310
  *         const char *name,
  *         param_values: Optional[Sequence[Optional[bytes]]],
  *         param_formats: Optional[Sequence[int]] = None,             # <<<<<<<<<<<<<<
  *         int result_format = PqFormat.TEXT,
  *     ) -> None:
@@ -30643,15 +31038,15 @@
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_5);
   __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_param_values, __pyx_kp_s_Optional_Sequence_Optional_bytes) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_param_formats, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_35send_query_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_query_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_35send_query_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_query_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_query_prepared, __pyx_t_3) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -30664,17 +31059,17 @@
  *         self,
  *         const char *name,
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_param_types, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_37prepare, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_prepare, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_37prepare, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_prepare, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__48);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__47);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_prepare, __pyx_t_5) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
   /* "psycopg_c/pq/pgconn.pyx":364
@@ -30687,15 +31082,15 @@
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_PqFormat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_k__11 = __pyx_t_4;
+  __pyx_k__10 = __pyx_t_4;
 
   /* "psycopg_c/pq/pgconn.pyx":363
  *         const char *name,
  *         param_values: Optional[Sequence[bytes]],
  *         param_formats: Optional[Sequence[int]] = None,             # <<<<<<<<<<<<<<
  *         int result_format = PqFormat.TEXT,
  *     ) -> PGresult:
@@ -30734,450 +31129,450 @@
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_5);
   __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_param_values, __pyx_kp_s_Optional_Sequence_bytes) < 0) __PYX_ERR(0, 359, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_param_formats, __pyx_kp_s_Optional_Sequence_int) < 0) __PYX_ERR(0, 359, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 359, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_39exec_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exec_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_39exec_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exec_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_exec_prepared, __pyx_t_2) < 0) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":388
+  /* "psycopg_c/pq/pgconn.pyx":390
  *         return PGresult._from_ptr(rv)
  * 
  *     def describe_prepared(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePrepared(self._pgconn_ptr, name)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_41describe_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_describe_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_41describe_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_describe_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_describe_prepared, __pyx_t_5) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_describe_prepared, __pyx_t_5) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":395
+  /* "psycopg_c/pq/pgconn.pyx":399
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_prepared(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePrepared(self._pgconn_ptr, name)
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 395, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 395, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_43send_describe_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_describe_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 395, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_43send_describe_prepared, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_describe_prepared, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_describe_prepared, __pyx_t_2) < 0) __PYX_ERR(0, 395, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_describe_prepared, __pyx_t_2) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":403
+  /* "psycopg_c/pq/pgconn.pyx":407
  *             )
  * 
  *     def describe_portal(self, const char *name) -> PGresult:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef libpq.PGresult *rv = libpq.PQdescribePortal(self._pgconn_ptr, name)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 403, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_45describe_portal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_describe_portal, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 403, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_45describe_portal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_describe_portal, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_describe_portal, __pyx_t_5) < 0) __PYX_ERR(0, 403, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_describe_portal, __pyx_t_5) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":410
+  /* "psycopg_c/pq/pgconn.pyx":416
  *         return PGresult._from_ptr(rv)
  * 
  *     def send_describe_portal(self, const char *name) -> None:             # <<<<<<<<<<<<<<
  *         _ensure_pgconn(self)
  *         cdef int rv = libpq.PQsendDescribePortal(self._pgconn_ptr, name)
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 410, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_47send_describe_portal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_describe_portal, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_47send_describe_portal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_describe_portal, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_describe_portal, __pyx_t_2) < 0) __PYX_ERR(0, 410, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_describe_portal, __pyx_t_2) < 0) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":418
+  /* "psycopg_c/pq/pgconn.pyx":424
  *             )
  * 
  *     def get_result(self) -> Optional["PGresult"]:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *pgresult = libpq.PQgetResult(self._pgconn_ptr)
  *         if pgresult is NULL:
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_Optional_PGresult) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_49get_result, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_get_result, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_Optional_PGresult) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_49get_result, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_get_result, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_get_result, __pyx_t_5) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_get_result, __pyx_t_5) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":424
+  /* "psycopg_c/pq/pgconn.pyx":430
  *         return PGresult._from_ptr(pgresult)
  * 
  *     def consume_input(self) -> None:             # <<<<<<<<<<<<<<
  *         if 1 != libpq.PQconsumeInput(self._pgconn_ptr):
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_51consume_input, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_consume_input, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_51consume_input, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_consume_input, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_consume_input, __pyx_t_2) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_consume_input, __pyx_t_2) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":428
+  /* "psycopg_c/pq/pgconn.pyx":434
  *             raise e.OperationalError(f"consuming input failed: {error_message(self)}")
  * 
  *     def is_busy(self) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         with nogil:
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_53is_busy, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_is_busy, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 434, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_53is_busy, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_is_busy, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__60)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_is_busy, __pyx_t_5) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_is_busy, __pyx_t_5) < 0) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":443
+  /* "psycopg_c/pq/pgconn.pyx":449
  *             raise e.OperationalError(f"setting nonblocking failed: {error_message(self)}")
  * 
  *     cpdef int flush(self) except -1:             # <<<<<<<<<<<<<<
  *         if self._pgconn_ptr == NULL:
  *             raise e.OperationalError(f"flushing failed: the connection is closed")
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_55flush, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_flush, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 443, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_55flush, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_flush, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_flush, __pyx_t_5) < 0) __PYX_ERR(0, 443, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_flush, __pyx_t_5) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":451
+  /* "psycopg_c/pq/pgconn.pyx":457
  *         return rv
  * 
  *     def set_single_row_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         if not libpq.PQsetSingleRowMode(self._pgconn_ptr):
  *             raise e.OperationalError("setting single row mode failed")
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 451, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_57set_single_row_mode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_set_single_row_mode, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__63)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_57set_single_row_mode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_set_single_row_mode, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_set_single_row_mode, __pyx_t_2) < 0) __PYX_ERR(0, 451, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_set_single_row_mode, __pyx_t_2) < 0) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":455
+  /* "psycopg_c/pq/pgconn.pyx":461
  *             raise e.OperationalError("setting single row mode failed")
  * 
  *     def get_cancel(self) -> PGcancel:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGcancel *ptr = libpq.PQgetCancel(self._pgconn_ptr)
  *         if not ptr:
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGcancel) < 0) __PYX_ERR(0, 455, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_59get_cancel, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_get_cancel, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 455, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGcancel) < 0) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_59get_cancel, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_get_cancel, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_get_cancel, __pyx_t_5) < 0) __PYX_ERR(0, 455, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_get_cancel, __pyx_t_5) < 0) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":461
+  /* "psycopg_c/pq/pgconn.pyx":467
  *         return PGcancel._from_ptr(ptr)
  * 
  *     cpdef object notifies(self):             # <<<<<<<<<<<<<<
  *         cdef libpq.PGnotify *ptr
  *         with nogil:
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_61notifies, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_notifies, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_61notifies, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_notifies, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_notifies, __pyx_t_5) < 0) __PYX_ERR(0, 461, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_notifies, __pyx_t_5) < 0) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":472
+  /* "psycopg_c/pq/pgconn.pyx":478
  *             return None
  * 
  *     def put_copy_data(self, buffer) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef char *cbuffer
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 472, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_63put_copy_data, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_put_copy_data, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 472, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_63put_copy_data, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_put_copy_data, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__67)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_put_copy_data, __pyx_t_2) < 0) __PYX_ERR(0, 472, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_put_copy_data, __pyx_t_2) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":483
+  /* "psycopg_c/pq/pgconn.pyx":489
  *         return rv
  * 
  *     def put_copy_end(self, error: Optional[bytes] = None) -> int:             # <<<<<<<<<<<<<<
  *         cdef int rv
  *         cdef const char *cerr = NULL
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_error, __pyx_kp_s_Optional_bytes) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_65put_copy_end, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_put_copy_end, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 483, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_error, __pyx_kp_s_Optional_bytes) < 0) __PYX_ERR(0, 489, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_65put_copy_end, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_put_copy_end, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__69)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__48);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__47);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_put_copy_end, __pyx_t_5) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_put_copy_end, __pyx_t_5) < 0) __PYX_ERR(0, 489, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":493
+  /* "psycopg_c/pq/pgconn.pyx":499
  *         return rv
  * 
  *     def get_copy_data(self, int async_) -> Tuple[int, memoryview]:             # <<<<<<<<<<<<<<
  *         cdef char *buffer_ptr = NULL
  *         cdef int nbytes
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_Tuple_int_memoryview) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_67get_copy_data, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_get_copy_data, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_Tuple_int_memoryview) < 0) __PYX_ERR(0, 499, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_67get_copy_data, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_get_copy_data, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__71)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_get_copy_data, __pyx_t_2) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_get_copy_data, __pyx_t_2) < 0) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":506
+  /* "psycopg_c/pq/pgconn.pyx":512
  *             return nbytes, b""  # won't parse it, doesn't really be memoryview
  * 
  *     def trace(self, fileno: int) -> None:             # <<<<<<<<<<<<<<
  *         if sys.platform != "linux":
  *             raise e.NotSupportedError("currently only supported on Linux")
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_fileno, __pyx_n_s_int) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_69trace, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_trace, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__74)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_fileno, __pyx_n_s_int) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_69trace, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_trace, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__73)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_trace, __pyx_t_5) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_trace, __pyx_t_5) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":512
+  /* "psycopg_c/pq/pgconn.pyx":518
  *         libpq.PQtrace(self._pgconn_ptr, stream)
  * 
  *     def set_trace_flags(self, flags: Trace) -> None:             # <<<<<<<<<<<<<<
  *         if libpq.PG_VERSION_NUM < 140000:
  *             raise e.NotSupportedError(
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flags, __pyx_n_s_Trace) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_71set_trace_flags, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_set_trace_flags, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flags, __pyx_n_s_Trace) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_71set_trace_flags, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_set_trace_flags, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_set_trace_flags, __pyx_t_2) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_set_trace_flags, __pyx_t_2) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":520
+  /* "psycopg_c/pq/pgconn.pyx":526
  *         libpq.PQsetTraceFlags(self._pgconn_ptr, flags)
  * 
  *     def untrace(self) -> None:             # <<<<<<<<<<<<<<
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 520, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_73untrace, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_untrace, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 526, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_73untrace, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_untrace, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_untrace, __pyx_t_5) < 0) __PYX_ERR(0, 520, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_untrace, __pyx_t_5) < 0) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":523
+  /* "psycopg_c/pq/pgconn.pyx":529
  *         libpq.PQuntrace(self._pgconn_ptr)
  * 
  *     def encrypt_password(             # <<<<<<<<<<<<<<
  *         self, const char *passwd, const char *user, algorithm = None
  *     ) -> bytes:
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 529, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_bytes_2) < 0) __PYX_ERR(0, 523, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_75encrypt_password, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_encrypt_password, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 523, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_bytes_2) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_75encrypt_password, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_encrypt_password, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__78)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 529, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__48);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__47);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_encrypt_password, __pyx_t_2) < 0) __PYX_ERR(0, 523, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_encrypt_password, __pyx_t_2) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":546
+  /* "psycopg_c/pq/pgconn.pyx":552
  *         return rv
  * 
  *     def make_empty_result(self, int exec_status) -> PGresult:             # <<<<<<<<<<<<<<
  *         cdef libpq.PGresult *rv = libpq.PQmakeEmptyPGresult(
  *             self._pgconn_ptr, <libpq.ExecStatusType>exec_status)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 546, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_77make_empty_result, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_make_empty_result, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 546, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_PGresult) < 0) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_77make_empty_result, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_make_empty_result, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 552, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_make_empty_result, __pyx_t_5) < 0) __PYX_ERR(0, 546, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_make_empty_result, __pyx_t_5) < 0) __PYX_ERR(0, 552, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":564
+  /* "psycopg_c/pq/pgconn.pyx":570
  *         return status
  * 
  *     def enter_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Enter pipeline mode.
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 564, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_79enter_pipeline_mode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_enter_pipeline_mode, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 570, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_79enter_pipeline_mode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_enter_pipeline_mode, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_enter_pipeline_mode, __pyx_t_2) < 0) __PYX_ERR(0, 564, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_enter_pipeline_mode, __pyx_t_2) < 0) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":578
+  /* "psycopg_c/pq/pgconn.pyx":584
  *             raise e.OperationalError("failed to enter pipeline mode")
  * 
  *     def exit_pipeline_mode(self) -> None:             # <<<<<<<<<<<<<<
  *         """Exit pipeline mode.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 578, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 578, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_81exit_pipeline_mode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exit_pipeline_mode, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 584, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_81exit_pipeline_mode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_exit_pipeline_mode, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_exit_pipeline_mode, __pyx_t_5) < 0) __PYX_ERR(0, 578, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_exit_pipeline_mode, __pyx_t_5) < 0) __PYX_ERR(0, 584, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":592
+  /* "psycopg_c/pq/pgconn.pyx":598
  *             raise e.OperationalError(error_message(self))
  * 
  *     def pipeline_sync(self) -> None:             # <<<<<<<<<<<<<<
  *         """Mark a synchronization point in a pipeline.
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_83pipeline_sync, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_pipeline_sync, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_83pipeline_sync, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_pipeline_sync, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_pipeline_sync, __pyx_t_2) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_pipeline_sync, __pyx_t_2) < 0) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
-  /* "psycopg_c/pq/pgconn.pyx":609
+  /* "psycopg_c/pq/pgconn.pyx":615
  *             raise e.OperationalError("failed to sync pipeline")
  * 
  *     def send_flush_request(self) -> None:             # <<<<<<<<<<<<<<
  *         """Sends a request for the server to flush its output buffer.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 609, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 609, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_85send_flush_request, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_flush_request, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__85)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 609, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_85send_flush_request, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn_send_flush_request, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_flush_request, __pyx_t_5) < 0) __PYX_ERR(0, 609, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGconn->tp_dict, __pyx_n_s_send_flush_request, __pyx_t_5) < 0) __PYX_ERR(0, 615, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGconn);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_87__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__86)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_87__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__85)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_5) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_89__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_6PGconn_89__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGconn___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_5) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "psycopg_c/pq/pgresult.pyx":10
  * from cpython.mem cimport PyMem_Malloc, PyMem_Free
  * 
@@ -31226,15 +31621,15 @@
  *     def clear(self) -> None:             # <<<<<<<<<<<<<<
  *         if self._pgresult_ptr is not NULL:
  *             libpq.PQclear(self._pgresult_ptr)
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_7clear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_clear, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_7clear, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_clear, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_clear, __pyx_t_2) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31244,15 +31639,15 @@
  *     def error_field(self, int fieldcode) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         cdef char * rv = libpq.PQresultErrorField(self._pgresult_ptr, fieldcode)
  *         if rv is not NULL:
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_Optional_bytes) < 0) __PYX_ERR(3, 53, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_9error_field, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_error_field, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__91)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 53, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_9error_field, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_error_field, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_error_field, __pyx_t_5) < 0) __PYX_ERR(3, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31262,15 +31657,15 @@
  *     def fname(self, int column_number) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         cdef char *rv = libpq.PQfname(self._pgresult_ptr, column_number)
  *         if rv is not NULL:
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_Optional_bytes) < 0) __PYX_ERR(3, 68, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_11fname, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fname, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__93)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 68, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_11fname, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fname, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_fname, __pyx_t_2) < 0) __PYX_ERR(3, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31280,15 +31675,15 @@
  *     def ftable(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQftable(self._pgresult_ptr, column_number)
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(3, 75, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_13ftable, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_ftable, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 75, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_13ftable, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_ftable, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__94)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_ftable, __pyx_t_5) < 0) __PYX_ERR(3, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31298,15 +31693,15 @@
  *     def ftablecol(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQftablecol(self._pgresult_ptr, column_number)
  * 
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(3, 78, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_15ftablecol, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_ftablecol, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 78, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_15ftablecol, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_ftablecol, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_ftablecol, __pyx_t_2) < 0) __PYX_ERR(3, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31316,15 +31711,15 @@
  *     def fformat(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQfformat(self._pgresult_ptr, column_number)
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(3, 81, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_17fformat, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fformat, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__97)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 81, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_17fformat, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fformat, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_fformat, __pyx_t_5) < 0) __PYX_ERR(3, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31334,15 +31729,15 @@
  *     def ftype(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQftype(self._pgresult_ptr, column_number)
  * 
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(3, 84, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_19ftype, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_ftype, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 84, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_19ftype, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_ftype, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__97)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_ftype, __pyx_t_2) < 0) __PYX_ERR(3, 84, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31352,15 +31747,15 @@
  *     def fmod(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQfmod(self._pgresult_ptr, column_number)
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(3, 87, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_21fmod, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fmod, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 87, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_21fmod, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fmod, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_fmod, __pyx_t_5) < 0) __PYX_ERR(3, 87, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31370,15 +31765,15 @@
  *     def fsize(self, int column_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQfsize(self._pgresult_ptr, column_number)
  * 
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(3, 90, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_23fsize, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fsize, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 90, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_23fsize, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_fsize, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_fsize, __pyx_t_2) < 0) __PYX_ERR(3, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31388,15 +31783,15 @@
  *     def get_value(self, int row_number, int column_number) -> Optional[bytes]:             # <<<<<<<<<<<<<<
  *         cdef int crow = row_number
  *         cdef int ccol = column_number
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_Optional_bytes) < 0) __PYX_ERR(3, 97, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_25get_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_get_value, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__102)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 97, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_25get_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_get_value, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__101)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_get_value, __pyx_t_5) < 0) __PYX_ERR(3, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31406,15 +31801,15 @@
  *     def param_type(self, int param_number) -> int:             # <<<<<<<<<<<<<<
  *         return libpq.PQparamtype(self._pgresult_ptr, param_number)
  * 
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(3, 116, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_27param_type, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_param_type, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__104)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 116, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_27param_type, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_param_type, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__103)); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_param_type, __pyx_t_2) < 0) __PYX_ERR(3, 116, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
@@ -31424,54 +31819,54 @@
  *     def set_attributes(self, descriptions: List[PGresAttDesc]):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t num = len(descriptions)
  *         cdef libpq.PGresAttDesc *attrs = <libpq.PGresAttDesc *>PyMem_Malloc(
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_descriptions, __pyx_kp_s_List_PGresAttDesc) < 0) __PYX_ERR(3, 139, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_29set_attributes, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_set_attributes, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 139, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_29set_attributes, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult_set_attributes, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__105)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGresult->tp_dict, __pyx_n_s_set_attributes, __pyx_t_5) < 0) __PYX_ERR(3, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGresult);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_31__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__107)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_31__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_5) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_33__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGresult_33__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGresult___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__107)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_5) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "psycopg_c/pq/pgcancel.pyx":21
  *         self.free()
  * 
  *     def free(self) -> None:             # <<<<<<<<<<<<<<
  *         if self.pgcancel_ptr is not NULL:
  *             libpq.PQfreeCancel(self.pgcancel_ptr)
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(4, 21, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_5free, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel_free, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__109)); if (unlikely(!__pyx_t_2)) __PYX_ERR(4, 21, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_5free, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel_free, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_2)) __PYX_ERR(4, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGcancel->tp_dict, __pyx_n_s_free, __pyx_t_2) < 0) __PYX_ERR(4, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGcancel);
 
@@ -31481,39 +31876,39 @@
  *     def cancel(self) -> None:             # <<<<<<<<<<<<<<
  *         cdef char buf[256]
  *         cdef int res = libpq.PQcancel(self.pgcancel_ptr, buf, sizeof(buf))
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(4, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(4, 26, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_7cancel, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel_cancel, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 26, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_7cancel, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel_cancel, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__110)); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_PGcancel->tp_dict, __pyx_n_s_cancel, __pyx_t_5) < 0) __PYX_ERR(4, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_PGcancel);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__112)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_5) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__113)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PGcancel_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PGcancel___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__112)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_5) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "psycopg_c/pq/conninfo.pyx":7
  * # Copyright (C) 2020 The Psycopg Team
  * 
@@ -31551,15 +31946,15 @@
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def get_defaults(cls) -> List[ConninfoOption]:
  *         cdef libpq.PQconninfoOption *opts = libpq.PQconndefaults()
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_List_ConninfoOption) < 0) __PYX_ERR(5, 11, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Conninfo_1get_defaults, __Pyx_CYFUNCTION_CLASSMETHOD, __pyx_n_s_Conninfo_get_defaults, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__115)); if (unlikely(!__pyx_t_3)) __PYX_ERR(5, 11, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Conninfo_1get_defaults, __Pyx_CYFUNCTION_CLASSMETHOD, __pyx_n_s_Conninfo_get_defaults, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__114)); if (unlikely(!__pyx_t_3)) __PYX_ERR(5, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_Method_ClassMethod(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_defaults, __pyx_t_5) < 0) __PYX_ERR(5, 11, __pyx_L1_error)
@@ -31571,15 +31966,15 @@
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def parse(cls, const char *conninfo) -> List[ConninfoOption]:
  *         cdef char *errmsg = NULL
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_List_ConninfoOption) < 0) __PYX_ERR(5, 20, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Conninfo_3parse, __Pyx_CYFUNCTION_CLASSMETHOD, __pyx_n_s_Conninfo_parse, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__117)); if (unlikely(!__pyx_t_3)) __PYX_ERR(5, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Conninfo_3parse, __Pyx_CYFUNCTION_CLASSMETHOD, __pyx_n_s_Conninfo_parse, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__116)); if (unlikely(!__pyx_t_3)) __PYX_ERR(5, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_Method_ClassMethod(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_parse, __pyx_t_5) < 0) __PYX_ERR(5, 20, __pyx_L1_error)
@@ -31588,15 +31983,15 @@
   /* "psycopg_c/pq/conninfo.pyx":36
  *         return rv
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f"<{type(self).__name__} ({self.keyword.decode('ascii')})>"
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Conninfo_5__repr__, 0, __pyx_n_s_Conninfo___repr, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__118)); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Conninfo_5__repr__, 0, __pyx_n_s_Conninfo___repr, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__117)); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_repr, __pyx_t_5) < 0) __PYX_ERR(5, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "psycopg_c/pq/conninfo.pyx":10
  * 
  * 
@@ -31613,133 +32008,133 @@
   /* "psycopg_c/pq/escaping.pyx":15
  *         self.conn = conn
  * 
  *     cpdef escape_literal(self, data):             # <<<<<<<<<<<<<<
  *         cdef char *out
  *         cdef char *ptr
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_3escape_literal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_literal, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__120)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_3escape_literal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_literal, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__119)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_Escaping->tp_dict, __pyx_n_s_escape_literal, __pyx_t_2) < 0) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_Escaping);
 
   /* "psycopg_c/pq/escaping.pyx":37
  *         return rv
  * 
  *     cpdef escape_identifier(self, data):             # <<<<<<<<<<<<<<
  *         cdef char *out
  *         cdef char *ptr
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_5escape_identifier, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_identifier, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__121)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 37, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_5escape_identifier, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_identifier, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__120)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_Escaping->tp_dict, __pyx_n_s_escape_identifier, __pyx_t_2) < 0) __PYX_ERR(6, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_Escaping);
 
   /* "psycopg_c/pq/escaping.pyx":59
  *         return rv
  * 
  *     cpdef escape_string(self, data):             # <<<<<<<<<<<<<<
  *         cdef int error
  *         cdef size_t len_out
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_7escape_string, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_string, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__122)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 59, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_7escape_string, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_string, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__121)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_Escaping->tp_dict, __pyx_n_s_escape_string, __pyx_t_2) < 0) __PYX_ERR(6, 59, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_Escaping);
 
   /* "psycopg_c/pq/escaping.pyx":90
  *         return rv
  * 
  *     cpdef escape_bytea(self, data):             # <<<<<<<<<<<<<<
  *         cdef size_t len_out
  *         cdef unsigned char *out
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_9escape_bytea, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_bytea, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__123)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 90, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_9escape_bytea, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_escape_bytea, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__122)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_Escaping->tp_dict, __pyx_n_s_escape_bytea, __pyx_t_2) < 0) __PYX_ERR(6, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_Escaping);
 
   /* "psycopg_c/pq/escaping.pyx":116
  *         return rv
  * 
  *     cpdef unescape_bytea(self, const unsigned char *data):             # <<<<<<<<<<<<<<
  *         # not needed, but let's keep it symmetric with the escaping:
  *         # if a connection is passed in, it must be valid.
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_11unescape_bytea, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_unescape_bytea, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__125)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 116, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_11unescape_bytea, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping_unescape_bytea, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__124)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_Escaping->tp_dict, __pyx_n_s_unescape_bytea, __pyx_t_2) < 0) __PYX_ERR(6, 116, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_Escaping);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_13__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__127)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_13__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__126)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_Escaping->tp_dict, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_Escaping);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Escaping, (type(self), 0x0804127, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Escaping__set_state(self, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_15__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__128)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8Escaping_15__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Escaping___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__127)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_9psycopg_c_2pq_Escaping->tp_dict, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_9psycopg_c_2pq_Escaping);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PQBuffer_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PQBuffer___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__129)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PQBuffer_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PQBuffer___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__128)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PQBuffer_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PQBuffer___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__130)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_8PQBuffer_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PQBuffer___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__129)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_10ViewBuffer_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ViewBuffer___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__131)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_10ViewBuffer_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ViewBuffer___reduce_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__130)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_10ViewBuffer_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ViewBuffer___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__132)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_10ViewBuffer_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ViewBuffer___setstate_cython, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__131)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "psycopg_c/pq.pyx":34
  * 
  * # importing the ssl module sets up Python's libcrypto callbacks
@@ -31760,15 +32155,15 @@
   PQinitOpenSSL(1, 0);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Escaping(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_3__pyx_unpickle_Escaping, 0, __pyx_n_s_pyx_unpickle_Escaping, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__134)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9psycopg_c_2pq_3__pyx_unpickle_Escaping, 0, __pyx_n_s_pyx_unpickle_Escaping, NULL, __pyx_n_s_psycopg_c_pq, __pyx_d, ((PyObject *)__pyx_codeobj__133)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Escaping, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "psycopg_c/pq.pyx":1
  * """             # <<<<<<<<<<<<<<
  * libpq Python wrapper using cython bindings.
@@ -34501,15 +34896,15 @@
     imported_module = PyImport_GetModule(name);
 #endif
     return imported_module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__22;
+    PyObject *module, *from_list, *star = __pyx_n_s__21;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -37154,15 +37549,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__135));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__134));
     }
     return name;
 }
 #endif
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
```

### Comparing `psycopg-c-3.1.7/psycopg_c/pq.pxd` & `psycopg-c-3.1.8/psycopg_c/pq.pxd`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/psycopg_c/types/numutils.c` & `psycopg-c-3.1.8/psycopg_c/types/numutils.c`

 * *Files identical despite different names*

### Comparing `psycopg-c-3.1.7/psycopg_c.egg-info/PKG-INFO` & `psycopg-c-3.1.8/psycopg_c.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: psycopg-c
-Version: 3.1.7
+Version: 3.1.8
 Summary: PostgreSQL database adapter for Python -- C optimisation distribution
 Home-page: https://psycopg.org/psycopg3/
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://psycopg.org/
+Project-URL: Documentation, https://psycopg.org/psycopg3/docs/
+Project-URL: Changes, https://psycopg.org/psycopg3/docs/news.html
 Project-URL: Code, https://github.com/psycopg/psycopg
 Project-URL: Issue Tracker, https://github.com/psycopg/psycopg/issues
 Project-URL: Download, https://pypi.org/project/psycopg-c/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -60,9 +61,7 @@
 more details.
 
 .. __: https://github.com/psycopg/psycopg#readme
 .. __: https://www.psycopg.org/psycopg3/docs/basic/install.html
 
 
 Copyright (C) 2020 The Psycopg Team
-
-
```

### Comparing `psycopg-c-3.1.7/setup.cfg` & `psycopg-c-3.1.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 description = PostgreSQL database adapter for Python -- C optimisation distribution
 url = https://psycopg.org/psycopg3/
 author = Daniele Varrazzo
 author_email = daniele.varrazzo@gmail.com
 license = GNU Lesser General Public License v3 (LGPLv3)
 project_urls = 
 	Homepage = https://psycopg.org/
+	Documentation = https://psycopg.org/psycopg3/docs/
+	Changes = https://psycopg.org/psycopg3/docs/news.html
 	Code = https://github.com/psycopg/psycopg
 	Issue Tracker = https://github.com/psycopg/psycopg/issues
 	Download = https://pypi.org/project/psycopg-c/
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -29,15 +31,14 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license_files = LICENSE.txt
 
 [options]
 python_requires = >= 3.7
-setup_requires = Cython >= 3.0.0a11
 packages = find:
 zip_safe = False
 
 [options.package_data]
 psycopg_c = 
 	py.typed
 	*.pyi
```

### Comparing `psycopg-c-3.1.7/setup.py` & `psycopg-c-3.1.8/setup.py`

 * *Files identical despite different names*

