# Comparing `tmp/hyta-0.0.4.tar.gz` & `tmp/hyta-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyta-0.0.4.tar", last modified: Sun Apr 30 19:23:32 2023, max compression
+gzip compressed data, was "hyta-0.1.4.tar", last modified: Tue May  2 18:58:31 2023, max compression
```

## Comparing `hyta-0.0.4.tar` & `hyta-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:23:32.658288 hyta-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 19:23:20.000000 hyta-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-30 19:23:32.658288 hyta-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-30 19:23:20.000000 hyta-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:23:32.658288 hyta-0.0.4/hyta/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/SMA.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/Stochastic_Oscillator.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/adx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/aroon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/atr.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/bollinger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/cci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/cmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/cmo.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/dema.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/dpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/dx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/hma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/ichimoku_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/kama.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/mfi.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/movingaverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/on_balance_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/ppo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/psar.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/roc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/rsi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/t3tillson.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/tma.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/tsi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/uo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/williams_r.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-30 19:23:20.000000 hyta-0.0.4/hyta/wma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:23:32.658288 hyta-0.0.4/hyta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-30 19:23:32.000000 hyta-0.0.4/hyta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-30 19:23:32.000000 hyta-0.0.4/hyta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 19:23:32.000000 hyta-0.0.4/hyta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 19:23:32.000000 hyta-0.0.4/hyta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 19:23:32.000000 hyta-0.0.4/hyta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 19:23:32.658288 hyta-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-30 19:23:20.000000 hyta-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:58:31.498340 hyta-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 18:58:13.000000 hyta-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-02 18:58:31.498340 hyta-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-02 18:58:13.000000 hyta-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:58:31.498340 hyta-0.1.4/hyta/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/Stochastic_Oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/adx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/aroon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/atr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/bollinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/cci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/cmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/cmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/dema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/dpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/dx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/hma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/ichimoku_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/kama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/mfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/movingaverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/on_balance_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/psar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/roc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/t3tillson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/tma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/tsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/uo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/williams_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 18:58:13.000000 hyta-0.1.4/hyta/wma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:58:31.498340 hyta-0.1.4/hyta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-02 18:58:31.000000 hyta-0.1.4/hyta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-02 18:58:31.000000 hyta-0.1.4/hyta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:58:31.000000 hyta-0.1.4/hyta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 18:58:31.000000 hyta-0.1.4/hyta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 18:58:31.000000 hyta-0.1.4/hyta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:58:31.498340 hyta-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-02 18:58:13.000000 hyta-0.1.4/setup.py
```

### Comparing `hyta-0.0.4/LICENSE` & `hyta-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/PKG-INFO` & `hyta-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyta
-Version: 0.0.4
+Version: 0.1.4
 Summary: Indicators for Hypance Project
 Home-page: https://github.com/Hypance/HypanceDataAnalysis
 Author: Toygar Aksoy
 Author-email: toygar.aksoy@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hyta Version: 0.0.4 Summary: Indicators for Hypance
+Metadata-Version: 2.1 Name: hyta Version: 0.1.4 Summary: Indicators for Hypance
 Project Home-page: https://github.com/Hypance/HypanceDataAnalysis Author:
 Toygar Aksoy Author-email: toygar.aksoy@gmail.com License: MIT Description-
 Content-Type: text/markdown License-File: LICENSE
         [https://avatars.githubusercontent.com/u/113800422?s=200&v=4"]
 ----------------- # HyTa - Technical Analysis Library ![](https://
 img.shields.io/badge/python-3.8-blue.svg) ![](https://img.shields.io/badge/
 python-3.9-blue.svg) ![](https://img.shields.io/badge/python-3.10-blue.svg) ![]
```

### Comparing `hyta-0.0.4/README.md` & `hyta-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/Stochastic_Oscillator.py` & `hyta-0.1.4/hyta/Stochastic_Oscillator.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/adx.py` & `hyta-0.1.4/hyta/adx.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/aroon.py` & `hyta-0.1.4/hyta/aroon.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/atr.py` & `hyta-0.1.4/hyta/atr.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/bollinger.py` & `hyta-0.1.4/hyta/bollinger.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/cci.py` & `hyta-0.1.4/hyta/cci.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/cmf.py` & `hyta-0.1.4/hyta/cmf.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/cmo.py` & `hyta-0.1.4/hyta/cmo.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/dema.py` & `hyta-0.1.4/hyta/dema.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/dpo.py` & `hyta-0.1.4/hyta/dpo.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/dx.py` & `hyta-0.1.4/hyta/dx.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/ema.py` & `hyta-0.1.4/hyta/ema.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/hma.py` & `hyta-0.1.4/hyta/hma.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/ichimoku_cloud.py` & `hyta-0.1.4/hyta/ichimoku_cloud.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/kama.py` & `hyta-0.1.4/hyta/kama.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/macd.py` & `hyta-0.1.4/hyta/macd.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/mfi.py` & `hyta-0.1.4/hyta/mfi.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/momentum.py` & `hyta-0.1.4/hyta/momentum.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/movingaverage.py` & `hyta-0.1.4/hyta/movingaverage.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/on_balance_volume.py` & `hyta-0.1.4/hyta/on_balance_volume.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/ppo.py` & `hyta-0.1.4/hyta/ppo.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/psar.py` & `hyta-0.1.4/hyta/psar.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/roc.py` & `hyta-0.1.4/hyta/roc.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/rsi.py` & `hyta-0.1.4/hyta/rsi.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/t3tillson.py` & `hyta-0.1.4/hyta/t3tillson.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/tma.py` & `hyta-0.1.4/hyta/tma.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/tsi.py` & `hyta-0.1.4/hyta/tsi.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/uo.py` & `hyta-0.1.4/hyta/uo.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/williams_r.py` & `hyta-0.1.4/hyta/williams_r.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta/wma.py` & `hyta-0.1.4/hyta/wma.py`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/hyta.egg-info/PKG-INFO` & `hyta-0.1.4/hyta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyta
-Version: 0.0.4
+Version: 0.1.4
 Summary: Indicators for Hypance Project
 Home-page: https://github.com/Hypance/HypanceDataAnalysis
 Author: Toygar Aksoy
 Author-email: toygar.aksoy@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hyta Version: 0.0.4 Summary: Indicators for Hypance
+Metadata-Version: 2.1 Name: hyta Version: 0.1.4 Summary: Indicators for Hypance
 Project Home-page: https://github.com/Hypance/HypanceDataAnalysis Author:
 Toygar Aksoy Author-email: toygar.aksoy@gmail.com License: MIT Description-
 Content-Type: text/markdown License-File: LICENSE
         [https://avatars.githubusercontent.com/u/113800422?s=200&v=4"]
 ----------------- # HyTa - Technical Analysis Library ![](https://
 img.shields.io/badge/python-3.8-blue.svg) ![](https://img.shields.io/badge/
 python-3.9-blue.svg) ![](https://img.shields.io/badge/python-3.10-blue.svg) ![]
```

### Comparing `hyta-0.0.4/hyta.egg-info/SOURCES.txt` & `hyta-0.1.4/hyta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyta-0.0.4/setup.py` & `hyta-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='hyta',
-    version='0.0.4',
+    version='0.1.4',
     author='Toygar Aksoy',
     author_email='toygar.aksoy@gmail.com',
     description='Indicators for Hypance Project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Hypance/HypanceDataAnalysis',
     # project_urls = {
```

