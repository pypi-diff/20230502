# Comparing `tmp/django-filter-autotools-0.0.3.tar.gz` & `tmp/django-filter-autotools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-filter-autotools-0.0.3.tar", last modified: Mon May  1 21:58:52 2023, max compression
+gzip compressed data, was "dist/django-filter-autotools-0.0.4.tar", last modified: Mon May  1 22:13:15 2023, max compression
```

## Comparing `django-filter-autotools-0.0.3.tar` & `django-filter-autotools-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-01 21:58:35.000000 django-filter-autotools-0.0.3/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      332 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4767 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.3/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4200 2023-05-01 21:58:23.000000 django-filter-autotools-0.0.3/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filters_autotools/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7354 2023-05-01 21:50:29.000000 django-filter-autotools-0.0.3/django_filters_autotools/mixins.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.3/django_filters_autotools/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4767 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/PKG-INFO
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-01 22:13:11.000000 django-filter-autotools-0.0.4/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      332 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4993 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.4/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4426 2023-05-01 22:13:05.000000 django-filter-autotools-0.0.4/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filters_autotools/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7354 2023-05-01 21:50:29.000000 django-filter-autotools-0.0.4/django_filters_autotools/mixins.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.4/django_filters_autotools/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4993 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/PKG-INFO
```

### Comparing `django-filter-autotools-0.0.3/setup.py` & `django-filter-autotools-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="django-filter-autotools", 
-    version="0.0.3", 
+    version="0.0.4", 
     description=(
         "Provides some mixins which allow automatic generation of filtersets with"
         "a list of lookups, including new lookups not registered into Django."
     ),
     author="Carlos Pastor",
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `django-filter-autotools-0.0.3/django_filter_autotools.egg-info/PKG-INFO` & `django-filter-autotools-0.0.4/django_filter_autotools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -84,14 +84,16 @@
 ## Integrating everything into DRF by default
 
 Complete example making available several lookups by default for all fields of type `CharField`:
 
 filters.py:
 ```python
 from django_filters import rest_framework as filters
+from django.db import models
+from django.core.validators import EMPTY_VALUES
 from django_filters_autotools.mixins import *
 
 
 class EmptyStringFilter(filters.BooleanFilter):
     def filter(self, qs, value):
         if value in EMPTY_VALUES:
             return qs
@@ -131,7 +133,12 @@
 REST_FRAMEWORK = {
     'DEFAULT_FILTER_BACKENDS': [
         'path.to.filters.MyFilterBackend',
     ],
 }
 ```
 
+## More info
+
+[PyPI project](https://pypi.org/project/django-filter-autotools/)
+[Github page](https://github.com/WhiteSage/django-filter-autotools)
+
```

### Comparing `django-filter-autotools-0.0.3/LICENSE` & `django-filter-autotools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.3/README.md` & `django-filter-autotools-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,16 @@
 ## Integrating everything into DRF by default
 
 Complete example making available several lookups by default for all fields of type `CharField`:
 
 filters.py:
 ```python
 from django_filters import rest_framework as filters
+from django.db import models
+from django.core.validators import EMPTY_VALUES
 from django_filters_autotools.mixins import *
 
 
 class EmptyStringFilter(filters.BooleanFilter):
     def filter(self, qs, value):
         if value in EMPTY_VALUES:
             return qs
@@ -113,8 +115,13 @@
 settings.py:
 ```python
 REST_FRAMEWORK = {
     'DEFAULT_FILTER_BACKENDS': [
         'path.to.filters.MyFilterBackend',
     ],
 }
-```
+```
+
+## More info
+
+[PyPI project](https://pypi.org/project/django-filter-autotools/)
+[Github page](https://github.com/WhiteSage/django-filter-autotools)
```

### Comparing `django-filter-autotools-0.0.3/django_filters_autotools/mixins.py` & `django-filter-autotools-0.0.4/django_filters_autotools/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.3/PKG-INFO` & `django-filter-autotools-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -84,14 +84,16 @@
 ## Integrating everything into DRF by default
 
 Complete example making available several lookups by default for all fields of type `CharField`:
 
 filters.py:
 ```python
 from django_filters import rest_framework as filters
+from django.db import models
+from django.core.validators import EMPTY_VALUES
 from django_filters_autotools.mixins import *
 
 
 class EmptyStringFilter(filters.BooleanFilter):
     def filter(self, qs, value):
         if value in EMPTY_VALUES:
             return qs
@@ -131,7 +133,12 @@
 REST_FRAMEWORK = {
     'DEFAULT_FILTER_BACKENDS': [
         'path.to.filters.MyFilterBackend',
     ],
 }
 ```
 
+## More info
+
+[PyPI project](https://pypi.org/project/django-filter-autotools/)
+[Github page](https://github.com/WhiteSage/django-filter-autotools)
+
```

