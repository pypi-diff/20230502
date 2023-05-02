# Comparing `tmp/django-more-admin-filters-1.6.tar.gz` & `tmp/django-more-admin-filters-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-more-admin-filters-1.6.tar", last modified: Fri Apr  7 20:38:06 2023, max compression
+gzip compressed data, was "django-more-admin-filters-1.7.tar", last modified: Tue May  2 14:06:43 2023, max compression
```

## Comparing `django-more-admin-filters-1.6.tar` & `django-more-admin-filters-1.7.tar`

### file list

```diff
@@ -1,23 +1,44 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2020-09-04 13:10:12.000000 django-more-admin-filters-1.6/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)       84 2020-09-05 09:10:25.000000 django-more-admin-filters-1.6/MANIFEST.in
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4473 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3127 2023-04-07 13:11:30.000000 django-more-admin-filters-1.6/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.612347 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4473 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      596 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       17 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       19 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2020-09-05 09:15:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/zip-safe
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/more_admin_filters/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      284 2023-02-12 20:36:36.000000 django-more-admin-filters-1.6/more_admin_filters/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      661 2023-04-07 20:37:08.000000 django-more-admin-filters-1.6/more_admin_filters/__version__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      116 2021-07-16 10:17:35.000000 django-more-admin-filters-1.6/more_admin_filters/apps.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14116 2023-02-12 20:36:36.000000 django-more-admin-filters-1.6/more_admin_filters/filters.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.612347 django-more-admin-filters-1.6/more_admin_filters/templates/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      962 2020-09-05 11:29:15.000000 django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/dropdownfilter.html
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1909 2020-09-05 11:29:18.000000 django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2252 2023-04-07 13:55:38.000000 django-more-admin-filters-1.6/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2020-09-04 13:10:12.000000 django-more-admin-filters-1.7/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       84 2020-09-05 09:10:25.000000 django-more-admin-filters-1.7/MANIFEST.in
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4541 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3156 2023-05-02 13:54:41.000000 django-more-admin-filters-1.7/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.094709 django-more-admin-filters-1.7/django_more_admin_filters.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4541 2023-05-02 14:06:43.000000 django-more-admin-filters-1.7/django_more_admin_filters.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1083 2023-05-02 14:06:43.000000 django-more-admin-filters-1.7/django_more_admin_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-05-02 14:06:43.000000 django-more-admin-filters-1.7/django_more_admin_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       17 2023-05-02 14:06:43.000000 django-more-admin-filters-1.7/django_more_admin_filters.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       36 2023-05-02 14:06:43.000000 django-more-admin-filters-1.7/django_more_admin_filters.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2020-09-05 09:15:06.000000 django-more-admin-filters-1.7/django_more_admin_filters.egg-info/zip-safe
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.094709 django-more-admin-filters-1.7/more_admin_filters/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      284 2023-02-12 20:36:36.000000 django-more-admin-filters-1.7/more_admin_filters/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      661 2023-05-02 13:54:14.000000 django-more-admin-filters-1.7/more_admin_filters/__version__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      116 2021-07-16 10:17:35.000000 django-more-admin-filters-1.7/more_admin_filters/apps.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14116 2023-02-12 20:36:36.000000 django-more-admin-filters-1.7/more_admin_filters/filters.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.090709 django-more-admin-filters-1.7/more_admin_filters/templates/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.094709 django-more-admin-filters-1.7/more_admin_filters/templates/more_admin_filters/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      962 2020-09-05 11:29:15.000000 django-more-admin-filters-1.7/more_admin_filters/templates/more_admin_filters/dropdownfilter.html
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1909 2020-09-05 11:29:18.000000 django-more-admin-filters-1.7/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2310 2023-05-02 14:06:33.000000 django-more-admin-filters-1.7/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.090709 django-more-admin-filters-1.7/tests/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/tests/testapp/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-09-04 13:08:44.000000 django-more-admin-filters-1.7/tests/testapp/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1476 2020-09-05 21:32:53.000000 django-more-admin-filters-1.7/tests/testapp/admin.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      114 2020-09-04 20:29:57.000000 django-more-admin-filters-1.7/tests/testapp/apps.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/tests/testapp/management/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-09-04 13:08:44.000000 django-more-admin-filters-1.7/tests/testapp/management/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/tests/testapp/management/commands/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-09-04 13:08:44.000000 django-more-admin-filters-1.7/tests/testapp/management/commands/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1646 2020-09-05 21:29:45.000000 django-more-admin-filters-1.7/tests/testapp/management/commands/createtestdata.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/tests/testapp/migrations/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2052 2020-09-05 21:10:17.000000 django-more-admin-filters-1.7/tests/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2020-09-04 20:32:06.000000 django-more-admin-filters-1.7/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1965 2020-09-05 21:10:04.000000 django-more-admin-filters-1.7/tests/testapp/models.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3272 2021-07-16 10:17:44.000000 django-more-admin-filters-1.7/tests/testapp/settings.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-02 14:06:43.098708 django-more-admin-filters-1.7/tests/testapp/tests/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2020-09-04 13:08:44.000000 django-more-admin-filters-1.7/tests/testapp/tests/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2260 2020-09-05 21:31:47.000000 django-more-admin-filters-1.7/tests/testapp/tests/test_filters.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7759 2023-04-07 20:28:06.000000 django-more-admin-filters-1.7/tests/testapp/tests/test_live_filters.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      757 2023-02-12 20:36:36.000000 django-more-admin-filters-1.7/tests/testapp/urls.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      391 2020-09-04 13:08:44.000000 django-more-admin-filters-1.7/tests/testapp/wsgi.py
```

### Comparing `django-more-admin-filters-1.6/LICENSE` & `django-more-admin-filters-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.6/PKG-INFO` & `django-more-admin-filters-1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-more-admin-filters
-Version: 1.6
+Version: 1.7
 Summary: Additional filters for django-admin.
 Home-page: https://github.com/thomst/django-more-admin-filters
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -43,17 +44,17 @@
     :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
     :alt: coveralls badge
 
 .. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
    :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
    :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
 
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
 Django-more-admin-filters is a collection of django admin filters with a focus
 on filters using dropdown widgets, multiple choice filters and filters working
 with annotated attributes.
