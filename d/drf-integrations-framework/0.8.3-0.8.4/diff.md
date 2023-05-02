# Comparing `tmp/drf-integrations-framework-0.8.3.tar.gz` & `tmp/drf_integrations_framework-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-integrations-framework-0.8.3.tar", max compression
+gzip compressed data, was "drf_integrations_framework-0.8.4.tar", max compression
```

## Comparing `drf-integrations-framework-0.8.3.tar` & `drf_integrations_framework-0.8.4.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/LICENSE
--rw-r--r--   0        0        0     6594 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/README.md
--rw-r--r--   0        0        0      244 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/__init__.py
--rw-r--r--   0        0        0     3186 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/admin.py
--rw-r--r--   0        0        0     1896 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/apps.py
--rw-r--r--   0        0        0     2330 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/auth_backends.py
--rw-r--r--   0        0        0       48 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/exceptions.py
--rw-r--r--   0        0        0     5049 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/fields.py
--rw-r--r--   0        0        0     3342 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/forms.py
--rw-r--r--   0        0        0      228 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/integrations/__init__.py
--rw-r--r--   0        0        0     8933 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/integrations/base.py
--rw-r--r--   0        0        0      368 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/integrations/managers.py
--rw-r--r--   0        0        0      643 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/integrations/models.py
--rw-r--r--   0        0        0     3234 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/integrations/registry.py
--rw-r--r--   0        0        0        0 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/management/commands/__init__.py
--rw-r--r--   0        0        0      435 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/management/commands/syncregistry.py
--rw-r--r--   0        0        0     3389 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/managers.py
--rw-r--r--   0        0        0    10827 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/migrations/0001_initial.py
--rw-r--r--   0        0        0      785 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/migrations/0002_auto_20200623_1421.py
--rw-r--r--   0        0        0      498 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/migrations/0003_auto_20210118_1317.py
--rw-r--r--   0        0        0      589 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/migrations/0004_auto_20220503_1428.py
--rw-r--r--   0        0        0      500 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/migrations/0005_alter_applicationinstallation_id.py
--rw-r--r--   0        0        0      381 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/migrations/__init__.py
--rw-r--r--   0        0        0    11744 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/models.py
--rw-r--r--   0        0        0      311 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/types.py
--rw-r--r--   0        0        0      758 2022-07-15 08:32:26.311953 drf-integrations-framework-0.8.3/drf_integrations/urls.py
--rw-r--r--   0        0        0     3655 2022-07-15 08:32:26.315953 drf-integrations-framework-0.8.3/drf_integrations/utils.py
--rw-r--r--   0        0        0     2175 2022-07-15 08:32:51.236000 drf-integrations-framework-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     7722 2022-07-15 08:32:52.681124 drf-integrations-framework-0.8.3/setup.py
--rw-r--r--   0        0        0     7754 2022-07-15 08:32:52.681851 drf-integrations-framework-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/LICENSE
+-rw-r--r--   0        0        0     6594 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/README.md
+-rw-r--r--   0        0        0      244 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/__init__.py
+-rw-r--r--   0        0        0     3186 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/admin.py
+-rw-r--r--   0        0        0     1896 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/apps.py
+-rw-r--r--   0        0        0     2346 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/auth_backends.py
+-rw-r--r--   0        0        0       48 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/exceptions.py
+-rw-r--r--   0        0        0     5049 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/fields.py
+-rw-r--r--   0        0        0     3342 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/forms.py
+-rw-r--r--   0        0        0      228 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/integrations/__init__.py
+-rw-r--r--   0        0        0     8933 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/integrations/base.py
+-rw-r--r--   0        0        0      368 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/integrations/managers.py
+-rw-r--r--   0        0        0      643 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/integrations/models.py
+-rw-r--r--   0        0        0     3250 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/integrations/registry.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/management/commands/__init__.py
+-rw-r--r--   0        0        0      435 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/management/commands/syncregistry.py
+-rw-r--r--   0        0        0     3389 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/managers.py
+-rw-r--r--   0        0        0    10827 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/migrations/0001_initial.py
+-rw-r--r--   0        0        0      785 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/migrations/0002_auto_20200623_1421.py
+-rw-r--r--   0        0        0      498 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/migrations/0003_auto_20210118_1317.py
+-rw-r--r--   0        0        0      589 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/migrations/0004_auto_20220503_1428.py
+-rw-r--r--   0        0        0      500 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/migrations/0005_alter_applicationinstallation_id.py
+-rw-r--r--   0        0        0      381 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/migrations/__init__.py
+-rw-r--r--   0        0        0    11744 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/models.py
+-rw-r--r--   0        0        0      311 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/types.py
+-rw-r--r--   0        0        0      758 2023-05-02 11:06:27.251484 drf_integrations_framework-0.8.4/drf_integrations/urls.py
+-rw-r--r--   0        0        0     3675 2023-05-02 11:06:27.255484 drf_integrations_framework-0.8.4/drf_integrations/utils.py
+-rw-r--r--   0        0        0     2168 2023-05-02 11:06:27.255484 drf_integrations_framework-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 drf_integrations_framework-0.8.4/PKG-INFO
```

### Comparing `drf-integrations-framework-0.8.3/LICENSE` & `drf_integrations_framework-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/README.md` & `drf_integrations_framework-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/admin.py` & `drf_integrations_framework-0.8.4/drf_integrations/admin.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/apps.py` & `drf_integrations_framework-0.8.4/drf_integrations/apps.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/auth_backends.py` & `drf_integrations_framework-0.8.4/drf_integrations/auth_backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,14 @@
                             request=request, application=token.application
                         )
                     )
                 )
             except (
                 ApplicationInstallation.DoesNotExist,
                 ApplicationInstallation.MultipleObjectsReturned,
-            ):
+            ) as err:
                 logger.exception("drf_integrations.auth_backends.invalid_installation")
