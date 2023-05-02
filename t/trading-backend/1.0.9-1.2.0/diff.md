# Comparing `tmp/trading-backend-1.0.9.tar.gz` & `tmp/trading-backend-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading-backend-1.0.9.tar", last modified: Wed Aug 25 07:00:37 2021, max compression
+gzip compressed data, was "trading-backend-1.2.0.tar", last modified: Tue May  2 20:39:10 2023, max compression
```

## Comparing `trading-backend-1.0.9.tar` & `trading-backend-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:37.664175 trading-backend-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      868 2021-08-25 07:00:15.000000 trading-backend-1.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-08-25 07:00:15.000000 trading-backend-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-08-25 07:00:15.000000 trading-backend-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-08-25 07:00:37.664175 trading-backend-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-08-25 07:00:15.000000 trading-backend-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-08-25 07:00:15.000000 trading-backend-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-08-25 07:00:37.664175 trading-backend-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-08-25 07:00:15.000000 trading-backend-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:37.660174 trading-backend-1.0.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:37.664175 trading-backend-1.0.9/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4816 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/exchanges/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/exchanges/test_ftx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/exchanges/test_okex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:37.664175 trading-backend-1.0.9/tests/util/
--rw-r--r--   0 runner    (1001) docker     (121)      716 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2021-08-25 07:00:15.000000 trading-backend-1.0.9/tests/util/create_order_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:37.664175 trading-backend-1.0.9/trading_backend/
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/exchange_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:37.664175 trading-backend-1.0.9/trading_backend/exchanges/
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/exchanges/binance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/exchanges/exchange.py
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/exchanges/ftx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/exchanges/gateio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-08-25 07:00:15.000000 trading-backend-1.0.9/trading_backend/exchanges/okex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 07:00:37.664175 trading-backend-1.0.9/trading_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-08-25 07:00:37.000000 trading-backend-1.0.9/trading_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      853 2021-08-25 07:00:37.000000 trading-backend-1.0.9/trading_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 07:00:37.000000 trading-backend-1.0.9/trading_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 07:00:37.000000 trading-backend-1.0.9/trading_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-08-25 07:00:37.000000 trading-backend-1.0.9/trading_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-25 07:00:37.000000 trading-backend-1.0.9/trading_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:10.785084 trading-backend-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-02 20:38:33.000000 trading-backend-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 20:38:33.000000 trading-backend-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 20:38:33.000000 trading-backend-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 20:39:10.785084 trading-backend-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 20:38:33.000000 trading-backend-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 20:38:33.000000 trading-backend-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 20:39:10.785084 trading-backend-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-02 20:38:33.000000 trading-backend-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:10.777084 trading-backend-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:10.781084 trading-backend-1.2.0/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/exchanges/test_phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:10.781084 trading-backend-1.2.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 20:38:33.000000 trading-backend-1.2.0/tests/util/create_order_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:10.781084 trading-backend-1.2.0/trading_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchange_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:10.785084 trading-backend-1.2.0/trading_backend/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 20:38:33.000000 trading-backend-1.2.0/trading_backend/exchanges/phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:10.781084 trading-backend-1.2.0/trading_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-02 20:39:10.000000 trading-backend-1.2.0/trading_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 20:39:10.000000 trading-backend-1.2.0/trading_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:39:10.000000 trading-backend-1.2.0/trading_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:39:10.000000 trading-backend-1.2.0/trading_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 20:39:10.000000 trading-backend-1.2.0/trading_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 20:39:10.000000 trading-backend-1.2.0/trading_backend.egg-info/top_level.txt
```

### Comparing `trading-backend-1.0.9/CHANGELOG.md` & `trading-backend-1.2.0/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,66 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.0] - 2023-05-02
+### Updated
+- Supported python versions
+
+## [1.0.19] - 2022-02-12
+### Added
+- Stop method
+
+## [1.0.18] - 2022-01-17
+### Updated
+- Bitget handling
+
+## [1.0.17] - 2022-10-12
+### Added
+- Exchange initialize
+- Binance legacy ids management
+### Updated
+- Binance broker id
+### Removed
+- FTX
+
+## [1.0.16] - 2022-10-12
+### Updated
+- CCXT version
+
+## [1.0.15] - 2022-09-24
+### Added
+- Phemex
+
+## [1.0.14] - 2022-08-07
+### Added
+- Bitget
+
+## [1.0.13] - 2022-06-05
+### Updated
+- Renamed OKEx into OKX
+
+## [1.0.12] - 2021-10-27
+### Added
+- Bybit spot and future
+- Ascendex
+
+### Fixed 
+- OKEx tests
+
+## [1.0.11] - 2021-08-31
+### Added
+- Huobi pro
+
+## [1.0.10] - 2021-08-27
+### Added
+- Huobi ids
+
 ## [1.0.9] - 2021-08-25
 ### Added
 - GateIO ids
 
 ## [1.0.8] - 2021-08-15
 ### Updated
 - Binance error messages
