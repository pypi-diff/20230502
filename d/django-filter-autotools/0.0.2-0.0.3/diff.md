# Comparing `tmp/django-filter-autotools-0.0.2.tar.gz` & `tmp/django-filter-autotools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-filter-autotools-0.0.2.tar", last modified: Mon May  1 20:56:38 2023, max compression
+gzip compressed data, was "dist/django-filter-autotools-0.0.3.tar", last modified: Mon May  1 21:58:52 2023, max compression
```

## Comparing `django-filter-autotools-0.0.2.tar` & `django-filter-autotools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-01 20:56:35.000000 django-filter-autotools-0.0.2/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      302 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      622 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/django_filter_autotools.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.2/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       55 2023-05-01 20:50:35.000000 django-filter-autotools-0.0.2/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/autotools/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6600 2023-05-01 17:15:11.000000 django-filter-autotools-0.0.2/autotools/mixins.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.2/autotools/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      622 2023-05-01 20:56:38.000000 django-filter-autotools-0.0.2/PKG-INFO
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-01 21:58:35.000000 django-filter-autotools-0.0.3/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      332 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4767 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filter_autotools.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.3/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4200 2023-05-01 21:58:23.000000 django-filter-autotools-0.0.3/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/django_filters_autotools/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7354 2023-05-01 21:50:29.000000 django-filter-autotools-0.0.3/django_filters_autotools/mixins.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.3/django_filters_autotools/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4767 2023-05-01 21:58:52.000000 django-filter-autotools-0.0.3/PKG-INFO
```

### Comparing `django-filter-autotools-0.0.2/setup.py` & `django-filter-autotools-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="django-filter-autotools", 
-    version="0.0.2", 
+    version="0.0.3", 
     description=(
         "Provides some mixins which allow automatic generation of filtersets with"
         "a list of lookups, including new lookups not registered into Django."
     ),
     author="Carlos Pastor",
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `django-filter-autotools-0.0.2/LICENSE` & `django-filter-autotools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.2/autotools/mixins.py` & `django-filter-autotools-0.0.3/django_filters_autotools/mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,56 +61,78 @@
               (not isinstance(user_fields, dict) or not user_fields[field_name]):
                 fields[field_name] = data
 
         return fields
 
 
 class PseudoLookupsMixin():
-    pseudo_lookups = {}
+    PSEUDO_LOOKUPS = {}
 
     @classmethod
-    def filter_for_pseudolookup(cls, field, lookup_type):
+    def patch_filter_class(cls, filter_class, old_lookup, new_lookup):
         """
-        Override this method to provide custom lookups.
-        By default it returns the class specified in 'filter_class' if not None.
-        If None was specified, it returns the class django-filters' would use
-        but modified to use the behaves_like lookup instead of the actual one.
+        Patches filter_class __init__ method to replace old_lookup with the new_lookup.
         """
-        params = cls.pseudo_lookups[lookup_type].get('extra', lambda f: {})(field)
-        behaves_like = cls.pseudo_lookups[lookup_type]['behaves_like']
-
-        if cls.pseudo_lookups[lookup_type]['filter_class'] is not None:
-            return cls.pseudo_lookups[lookup_type]['filter_class'], params
-        
-        # Query django-filters for the lookup, and patch it
-        df_filter, df_params = super().filter_for_lookup(field, behaves_like)
 
         class PseudoLookupsFilterMetaclass(type):
             def __str__(self):
-                return '<' + str(df_filter) + ' wrapped by ' + str(self) + '>'
+                return '<' + str(filter_class) + ' wrapped by ' + str(self) + '>'
 
-        class PseudoLookupsFilter(df_filter, metaclass=PseudoLookupsFilterMetaclass):
+        class PseudoLookupsFilter(filter_class, metaclass=PseudoLookupsFilterMetaclass):
             def __init__(self, *args, **kwargs):
                 if 'lookup_expr' in kwargs:
-                    kwargs['lookup_expr'] = kwargs['lookup_expr'][:-len(lookup_type)] + behaves_like
+                    kwargs['lookup_expr'] = kwargs['lookup_expr'][:-len(old_lookup)] + new_lookup
                 super().__init__(*args, **kwargs)
 
-        df_params.update(params)
-        return PseudoLookupsFilter, df_params
+        return PseudoLookupsFilter
+
+
+    @classmethod
+    def filter_for_pseudolookup(cls, field, lookup_type):
+        """
+        Override this method to provide custom lookups.
+        By default it returns the class specified in 'filter_class' if not None.
+        If None was specified, it returns the class django-filters' would use.
+        If 'replace_lookup' is set, patches the class to receive this lookup 
+        instead of the actual one.
+
+        Args:
+            field: resulting field from applying all transforms to the LHS
+            lookup_type: lookup excluding any transforms
+
+        Return value:
+            Tuple (filterset_class, kwargs)
+        """
+        params = cls.PSEUDO_LOOKUPS[lookup_type].get('extra', lambda f: {})(field)
+        behaves_like = cls.PSEUDO_LOOKUPS[lookup_type]['behaves_like']
+
+        if cls.PSEUDO_LOOKUPS[lookup_type].get('filter_class', None) is not None:
+            filter_class = cls.PSEUDO_LOOKUPS[lookup_type]['filter_class']
+        else:
+            filter_class, df_params = super().filter_for_lookup(field, behaves_like)
+
+            df_params.update(params)
+            params = df_params
+
+        # Patch the class if we have to so that it receives the new lookup
+        if cls.PSEUDO_LOOKUPS[lookup_type].get('replace_lookup', None):
+            filter_class = cls.patch_filter_class(filter_class, lookup_type, cls.PSEUDO_LOOKUPS[lookup_type]['replace_lookup'])
+
+        return filter_class, params
 
                 
 
     @classmethod
     def filter_for_lookup(cls, field, lookup_type):
         """
         Support for pseudo-lookups
         """
-        pseudo_lookups = getattr(cls, 'pseudo_lookups', {})
+        PSEUDO_LOOKUPS = getattr(cls, 'PSEUDO_LOOKUPS', {})
 
-        if lookup_type in pseudo_lookups:
+        if lookup_type in PSEUDO_LOOKUPS:
             filter, params = cls.filter_for_pseudolookup(field, lookup_type)
         else:
             filter, params = super().filter_for_lookup(field, lookup_type)
 
         return filter, params
     
 
@@ -121,21 +143,21 @@
         and a final lookup. At the same time it computes the field type
         resulting from applying the transforms.
 
         For pseudo-lookups the underlying Django machinery will fail,
         therefore we will swap them for a Django-compliant one with the
         same semantics, and then swap it back
         """
-        pseudo_lookups = getattr(cls, 'pseudo_lookups', [])
+        PSEUDO_LOOKUPS = getattr(cls, 'PSEUDO_LOOKUPS', [])
 
         pseudo = None
-        for lookup in pseudo_lookups:
+        for lookup in PSEUDO_LOOKUPS:
             if lookup_expr.endswith(lookup):
                 pseudo = lookup
-                lookup_expr = lookup_expr[:-len(lookup)] + pseudo_lookups[lookup]['behaves_like']
+                lookup_expr = lookup_expr[:-len(lookup)] + PSEUDO_LOOKUPS[lookup]['behaves_like']
                 break
 
         field, lookup_type = django_filter_resolve_field(field, lookup_expr)
 
         if pseudo:
             lookup_type = pseudo
```

