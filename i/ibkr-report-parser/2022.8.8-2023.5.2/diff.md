# Comparing `tmp/ibkr-report-parser-2022.8.8.tar.gz` & `tmp/ibkr-report-parser-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibkr-report-parser-2022.8.8.tar", last modified: Mon Aug  8 13:19:10 2022, max compression
+gzip compressed data, was "ibkr-report-parser-2023.5.2.tar", last modified: Tue May  2 09:39:10 2023, max compression
```

## Comparing `ibkr-report-parser-2022.8.8.tar` & `ibkr-report-parser-2023.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4574 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/ibkr_report/
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/cron.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5006 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/exchangerates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4713 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.333444 ibkr-report-parser-2022.8.8/ibkr_report/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/ibkr_report/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/static/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/ibkr_report/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)   109579 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/static/images/custom_statement.png
--rw-r--r--   0 runner    (1001) docker     (121)    53837 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/static/images/run_statement.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/ibkr_report/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (121)     6413 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/ibkr_report/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/templates/result.html
--rw-r--r--   0 runner    (1001) docker     (121)     4494 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     5704 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/trade.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/ibkr_report/website.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4574 2022-08-08 13:19:10.000000 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-08-08 13:19:10.000000 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 13:19:10.000000 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-08 13:19:10.000000 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 13:19:10.000000 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-08 13:19:10.000000 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-08 13:19:10.000000 ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:10.337444 ibkr-report-parser-2022.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/tests/test_cron.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/tests/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     9338 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-08-08 13:19:01.000000 ibkr-report-parser-2022.8.8/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.898829 ibkr-report-parser-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-05-02 09:39:10.898829 ibkr-report-parser-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3630 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.894829 ibkr-report-parser-2023.5.2/ibkr_report/
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      647 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/cron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5061 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/exchangerates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.890829 ibkr-report-parser-2023.5.2/ibkr_report/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.894829 ibkr-report-parser-2023.5.2/ibkr_report/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/static/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.894829 ibkr-report-parser-2023.5.2/ibkr_report/static/images/
+-rw-r--r--   0 runner    (1001) docker     (122)   109579 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/static/images/custom_statement.png
+-rw-r--r--   0 runner    (1001) docker     (122)    53837 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/static/images/run_statement.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.894829 ibkr-report-parser-2023.5.2/ibkr_report/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6490 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.894829 ibkr-report-parser-2023.5.2/ibkr_report/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/templates/result.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/trade.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/ibkr_report/website.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.894829 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-05-02 09:39:10.000000 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-05-02 09:39:10.000000 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 09:39:10.000000 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-02 09:39:10.000000 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 09:39:10.000000 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-05-02 09:39:10.000000 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-02 09:39:10.000000 ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 09:39:10.898829 ibkr-report-parser-2023.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:39:10.894829 ibkr-report-parser-2023.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2869 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/tests/test_cron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/tests/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9338 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3686 2023-05-02 09:38:56.000000 ibkr-report-parser-2023.5.2/tests/test_storage.py
```

### Comparing `ibkr-report-parser-2022.8.8/LICENSE` & `ibkr-report-parser-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/PKG-INFO` & `ibkr-report-parser-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ibkr-report-parser
-Version: 2022.8.8
+Version: 2023.5.2
 Summary: Interactive Brokers (IBKR) Report Parser for MyTax (vero.fi)
 Home-page: https://github.com/oittaa/ibkr-report-parser
 Author: Oittaa
 Author-email: 
 Keywords: Interactive Brokers,IBKR,OmaVero,MyTax,vero.fi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: docker
 Provides-Extra: gcp
 License-File: LICENSE
 
 # ibkr-report-parser
```

### Comparing `ibkr-report-parser-2022.8.8/README.md` & `ibkr-report-parser-2023.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/__init__.py` & `ibkr-report-parser-2023.5.2/ibkr_report/__init__.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/__main__.py` & `ibkr-report-parser-2023.5.2/ibkr_report/__main__.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/cron.py` & `ibkr-report-parser-2023.5.2/ibkr_report/cron.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/definitions.py` & `ibkr-report-parser-2023.5.2/ibkr_report/definitions.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/exchangerates.py` & `ibkr-report-parser-2023.5.2/ibkr_report/exchangerates.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import csv
 import logging
 import re
 from codecs import iterdecode
 from datetime import timedelta
 from decimal import Decimal
 from io import BytesIO