-                raise exceptions.AuthenticationFailed()
+                raise exceptions.AuthenticationFailed() from err
 
             request.auth_context = installation.get_context()
 
         return result
```

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/fields.py` & `drf_integrations_framework-0.8.4/drf_integrations/fields.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/forms.py` & `drf_integrations_framework-0.8.4/drf_integrations/forms.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/integrations/base.py` & `drf_integrations_framework-0.8.4/drf_integrations/integrations/base.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/integrations/models.py` & `drf_integrations_framework-0.8.4/drf_integrations/integrations/models.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/integrations/registry.py` & `drf_integrations_framework-0.8.4/drf_integrations/integrations/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         try:
             if isinstance(name_or_class, str):
                 integration = self.integrations[name_or_class]
             elif inspect.isclass(name_or_class) and issubclass(name_or_class, BaseIntegration):
                 integration = self.integrations[name_or_class.name]
             else:
                 raise ValueError("invalid name or base integration class")
-        except KeyError:
-            raise Registry.IntegrationUnavailableException()
+        except KeyError as err:
+            raise Registry.IntegrationUnavailableException() from err
 
         return integration
 
     def get_urls(self, basepath="api/integrations/") -> List:
         """Get URLConf for all registered integrations."""
         urls = []
         for name, integration_cls in self.integrations.items():
```

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/managers.py` & `drf_integrations_framework-0.8.4/drf_integrations/managers.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/migrations/0001_initial.py` & `drf_integrations_framework-0.8.4/drf_integrations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/migrations/0002_auto_20200623_1421.py` & `drf_integrations_framework-0.8.4/drf_integrations/migrations/0002_auto_20200623_1421.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/migrations/0004_auto_20220503_1428.py` & `drf_integrations_framework-0.8.4/drf_integrations/migrations/0004_auto_20220503_1428.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/models.py` & `drf_integrations_framework-0.8.4/drf_integrations/models.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/urls.py` & `drf_integrations_framework-0.8.4/drf_integrations/urls.py`

 * *Files identical despite different names*

### Comparing `drf-integrations-framework-0.8.3/drf_integrations/utils.py` & `drf_integrations_framework-0.8.4/drf_integrations/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     try:
         return import_string(form_field)
     except ImportError:
         raise ImportError(
             "drf_integrations can only work with a backend that supports JSON fields, "
             "please make sure you set the DB_BACKEND_JSON_FORM_FIELD setting to the "
             "JSONField of your backend."
-        )
+        ) from None
 
 
 def get_json_model_field_import_name():
     # if the Django version >= 3.2 then user the new default JSONField
     if django.VERSION[0:2] >= (3, 2):
         default = "django.db.models.JSONField"
     else:
