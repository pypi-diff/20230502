# Comparing `tmp/kojo-0.14.0.tar.gz` & `tmp/kojo-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojo-0.14.0.tar", last modified: Fri Apr 28 09:50:17 2023, max compression
+gzip compressed data, was "kojo-0.15.0.tar", last modified: Tue May  2 12:03:57 2023, max compression
```

## Comparing `kojo-0.14.0.tar` & `kojo-0.15.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-04-28 09:50:17.305655 kojo-0.14.0/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      612 2023-04-28 09:50:17.305655 kojo-0.14.0/PKG-INFO
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-04-28 09:50:17.305655 kojo-0.14.0/kojo/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.007066 kojo-0.14.0/kojo/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      454 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/duplicatefinder.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     2197 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/io.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     3451 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/item.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      947 2023-04-28 09:46:09.112495 kojo-0.14.0/kojo/jsonschemavalidator.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      962 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/process.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1844 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/propertiesconverter.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       39 2023-04-27 08:31:58.877706 kojo-0.14.0/setup.cfg
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      743 2023-04-28 09:48:06.255154 kojo-0.14.0/setup.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-05-02 12:03:57.938827 kojo-0.15.0/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      612 2023-05-02 12:03:57.938827 kojo-0.15.0/PKG-INFO
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-05-02 12:03:57.938827 kojo-0.15.0/kojo/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.007066 kojo-0.15.0/kojo/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      454 2023-04-27 08:31:58.877706 kojo-0.15.0/kojo/duplicatefinder.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     2197 2023-04-27 08:31:58.877706 kojo-0.15.0/kojo/io.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     3455 2023-05-02 12:01:05.544818 kojo-0.15.0/kojo/item.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      947 2023-04-28 09:56:03.337703 kojo-0.15.0/kojo/jsonschemavalidator.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      962 2023-04-27 08:31:58.877706 kojo-0.15.0/kojo/process.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1844 2023-04-27 08:31:58.877706 kojo-0.15.0/kojo/propertiesconverter.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       39 2023-04-27 08:31:58.877706 kojo-0.15.0/setup.cfg
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      743 2023-05-02 12:01:29.684543 kojo-0.15.0/setup.py
```

### Comparing `kojo-0.14.0/PKG-INFO` & `kojo-0.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: kojo
-Version: 0.14.0
+Version: 0.15.0
 Summary: A library to transform data through a pipeline
 Home-page: https://gitlab.com/filchos/kojo
 Author: Olaf Schneider
 Author-email: mail@olafschneider.com
 License: GNU GPLv3
-Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.14.0/kojo-0.14.0.tar.gz
+Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.15.0/kojo-0.15.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kojo-0.14.0/kojo/io.py` & `kojo-0.15.0/kojo/io.py`

 * *Files identical despite different names*

### Comparing `kojo-0.14.0/kojo/item.py` & `kojo-0.15.0/kojo/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.log = ItemLog()
         self.meta = {}
 
     def clone(self):
-        item = copy.copy(self)
+        item = copy.deepcopy(self)
         item.log = self.log.clone()
         item.meta = copy.copy(self.meta)
         return item
 
     def flatten(self):
         item = Item(flatten(self))
         item.log = self.log.clone()
```

### Comparing `kojo-0.14.0/kojo/jsonschemavalidator.py` & `kojo-0.15.0/kojo/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `kojo-0.14.0/kojo/process.py` & `kojo-0.15.0/kojo/process.py`

 * *Files identical despite different names*

### Comparing `kojo-0.14.0/kojo/propertiesconverter.py` & `kojo-0.15.0/kojo/propertiesconverter.py`

 * *Files identical despite different names*

### Comparing `kojo-0.14.0/setup.py` & `kojo-0.15.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name="kojo",
     packages=["kojo"],
-    version="0.14.0",
+    version="0.15.0",
     license="GNU GPLv3",
     description="A library to transform data through a pipeline",
     author="Olaf Schneider",
     author_email="mail@olafschneider.com",
     url="https://gitlab.com/filchos/kojo",
-    download_url="https://gitlab.com/filchos/kojo/-/archive/0.14.0/kojo-0.14.0.tar.gz",
+    download_url="https://gitlab.com/filchos/kojo/-/archive/0.15.0/kojo-0.15.0.tar.gz",
     install_requires=["jsonschema"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
```

