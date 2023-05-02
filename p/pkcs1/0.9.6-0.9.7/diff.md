# Comparing `tmp/pkcs1-0.9.6.tar.gz` & `tmp/pkcs1-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pkcs1-0.9.6.tar", last modified: Fri Nov 11 16:31:18 2016, max compression
+gzip compressed data, was "pkcs1-0.9.7.tar", last modified: Tue May  2 07:25:54 2023, max compression
```

## Comparing `pkcs1-0.9.6.tar` & `pkcs1-0.9.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-11-11 16:31:18.000000 pkcs1-0.9.6/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1201 2016-11-11 16:24:13.000000 pkcs1-0.9.6/README.rst
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-11-11 16:31:18.000000 pkcs1-0.9.6/ref/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    34834 2016-11-11 15:47:23.000000 pkcs1-0.9.6/ref/rfc3447.txt.gz
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    26671 2016-11-11 15:47:23.000000 pkcs1-0.9.6/ref/rfc5958.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       91 2016-11-11 15:47:23.000000 pkcs1-0.9.6/MANIFEST.in
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      291 2016-11-11 16:31:18.000000 pkcs1-0.9.6/PKG-INFO
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-11-11 16:31:18.000000 pkcs1-0.9.6/tests/
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-11-11 16:31:18.000000 pkcs1-0.9.6/tests/data/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)   340408 2016-11-11 15:47:23.000000 pkcs1-0.9.6/tests/data/pkcs1v15crypt-vectors.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    74341 2016-11-11 15:47:23.000000 pkcs1-0.9.6/tests/data/oaep-vect.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      678 2016-11-11 15:47:23.000000 pkcs1-0.9.6/tests/data/readme.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     5702 2016-11-11 15:47:23.000000 pkcs1-0.9.6/tests/data/pss-int.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)   325453 2016-11-11 15:47:23.000000 pkcs1-0.9.6/tests/data/pkcs1v15sign-vectors.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    92291 2016-11-11 15:47:23.000000 pkcs1-0.9.6/tests/data/pss-vect.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    11400 2016-11-11 15:47:23.000000 pkcs1-0.9.6/tests/data/oaep-int.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      993 2016-11-11 16:20:14.000000 pkcs1-0.9.6/tests/test_rsaes_pkcs1_v15.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      536 2016-11-11 16:20:14.000000 pkcs1-0.9.6/tests/test_naive_encryption.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1595 2016-11-11 16:20:14.000000 pkcs1-0.9.6/tests/test_rsassa_pss.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      420 2016-11-11 16:20:14.000000 pkcs1-0.9.6/tests/test_emsa_pss.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      815 2016-11-11 16:20:14.000000 pkcs1-0.9.6/tests/test_rsassa_pkcs1_v15.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1349 2016-11-11 16:04:12.000000 pkcs1-0.9.6/tests/rsaes_oaep.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1061 2016-11-11 16:20:14.000000 pkcs1-0.9.6/tests/test_rsaes_oaep.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     8854 2016-11-11 16:04:12.000000 pkcs1-0.9.6/tests/data.py
--rwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)      421 2016-11-11 16:20:14.000000 pkcs1-0.9.6/setup.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       59 2016-11-11 16:31:18.000000 pkcs1-0.9.6/setup.cfg
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-11-11 16:31:18.000000 pkcs1-0.9.6/pkcs1.egg-info/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      847 2016-11-11 16:31:18.000000 pkcs1-0.9.6/pkcs1.egg-info/SOURCES.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      291 2016-11-11 16:31:18.000000 pkcs1-0.9.6/pkcs1.egg-info/PKG-INFO
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        6 2016-11-11 16:31:18.000000 pkcs1-0.9.6/pkcs1.egg-info/top_level.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        1 2016-11-11 16:31:18.000000 pkcs1-0.9.6/pkcs1.egg-info/dependency_links.txt
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-11-11 16:31:18.000000 pkcs1-0.9.6/pkcs1/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     4683 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/primes.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     3323 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/primitives.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1042 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/rsaes_pkcs1_v15.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1574 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/eme_pkcs1_v15.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      180 2016-11-11 16:05:17.000000 pkcs1-0.9.6/pkcs1/__init__.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      679 2016-11-11 15:47:23.000000 pkcs1-0.9.6/pkcs1/exceptions.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     5546 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/keys.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2120 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/rsassa_pss.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1008 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/emsa_pkcs1_v15.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1587 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/rsassa_pkcs1_v15.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      101 2016-11-11 15:47:23.000000 pkcs1-0.9.6/pkcs1/defaults.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     4115 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/emsa_pss.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     3464 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/rsaes_oaep.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      763 2016-11-11 16:04:12.000000 pkcs1-0.9.6/pkcs1/mgf.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2023-05-02 07:25:54.210227 pkcs1-0.9.7/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       91 2023-05-02 07:21:19.000000 pkcs1-0.9.7/MANIFEST.in
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1454 2023-05-02 07:25:54.210227 pkcs1-0.9.7/PKG-INFO
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1201 2023-05-02 07:21:19.000000 pkcs1-0.9.7/README.rst
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2023-05-02 07:25:54.206227 pkcs1-0.9.7/pkcs1/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      180 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/__init__.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      101 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/defaults.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1574 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/eme_pkcs1_v15.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1008 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/emsa_pkcs1_v15.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     4115 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/emsa_pss.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      679 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/exceptions.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     5532 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/keys.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      763 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/mgf.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     4674 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/primes.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     3322 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/primitives.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     3464 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/rsaes_oaep.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1042 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/rsaes_pkcs1_v15.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1587 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/rsassa_pkcs1_v15.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2120 2023-05-02 07:21:19.000000 pkcs1-0.9.7/pkcs1/rsassa_pss.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2023-05-02 07:25:54.206227 pkcs1-0.9.7/pkcs1.egg-info/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1454 2023-05-02 07:25:53.000000 pkcs1-0.9.7/pkcs1.egg-info/PKG-INFO
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      847 2023-05-02 07:25:54.000000 pkcs1-0.9.7/pkcs1.egg-info/SOURCES.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        1 2023-05-02 07:25:53.000000 pkcs1-0.9.7/pkcs1.egg-info/dependency_links.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        6 2023-05-02 07:25:53.000000 pkcs1-0.9.7/pkcs1.egg-info/top_level.txt
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2023-05-02 07:25:54.206227 pkcs1-0.9.7/ref/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    34834 2023-05-02 07:21:19.000000 pkcs1-0.9.7/ref/rfc3447.txt.gz
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    26671 2023-05-02 07:21:19.000000 pkcs1-0.9.7/ref/rfc5958.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       38 2023-05-02 07:25:54.210227 pkcs1-0.9.7/setup.cfg
+-rwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)      570 2023-05-02 07:25:17.000000 pkcs1-0.9.7/setup.py
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2023-05-02 07:25:54.206227 pkcs1-0.9.7/tests/
+drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2023-05-02 07:25:54.210227 pkcs1-0.9.7/tests/data/
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    11400 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data/oaep-int.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    74341 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data/oaep-vect.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)   340408 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data/pkcs1v15crypt-vectors.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)   325453 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data/pkcs1v15sign-vectors.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     5702 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data/pss-int.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    92291 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data/pss-vect.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      678 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data/readme.txt
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     8854 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/data.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1349 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/rsaes_oaep.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      420 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/test_emsa_pss.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      536 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/test_naive_encryption.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1061 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/test_rsaes_oaep.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      993 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/test_rsaes_pkcs1_v15.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      815 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/test_rsassa_pkcs1_v15.py
+-rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1595 2023-05-02 07:21:19.000000 pkcs1-0.9.7/tests/test_rsassa_pss.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pkcs1-0.9.6/README.rst` & `pkcs1-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/ref/rfc3447.txt.gz` & `pkcs1-0.9.7/ref/rfc3447.txt.gz`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/ref/rfc5958.txt` & `pkcs1-0.9.7/ref/rfc5958.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data/pkcs1v15crypt-vectors.txt` & `pkcs1-0.9.7/tests/data/pkcs1v15crypt-vectors.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data/oaep-vect.txt` & `pkcs1-0.9.7/tests/data/oaep-vect.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data/readme.txt` & `pkcs1-0.9.7/tests/data/readme.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data/pss-int.txt` & `pkcs1-0.9.7/tests/data/pss-int.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data/pkcs1v15sign-vectors.txt` & `pkcs1-0.9.7/tests/data/pkcs1v15sign-vectors.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data/pss-vect.txt` & `pkcs1-0.9.7/tests/data/pss-vect.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data/oaep-int.txt` & `pkcs1-0.9.7/tests/data/oaep-int.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/test_rsaes_pkcs1_v15.py` & `pkcs1-0.9.7/tests/test_rsaes_pkcs1_v15.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/test_naive_encryption.py` & `pkcs1-0.9.7/tests/test_naive_encryption.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/test_rsassa_pss.py` & `pkcs1-0.9.7/tests/test_rsassa_pss.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/test_rsassa_pkcs1_v15.py` & `pkcs1-0.9.7/tests/test_rsassa_pkcs1_v15.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/rsaes_oaep.py` & `pkcs1-0.9.7/tests/rsaes_oaep.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/test_rsaes_oaep.py` & `pkcs1-0.9.7/tests/test_rsaes_oaep.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/tests/data.py` & `pkcs1-0.9.7/tests/data.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1.egg-info/SOURCES.txt` & `pkcs1-0.9.7/pkcs1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/primes.py` & `pkcs1-0.9.7/pkcs1/primes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import fractions
+import math
 from . import primitives
 
 from .defaults import default_pseudo_random, default_crypto_random
 
 PRIME_ALGO = 'miller-rabin'
 gmpy = None
 try:
@@ -134,15 +134,15 @@
        rnd - a random generator
    '''
     s = 0
     d = n-1
     # Find nearest power of 2
     s = primitives.integer_bit_size(n)
     # Find greatest factor which is a power of 2
-    s = fractions.gcd(2**s, n-1)
+    s = math.gcd(2**s, n-1)
     d = (n-1) // s
     s = primitives.integer_bit_size(s) - 1
     while k:
         k = k - 1
         a = rnd.randint(2, n-2)
         x = pow(a,d,n)
         if x == 1 or x == n - 1:
@@ -157,8 +157,8 @@
             return False
     return True
 
 try:
     xrange
 except NameError:
     # Python 3
-    xrange = range
+    xrange = range
```

