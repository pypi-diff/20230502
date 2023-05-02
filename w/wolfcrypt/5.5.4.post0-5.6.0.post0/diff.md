# Comparing `tmp/wolfcrypt-5.5.4.post0.tar.gz` & `tmp/wolfcrypt-5.6.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolfcrypt-5.5.4.post0.tar", last modified: Fri Dec 30 17:43:44 2022, max compression
+gzip compressed data, was "wolfcrypt-5.6.0.post0.tar", last modified: Tue May  2 15:47:46 2023, max compression
```

## Comparing `wolfcrypt-5.5.4.post0.tar` & `wolfcrypt-5.6.0.post0.tar`

### file list

```diff
@@ -1,66 +1,72 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.159306 wolfcrypt-5.5.4.post0/
--rw-r--r--   0 dan       (1000) dan       (1000)     1591 2022-12-30 17:28:37.000000 wolfcrypt-5.5.4.post0/ChangeLog.rst
--rw-r--r--   0 dan       (1000) dan       (1000)      918 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/LICENSING.rst
--rw-r--r--   0 dan       (1000) dan       (1000)      284 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/MANIFEST.in
--rw-r--r--   0 dan       (1000) dan       (1000)     4322 2022-12-30 17:43:44.159306 wolfcrypt-5.5.4.post0/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     3426 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/README.rst
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/docs/
--rw-r--r--   0 dan       (1000) dan       (1000)     8872 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/Makefile
--rw-r--r--   0 dan       (1000) dan       (1000)     4036 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/asymmetric.rst
--rw-r--r--   0 dan       (1000) dan       (1000)     9672 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/conf.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1770 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/digest.rst
--rw-r--r--   0 dan       (1000) dan       (1000)      173 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/index.rst
--rw-r--r--   0 dan       (1000) dan       (1000)     1805 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/mac.rst
--rw-r--r--   0 dan       (1000) dan       (1000)      805 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/random.rst
--rw-r--r--   0 dan       (1000) dan       (1000)      869 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/streaming.rst
--rw-r--r--   0 dan       (1000) dan       (1000)     1367 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/docs/symmetric.rst
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/requirements/
--rw-r--r--   0 dan       (1000) dan       (1000)       36 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/requirements/docs.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        5 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/requirements/prod.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       12 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/requirements/setup.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       23 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/requirements/test.txt
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/scripts/
--rw-r--r--   0 dan       (1000) dan       (1000)    35924 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/scripts/build_ffi.py
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2022-12-30 17:43:44.159306 wolfcrypt-5.5.4.post0/setup.cfg
--rwxr-xr-x   0 dan       (1000) dan       (1000)     3012 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/setup.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/tests/
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/tests/__pycache__/
--rw-r--r--   0 dan       (1000) dan       (1000)     7770 2022-12-30 16:17:34.000000 wolfcrypt-5.5.4.post0/tests/__pycache__/test_aesgcmstream.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 dan       (1000) dan       (1000)     5340 2022-12-30 16:17:34.000000 wolfcrypt-5.5.4.post0/tests/__pycache__/test_asn.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 dan       (1000) dan       (1000)    31951 2022-12-30 16:17:34.000000 wolfcrypt-5.5.4.post0/tests/__pycache__/test_ciphers.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 dan       (1000) dan       (1000)     5753 2022-12-30 16:17:34.000000 wolfcrypt-5.5.4.post0/tests/__pycache__/test_hashes.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 dan       (1000) dan       (1000)     1840 2022-12-30 16:17:34.000000 wolfcrypt-5.5.4.post0/tests/__pycache__/test_pwdbased.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 dan       (1000) dan       (1000)     2259 2022-12-30 16:17:34.000000 wolfcrypt-5.5.4.post0/tests/__pycache__/test_random.cpython-310-pytest-7.2.0.pyc
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/tests/certs/
--rw-r--r--   0 dan       (1000) dan       (1000)     1249 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/certs/server-cert.der
--rw-r--r--   0 dan       (1000) dan       (1000)     1749 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/certs/server-cert.pem
--rw-r--r--   0 dan       (1000) dan       (1000)     1193 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/certs/server-key.der
--rw-r--r--   0 dan       (1000) dan       (1000)     1679 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/certs/server-key.pem
--rw-r--r--   0 dan       (1000) dan       (1000)      459 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/certs/server-keyPub.pem
--rw-r--r--   0 dan       (1000) dan       (1000)     4658 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/test_aesgcmstream.py
--rw-r--r--   0 dan       (1000) dan       (1000)     4479 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/test_asn.py
--rw-r--r--   0 dan       (1000) dan       (1000)    27350 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/test_ciphers.py
--rw-r--r--   0 dan       (1000) dan       (1000)     5874 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/test_hashes.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2168 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/test_pwdbased.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1138 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/tests/test_random.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/windows/
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/windows/fips_ready/
--rw-r--r--   0 dan       (1000) dan       (1000)     1387 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/windows/fips_ready/user_settings.h
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.155306 wolfcrypt-5.5.4.post0/windows/non_fips/
--rw-r--r--   0 dan       (1000) dan       (1000)     1307 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/windows/non_fips/user_settings.h
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.159306 wolfcrypt-5.5.4.post0/wolfcrypt/
--rw-r--r--   0 dan       (1000) dan       (1000)     2325 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)      366 2022-12-30 17:28:37.000000 wolfcrypt-5.5.4.post0/wolfcrypt/_version.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3723 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/asn.py
--rw-r--r--   0 dan       (1000) dan       (1000)    57839 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/ciphers.py
--rw-r--r--   0 dan       (1000) dan       (1000)      858 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/exceptions.py
--rw-r--r--   0 dan       (1000) dan       (1000)    13715 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/hashes.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1552 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/pwdbased.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2432 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/random.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1239 2022-12-30 16:15:32.000000 wolfcrypt-5.5.4.post0/wolfcrypt/utils.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-12-30 17:43:44.159306 wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     4322 2022-12-30 17:43:44.000000 wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     1365 2022-12-30 17:43:44.000000 wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2022-12-30 17:43:44.000000 wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       12 2022-12-30 17:43:44.000000 wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       10 2022-12-30 17:43:44.000000 wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/top_level.txt
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.545830 wolfcrypt-5.6.0.post0/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1783 2023-05-02 15:47:27.000000 wolfcrypt-5.6.0.post0/ChangeLog.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)      918 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/LICENSING.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)      284 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/MANIFEST.in
+-rw-r--r--   0 dan       (1000) dan       (1000)     4322 2023-05-02 15:47:46.545830 wolfcrypt-5.6.0.post0/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     3426 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/README.rst
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/docs/
+-rw-r--r--   0 dan       (1000) dan       (1000)     8872 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/Makefile
+-rw-r--r--   0 dan       (1000) dan       (1000)     4036 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/asymmetric.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)     9672 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/conf.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1770 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/digest.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)      173 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/index.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)     1805 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/mac.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)      805 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/random.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)      869 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/streaming.rst
+-rw-r--r--   0 dan       (1000) dan       (1000)     1367 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/docs/symmetric.rst
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/requirements/
+-rw-r--r--   0 dan       (1000) dan       (1000)       36 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/requirements/docs.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        5 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/requirements/prod.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       12 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/requirements/setup.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       23 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/requirements/test.txt
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/scripts/
+-rw-r--r--   0 dan       (1000) dan       (1000)    36141 2023-04-19 10:54:30.000000 wolfcrypt-5.6.0.post0/scripts/build_ffi.py
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-05-02 15:47:46.545830 wolfcrypt-5.6.0.post0/setup.cfg
+-rwxr-xr-x   0 dan       (1000) dan       (1000)     3012 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/tests/
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/tests/__pycache__/
+-rw-r--r--   0 dan       (1000) dan       (1000)     7770 2022-12-30 16:17:34.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_aesgcmstream.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)    25741 2023-05-02 10:36:28.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_aesgcmstream.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)     5340 2022-12-30 16:17:34.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_asn.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)    11758 2023-05-02 10:36:28.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_asn.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)    31951 2022-12-30 16:17:34.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_ciphers.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)   105663 2023-05-02 10:36:28.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_ciphers.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)     5753 2022-12-30 16:17:34.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_hashes.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)    13493 2023-05-02 10:36:28.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_hashes.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)     1840 2022-12-30 16:17:34.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_pwdbased.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)     3376 2023-05-02 10:36:28.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_pwdbased.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)     2259 2022-12-30 16:17:34.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_random.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 dan       (1000) dan       (1000)     5889 2023-05-02 10:36:28.000000 wolfcrypt-5.6.0.post0/tests/__pycache__/test_random.cpython-311-pytest-7.3.1.pyc
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/tests/certs/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1249 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/certs/server-cert.der
+-rw-r--r--   0 dan       (1000) dan       (1000)     1749 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/certs/server-cert.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)     1193 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/certs/server-key.der
+-rw-r--r--   0 dan       (1000) dan       (1000)     1679 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/certs/server-key.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)      459 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/certs/server-keyPub.pem
+-rw-r--r--   0 dan       (1000) dan       (1000)     4658 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/test_aesgcmstream.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     4479 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/test_asn.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    27350 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/test_ciphers.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     5874 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/test_hashes.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2168 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/test_pwdbased.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1138 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/tests/test_random.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.537830 wolfcrypt-5.6.0.post0/windows/
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/windows/fips_ready/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1387 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/windows/fips_ready/user_settings.h
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/windows/non_fips/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1307 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/windows/non_fips/user_settings.h
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/wolfcrypt/
+-rw-r--r--   0 dan       (1000) dan       (1000)     2325 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      366 2023-05-02 09:10:58.000000 wolfcrypt-5.6.0.post0/wolfcrypt/_version.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3723 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/asn.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    57839 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/ciphers.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      858 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/exceptions.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    13715 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/hashes.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1552 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/pwdbased.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2432 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/random.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1239 2022-12-30 16:15:32.000000 wolfcrypt-5.6.0.post0/wolfcrypt/utils.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-02 15:47:46.541830 wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     4322 2023-05-02 15:47:46.000000 wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     1725 2023-05-02 15:47:46.000000 wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-05-02 15:47:46.000000 wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       12 2023-05-02 15:47:46.000000 wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       10 2023-05-02 15:47:46.000000 wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/top_level.txt
```

### Comparing `wolfcrypt-5.5.4.post0/ChangeLog.rst` & `wolfcrypt-5.6.0.post0/ChangeLog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+wolfCrypt-py Release 5.6.0 (May 2, 2022)
+==========================================
+
+* Add user settings path for scripts/user_settings_asm.sh during cmake
+* Update to wolfSSL version 5.6.0
+
+
 wolfCrypt-py Release 5.5.4 (December 30, 2022)
 ==========================================
 
 * Update to wolfSSL version 5.5.4
 
 wolfCrypt-py Release 5.5.3 (November 7, 2022)
 ==========================================
