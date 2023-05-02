# Comparing `tmp/pyridy-1.0.0.tar.gz` & `tmp/pyridy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyridy-1.0.0.tar", max compression
+gzip compressed data, was "pyridy-1.0.1.tar", max compression
```

## Comparing `pyridy-1.0.0.tar` & `pyridy-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.0/LICENSE
--rw-r--r--   0        0        0      973 2023-03-09 16:44:31.553464 pyridy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.0/pyridy/__init__.py
--rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.0/pyridy/campaign.py
--rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.0/pyridy/config.py
--rw-r--r--   0        0        0    62789 2023-03-09 12:44:02.626960 pyridy-1.0.0/pyridy/file.py
--rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.0/pyridy/osm/__init__.py
--rw-r--r--   0        0        0    30563 2023-03-09 12:44:02.633958 pyridy-1.0.0/pyridy/osm/osm.py
--rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.0/pyridy/osm/utils/__init__.py
--rw-r--r--   0        0        0    12412 2023-03-09 16:42:58.458608 pyridy-1.0.0/pyridy/osm/utils/elements.py
--rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.0/pyridy/osm/utils/overpass.py
--rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.0/pyridy/osm/utils/query.py
--rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.0/pyridy/osm/utils/relation.py
--rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.0/pyridy/osm/utils/tools.py
--rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.0/pyridy/processing/__init__.py
--rw-r--r--   0        0        0    16957 2023-03-09 16:42:58.467625 pyridy-1.0.0/pyridy/processing/comfort.py
--rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.0/pyridy/processing/condition.py
--rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.0/pyridy/processing/excitation.py
--rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.0/pyridy/processing/processor.py
--rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.0/pyridy/utils/__init__.py
--rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.0/pyridy/utils/device.py
--rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.0/pyridy/utils/sensor.py
--rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.0/pyridy/utils/timeseries.py
--rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.0/pyridy/utils/tools.py
--rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.0/pyridy/widgets/__init__.py
--rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.0/pyridy/widgets/map.py
--rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.0/README.md
--rw-r--r--   0        0        0     3498 1970-01-01 00:00:00.000000 pyridy-1.0.0/setup.py
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 pyridy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11583 2023-02-14 16:19:37.926633 pyridy-1.0.1/LICENSE
+-rw-r--r--   0        0        0      971 2023-05-02 13:24:54.187899 pyridy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-02-14 16:19:37.951522 pyridy-1.0.1/pyridy/__init__.py
+-rw-r--r--   0        0        0    22145 2023-03-09 12:44:02.621957 pyridy-1.0.1/pyridy/campaign.py
+-rw-r--r--   0        0        0     2402 2023-02-14 16:19:37.954033 pyridy-1.0.1/pyridy/config.py
+-rw-r--r--   0        0        0    62789 2023-03-09 12:44:02.626960 pyridy-1.0.1/pyridy/file.py
+-rw-r--r--   0        0        0       22 2023-02-14 16:19:37.955033 pyridy-1.0.1/pyridy/osm/__init__.py
+-rw-r--r--   0        0        0    30598 2023-04-27 12:36:22.469380 pyridy-1.0.1/pyridy/osm/osm.py
+-rw-r--r--   0        0        0      121 2023-02-14 16:19:37.956033 pyridy-1.0.1/pyridy/osm/utils/__init__.py
+-rw-r--r--   0        0        0    12461 2023-04-27 12:36:22.472382 pyridy-1.0.1/pyridy/osm/utils/elements.py
+-rw-r--r--   0        0        0     6329 2023-03-09 12:44:02.642961 pyridy-1.0.1/pyridy/osm/utils/overpass.py
+-rw-r--r--   0        0        0     1173 2023-03-09 12:44:02.647963 pyridy-1.0.1/pyridy/osm/utils/query.py
+-rw-r--r--   0        0        0       60 2023-02-14 16:19:37.958033 pyridy-1.0.1/pyridy/osm/utils/relation.py
+-rw-r--r--   0        0        0    14525 2023-03-09 16:42:58.451384 pyridy-1.0.1/pyridy/osm/utils/tools.py
+-rw-r--r--   0        0        0      105 2023-02-14 16:19:37.959032 pyridy-1.0.1/pyridy/processing/__init__.py
+-rw-r--r--   0        0        0    16957 2023-03-09 16:42:58.467625 pyridy-1.0.1/pyridy/processing/comfort.py
+-rw-r--r--   0        0        0     6510 2023-03-09 12:44:02.659964 pyridy-1.0.1/pyridy/processing/condition.py
+-rw-r--r--   0        0        0     8805 2023-03-09 16:42:58.476180 pyridy-1.0.1/pyridy/processing/excitation.py
+-rw-r--r--   0        0        0      239 2023-02-14 16:19:37.961198 pyridy-1.0.1/pyridy/processing/processor.py
+-rw-r--r--   0        0        0       57 2023-02-14 16:19:37.962255 pyridy-1.0.1/pyridy/utils/__init__.py
+-rw-r--r--   0        0        0     3740 2023-02-14 16:19:37.962255 pyridy-1.0.1/pyridy/utils/device.py
+-rw-r--r--   0        0        0     2000 2023-02-14 16:19:37.963205 pyridy-1.0.1/pyridy/utils/sensor.py
+-rw-r--r--   0        0        0    46523 2023-03-09 16:42:58.434611 pyridy-1.0.1/pyridy/utils/timeseries.py
+-rw-r--r--   0        0        0     3890 2023-03-09 16:42:58.443203 pyridy-1.0.1/pyridy/utils/tools.py
+-rw-r--r--   0        0        0       18 2023-02-14 16:19:37.965205 pyridy-1.0.1/pyridy/widgets/__init__.py
+-rw-r--r--   0        0        0    12800 2023-02-14 16:19:37.965205 pyridy-1.0.1/pyridy/widgets/map.py
+-rw-r--r--   0        0        0     2332 2023-02-14 16:19:37.926633 pyridy-1.0.1/README.md
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 pyridy-1.0.1/setup.py
+-rw-r--r--   0        0        0     3626 1970-01-01 00:00:00.000000 pyridy-1.0.1/PKG-INFO
```

### Comparing `pyridy-1.0.0/LICENSE` & `pyridy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyproject.toml` & `pyridy-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyridy"
-version = "1.0.0"
+version = "1.0.1"
 description = "Support library for measurements made with the Ridy Android App"
 authors = ["Philipp Simon Leibner <philipp.leibner@ifs.rwth-aachen.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 classifiers = [
     "Topic :: Scientific/Engineering :: Information Analysis",
@@ -18,26 +18,26 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8, <3.11"
 pytest = "^7.1.1"
 numpy = "^1.21.5"
 requests = "^2.28.1"
-pandas = "^1.2.4"
+pandas = "^2.0.1"
 matplotlib = "^3.4.1"
 tqdm = "^4.60.0"
 overpy = "^0.6"
 geopy = "^2.1.0"
 scipy = "^1.6.3"
 pyproj = "^3.3.0"
 ipyleaflet = "^0.17.0"
-networkx = "^2.6.3"
+networkx = "^3.1"
 HeapDict = "^1.0.1"
 Shapely = "^1.8.1"
-requests-cache = "^0.9.5"
-rwthcolors = "^0.1.6"
+requests-cache = "^1.0.1"
+rwthcolors = "^0.2.3"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pyridy-1.0.0/pyridy/campaign.py` & `pyridy-1.0.1/pyridy/campaign.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/config.py` & `pyridy-1.0.1/pyridy/config.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/file.py` & `pyridy-1.0.1/pyridy/file.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/osm/osm.py` & `pyridy-1.0.1/pyridy/osm/osm.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,16 @@
         attempts: int
             Number of attempts
         overpass_instances: List[Overpass]
             A list of Overpass API instances
 
         Returns
         -------
-        Parsed result: Overp
+        Parsed result: Overpy.Result
+            Parsed result
 
         Raises:
         -------
         QueryToOverpassApiFailed
             Raised when query to overpass fails
         """
         if attempts is None:
```

### Comparing `pyridy-1.0.0/pyridy/osm/utils/elements.py` & `pyridy-1.0.1/pyridy/osm/utils/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         lat: float
             Latitude of node coordinate
         lon: float
             Longitude of node coordinate
         value:
             Node value
         f: RDYFile
+            Ridy File containing measurements
         proc: processor
             Postprocessing Processor used
         direction: str
             Axis that has been used
         color: str
             Node color. Defaults to None.
 
@@ -48,15 +49,15 @@
         self.color = '#CC071E' if not color else color
 
     def __repr__(self):
         return f'Result node at ({self.lon}, {self.lat} of value {self.value})'
 
 
 class OSMResultWay:
-    def __init(self, way, res: float = .5):
+    def __init__(self, way, res: float = .5):
         """
         Class representing an element of type way
 
         Parameters
         ----------
         way : overpy.Way
             OSM Way retrieved using Overpy
```

### Comparing `pyridy-1.0.0/pyridy/osm/utils/overpass.py` & `pyridy-1.0.1/pyridy/osm/utils/overpass.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/osm/utils/query.py` & `pyridy-1.0.1/pyridy/osm/utils/query.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/osm/utils/tools.py` & `pyridy-1.0.1/pyridy/osm/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/processing/comfort.py` & `pyridy-1.0.1/pyridy/processing/comfort.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/processing/condition.py` & `pyridy-1.0.1/pyridy/processing/condition.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/processing/excitation.py` & `pyridy-1.0.1/pyridy/processing/excitation.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/utils/device.py` & `pyridy-1.0.1/pyridy/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/utils/sensor.py` & `pyridy-1.0.1/pyridy/utils/sensor.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/utils/timeseries.py` & `pyridy-1.0.1/pyridy/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/utils/tools.py` & `pyridy-1.0.1/pyridy/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/pyridy/widgets/map.py` & `pyridy-1.0.1/pyridy/widgets/map.py`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/README.md` & `pyridy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyridy-1.0.0/setup.py` & `pyridy-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 
 install_requires = \
 ['HeapDict>=1.0.1,<2.0.0',
  'Shapely>=1.8.1,<2.0.0',
  'geopy>=2.1.0,<3.0.0',
  'ipyleaflet>=0.17.0,<0.18.0',
  'matplotlib>=3.4.1,<4.0.0',
- 'networkx>=2.6.3,<3.0.0',
+ 'networkx>=3.1,<4.0',
  'numpy>=1.21.5,<2.0.0',
  'overpy>=0.6,<0.7',
- 'pandas>=1.2.4,<2.0.0',
+ 'pandas>=2.0.1,<3.0.0',
  'pyproj>=3.3.0,<4.0.0',
  'pytest>=7.1.1,<8.0.0',
- 'requests-cache>=0.9.5,<0.10.0',
+ 'requests-cache>=1.0.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
- 'rwthcolors>=0.1.6,<0.2.0',
+ 'rwthcolors>=0.2.3,<0.3.0',
  'scipy>=1.6.3,<2.0.0',
  'tqdm>=4.60.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pyridy',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Support library for measurements made with the Ridy Android App',
     'long_description': '# PyRidy\n\n![alt text](assets/ic_launcher.png "PyRidy Logo")\n\nPython Support Library to import and process Ridy files\n\n### About Ridy\nRidy is an Android App to record sensor data for uses in science and engineering. The app is currently actively being \ndeveloped at the [Chair and Institute for Rail Vehicles and Transport Systems (IFS)](http://www.ifs.rwth-aachen.de/en/start/)\n\n<img src="assets/screenshot.png" alt="Ridy Screenshot" width="200"/>\n\nAt the institute Ridy is e.g. used for condition monitoring of railway tracks and several more use-cases are currently\nresearched upon.\nAmong other, Ridy can record:\n* Acceleration\n* Linear Acceleration (i.e., without g-Force)\n* Magnetic Field\n* Gyroscope\n* Orientation\n* GNSS Location (+ Android Raw GNSS Measurements)\n* Pressure, Humidity, Temperature, Ambient Light\n\nCompared to other existing apps Ridy can perform long measurements even in the background when the phone is locked.\nThe app supports two formats for data export, JSON and SQLITE. If you would like to use or try out the app please contact the\ndeveloper (see below) to get access.\n\n### About PyRidy\nPyRidy is the companion python library for the Ridy Android App. It provides easy access to the data no matter which\nrecording format was used. If pyridy is used, one does no longer need to manually write code to import the files.\n\nIn addition, pyridy provides several more features:\n* Automatic conversion of sensor data into objects and numpy arrays\n* Conversion of arrays to Pandas DataFrame objects\n* Time synchronization of individual files (e.g. from different phones)\n* Download of OSM Railway Data via the Overpass API\n* Plotting of GPS tracks onto a map using ipyleaflet\n\n### Documentation\n[PyRidy Documentation](https://pyridy.readthedocs.io/)\n#### Installation\n\nInstall using pip\n```python\n    pip install pyridy\n```\n\n#### Usage\n\nInformation and examples on how to use the library can be found in the [PyRidy documentation](https://pyridy.readthedocs.io/)\n\n### Creator\nPhilipp Leibner - philipp.leibner@ifs.rwth-aachen.de\n\n### Contributor\nDaniel Pujiula Buhl - daniel.pujiula@rwth-aachen.de\nSarra Bouchkati - sarra.bouchkati@rwth-aachen.de\n\n<div>  \n<a href="">\n    <img src="assets/ifs_logo_rgb.svg" alt="IFS Logo" width="400">\n  </a>\n</div>\n',
     'author': 'Philipp Simon Leibner',
     'author_email': 'philipp.leibner@ifs.rwth-aachen.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,45 +1,44 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['pyridy',
 'pyridy.osm', 'pyridy.osm.utils', 'pyridy.processing', 'pyridy.utils',
 'pyridy.widgets'] package_data = \ {'': ['*']} install_requires = \
 ['HeapDict>=1.0.1,<2.0.0', 'Shapely>=1.8.1,<2.0.0', 'geopy>=2.1.0,<3.0.0',
-'ipyleaflet>=0.17.0,<0.18.0', 'matplotlib>=3.4.1,<4.0.0',
-'networkx>=2.6.3,<3.0.0', 'numpy>=1.21.5,<2.0.0', 'overpy>=0.6,<0.7',
-'pandas>=1.2.4,<2.0.0', 'pyproj>=3.3.0,<4.0.0', 'pytest>=7.1.1,<8.0.0',
-'requests-cache>=0.9.5,<0.10.0', 'requests>=2.28.1,<3.0.0',
-'rwthcolors>=0.1.6,<0.2.0', 'scipy>=1.6.3,<2.0.0', 'tqdm>=4.60.0,<5.0.0']
-setup_kwargs = { 'name': 'pyridy', 'version': '1.0.0', 'description': 'Support
-library for measurements made with the Ridy Android App', 'long_description':
-'# PyRidy\n\n![alt text](assets/ic_launcher.png "PyRidy Logo")\n\nPython
-Support Library to import and process Ridy files\n\n### About Ridy\nRidy is an
-Android App to record sensor data for uses in science and engineering. The app
-is currently actively being \ndeveloped at the [Chair and Institute for Rail
-Vehicles and Transport Systems (IFS)](http://www.ifs.rwth-aachen.de/en/start/
-)\n\n[Ridy Screenshot]\n\nAt the institute Ridy is e.g. used for condition
-monitoring of railway tracks and several more use-cases are
-currently\nresearched upon.\nAmong other, Ridy can record:\n* Acceleration\n*
-Linear Acceleration (i.e., without g-Force)\n* Magnetic Field\n* Gyroscope\n*
-Orientation\n* GNSS Location (+ Android Raw GNSS Measurements)\n* Pressure,
-Humidity, Temperature, Ambient Light\n\nCompared to other existing apps Ridy
-can perform long measurements even in the background when the phone is
-locked.\nThe app supports two formats for data export, JSON and SQLITE. If you
-would like to use or try out the app please contact the\ndeveloper (see below)
-to get access.\n\n### About PyRidy\nPyRidy is the companion python library for
-the Ridy Android App. It provides easy access to the data no matter
-which\nrecording format was used. If pyridy is used, one does no longer need to
-manually write code to import the files.\n\nIn addition, pyridy provides
-several more features:\n* Automatic conversion of sensor data into objects and
-numpy arrays\n* Conversion of arrays to Pandas DataFrame objects\n* Time
-synchronization of individual files (e.g. from different phones)\n* Download of
-OSM Railway Data via the Overpass API\n* Plotting of GPS tracks onto a map
-using ipyleaflet\n\n### Documentation\n[PyRidy Documentation](https://
-pyridy.readthedocs.io/)\n#### Installation\n\nInstall using pip\n```python\n
-pip install pyridy\n```\n\n#### Usage\n\nInformation and examples on how to use
-the library can be found in the [PyRidy documentation](https://
-pyridy.readthedocs.io/)\n\n### Creator\nPhilipp Leibner -
+'ipyleaflet>=0.17.0,<0.18.0', 'matplotlib>=3.4.1,<4.0.0', 'networkx>=3.1,<4.0',
+'numpy>=1.21.5,<2.0.0', 'overpy>=0.6,<0.7', 'pandas>=2.0.1,<3.0.0',
+'pyproj>=3.3.0,<4.0.0', 'pytest>=7.1.1,<8.0.0', 'requests-cache>=1.0.1,<2.0.0',
+'requests>=2.28.1,<3.0.0', 'rwthcolors>=0.2.3,<0.3.0', 'scipy>=1.6.3,<2.0.0',
+'tqdm>=4.60.0,<5.0.0'] setup_kwargs = { 'name': 'pyridy', 'version': '1.0.1',
+'description': 'Support library for measurements made with the Ridy Android
+App', 'long_description': '# PyRidy\n\n![alt text](assets/ic_launcher.png
+"PyRidy Logo")\n\nPython Support Library to import and process Ridy
+files\n\n### About Ridy\nRidy is an Android App to record sensor data for uses
+in science and engineering. The app is currently actively being \ndeveloped at
+the [Chair and Institute for Rail Vehicles and Transport Systems (IFS)](http://
+www.ifs.rwth-aachen.de/en/start/)\n\n[Ridy Screenshot]\n\nAt the institute Ridy
+is e.g. used for condition monitoring of railway tracks and several more use-
+cases are currently\nresearched upon.\nAmong other, Ridy can record:\n*
+Acceleration\n* Linear Acceleration (i.e., without g-Force)\n* Magnetic
+Field\n* Gyroscope\n* Orientation\n* GNSS Location (+ Android Raw GNSS
+Measurements)\n* Pressure, Humidity, Temperature, Ambient Light\n\nCompared to
+other existing apps Ridy can perform long measurements even in the background
+when the phone is locked.\nThe app supports two formats for data export, JSON
+and SQLITE. If you would like to use or try out the app please contact
+the\ndeveloper (see below) to get access.\n\n### About PyRidy\nPyRidy is the
+companion python library for the Ridy Android App. It provides easy access to
+the data no matter which\nrecording format was used. If pyridy is used, one
+does no longer need to manually write code to import the files.\n\nIn addition,
+pyridy provides several more features:\n* Automatic conversion of sensor data
+into objects and numpy arrays\n* Conversion of arrays to Pandas DataFrame
+objects\n* Time synchronization of individual files (e.g. from different
+phones)\n* Download of OSM Railway Data via the Overpass API\n* Plotting of GPS
+tracks onto a map using ipyleaflet\n\n### Documentation\n[PyRidy Documentation]
+(https://pyridy.readthedocs.io/)\n#### Installation\n\nInstall using
+pip\n```python\n pip install pyridy\n```\n\n#### Usage\n\nInformation and
+examples on how to use the library can be found in the [PyRidy documentation]
+(https://pyridy.readthedocs.io/)\n\n### Creator\nPhilipp Leibner -
 philipp.leibner@ifs.rwth-aachen.de\n\n### Contributor\nDaniel Pujiula Buhl -
 daniel.pujiula@rwth-aachen.de\nSarra Bouchkati - sarra.bouchkati@rwth-
 aachen.de\n\n
 \n\n [IFS Logo]\n\n
 \n', 'author': 'Philipp Simon Leibner', 'author_email':
 'philipp.leibner@ifs.rwth-aachen.de', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
```

### Comparing `pyridy-1.0.0/PKG-INFO` & `pyridy-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyridy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Support library for measurements made with the Ridy Android App
 License: Apache-2.0
 Keywords: signal processing,ridy,android
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Science/Research
@@ -15,23 +15,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: HeapDict (>=1.0.1,<2.0.0)
 Requires-Dist: Shapely (>=1.8.1,<2.0.0)
 Requires-Dist: geopy (>=2.1.0,<3.0.0)
 Requires-Dist: ipyleaflet (>=0.17.0,<0.18.0)
 Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
-Requires-Dist: networkx (>=2.6.3,<3.0.0)
+Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.21.5,<2.0.0)
 Requires-Dist: overpy (>=0.6,<0.7)
