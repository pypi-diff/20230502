# Comparing `tmp/pysurfex-0.0.3.2.tar.gz` & `tmp/pysurfex-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurfex-0.0.3.2.tar", max compression
+gzip compressed data, was "pysurfex-0.0.3.3.tar", max compression
```

## Comparing `pysurfex-0.0.3.2.tar` & `pysurfex-0.0.3.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3318 2023-05-02 18:57:12.959139 pysurfex-0.0.3.2/README.rst
--rw-r--r--   0        0        0     5202 2023-05-02 18:57:12.963139 pysurfex-0.0.3.2/pyproject.toml
--rw-r--r--   0        0        0      142 2023-05-02 18:57:12.963139 pysurfex-0.0.3.2/pysurfex/__init__.py
--rw-r--r--   0        0        0    30965 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/binary_input.py
--rw-r--r--   0        0        0    18837 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/bufr.py
--rw-r--r--   0        0        0    10460 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cache.py
--rw-r--r--   0        0        0    19335 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/config.yml
--rw-r--r--   0        0        0     8985 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/config_exp_surfex.toml
--rw-r--r--   0        0        0      135 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/default_thredds.cfg
--rw-r--r--   0        0        0     5253 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/first_guess.yml
--rw-r--r--   0        0        0      192 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/qc_codes.json
--rw-r--r--   0        0        0      370 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/user.yml
--rw-r--r--   0        0        0    62389 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cli.py
--rw-r--r--   0        0        0    62271 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cmd_parsing.py
--rw-r--r--   0        0        0    32663 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/configuration.py
--rw-r--r--   0        0        0     1291 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/datetime_utils.py
--rw-r--r--   0        0        0     8511 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/ecoclimap.py
--rw-r--r--   0        0        0     3891 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/fa.py
--rw-r--r--   0        0        0    58096 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/file.py
--rw-r--r--   0        0        0    35668 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/forcing.py
--rw-r--r--   0        0        0    33675 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/geo.py
--rw-r--r--   0        0        0    22471 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/grib.py
--rw-r--r--   0        0        0    14928 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/input_methods.py
--rw-r--r--   0        0        0    18924 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/interpolation.py
--rw-r--r--   0        0        0   100050 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/namelist.py
--rw-r--r--   0        0        0    34770 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/netcdf.py
--rw-r--r--   0        0        0    37729 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/obs.py
--rw-r--r--   0        0        0     4483 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/observation.py
--rw-r--r--   0        0        0    12016 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/obsmon.py
--rw-r--r--   0        0        0     6415 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/obsoul.py
--rw-r--r--   0        0        0    16227 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/platform.py
--rw-r--r--   0        0        0       20 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/plot.py
--rw-r--r--   0        0        0    17168 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/read.py
--rw-r--r--   0        0        0    11682 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/run.py
--rw-r--r--   0        0        0     2254 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/assimilation.json
--rw-r--r--   0        0        0        0 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/filetype.json
--rw-r--r--   0        0        0     1075 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/forecast.json
--rw-r--r--   0        0        0     1305 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/pgd.json
--rw-r--r--   0        0        0      952 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/prep.json
--rw-r--r--   0        0        0     3499 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/timeseries.py
--rw-r--r--   0        0        0    67688 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/titan.py
--rw-r--r--   0        0        0     3463 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/util.py
--rw-r--r--   0        0        0    19977 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/variable.py
--rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 pysurfex-0.0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3318 2023-05-02 20:59:12.790631 pysurfex-0.0.3.3/README.rst
+-rw-r--r--   0        0        0     5202 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/__init__.py
+-rw-r--r--   0        0        0    30965 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/binary_input.py
+-rw-r--r--   0        0        0    18837 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/bufr.py
+-rw-r--r--   0        0        0    10460 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cache.py
+-rw-r--r--   0        0        0    19335 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cfg/config.yml
+-rw-r--r--   0        0        0     8985 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cfg/config_exp_surfex.toml
+-rw-r--r--   0        0        0      135 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cfg/default_thredds.cfg
+-rw-r--r--   0        0        0     5253 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cfg/first_guess.yml
+-rw-r--r--   0        0        0      192 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cfg/qc_codes.json
+-rw-r--r--   0        0        0      370 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cfg/user.yml
+-rw-r--r--   0        0        0    62389 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cli.py
+-rw-r--r--   0        0        0    62271 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/cmd_parsing.py
+-rw-r--r--   0        0        0    32663 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/configuration.py
+-rw-r--r--   0        0        0     1291 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/datetime_utils.py
+-rw-r--r--   0        0        0     8511 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/ecoclimap.py
+-rw-r--r--   0        0        0     3891 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/fa.py
+-rw-r--r--   0        0        0    58096 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/file.py
+-rw-r--r--   0        0        0    35668 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/forcing.py
+-rw-r--r--   0        0        0    33675 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/geo.py
+-rw-r--r--   0        0        0    22471 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/grib.py
+-rw-r--r--   0        0        0    14928 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/input_methods.py
+-rw-r--r--   0        0        0    18924 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/interpolation.py
+-rw-r--r--   0        0        0   100050 2023-05-02 20:59:12.798631 pysurfex-0.0.3.3/pysurfex/namelist.py
+-rw-r--r--   0        0        0    34770 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/netcdf.py
+-rw-r--r--   0        0        0    37729 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/obs.py
+-rw-r--r--   0        0        0     4483 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/observation.py
+-rw-r--r--   0        0        0    12016 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/obsmon.py
+-rw-r--r--   0        0        0     6415 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/obsoul.py
+-rw-r--r--   0        0        0    16227 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/platform.py
+-rw-r--r--   0        0        0       20 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/plot.py
+-rw-r--r--   0        0        0    17168 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/read.py
+-rw-r--r--   0        0        0    11682 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/run.py
+-rw-r--r--   0        0        0     2254 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/settings/assimilation.json
+-rw-r--r--   0        0        0        0 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/settings/filetype.json
+-rw-r--r--   0        0        0     1075 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/settings/forecast.json
+-rw-r--r--   0        0        0     1305 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/settings/pgd.json
+-rw-r--r--   0        0        0      952 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/settings/prep.json
+-rw-r--r--   0        0        0     3499 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/timeseries.py
+-rw-r--r--   0        0        0    67688 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/titan.py
+-rw-r--r--   0        0        0     3463 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/util.py
+-rw-r--r--   0        0        0    19977 2023-05-02 20:59:12.802631 pysurfex-0.0.3.3/pysurfex/variable.py
+-rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 pysurfex-0.0.3.3/PKG-INFO
```

### Comparing `pysurfex-0.0.3.2/README.rst` & `pysurfex-0.0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pyproject.toml` & `pysurfex-0.0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "pysurfex"
-    version = "0.0.3.2"
+    version = "0.0.3.3"
     description = "Python API to SURFEX"
     authors = ["Trygve Aspelien"]
     license = "MIT"
     readme = "README.rst"
     repository = "https://github.com/metno/pysurfex"
     documentation = "https://metno.github.io/pysurfex/"