```

### Comparing `wolfcrypt-5.5.4.post0/LICENSING.rst` & `wolfcrypt-5.6.0.post0/LICENSING.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/PKG-INFO` & `wolfcrypt-5.6.0.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfcrypt
-Version: 5.5.4.post0
+Version: 5.6.0.post0
 Summary: Python module that encapsulates wolfSSL's crypto engine API.
 Home-page: https://github.com/wolfssl/wolfcrypt-py
 Author: wolfSSL Inc.
 Author-email: info@wolfssl.com
 License: GPLv2 or Commercial License
 Keywords: wolfssl,wolfcrypt,security,cryptography
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `wolfcrypt-5.5.4.post0/README.rst` & `wolfcrypt-5.6.0.post0/README.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/Makefile` & `wolfcrypt-5.6.0.post0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/asymmetric.rst` & `wolfcrypt-5.6.0.post0/docs/asymmetric.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/conf.py` & `wolfcrypt-5.6.0.post0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/digest.rst` & `wolfcrypt-5.6.0.post0/docs/digest.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/mac.rst` & `wolfcrypt-5.6.0.post0/docs/mac.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/random.rst` & `wolfcrypt-5.6.0.post0/docs/random.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/streaming.rst` & `wolfcrypt-5.6.0.post0/docs/streaming.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/docs/symmetric.rst` & `wolfcrypt-5.6.0.post0/docs/symmetric.rst`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/scripts/build_ffi.py` & `wolfcrypt-5.6.0.post0/scripts/build_ffi.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,24 +163,28 @@
 
     if not os.path.isdir(os.path.join(WOLFSSL_SRC_PATH, "wolfssl")):
         subprocess.run(["git", "submodule", "update", "--init", "--depth=1"])
 
     return checkout_version(version)
 
 