-from typing import Iterable
+from typing import Iterable, Optional
 from urllib.error import HTTPError
 from urllib.request import urlopen
 from zipfile import BadZipFile, ZipFile
 
 from ibkr_report.definitions import (
     DATE_FORMAT,
     EXCHANGE_RATES_URL,
@@ -28,15 +28,18 @@
 
 class ExchangeRates:
     """Euro foreign exchange rates"""
 
     rates: CurrencyDict
 
     def __init__(
-        self, url: str = None, storage_type: StorageType = None, **kwargs
+        self,
+        url: Optional[str] = None,
+        storage_type: Optional[StorageType] = None,
+        **kwargs,
     ) -> None:
         """Tries to fetch a previously built exchange rate dictionary from a
         Storage backend. If that's not available, downloads the official
         exchange rates from European Central Bank and builds a new dictionary
         from it.
         """
         url = url or EXCHANGE_RATES_URL
```

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/report.py` & `ibkr-report-parser-2023.5.2/ibkr_report/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     details: List[TradeDetails]
     options: ReportOptions
     rates: ExchangeRates
     _trade: Optional[Trade] = None
 
     def __init__(
         self,
-        file: Iterable[bytes] = None,
+        file: Optional[Iterable[bytes]] = None,
         report_currency: str = CURRENCY,
         use_deemed_acquisition_cost: bool = USE_DEEMED_ACQUISITION_COST,
     ) -> None:
         self.details = []
         self.options = ReportOptions(
             report_currency=report_currency.upper(),
             deemed_acquisition_cost=use_deemed_acquisition_cost,
```

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/static/css/main.css` & `ibkr-report-parser-2023.5.2/ibkr_report/static/css/main.css`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/static/images/custom_statement.png` & `ibkr-report-parser-2023.5.2/ibkr_report/static/images/custom_statement.png`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/static/images/run_statement.png` & `ibkr-report-parser-2023.5.2/ibkr_report/static/images/run_statement.png`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/storage.py` & `ibkr-report-parser-2023.5.2/ibkr_report/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 
 class Storage(ABC):
     """Storage class to save exchange rates."""
 
     cache: bool = True
 
-    def save(self, content: CurrencyDict, filename: str = None) -> None:
+    def save(self, content: CurrencyDict, filename: Optional[str] = None) -> None:
         """Save CurrencyDict to storage."""
         filename = filename or self.get_filename()
         log.debug("Save to '%s' using %s backend.", filename, self.name)
         if self.cache:
             Cache.set(filename, content)
         self._save(content, filename)
 
-    def load(self, filename: str = None) -> CurrencyDict:
+    def load(self, filename: Optional[str] = None) -> CurrencyDict:
         """Load CurrencyDict from storage."""
         filename = filename or self.get_filename()
         log.debug("Load '%s' using %s backend.", filename, self.name)
         if self.cache:
             content = Cache.get(filename)
             if content:
                 log.debug("Cache hit: %s", filename)
@@ -61,15 +61,15 @@
 
     @property
     def name(self) -> str:
         """Class name"""
         return self.__class__.__name__
 
     @staticmethod
-    def get_filename(identifier: str = None) -> str:
+    def get_filename(identifier: Optional[str] = None) -> str:
         """Generate a filename based on the current date.
 
         Optionally you can give your own identifier that distinguishes files.
         """
         if identifier is None:
             identifier = datetime.now().strftime(DATE_FORMAT)
         return SAVED_RATES_FILE.format(identifier)
@@ -94,15 +94,15 @@
     def _load(self, filename: str) -> CurrencyDict:
         return {}
 
 
 class AmazonS3(Storage):
     """Amazon S3 backend"""
 
-    def __init__(self, bucket_id: str = None) -> None:
+    def __init__(self, bucket_id: Optional[str] = None) -> None:
         boto3 = importlib.import_module("boto3")
 
         log.debug("Using %s backend.", self.name)
         self.bucket_id = bucket_id or BUCKET_ID
         self.aws_s3 = boto3.resource("s3")  # type: ignore
         bucket = self.aws_s3.Bucket(self.bucket_id)
         bucket.create()
@@ -118,15 +118,15 @@
         except self.aws_s3.meta.client.exceptions.NoSuchKey:
             return {}
 
 
 class GoogleCloudStorage(Storage):
     """Google Cloud Storage backend"""
 
-    def __init__(self, bucket_id: str = None) -> None:
+    def __init__(self, bucket_id: Optional[str] = None) -> None:
         storage = importlib.import_module("google.cloud.storage")
         exceptions = importlib.import_module("google.cloud.exceptions")
 
         log.debug("Using %s backend.", self.name)
         self.bucket_id = bucket_id or BUCKET_ID
         client = storage.Client()  # type: ignore
         try:
@@ -161,15 +161,15 @@
         try:
             with open(self.storage_dir.joinpath(filename), "rb") as file:
                 return self.decode(file.read())
         except FileNotFoundError:
             return {}
 
 
-def get_storage(storage_type: StorageType = None) -> Type[Storage]:
+def get_storage(storage_type: Optional[StorageType] = None) -> Type[Storage]:
     """Returns a storage backend."""
     if storage_type is None:
         storage_type = StorageType(STORAGE_TYPE)
 
     cloud_storage = get_cloud_storage(storage_type)
     if cloud_storage:
         return cloud_storage
@@ -178,15 +178,17 @@
         return LocalStorage
     if storage_type is StorageType.DISABLED:
         return StorageDisabled
 
     raise NotImplementedError(f"Not implemented: {storage_type!r}")
 
 
-def get_cloud_storage(storage_type: StorageType = None) -> Optional[Type[Storage]]:
+def get_cloud_storage(
+    storage_type: Optional[StorageType] = None,
+) -> Optional[Type[Storage]]:
     """Cloud storages with storage buckets."""
     if storage_type is StorageType.AWS:
         return AmazonS3
     if storage_type is StorageType.GCP:
         return GoogleCloudStorage
     # Past the cloud storage options, fail if BUCKET_ID is set
     if BUCKET_ID:
```

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/templates/index.html` & `ibkr-report-parser-2023.5.2/ibkr_report/templates/index.html`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/templates/result.html` & `ibkr-report-parser-2023.5.2/ibkr_report/templates/result.html`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/tools.py` & `ibkr-report-parser-2023.5.2/ibkr_report/tools.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/trade.py` & `ibkr-report-parser-2023.5.2/ibkr_report/trade.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report/website.py` & `ibkr-report-parser-2023.5.2/ibkr_report/website.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/PKG-INFO` & `ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ibkr-report-parser
-Version: 2022.8.8
+Version: 2023.5.2
 Summary: Interactive Brokers (IBKR) Report Parser for MyTax (vero.fi)
 Home-page: https://github.com/oittaa/ibkr-report-parser
 Author: Oittaa
 Author-email: 
 Keywords: Interactive Brokers,IBKR,OmaVero,MyTax,vero.fi
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: docker
 Provides-Extra: gcp
 License-File: LICENSE
 
 # ibkr-report-parser
```

### Comparing `ibkr-report-parser-2022.8.8/ibkr_report_parser.egg-info/SOURCES.txt` & `ibkr-report-parser-2023.5.2/ibkr_report_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/setup.py` & `ibkr-report-parser-2023.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,28 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Other Audience",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     entry_points={
         "console_scripts": [
             "ibkr-report-parser=ibkr_report.__main__:main",
         ],
     },
     setup_requires=[
         "wheel",
     ],
-    install_requires=["flask==2.2.1"],
+    install_requires=["flask==2.3.2"],
     extras_require={
-        "aws": ["boto3==1.24.46"],
+        "aws": ["boto3==1.26.124"],
         "docker": ["gunicorn==20.1.0"],
-        "gcp": ["google-cloud-storage==2.5.0"],
+        "gcp": ["google-cloud-storage==2.8.0"],
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

### Comparing `ibkr-report-parser-2022.8.8/tests/test_cron.py` & `ibkr-report-parser-2023.5.2/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/tests/test_exchange.py` & `ibkr-report-parser-2023.5.2/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/tests/test_report.py` & `ibkr-report-parser-2023.5.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/tests/test_smoke.py` & `ibkr-report-parser-2023.5.2/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `ibkr-report-parser-2022.8.8/tests/test_storage.py` & `ibkr-report-parser-2023.5.2/tests/test_storage.py`

 * *Files identical despite different names*

