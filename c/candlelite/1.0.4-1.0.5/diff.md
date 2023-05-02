# Comparing `tmp/candlelite-1.0.4.tar.gz` & `tmp/candlelite-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/candlelite-1.0.4.tar", last modified: Mon Mar  6 06:27:55 2023, max compression
+gzip compressed data, was "dist/candlelite-1.0.5.tar", last modified: Tue May  2 04:21:39 2023, max compression
```

## Comparing `candlelite-1.0.4.tar` & `candlelite-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.149849 candlelite-1.0.4/
--rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-03-06 06:27:55.149557 candlelite-1.0.4/PKG-INFO
--rw-r--r--   0 kzlknight   (501) staff       (20)       25 2023-02-21 10:35:06.000000 candlelite-1.0.4/README.md
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.135700 candlelite-1.0.4/candlelite/
--rw-r--r--   0 kzlknight   (501) staff       (20)      242 2023-03-06 06:27:18.000000 candlelite-1.0.4/candlelite/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.139684 candlelite-1.0.4/candlelite/calculate/
--rw-r--r--   0 kzlknight   (501) staff       (20)      204 2023-01-25 20:14:09.000000 candlelite-1.0.4/candlelite/calculate/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1123 2023-01-25 19:21:42.000000 candlelite-1.0.4/candlelite/calculate/bar.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1059 2023-01-25 19:28:05.000000 candlelite-1.0.4/candlelite/calculate/interval.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     5141 2023-01-25 19:36:00.000000 candlelite-1.0.4/candlelite/calculate/technical.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     6651 2023-01-25 20:11:14.000000 candlelite-1.0.4/candlelite/calculate/transform.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     5104 2023-01-26 21:55:48.000000 candlelite-1.0.4/candlelite/calculate/valid.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.139916 candlelite-1.0.4/candlelite/cmdline/
--rw-r--r--   0 kzlknight   (501) staff       (20)      975 2023-01-26 07:20:12.000000 candlelite-1.0.4/candlelite/cmdline/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.146849 candlelite-1.0.4/candlelite/crypto/
--rw-r--r--   0 kzlknight   (501) staff       (20)      101 2023-02-21 10:35:06.000000 candlelite-1.0.4/candlelite/crypto/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     9027 2023-02-21 10:35:06.000000 candlelite-1.0.4/candlelite/crypto/_base.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      885 2023-01-29 21:17:12.000000 candlelite-1.0.4/candlelite/crypto/binace_lite.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      818 2023-01-25 21:49:55.000000 candlelite-1.0.4/candlelite/crypto/okx_lite.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.147971 candlelite-1.0.4/candlelite/exception/
--rw-r--r--   0 kzlknight   (501) staff       (20)      131 2023-01-25 19:19:56.000000 candlelite-1.0.4/candlelite/exception/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      235 2023-01-25 19:24:42.000000 candlelite-1.0.4/candlelite/exception/_base.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1182 2023-01-13 21:53:32.000000 candlelite-1.0.4/candlelite/exception/candle.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      202 2023-01-25 19:25:08.000000 candlelite-1.0.4/candlelite/exception/execute.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      813 2023-01-25 20:07:05.000000 candlelite-1.0.4/candlelite/exception/param.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.148996 candlelite-1.0.4/candlelite/io/
--rw-r--r--   0 kzlknight   (501) staff       (20)       93 2023-02-21 10:35:06.000000 candlelite-1.0.4/candlelite/io/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)    10042 2023-03-06 06:05:18.000000 candlelite-1.0.4/candlelite/io/load.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     5385 2023-02-21 10:35:06.000000 candlelite-1.0.4/candlelite/io/path.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     7368 2023-03-06 06:06:56.000000 candlelite-1.0.4/candlelite/io/save.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.149213 candlelite-1.0.4/candlelite/settings/
--rw-r--r--   0 kzlknight   (501) staff       (20)     4485 2023-01-29 21:19:01.000000 candlelite-1.0.4/candlelite/settings/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-06 06:27:55.138147 candlelite-1.0.4/candlelite.egg-info/
--rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-03-06 06:27:54.000000 candlelite-1.0.4/candlelite.egg-info/PKG-INFO
--rw-r--r--   0 kzlknight   (501) staff       (20)      870 2023-03-06 06:27:55.000000 candlelite-1.0.4/candlelite.egg-info/SOURCES.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-03-06 06:27:54.000000 candlelite-1.0.4/candlelite.egg-info/dependency_links.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       54 2023-03-06 06:27:54.000000 candlelite-1.0.4/candlelite.egg-info/entry_points.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       18 2023-03-06 06:27:54.000000 candlelite-1.0.4/candlelite.egg-info/requires.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       11 2023-03-06 06:27:54.000000 candlelite-1.0.4/candlelite.egg-info/top_level.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-03-06 06:27:55.149996 candlelite-1.0.4/setup.cfg
--rw-r--r--   0 kzlknight   (501) staff       (20)     2835 2023-03-06 06:27:22.000000 candlelite-1.0.4/setup.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.455657 candlelite-1.0.5/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-05-02 04:21:39.455077 candlelite-1.0.5/PKG-INFO
+-rw-r--r--   0 kzlknight   (501) staff       (20)       25 2023-02-21 10:35:06.000000 candlelite-1.0.5/README.md
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.433872 candlelite-1.0.5/candlelite/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      242 2023-05-02 04:19:38.000000 candlelite-1.0.5/candlelite/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.440899 candlelite-1.0.5/candlelite/calculate/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      204 2023-01-25 20:14:09.000000 candlelite-1.0.5/candlelite/calculate/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1123 2023-01-25 19:21:42.000000 candlelite-1.0.5/candlelite/calculate/bar.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1059 2023-01-25 19:28:05.000000 candlelite-1.0.5/candlelite/calculate/interval.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     5141 2023-01-25 19:36:00.000000 candlelite-1.0.5/candlelite/calculate/technical.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     6651 2023-01-25 20:11:14.000000 candlelite-1.0.5/candlelite/calculate/transform.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     5104 2023-01-26 21:55:48.000000 candlelite-1.0.5/candlelite/calculate/valid.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.442160 candlelite-1.0.5/candlelite/cmdline/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      975 2023-01-26 07:20:12.000000 candlelite-1.0.5/candlelite/cmdline/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.445618 candlelite-1.0.5/candlelite/crypto/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      101 2023-02-21 10:35:06.000000 candlelite-1.0.5/candlelite/crypto/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    11149 2023-05-02 04:19:38.000000 candlelite-1.0.5/candlelite/crypto/_base.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      885 2023-01-29 21:17:12.000000 candlelite-1.0.5/candlelite/crypto/binace_lite.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      818 2023-01-25 21:49:55.000000 candlelite-1.0.5/candlelite/crypto/okx_lite.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.449875 candlelite-1.0.5/candlelite/exception/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      131 2023-01-25 19:19:56.000000 candlelite-1.0.5/candlelite/exception/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      235 2023-01-25 19:24:42.000000 candlelite-1.0.5/candlelite/exception/_base.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1294 2023-05-02 04:09:34.000000 candlelite-1.0.5/candlelite/exception/candle.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      202 2023-01-25 19:25:08.000000 candlelite-1.0.5/candlelite/exception/execute.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      813 2023-01-25 20:07:05.000000 candlelite-1.0.5/candlelite/exception/param.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.453843 candlelite-1.0.5/candlelite/io/
+-rw-r--r--   0 kzlknight   (501) staff       (20)       93 2023-02-21 10:35:06.000000 candlelite-1.0.5/candlelite/io/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    11492 2023-05-02 04:14:58.000000 candlelite-1.0.5/candlelite/io/load.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     8693 2023-05-01 14:46:48.000000 candlelite-1.0.5/candlelite/io/path.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     7368 2023-03-06 06:06:56.000000 candlelite-1.0.5/candlelite/io/save.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.454360 candlelite-1.0.5/candlelite/settings/
+-rw-r--r--   0 kzlknight   (501) staff       (20)     4485 2023-01-29 21:19:01.000000 candlelite-1.0.5/candlelite/settings/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-05-02 04:21:39.436057 candlelite-1.0.5/candlelite.egg-info/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-05-02 04:21:39.000000 candlelite-1.0.5/candlelite.egg-info/PKG-INFO
+-rw-r--r--   0 kzlknight   (501) staff       (20)      870 2023-05-02 04:21:39.000000 candlelite-1.0.5/candlelite.egg-info/SOURCES.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-05-02 04:21:39.000000 candlelite-1.0.5/candlelite.egg-info/dependency_links.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       54 2023-05-02 04:21:39.000000 candlelite-1.0.5/candlelite.egg-info/entry_points.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       18 2023-05-02 04:21:39.000000 candlelite-1.0.5/candlelite.egg-info/requires.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       11 2023-05-02 04:21:39.000000 candlelite-1.0.5/candlelite.egg-info/top_level.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-05-02 04:21:39.455802 candlelite-1.0.5/setup.cfg
+-rw-r--r--   0 kzlknight   (501) staff       (20)     2835 2023-05-02 04:19:52.000000 candlelite-1.0.5/setup.py
```

### Comparing `candlelite-1.0.4/PKG-INFO` & `candlelite-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlelite
-Version: 1.0.4
+Version: 1.0.5
 Summary: History candle database and utils
 Home-page: https://github.com/pyted/candlelite
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `candlelite-1.0.4/candlelite/calculate/bar.py` & `candlelite-1.0.5/candlelite/calculate/bar.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/calculate/interval.py` & `candlelite-1.0.5/candlelite/calculate/interval.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/calculate/technical.py` & `candlelite-1.0.5/candlelite/calculate/technical.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/calculate/transform.py` & `candlelite-1.0.5/candlelite/calculate/transform.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/calculate/valid.py` & `candlelite-1.0.5/candlelite/calculate/valid.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/cmdline/__init__.py` & `candlelite-1.0.5/candlelite/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/crypto/_base.py` & `candlelite-1.0.5/candlelite/crypto/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,80 @@
 
 class IO():
     CANDLE_DATE_BASE_DIR: str
     CANDLE_FILE_BASE_DIR: str
     TIMEZONE: str
     BAR: str
 
+    # 获取candle具备数据的日期序列
+    def get_candle_dates(
+            self,
+            instType: str,
+            symbol: str,
+            base_dir: str = None,
+            timezone: str = None,
+            bar: Literal['1m', '3m', '5m', '15m', '1H', '2H', '4H'] = None,
+    ):
+        if base_dir == None:
+            base_dir = self.CANDLE_DATE_BASE_DIR
+        if timezone == None:
+            timezone = self.TIMEZONE
+        if bar == None:
+            bar = self.BAR
+        return path.get_candle_dates(**to_local(locals()))
+
+    # 获取全部的产品名称
+    def get_symbols_all(
+            self,
+            instType: str,
+            base_dir: str = None,
+            timezone: str = None,
+            bar: Literal['1m', '3m', '5m', '15m', '1H', '2H', '4H'] = None,
+    ):
+        if base_dir == None:
+            base_dir = self.CANDLE_DATE_BASE_DIR
+        if timezone == None:
+            timezone = self.TIMEZONE
+        if bar == None:
+            bar = self.BAR
+        return path.get_symbols_all(**to_local(locals()))
+
+    # 加载一个产品已有的全部K线
+    def load_candle_all(
+            self,
+            instType: str,
+            symbol: str,
+            base_dir: str = None,
+            timezone: str = None,
+            bar: Literal['1m', '3m', '5m', '15m', '1H', '2H', '4H'] = None,
+    ):
+        if base_dir == None:
+            base_dir = self.CANDLE_DATE_BASE_DIR
+        if timezone == None:
+            timezone = self.TIMEZONE
+        if bar == None:
+            bar = self.BAR
+        return load.load_candle_all(**to_local(locals()))
+
+    # 加载全部产品已有的K线
+    def load_candle_map_all(
+            self,
+            instType: str,
+            base_dir: str = None,
+            timezone: str = None,
+            bar: Literal['1m', '3m', '5m', '15m', '1H', '2H', '4H'] = None,
+    ):
+        if base_dir == None:
+            base_dir = self.CANDLE_DATE_BASE_DIR
+        if timezone == None:
+            timezone = self.TIMEZONE
+        if bar == None:
+            bar = self.BAR
+        return load.load_candle_map_all(**to_local(locals()))
+
     # 读取从start~end日期的历史K线数据
     def load_candle_by_date(
             self,
             instType: str,
             symbol: str,
             start: Union[int, float, str, datetime.date],
             end: Union[int, float, str, datetime.date],
```

