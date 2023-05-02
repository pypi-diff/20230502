# Comparing `tmp/pvlive_api-0.12.tar.gz` & `tmp/pvlive_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvlive_api-0.12.tar", last modified: Fri Dec  9 14:28:04 2022, max compression
+gzip compressed data, was "pvlive_api-1.0.0.tar", last modified: Tue May  2 16:49:49 2023, max compression
```

## Comparing `pvlive_api-0.12.tar` & `pvlive_api-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-12-09 14:28:04.385340 pvlive_api-0.12/
--rw-rw-rw-   0        0        0     9632 2022-12-09 14:28:04.388745 pvlive_api-0.12/PKG-INFO
--rw-rw-rw-   0        0        0     8479 2022-12-09 13:37:45.000000 pvlive_api-0.12/README.md
-drwxrwxrwx   0        0        0        0 2022-12-09 14:28:04.345580 pvlive_api-0.12/Tests/
--rw-rw-rw-   0        0        0        0 2022-12-09 13:10:52.000000 pvlive_api-0.12/Tests/__init__.py
--rw-rw-rw-   0        0        0    10205 2022-12-09 13:10:52.000000 pvlive_api-0.12/Tests/test_pvlive_api.py
-drwxrwxrwx   0        0        0        0 2022-12-09 14:28:04.345580 pvlive_api-0.12/pvlive_api/
--rw-rw-rw-   0        0        0       62 2022-12-09 13:10:52.000000 pvlive_api-0.12/pvlive_api/__init__.py
--rw-rw-rw-   0        0        0    22560 2022-12-09 13:10:52.000000 pvlive_api-0.12/pvlive_api/pvlive.py
-drwxrwxrwx   0        0        0        0 2022-12-09 14:28:04.385340 pvlive_api-0.12/pvlive_api.egg-info/
--rw-rw-rw-   0        0        0     9632 2022-12-09 14:28:03.000000 pvlive_api-0.12/pvlive_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2022-12-09 14:28:04.000000 pvlive_api-0.12/pvlive_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-09 14:28:03.000000 pvlive_api-0.12/pvlive_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-12-09 14:28:03.000000 pvlive_api-0.12/pvlive_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2022-12-09 14:28:03.000000 pvlive_api-0.12/pvlive_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-12-09 14:28:03.000000 pvlive_api-0.12/pvlive_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-12-09 14:28:04.397724 pvlive_api-0.12/setup.cfg
--rw-rw-rw-   0        0        0     4317 2022-12-09 14:27:24.000000 pvlive_api-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.397793 pvlive_api-1.0.0/
+-rw-rw-rw-   0        0        0    12410 2023-05-02 16:49:49.397793 pvlive_api-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11433 2023-05-02 16:23:49.000000 pvlive_api-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.379450 pvlive_api-1.0.0/Tests/
+-rw-rw-rw-   0        0        0        0 2023-02-15 16:12:03.000000 pvlive_api-1.0.0/Tests/__init__.py
+-rw-rw-rw-   0        0        0    10205 2023-05-02 16:44:24.000000 pvlive_api-1.0.0/Tests/test_pvlive_api.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.381427 pvlive_api-1.0.0/pvlive_api/
+-rw-rw-rw-   0        0        0       62 2023-02-15 16:12:03.000000 pvlive_api-1.0.0/pvlive_api/__init__.py
+-rw-rw-rw-   0        0        0    23398 2023-05-02 16:46:04.000000 pvlive_api-1.0.0/pvlive_api/pvlive.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.396783 pvlive_api-1.0.0/pvlive_api.egg-info/
+-rw-rw-rw-   0        0        0    12410 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-02 16:49:49.401321 pvlive_api-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     4330 2023-05-02 16:24:35.000000 pvlive_api-1.0.0/setup.py
```

### Comparing `pvlive_api-0.12/Tests/test_pvlive_api.py` & `pvlive_api-1.0.0/Tests/test_pvlive_api.py`

 * *Files identical despite different names*

### Comparing `pvlive_api-0.12/pvlive_api/pvlive.py` & `pvlive_api-1.0.0/pvlive_api/pvlive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 """
 A Python interface for the PV_Live web API from Sheffield Solar.
 
 - Jamie Taylor <jamie.taylor@sheffield.ac.uk>
 - Ethan Jones <ejones18@sheffield.ac.uk>
 - First Authored: 2018-06-04
-- Updated: 2020-10-20 to return Pandas dataframe object
-- Updated: 2021-01-15 to use v3 of the PV_Live API and expose GSP endpoints as well as PES
-- Updated: 2022-07-19 to use v4 of the PV_Live API
 """
 
 import sys
 import os
 import json
 from datetime import datetime, timedelta, date, time
 from time import sleep
