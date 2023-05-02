# Comparing `tmp/django-filter-autotools-0.0.4.tar.gz` & `tmp/django-filter-autotools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-filter-autotools-0.0.4.tar", last modified: Mon May  1 22:13:15 2023, max compression
+gzip compressed data, was "dist/django-filter-autotools-0.0.5.tar", last modified: Tue May  2 09:36:06 2023, max compression
```

## Comparing `django-filter-autotools-0.0.4.tar` & `django-filter-autotools-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-01 22:13:11.000000 django-filter-autotools-0.0.4/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      332 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4993 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filter_autotools.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.4/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4426 2023-05-01 22:13:05.000000 django-filter-autotools-0.0.4/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/django_filters_autotools/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7354 2023-05-01 21:50:29.000000 django-filter-autotools-0.0.4/django_filters_autotools/mixins.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.4/django_filters_autotools/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4993 2023-05-01 22:13:15.000000 django-filter-autotools-0.0.4/PKG-INFO
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-02 09:32:26.000000 django-filter-autotools-0.0.5/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      332 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5095 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.5/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4528 2023-05-02 09:31:40.000000 django-filter-autotools-0.0.5/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filters_autotools/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7459 2023-05-02 09:31:25.000000 django-filter-autotools-0.0.5/django_filters_autotools/mixins.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.5/django_filters_autotools/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5095 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/PKG-INFO
```

### Comparing `django-filter-autotools-0.0.4/setup.py` & `django-filter-autotools-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="django-filter-autotools", 
-    version="0.0.4", 
+    version="0.0.5", 
     description=(
         "Provides some mixins which allow automatic generation of filtersets with"
         "a list of lookups, including new lookups not registered into Django."
     ),
     author="Carlos Pastor",
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `django-filter-autotools-0.0.4/django_filter_autotools.egg-info/PKG-INFO` & `django-filter-autotools-0.0.5/django_filter_autotools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -14,18 +14,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-filter-autotools
 
 ## Installation
 
+Either using pip
+
 ```bash
 python -m pip install django-filter-autotools
 ```
 
+or directly copying the file `django_filters_autotools/mixins.py` into your project.
+
+
 ## DefaultLookupsMixin
 
 By default django-filter FilterSet class will only generate `exact` lookups if given a list of fields. This mixin can be used to customize this behaviour:
 ```python
 class MyFilterSet(DefaultLookupsMixin, FilterSet):
 
     DEFAULT_LOOKUPS = {
@@ -59,27 +64,27 @@
         'isempty': {
             'behaves_like': 'isnull',
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
-            'replace_lookup': 'icontains',
+            'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
         }
     }
 ```
 
 Under the hood this works by replacing the lookup with the one specified in the `behaves_like` key, running the filter creation algorithm and then patching the filters if necessary. This way any transformer or any extra lookups registered into Django will also be available.
 
-PSEUDO_LOOKUPS is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
+`PSEUDO_LOOKUPS` is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
 
 * `behaves_like`: should be a lookup registered in Django with similar semantics.
 * `filter_class`: filter class to be used for this lookup. If not specified or None, the one chosen django-filters for the `behaves_like` lookup will be used. Note these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
-* `replace_lookup`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
+* `replace_with`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
 * `extra`: if present the object returned from applying this function to the field will be merged into the filter class kwargs.
 
 Note that more fine-tuning by overriding the `filter_for_pseudolookup` class method (for example, choosing the filter class based on the field type).
 
 
 ## Integrating everything into DRF by default
 
@@ -110,15 +115,15 @@
         'isempty': {
             'behaves_like': 'isnull',
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
-            'replace_lookup': 'icontains',
+            'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
         }
     }
 
     DEFAULT_LOOKUPS = {
         models.CharField:      [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
     }
@@ -136,9 +141,10 @@
     ],
 }
 ```
 
 ## More info
 
 [PyPI project](https://pypi.org/project/django-filter-autotools/)
+
 [Github page](https://github.com/WhiteSage/django-filter-autotools)
```

### Comparing `django-filter-autotools-0.0.4/LICENSE` & `django-filter-autotools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.4/README.md` & `django-filter-autotools-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # django-filter-autotools
 
 ## Installation
 
+Either using pip
+
 ```bash
 python -m pip install django-filter-autotools
 ```
 
+or directly copying the file `django_filters_autotools/mixins.py` into your project.
+
+
 ## DefaultLookupsMixin
 
 By default django-filter FilterSet class will only generate `exact` lookups if given a list of fields. This mixin can be used to customize this behaviour:
 ```python
 class MyFilterSet(DefaultLookupsMixin, FilterSet):
 
     DEFAULT_LOOKUPS = {
@@ -43,27 +48,27 @@
         'isempty': {
             'behaves_like': 'isnull',
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
-            'replace_lookup': 'icontains',
+            'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
         }
     }
 ```
 
 Under the hood this works by replacing the lookup with the one specified in the `behaves_like` key, running the filter creation algorithm and then patching the filters if necessary. This way any transformer or any extra lookups registered into Django will also be available.
 
-PSEUDO_LOOKUPS is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
+`PSEUDO_LOOKUPS` is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
 
 * `behaves_like`: should be a lookup registered in Django with similar semantics.
 * `filter_class`: filter class to be used for this lookup. If not specified or None, the one chosen django-filters for the `behaves_like` lookup will be used. Note these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
-* `replace_lookup`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
+* `replace_with`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
 * `extra`: if present the object returned from applying this function to the field will be merged into the filter class kwargs.
 
 Note that more fine-tuning by overriding the `filter_for_pseudolookup` class method (for example, choosing the filter class based on the field type).
 
 
 ## Integrating everything into DRF by default
 
@@ -94,15 +99,15 @@
         'isempty': {
             'behaves_like': 'isnull',
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
-            'replace_lookup': 'icontains',
+            'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
         }
     }
 
     DEFAULT_LOOKUPS = {
         models.CharField:      [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
     }
@@ -120,8 +125,9 @@
     ],
 }
 ```
 
 ## More info
 
 [PyPI project](https://pypi.org/project/django-filter-autotools/)
+
 [Github page](https://github.com/WhiteSage/django-filter-autotools)
```