-def make_flags(prefix):
+def make_flags(prefix, fips):
     """ Returns compilation flags.
     """
     if sys.platform == "win32":
         flags = []
         flags.append("-DCMAKE_INSTALL_PREFIX={}".format(prefix))
         flags.append("-DWOLFSSL_CRYPT_TESTS=no")
         flags.append("-DWOLFSSL_EXAMPLES=no")
         flags.append("-DBUILD_SHARED_LIBS=no")
         flags.append("-DWOLFSSL_USER_SETTINGS=yes")
+        if fips:
+            flags.append("-DCMAKE_CXX_FLAGS=-I" + local_path("../IDE/WIN10"))
+        else:
+            flags.append("-DCMAKE_CXX_FLAGS=-I" + local_path("../IDE/WIN"))
         return " ".join(flags)
     else:
         flags = []
 
         if get_platform() in ["linux-x86_64", "linux-i686"]:
             flags.append("CFLAGS=-fPIC")
 
@@ -283,18 +287,18 @@
             if not os.path.exists(libwolfssl_path):
                 return False
             else:
                 return True
         else:
             return True
 
-def generate_libwolfssl():
+def generate_libwolfssl(fips):
     ensure_wolfssl_src(version)
     prefix = os.path.join(WOLFSSL_SRC_PATH, get_platform(), version)