-from typing import List, Union, Tuple
+from typing import List, Union, Tuple, Dict, Optional
 import inspect
+import argparse
+
 import pytz
 import requests
-import argparse
 from numpy import nan, int64
 import pandas as pd
 
-
 class PVLiveException(Exception):
     """An Exception specific to the PVLive class."""
     def __init__(self, msg):
         try:
             caller_file = inspect.stack()[2][1]
         except:
             caller_file = os.path.basename(__file__)
-        self.msg = "%s (in '%s')" % (msg, caller_file)
+        self.msg = f"{msg} (in '{caller_file}')"
 
     def __str__(self):
         return self.msg
 
-
 class PVLive:
     """
     Interface with the PV_Live web API.
 
     Parameters
     ----------
     `retries` : int
         Optionally specify the number of retries to use should the API respond with anything
         other than status code 200. Exponential back-off applies inbetween retries.
+    `proxies` : Optional[Dict]
+        Optionally specify a Dict of proxies for http and https requests in the format:
+        {"http": "<address>", "https": "<address>"}
     """
-    def __init__(self, retries: int = 3):
+    def __init__(self, retries: int = 3, proxies: Optional[Dict] = None):
         self.base_url = "https://api0.solar.sheffield.ac.uk/pvlive/api/v4/"
         self.max_range = {"national": timedelta(days=365), "regional": timedelta(days=30)}
         self.retries = retries
+        self.proxies = proxies
         self.gsp_list = self._get_gsp_list()
         self.pes_list = self._get_pes_list()
         self.gsp_ids = self.gsp_list.gsp_id.dropna().astype(int64).unique()
         self.pes_ids = self.pes_list.pes_id.dropna().astype(int64).unique()
 
     def _get_gsp_list(self):
         """Fetch the GSP list from the API and convert to Pandas DataFrame."""
@@ -358,27 +358,27 @@
         data = pd.DataFrame(data, columns=columns)
         if "datetime_gmt" in data.columns:
             data.datetime_gmt = pd.to_datetime(data.datetime_gmt)
         return data
 
     def _build_url(self, entity_type, entity_id, params):
         """Construct the appropriate URL for a given set of parameters."""
-        base_url = "{}{}/{}".format(self.base_url, entity_type, entity_id)
+        base_url = f"{self.base_url}{entity_type}/{entity_id}"
         url = base_url + "?" + "&".join(["{}={}".format(k, params[k]) for k in params])
         return url
 
     def _fetch_url(self, url):
         """Fetch the URL with GET request."""
         success = False
         try_counter = 0
         delay = 1
         while not success and try_counter < self.retries + 1:
             try_counter += 1
             try:
-                page = requests.get(url)
+                page = requests.get(url, proxies=self.proxies)
                 page.raise_for_status()
                 success = True
             except requests.exceptions.HTTPError:
                 sleep(delay)
                 delay *= 2
                 continue
         if not success:
@@ -410,44 +410,49 @@
             if entity_id not in self.gsp_ids:
                 raise PVLiveException(f"The gsp_id {entity_id} was not found.")
         periods = [5, 30]
         if period not in periods:
             raise ValueError("The period parameter must be one of: "
                              f"{', '.join(map(str, periods))}.")
 
