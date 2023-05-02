# Comparing `tmp/wagtail-site-inheritance-0.0.1.tar.gz` & `tmp/wagtail-site-inheritance-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-site-inheritance-0.0.1.tar", last modified: Mon Mar  9 10:14:44 2020, max compression
+gzip compressed data, was "wagtail-site-inheritance-1.0.0.tar", last modified: Tue May  2 13:31:31 2023, max compression
```

## Comparing `wagtail-site-inheritance-0.0.1.tar` & `wagtail-site-inheritance-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/
--rw-r--r--   0 mvantellingen   (501) staff       (20)       57 2019-07-08 07:11:09.000000 wagtail-site-inheritance-0.0.1/CHANGES
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1090 2020-03-09 09:49:04.000000 wagtail-site-inheritance-0.0.1/LICENSE
--rw-r--r--   0 mvantellingen   (501) staff       (20)      281 2020-03-09 09:57:40.000000 wagtail-site-inheritance-0.0.1/MANIFEST.in
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1147 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/PKG-INFO
--rw-r--r--   0 mvantellingen   (501) staff       (20)      776 2020-03-09 09:49:04.000000 wagtail-site-inheritance-0.0.1/README.md
--rw-r--r--   0 mvantellingen   (501) staff       (20)      553 2020-03-09 09:39:35.000000 wagtail-site-inheritance-0.0.1/pyproject.toml
--rw-r--r--   0 mvantellingen   (501) staff       (20)      125 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/setup.cfg
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1782 2020-03-09 09:55:10.000000 wagtail-site-inheritance-0.0.1/setup.py
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/
--rw-r--r--   0 mvantellingen   (501) staff       (20)      108 2020-03-09 07:21:34.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/__init__.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)      561 2020-03-09 07:21:34.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/admin.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)      361 2020-03-09 07:21:34.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/apps.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1473 2020-03-09 09:39:35.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/forms.py
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/locale/
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/locale/nl/
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1655 2020-03-09 07:21:34.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 mvantellingen   (501) staff       (20)     2448 2020-03-09 07:21:34.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/migrations/
--rw-r--r--   0 mvantellingen   (501) staff       (20)     2460 2020-03-09 09:39:35.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/migrations/0001_initial.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)        0 2019-07-08 07:11:09.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/migrations/__init__.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)     3618 2020-03-09 09:39:35.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/models.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)      415 2020-03-09 07:21:34.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/permissions.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)      780 2020-03-09 09:39:35.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/receivers.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)      763 2020-03-09 07:21:34.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/views.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1723 2020-03-09 09:39:35.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/wagtail_forms.py
--rw-r--r--   0 mvantellingen   (501) staff       (20)     5679 2020-03-09 09:39:35.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/wagtail_hooks.py
-drwxr-xr-x   0 mvantellingen   (501) staff       (20)        0 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1147 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/PKG-INFO
--rw-r--r--   0 mvantellingen   (501) staff       (20)     1020 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/SOURCES.txt
--rw-r--r--   0 mvantellingen   (501) staff       (20)        1 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/dependency_links.txt
--rw-r--r--   0 mvantellingen   (501) staff       (20)        1 2020-03-09 09:57:18.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/not-zip-safe
--rw-r--r--   0 mvantellingen   (501) staff       (20)      262 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/requires.txt
--rw-r--r--   0 mvantellingen   (501) staff       (20)       25 2020-03-09 10:14:44.000000 wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.839161 wagtail-site-inheritance-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.839161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.839161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wagtail-site-inheritance-0.0.1/LICENSE` & `wagtail-site-inheritance-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-0.0.1/PKG-INFO` & `wagtail-site-inheritance-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-site-inheritance
-Version: 0.0.1
+Version: 1.0.0
 Summary: Site Inheritance for Wagtail
 Home-page: https://github.com/labd/wagtail-site-inheritance
 Author: Lab Digital
 Author-email: opensource@labdigital.nl
 License: MIT
 Description: 
         # Wagtail Site Inheritance
@@ -19,19 +19,20 @@
         ## TODO
          - [ ] https://github.com/wagtail/wagtail/issues/4925
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
```

### Comparing `wagtail-site-inheritance-0.0.1/README.md` & `wagtail-site-inheritance-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-0.0.1/setup.py` & `wagtail-site-inheritance-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import re
 
 from setuptools import find_packages, setup
 
 docs_require = ["sphinx>=1.4.0"]
 
 tests_require = [
-    "coverage[toml]==5.0.3",
-    "freezegun==0.3.15",
-    "pytest==5.3.5",
-    "pytest-django==3.8.0",
-    "pytest-cov==2.8.1",
-    "wagtail-factories==2.0.0",
+    "coverage[toml]==5.2.1",
+    "factory-boy==3.2.0",
+    "freezegun==1.1.0",
+    "pytest==6.2.4",
+    "pytest-django==4.4.0",
+    "pytest-cov==2.12.1",
+    "wagtail-factories==2.0.1",
+    "mock==4.0.3",
     # Linting
     "isort[pyproject]==4.3.21",
     "flake8==3.7.9",
     "flake8-blind-except==0.1.1",
     "flake8-debugger==3.1.0"
 ]
 
