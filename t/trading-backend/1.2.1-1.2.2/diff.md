# Comparing `tmp/trading-backend-1.2.1.tar.gz` & `tmp/trading-backend-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading-backend-1.2.1.tar", last modified: Tue May  2 21:02:18 2023, max compression
+gzip compressed data, was "trading-backend-1.2.2.tar", last modified: Tue May  2 21:15:20 2023, max compression
```

## Comparing `trading-backend-1.2.1.tar` & `trading-backend-1.2.2.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:18.453791 trading-backend-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-02 21:01:48.000000 trading-backend-1.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 21:01:48.000000 trading-backend-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 21:01:48.000000 trading-backend-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 21:02:18.453791 trading-backend-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 21:01:48.000000 trading-backend-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 21:01:48.000000 trading-backend-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 21:02:18.453791 trading-backend-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-02 21:01:48.000000 trading-backend-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:18.449791 trading-backend-1.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:18.453791 trading-backend-1.2.1/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/exchanges/test_phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:18.453791 trading-backend-1.2.1/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 21:01:48.000000 trading-backend-1.2.1/tests/util/create_order_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:18.453791 trading-backend-1.2.1/trading_backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchange_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:18.453791 trading-backend-1.2.1/trading_backend/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 21:01:48.000000 trading-backend-1.2.1/trading_backend/exchanges/phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:18.453791 trading-backend-1.2.1/trading_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 21:02:18.000000 trading-backend-1.2.1/trading_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-02 21:02:18.000000 trading-backend-1.2.1/trading_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:02:18.000000 trading-backend-1.2.1/trading_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:02:18.000000 trading-backend-1.2.1/trading_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 21:02:18.000000 trading-backend-1.2.1/trading_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 21:02:18.000000 trading-backend-1.2.1/trading_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:20.240985 trading-backend-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-02 21:14:33.000000 trading-backend-1.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 21:14:33.000000 trading-backend-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 21:14:33.000000 trading-backend-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 21:15:20.240985 trading-backend-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 21:14:33.000000 trading-backend-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 21:14:33.000000 trading-backend-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 21:15:20.240985 trading-backend-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-02 21:14:33.000000 trading-backend-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:20.236986 trading-backend-1.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:20.236986 trading-backend-1.2.2/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/exchanges/test_phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:20.236986 trading-backend-1.2.2/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 21:14:33.000000 trading-backend-1.2.2/tests/util/create_order_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:20.236986 trading-backend-1.2.2/trading_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchange_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:20.240985 trading-backend-1.2.2/trading_backend/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 21:14:33.000000 trading-backend-1.2.2/trading_backend/exchanges/phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:15:20.236986 trading-backend-1.2.2/trading_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 21:15:20.000000 trading-backend-1.2.2/trading_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 21:15:20.000000 trading-backend-1.2.2/trading_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:15:20.000000 trading-backend-1.2.2/trading_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:15:20.000000 trading-backend-1.2.2/trading_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 21:15:20.000000 trading-backend-1.2.2/trading_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 21:15:20.000000 trading-backend-1.2.2/trading_backend.egg-info/top_level.txt
```

### Comparing `trading-backend-1.2.1/CHANGELOG.md` & `trading-backend-1.2.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.2] - 2023-05-02
+### Remove
+- Constants
+
 ## [1.2.1] - 2023-05-02
 ### Added
 - Constants
 
 ## [1.2.0] - 2023-05-02
 ### Updated
 - Supported python versions