```

### Comparing `trading-backend-1.0.9/LICENSE` & `trading-backend-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trading-backend-1.0.9/PKG-INFO` & `trading-backend-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.0.9
+Version: 1.2.0
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # trading-backend [1.0.9](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
-        [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
-        [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
-        
-        - Install trading-backend from pip : 
-        
-        ``` {.sourceCode .bash}
-        $ python3 -m pip install trading-backend
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# trading-backend [1.2.0](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+[![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
+[![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
+[![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
+
+- Install trading-backend from pip : 
+
+``` {.sourceCode .bash}
+$ python3 -m pip install trading-backend
+```
```

### Comparing `trading-backend-1.0.9/README.md` & `trading-backend-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# trading-backend [1.0.9](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.0](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.0.9/setup.py` & `trading-backend-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,39 +17,37 @@
 from setuptools import find_packages
 from setuptools import setup
 
 from trading_backend import PROJECT_NAME, VERSION
 
 PACKAGES = find_packages(exclude=["tests"])
 
-packages_list = []
 
 # long description from README file
 with open('README.md', encoding='utf-8') as f:
     DESCRIPTION = f.read()
 
 REQUIRED = open('requirements.txt').readlines()
 REQUIRES_PYTHON = '>=3.8'
 
 setup(
     name=PROJECT_NAME,
     version=VERSION,
     url='https://github.com/Drakkar-Software/trading-backend',
     license='LGPL-3.0',
     author='Drakkar-Software',
-    author_email='drakkar-software@protonmail.com',
+    author_email='contact@drakkar.software',
     description='Trading tools',
     packages=PACKAGES,
     include_package_data=True,
     long_description=DESCRIPTION,
     tests_require=["pytest"],
     test_suite="tests",
     zip_safe=False,
     data_files=[],
-    setup_requires=REQUIRED,
     install_requires=REQUIRED,
     python_requires=REQUIRES_PYTHON,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
```

### Comparing `trading-backend-1.0.9/tests/exchanges/test_ftx.py` & `trading-backend-1.2.0/tests/exchanges/test_phemex.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,25 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import pytest
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
-from tests import ftx_exchange
+from tests import phemex_exchange
 
 
-def test_get_name(ftx_exchange):
-    assert exchanges.FTX(ftx_exchange).get_name() == ccxt.async_support.ftx().name.lower()
+def test_get_name(phemex_exchange):
+    assert exchanges.Phemex(phemex_exchange).get_name() == ccxt.async_support.phemex().name.lower()
 
 
 @pytest.mark.asyncio
-async def test_get_orders_parameters(ftx_exchange):
-    exchange = exchanges.FTX(ftx_exchange)
-    await create_order_tests.create_order_mocked_test(exchange,
-                                                      exchange_private_post_order_method_name="privatePostOrders",
-                                                      exchange_request_referral_key="externalReferralProgram",
-                                                      should_contains=False)
+async def test_get_orders_parameters(phemex_exchange):
+    exchange = exchanges.Phemex(phemex_exchange)
+    # stopPxEp not in ccxt "market" which is used as default value, provide it in mock
+    await create_order_tests.create_order_mocked_test_args(
+        exchange,
+        exchange_private_post_order_method_name="privatePostSpotOrders",
+        exchange_request_referral_key="clOrdID",
+        should_contains=True,
+        result_is_list=False,
+        post_order_mock_return_value={'data': {'stopPxEp': 0}})
```

### Comparing `trading-backend-1.0.9/tests/exchanges/test_gateio.py` & `trading-backend-1.2.0/tests/exchanges/test_ascendex.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import mock
+import pytest
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
-from tests import gateio_exchange
+import tests.util.create_order_tests as create_order_tests
+from tests import ascendex_exchange
 
 
-def test_get_name(gateio_exchange):
-    assert exchanges.GateIO(gateio_exchange).get_name() == ccxt.async_support.gateio().name.lower()
+def test_get_name(ascendex_exchange):
+    assert exchanges.Ascendex(ascendex_exchange).get_name() == ccxt.async_support.ascendex().name.lower()
 
 
-def test_get_orders_parameters(gateio_exchange):
-    exchange = exchanges.GateIO(gateio_exchange)
-    assert exchange.get_headers() == {exchange.HEADER_KEY: exchange._get_id()}
+@pytest.mark.asyncio
+async def test_get_orders_parameters(ascendex_exchange):
+    exchange = exchanges.Ascendex(ascendex_exchange)
+    with mock.patch.object(exchange._exchange.connector.client, "v1PrivateGetInfo", mock.AsyncMock(return_value={})):
+        await create_order_tests.create_order_mocked_test_args(
+            exchange,
+            exchange_private_post_order_method_name="v1PrivateAccountCategoryPostOrder",
+            exchange_request_referral_key="id",
+            should_contains=True)
```

### Comparing `trading-backend-1.0.9/tests/exchanges/test_okex.py` & `trading-backend-1.2.0/tests/exchanges/test_bitget.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import mock
 import pytest
 import ccxt.async_support
 import trading_backend.exchanges as exchanges
 import tests.util.create_order_tests as create_order_tests
-from tests import okex_exchange
+from tests import bitget_exchange
 
 
-def test_get_name(okex_exchange):
-    assert exchanges.OKEx(okex_exchange).get_name() == ccxt.async_support.okex().name.lower()
+def test_get_name(bitget_exchange):
+    assert exchanges.Bitget(bitget_exchange).get_name() == ccxt.async_support.bitget().name.lower()
 
 
 @pytest.mark.asyncio
-async def test_get_orders_parameters(okex_exchange):
-    exchange = exchanges.OKEx(okex_exchange)
-    await create_order_tests.create_order_mocked_test(exchange,
-                                                      exchange_private_post_order_method_name="privatePostTradeOrder",
-                                                      exchange_request_referral_key="clOrdId",
-                                                      should_contains=True)
+async def test_get_orders_parameters(bitget_exchange):
+    exchange = exchanges.Bitget(bitget_exchange)
+    await create_order_tests.create_order_mocked_test_args(
+        exchange,
+        exchange_private_post_order_method_name="privateSpotPostTradeOrders",
+        exchange_request_referral_key="clientOrderId",
+        should_contains=True)
```

### Comparing `trading-backend-1.0.9/tests/util/__init__.py` & `trading-backend-1.2.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.0.9/tests/util/create_order_tests.py` & `trading-backend-1.2.0/tests/exchanges/test_huobipro.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,34 +10,30 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import mock
+import pytest
+import ccxt.async_support
 import trading_backend.exchanges as exchanges
+import tests.util.create_order_tests as create_order_tests
+from tests import huobipro_exchange
 
 
-async def create_order_mocked_test(exchange: exchanges.Exchange,
-                                   exchange_private_post_order_method_name: str,
-                                   exchange_request_referral_key: str,
-                                   should_contains: bool = True,
-                                   symbol: str = "BTC/USDT",
-                                   amount: int = 1,
-                                   price: int = 1):
-    with mock.patch.object(exchange._exchange.connector.client,
-                           exchange_private_post_order_method_name,
-                           mock.AsyncMock(return_value={})) as post_order_mock:
-        # without referral patch
-        await exchange._exchange.connector.client.create_limit_buy_order(symbol, amount, price)
-        if should_contains:
-            assert exchange._get_id() not in post_order_mock.call_args[0][0].get(exchange_request_referral_key, "")
-        else:
-            assert exchange._get_id() != post_order_mock.call_args[0][0].get(exchange_request_referral_key, "")
+def test_get_name(huobipro_exchange):
+    # huobi on ccxt
+    assert exchanges.HuobiPro(huobipro_exchange).get_name() != ccxt.async_support.huobipro().name.lower()
+    assert exchanges.HuobiPro(huobipro_exchange).get_name() == "huobipro"
+
 
-        # with referral patch
-        await exchange._exchange.connector.client.create_limit_buy_order(symbol, amount, price,
-                                                                         params=exchange.get_orders_parameters())
-        if should_contains:
-            assert exchange._get_id() in post_order_mock.call_args[0][0].get(exchange_request_referral_key, "")
-        else:
-            assert exchange._get_id() == post_order_mock.call_args[0][0].get(exchange_request_referral_key, "")
+@pytest.mark.asyncio
+async def test_get_orders_parameters(huobipro_exchange):
+    exchange = exchanges.HuobiPro(huobipro_exchange)
+    with mock.patch.object(exchange._exchange.connector.client,
+                           "fetch_accounts", mock.AsyncMock(return_value=[{'id': 1}])):
+        await create_order_tests.create_order_mocked_test_args(
+            exchange,
+            exchange_private_post_order_method_name="spotPrivatePostV1OrderOrdersPlace",
+            exchange_request_referral_key="client-order-id",
+            should_contains=True)
```

### Comparing `trading-backend-1.0.9/trading_backend/__init__.py` & `trading-backend-1.2.0/trading_backend/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-VERSION = "1.0.9"
+VERSION = "1.2.0"
 PROJECT_NAME = "trading-backend"
 
 from trading_backend import exchange_factory
 from trading_backend.exchange_factory import (
     create_exchange_backend,
     is_sponsoring,
 )
```

### Comparing `trading-backend-1.0.9/trading_backend/errors.py` & `trading-backend-1.2.0/trading_backend/errors.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.0.9/trading_backend/exchange_factory.py` & `trading-backend-1.2.0/trading_backend/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.0.9/trading_backend/exchanges/binance.py` & `trading-backend-1.2.0/trading_backend/exchanges/binance.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,50 +9,80 @@
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
 
 
 class Binance(exchanges.Exchange):
-    SPOT_ID = "T9698EB7"
+    LEGACY_SPOT_ID = "T9698EB7"
+    SPOT_ID = "HR452G85"
     MARGIN_ID = None
+    LEGACY_FUTURE_ID = "uquVg2pc"
     FUTURE_ID = "uquVg2pc"
-    REF_ID = "135007948"
+    LEGACY_REF_ID = "135007948"
+    REF_ID = "528112221"
     IS_SPONSORING = True
 
     @classmethod
     def get_name(cls):
         return 'binance'
 
     def _get_order_custom_id(self):
         return f"x-{self._get_id()}{self._exchange.connector.client.uuid22()}"
 
+    @classmethod
+    def use_legacy_ids(cls):
+        cls.SPOT_ID = cls.LEGACY_SPOT_ID
+        cls.FUTURE_ID = cls.LEGACY_FUTURE_ID
+
     def get_orders_parameters(self, params=None) -> dict:
         params = super().get_orders_parameters(params)
         params.update({'newClientOrderId': self._get_order_custom_id()})
         return params
 
+    async def _ensure_broker_status(self):
+        try:
+            details = await self._get_account_referral_details()
+            if not details.get("rebateWorking", False):
+                if (ref_id := details.get("referrerId", None)) and ref_id == self.LEGACY_REF_ID:
+                    self.use_legacy_ids()
+                    details = await self._get_account_referral_details()
+                    if details.get("rebateWorking", False):
+                        return "Using legacy broker id"
+                return f"Broker rebate not working: {details}"
+            return f"Broker rebate is enabled."
+        except Exception as err:
+            return f"Broker rebate check error: {err}"
+
+    async def _get_account_referral_details(self) -> dict:
+        return await self._exchange.connector.client.sapi_get_apireferral_ifnewuser(
+            params=self._exchange._get_params({
+                "apiAgentCode": self._get_id()
+            })
+        )
+
     async def _inner_is_valid_account(self) -> (bool, str):
+        details = None
         try:
-            details = await self._exchange.connector.client.sapi_get_apireferral_ifnewuser(
-                params=self._exchange._get_params({
-                    "apiAgentCode": self._get_id()
-                })
-            )
+            details = await self._get_account_referral_details()
             if not details.get("rebateWorking", False):
                 ref_id = details.get("referrerId", None)
                 if ref_id is not None:
                     return False, f"This account has a referral id equal to {ref_id} " \
                                   f"which is incompatible ({self.REF_ID} as referral id or no referral id is required)"
                 return False, f"This account is incompatible, details: {details}. Please report this message to " \
                               f"admins for investigation. " \
                               f"An account with {self.REF_ID} as referral id or no referral id is required."
             if not details.get("ifNewUser", False):
                 return False, "Binance requires accounts that were created after july 1st 2021, " \
                               "this account is too old."
         except AttributeError:
+            if isinstance(details, aiohttp.streams.StreamReader):
+                return False, "Error when fetching exchange data (unreadable response)"
             return False, "Invalid request parameters"
         return True, None
```

### Comparing `trading-backend-1.0.9/trading_backend/exchanges/exchange.py` & `trading-backend-1.2.0/trading_backend/exchanges/exchange.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,22 +23,35 @@
     MARGIN_ID = None
     FUTURE_ID = None
     IS_SPONSORING = False
 
     def __init__(self, exchange):
         self._exchange = exchange
 
+        # add backend headers
+        self._exchange.connector.add_headers(self.get_headers())
+
+    def stop(self):
+        self._exchange = None
+
     @classmethod
     def get_name(cls):
         return 'default'
 
     @classmethod
     def is_sponsoring(cls) -> bool:
         return cls.IS_SPONSORING
 
+    async def initialize(self) -> str:
+        default = f"{self.get_name().capitalize()} backend initialized."
+        return f"{default} {await self._ensure_broker_status()}" if self.is_sponsoring() else default
+
+    async def _ensure_broker_status(self):
+        return f"Broker rebate is enabled."
+
     def get_headers(self) -> dict:
         return {}
 
     def get_orders_parameters(self, params=None) -> dict:
         if params is None:
             params = {}
         return params
```

### Comparing `trading-backend-1.0.9/trading_backend/exchanges/ftx.py` & `trading-backend-1.2.0/trading_backend/exchanges/gateio.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,37 +12,24 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import trading_backend.exchanges as exchanges
 
 
-class FTX(exchanges.Exchange):
+class GateIO(exchanges.Exchange):
     SPOT_ID = "Octobot"
     MARGIN_ID = "Octobot"
     FUTURE_ID = "Octobot"
-    REF_ID = "33613187"
     IS_SPONSORING = True
+    HEADER_KEY = "X-Gate-Channel-Id"
 
     @classmethod
     def get_name(cls):
-        return 'ftx'
+        return 'gateio'
 
-    def get_orders_parameters(self, params=None) -> dict:
-        params = super().get_orders_parameters(params)
-        params.update({'externalReferralProgram': self._get_id()})
-        return params
+    def get_headers(self):
+        return {self.HEADER_KEY: self._get_id()}
 
     async def _inner_is_valid_account(self) -> (bool, str):
-        """
-        Response doc from https://help.ftx.com/hc/en-us/articles/360044373831-External-Referral-Programs
-        {
-        'enabled': True,
-        'externalReferralProgram': 'TradeX100',
-        'readOnly': False,
-        'requireWhitelistedIp': False,
-        'subaccountNickname': None,
-        'withdrawalEnabled': False
-        }
-        """
-        # Seems to be unnecessary because the program name is overwritten in `get_orders_parameters`
+        # Nothing to do
         return await super()._inner_is_valid_account()
```

### Comparing `trading-backend-1.0.9/trading_backend/exchanges/gateio.py` & `trading-backend-1.2.0/trading_backend/exchanges/bitget.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import trading_backend.exchanges as exchanges
 
 
-class GateIO(exchanges.Exchange):
-    SPOT_ID = "Octobot"
-    MARGIN_ID = "Octobot"
-    FUTURE_ID = "Octobot"
+class Bitget(exchanges.Exchange):
+    SPOT_ID = "Octobot"      # include # as it is required to generate client_oid
+    FUTURE_ID = "Octobot"    # include # as it is required to generate client_oid
     IS_SPONSORING = True
-    HEADER_KEY = "X-Gate-Channel-Id"
 
     @classmethod
     def get_name(cls):
-        return 'gate.io'
+        return 'bitget'
 
-    def get_headers(self):
-        return {self.HEADER_KEY: self._get_id()}
+    def _generate_order_id(self):
+        return f"{self._get_id()}#{self._exchange.connector.client.uuid22()}"
+
+    def get_orders_parameters(self, params=None) -> dict:
+        self._exchange.connector.client.options["broker"] = self._get_id()
+        params = super().get_orders_parameters(params)
+        params["clientOrderId"] = self._generate_order_id()
+        return super().get_orders_parameters(params)
 
     async def _inner_is_valid_account(self) -> (bool, str):
         # Nothing to do
         return await super()._inner_is_valid_account()
```

### Comparing `trading-backend-1.0.9/trading_backend/exchanges/okex.py` & `trading-backend-1.2.0/trading_backend/exchanges/okx.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import trading_backend.exchanges as exchanges
 
 
-class OKEx(exchanges.Exchange):
+class OKX(exchanges.Exchange):
     SPOT_ID = "c812bf5944b749BC"
     MARGIN_ID = "c812bf5944b749BC"
     FUTURE_ID = "c812bf5944b749BC"
     IS_SPONSORING = True
 
     @classmethod
     def get_name(cls):
-        return 'okex'
+        return 'okx'
 
     def get_orders_parameters(self, params=None) -> dict:
         if self._exchange.connector.client.options.get("brokerId", "") != self._get_id():
             self._exchange.connector.client.options["brokerId"] = self._get_id()
         return super().get_orders_parameters(params)
 
     async def _inner_is_valid_account(self) -> (bool, str):
```

### Comparing `trading-backend-1.0.9/trading_backend.egg-info/PKG-INFO` & `trading-backend-1.2.0/trading_backend.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.0.9
+Version: 1.2.0
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
-Author-email: drakkar-software@protonmail.com
+Author-email: contact@drakkar.software
 License: LGPL-3.0
-Description: # trading-backend [1.0.9](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
-        [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
-        [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
-        [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
-        
-        - Install trading-backend from pip : 
-        
-        ``` {.sourceCode .bash}
-        $ python3 -m pip install trading-backend
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# trading-backend [1.2.0](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+[![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
+[![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
+[![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
+
+- Install trading-backend from pip : 
+
+``` {.sourceCode .bash}
+$ python3 -m pip install trading-backend
+```
```

