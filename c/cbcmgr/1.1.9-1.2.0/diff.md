# Comparing `tmp/cbcmgr-1.1.9.tar.gz` & `tmp/cbcmgr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.1.9.tar", last modified: Tue Apr 18 19:33:05 2023, max compression
+gzip compressed data, was "cbcmgr-1.2.0.tar", last modified: Tue May  2 21:52:44 2023, max compression
```

## Comparing `cbcmgr-1.1.9.tar` & `cbcmgr-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-18 19:33:05.734414 cbcmgr-1.1.9/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.1.9/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-04-18 19:33:05.734233 cbcmgr-1.1.9/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.1.9/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-18 19:33:05.672721 cbcmgr-1.1.9/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.1.9/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.1.9/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.1.9/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.1.9/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     4051 2023-02-14 15:09:46.000000 cbcmgr-1.1.9/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    10675 2023-02-22 16:29:09.000000 cbcmgr-1.1.9/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.1.9/cbcmgr/retry.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-18 19:33:05.733841 cbcmgr-1.1.9/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      326 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-04-18 19:33:05.000000 cbcmgr-1.1.9/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-18 19:33:05.734485 cbcmgr-1.1.9/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      705 2023-04-18 19:15:38.000000 cbcmgr-1.1.9/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-02 21:52:44.433478 cbcmgr-1.2.0/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.0/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-02 21:52:44.433359 cbcmgr-1.2.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-02 21:52:44.427026 cbcmgr-1.2.0/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.0/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.0/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.0/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.0/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     4098 2023-05-02 21:24:28.000000 cbcmgr-1.2.0/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    10675 2023-02-22 16:29:09.000000 cbcmgr-1.2.0/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.0/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.0/cbcmgr/schema.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-02 21:52:44.433157 cbcmgr-1.2.0/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      343 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       57 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-02 21:52:44.433519 cbcmgr-1.2.0/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      705 2023-05-02 21:27:42.000000 cbcmgr-1.2.0/setup.py
```

### Comparing `cbcmgr-1.1.9/LICENSE.txt` & `cbcmgr-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.9/PKG-INFO` & `cbcmgr-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.1.9
+Version: 1.2.0
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.1.9/README.md` & `cbcmgr-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.9/cbcmgr/cb_connect.py` & `cbcmgr-1.2.0/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.9/cbcmgr/cb_management.py` & `cbcmgr-1.2.0/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.9/cbcmgr/cb_session.py` & `cbcmgr-1.2.0/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.9/cbcmgr/exceptions.py` & `cbcmgr-1.2.0/cbcmgr/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,7 +296,11 @@
 
 class ScopeNotConnected(CBException):
     pass
 
 
 class CollectionNotConnected(CBException):
     pass
+
+
+class SchemaFileError(CBException):
+    pass
```

### Comparing `cbcmgr-1.1.9/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.2.0/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.9/cbcmgr/retry.py` & `cbcmgr-1.2.0/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.1.9/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.2.0/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.1.9
+Version: 1.2.0
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.1.9/setup.py` & `cbcmgr-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.1.9',
+    version='1.2.0',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