### Comparing `pkcs1-0.9.6/pkcs1/primitives.py` & `pkcs1-0.9.7/pkcs1/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 '''Primitive functions extracted from the PKCS1 RFC'''
 
 def _pow(a, b, mod):
     '''Exponentiation function using acceleration from gmpy if possible'''
     if gmpy:
-        return long(pow(gmpy.mpz(a), gmpy.mpz(b), gmpy.mpz(mod)))
+        return int(pow(gmpy.mpz(a), gmpy.mpz(b), gmpy.mpz(mod)))
     else:
         return pow(a, b, mod)
 
 def integer_ceil(a, b):
     '''Return the ceil integer of a div b.'''
     quanta, mod = divmod(a, b)
     if mod:
```

### Comparing `pkcs1-0.9.6/pkcs1/rsaes_pkcs1_v15.py` & `pkcs1-0.9.7/pkcs1/rsaes_pkcs1_v15.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/eme_pkcs1_v15.py` & `pkcs1-0.9.7/pkcs1/eme_pkcs1_v15.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/exceptions.py` & `pkcs1-0.9.7/pkcs1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/keys.py` & `pkcs1-0.9.7/pkcs1/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import fractions
+import math
 from . import primitives
 from . import exceptions
 
 from .defaults import default_crypto_random
 from .primes import get_prime, DEFAULT_ITERATION
 
 class RsaPublicKey(object):