### Comparing `candlelite-1.0.4/candlelite/crypto/binace_lite.py` & `candlelite-1.0.5/candlelite/crypto/binace_lite.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/crypto/okx_lite.py` & `candlelite-1.0.5/candlelite/crypto/okx_lite.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/exception/candle.py` & `candlelite-1.0.5/candlelite/exception/candle.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,7 +46,12 @@
             symbol: str,
             msg: str,
     ):
         self.error_msg = 'symbol={symbol:<10} msg={msg}'.format(
             symbol=str(symbol),
             msg=str(msg)
         )
+
+
+class CandleDatesNonError(AbstractEXP):
+    def __init__(self, error_msg):
+        self.error_msg = error_msg
```

### Comparing `candlelite-1.0.4/candlelite/exception/param.py` & `candlelite-1.0.5/candlelite/exception/param.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/io/load.py` & `candlelite-1.0.5/candlelite/io/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         if not valid_start_result['code']:
             raise exception.CandleStartError(
                 symbol=symbol,
                 msg=valid_start_result['msg'],
             )
     # 验证end
     if valid_end:
-        end_ts = _date.tomorrow(date=date_range[-1],timezone=timezone).timestamp() * 1000 - _interval.get_interval(bar)
+        end_ts = _date.tomorrow(date=date_range[-1], timezone=timezone).timestamp() * 1000 - _interval.get_interval(bar)
         # end_ts = _date.to_ts(date=date_range[-1], timezone=timezone) + 1000 * 60 * 60 * 24 - _interval.get_interval(bar)
         valid_end_result = _valid.valid_end(candle=candle, end=end_ts, timezone=timezone)
         if not valid_end_result['code']:
             raise exception.CandleEndError(
                 symbol=symbol,
                 msg=valid_end_result['msg'],
             )
