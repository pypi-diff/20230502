# Comparing `tmp/tlbx-0.1.8.tar.gz` & `tmp/tlbx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tlbx-0.1.8.tar", last modified: Wed Oct 16 15:45:13 2019, max compression
+gzip compressed data, was "dist/tlbx-0.1.9.tar", last modified: Sun Jan 12 16:40:09 2020, max compression
```

## Comparing `tlbx-0.1.8.tar` & `tlbx-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kurt       (501) staff       (20)        0 2019-10-16 15:45:13.000000 tlbx-0.1.8/
--rw-r--r--   0 kurt       (501) staff       (20)     1038 2019-10-16 15:45:13.000000 tlbx-0.1.8/PKG-INFO
--rw-r--r--   0 kurt       (501) staff       (20)      429 2019-09-22 13:02:11.000000 tlbx-0.1.8/README.md
--rw-r--r--   0 kurt       (501) staff       (20)       38 2019-10-16 15:45:13.000000 tlbx-0.1.8/setup.cfg
--rw-r--r--   0 kurt       (501) staff       (20)     1091 2019-10-06 23:12:32.000000 tlbx-0.1.8/setup.py
-drwxr-xr-x   0 kurt       (501) staff       (20)        0 2019-10-16 15:45:13.000000 tlbx-0.1.8/tlbx/
--rw-r--r--   0 kurt       (501) staff       (20)      315 2019-09-21 15:33:29.000000 tlbx-0.1.8/tlbx/__init__.py
--rw-r--r--   0 kurt       (501) staff       (20)     1697 2019-09-21 15:37:14.000000 tlbx-0.1.8/tlbx/callable_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)     1671 2019-09-25 15:55:20.000000 tlbx-0.1.8/tlbx/cli_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)       94 2019-09-21 15:37:13.000000 tlbx-0.1.8/tlbx/date_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)     2026 2019-09-05 19:35:30.000000 tlbx-0.1.8/tlbx/dict_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)     5702 2019-09-21 15:34:06.000000 tlbx-0.1.8/tlbx/email_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)      347 2019-09-21 15:37:13.000000 tlbx-0.1.8/tlbx/file_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)     1316 2019-10-16 15:40:32.000000 tlbx-0.1.8/tlbx/iterable_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)     5185 2019-09-25 14:13:54.000000 tlbx-0.1.8/tlbx/logging_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)     2170 2019-09-24 19:49:20.000000 tlbx-0.1.8/tlbx/object_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)      822 2019-09-05 19:35:30.000000 tlbx-0.1.8/tlbx/string_utils.py
--rw-r--r--   0 kurt       (501) staff       (20)       22 2019-10-16 15:42:21.000000 tlbx-0.1.8/tlbx/version.py
-drwxr-xr-x   0 kurt       (501) staff       (20)        0 2019-10-16 15:45:13.000000 tlbx-0.1.8/tlbx.egg-info/
--rw-r--r--   0 kurt       (501) staff       (20)     1038 2019-10-16 15:45:12.000000 tlbx-0.1.8/tlbx.egg-info/PKG-INFO
--rw-r--r--   0 kurt       (501) staff       (20)      395 2019-10-16 15:45:13.000000 tlbx-0.1.8/tlbx.egg-info/SOURCES.txt
--rw-r--r--   0 kurt       (501) staff       (20)        1 2019-10-16 15:45:12.000000 tlbx-0.1.8/tlbx.egg-info/dependency_links.txt
--rw-r--r--   0 kurt       (501) staff       (20)      117 2019-10-16 15:45:12.000000 tlbx-0.1.8/tlbx.egg-info/requires.txt
--rw-r--r--   0 kurt       (501) staff       (20)        5 2019-10-16 15:45:12.000000 tlbx-0.1.8/tlbx.egg-info/top_level.txt
+drwxr-xr-x   0 kurt       (501) staff       (20)        0 2020-01-12 16:40:09.000000 tlbx-0.1.9/
+-rw-r--r--   0 kurt       (501) staff       (20)     1038 2020-01-12 16:40:09.000000 tlbx-0.1.9/PKG-INFO
+-rw-r--r--   0 kurt       (501) staff       (20)      429 2019-09-22 13:02:11.000000 tlbx-0.1.9/README.md
+-rw-r--r--   0 kurt       (501) staff       (20)       38 2020-01-12 16:40:09.000000 tlbx-0.1.9/setup.cfg
+-rw-r--r--   0 kurt       (501) staff       (20)     1091 2019-10-06 23:12:32.000000 tlbx-0.1.9/setup.py
+drwxr-xr-x   0 kurt       (501) staff       (20)        0 2020-01-12 16:40:09.000000 tlbx-0.1.9/tlbx/
+-rw-r--r--   0 kurt       (501) staff       (20)      315 2019-09-21 15:33:29.000000 tlbx-0.1.9/tlbx/__init__.py
+-rw-r--r--   0 kurt       (501) staff       (20)     1697 2019-09-21 15:37:14.000000 tlbx-0.1.9/tlbx/callable_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)     1671 2019-10-24 22:27:49.000000 tlbx-0.1.9/tlbx/cli_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)       94 2019-09-21 15:37:13.000000 tlbx-0.1.9/tlbx/date_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)     2026 2019-09-05 19:35:30.000000 tlbx-0.1.9/tlbx/dict_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)     5702 2019-09-21 15:34:06.000000 tlbx-0.1.9/tlbx/email_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)     1476 2020-01-12 16:34:45.000000 tlbx-0.1.9/tlbx/file_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)     1316 2019-10-16 15:40:32.000000 tlbx-0.1.9/tlbx/iterable_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)     5195 2020-01-12 16:30:24.000000 tlbx-0.1.9/tlbx/logging_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)     2170 2019-09-24 19:49:20.000000 tlbx-0.1.9/tlbx/object_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)      822 2019-09-05 19:35:30.000000 tlbx-0.1.9/tlbx/string_utils.py
+-rw-r--r--   0 kurt       (501) staff       (20)       22 2020-01-12 16:34:35.000000 tlbx-0.1.9/tlbx/version.py
+drwxr-xr-x   0 kurt       (501) staff       (20)        0 2020-01-12 16:40:09.000000 tlbx-0.1.9/tlbx.egg-info/
+-rw-r--r--   0 kurt       (501) staff       (20)     1038 2020-01-12 16:40:09.000000 tlbx-0.1.9/tlbx.egg-info/PKG-INFO
+-rw-r--r--   0 kurt       (501) staff       (20)      395 2020-01-12 16:40:09.000000 tlbx-0.1.9/tlbx.egg-info/SOURCES.txt
+-rw-r--r--   0 kurt       (501) staff       (20)        1 2020-01-12 16:40:09.000000 tlbx-0.1.9/tlbx.egg-info/dependency_links.txt
+-rw-r--r--   0 kurt       (501) staff       (20)      124 2020-01-12 16:40:09.000000 tlbx-0.1.9/tlbx.egg-info/requires.txt
+-rw-r--r--   0 kurt       (501) staff       (20)        5 2020-01-12 16:40:09.000000 tlbx-0.1.9/tlbx.egg-info/top_level.txt
```

### Comparing `tlbx-0.1.8/PKG-INFO` & `tlbx-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlbx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Just some common utilities.
 Home-page: https://github.com/totalhack/tlbx
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: MIT
 Description: tlbx: just some common utilities
