# Comparing `tmp/forecast-weather-0.1.1.tar.gz` & `tmp/forecast-weather-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecast-weather-0.1.1.tar", last modified: Mon Apr  3 20:42:46 2023, max compression
+gzip compressed data, was "forecast-weather-0.1.2.tar", last modified: Tue May  2 21:53:51 2023, max compression
```

## Comparing `forecast-weather-0.1.1.tar` & `forecast-weather-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-04-03 20:42:46.626721 forecast-weather-0.1.1/
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      402 2023-04-03 20:38:23.000000 forecast-weather-0.1.1/.bumpversion.cfg
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      522 2023-04-03 20:13:06.000000 forecast-weather-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)    11357 2023-02-18 18:28:16.000000 forecast-weather-0.1.1/LICENSE
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      493 2023-04-03 17:41:06.000000 forecast-weather-0.1.1/MANIFEST.in
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)     2286 2023-03-10 22:08:02.000000 forecast-weather-0.1.1/Makefile
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)    16154 2023-04-03 20:42:46.626721 forecast-weather-0.1.1/PKG-INFO
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)     2312 2023-04-03 20:38:23.000000 forecast-weather-0.1.1/README.md
-drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-04-03 20:42:46.626721 forecast-weather-0.1.1/docs/
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      634 2023-04-03 17:41:06.000000 forecast-weather-0.1.1/docs/Makefile
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)     1333 2023-04-03 20:38:23.000000 forecast-weather-0.1.1/docs/conf.py
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      246 2023-04-03 17:41:06.000000 forecast-weather-0.1.1/docs/index.md
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      765 2023-04-03 17:41:06.000000 forecast-weather-0.1.1/docs/make.bat
-drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-04-03 20:42:46.626721 forecast-weather-0.1.1/forecast_weather/
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)       57 2023-03-02 07:29:31.000000 forecast-weather-0.1.1/forecast_weather/__init__.py
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)       93 2023-03-02 07:29:31.000000 forecast-weather-0.1.1/forecast_weather/__main__.py
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)       22 2023-04-03 20:38:23.000000 forecast-weather-0.1.1/forecast_weather/_version.py
-drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-04-03 20:42:46.626721 forecast-weather-0.1.1/forecast_weather/tests/
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)    14218 2023-04-03 17:41:06.000000 forecast-weather-0.1.1/forecast_weather/tests/test_all.py
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)     3236 2023-04-03 20:11:14.000000 forecast-weather-0.1.1/forecast_weather/weather.py
-drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-04-03 20:42:46.626721 forecast-weather-0.1.1/forecast_weather.egg-info/
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)    16154 2023-04-03 20:42:46.000000 forecast-weather-0.1.1/forecast_weather.egg-info/PKG-INFO
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      499 2023-04-03 20:42:46.000000 forecast-weather-0.1.1/forecast_weather.egg-info/SOURCES.txt
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)        1 2023-04-03 20:42:46.000000 forecast-weather-0.1.1/forecast_weather.egg-info/dependency_links.txt
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)      156 2023-04-03 20:42:46.000000 forecast-weather-0.1.1/forecast_weather.egg-info/requires.txt
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)       17 2023-04-03 20:42:46.000000 forecast-weather-0.1.1/forecast_weather.egg-info/top_level.txt
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)     2240 2023-04-03 20:38:23.000000 forecast-weather-0.1.1/pyproject.toml
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)       38 2023-04-03 20:42:46.626721 forecast-weather-0.1.1/setup.cfg
--rw-r--r--   0 e7kim     (1000) e7kim     (1000)       39 2023-03-27 03:07:13.000000 forecast-weather-0.1.1/setup.py
+drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-05-02 21:53:51.566404 forecast-weather-0.1.2/
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)      402 2023-05-02 20:25:37.000000 forecast-weather-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)      522 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)    11357 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/LICENSE
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)      551 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/MANIFEST.in
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)     2286 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/Makefile
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)    16760 2023-05-02 21:53:51.566404 forecast-weather-0.1.2/PKG-INFO
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)     2918 2023-04-05 07:38:21.000000 forecast-weather-0.1.2/README.md
+drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-05-02 21:53:51.556404 forecast-weather-0.1.2/docs/
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)      634 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/docs/Makefile
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)     1408 2023-05-02 20:25:37.000000 forecast-weather-0.1.2/docs/conf.py
+drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-05-02 21:53:51.556404 forecast-weather-0.1.2/docs/img/
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)   173495 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/docs/img/demo.gif
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)     3332 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/docs/index.md
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)      765 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/docs/make.bat
+drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-05-02 21:53:51.556404 forecast-weather-0.1.2/docs/source/
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)       96 2023-04-05 07:19:26.000000 forecast-weather-0.1.2/docs/source/forecast_weather.rst
+drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-05-02 21:53:51.566404 forecast-weather-0.1.2/forecast_weather/
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)       57 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/forecast_weather/__init__.py
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)       88 2023-05-02 20:25:37.000000 forecast-weather-0.1.2/forecast_weather/__main__.py
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)       22 2023-05-02 20:25:37.000000 forecast-weather-0.1.2/forecast_weather/_version.py
+drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-05-02 21:53:51.566404 forecast-weather-0.1.2/forecast_weather/tests/
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)    14218 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/forecast_weather/tests/test_all.py
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)     6467 2023-05-02 20:25:37.000000 forecast-weather-0.1.2/forecast_weather/weather.py
+drwxr-xr-x   0 e7kim     (1000) e7kim     (1000)        0 2023-05-02 21:53:51.566404 forecast-weather-0.1.2/forecast_weather.egg-info/
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)    16760 2023-05-02 21:53:51.000000 forecast-weather-0.1.2/forecast_weather.egg-info/PKG-INFO
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)      550 2023-05-02 21:53:51.000000 forecast-weather-0.1.2/forecast_weather.egg-info/SOURCES.txt
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)        1 2023-05-02 21:53:51.000000 forecast-weather-0.1.2/forecast_weather.egg-info/dependency_links.txt
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)      156 2023-05-02 21:53:51.000000 forecast-weather-0.1.2/forecast_weather.egg-info/requires.txt
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)       17 2023-05-02 21:53:51.000000 forecast-weather-0.1.2/forecast_weather.egg-info/top_level.txt
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)     2240 2023-05-02 20:25:37.000000 forecast-weather-0.1.2/pyproject.toml
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)       38 2023-05-02 21:53:51.566404 forecast-weather-0.1.2/setup.cfg
+-rw-r--r--   0 e7kim     (1000) e7kim     (1000)       39 2023-04-05 04:25:44.000000 forecast-weather-0.1.2/setup.py
```

### Comparing `forecast-weather-0.1.1/CONTRIBUTING.md` & `forecast-weather-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `forecast-weather-0.1.1/LICENSE` & `forecast-weather-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forecast-weather-0.1.1/Makefile` & `forecast-weather-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `forecast-weather-0.1.1/PKG-INFO` & `forecast-weather-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecast-weather
-Version: 0.1.1
+Version: 0.1.2
 Summary: This python library easily obtains weather data across various locations and dates.
 Author-email: Eugene Kim <ek3192@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,36 +224,61 @@
 This python library easily obtains weather data across various locations and dates.
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/github/issues/e7kim/forecast-weather)](https://github.com/e7kim/forecast-weather/issues)
 [![Build Status](https://github.com/e7kim/forecast-weather/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/e7kim/forecast-weather/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/e7kim/forecast-weather/branch/main/graph/badge.svg)](https://codecov.io/gh/e7kim/forecast-weather)
 [![PyPI](https://img.shields.io/pypi/v/forecast-weather)](https://pypi.org/project/forecast-weather/)
+[![Docs](https://readthedocs.org/projects/forecast-weather/badge/?version=latest)](https://forecast-weather.readthedocs.io/en/latest/?badge=latest)
 
 # Overview
 `forecast-weather` is a library that allows a user to easily obtain weather data (temperatures, pressure, humidity, precipitation, wind, cloud coverage, etc.) across various locations and dates. The library will make calls to a public weather API and will organize the returned data for ease of use. Some extra functionality in consideration include some form of visual plot/graph generation.
 
 ## Install
 ```
 pip install forecast-weather
 ```
 
 ## API Key
 Go to [weatherapi.com](https://www.weatherapi.com/) to register an account for your free api key. Create a new file **./api_key** and paste your api key here.
 
 ## Usage
-```
+```python
 import forecast_weather as fw
 
 fw.show_current(location = "10027")
 fw.show_forecast(location = "10027", days = "2")
 current = fw.get_current(location = "10027")
 forecast = fw.get_forecast(location = "10027", days = "3")
 ```
 
+## Example
+Running the following code
+```python
+import forecast_weather as fw
+
+fw.show_current(location = "10027")
+```
+Outputs something like this to the console
+```
+Current weather at New York is: 
+Temperature: 68.0 F/ 20.0 C
+Condition: Overcast
+Wind speed: 2.2 mph
+Pressure: 1017.0 mb
+Precipitation: 0.0 in
+Humidity: 55%
+Cloud coverage: 100%
+UV: 4.0
+```
+
+## Demo
+
+![](https://raw.githubusercontent.com/e7kim/forecast-weather/main/docs/img/demo.gif)
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
```

### Comparing `forecast-weather-0.1.1/README.md` & `forecast-weather-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,36 +2,61 @@
 This python library easily obtains weather data across various locations and dates.
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/github/issues/e7kim/forecast-weather)](https://github.com/e7kim/forecast-weather/issues)
 [![Build Status](https://github.com/e7kim/forecast-weather/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/e7kim/forecast-weather/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/e7kim/forecast-weather/branch/main/graph/badge.svg)](https://codecov.io/gh/e7kim/forecast-weather)
 [![PyPI](https://img.shields.io/pypi/v/forecast-weather)](https://pypi.org/project/forecast-weather/)
+[![Docs](https://readthedocs.org/projects/forecast-weather/badge/?version=latest)](https://forecast-weather.readthedocs.io/en/latest/?badge=latest)
 
 # Overview
 `forecast-weather` is a library that allows a user to easily obtain weather data (temperatures, pressure, humidity, precipitation, wind, cloud coverage, etc.) across various locations and dates. The library will make calls to a public weather API and will organize the returned data for ease of use. Some extra functionality in consideration include some form of visual plot/graph generation.
 
 ## Install
 ```
 pip install forecast-weather
 ```
 
 ## API Key
 Go to [weatherapi.com](https://www.weatherapi.com/) to register an account for your free api key. Create a new file **./api_key** and paste your api key here.
 
 ## Usage
-```
+```python
 import forecast_weather as fw
 
 fw.show_current(location = "10027")
 fw.show_forecast(location = "10027", days = "2")
 current = fw.get_current(location = "10027")
 forecast = fw.get_forecast(location = "10027", days = "3")
 ```
 
+## Example
+Running the following code
+```python
+import forecast_weather as fw
+
+fw.show_current(location = "10027")
+```
+Outputs something like this to the console
+```
+Current weather at New York is: 
+Temperature: 68.0 F/ 20.0 C
+Condition: Overcast
+Wind speed: 2.2 mph
+Pressure: 1017.0 mb
+Precipitation: 0.0 in
+Humidity: 55%
+Cloud coverage: 100%
+UV: 4.0
+```
+
+## Demo
+
+![](https://raw.githubusercontent.com/e7kim/forecast-weather/main/docs/img/demo.gif)
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
```

### Comparing `forecast-weather-0.1.1/docs/Makefile` & `forecast-weather-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `forecast-weather-0.1.1/docs/conf.py` & `forecast-weather-0.1.2/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-import sphinx_rtd_theme
+import sphinx_rtd_theme, sys, os
 from recommonmark.transform import AutoStructify
 
 project = 'forecast-weather'
 copyright = '2023, Eugene Kim'
 author = 'Eugene Kim'
-release = '0.1.1'
+release = '0.1.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
-extensions = ['recommonmark', 'sphinx.ext.autodoc']
+extensions = ['recommonmark', 'sphinx.ext.autodoc', 'sphinx.ext.napoleon']
 source_suffix = ['.rst', '.md']
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 
 
@@ -30,8 +30,10 @@
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 html_static_path = ['_static']
 
 def setup(app):
     app.add_config_value('recommonmark_config', {
         'auto_toc_tree_section': 'Contents',
     }, True)
-    app.add_transform(AutoStructify)
+    app.add_transform(AutoStructify)
+
+sys.path.insert(0, os.path.abspath('..'))
```

### Comparing `forecast-weather-0.1.1/docs/make.bat` & `forecast-weather-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `forecast-weather-0.1.1/forecast_weather/tests/test_all.py` & `forecast-weather-0.1.2/forecast_weather/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `forecast-weather-0.1.1/forecast_weather.egg-info/PKG-INFO` & `forecast-weather-0.1.2/forecast_weather.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecast-weather
-Version: 0.1.1
+Version: 0.1.2
 Summary: This python library easily obtains weather data across various locations and dates.
 Author-email: Eugene Kim <ek3192@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,36 +224,61 @@
 This python library easily obtains weather data across various locations and dates.
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/github/issues/e7kim/forecast-weather)](https://github.com/e7kim/forecast-weather/issues)
 [![Build Status](https://github.com/e7kim/forecast-weather/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/e7kim/forecast-weather/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/e7kim/forecast-weather/branch/main/graph/badge.svg)](https://codecov.io/gh/e7kim/forecast-weather)
 [![PyPI](https://img.shields.io/pypi/v/forecast-weather)](https://pypi.org/project/forecast-weather/)
+[![Docs](https://readthedocs.org/projects/forecast-weather/badge/?version=latest)](https://forecast-weather.readthedocs.io/en/latest/?badge=latest)
 
 # Overview
 `forecast-weather` is a library that allows a user to easily obtain weather data (temperatures, pressure, humidity, precipitation, wind, cloud coverage, etc.) across various locations and dates. The library will make calls to a public weather API and will organize the returned data for ease of use. Some extra functionality in consideration include some form of visual plot/graph generation.
 
 ## Install
 ```
 pip install forecast-weather
 ```
 
 ## API Key
 Go to [weatherapi.com](https://www.weatherapi.com/) to register an account for your free api key. Create a new file **./api_key** and paste your api key here.
 
 ## Usage
-```
+```python
 import forecast_weather as fw
 
 fw.show_current(location = "10027")
 fw.show_forecast(location = "10027", days = "2")
 current = fw.get_current(location = "10027")
 forecast = fw.get_forecast(location = "10027", days = "3")
 ```
 
+## Example
+Running the following code
+```python
+import forecast_weather as fw
+
+fw.show_current(location = "10027")
+```
+Outputs something like this to the console
+```
+Current weather at New York is: 
+Temperature: 68.0 F/ 20.0 C
+Condition: Overcast
+Wind speed: 2.2 mph
+Pressure: 1017.0 mb
+Precipitation: 0.0 in
+Humidity: 55%
+Cloud coverage: 100%
+UV: 4.0
+```
+
+## Demo
+
+![](https://raw.githubusercontent.com/e7kim/forecast-weather/main/docs/img/demo.gif)
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
```

### Comparing `forecast-weather-0.1.1/pyproject.toml` & `forecast-weather-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "forecast-weather"
 authors = [{name = "Eugene Kim", email = "ek3192@columbia.edu"}]
 description="This python library easily obtains weather data across various locations and dates."
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

