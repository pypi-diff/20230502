# Comparing `tmp/betterconfigs-0.8.2.tar.gz` & `tmp/betterconfigs-0.8.3.tar.gz`

## Comparing `betterconfigs-0.8.2.tar` & `betterconfigs-0.8.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/buildscript.sh
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/test_conf.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/src/betterconfigs/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/src/betterconfigs/utilities.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/LICENSE
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/README.md
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 betterconfigs-0.8.2/PKG-INFO
+-rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/buildscript.sh
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/test_conf.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/src/betterconfigs/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/src/betterconfigs/utilities.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 betterconfigs-0.8.3/PKG-INFO
```

### Comparing `betterconfigs-0.8.2/test_conf.py` & `betterconfigs-0.8.3/test_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     h = config('test.config')
     assert(h['_encrypted']==False)
     assert(h.encKey!=None)
     h['hello']='world'
     assert(h.encryptFile()==0)
     assert(h['hello']=='world')
     assert(h.getRaw('hello')!='world')
-    assert(h.getRaw('_version')=='0.8.2')
+    assert(h.getRaw('_version')=='0.8.3')
     encryptionKey = h.encKey
     t = config('test.config')
     assert(t.getRaw('_encrypted')==True)
     with pytest.raises(Exception):
         t['hello']='world'
     os.remove('test.config')
 def test_decryption():
```

### Comparing `betterconfigs-0.8.2/.github/workflows/python-publish.yml` & `betterconfigs-0.8.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8.2/src/betterconfigs/__init__.py` & `betterconfigs-0.8.3/src/betterconfigs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import os
 import warnings
 from cryptography.fernet import Fernet
-executableVersion = "0.8.2"
+executableVersion = "0.8.3"
 supportedTypes=[int, str, list, bool]
 class config:
     def __init__(self, path) -> None:
         self.path = path
         self.encKey = None
         if os.path.exists(path)==False:
             try:
```

### Comparing `betterconfigs-0.8.2/LICENSE` & `betterconfigs-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8.2/README.md` & `betterconfigs-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8.2/pyproject.toml` & `betterconfigs-0.8.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "betterconfigs"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="Iain Rosen", email="hello@iainrosen.me" },
 ]
 description = "A small package to simplify configuration storing and retrieving"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "warnings",
   "cryptography",
 ]
 [project.urls]
 "Homepage" = "https://github.com/iainrosen/betterconfigs"
 "Bug Tracker" = "https://github.com/iainrosen/betterconfigs/issues"
```

### Comparing `betterconfigs-0.8.2/PKG-INFO` & `betterconfigs-0.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: betterconfigs
-Version: 0.8.2
+Version: 0.8.3
 Summary: A small package to simplify configuration storing and retrieving
 Project-URL: Homepage, https://github.com/iainrosen/betterconfigs
 Project-URL: Bug Tracker, https://github.com/iainrosen/betterconfigs/issues
 Author-email: Iain Rosen <hello@iainrosen.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: cryptography
-Requires-Dist: warnings
 Description-Content-Type: text/markdown
 
 # BetterConfigs
 
 A small package to simplify configuration storing and retrieving
 
 ## Usage
```