```

### Comparing `trading-backend-1.2.1/LICENSE` & `trading-backend-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/PKG-INFO` & `trading-backend-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.1
+Version: 1.2.2
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.1](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.2](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.1/README.md` & `trading-backend-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# trading-backend [1.2.1](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.2](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.1/setup.py` & `trading-backend-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 # from distutils.extension import Extension
 from setuptools import find_packages
 from setuptools import setup
 
-from trading_backend.constants import PROJECT_NAME, VERSION
+from trading_backend import PROJECT_NAME, VERSION
 
 PACKAGES = find_packages(exclude=["tests"])
 
 
 # long description from README file
 with open('README.md', encoding='utf-8') as f:
     DESCRIPTION = f.read()
@@ -40,14 +40,15 @@
     packages=PACKAGES,
     include_package_data=True,
     long_description=DESCRIPTION,
     tests_require=["pytest"],
     test_suite="tests",
     zip_safe=False,
     data_files=[],
+    setup_requires=REQUIRED,
     install_requires=REQUIRED,
     python_requires=REQUIRES_PYTHON,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
```

### Comparing `trading-backend-1.2.1/tests/exchanges/test_ascendex.py` & `trading-backend-1.2.2/tests/exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_binance.py` & `trading-backend-1.2.2/tests/exchanges/test_binance.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_bitget.py` & `trading-backend-1.2.2/tests/exchanges/test_bitget.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_bybit.py` & `trading-backend-1.2.2/tests/exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_exchange.py` & `trading-backend-1.2.2/tests/exchanges/test_exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_gateio.py` & `trading-backend-1.2.2/tests/exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_huobi.py` & `trading-backend-1.2.2/tests/exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_huobipro.py` & `trading-backend-1.2.2/tests/exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_okx.py` & `trading-backend-1.2.2/tests/exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/exchanges/test_phemex.py` & `trading-backend-1.2.2/tests/exchanges/test_phemex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/util/__init__.py` & `trading-backend-1.2.2/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/tests/util/create_order_tests.py` & `trading-backend-1.2.2/tests/util/create_order_tests.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/__init__.py` & `trading-backend-1.2.2/trading_backend/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-from trading_backend.constants import (
-    VERSION,
-    PROJECT_NAME,
-)
+VERSION = "1.2.2"
+PROJECT_NAME = "trading-backend"
 
 from trading_backend import exchange_factory
 from trading_backend.exchange_factory import (
     create_exchange_backend,
     is_sponsoring,
 )
 from trading_backend import errors
```

### Comparing `trading-backend-1.2.1/trading_backend/constants.py` & `trading-backend-1.2.2/trading_backend/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,9 +9,15 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-VERSION = "1.2.1"
-PROJECT_NAME = "trading-backend"
+
+
+class TimeSyncError(RuntimeError):
+    pass
+
+
+class ExchangeAuthError(RuntimeError):
+    pass
```

### Comparing `trading-backend-1.2.1/trading_backend/errors.py` & `trading-backend-1.2.2/trading_backend/exchanges/huobipro.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import trading_backend.exchanges as exchanges
 
 
-class TimeSyncError(RuntimeError):
-    pass
+class HuobiPro(exchanges.Huobi):
 
-
-class ExchangeAuthError(RuntimeError):
-    pass
+    @classmethod
+    def get_name(cls):
+        return 'huobipro'
```

### Comparing `trading-backend-1.2.1/trading_backend/exchange_factory.py` & `trading-backend-1.2.2/trading_backend/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/__init__.py` & `trading-backend-1.2.2/trading_backend/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/ascendex.py` & `trading-backend-1.2.2/trading_backend/exchanges/ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/binance.py` & `trading-backend-1.2.2/trading_backend/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/bitget.py` & `trading-backend-1.2.2/trading_backend/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/bybit.py` & `trading-backend-1.2.2/trading_backend/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/exchange.py` & `trading-backend-1.2.2/trading_backend/exchanges/exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/gateio.py` & `trading-backend-1.2.2/trading_backend/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/huobi.py` & `trading-backend-1.2.2/trading_backend/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/huobipro.py` & `trading-backend-1.2.2/trading_backend/exchanges/phemex.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,29 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import aiohttp.streams
+
 import trading_backend.exchanges as exchanges
 
 
-class HuobiPro(exchanges.Huobi):
+class Phemex(exchanges.Exchange):
+    SPOT_ID = "Octobot"
+    MARGIN_ID = None
+    FUTURE_ID = "Octobot"
+    IS_SPONSORING = True
 
     @classmethod
     def get_name(cls):
-        return 'huobipro'
+        return 'phemex'
+
+    def _get_order_custom_id(self):
+        return f"{self._get_id()}{self._exchange.connector.client.uuid16()}"
+
+    def get_orders_parameters(self, params=None) -> dict:
+        if self._exchange.connector.client.options.get("brokerId", "") != self._get_id():
+            self._exchange.connector.client.options["brokerId"] = self._get_id()
+        return super().get_orders_parameters(params)
```

### Comparing `trading-backend-1.2.1/trading_backend/exchanges/okx.py` & `trading-backend-1.2.2/trading_backend/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.1/trading_backend.egg-info/PKG-INFO` & `trading-backend-1.2.2/trading_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.1
+Version: 1.2.2
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.1](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.2](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.1/trading_backend.egg-info/SOURCES.txt` & `trading-backend-1.2.2/trading_backend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 tests/exchanges/test_huobi.py
 tests/exchanges/test_huobipro.py
 tests/exchanges/test_okx.py
 tests/exchanges/test_phemex.py
 tests/util/__init__.py
 tests/util/create_order_tests.py
 trading_backend/__init__.py
-trading_backend/constants.py
 trading_backend/errors.py
 trading_backend/exchange_factory.py
 trading_backend.egg-info/PKG-INFO
 trading_backend.egg-info/SOURCES.txt
 trading_backend.egg-info/dependency_links.txt
 trading_backend.egg-info/not-zip-safe
 trading_backend.egg-info/requires.txt
```