@@ -25,38 +27,42 @@
         fh.read(),
         flags=re.M | re.S,
     )
 
 
 setup(
     name="wagtail-site-inheritance",
-    version="0.0.1",
+    version="1.0.0",
     description="Site Inheritance for Wagtail",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/labd/wagtail-site-inheritance",
     author="Lab Digital",
     author_email="opensource@labdigital.nl",
-    install_requires=["Django>=2.2", "wagtail>=2.6"],
+    install_requires=[
+        "Django>=2.2",
+        "wagtail>=2.16,<4.0"
+    ],
     tests_require=tests_require,
     extras_require={"docs": docs_require, "test": tests_require},
     entry_points={},
     package_dir={"": "src"},
     packages=find_packages("src"),
     include_package_data=True,
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Wagtail",
         "Framework :: Wagtail :: 2",
+        "Framework :: Wagtail :: 3",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     zip_safe=False,
 )
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/admin.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/forms.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 __all__ = ["get_readonly_widget"]
 
 
 def get_readonly_widget(field):
     widget = field.widget
     widget_class = widget.__class__
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/migrations/0001_initial.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.4 on 2019-09-07 08:53
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("wagtailcore", "0041_group_collection_permissions_verbose_name_plural"),
     ]
 
     operations = [
@@ -69,10 +68,12 @@
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.PROTECT,
                         related_name="+",
                         to="wagtailcore.Page",
                     ),
                 ),
             ],
-            options={"unique_together": {("page", "inherited_page")},},
+            options={
+                "unique_together": {("page", "inherited_page")},
+            },
         ),
     ]
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/models.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
+from wagtail import VERSION as wagtail_version
 from wagtail.admin.edit_handlers import FieldPanel, MultiFieldPanel
 from wagtail.admin.forms import WagtailAdminPageForm
-from wagtail.core.models import Page, Site
 
 from wagtail_site_inheritance.forms import get_readonly_widget
 from wagtail_site_inheritance.wagtail_forms import SiteInheritanceAdminForm
 
+if wagtail_version >= (3, 0):
+    from wagtail.models import Page, Site
+else:
+    from wagtail.core.models import Page, Site
+
 
 class SiteInheritance(models.Model):
     parent = models.ForeignKey(
         Site,
         verbose_name=_("parent site"),
         related_name="site_children",
         on_delete=models.PROTECT,
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/receivers.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/receivers.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/views.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from django.db import transaction
+from wagtail import VERSION as wagtail_version
 from wagtail.contrib.modeladmin.views import DeleteView
-from wagtail.core.models import Page
 
 from wagtail_site_inheritance.models import PageInheritanceItem
 
+if wagtail_version >= (3, 0):
+    from wagtail.models import Page
+else:
+    from wagtail.core.models import Page
+
 
 class SiteInheritanceDeleteView(DeleteView):
     @transaction.atomic()
     def post(self, request, *args, **kwargs):
         """
         Remove the PageInheritanceItems before removing the SiteInheritance.
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/wagtail_forms.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django import forms
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from wagtail.admin.forms import WagtailAdminModelForm
 from wagtail.core import hooks
 
 
 class SiteInheritanceAdminForm(WagtailAdminModelForm):
     class Meta:
         fields = ["parent", "site"]
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance/wagtail_hooks.py` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import transaction
 from django.db.models import OneToOneField
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from modelcluster.models import get_all_child_m2m_relations, get_all_child_relations
 from wagtail.contrib.modeladmin.options import ModelAdmin, modeladmin_register
 from wagtail.core import hooks
 
 from wagtail_site_inheritance import models, permissions, views
 
 
@@ -47,22 +47,22 @@
     is_publishing = (
         bool(request.POST.get("action-publish"))
         and parent_page_perms.can_publish_subpage()
     )
     if not is_publishing:
         return
 
+    # Mark edited page as modified
+    models.PageInheritanceItem.objects.filter(page=page, modified=False).update(
+        modified=True
+    )
+
     create_non_existing_pages(request, page, parent_page)
     sync_existing_pages(request, page)
 
-    # Mark edited page as modified
-    models.PageInheritanceItem.objects.filter(
-        inherited_page=page, modified=False
-    ).update(modified=True)
-
 
 def create_non_existing_pages(request, page, parent_page):
     # Create non existing pages in other trees.
     inherited_parents = [
         pii.inherited_page.get_parent()
         for pii in models.PageInheritanceItem.objects.filter(page=page)
     ]
@@ -89,14 +89,15 @@
         "id",
         "path",
         "depth",
         "numchild",
         "url_path",
         "path",
         "index_entries",
+        "slug",
     ]
     skip_fields = (
         default_exclude_fields
         + page.exclude_fields_in_copy
         + ["live_revision", "content_type"]
     )
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/PKG-INFO` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-site-inheritance
-Version: 0.0.1
+Version: 1.0.0
 Summary: Site Inheritance for Wagtail
 Home-page: https://github.com/labd/wagtail-site-inheritance
 Author: Lab Digital
 Author-email: opensource@labdigital.nl
 License: MIT
 Description: 
         # Wagtail Site Inheritance
@@ -19,19 +19,20 @@
         ## TODO
          - [ ] https://github.com/wagtail/wagtail/issues/4925
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
```

### Comparing `wagtail-site-inheritance-0.0.1/src/wagtail_site_inheritance.egg-info/SOURCES.txt` & `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/wagtail_site_inheritance/__init__.py
 src/wagtail_site_inheritance/admin.py
-src/wagtail_site_inheritance/apps.py
 src/wagtail_site_inheritance/forms.py
 src/wagtail_site_inheritance/models.py
 src/wagtail_site_inheritance/permissions.py
 src/wagtail_site_inheritance/receivers.py
 src/wagtail_site_inheritance/views.py
 src/wagtail_site_inheritance/wagtail_forms.py
 src/wagtail_site_inheritance/wagtail_hooks.py
```