@@ -110,8 +110,8 @@
     try:
         return import_string(model_field)
     except ImportError:
         raise ImportError(
             "drf_integrations can only work with a backend that supports JSON fields, "
             "please make sure you set the DB_BACKEND_JSON_FIELD setting to the "
             "JSONField of your backend."
-        )
+        ) from None
```

### Comparing `drf-integrations-framework-0.8.3/pyproject.toml` & `drf_integrations_framework-0.8.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "drf-integrations-framework"
-version = "v0.8.3"
+version = "0.8.4"
 description = "Django REST Framework plugin that simplifies the management of third party integrations"
 authors = ["Yoyo <dev@yoyowallet.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/yoyowallet/drf-integrations-framework"
 repository = "https://github.com/yoyowallet/drf-integrations-framework"
 keywords = ["drf"]
@@ -26,31 +26,30 @@
     "LICENSE",
 ]
 packages = [
     { include="drf_integrations" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
+python = ">=3.7,<3.12"
 djangorestframework = "^3.11.0"
 # Going above 1.5 causes issues with OAUTH2_PROVIDER_ACCESS_TOKEN_MODEL
 # And swappable dependencies
-django-oauth-toolkit = ">=1.3"
-django-environ = "0.9.0"
-Pillow = "^9.1.0"
+django-oauth-toolkit = ">=1.3,<1.5"
+django-environ = "^0.9.0"
+Pillow = ">=7.0.0,<10.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 factory-boy = "^3.2.1"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 mixpanel = "^4.9.0"
 oauth2client = "^4.1.3"
 pre-commit = "^2.20.0"
-psycopg2 =  "^2.9.3"
 psycopg2-binary = "^2.9.3"
 pytest = "^7.1.1"
 pytest-django = "^4.5.2"
 pytest-mock = "^3.8.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `drf-integrations-framework-0.8.3/setup.py` & `drf_integrations_framework-0.8.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,177 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: drf-integrations-framework
+Version: 0.8.4
+Summary: Django REST Framework plugin that simplifies the management of third party integrations
+Home-page: https://github.com/yoyowallet/drf-integrations-framework
+License: MIT
+Keywords: drf
+Author: Yoyo
+Author-email: dev@yoyowallet.com
+Requires-Python: >=3.7,<3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: Pillow (>=7.0.0,<10.0.0)
+Requires-Dist: django-environ (>=0.9.0,<0.10.0)
+Requires-Dist: django-oauth-toolkit (>=1.3,<1.5)
+Requires-Dist: djangorestframework (>=3.11.0,<4.0.0)
+Project-URL: Repository, https://github.com/yoyowallet/drf-integrations-framework
+Description-Content-Type: text/markdown
+
+# DRF Integrations Framework
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fyoyowallet%2Fdrf-integrations-framework%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/yoyowallet/drf-integrations-framework/goto?ref=master)
+
+DRF Integrations Framework is a toolkit that plugs in to [Django REST Framework](https://www.django-rest-framework.org/)
+and simplifies the management of third party integrations. If you find yourself connecting to multiple services with
+different sets of credentials, or handling multiple inbound requests from third party services, DRF Integrations
+Framework will probably simplify that for you. DRF Integrations Framework will help you split the responsibilities
+between the source/destiny of events, how these requests are authenticated and the business logic associated to them.
+
+## Requirements
+- Python 3.7+
+- Django 2.2+
+- Django REST Framework 3.9.2+
+- Django OAuth Toolkit 1.7.1+
+
+## Installation
+
+The following library is required in order to build on `Linux systems`. It fixes the
+problem where `Error: pg_config executable not found.` is given when installing psycopg2
+via `poetry install`
+```
+sudo apt install libpq-dev
+```
+
+Install from PyPi:
+```bash
+pip install drf-integrations-framework
+```
+Or install from source:
+```bash
+pip install https://github.com/yoyowallet/drf-integrations-framework/archive/v0.7.1.tar.gz
+```
+
+Add the apps to your `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = [
+    ...,
+    "rest_framework",
+    "oauth2_provider",
+    "drf_integrations",
+]
+```
+
+If you are going to configure any inbound integration, you will want to add the integration URLs to your `urls.py`:
+```python
+from drf_integrations import integrations
+
+urlpatterns = [
+    ...
+] + integrations.get_urls()
+```
+
+## Configuration
+### Settings
+DRF Integrations Framework relies on Django OAuth Toolkit to manage third party applications. In order to be able to use
+it, first you'll need to configure DOT by setting (at least) the model references in your settings.
+```python
+OAUTH2_PROVIDER_APPLICATION_MODEL = "drf_integrations.Application"
+OAUTH2_PROVIDER_ACCESS_TOKEN_MODEL = "drf_integrations.AccessToken"
+OAUTH2_PROVIDER_GRANT_MODEL = "drf_integrations.Grant"
+OAUTH2_PROVIDER_REFRESH_TOKEN_MODEL = "drf_integrations.RefreshToken"
+```
+Then, similarly, you will have to configure the model for the integrations.
+```python
+INTEGRATIONS_APPLICATION_INSTALLATION_MODEL = "drf_integrations.ApplicationInstallation"
+```
+You will also have to configure how the integrations are stored in the database. On the one hand, you will have to set
+the type of JSON field your DB uses. On the other hand, you will have to set the name of the attribute where you want to
+relate the integrations.
+```python
+DB_BACKEND_JSON_FIELD = "django.db.models.JSONField"
+INTEGRATIONS_APPLICATION_INSTALLATION_INSTALL_ATTRIBUTE = "organisation"
+```
+Finally, you have to set the list of integrations that are available in your system (see the following section to learn
+about creating integrations).
+```python
+INSTALLED_INTEGRATIONS = [
+    "example.drf_integrations_example.api.integrations.APIClientIntegration",
+]
+```
+### Creating integrations
+An integration is represented by an extension of `BaseIntegration`. Then, the integration will be available to be
+installed to different clients (as related with the previously configured
+`INTEGRATIONS_APPLICATION_INSTALLATION_INSTALL_ATTRIBUTE`) once it is stored into an `Application`. This can be done in
+two different ways:
+1. Internal integrations (or non-local integrations) are those that can be configured once and installed to different clients with different
+parameters. For example, your system may connect to Mixpanel, the connections and interactions with the service are all
+the same, only the secret in the connection changes.
+
+   These will only have 1 `Application` object in the database, and it can be related to multiple installations. They
+   can also be automatically created by using the `syncregistry` management command.
+   ```bash
+   python manage.py syncregistry
+   ```
+
+1. Local integrations are those that are specific to just one client. For example, OAuth clients are local, there is
+1 application per client, which will have the specific credentials for them, so they can only be installed once. These
+are usually created on demand as required by clients.
+
+An integration broadly has 3 functions:
+1. Generates a list of URLs that a third party represented by this integration can connect to.
+Mainly used for inward integrations.
+1. Returns a client that can connect to the third party it represents. Mainly used for outward integrations.
+1. Produce queryset filter lookups to search for installations of the integration.
+
+Once you have a class inheriting from `BaseIntegration` that represents a third party, simply add it to
+`INSTALLED_INTEGRATIONS` in your settings and the sky is the limit! You can create custom authentication backends,
+permissions, event hooks... Take a look at [the example](example) to see some basic examples of how you can make use
+of DRF Integrations Framework.
+
+### Preconfigured
+There are some features that DRF Integrations Framework provides out of the box.
+
+- Admin model for `ApplicationInstallation` that already handles integration-specific configuration via dynamic forms.
+- Automatic form validation for integrations that have one.
+- An authentication backend for local OAuth2 integrations
+(`drf_integrations.auth_backends.IntegrationOAuth2Authentication`).
+
+## Running the tests
+
+To run the tests you need to have a postgresql server running on localhost and have a
+postgres user/role defined. To create the postgres user and role you can use the
+following:
+
+```psql -c 'CREATE ROLE postgres WITH LOGIN SUPERUSER' ```
+
+To run the tests execute the following
+
+```make tests```
+
+If running tests under pycharm ensure that `python tests` -> `pytest` is used and set
+the `Additional Arguments` to `--no-migrations`
+
+Failing to specify `--no-migrations` will result in the following error:
+```
+ValueError: Related model 'oauth2_provider.idtoken' cannot be resolved
+```
+
+## Changelog
+See [Releases](https://github.com/yoyowallet/drf-integrations-framework/releases)
+
+## Authors
+DRF Integrations Framework is an original idea by [@jianyuan](https://github.com/jianyuan), developed and maintained by
+the platform team at [@yoyowallet](https://github.com/yoyowallet).
 
-packages = \
-['drf_integrations',
- 'drf_integrations.integrations',
- 'drf_integrations.management',
- 'drf_integrations.management.commands',
- 'drf_integrations.migrations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pillow>=9.1.0,<10.0.0',
- 'django-environ==0.9.0',
- 'django-oauth-toolkit>=1.3',
- 'djangorestframework>=3.11.0,<4.0.0']
-
-setup_kwargs = {
-    'name': 'drf-integrations-framework',
-    'version': '0.8.3',
-    'description': 'Django REST Framework plugin that simplifies the management of third party integrations',
-    'long_description': '# DRF Integrations Framework\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fyoyowallet%2Fdrf-integrations-framework%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/yoyowallet/drf-integrations-framework/goto?ref=master)\n\nDRF Integrations Framework is a toolkit that plugs in to [Django REST Framework](https://www.django-rest-framework.org/)\nand simplifies the management of third party integrations. If you find yourself connecting to multiple services with\ndifferent sets of credentials, or handling multiple inbound requests from third party services, DRF Integrations\nFramework will probably simplify that for you. DRF Integrations Framework will help you split the responsibilities\nbetween the source/destiny of events, how these requests are authenticated and the business logic associated to them.\n\n## Requirements\n- Python 3.7+\n- Django 2.2+\n- Django REST Framework 3.9.2+\n- Django OAuth Toolkit 1.7.1+\n\n## Installation\n\nThe following library is required in order to build on `Linux systems`. It fixes the\nproblem where `Error: pg_config executable not found.` is given when installing psycopg2\nvia `poetry install`\n```\nsudo apt install libpq-dev\n```\n\nInstall from PyPi:\n```bash\npip install drf-integrations-framework\n```\nOr install from source:\n```bash\npip install https://github.com/yoyowallet/drf-integrations-framework/archive/v0.7.1.tar.gz\n```\n\nAdd the apps to your `INSTALLED_APPS`:\n```python\nINSTALLED_APPS = [\n    ...,\n    "rest_framework",\n    "oauth2_provider",\n    "drf_integrations",\n]\n```\n\nIf you are going to configure any inbound integration, you will want to add the integration URLs to your `urls.py`:\n```python\nfrom drf_integrations import integrations\n\nurlpatterns = [\n    ...\n] + integrations.get_urls()\n```\n\n## Configuration\n### Settings\nDRF Integrations Framework relies on Django OAuth Toolkit to manage third party applications. In order to be able to use\nit, first you\'ll need to configure DOT by setting (at least) the model references in your settings.\n```python\nOAUTH2_PROVIDER_APPLICATION_MODEL = "drf_integrations.Application"\nOAUTH2_PROVIDER_ACCESS_TOKEN_MODEL = "drf_integrations.AccessToken"\nOAUTH2_PROVIDER_GRANT_MODEL = "drf_integrations.Grant"\nOAUTH2_PROVIDER_REFRESH_TOKEN_MODEL = "drf_integrations.RefreshToken"\n```\nThen, similarly, you will have to configure the model for the integrations.\n```python\nINTEGRATIONS_APPLICATION_INSTALLATION_MODEL = "drf_integrations.ApplicationInstallation"\n```\nYou will also have to configure how the integrations are stored in the database. On the one hand, you will have to set\nthe type of JSON field your DB uses. On the other hand, you will have to set the name of the attribute where you want to\nrelate the integrations.\n```python\nDB_BACKEND_JSON_FIELD = "django.db.models.JSONField"\nINTEGRATIONS_APPLICATION_INSTALLATION_INSTALL_ATTRIBUTE = "organisation"\n```\nFinally, you have to set the list of integrations that are available in your system (see the following section to learn\nabout creating integrations).\n```python\nINSTALLED_INTEGRATIONS = [\n    "example.drf_integrations_example.api.integrations.APIClientIntegration",\n]\n```\n### Creating integrations\nAn integration is represented by an extension of `BaseIntegration`. Then, the integration will be available to be\ninstalled to different clients (as related with the previously configured\n`INTEGRATIONS_APPLICATION_INSTALLATION_INSTALL_ATTRIBUTE`) once it is stored into an `Application`. This can be done in\ntwo different ways:\n1. Internal integrations (or non-local integrations) are those that can be configured once and installed to different clients with different\nparameters. For example, your system may connect to Mixpanel, the connections and interactions with the service are all\nthe same, only the secret in the connection changes.\n\n   These will only have 1 `Application` object in the database, and it can be related to multiple installations. They\n   can also be automatically created by using the `syncregistry` management command.\n   ```bash\n   python manage.py syncregistry\n   ```\n\n1. Local integrations are those that are specific to just one client. For example, OAuth clients are local, there is\n1 application per client, which will have the specific credentials for them, so they can only be installed once. These\nare usually created on demand as required by clients.\n\nAn integration broadly has 3 functions:\n1. Generates a list of URLs that a third party represented by this integration can connect to.\nMainly used for inward integrations.\n1. Returns a client that can connect to the third party it represents. Mainly used for outward integrations.\n1. Produce queryset filter lookups to search for installations of the integration.\n\nOnce you have a class inheriting from `BaseIntegration` that represents a third party, simply add it to\n`INSTALLED_INTEGRATIONS` in your settings and the sky is the limit! You can create custom authentication backends,\npermissions, event hooks... Take a look at [the example](example) to see some basic examples of how you can make use\nof DRF Integrations Framework.\n\n### Preconfigured\nThere are some features that DRF Integrations Framework provides out of the box.\n\n- Admin model for `ApplicationInstallation` that already handles integration-specific configuration via dynamic forms.\n- Automatic form validation for integrations that have one.\n- An authentication backend for local OAuth2 integrations\n(`drf_integrations.auth_backends.IntegrationOAuth2Authentication`).\n\n## Running the tests\n\nTo run the tests you need to have a postgresql server running on localhost and have a\npostgres user/role defined. To create the postgres user and role you can use the\nfollowing:\n\n```psql -c \'CREATE ROLE postgres WITH LOGIN SUPERUSER\' ```\n\nTo run the tests execute the following\n\n```make tests```\n\nIf running tests under pycharm ensure that `python tests` -> `pytest` is used and set\nthe `Additional Arguments` to `--no-migrations`\n\nFailing to specify `--no-migrations` will result in the following error:\n```\nValueError: Related model \'oauth2_provider.idtoken\' cannot be resolved\n```\n\n## Changelog\nSee [Releases](https://github.com/yoyowallet/drf-integrations-framework/releases)\n\n## Authors\nDRF Integrations Framework is an original idea by [@jianyuan](https://github.com/jianyuan), developed and maintained by\nthe platform team at [@yoyowallet](https://github.com/yoyowallet).\n',
-    'author': 'Yoyo',
-    'author_email': 'dev@yoyowallet.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/yoyowallet/drf-integrations-framework',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