```

### Comparing `pysurfex-0.0.3.2/pysurfex/binary_input.py` & `pysurfex-0.0.3.3/pysurfex/binary_input.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/bufr.py` & `pysurfex-0.0.3.3/pysurfex/bufr.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/cache.py` & `pysurfex-0.0.3.3/pysurfex/cache.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/cfg/config.yml` & `pysurfex-0.0.3.3/pysurfex/cfg/config.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/cfg/config_exp_surfex.toml` & `pysurfex-0.0.3.3/pysurfex/cfg/config_exp_surfex.toml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/cfg/first_guess.yml` & `pysurfex-0.0.3.3/pysurfex/cfg/first_guess.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/cli.py` & `pysurfex-0.0.3.3/pysurfex/cli.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/cmd_parsing.py` & `pysurfex-0.0.3.3/pysurfex/cmd_parsing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/configuration.py` & `pysurfex-0.0.3.3/pysurfex/configuration.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/datetime_utils.py` & `pysurfex-0.0.3.3/pysurfex/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/ecoclimap.py` & `pysurfex-0.0.3.3/pysurfex/ecoclimap.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/fa.py` & `pysurfex-0.0.3.3/pysurfex/fa.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/file.py` & `pysurfex-0.0.3.3/pysurfex/file.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/forcing.py` & `pysurfex-0.0.3.3/pysurfex/forcing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/geo.py` & `pysurfex-0.0.3.3/pysurfex/geo.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/grib.py` & `pysurfex-0.0.3.3/pysurfex/grib.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/input_methods.py` & `pysurfex-0.0.3.3/pysurfex/input_methods.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/interpolation.py` & `pysurfex-0.0.3.3/pysurfex/interpolation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/namelist.py` & `pysurfex-0.0.3.3/pysurfex/namelist.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/netcdf.py` & `pysurfex-0.0.3.3/pysurfex/netcdf.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/obs.py` & `pysurfex-0.0.3.3/pysurfex/obs.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/observation.py` & `pysurfex-0.0.3.3/pysurfex/observation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/obsmon.py` & `pysurfex-0.0.3.3/pysurfex/obsmon.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/obsoul.py` & `pysurfex-0.0.3.3/pysurfex/obsoul.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/platform.py` & `pysurfex-0.0.3.3/pysurfex/platform.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/read.py` & `pysurfex-0.0.3.3/pysurfex/read.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/run.py` & `pysurfex-0.0.3.3/pysurfex/run.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/settings/assimilation.json` & `pysurfex-0.0.3.3/pysurfex/settings/assimilation.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/settings/forecast.json` & `pysurfex-0.0.3.3/pysurfex/settings/forecast.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/settings/pgd.json` & `pysurfex-0.0.3.3/pysurfex/settings/pgd.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/settings/prep.json` & `pysurfex-0.0.3.3/pysurfex/settings/prep.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/timeseries.py` & `pysurfex-0.0.3.3/pysurfex/timeseries.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/titan.py` & `pysurfex-0.0.3.3/pysurfex/titan.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/util.py` & `pysurfex-0.0.3.3/pysurfex/util.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/pysurfex/variable.py` & `pysurfex-0.0.3.3/pysurfex/variable.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.2/PKG-INFO` & `pysurfex-0.0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysurfex
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: Python API to SURFEX
 Home-page: https://github.com/metno/pysurfex
 License: MIT
 Author: Trygve Aspelien
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

