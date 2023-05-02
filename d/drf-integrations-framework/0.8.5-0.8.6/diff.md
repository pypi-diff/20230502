# Comparing `tmp/drf_integrations_framework-0.8.5.tar.gz` & `tmp/drf_integrations_framework-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_integrations_framework-0.8.5.tar", max compression
+gzip compressed data, was "drf_integrations_framework-0.8.6.tar", max compression
```

## Comparing `drf_integrations_framework-0.8.5.tar` & `drf_integrations_framework-0.8.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/LICENSE
--rw-r--r--   0        0        0     6594 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/README.md
--rw-r--r--   0        0        0      244 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/__init__.py
--rw-r--r--   0        0        0     3186 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/admin.py
--rw-r--r--   0        0        0     1896 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/apps.py
--rw-r--r--   0        0        0     2346 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/auth_backends.py
--rw-r--r--   0        0        0       48 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/exceptions.py
--rw-r--r--   0        0        0     5049 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/fields.py
--rw-r--r--   0        0        0     3342 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/forms.py
--rw-r--r--   0        0        0      228 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/integrations/__init__.py
--rw-r--r--   0        0        0     8933 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/integrations/base.py
--rw-r--r--   0        0        0      368 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/integrations/managers.py
--rw-r--r--   0        0        0      643 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/integrations/models.py
--rw-r--r--   0        0        0     3250 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/integrations/registry.py
--rw-r--r--   0        0        0        0 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/management/commands/__init__.py
--rw-r--r--   0        0        0      435 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/management/commands/syncregistry.py
--rw-r--r--   0        0        0     3389 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/managers.py
--rw-r--r--   0        0        0    10827 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/migrations/0001_initial.py
--rw-r--r--   0        0        0      785 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/migrations/0002_auto_20200623_1421.py
--rw-r--r--   0        0        0      498 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/migrations/0003_auto_20210118_1317.py
--rw-r--r--   0        0        0      589 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/migrations/0004_auto_20220503_1428.py
--rw-r--r--   0        0        0      500 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/migrations/0005_alter_applicationinstallation_id.py
--rw-r--r--   0        0        0      381 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/migrations/__init__.py
--rw-r--r--   0        0        0    11744 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/models.py
--rw-r--r--   0        0        0      311 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/types.py
--rw-r--r--   0        0        0      758 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/urls.py
--rw-r--r--   0        0        0     3675 2023-05-02 14:01:34.076418 drf_integrations_framework-0.8.5/drf_integrations/utils.py
--rw-r--r--   0        0        0     2065 2023-05-02 14:01:34.080418 drf_integrations_framework-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     7864 1970-01-01 00:00:00.000000 drf_integrations_framework-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/LICENSE
+-rw-r--r--   0        0        0     6594 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/README.md
+-rw-r--r--   0        0        0      244 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/__init__.py
+-rw-r--r--   0        0        0     3186 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/admin.py
+-rw-r--r--   0        0        0     1896 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/apps.py
+-rw-r--r--   0        0        0     2346 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/auth_backends.py
+-rw-r--r--   0        0        0       48 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/exceptions.py
+-rw-r--r--   0        0        0     5049 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/fields.py
+-rw-r--r--   0        0        0     3342 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/forms.py
+-rw-r--r--   0        0        0      228 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/integrations/__init__.py
+-rw-r--r--   0        0        0     8933 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/integrations/base.py
+-rw-r--r--   0        0        0      368 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/integrations/managers.py
+-rw-r--r--   0        0        0      643 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/integrations/models.py
+-rw-r--r--   0        0        0     3250 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/integrations/registry.py
+-rw-r--r--   0        0        0        0 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/management/commands/__init__.py
+-rw-r--r--   0        0        0      435 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/management/commands/syncregistry.py
+-rw-r--r--   0        0        0     3389 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/managers.py
+-rw-r--r--   0        0        0    10827 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/migrations/0001_initial.py
+-rw-r--r--   0        0        0      785 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/migrations/0002_auto_20200623_1421.py
+-rw-r--r--   0        0        0      498 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/migrations/0003_auto_20210118_1317.py
+-rw-r--r--   0        0        0      444 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/migrations/0004_auto_20220503_1428.py
+-rw-r--r--   0        0        0      500 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/migrations/0005_alter_applicationinstallation_id.py
+-rw-r--r--   0        0        0      381 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/migrations/__init__.py
+-rw-r--r--   0        0        0    11744 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/models.py
+-rw-r--r--   0        0        0      311 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/types.py
+-rw-r--r--   0        0        0      758 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/urls.py
+-rw-r--r--   0        0        0     3675 2023-05-02 16:53:24.621315 drf_integrations_framework-0.8.6/drf_integrations/utils.py
+-rw-r--r--   0        0        0     2189 2023-05-02 16:53:24.625315 drf_integrations_framework-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 drf_integrations_framework-0.8.6/PKG-INFO
```

### Comparing `drf_integrations_framework-0.8.5/LICENSE` & `drf_integrations_framework-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/README.md` & `drf_integrations_framework-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/admin.py` & `drf_integrations_framework-0.8.6/drf_integrations/admin.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/apps.py` & `drf_integrations_framework-0.8.6/drf_integrations/apps.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/auth_backends.py` & `drf_integrations_framework-0.8.6/drf_integrations/auth_backends.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/fields.py` & `drf_integrations_framework-0.8.6/drf_integrations/fields.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/forms.py` & `drf_integrations_framework-0.8.6/drf_integrations/forms.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/integrations/base.py` & `drf_integrations_framework-0.8.6/drf_integrations/integrations/base.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/integrations/models.py` & `drf_integrations_framework-0.8.6/drf_integrations/integrations/models.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/integrations/registry.py` & `drf_integrations_framework-0.8.6/drf_integrations/integrations/registry.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/managers.py` & `drf_integrations_framework-0.8.6/drf_integrations/managers.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/migrations/0001_initial.py` & `drf_integrations_framework-0.8.6/drf_integrations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/migrations/0002_auto_20200623_1421.py` & `drf_integrations_framework-0.8.6/drf_integrations/migrations/0002_auto_20200623_1421.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/models.py` & `drf_integrations_framework-0.8.6/drf_integrations/models.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/urls.py` & `drf_integrations_framework-0.8.6/drf_integrations/urls.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/drf_integrations/utils.py` & `drf_integrations_framework-0.8.6/drf_integrations/utils.py`

 * *Files identical despite different names*

### Comparing `drf_integrations_framework-0.8.5/pyproject.toml` & `drf_integrations_framework-0.8.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "drf-integrations-framework"
-version = "0.8.5"
+version = "0.8.6"
 description = "Django REST Framework plugin that simplifies the management of third party integrations"
 authors = ["Yoyo <dev@yoyowallet.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/yoyowallet/drf-integrations-framework"
 repository = "https://github.com/yoyowallet/drf-integrations-framework"
 keywords = ["drf"]
@@ -28,15 +28,17 @@
 packages = [
     { include="drf_integrations" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 djangorestframework = "^3.11.0"
-django-oauth-toolkit = ">=1.3,<3"
+# Going above django-oauth-toolkit 1.5 causes issues with OAUTH2_PROVIDER_ACCESS_TOKEN_MODEL
+# And swappable dependencies
+django-oauth-toolkit = ">=1.3,<1.5"
 django-environ = "^0.9.0"
 Pillow = ">=7.0.0,<10.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 factory-boy = "^3.2.1"
 flake8 = "^4.0.1"
```

### Comparing `drf_integrations_framework-0.8.5/PKG-INFO` & `drf_integrations_framework-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-integrations-framework
-Version: 0.8.5
+Version: 0.8.6
 Summary: Django REST Framework plugin that simplifies the management of third party integrations
 Home-page: https://github.com/yoyowallet/drf-integrations-framework
 License: MIT
 Keywords: drf
 Author: Yoyo
 Author-email: dev@yoyowallet.com
 Requires-Python: >=3.7,<3.12
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: Pillow (>=7.0.0,<10.0.0)
 Requires-Dist: django-environ (>=0.9.0,<0.10.0)
-Requires-Dist: django-oauth-toolkit (>=1.3,<3)
+Requires-Dist: django-oauth-toolkit (>=1.3,<1.5)
 Requires-Dist: djangorestframework (>=3.11.0,<4.0.0)
 Project-URL: Repository, https://github.com/yoyowallet/drf-integrations-framework
 Description-Content-Type: text/markdown
 
 # DRF Integrations Framework
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
```

