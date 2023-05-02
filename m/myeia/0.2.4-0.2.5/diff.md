# Comparing `tmp/myeia-0.2.4.tar.gz` & `tmp/myeia-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myeia-0.2.4.tar", last modified: Wed Feb  8 01:11:56 2023, max compression
+gzip compressed data, was "myeia-0.2.5.tar", last modified: Tue May  2 12:57:15 2023, max compression
```

## Comparing `myeia-0.2.4.tar` & `myeia-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 01:11:56.473852 myeia-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-08 01:11:34.000000 myeia-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-02-08 01:11:56.473852 myeia-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-02-08 01:11:34.000000 myeia-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 01:11:56.473852 myeia-0.2.4/myeia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 01:11:34.000000 myeia-0.2.4/myeia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-02-08 01:11:34.000000 myeia-0.2.4/myeia/api.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-08 01:11:34.000000 myeia-0.2.4/myeia/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 01:11:56.473852 myeia-0.2.4/myeia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-02-08 01:11:56.000000 myeia-0.2.4/myeia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-08 01:11:56.000000 myeia-0.2.4/myeia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 01:11:56.000000 myeia-0.2.4/myeia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-08 01:11:56.000000 myeia-0.2.4/myeia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-08 01:11:56.000000 myeia-0.2.4/myeia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-08 01:11:34.000000 myeia-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-08 01:11:56.473852 myeia-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-02-08 01:11:34.000000 myeia-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:57:15.112279 myeia-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 12:56:48.000000 myeia-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-02 12:57:15.112279 myeia-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-02 12:56:48.000000 myeia-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:57:15.112279 myeia-0.2.5/myeia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:56:48.000000 myeia-0.2.5/myeia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-02 12:56:48.000000 myeia-0.2.5/myeia/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 12:56:48.000000 myeia-0.2.5/myeia/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:57:15.112279 myeia-0.2.5/myeia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-02 12:57:15.000000 myeia-0.2.5/myeia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-02 12:57:15.000000 myeia-0.2.5/myeia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:57:15.000000 myeia-0.2.5/myeia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 12:57:15.000000 myeia-0.2.5/myeia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 12:57:15.000000 myeia-0.2.5/myeia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 12:56:48.000000 myeia-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 12:57:15.112279 myeia-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-02 12:56:48.000000 myeia-0.2.5/setup.py
```

### Comparing `myeia-0.2.4/LICENSE` & `myeia-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myeia-0.2.4/PKG-INFO` & `myeia-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myeia
-Version: 0.2.4
+Version: 0.2.5
 Summary: UNKNOWN
 Home-page: https://github.com/philsv/myeia
 Author: philsv
 Author-email: frphsv@gmail.com
 License: MIT
 Description: # myeia
```

### Comparing `myeia-0.2.4/README.md` & `myeia-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `myeia-0.2.4/myeia/api.py` & `myeia-0.2.5/myeia/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 import warnings
 from dataclasses import dataclass
 from typing import Optional
 
 import pandas as pd
 import requests
 from dotenv import load_dotenv
-from pandas.errors import SettingWithCopyWarning
+
+try:
+    from pandas.errors import SettingWithCopyWarning
+except ImportError as e:
+    raise ImportError("Please upgrade your version of pandas to 1.5.3 or higher.") from e
 
 warnings.simplefilter(action="ignore", category=SettingWithCopyWarning)
+
 load_dotenv()
 
 
 @dataclass
 class API:
     """
     Python Wrapper for U.S. Energy Information Administration (EIA) APIv2.
@@ -28,38 +33,31 @@
     ) -> pd.DataFrame:
         """
         Returns data for a given series in the simpler APIv1 format.
 
         Args:
             series_id (str): The series ID. For example, "NG.RNGC1.W".
             new_name (str): A name you want to give the value column.
+
         Returns:
             pd.DataFrame: A DataFrame with the date and value columns.
         """
         headers = {"Accept": "*/*"}
         url = f"{self.url}seriesid/{series_id}?api_key={self.token}"
-        response = requests.get(url, headers=headers)
-        response.raise_for_status()
-        json_response = response.json()
+        base_df = self.get_json_response(url, headers)
 
-        base_df = pd.DataFrame(json_response["response"]["data"])
-
-        if "series-description" in base_df.columns:
-            series_description = base_df["series-description"][0]
+        if not new_name:
+            series_description = base_df["series-description"][0] if "series-description" in base_df.columns else series_id
         else:
-            series_description = series_id
-
-        if new_name != "":
             series_description = new_name
 
         df = base_df[["period", "value"]]
+
         df.rename(columns={df.columns[0]: "Date", df.columns[1]: series_description}, inplace=True)
-        df["Date"] = pd.to_datetime(df["Date"])
-        df.set_index("Date", inplace=True)
-        return df
+        return self.format_time_series_data(df)
 
     def get_series_via_route(
         self,
         route: str,
         series: str,
         frequency: str,
         facet: str = "series",
@@ -70,44 +68,50 @@
 
         Args:
             route (str): The route to the series. For example, "natural-gas/pri/fut".
             series (str): The series ID. For example, "RNGC1".
             frequency (str): The frequency of the series. For example, "daily".
             facet (str): The facet of the series. For example, "series", "seriesId".
             new_name (str): A name you want to give the value column.
+
         Returns:
             pd.DataFrame: A DataFrame with the date and value columns.
         """
         headers = {"Accept": "*/*"}
 
         api_route = f"{route}/data/?api_key={self.token}&data[]=value&frequency={frequency}"
         series = f"&facets[{facet}][]={series}"
         sort = "&sort[0][column]=period&sort[0][direction]=desc"
         url = f"{self.url}{api_route}{series}{sort}"
 
-        response = requests.get(url, headers=headers)
-        response.raise_for_status()
-        json_response = response.json()
-
-        base_df = pd.DataFrame(json_response["response"]["data"])
+        base_df = self.get_json_response(url, headers)
 
         if facet == "series":
             df = base_df[["period", "value", "series-description", "series"]]
-
         elif facet == "seriesId":
             df = base_df[["period", "value", "seriesDescription", "seriesId"]]
 
         df.reset_index(drop=True, inplace=True)
 
-        name = df[df.columns[2]][0]
-
-        if new_name != "":
-            name = new_name
-
+        name = new_name if new_name != "" else df[df.columns[2]][0]
         df.rename(columns={df.columns[1]: name}, inplace=True)
-
         df = df.iloc[:, :2]
 
         df.rename(columns={df.columns[0]: "Date"}, inplace=True)
+        return self.format_time_series_data(df)
+
+    def format_time_series_data(self, df):
+        """
+        Helper function to format time series data.
+        """
         df["Date"] = pd.to_datetime(df["Date"])
         df.set_index("Date", inplace=True)
         return df
+
+    def get_json_response(self, url: str, headers: dict):
+        """
+        Helper function to get JSON response from API.
+        """
+        response = requests.get(url, headers=headers)
+        response.raise_for_status()
+        json_response = response.json()
+        return pd.DataFrame(json_response["response"]["data"])
```

### Comparing `myeia-0.2.4/myeia.egg-info/PKG-INFO` & `myeia-0.2.5/myeia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myeia
-Version: 0.2.4
+Version: 0.2.5
 Summary: UNKNOWN
 Home-page: https://github.com/philsv/myeia
 Author: philsv
 Author-email: frphsv@gmail.com
 License: MIT
 Description: # myeia
```

### Comparing `myeia-0.2.4/setup.py` & `myeia-0.2.5/setup.py`

 * *Files identical despite different names*

