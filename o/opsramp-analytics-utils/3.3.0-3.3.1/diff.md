# Comparing `tmp/opsramp-analytics-utils-3.3.0.tar.gz` & `tmp/opsramp-analytics-utils-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.3.0.tar", last modified: Wed Apr 12 10:54:01 2023, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.3.1.tar", last modified: Tue May  2 05:54:52 2023, max compression
```

## Comparing `opsramp-analytics-utils-3.3.0.tar` & `opsramp-analytics-utils-3.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-12 10:54:01.512471 opsramp-analytics-utils-3.3.0/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/LICENSE
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/MANIFEST.in
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-04-12 10:54:01.508471 opsramp-analytics-utils-3.3.0/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/README.md
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-12 10:54:01.344473 opsramp-analytics-utils-3.3.0/analytics_sdk/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/__init__.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-12 10:54:01.400472 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/main.js
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-12 10:54:01.484471 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/components.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/constants.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/oap_dash.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-12 10:54:01.488471 opsramp-analytics-utils-3.3.0/analytics_sdk/process/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/process/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     5809 2023-04-10 11:19:33.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/process/process.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/process/querybuilder.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-12 10:54:01.496471 opsramp-analytics-utils-3.3.0/analytics_sdk/renderer/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/renderer/__init__.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    30959 2023-03-14 08:52:14.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/renderer/excel.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/renderer/pdf.py
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    39299 2023-04-12 10:51:32.000000 opsramp-analytics-utils-3.3.0/analytics_sdk/utilities.py
-drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-04-12 10:54:01.508471 opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-04-12 10:54:01.000000 opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-04-12 10:54:01.000000 opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-04-12 10:54:01.000000 opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-12 10:54:01.000000 opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/requires.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-04-12 10:54:01.000000 opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/top_level.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-03 11:09:31.000000 opsramp-analytics-utils-3.3.0/requires-install.txt
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-04-12 10:54:01.512471 opsramp-analytics-utils-3.3.0/setup.cfg
--rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-04-12 10:52:16.000000 opsramp-analytics-utils-3.3.0/setup.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-02 05:54:52.321452 opsramp-analytics-utils-3.3.1/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1073 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/LICENSE
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      186 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/MANIFEST.in
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-05-02 05:54:52.321452 opsramp-analytics-utils-3.3.1/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      711 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/README.md
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-02 05:54:51.917441 opsramp-analytics-utils-3.3.1/analytics_sdk/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       30 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/__init__.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-02 05:54:52.065445 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      921 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/main.js
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  3321723 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)  2628164 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-02 05:54:52.265451 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      320 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    34172 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)   148200 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64440 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    29136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    64608 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      602 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      861 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1403 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     7536 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    11968 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    12136 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      733 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     4129 2022-07-11 05:34:48.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/components.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/constants.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    10055 2023-01-25 12:47:16.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/oap_dash.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-02 05:54:52.289451 opsramp-analytics-utils-3.3.1/analytics_sdk/process/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-07-27 14:35:38.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/process/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     5809 2023-04-10 11:19:33.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/process/process.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     3287 2022-09-28 12:26:39.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/process/querybuilder.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-02 05:54:52.309452 opsramp-analytics-utils-3.3.1/analytics_sdk/renderer/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        0 2022-06-27 12:21:56.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/renderer/__init__.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    30959 2023-03-14 08:52:14.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/renderer/excel.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     2887 2022-10-28 05:58:48.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/renderer/pdf.py
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)    40198 2023-05-02 05:53:28.000000 opsramp-analytics-utils-3.3.1/analytics_sdk/utilities.py
+drwxrwxr-x   0 rajumummidi  (1001) rajumummidi  (1001)        0 2023-05-02 05:54:52.317452 opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1361 2023-05-02 05:54:51.000000 opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)     1542 2023-05-02 05:54:51.000000 opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)        1 2023-05-02 05:54:51.000000 opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-05-02 05:54:51.000000 opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/requires.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       14 2023-05-02 05:54:51.000000 opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      108 2023-04-03 11:09:31.000000 opsramp-analytics-utils-3.3.1/requires-install.txt
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)       38 2023-05-02 05:54:52.321452 opsramp-analytics-utils-3.3.1/setup.cfg
+-rw-rw-r--   0 rajumummidi  (1001) rajumummidi  (1001)      941 2023-05-02 05:53:28.000000 opsramp-analytics-utils-3.3.1/setup.py
```

### Comparing `opsramp-analytics-utils-3.3.0/LICENSE` & `opsramp-analytics-utils-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/PKG-INFO` & `opsramp-analytics-utils-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.3.0
+Version: 3.3.1
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.3.0/README.md` & `opsramp-analytics-utils-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.3.1/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/components.py` & `opsramp-analytics-utils-3.3.1/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.3.1/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.3.1/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.3.1/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.3.1/analytics_sdk/renderer/excel.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.3.1/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.3.1/analytics_sdk/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,15 +594,14 @@
         logger.info('Status update response is %s', res)
     except Exception as e:
         logger.error("Exception raised due to : " + repr(e))
         traceback.print_exc()
     logger.info('finished init_mail method')
 
 
-
 def send_internal_failure_notification_mail(run_id, app_name, err_msg, partner_id, partner_name, client_id, client_name):
     logger.info('Entered into send_internal_failure_notification_mail method')
     try:
         url = BASE_API_URL + f'/reporting/api/v3/sendInternalFailureNotifications'
         data = {
             "runId": run_id,
             "appName": app_name,
@@ -622,14 +621,32 @@
     except Exception as e:
         raise e
         logger.error("Exception raised due to : " + repr(e))
         traceback.print_exc()
     logger.info('finished send_internal_failure_notification_mail method')
 
 
+def send_user_failure_notification(run_id, org_id):
+    logger.info('Entered into send_user_failure_notification method')
+    try:
+        url = BASE_API_URL + f'/reporting/api/v3/tenants/{org_id}/runs/{run_id}/failureNotification'
+        data = {}
+        t1 = int(time.time())
+        res = call_post_requests(url , data=json.dumps(data), verify=False)
+        t2 = int(time.time())
+        duration = t2-t1
+        if duration > API_TIME_STACKS:
+            logging.info('Send internal failure notification to customer mail response took %d (greater than %d) seconds', duration, API_TIME_STACKS)
+        logger.info('Send internal failure notification to customer mail response is %s', res)
+    except Exception as e:
+        raise e
+        logger.error("Exception raised due to : " + repr(e))
+        traceback.print_exc()
+    logger.info('finished send_user_failure_notification method')
+    
 
 def upload_excel(analysis_run, excel_file):
     timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
     s3_path = f'{analysis_run.analysis.app.slug}/excel/{timestamp}.xlsx'
 
     return upload_to_storage(excel_file, s3_path)
```

### Comparing `opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.3.0
+Version: 3.3.1
 Summary: OpsRamp Analytics SDK
 Home-page: https://github.com/opsramp/analytics-sdk
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.3.0/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.3.1/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.3.0/setup.py` & `opsramp-analytics-utils-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.3.0",
+    version="3.3.1",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     url="https://github.com/opsramp/analytics-sdk",
```