```

### Comparing `django-more-admin-filters-1.6/README.rst` & `django-more-admin-filters-1.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
     :alt: coveralls badge
 
 .. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
    :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
    :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
 
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
 Django-more-admin-filters is a collection of django admin filters with a focus
 on filters using dropdown widgets, multiple choice filters and filters working
 with annotated attributes.
```

### Comparing `django-more-admin-filters-1.6/django_more_admin_filters.egg-info/PKG-INFO` & `django-more-admin-filters-1.7/django_more_admin_filters.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-more-admin-filters
-Version: 1.6
+Version: 1.7
 Summary: Additional filters for django-admin.
 Home-page: https://github.com/thomst/django-more-admin-filters
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -43,17 +44,17 @@
     :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
     :alt: coveralls badge
 
 .. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
    :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
    :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
 
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
 Django-more-admin-filters is a collection of django admin filters with a focus
 on filters using dropdown widgets, multiple choice filters and filters working
 with annotated attributes.
```

### Comparing `django-more-admin-filters-1.6/more_admin_filters/__version__.py` & `django-more-admin-filters-1.7/more_admin_filters/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 """
 
-__version__ = "1.6"
+__version__ = "1.7"
```

### Comparing `django-more-admin-filters-1.6/more_admin_filters/filters.py` & `django-more-admin-filters-1.7/more_admin_filters/filters.py`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/dropdownfilter.html` & `django-more-admin-filters-1.7/more_admin_filters/templates/more_admin_filters/dropdownfilter.html`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html` & `django-more-admin-filters-1.7/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.6/setup.py` & `django-more-admin-filters-1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import os
 from setuptools import setup
-from setuptools import find_packages
+from setuptools import find_namespace_packages
 from pathlib import Path
 
 
 def version():
     """Get the local package version."""
     namespace = {}
     path = Path("more_admin_filters", "__version__.py")
@@ -35,28 +35,29 @@
     description="Additional filters for django-admin.",
     long_description=read("README.rst"),
     author="Thomas Leichtfuß",
     author_email="thomas.leichtfuss@posteo.de",
     url="https://github.com/thomst/django-more-admin-filters",
     license="BSD License",
     platforms=["OS Independent"],
-    packages=find_packages(exclude=["tests"]),
+    packages=find_namespace_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
-        "Django>=2.2,<4.2",
+        "Django>=2.2,<5.0",
     ],
     classifiers=[
         dev_status,
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

