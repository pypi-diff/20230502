# Comparing `tmp/pyhtcc-0.1.8.tar.gz` & `tmp/pyhtcc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtcc-0.1.8.tar", last modified: Sat Feb 12 18:25:42 2022, max compression
+gzip compressed data, was "pyhtcc-0.1.9.tar", last modified: Sat Jul 30 22:00:53 2022, max compression
```

## Comparing `pyhtcc-0.1.8.tar` & `pyhtcc-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-02-12 18:25:42.241139 pyhtcc-0.1.8/
--rw-rw-rw-   0        0        0     2400 2022-02-12 18:25:42.240138 pyhtcc-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2022-02-12 18:20:05.000000 pyhtcc-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-02-12 18:25:42.220139 pyhtcc-0.1.8/pyhtcc/
--rw-rw-rw-   0        0        0       44 2022-02-12 18:25:16.000000 pyhtcc-0.1.8/pyhtcc/__init__.py
--rw-rw-rw-   0        0        0     2467 2022-02-12 18:20:05.000000 pyhtcc-0.1.8/pyhtcc/__main__.py
--rw-rw-rw-   0        0        0    19936 2022-02-12 18:20:05.000000 pyhtcc-0.1.8/pyhtcc/pyhtcc.py
-drwxrwxrwx   0        0        0        0 2022-02-12 18:25:42.239139 pyhtcc-0.1.8/pyhtcc.egg-info/
--rw-rw-rw-   0        0        0     2400 2022-02-12 18:25:42.000000 pyhtcc-0.1.8/pyhtcc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2022-02-12 18:25:42.000000 pyhtcc-0.1.8/pyhtcc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-12 18:25:42.000000 pyhtcc-0.1.8/pyhtcc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-02-12 18:25:42.000000 pyhtcc-0.1.8/pyhtcc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2022-02-12 18:25:42.000000 pyhtcc-0.1.8/pyhtcc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-02-12 18:25:42.000000 pyhtcc-0.1.8/pyhtcc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-12 18:25:42.241139 pyhtcc-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1379 2022-02-12 18:20:05.000000 pyhtcc-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-30 22:00:53.629228 pyhtcc-0.1.9/
+-rw-rw-rw-   0        0        0     2359 2022-07-30 22:00:53.628229 pyhtcc-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1748 2022-07-30 21:54:39.000000 pyhtcc-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-30 22:00:53.613228 pyhtcc-0.1.9/pyhtcc/
+-rw-rw-rw-   0        0        0       44 2022-07-30 21:59:42.000000 pyhtcc-0.1.9/pyhtcc/__init__.py
+-rw-rw-rw-   0        0        0     2467 2022-07-30 21:54:39.000000 pyhtcc-0.1.9/pyhtcc/__main__.py
+-rw-rw-rw-   0        0        0    19966 2022-07-30 21:56:23.000000 pyhtcc-0.1.9/pyhtcc/pyhtcc.py
+drwxrwxrwx   0        0        0        0 2022-07-30 22:00:53.627227 pyhtcc-0.1.9/pyhtcc.egg-info/
+-rw-rw-rw-   0        0        0     2359 2022-07-30 22:00:53.000000 pyhtcc-0.1.9/pyhtcc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2022-07-30 22:00:53.000000 pyhtcc-0.1.9/pyhtcc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-30 22:00:53.000000 pyhtcc-0.1.9/pyhtcc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2022-07-30 22:00:53.000000 pyhtcc-0.1.9/pyhtcc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2022-07-30 22:00:53.000000 pyhtcc-0.1.9/pyhtcc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-07-30 22:00:53.000000 pyhtcc-0.1.9/pyhtcc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-07-30 22:00:53.629228 pyhtcc-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2022-07-30 21:54:39.000000 pyhtcc-0.1.9/setup.py
```

### Comparing `pyhtcc-0.1.8/PKG-INFO` & `pyhtcc-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyhtcc
-Version: 0.1.8
-Summary: UNKNOWN
+Version: 0.1.9
 Home-page: http://github.com/csm10495/pyhtcc
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
@@ -65,9 +63,7 @@
   -C COOL, --cool COOL  Set a target cooling temperature
 
 ```
 [CLI_OUTPUT_MARKER]::
 
 ## License
 MIT License
-
-
```

### Comparing `pyhtcc-0.1.8/README.md` & `pyhtcc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyhtcc-0.1.8/pyhtcc/__main__.py` & `pyhtcc-0.1.9/pyhtcc/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhtcc-0.1.8/pyhtcc/pyhtcc.py` & `pyhtcc-0.1.9/pyhtcc/pyhtcc.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,21 +382,21 @@
         Private API to find the outdoor information on one of the logged in pages
         '''
         result = self.session.get(f'https://mytotalconnectcomfort.com/portal/Device/Control/{device_id}?page=1')
         result.raise_for_status()
 
         text_data = result.text
         try:
-            outdoor_temp = int(text_data.split('Control.Model.Property.outdoorTemp,')[1].split(')', 1)[0])
+            outdoor_temp = int(float(text_data.split('Control.Model.Property.outdoorTemp,')[1].split(')', 1)[0].strip()))
         except:
             logger.exception("Unable to find the outdoor temperature.")
             outdoor_temp = None
 
         try:
-            outdoor_humidity = int(text_data.split('Control.Model.Property.outdoorHumidity,')[1].split(')', 1)[0])
+            outdoor_humidity = int(float(text_data.split('Control.Model.Property.outdoorHumidity,')[1].split(')', 1)[0].strip()))
         except:
             logger.exception("Unable to find the outdoor humidity.")
             outdoor_humidity = None
 
         return {
             'OutdoorTemperature' : outdoor_temp,
             'OutdoorHumidity' : outdoor_humidity,
```

### Comparing `pyhtcc-0.1.8/pyhtcc.egg-info/PKG-INFO` & `pyhtcc-0.1.9/pyhtcc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyhtcc
-Version: 0.1.8
-Summary: UNKNOWN
+Version: 0.1.9
 Home-page: http://github.com/csm10495/pyhtcc
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
@@ -65,9 +63,7 @@
   -C COOL, --cool COOL  Set a target cooling temperature
 
 ```
 [CLI_OUTPUT_MARKER]::
 
 ## License
 MIT License
-
-
```

### Comparing `pyhtcc-0.1.8/setup.py` & `pyhtcc-0.1.9/setup.py`

 * *Files identical despite different names*

