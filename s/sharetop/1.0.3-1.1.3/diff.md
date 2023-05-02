# Comparing `tmp/sharetop-1.0.3.tar.gz` & `tmp/sharetop-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.0.3.tar", last modified: Sun Apr 30 13:59:36 2023, max compression
+gzip compressed data, was "sharetop-1.1.3.tar", last modified: Tue May  2 15:40:57 2023, max compression
```

## Comparing `sharetop-1.0.3.tar` & `sharetop-1.1.3.tar`

### file list

```diff
@@ -1,65 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.691547 sharetop-1.0.3/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    39033 2023-04-30 13:59:36.656552 sharetop-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    37774 2023-04-29 10:56:21.000000 sharetop-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 13:59:36.691547 sharetop-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.116289 sharetop-1.0.3/sharetop/
--rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.0.3/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-04-30 13:59:33.000000 sharetop-1.0.3/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.182171 sharetop-1.0.3/sharetop/api/
--rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.0.3/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.196872 sharetop-1.0.3/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.0.3/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.205594 sharetop-1.0.3/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.0.3/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.303960 sharetop-1.0.3/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.0.3/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.0.3/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.0.3/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.0.3/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.329184 sharetop-1.0.3/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.0.3/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.0.3/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12266 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.0.3/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.480328 sharetop-1.0.3/sharetop/core/fund/
--rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.0.3/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.0.3/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.515791 sharetop-1.0.3/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.0.3/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.0.3/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.591429 sharetop-1.0.3/sharetop/core/stock/
--rw-rw-rw-   0        0        0      491 2023-04-25 21:15:03.000000 sharetop-1.0.3/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.0.3/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.0.3/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14300 2023-04-27 15:24:55.000000 sharetop-1.0.3/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.0.3/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.626407 sharetop-1.0.3/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.0.3/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.0.3/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     2704 2023-04-24 00:30:13.000000 sharetop-1.0.3/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.652329 sharetop-1.0.3/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.0.3/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0      419 2023-04-10 00:57:53.000000 sharetop-1.0.3/sharetop/parser/base.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.655192 sharetop-1.0.3/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.0.3/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.0.3/sharetop/test/test1.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.179856 sharetop-1.0.3/sharetop.egg-info/
--rw-rw-rw-   0        0        0    39033 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1501 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.887937 sharetop-1.1.3/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0    39033 2023-05-02 15:40:57.886932 sharetop-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    37774 2023-04-29 10:56:21.000000 sharetop-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 15:40:57.887937 sharetop-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.647402 sharetop-1.1.3/sharetop/
+-rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.1.3/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-05-02 15:40:33.000000 sharetop-1.1.3/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.692767 sharetop-1.1.3/sharetop/api/
+-rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.1.3/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.699779 sharetop-1.1.3/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.1.3/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.1.3/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.712067 sharetop-1.1.3/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.1.3/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.750265 sharetop-1.1.3/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.1.3/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.1.3/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.1.3/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.1.3/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.1.3/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.769236 sharetop-1.1.3/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.1.3/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     2374 2023-05-02 15:19:23.000000 sharetop-1.1.3/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.1.3/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12300 2023-05-02 15:02:38.000000 sharetop-1.1.3/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.1.3/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.835891 sharetop-1.1.3/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.1.3/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.1.3/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.1.3/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.1.3/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.1.3/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.1.3/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.1.3/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.1.3/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.1.3/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.1.3/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.855749 sharetop-1.1.3/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.1.3/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.1.3/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.870445 sharetop-1.1.3/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      569 2023-05-02 15:39:30.000000 sharetop-1.1.3/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.1.3/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.1.3/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14302 2023-05-02 01:29:25.000000 sharetop-1.1.3/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.1.3/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.1.3/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.1.3/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.1.3/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.879830 sharetop-1.1.3/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.1.3/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.1.3/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     2873 2023-05-02 14:46:41.000000 sharetop-1.1.3/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.883932 sharetop-1.1.3/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.1.3/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     3558 2023-05-02 15:37:32.000000 sharetop-1.1.3/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     1948 2023-05-02 15:34:17.000000 sharetop-1.1.3/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.885935 sharetop-1.1.3/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.1.3/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.1.3/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.1.3/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0      126 2023-05-02 15:37:32.000000 sharetop-1.1.3/sharetop/test/test3.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:40:57.685355 sharetop-1.1.3/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    39033 2023-05-02 15:40:57.000000 sharetop-1.1.3/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1656 2023-05-02 15:40:57.000000 sharetop-1.1.3/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 15:40:57.000000 sharetop-1.1.3/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-02 15:40:57.000000 sharetop-1.1.3/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 15:40:57.000000 sharetop-1.1.3/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.0.3/LICENSE` & `sharetop-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/PKG-INFO` & `sharetop-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.3
+Version: 1.1.3
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-1.0.3/README.md` & `sharetop-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/setup.py` & `sharetop-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/application/base.py` & `sharetop-1.1.3/sharetop/application/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/bond/__init__.py` & `sharetop-1.1.3/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/bond/config.py` & `sharetop-1.1.3/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/bond/get_bond_info.py` & `sharetop-1.1.3/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/bond/get_bond_public_info.py` & `sharetop-1.1.3/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/cache.py` & `sharetop-1.1.3/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/common/config.py` & `sharetop-1.1.3/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/common/getter.py` & `sharetop-1.1.3/sharetop/core/common/getter.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
         **kwargs
 ) -> pd.DataFrame:
     """
         获取单只股票、债券 实时的基本数据
     """
     columns = list(EM_REAL_TIME_FIELDS.values())
     quote_id = get_quote_id(code)