@@ -121,15 +121,15 @@
         symbols: list,
         start: Union[int, float, str, datetime.date],
         end: Union[int, float, str, datetime.date],
         base_dir: str,
         timezone: str = None,
         bar: Literal['1m', '3m', '5m', '15m', '1H', '2H', '4H'] = '1m',
         endswith: str = '',
-        contains:str = '',
+        contains: str = '',
         p_num: int = 4,
         valid_interval: bool = True,
         valid_start: bool = True,
         valid_end: bool = True,
 ) -> dict:
     '''
     :param instType: 产品类型
@@ -223,14 +223,69 @@
     candle_map_sorted = {}
     symbols = sorted([symbol for symbol in candle_map.keys()])
     for symbol in symbols:
         candle_map_sorted[symbol] = candle_map[symbol]
     return candle_map_sorted
 
 
+# 加载一个产品已有的全部K线
+def load_candle_all(
+        instType: str,
+        symbol: str,
+        base_dir: str,
+        timezone: str = None,
+        bar: Literal['1m', '3m', '5m', '15m', '1H', '2H', '4H'] = '1m',
+):
+    candle_dates_result = _path.get_candle_dates(
+        instType=instType,
+        symbol=symbol,
+        base_dir=base_dir,
+        timezone=timezone,
+        bar=bar,
+    )
+    if candle_dates_result['code'] != True:
+        raise exception.CandleDatesNonError(str(candle_dates_result))
+    candle = load_candle_by_date(
+        instType=instType,
+        start=candle_dates_result['data']['start'],
+        end=candle_dates_result['data']['end'],
+        symbol=symbol,
+        base_dir=base_dir,
+        timezone=timezone,
+        bar=bar,
+    )
+    return candle
+
+
+# 加载全部产品已有的K线
+def load_candle_map_all(
+        instType: str,
+        base_dir: str,
+        timezone: str = None,
+        bar: Literal['1m', '3m', '5m', '15m', '1H', '2H', '4H'] = '1m',
+):
+    symbols = _path.get_symbols_all(
+        instType=instType,
+        base_dir=base_dir,
+        timezone=timezone,
+        bar=bar,
+    )
+    candle_map = {}
+    for symbol in symbols:
+        candle = load_candle_all(
+            instType=instType,
+            symbol=symbol,
+            base_dir=base_dir,
+            timezone=timezone,
+            bar=bar,
+        )
+        candle_map[symbol] = candle
+    return candle_map
+
+
 # 通过文件地址读取Candle
 def load_candle_by_file(
         instType: str,
         symbol: str,
         path: str = None,
         base_dir: str = '',
         timezone: str = None,
```

### Comparing `candlelite-1.0.4/candlelite/io/save.py` & `candlelite-1.0.5/candlelite/io/save.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite/settings/__init__.py` & `candlelite-1.0.5/candlelite/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/candlelite.egg-info/PKG-INFO` & `candlelite-1.0.5/candlelite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlelite
-Version: 1.0.4
+Version: 1.0.5
 Summary: History candle database and utils
 Home-page: https://github.com/pyted/candlelite
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `candlelite-1.0.4/candlelite.egg-info/SOURCES.txt` & `candlelite-1.0.5/candlelite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.4/setup.py` & `candlelite-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'candlelite'
 DESCRIPTION = 'History candle database and utils'
 URL = "https://github.com/pyted/candlelite"
 EMAIL = 'pyted@outlook.com'
 AUTHOR = 'pyted'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 
 REQUIRED = [
     'numpy',
     'pandas',
     'paux',
 ]
```

