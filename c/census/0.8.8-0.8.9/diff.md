# Comparing `tmp/census-0.8.8.tar.gz` & `tmp/census-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/census-0.8.8.tar", last modified: Thu Nov 29 04:54:51 2018, max compression
+gzip compressed data, was "dist/census-0.8.9.tar", last modified: Thu Nov 29 15:42:31 2018, max compression
```

## Comparing `census-0.8.8.tar` & `census-0.8.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 04:54:51.000000 census-0.8.8/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 04:54:51.000000 census-0.8.8/census/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 04:54:51.000000 census-0.8.8/census/tests/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-11-29 04:54:11.000000 census-0.8.8/census/tests/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9093 2018-11-29 04:54:11.000000 census-0.8.8/census/tests/test_census.py
--rw-r--r--   0 travis    (2000) travis    (2000)      106 2018-11-29 04:54:11.000000 census-0.8.8/census/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    16576 2018-11-29 04:54:11.000000 census-0.8.8/census/core.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 04:54:51.000000 census-0.8.8/census.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     7768 2018-11-29 04:54:51.000000 census-0.8.8/census.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      285 2018-11-29 04:54:51.000000 census-0.8.8/census.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-11-29 04:54:51.000000 census-0.8.8/census.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       80 2018-11-29 04:54:51.000000 census-0.8.8/census.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        7 2018-11-29 04:54:51.000000 census-0.8.8/census.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     1541 2018-11-29 04:54:11.000000 census-0.8.8/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)       26 2018-11-29 04:54:11.000000 census-0.8.8/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     5719 2018-11-29 04:54:11.000000 census-0.8.8/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       67 2018-11-29 04:54:51.000000 census-0.8.8/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)      975 2018-11-29 04:54:11.000000 census-0.8.8/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7768 2018-11-29 04:54:51.000000 census-0.8.8/PKG-INFO
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 15:42:31.000000 census-0.8.9/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 15:42:31.000000 census-0.8.9/census/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 15:42:31.000000 census-0.8.9/census/tests/
+-rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-11-29 15:41:40.000000 census-0.8.9/census/tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9093 2018-11-29 15:41:40.000000 census-0.8.9/census/tests/test_census.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      106 2018-11-29 15:41:40.000000 census-0.8.9/census/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    16588 2018-11-29 15:41:40.000000 census-0.8.9/census/core.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-11-29 15:42:31.000000 census-0.8.9/census.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     7768 2018-11-29 15:42:31.000000 census-0.8.9/census.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      285 2018-11-29 15:42:31.000000 census-0.8.9/census.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-11-29 15:42:31.000000 census-0.8.9/census.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       80 2018-11-29 15:42:31.000000 census-0.8.9/census.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        7 2018-11-29 15:42:31.000000 census-0.8.9/census.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)     1541 2018-11-29 15:41:40.000000 census-0.8.9/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)       26 2018-11-29 15:41:40.000000 census-0.8.9/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     5719 2018-11-29 15:41:40.000000 census-0.8.9/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)       67 2018-11-29 15:42:31.000000 census-0.8.9/setup.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)      975 2018-11-29 15:41:40.000000 census-0.8.9/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7768 2018-11-29 15:42:31.000000 census-0.8.9/PKG-INFO
```

### Comparing `census-0.8.8/census/tests/test_census.py` & `census-0.8.9/census/tests/test_census.py`

 * *Files identical despite different names*

### Comparing `census-0.8.8/census/core.py` & `census-0.8.9/census/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,32 +340,32 @@
 class ACS3DpClient(ACS3Client):
 
     dataset = 'acs3/profile'
 
 
 class ACS1Client(ACSClient):
 
-    default_year = 2016
+    default_year = 2017
     dataset = 'acs1'
 
-    years = (2016, 2015, 2014, 2013, 2012, 2011)
+    years = (2017, 2016, 2015, 2014, 2013, 2012, 2011)
 
     @supported_years()
     def state_county_subdivision(self, fields, state_fips,
                                  county_fips, subdiv_fips, **kwargs):
         return self.get(fields, geo={
             'for': 'county subdivision:{}'.format(subdiv_fips),
             'in': 'state:{} county:{}'.format(state_fips, county_fips),
         }, **kwargs)
 
 class ACS1DpClient(ACS1Client):
 
     dataset = 'acs1/profile'
 
-    years = (2016, 2015, 2014, 2013, 2012)
+    years = (2017, 2016, 2015, 2014, 2013, 2012)
 
 
 class SF1Client(Client):
 
     default_year = 2010
     dataset = 'sf1'
```

### Comparing `census-0.8.8/census.egg-info/PKG-INFO` & `census-0.8.9/census.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: census
-Version: 0.8.8
+Version: 0.8.9
 Summary: A wrapper for the US Census Bureau's API
 Home-page: http://github.com/datamade/census
 Author: Jeremy Carbaugh
 Author-email: jcarbaugh@sunlightfoundation.com
 Maintainer: Forest Gregg
 Maintainer-email: fgregg@gmail.com
 License: BSD
```

### Comparing `census-0.8.8/LICENSE` & `census-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `census-0.8.8/README.rst` & `census-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `census-0.8.8/setup.py` & `census-0.8.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 long_description = open('README.rst').read()
 
 setup(
     name="census",
-    version="0.8.8",
+    version="0.8.9",
     py_modules=['census'],
     author="Jeremy Carbaugh",
     author_email='jcarbaugh@sunlightfoundation.com',
     maintainer='Forest Gregg',
     maintainer_email='fgregg@gmail.com',
     license="BSD",
     url="http://github.com/datamade/census",
```

### Comparing `census-0.8.8/PKG-INFO` & `census-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: census
-Version: 0.8.8
+Version: 0.8.9
 Summary: A wrapper for the US Census Bureau's API
 Home-page: http://github.com/datamade/census
 Author: Jeremy Carbaugh
 Author-email: jcarbaugh@sunlightfoundation.com
 Maintainer: Forest Gregg
 Maintainer-email: fgregg@gmail.com
 License: BSD
```