```

### Comparing `tlbx-0.1.8/setup.py` & `tlbx-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx/callable_utils.py` & `tlbx-0.1.9/tlbx/callable_utils.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx/cli_utils.py` & `tlbx-0.1.9/tlbx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx/dict_utils.py` & `tlbx-0.1.9/tlbx/dict_utils.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx/email_utils.py` & `tlbx-0.1.9/tlbx/email_utils.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx/iterable_utils.py` & `tlbx-0.1.9/tlbx/iterable_utils.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx/logging_utils.py` & `tlbx-0.1.9/tlbx/logging_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,16 @@
 
     def __repr__(self):
         if self.repr_attrs:
             return "<%s %s>" % (
                 type(self).__name__,
                 " ".join(
                     [
-                        "%s=%s" % (field, getattr(self, field))
+                        "%s=%s" % (field, repr(getattr(self, field)))
                         for field in self.repr_attrs
                     ]
                 ),
             )
         return "<%s %s>" % (type(self).__name__, id(self))
 
     def __str__(self):
-        return str(vars(self))
+        return str(pf(vars(self)))
```

### Comparing `tlbx-0.1.8/tlbx/object_utils.py` & `tlbx-0.1.9/tlbx/object_utils.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx/string_utils.py` & `tlbx-0.1.9/tlbx/string_utils.py`

 * *Files identical despite different names*

### Comparing `tlbx-0.1.8/tlbx.egg-info/PKG-INFO` & `tlbx-0.1.9/tlbx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlbx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Just some common utilities.
 Home-page: https://github.com/totalhack/tlbx
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: MIT
 Description: tlbx: just some common utilities
```

