# Comparing `tmp/dxsp-1.6.0.tar.gz` & `tmp/dxsp-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.6.0.tar", max compression
+gzip compressed data, was "dxsp-1.6.1.tar", max compression
```

## Comparing `dxsp-1.6.0.tar` & `dxsp-1.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-02 06:34:10.479825 dxsp-1.6.0/LICENSE
--rw-r--r--   0        0        0     3225 2023-05-02 06:34:10.479825 dxsp-1.6.0/README.md
--rw-r--r--   0        0        0       38 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-02 06:34:11.219831 dxsp-1.6.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    29576 2023-05-02 06:34:10.479825 dxsp-1.6.0/dxsp/main.py
--rw-r--r--   0        0        0     1045 2023-05-02 06:34:11.215831 dxsp-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-02 07:11:52.658259 dxsp-1.6.1/LICENSE
+-rw-r--r--   0        0        0     3225 2023-05-02 07:11:52.658259 dxsp-1.6.1/README.md
+-rw-r--r--   0        0        0       38 2023-05-02 07:11:52.658259 dxsp-1.6.1/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-02 07:11:53.546260 dxsp-1.6.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-02 07:11:52.658259 dxsp-1.6.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-02 07:11:52.658259 dxsp-1.6.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-02 07:11:52.658259 dxsp-1.6.1/dxsp/config.py
+-rw-r--r--   0        0        0      564 2023-05-02 07:11:52.658259 dxsp-1.6.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    29576 2023-05-02 07:11:52.658259 dxsp-1.6.1/dxsp/main.py
+-rw-r--r--   0        0        0     1045 2023-05-02 07:11:53.546260 dxsp-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.6.1/PKG-INFO
```

### Comparing `dxsp-1.6.0/LICENSE` & `dxsp-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.0/README.md` & `dxsp-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.0/dxsp/assets/blockchains.py` & `dxsp-1.6.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.0/dxsp/default_settings.toml` & `dxsp-1.6.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.0/dxsp/main.py` & `dxsp-1.6.1/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.6.0/pyproject.toml` & `dxsp-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.6.0"
+version = "1.6.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.6.0/PKG-INFO` & `dxsp-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.6.0
+Version: 1.6.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