+    print("quote_id:", quote_id)
     params = {
         "fields": EM_REAL_TIME_FIELDS_PARAMS
     }
     params = quote_id_process(params, quote_id)
     url = ''.join(real_time_url_list)
     json_response = requests_obj.get(
         url, params, user_agent=False
```

### Comparing `sharetop-1.0.3/sharetop/core/config.py` & `sharetop-1.1.3/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/__init__.py` & `sharetop-1.1.3/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/fund_list.py` & `sharetop-1.1.3/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/get_fund_base_info.py` & `sharetop-1.1.3/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/get_fund_history_data.py` & `sharetop-1.1.3/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-1.1.3/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-1.1.3/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/get_fund_real_time.py` & `sharetop-1.1.3/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/get_period_change_info.py` & `sharetop-1.1.3/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-1.1.3/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/futures/get_futures_info.py` & `sharetop-1.1.3/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/stock/bill_monitor.py` & `sharetop-1.1.3/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/stock/config.py` & `sharetop-1.1.3/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/stock/getter.py` & `sharetop-1.1.3/sharetop/core/stock/getter.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -209,8 +209,8 @@
         # 给空列表时 试用沪深A股行情
         if not fs_list:
             fs_list.append(FS_DICT['stock'])
     fs_str = ','.join(fs_list)
     df = get_market_realtime_by_fs(fs_str, **kwargs)
     df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
 
-    return df
+    return df
```

### Comparing `sharetop-1.0.3/sharetop/core/stock/quarterly_report.py` & `sharetop-1.1.3/sharetop/core/stock/quarterly_report.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/stock/rank_list.py` & `sharetop-1.1.3/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/core/utils.py` & `sharetop-1.1.3/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/crawl/base.py` & `sharetop-1.1.3/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.3/sharetop/crawl/settings.py` & `sharetop-1.1.3/sharetop/crawl/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,10 @@
 
 fund_basic_url = ['htt', 'ps:/', '/fun', 'dmo', 'bap', 'i.ea', 'stm', 'oney', '.co', 'm/Fu', 'ndMN', 'ewA', 'pi/F' ,'undM', 'NNB', 'asic', 'Info', 'rmat', 'ion']
 
 fund_industry_url = ['htt', 'ps:/', '/fun', 'dmo', 'bap', 'i.ea', 'stm', 'one', 'y.co', 'm/Fu', 'ndM', 'NewA', 'pi/', 'Fun', 'dMNS', 'ecto', 'rAl', 'loc', 'ation']
 
 bond_base_list_url = ['htt', 'p:/', '/dat', 'acen', 'ter', '-we', 'b.ea', 'stmo', 'ney', '.co', 'm/a', 'pi/d', 'ata', '/v', '1/g', 'et']
 
-bond_base_info_url = ['htt', 'p:/', '/dat', 'acen', 'ter-w', 'eb.e', 'astm', 'one', 'y.co', 'm/ap', 'i/da', 'ta/v', '1/g', 'et']
+bond_base_info_url = ['htt', 'p:/', '/dat', 'acen', 'ter-w', 'eb.e', 'astm', 'one', 'y.co', 'm/ap', 'i/da', 'ta/v', '1/g', 'et']
+
+stock_base_info_url = ['htt', 'p:/', '/em', 'we', 'b.se', 'curi', 'ties.', 'eas', 'tmon', 'ey.c', 'om/P', 'C_HS', 'F10/C', 'ompa', 'nySu', 'rve', 'y/Pa', 'geAj', 'ax']
```

### Comparing `sharetop-1.0.3/sharetop.egg-info/PKG-INFO` & `sharetop-1.1.3/sharetop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.3
+Version: 1.1.3
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-1.0.3/sharetop.egg-info/SOURCES.txt` & `sharetop-1.1.3/sharetop.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 sharetop/core/config.py
 sharetop/core/utils.py
 sharetop/core/bond/__init__.py
 sharetop/core/bond/config.py
 sharetop/core/bond/get_bond_info.py
 sharetop/core/bond/get_bond_public_info.py
 sharetop/core/common/__init__.py
+sharetop/core/common/common_base.py
 sharetop/core/common/config.py
 sharetop/core/common/getter.py
 sharetop/core/fund/__init__.py
 sharetop/core/fund/config.py
 sharetop/core/fund/fund_list.py
 sharetop/core/fund/get_fund_base_info.py
 sharetop/core/fund/get_fund_history_data.py
@@ -36,14 +37,18 @@
 sharetop/core/futures/get_futures_info.py
 sharetop/core/stock/__init__.py
 sharetop/core/stock/bill_monitor.py
 sharetop/core/stock/config.py
 sharetop/core/stock/getter.py
 sharetop/core/stock/quarterly_report.py
 sharetop/core/stock/rank_list.py
+sharetop/core/stock/stock_base_info.py
 sharetop/crawl/__init__.py
 sharetop/crawl/base.py
 sharetop/crawl/settings.py
 sharetop/parser/__init__.py
 sharetop/parser/base.py
+sharetop/parser/config.py
 sharetop/test/__init__.py
-sharetop/test/test1.py
+sharetop/test/test1.py
+sharetop/test/test2-akshare.py
+sharetop/test/test3.py
```

