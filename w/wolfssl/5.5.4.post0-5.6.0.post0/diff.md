# Comparing `tmp/wolfssl-5.5.4.post0.tar.gz` & `tmp/wolfssl-5.6.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolfssl-5.5.4.post0.tar", last modified: Fri Dec 30 17:44:52 2022, max compression
+gzip compressed data, was "wolfssl-5.6.0.post0.tar", last modified: Tue May  2 16:03:47 2023, max compression
```

## Comparing `wolfssl-5.5.4.post0.tar` & `wolfssl-5.6.0.post0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/
--rw-r--r--   0 dan       (1000) dan       (1000)      938 2022-12-30 17:29:41.000000 wolfssl-5.5.4.post0/ChangeLog.rst
--rw-r--r--   0 dan       (1000) dan       (1000)      918 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/LICENSING.rst
--rw-r--r--   0 dan       (1000) dan       (1000)      261 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/MANIFEST.in
--rw-r--r--   0 dan       (1000) dan       (1000)     3611 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     2767 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/README.rst
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:44:52.367308 wolfssl-5.5.4.post0/certs/
--rw-r--r--   0 dan       (1000) dan       (1000)     5314 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/certs/ca-cert.pem
--rw-r--r--   0 dan       (1000) dan       (1000)     1229 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/certs/ca-globalsign-r3.pem
--rw-r--r--   0 dan       (1000) dan       (1000)     5384 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/certs/client-cert.pem
--rw-r--r--   0 dan       (1000) dan       (1000)     1679 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/certs/client-key.pem
--rw-r--r--   0 dan       (1000) dan       (1000)     2229 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/certs/crl.pem
--rw-r--r--   0 dan       (1000) dan       (1000)    10574 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/certs/server-cert.pem
--rw-r--r--   0 dan       (1000) dan       (1000)     1679 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/certs/server-key.pem
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/docs/
--rw-r--r--   0 dan       (1000) dan       (1000)     8864 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/Makefile
--rw-r--r--   0 dan       (1000) dan       (1000)      258 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/api.rst
--rw-r--r--   0 dan       (1000) dan       (1000)     9649 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/conf.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3162 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/examples.rst
--rw-r--r--   0 dan       (1000) dan       (1000)       93 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/index.rst
--rw-r--r--   0 dan       (1000) dan       (1000)       27 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/installation.rst
--rw-r--r--   0 dan       (1000) dan       (1000)       30 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/licensing.rst
--rw-r--r--   0 dan       (1000) dan       (1000)     3779 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/docs/usage.rst
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/requirements/
--rw-r--r--   0 dan       (1000) dan       (1000)       36 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/requirements/docs.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        5 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/requirements/prod.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       12 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/requirements/setup.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       23 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/requirements/test.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/setup.cfg
--rwxr-xr-x   0 dan       (1000) dan       (1000)     2961 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/setup.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/tests/
--rw-r--r--   0 dan       (1000) dan       (1000)     2003 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/tests/conftest.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2398 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/tests/test_client.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2226 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/tests/test_context.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2325 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/tests/test_methods.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/wolfssl/
--rw-r--r--   0 dan       (1000) dan       (1000)     1373 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/wolfssl/__about__.py
--rw-r--r--   0 dan       (1000) dan       (1000)    36240 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/wolfssl/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)    19426 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/wolfssl/_build_ffi.py
--rw-r--r--   0 dan       (1000) dan       (1000)     4290 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/wolfssl/_methods.py
--rw-r--r--   0 dan       (1000) dan       (1000)    12798 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/wolfssl/_openssl.py
--rw-r--r--   0 dan       (1000) dan       (1000)      365 2022-12-30 17:29:41.000000 wolfssl-5.5.4.post0/wolfssl/_version.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3221 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/wolfssl/exceptions.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1283 2022-12-30 16:21:50.000000 wolfssl-5.5.4.post0/wolfssl/utils.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:44:52.371308 wolfssl-5.5.4.post0/wolfssl.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     3611 2022-12-30 17:44:52.000000 wolfssl-5.5.4.post0/wolfssl.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      851 2022-12-30 17:44:52.000000 wolfssl-5.5.4.post0/wolfssl.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2022-12-30 17:44:52.000000 wolfssl-5.5.4.post0/wolfssl.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2022-12-30 16:26:18.000000 wolfssl-5.5.4.post0/wolfssl.egg-info/not-zip-safe
--rw-r--r--   0 dan       (1000) dan       (1000)        5 2022-12-30 17:44:52.000000 wolfssl-5.5.4.post0/wolfssl.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        8 2022-12-30 17:44:52.000000 wolfssl-5.5.4.post0/wolfssl.egg-info/top_level.txt
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 16:03:47.945860 wolfssl-5.6.0.post0/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1057 2023-05-02 16:00:31.000000 wolfssl-5.6.0.post0/ChangeLog.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)      918 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/LICENSING.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)      261 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/MANIFEST.in
+-rw-r--r--   0 dan       (1000) dan       (1000)     3611 2023-05-02 16:03:47.945860 wolfssl-5.6.0.post0/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     2767 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/README.rst
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 16:03:47.941860 wolfssl-5.6.0.post0/certs/
+-rw-r--r--   0 dan       (1000) dan       (1000)     5314 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/certs/ca-cert.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)     1229 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/certs/ca-globalsign-r3.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)     5384 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/certs/client-cert.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)     1679 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/certs/client-key.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)     2229 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/certs/crl.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)    10574 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/certs/server-cert.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)     1679 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/certs/server-key.pem
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 16:03:47.941860 wolfssl-5.6.0.post0/docs/
+-rw-r--r--   0 dan       (1000) dan       (1000)     8864 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/Makefile
+-rw-r--r--   0 dan       (1000) dan       (1000)      258 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/api.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)     9649 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/conf.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3162 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/examples.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)       93 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/index.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)       27 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/installation.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)       30 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/licensing.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)     3779 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/docs/usage.rst
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 16:03:47.941860 wolfssl-5.6.0.post0/requirements/
+-rw-r--r--   0 dan       (1000) dan       (1000)       36 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/requirements/docs.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        5 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/requirements/prod.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       12 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/requirements/setup.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       23 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/requirements/test.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-05-02 16:03:47.945860 wolfssl-5.6.0.post0/setup.cfg
+-rwxr-xr-x   0 dan       (1000) dan       (1000)     2961 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 16:03:47.941860 wolfssl-5.6.0.post0/tests/
+-rw-r--r--   0 dan       (1000) dan       (1000)     2003 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/tests/conftest.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2398 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/tests/test_client.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2226 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/tests/test_context.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2325 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/tests/test_methods.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 16:03:47.945860 wolfssl-5.6.0.post0/wolfssl/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1373 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/wolfssl/__about__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    36240 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/wolfssl/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    19426 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/wolfssl/_build_ffi.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     4290 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/wolfssl/_methods.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    12798 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/wolfssl/_openssl.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      365 2023-05-02 16:00:31.000000 wolfssl-5.6.0.post0/wolfssl/_version.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3221 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/wolfssl/exceptions.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1283 2022-12-30 16:21:50.000000 wolfssl-5.6.0.post0/wolfssl/utils.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 16:03:47.945860 wolfssl-5.6.0.post0/wolfssl.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     3611 2023-05-02 16:03:47.000000 wolfssl-5.6.0.post0/wolfssl.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      851 2023-05-02 16:03:47.000000 wolfssl-5.6.0.post0/wolfssl.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-05-02 16:03:47.000000 wolfssl-5.6.0.post0/wolfssl.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2022-12-30 16:26:18.000000 wolfssl-5.6.0.post0/wolfssl.egg-info/not-zip-safe
+-rw-r--r--   0 dan       (1000) dan       (1000)        5 2023-05-02 16:03:47.000000 wolfssl-5.6.0.post0/wolfssl.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        8 2023-05-02 16:03:47.000000 wolfssl-5.6.0.post0/wolfssl.egg-info/top_level.txt
```

### Comparing `wolfssl-5.5.4.post0/LICENSING.rst` & `wolfssl-5.6.0.post0/LICENSING.rst`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/PKG-INFO` & `wolfssl-5.6.0.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfssl
-Version: 5.5.4.post0
+Version: 5.6.0.post0
 Summary: Python module that encapsulates wolfSSL's C SSL/TLS library.
 Home-page: https://github.com/wolfssl/wolfssl-py
 Author: wolfSSL Inc.
 Author-email: info@wolfssl.com
 License: GPLv2 or Commercial License
 Keywords: wolfssl,wolfcrypt,security,cryptography
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `wolfssl-5.5.4.post0/README.rst` & `wolfssl-5.6.0.post0/README.rst`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/certs/ca-cert.pem` & `wolfssl-5.6.0.post0/certs/ca-cert.pem`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/certs/ca-globalsign-r3.pem` & `wolfssl-5.6.0.post0/certs/ca-globalsign-r3.pem`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/certs/client-cert.pem` & `wolfssl-5.6.0.post0/certs/client-cert.pem`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/certs/client-key.pem` & `wolfssl-5.6.0.post0/certs/client-key.pem`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/certs/crl.pem` & `wolfssl-5.6.0.post0/certs/crl.pem`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/certs/server-cert.pem` & `wolfssl-5.6.0.post0/certs/server-cert.pem`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/certs/server-key.pem` & `wolfssl-5.6.0.post0/certs/server-key.pem`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/docs/Makefile` & `wolfssl-5.6.0.post0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/docs/conf.py` & `wolfssl-5.6.0.post0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/docs/examples.rst` & `wolfssl-5.6.0.post0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/docs/usage.rst` & `wolfssl-5.6.0.post0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/setup.py` & `wolfssl-5.6.0.post0/setup.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/tests/conftest.py` & `wolfssl-5.6.0.post0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/tests/test_client.py` & `wolfssl-5.6.0.post0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/tests/test_context.py` & `wolfssl-5.6.0.post0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/tests/test_methods.py` & `wolfssl-5.6.0.post0/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl/__about__.py` & `wolfssl-5.6.0.post0/wolfssl/__about__.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl/__init__.py` & `wolfssl-5.6.0.post0/wolfssl/__init__.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl/_build_ffi.py` & `wolfssl-5.6.0.post0/wolfssl/_build_ffi.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl/_methods.py` & `wolfssl-5.6.0.post0/wolfssl/_methods.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl/_openssl.py` & `wolfssl-5.6.0.post0/wolfssl/_openssl.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl/exceptions.py` & `wolfssl-5.6.0.post0/wolfssl/exceptions.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl/utils.py` & `wolfssl-5.6.0.post0/wolfssl/utils.py`

 * *Files identical despite different names*

### Comparing `wolfssl-5.5.4.post0/wolfssl.egg-info/PKG-INFO` & `wolfssl-5.6.0.post0/wolfssl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfssl
-Version: 5.5.4.post0
+Version: 5.6.0.post0
 Summary: Python module that encapsulates wolfSSL's C SSL/TLS library.
 Home-page: https://github.com/wolfssl/wolfssl-py
 Author: wolfSSL Inc.
 Author-email: info@wolfssl.com
 License: GPLv2 or Commercial License
 Keywords: wolfssl,wolfcrypt,security,cryptography
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `wolfssl-5.5.4.post0/wolfssl.egg-info/SOURCES.txt` & `wolfssl-5.6.0.post0/wolfssl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

