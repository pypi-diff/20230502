# Comparing `tmp/asyncscope-0.9.2.tar.gz` & `tmp/asyncscope-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncscope-0.9.2.tar", last modified: Tue Apr 25 12:10:16 2023, max compression
+gzip compressed data, was "asyncscope-0.9.3.tar", last modified: Tue Apr 25 16:57:28 2023, max compression
```

## Comparing `asyncscope-0.9.2.tar` & `asyncscope-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 12:10:16.607218 asyncscope-0.9.2/
--rw-r--r--   0 smurf      (501) smurf      (501)       70 2022-12-30 20:42:44.000000 asyncscope-0.9.2/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      151 2020-07-16 11:23:07.000000 asyncscope-0.9.2/.pylintrc
--rw-r--r--   0 smurf      (501) smurf      (501)      223 2020-07-16 10:37:48.000000 asyncscope-0.9.2/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)    11832 2023-04-25 12:10:16.607218 asyncscope-0.9.2/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)    11082 2022-12-30 18:51:11.000000 asyncscope-0.9.2/README.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 12:10:16.603218 asyncscope-0.9.2/asyncscope/
--rw-r--r--   0 smurf      (501) smurf      (501)    18257 2023-04-25 12:10:08.000000 asyncscope-0.9.2/asyncscope/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 12:10:16.603218 asyncscope-0.9.2/asyncscope.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)    11832 2023-04-25 12:10:15.000000 asyncscope-0.9.2/asyncscope.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)      308 2023-04-25 12:10:16.000000 asyncscope-0.9.2/asyncscope.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-04-25 12:10:15.000000 asyncscope-0.9.2/asyncscope.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       20 2023-04-25 12:10:15.000000 asyncscope-0.9.2/asyncscope.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       17 2023-04-25 12:10:15.000000 asyncscope-0.9.2/asyncscope.egg-info/top_level.txt
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 12:10:16.603218 asyncscope-0.9.2/examples/
--rw-r--r--   0 smurf      (501) smurf      (501)     1470 2021-03-31 09:18:05.000000 asyncscope-0.9.2/examples/scoped.py
--rw-r--r--   0 smurf      (501) smurf      (501)      138 2023-04-25 12:10:16.611218 asyncscope-0.9.2/setup.cfg
--rw-r--r--   0 smurf      (501) smurf      (501)     1128 2022-12-17 11:24:32.000000 asyncscope-0.9.2/setup.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 12:10:16.607218 asyncscope-0.9.2/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)     1157 2022-12-17 11:24:32.000000 asyncscope-0.9.2/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3976 2022-12-30 20:42:20.000000 asyncscope-0.9.2/tests/test_basic.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 16:57:28.449098 asyncscope-0.9.3/
+-rw-r--r--   0 smurf      (501) smurf      (501)       70 2023-04-25 16:57:27.000000 asyncscope-0.9.3/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      151 2020-07-16 11:23:07.000000 asyncscope-0.9.3/.pylintrc
+-rw-r--r--   0 smurf      (501) smurf      (501)      223 2020-07-16 10:37:48.000000 asyncscope-0.9.3/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)    11832 2023-04-25 16:57:28.449098 asyncscope-0.9.3/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)    11082 2022-12-30 18:51:11.000000 asyncscope-0.9.3/README.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 16:57:28.449098 asyncscope-0.9.3/asyncscope/
+-rw-r--r--   0 smurf      (501) smurf      (501)    18184 2023-04-25 16:57:06.000000 asyncscope-0.9.3/asyncscope/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 16:57:28.449098 asyncscope-0.9.3/asyncscope.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)    11832 2023-04-25 16:57:27.000000 asyncscope-0.9.3/asyncscope.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)      308 2023-04-25 16:57:28.000000 asyncscope-0.9.3/asyncscope.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-04-25 16:57:27.000000 asyncscope-0.9.3/asyncscope.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       20 2023-04-25 16:57:27.000000 asyncscope-0.9.3/asyncscope.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       17 2023-04-25 16:57:27.000000 asyncscope-0.9.3/asyncscope.egg-info/top_level.txt
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 16:57:28.449098 asyncscope-0.9.3/examples/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1470 2021-03-31 09:18:05.000000 asyncscope-0.9.3/examples/scoped.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      138 2023-04-25 16:57:28.453098 asyncscope-0.9.3/setup.cfg
+-rw-r--r--   0 smurf      (501) smurf      (501)     1128 2022-12-17 11:24:32.000000 asyncscope-0.9.3/setup.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-04-25 16:57:28.449098 asyncscope-0.9.3/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1157 2022-12-17 11:24:32.000000 asyncscope-0.9.3/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3976 2022-12-30 20:42:20.000000 asyncscope-0.9.3/tests/test_basic.py
```

### Comparing `asyncscope-0.9.2/PKG-INFO` & `asyncscope-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncscope
-Version: 0.9.2
+Version: 0.9.3
 Summary: Task scopes for AnyIO
 Home-page: http://github.com/M-o-a-T/asyncscope
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 License: GPLv3 or later
 Keywords: async
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `asyncscope-0.9.2/README.rst` & `asyncscope-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `asyncscope-0.9.2/asyncscope/__init__.py` & `asyncscope-0.9.3/asyncscope/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,16 +284,15 @@
                 if not self._new and current_scope is not None:
                     current_scope.requires(self)
 
                 try:
                     yield self
                 finally:
                     del self._set[self._name]
-                    with anyio.CancelScope(shield=True):
-                        await self.cancel_immediate()
+                    self.cancel_immediate()
 
         except Exception as exc:
             if self._data_lock.is_set():
                 raise
             self.logger.exception("Ugh %r", exc)
             self._error = exc
             self._data_lock.set()
@@ -450,15 +449,15 @@
         """
         self.logger.debug("Cancel dependents")
         for s in self.dependents:
             s.no_more()
             await s.wait()
         self.logger.debug("Cancel dependents done")
 
-    async def cancel_immediate(self):
+    def cancel_immediate(self):
         """
         Cancel this scope.
 
         This will cancel all scopes that depend on this one without waiting
         for them to terminate.
         """
         self.logger.debug("Cancel Immediate")
```

### Comparing `asyncscope-0.9.2/asyncscope.egg-info/PKG-INFO` & `asyncscope-0.9.3/asyncscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncscope
-Version: 0.9.2
+Version: 0.9.3
 Summary: Task scopes for AnyIO
 Home-page: http://github.com/M-o-a-T/asyncscope
 Author: Matthias Urlichs
 Author-email: matthias@urlichs.de
 License: GPLv3 or later
 Keywords: async
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `asyncscope-0.9.2/examples/scoped.py` & `asyncscope-0.9.3/examples/scoped.py`

 * *Files identical despite different names*

### Comparing `asyncscope-0.9.2/setup.py` & `asyncscope-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `asyncscope-0.9.2/tests/__init__.py` & `asyncscope-0.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncscope-0.9.2/tests/test_basic.py` & `asyncscope-0.9.3/tests/test_basic.py`

 * *Files identical despite different names*

