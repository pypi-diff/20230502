# Comparing `tmp/dia-adfpro-0.0.2.tar.gz` & `tmp/dia-adfpro-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dia-adfpro-0.0.2.tar", last modified: Tue May  2 13:28:12 2023, max compression
+gzip compressed data, was "dia-adfpro-1.6.2.tar", last modified: Tue May  2 14:18:23 2023, max compression
```

## Comparing `dia-adfpro-0.0.2.tar` & `dia-adfpro-1.6.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:28:12.731713 dia-adfpro-0.0.2/
--rw-rw-rw-   0        0        0     1089 2021-09-24 08:00:55.000000 dia-adfpro-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 10:00:29.000000 dia-adfpro-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1046 2023-05-02 13:28:12.731713 dia-adfpro-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 13:28:12.684822 dia-adfpro-0.0.2/dia_adfpro.egg-info/
--rw-rw-rw-   0        0        0     1046 2023-05-02 13:28:12.000000 dia-adfpro-0.0.2/dia_adfpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-05-02 13:28:12.000000 dia-adfpro-0.0.2/dia_adfpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:28:12.000000 dia-adfpro-0.0.2/dia_adfpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 13:28:12.000000 dia-adfpro-0.0.2/dia_adfpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 13:28:12.000000 dia-adfpro-0.0.2/dia_adfpro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 13:28:12.684822 dia-adfpro-0.0.2/diaadfpro/
--rw-rw-rw-   0        0        0      295 2023-05-02 13:27:58.000000 dia-adfpro-0.0.2/diaadfpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:28:12.700449 dia-adfpro-0.0.2/diaadfpro/adfpro/
--rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/__init__.py
--rw-rw-rw-   0        0        0    10059 2023-04-28 12:49:53.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/classify.py
--rw-rw-rw-   0        0        0    13958 2023-04-05 13:22:26.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/configuration.py
--rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/constants.py
--rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/explain.py
--rw-rw-rw-   0        0        0    27722 2023-03-27 10:16:17.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/feature_extract.py
--rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/feature_extractors.py
--rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/golden.py
--rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/model.py
--rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/offload.py
--rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/train.py
--rw-rw-rw-   0        0        0    54884 2023-04-28 12:40:42.000000 dia-adfpro-0.0.2/diaadfpro/adfpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:28:12.731713 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/
--rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/__init__.py
--rw-rw-rw-   0        0        0     4014 2023-04-28 12:40:59.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/constants.py
--rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_anomaly_plots.py
--rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_app.py
--rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_components.py
--rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_env_cfg.py
--rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
--rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_ohlc_plots.py
--rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_retrain.py
--rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_summary_table.py
--rw-rw-rw-   0        0        0      115 2023-05-02 13:28:12.731713 dia-adfpro-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1239 2023-05-02 10:01:23.000000 dia-adfpro-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:18:23.793269 dia-adfpro-1.6.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-02 13:38:04.000000 dia-adfpro-1.6.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 13:38:04.000000 dia-adfpro-1.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1046 2023-05-02 14:18:23.793269 dia-adfpro-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-1.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 14:18:23.510394 dia-adfpro-1.6.2/dia_adfpro.egg-info/
+-rw-rw-rw-   0        0        0     1046 2023-05-02 14:18:23.000000 dia-adfpro-1.6.2/dia_adfpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-05-02 14:18:23.000000 dia-adfpro-1.6.2/dia_adfpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 14:18:23.000000 dia-adfpro-1.6.2/dia_adfpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 14:18:23.000000 dia-adfpro-1.6.2/dia_adfpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-02 14:18:23.000000 dia-adfpro-1.6.2/dia_adfpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 14:18:23.510394 dia-adfpro-1.6.2/diaadfpro/
+-rw-rw-rw-   0        0        0      295 2023-05-02 13:51:03.000000 dia-adfpro-1.6.2/diaadfpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:18:23.668268 dia-adfpro-1.6.2/diaadfpro/adfpro/
+-rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/__init__.py
+-rw-rw-rw-   0        0        0    10059 2023-05-02 13:38:04.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/classify.py
+-rw-rw-rw-   0        0        0    13958 2023-04-05 13:22:26.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/configuration.py
+-rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/constants.py
+-rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/explain.py
+-rw-rw-rw-   0        0        0    27722 2023-03-27 10:16:17.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/feature_extract.py
+-rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/feature_extractors.py
+-rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/golden.py
+-rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/model.py
+-rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/offload.py
+-rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/train.py
+-rw-rw-rw-   0        0        0    54884 2023-04-28 12:40:42.000000 dia-adfpro-1.6.2/diaadfpro/adfpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:18:23.793269 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/
+-rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/__init__.py
+-rw-rw-rw-   0        0        0     4014 2023-05-02 13:51:03.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/constants.py
+-rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_anomaly_plots.py
+-rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_app.py
+-rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_components.py
+-rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_env_cfg.py
+-rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
+-rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_ohlc_plots.py
+-rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_retrain.py
+-rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_summary_table.py
+-rw-rw-rw-   0        0        0      115 2023-05-02 14:18:23.793269 dia-adfpro-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1239 2023-05-02 13:38:04.000000 dia-adfpro-1.6.2/setup.py
```

### Comparing `dia-adfpro-0.0.2/LICENSE.txt` & `dia-adfpro-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/PKG-INFO` & `dia-adfpro-1.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 0.0.2
+Version: 1.6.2
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dia-adfpro-0.0.2/README.md` & `dia-adfpro-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/dia_adfpro.egg-info/PKG-INFO` & `dia-adfpro-1.6.2/dia_adfpro.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 0.0.2
+Version: 1.6.2
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dia-adfpro-0.0.2/dia_adfpro.egg-info/SOURCES.txt` & `dia-adfpro-1.6.2/dia_adfpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/classify.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/classify.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/configuration.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/configuration.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/constants.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/constants.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/explain.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/explain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/feature_extract.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/feature_extract.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/feature_extractors.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/golden.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/golden.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/model.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/model.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/offload.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/offload.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/train.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/train.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro/utils.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro/utils.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/constants.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             Manjunath C Bagewadi <bagewadi_manjunath_c@lilly.com>, 
             Henson Tauro <tauro_henson@lilly.com> 
             (MQ IDS - Data Integration and Analytics)
 License:    MIT
 """
 
 class ADFPCUI:
-    REPORT_VERSION = "1.6.1 (2023-04-28)"
+    REPORT_VERSION = "1.6.2 (2023-05-02)"
 
     #use for html id's
     ID_REFRESH = "btn-refresh"                                       #Refresh tab1
     ID_LATESTFETCH = "lbl-latestfetch"                               # latestfetch tab1
     ID_SUMMARY_TBL_CONTAINER = "div-summary-tbl-container"
     
     RETRAIN_YML = "/mnt/py/cfg.jobs/temp_retrain_job.yml"
```

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_anomaly_plots.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_anomaly_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_app.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_app.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_components.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_components.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_env_cfg.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_env_cfg.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_env_cfg.sample.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_env_cfg.sample.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_ohlc_plots.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_ohlc_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_retrain.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_retrain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/diaadfpro/adfpro_ui/ui_summary_table.py` & `dia-adfpro-1.6.2/diaadfpro/adfpro_ui/ui_summary_table.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-0.0.2/setup.py` & `dia-adfpro-1.6.2/setup.py`

 * *Files identical despite different names*