-    make(make_flags(prefix))
+    make(make_flags(prefix, fips))
 
 def get_features(local_wolfssl, features):
     fips = False
 
     if sys.platform == "win32":
         # On Windows, we assume the local_wolfssl path is to a wolfSSL source
         # directory where the library has been built.
@@ -943,15 +947,15 @@
     if features["RSA_BLINDING"] and features["FIPS"]:
         # These settings can't coexist. See settings.h.
         features["RSA_BLINDING"] = 0
 
     if not local_wolfssl:
         print("Building wolfSSL...")
         if not get_libwolfssl():
-            generate_libwolfssl()
+            generate_libwolfssl(features["FIPS"])
 
     build_ffi(local_wolfssl, features)
 
 
 ffibuilder = FFI()
 main(ffibuilder)
```

### Comparing `wolfcrypt-5.5.4.post0/setup.py` & `wolfcrypt-5.6.0.post0/setup.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/__pycache__/test_aesgcmstream.cpython-310-pytest-7.2.0.pyc` & `wolfcrypt-5.6.0.post0/tests/__pycache__/test_aesgcmstream.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/__pycache__/test_asn.cpython-310-pytest-7.2.0.pyc` & `wolfcrypt-5.6.0.post0/tests/__pycache__/test_asn.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/__pycache__/test_ciphers.cpython-310-pytest-7.2.0.pyc` & `wolfcrypt-5.6.0.post0/tests/__pycache__/test_ciphers.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/__pycache__/test_hashes.cpython-310-pytest-7.2.0.pyc` & `wolfcrypt-5.6.0.post0/tests/__pycache__/test_hashes.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/__pycache__/test_pwdbased.cpython-310-pytest-7.2.0.pyc` & `wolfcrypt-5.6.0.post0/tests/__pycache__/test_pwdbased.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/__pycache__/test_random.cpython-310-pytest-7.2.0.pyc` & `wolfcrypt-5.6.0.post0/tests/__pycache__/test_random.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/certs/server-cert.der` & `wolfcrypt-5.6.0.post0/tests/certs/server-cert.der`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/certs/server-cert.pem` & `wolfcrypt-5.6.0.post0/tests/certs/server-cert.pem`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/certs/server-key.der` & `wolfcrypt-5.6.0.post0/tests/certs/server-key.der`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/certs/server-key.pem` & `wolfcrypt-5.6.0.post0/tests/certs/server-key.pem`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/test_aesgcmstream.py` & `wolfcrypt-5.6.0.post0/tests/test_aesgcmstream.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/test_asn.py` & `wolfcrypt-5.6.0.post0/tests/test_asn.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/test_ciphers.py` & `wolfcrypt-5.6.0.post0/tests/test_ciphers.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/test_hashes.py` & `wolfcrypt-5.6.0.post0/tests/test_hashes.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/test_pwdbased.py` & `wolfcrypt-5.6.0.post0/tests/test_pwdbased.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/tests/test_random.py` & `wolfcrypt-5.6.0.post0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/windows/fips_ready/user_settings.h` & `wolfcrypt-5.6.0.post0/windows/fips_ready/user_settings.h`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/windows/non_fips/user_settings.h` & `wolfcrypt-5.6.0.post0/windows/non_fips/user_settings.h`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/__init__.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/asn.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/asn.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/ciphers.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/ciphers.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/exceptions.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/exceptions.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/hashes.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/hashes.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/pwdbased.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/pwdbased.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/random.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/random.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt/utils.py` & `wolfcrypt-5.6.0.post0/wolfcrypt/utils.py`

 * *Files identical despite different names*

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/PKG-INFO` & `wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfcrypt
-Version: 5.5.4.post0
+Version: 5.6.0.post0
 Summary: Python module that encapsulates wolfSSL's crypto engine API.
 Home-page: https://github.com/wolfssl/wolfcrypt-py
 Author: wolfSSL Inc.
 Author-email: info@wolfssl.com
 License: GPLv2 or Commercial License
 Keywords: wolfssl,wolfcrypt,security,cryptography
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `wolfcrypt-5.5.4.post0/wolfcrypt.egg-info/SOURCES.txt` & `wolfcrypt-5.6.0.post0/wolfcrypt.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -20,19 +20,25 @@
 tests/test_aesgcmstream.py
 tests/test_asn.py
 tests/test_ciphers.py
 tests/test_hashes.py
 tests/test_pwdbased.py
 tests/test_random.py
 tests/__pycache__/test_aesgcmstream.cpython-310-pytest-7.2.0.pyc
+tests/__pycache__/test_aesgcmstream.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_asn.cpython-310-pytest-7.2.0.pyc
+tests/__pycache__/test_asn.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_ciphers.cpython-310-pytest-7.2.0.pyc
+tests/__pycache__/test_ciphers.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_hashes.cpython-310-pytest-7.2.0.pyc
+tests/__pycache__/test_hashes.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_pwdbased.cpython-310-pytest-7.2.0.pyc
+tests/__pycache__/test_pwdbased.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_random.cpython-310-pytest-7.2.0.pyc
+tests/__pycache__/test_random.cpython-311-pytest-7.3.1.pyc
 tests/certs/server-cert.der
 tests/certs/server-cert.pem
 tests/certs/server-key.der
 tests/certs/server-key.pem
 tests/certs/server-keyPub.pem
 windows/fips_ready/user_settings.h
 windows/non_fips/user_settings.h
```