@@ -142,24 +142,24 @@
     n = 1
     while len(primes) < number:
         if number - len(primes) == 1:
             bits = size - primitives.integer_bit_size(n) + 1
         prime = get_prime(bits, rnd, k, algorithm=primality_algorithm)
         if prime in primes:
             continue
-        if e is not None and fractions.gcd(e, lbda) != 1:
+        if e is not None and math.gcd(e, lbda) != 1:
             continue
         if strict_size and number - len(primes) == 1 and primitives.integer_bit_size(n*prime) != size:
             continue
         primes.append(prime)
         n *= prime
         lbda *= prime - 1
     if e is None:
         e = 0x10001
         while e < lbda:
-            if fractions.gcd(e, lbda) == 1:
+            if math.gcd(e, lbda) == 1:
                 break
             e += 2
     assert 3 <= e <= n-1
     public = RsaPublicKey(n, e)
     private = MultiPrimeRsaPrivateKey(primes, e, blind=True, rnd=rnd)
-    return public, private
+    return public, private
```

### Comparing `pkcs1-0.9.6/pkcs1/rsassa_pss.py` & `pkcs1-0.9.7/pkcs1/rsassa_pss.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/emsa_pkcs1_v15.py` & `pkcs1-0.9.7/pkcs1/emsa_pkcs1_v15.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/rsassa_pkcs1_v15.py` & `pkcs1-0.9.7/pkcs1/rsassa_pkcs1_v15.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/emsa_pss.py` & `pkcs1-0.9.7/pkcs1/emsa_pss.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/rsaes_oaep.py` & `pkcs1-0.9.7/pkcs1/rsaes_oaep.py`

 * *Files identical despite different names*

### Comparing `pkcs1-0.9.6/pkcs1/mgf.py` & `pkcs1-0.9.7/pkcs1/mgf.py`

 * *Files identical despite different names*