-
 def parse_options():
     """Parse command line options."""
     parser = argparse.ArgumentParser(description=("This is a command line interface (CLI) for the "
                                                   "PV_Live API module"),
-                                     epilog="Jamie Taylor, 2018-06-04")
+                                     epilog="Jamie Taylor & Ethan Jones, 2018-06-04")
     parser.add_argument("-s", "--start", metavar="\"<yyyy-mm-dd HH:MM:SS>\"", dest="start",
                         action="store", type=str, required=False, default=None,
                         help="Specify a UTC start date in 'yyyy-mm-dd HH:MM:SS' format "
                              "(inclusive), default behaviour is to retrieve the latest outturn.")
     parser.add_argument("-e", "--end", metavar="\"<yyyy-mm-dd HH:MM:SS>\"", dest="end",
                         action="store", type=str, required=False, default=None,
                         help="Specify a UTC end date in 'yyyy-mm-dd HH:MM:SS' format (inclusive), "
                         "default behaviour is to retrieve the latest outturn.")
     parser.add_argument("--entity_type", metavar="<entity_type>", dest="entity_type",
                         action="store", type=str, required=False, default="gsp",
                         choices=["gsp", "pes"],
-                        help="Specify an entity type, either 'gsp' or 'pes'. Default is 'pes'.")
+                        help="Specify an entity type, either 'gsp' or 'pes'. Default is 'gsp'.")
     parser.add_argument("--entity_id", metavar="<entity_id>", dest="entity_id", action="store",
                         type=int, required=False, default=0,
                         help="Specify an entity ID, default is 0 (i.e. national).")
     parser.add_argument("--period", metavar="<5|30>", dest="period", action="store",
                         type=int, required=False, default=30, choices=(5, 30),
                         help="Desired temporal resolution (in minutes) for PV outturn estimates. "
                              "Default is 30.")
     parser.add_argument("-q", "--quiet", dest="quiet", action="store_true",
                         required=False, help="Specify to not print anything to stdout.")
     parser.add_argument("-o", "--outfile", metavar="</path/to/output/file>", dest="outfile",
                         action="store", type=str, required=False,
                         help="Specify a CSV file to write results to.")
+    parser.add_argument('-http', '--http-proxy', metavar="<http_proxy>", dest="http",
+                        type=str, required=False, default=None, action="store",
+                        help="HTTP Proxy address")
+    parser.add_argument('-https', '--https-proxy', metavar="<https_proxy>", dest="https",
+                        type=str, required=False, default=None, action="store",
+                        help="HTTPS Proxy address")
     options = parser.parse_args()
 
     def handle_options(options):
         """Validate command line args and pre-process where necessary."""
         if (options.outfile is not None and os.path.exists(options.outfile)) and not options.quiet:
             try:
                 input(f"The output file '{options.outfile}' already exists and will be "
@@ -467,22 +472,27 @@
                                 "'yyyy-mm-dd HH:MM:SS' format.")
         if options.end is not None:
             try:
                 options.end = pytz.utc.localize(datetime.strptime(options.end, "%Y-%m-%d %H:%M:%S"))
             except:
                 raise Exception("OptionsError: Failed to parse end datetime, make sure you use "
                                 "'yyyy-mm-dd HH:MM:SS' format.")
+        proxies = {} if options.http is not None or options.https is not None else None
+        if options.http is not None:
+            proxies.update({"http": options.http})
+        if options.https is not None:
+            proxies.update({"https": options.https})
+        options.proxies = proxies
         return options
     return handle_options(options)
 
-
 def main():
     """Load CLI options and access the API accordingly."""
     options = parse_options()
-    pvl = PVLive()
+    pvl = PVLive(proxies=options.proxies)
     if options.start is None and options.end is None:
         data = pvl.latest(entity_type=options.entity_type, entity_id=options.entity_id,
                           extra_fields="installedcapacity_mwp", dataframe=True)
     else:
         start = datetime(2014, 1, 1, 0, 30, tzinfo=pytz.utc) if options.start is None \
             else options.start
         end = pytz.utc.localize(datetime.utcnow()) if options.end is None else options.end
@@ -490,10 +500,9 @@
                            extra_fields="installedcapacity_mwp", period=options.period,
                            dataframe=True)
     if options.outfile is not None:
         data.to_csv(options.outfile, float_format="%.3f", index=False)
     if not options.quiet:
         print(data)
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `pvlive_api-0.12/setup.py` & `pvlive_api-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
-    long_description = f.read()
+    long_description = f.read().replace('\r', '')
 
 setup(
     name="pvlive_api",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.12",
+    version="1.0.0",
 
     description="A Python interface for the PV_Live web API from Sheffield Solar.",
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url="https://github.com/SheffieldSolar/PV_Live",
 
-    download_url="https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/0.12.tar.gz",
+    download_url="https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/1.0.0.tar.gz",
 
     # Author details
     author="Jamie Taylor",
     author_email="jamie.taylor@sheffield.ac.uk",
 
     # Choose your license
     license="None",
@@ -56,19 +56,19 @@
         "Topic :: Utilities",
 
         # Pick your license as you wish (should match "license" above)
         # "License :: OSI Approved :: MIT License",
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 
     # What does your project relate to?
     keywords="solar pv pv_live api",
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
```