### Comparing `django-filter-autotools-0.0.4/django_filters_autotools/mixins.py` & `django-filter-autotools-0.0.5/django_filters_autotools/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django_filters.conf import settings as django_filter_settings
 from django_filters.utils import resolve_field as django_filter_resolve_field
 from django_filters.utils import get_model_field, try_dbfield
 from django.db import models
 from django.db.models.fields.related import (ManyToManyRel, ManyToOneRel, OneToOneRel)
 from django.core.validators import EMPTY_VALUES
+from django.db.models.constants import LOOKUP_SEP
 
 
 
 class DefaultLookupsMixin():
     DEFAULT_LOOKUPS = {
         models.AutoField:                   None,
         models.CharField:                   None,
@@ -88,15 +89,15 @@
 
     @classmethod
     def filter_for_pseudolookup(cls, field, lookup_type):
         """
         Override this method to provide custom lookups.
         By default it returns the class specified in 'filter_class' if not None.
         If None was specified, it returns the class django-filters' would use.
-        If 'replace_lookup' is set, patches the class to receive this lookup 
+        If 'replace_with' is set, patches the class to receive this lookup 
         instead of the actual one.
 
         Args:
             field: resulting field from applying all transforms to the LHS
             lookup_type: lookup excluding any transforms
 
         Return value:
@@ -110,16 +111,16 @@
         else:
             filter_class, df_params = super().filter_for_lookup(field, behaves_like)
 
             df_params.update(params)
             params = df_params
 
         # Patch the class if we have to so that it receives the new lookup
-        if cls.PSEUDO_LOOKUPS[lookup_type].get('replace_lookup', None):
-            filter_class = cls.patch_filter_class(filter_class, lookup_type, cls.PSEUDO_LOOKUPS[lookup_type]['replace_lookup'])
+        if cls.PSEUDO_LOOKUPS[lookup_type].get('replace_with', None):
+            filter_class = cls.patch_filter_class(filter_class, lookup_type, cls.PSEUDO_LOOKUPS[lookup_type]['replace_with'])
 
         return filter_class, params
 
                 
 
     @classmethod
     def filter_for_lookup(cls, field, lookup_type):
@@ -146,16 +147,17 @@
         For pseudo-lookups the underlying Django machinery will fail,
         therefore we will swap them for a Django-compliant one with the
         same semantics, and then swap it back
         """
         PSEUDO_LOOKUPS = getattr(cls, 'PSEUDO_LOOKUPS', [])
 
         pseudo = None
+        lookup_expr_parts = lookup_expr.split(LOOKUP_SEP)
         for lookup in PSEUDO_LOOKUPS:
-            if lookup_expr.endswith(lookup):
+            if lookup_expr_parts[-1] == lookup:
                 pseudo = lookup
                 lookup_expr = lookup_expr[:-len(lookup)] + PSEUDO_LOOKUPS[lookup]['behaves_like']
                 break
 
         field, lookup_type = django_filter_resolve_field(field, lookup_expr)
 
         if pseudo:
```

### Comparing `django-filter-autotools-0.0.4/PKG-INFO` & `django-filter-autotools-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -14,18 +14,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-filter-autotools
 
 ## Installation
 
+Either using pip
+
 ```bash
 python -m pip install django-filter-autotools
 ```
 
+or directly copying the file `django_filters_autotools/mixins.py` into your project.
+
+
 ## DefaultLookupsMixin
 
 By default django-filter FilterSet class will only generate `exact` lookups if given a list of fields. This mixin can be used to customize this behaviour:
 ```python
 class MyFilterSet(DefaultLookupsMixin, FilterSet):
 
     DEFAULT_LOOKUPS = {
@@ -59,27 +64,27 @@
         'isempty': {
             'behaves_like': 'isnull',
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
-            'replace_lookup': 'icontains',
+            'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
         }
     }
 ```
 
 Under the hood this works by replacing the lookup with the one specified in the `behaves_like` key, running the filter creation algorithm and then patching the filters if necessary. This way any transformer or any extra lookups registered into Django will also be available.
 
-PSEUDO_LOOKUPS is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
+`PSEUDO_LOOKUPS` is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
 
 * `behaves_like`: should be a lookup registered in Django with similar semantics.
 * `filter_class`: filter class to be used for this lookup. If not specified or None, the one chosen django-filters for the `behaves_like` lookup will be used. Note these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
-* `replace_lookup`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
+* `replace_with`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
 * `extra`: if present the object returned from applying this function to the field will be merged into the filter class kwargs.
 
 Note that more fine-tuning by overriding the `filter_for_pseudolookup` class method (for example, choosing the filter class based on the field type).
 
 
 ## Integrating everything into DRF by default
 
@@ -110,15 +115,15 @@
         'isempty': {
             'behaves_like': 'isnull',
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
-            'replace_lookup': 'icontains',
+            'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
         }
     }
 
     DEFAULT_LOOKUPS = {
         models.CharField:      [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
     }
@@ -136,9 +141,10 @@
     ],
 }
 ```
 
 ## More info
 
 [PyPI project](https://pypi.org/project/django-filter-autotools/)
+
 [Github page](https://github.com/WhiteSage/django-filter-autotools)
```