-Requires-Dist: pandas (>=1.2.4,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyproj (>=3.3.0,<4.0.0)
 Requires-Dist: pytest (>=7.1.1,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: requests-cache (>=0.9.5,<0.10.0)
-Requires-Dist: rwthcolors (>=0.1.6,<0.2.0)
+Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
+Requires-Dist: rwthcolors (>=0.2.3,<0.3.0)
 Requires-Dist: scipy (>=1.6.3,<2.0.0)
 Requires-Dist: tqdm (>=4.60.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # PyRidy
 
 ![alt text](assets/ic_launcher.png "PyRidy Logo")
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pyridy Version: 1.0.0 Summary: Support library for
+Metadata-Version: 2.1 Name: pyridy Version: 1.0.1 Summary: Support library for
 measurements made with the Ridy Android App License: Apache-2.0 Keywords:
 signal processing,ridy,android Author: Philipp Simon Leibner Author-email:
 philipp.leibner@ifs.rwth-aachen.de Requires-Python: >=3.8,<3.11 Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Information Analysis Requires-
 Dist: HeapDict (>=1.0.1,<2.0.0) Requires-Dist: Shapely (>=1.8.1,<2.0.0)
 Requires-Dist: geopy (>=2.1.0,<3.0.0) Requires-Dist: ipyleaflet
 (>=0.17.0,<0.18.0) Requires-Dist: matplotlib (>=3.4.1,<4.0.0) Requires-Dist:
-networkx (>=2.6.3,<3.0.0) Requires-Dist: numpy (>=1.21.5,<2.0.0) Requires-Dist:
-overpy (>=0.6,<0.7) Requires-Dist: pandas (>=1.2.4,<2.0.0) Requires-Dist:
+networkx (>=3.1,<4.0) Requires-Dist: numpy (>=1.21.5,<2.0.0) Requires-Dist:
+overpy (>=0.6,<0.7) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist:
 pyproj (>=3.3.0,<4.0.0) Requires-Dist: pytest (>=7.1.1,<8.0.0) Requires-Dist:
-requests (>=2.28.1,<3.0.0) Requires-Dist: requests-cache (>=0.9.5,<0.10.0)
-Requires-Dist: rwthcolors (>=0.1.6,<0.2.0) Requires-Dist: scipy
+requests (>=2.28.1,<3.0.0) Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
+Requires-Dist: rwthcolors (>=0.2.3,<0.3.0) Requires-Dist: scipy
 (>=1.6.3,<2.0.0) Requires-Dist: tqdm (>=4.60.0,<5.0.0) Description-Content-
 Type: text/markdown # PyRidy ![alt text](assets/ic_launcher.png "PyRidy Logo")
 Python Support Library to import and process Ridy files ### About Ridy Ridy is
 an Android App to record sensor data for uses in science and engineering. The
 app is currently actively being developed at the [Chair and Institute for Rail
 Vehicles and Transport Systems (IFS)](http://www.ifs.rwth-aachen.de/en/start/)
 [Ridy Screenshot] At the institute Ridy is e.g. used for condition monitoring
```

