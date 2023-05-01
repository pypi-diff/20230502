# Comparing `tmp/vanoma_api_utils-0.86.0.tar.gz` & `tmp/vanoma-api-utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanoma_api_utils-0.86.0.tar", max compression
+gzip compressed data, was "vanoma-api-utils-0.9.0.tar", max compression
```

## Comparing `vanoma_api_utils-0.86.0.tar` & `vanoma-api-utils-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,21 @@
--rw-r--r--   0        0        0      769 2023-05-01 23:40:06.493466 vanoma_api_utils-0.86.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-20 15:41:36.379982 vanoma_api_utils-0.86.0/vanoma_api_utils/__init__.py
--rw-r--r--   0        0        0     1038 2022-11-12 13:50:51.021781 vanoma_api_utils-0.86.0/vanoma_api_utils/auth_api.py
--rw-r--r--   0        0        0     1505 2022-11-12 13:51:07.717256 vanoma_api_utils-0.86.0/vanoma_api_utils/communication_api.py
--rw-r--r--   0        0        0      256 2021-12-21 21:17:43.572975 vanoma_api_utils-0.86.0/vanoma_api_utils/constants.py
--rw-r--r--   0        0        0        0 2021-11-23 16:02:21.945089 vanoma_api_utils-0.86.0/vanoma_api_utils/django/__init__.py
--rw-r--r--   0        0        0     2847 2023-01-09 12:46:03.473102 vanoma_api_utils-0.86.0/vanoma_api_utils/django/fields.py
--rw-r--r--   0        0        0      511 2023-01-10 10:59:21.300355 vanoma_api_utils-0.86.0/vanoma_api_utils/django/functions.py
--rw-r--r--   0        0        0     1328 2022-12-28 22:45:38.576188 vanoma_api_utils-0.86.0/vanoma_api_utils/django/middlewares.py
--rw-r--r--   0        0        0     2490 2023-04-03 19:00:38.400283 vanoma_api_utils-0.86.0/vanoma_api_utils/django/settings.py
--rw-r--r--   0        0        0     1138 2023-03-03 14:56:46.353080 vanoma_api_utils-0.86.0/vanoma_api_utils/django/tests.py
--rw-r--r--   0        0        0      564 2021-11-29 19:45:24.704407 vanoma_api_utils-0.86.0/vanoma_api_utils/django/validators.py
--rw-r--r--   0        0        0      359 2021-11-29 17:39:47.918553 vanoma_api_utils-0.86.0/vanoma_api_utils/django/views.py
--rw-r--r--   0        0        0      460 2022-11-12 13:53:13.472533 vanoma_api_utils-0.86.0/vanoma_api_utils/exceptions.py
--rw-r--r--   0        0        0     2053 2023-02-12 23:15:14.422967 vanoma_api_utils-0.86.0/vanoma_api_utils/http.py
--rw-r--r--   0        0        0      731 2022-09-29 11:16:04.699469 vanoma_api_utils-0.86.0/vanoma_api_utils/jwt.py
--rw-r--r--   0        0        0      745 2023-03-03 10:18:23.340558 vanoma_api_utils-0.86.0/vanoma_api_utils/misc.py
--rw-r--r--   0        0        0      719 2022-09-29 10:09:58.436537 vanoma_api_utils-0.86.0/vanoma_api_utils/phone_numbers.py
--rw-r--r--   0        0        0        0 2021-11-21 15:05:33.075892 vanoma_api_utils-0.86.0/vanoma_api_utils/py.typed
--rw-r--r--   0        0        0      248 2023-02-14 13:41:15.228232 vanoma_api_utils-0.86.0/vanoma_api_utils/request.py
--rw-r--r--   0        0        0        0 2021-11-23 15:40:52.590038 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/__init__.py
--rw-r--r--   0        0        0      480 2022-11-12 13:23:20.002099 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/exceptions.py
--rw-r--r--   0        0        0      142 2022-05-30 10:26:27.381278 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/filters.py
--rw-r--r--   0        0        0     1144 2022-10-10 09:49:31.420992 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/generics.py
--rw-r--r--   0        0        0     1424 2023-05-01 23:39:19.933610 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/pagination.py
--rw-r--r--   0        0        0      547 2021-11-23 15:53:50.202000 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/parsers.py
--rw-r--r--   0        0        0      351 2021-11-27 13:19:26.452320 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/renderers.py
--rw-r--r--   0        0        0      291 2022-10-18 18:19:28.688546 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/responses.py
--rw-r--r--   0        0        0     6379 2023-01-17 11:33:02.221744 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/serializers.py
--rw-r--r--   0        0        0      215 2022-10-18 18:19:00.551261 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/tests.py
--rw-r--r--   0        0        0     3168 2023-01-08 23:09:08.723575 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/views.py
--rw-r--r--   0        0        0      314 2021-11-24 10:01:52.245853 vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/viewsets.py
--rw-r--r--   0        0        0      338 2021-11-28 15:16:26.130594 vanoma_api_utils-0.86.0/vanoma_api_utils/sentry.py
--rw-r--r--   0        0        0      398 2022-11-10 16:20:16.971278 vanoma_api_utils-0.86.0/vanoma_api_utils/tests.py
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 vanoma_api_utils-0.86.0/setup.py
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 vanoma_api_utils-0.86.0/PKG-INFO
+-rw-r--r--   0        0        0      546 2021-11-27 13:25:43.482096 vanoma-api-utils-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-20 15:41:36.379982 vanoma-api-utils-0.9.0/vanoma_api_utils/__init__.py
+-rw-r--r--   0        0        0      190 2021-11-20 15:41:36.380115 vanoma-api-utils-0.9.0/vanoma_api_utils/constants.py
+-rw-r--r--   0        0        0      207 2021-11-20 15:49:23.694275 vanoma-api-utils-0.9.0/vanoma_api_utils/dates.py
+-rw-r--r--   0        0        0        0 2021-11-23 16:02:21.945089 vanoma-api-utils-0.9.0/vanoma_api_utils/django/__init__.py
+-rw-r--r--   0        0        0     1103 2021-11-26 12:50:37.252425 vanoma-api-utils-0.9.0/vanoma_api_utils/django/fields.py
+-rw-r--r--   0        0        0      849 2021-11-26 12:50:49.598502 vanoma-api-utils-0.9.0/vanoma_api_utils/phone_numbers.py
+-rw-r--r--   0        0        0        0 2021-11-21 15:05:33.075892 vanoma-api-utils-0.9.0/vanoma_api_utils/py.typed
+-rw-r--r--   0        0        0        0 2021-11-27 10:52:06.484387 vanoma-api-utils-0.9.0/vanoma_api_utils/response_types/__init__.py
+-rw-r--r--   0        0        0     1031 2021-11-27 13:17:51.097932 vanoma-api-utils-0.9.0/vanoma_api_utils/response_types/payment_method.py
+-rw-r--r--   0        0        0        0 2021-11-23 15:40:52.590038 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/__init__.py
+-rw-r--r--   0        0        0      297 2021-11-23 15:47:44.140000 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/exceptions.py
+-rw-r--r--   0        0        0     1035 2021-11-27 13:19:12.811213 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/generics.py
+-rw-r--r--   0        0        0      547 2021-11-23 15:53:50.202000 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/parsers.py
+-rw-r--r--   0        0        0      351 2021-11-27 13:19:26.452320 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/renderers.py
+-rw-r--r--   0        0        0      244 2021-11-23 15:47:59.179000 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/responses.py
+-rw-r--r--   0        0        0     1196 2021-11-27 13:24:07.134134 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/tests.py
+-rw-r--r--   0        0        0     1955 2021-11-26 12:15:54.347175 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/views.py
+-rw-r--r--   0        0        0      314 2021-11-24 10:01:52.245853 vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/viewsets.py
+-rw-r--r--   0        0        0      937 2021-11-27 13:26:35.931565 vanoma-api-utils-0.9.0/setup.py
+-rw-r--r--   0        0        0      711 2021-11-27 13:26:35.931898 vanoma-api-utils-0.9.0/PKG-INFO
```

### Comparing `vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/parsers.py` & `vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `vanoma_api_utils-0.86.0/vanoma_api_utils/rest_framework/views.py` & `vanoma-api-utils-0.9.0/vanoma_api_utils/rest_framework/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,58 @@
 import logging
 from typing import Any, Dict
 from django.http import Http404
-from django.core.exceptions import PermissionDenied, ObjectDoesNotExist
+from django.core.exceptions import PermissionDenied
 from rest_framework import exceptions, status
 from rest_framework.response import Response
 from rest_framework.views import set_rollback
 from vanoma_api_utils.constants import ERROR_CODE
 from .responses import generic_error
-from ..exceptions import BackendServiceException
-
-EMPTY_STRING = ""
-
-
-def _extract_message_from_detail(detail: Any) -> str:
-    if isinstance(detail, list):
-        errors = [_extract_message_from_detail(d) for d in detail]
-        # Return the first error. Subsequent errors will be shown once the user fixes the first one.
-        # This is so we can keep the "message" returned in the error as a whole string.
-        for error in errors:
-            # It's possible for error to be an empty string (see below). Return the first non-None error.
-            if error != EMPTY_STRING:
-                return error
-        # We shouldn't get here in theory, but just in case we returned empty strings from below.
-        return EMPTY_STRING
-    elif isinstance(detail, dict):
-        # Return the first error. Subsequent errors will be shown once the user fixes the first one.
-        # This is so we can keep the "message" returned in the error as a whole string.
-        for key, value in detail.items():
-            if str(key).strip().lower() == "non_field_errors":
-                return _extract_message_from_detail(value)
-
-            return f"{key}: {_extract_message_from_detail(value)}"
-        # We have an empty dictionary which can happen if one of the fields of a modal has no validation
-        # errors. See https://sentry.io/share/issue/a031ebc008fe4aee8c0c131e1c747418/
-        return EMPTY_STRING
-    else:
-        return str(detail)
 
 
 def exception_handler(exc: Exception, context: Dict[str, Any]) -> Response:
     """
     Mostly copied from https://github.com/encode/django-rest-framework/blob/master/rest_framework/views.py#L71
     """
-    if isinstance(exc, Http404) or isinstance(exc, ObjectDoesNotExist):
+    if isinstance(exc, Http404):
         return generic_error(
             status.HTTP_404_NOT_FOUND,
             ERROR_CODE.RESOURCE_NOT_FOUND,
             str(exc),
         )
 
     if isinstance(exc, PermissionDenied):
         return generic_error(
             status.HTTP_403_FORBIDDEN,
             ERROR_CODE.AUTHORIZATION_ERROR,
             str(exc),
         )
 
     if isinstance(exc, exceptions.APIException):
-        set_rollback()
-        return generic_error(
-            exc.status_code,
-            ERROR_CODE.INVALID_REQUEST,
-            _extract_message_from_detail(exc.detail),
-        )
+        # Commented out to please mypy which was complaning about
+        # APIException not having attributes below
+        #
+        # headers = {}
+        # if getattr(exc, "auth_header", None):
+        #     headers["WWW-Authenticate"] = exc.auth_header
+        # if getattr(exc, "wait", None):
+        #     headers["Retry-After"] = "%d" % exc.wait
+
+        if isinstance(exc.detail, list):
+            message = ". ".join(exc.detail)
+        elif isinstance(exc.detail, dict):
+            errors = ["{}-{}".format(k, e) for k, e in exc.detail.items()]
+            message = ". ".join(errors)
+        else:
+            message = exc.detail
 
-    if isinstance(exc, BackendServiceException) and exc.is_client_side():
         set_rollback()
         return generic_error(
-            exc.status_code,
-            ERROR_CODE(exc.error_code),
-            exc.error_message,
+            status.HTTP_400_BAD_REQUEST, ERROR_CODE.INVALID_REQUEST, message
         )
 
-    # This will sent the current exception to sentry - https://docs.sentry.io/platforms/python/guides/logging/
-    logging.exception(str(exc))
+    # TODO: use sentry to report 500
+    logging.error(str(exc), exc_info=True)
 
     return generic_error(
         status.HTTP_500_INTERNAL_SERVER_ERROR, ERROR_CODE.INTERNAL_ERROR, str(exc)
     )
```

### Comparing `vanoma_api_utils-0.86.0/setup.py` & `vanoma-api-utils-0.9.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['vanoma_api_utils',
  'vanoma_api_utils.django',
+ 'vanoma_api_utils.response_types',
  'vanoma_api_utils.rest_framework']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Faker>=9.9.1,<10.0.0',
- 'PyJWT>=2.3.0,<3.0.0',
- 'babel>=2.12.1,<3.0.0',
- 'boto3>=1.24.89,<2.0.0',
- 'dj-database-url>=0.5.0,<0.6.0',
- 'django-filter>=21.1,<22.0',
- 'django-storages>=1.13.1,<2.0.0',
- 'django>=4.2,<5.0',
+['Django>=3.2.9,<4.0.0',
+ 'dataclasses-json>=0.5.6,<0.6.0',
  'djangorestframework-camel-case>=1.2.0,<2.0.0',
- 'djangorestframework>=3.14.0,<4.0.0',
+ 'djangorestframework>=3.12.4,<4.0.0',
  'phonenumbers>=8.12.37,<9.0.0',
- 'psycopg2>=2.9.3,<3.0.0',
- 'pyhumps>=3.5.3,<4.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'sentry-sdk>=1.12.1,<2.0.0',
- 'shortuuid>=1.0.9,<2.0.0']
+ 'pytest>=6.2.5,<7.0.0',
+ 'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'vanoma-api-utils',
-    'version': '0.86.0',
+    'version': '0.9.0',
     'description': 'Python utils for vanoma APIs',
-    'long_description': 'None',
+    'long_description': None,
     'author': 'Vanoma',
     'author_email': 'contact@vanoma.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `vanoma_api_utils-0.86.0/PKG-INFO` & `vanoma-api-utils-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,18 @@
 Metadata-Version: 2.1
 Name: vanoma-api-utils
-Version: 0.86.0
+Version: 0.9.0
 Summary: Python utils for vanoma APIs
 Author: Vanoma
 Author-email: contact@vanoma.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Faker (>=9.9.1,<10.0.0)
-Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
-Requires-Dist: babel (>=2.12.1,<3.0.0)
-Requires-Dist: boto3 (>=1.24.89,<2.0.0)
-Requires-Dist: dj-database-url (>=0.5.0,<0.6.0)
-Requires-Dist: django (>=4.2,<5.0)
-Requires-Dist: django-filter (>=21.1,<22.0)
-Requires-Dist: django-storages (>=1.13.1,<2.0.0)
-Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: Django (>=3.2.9,<4.0.0)
+Requires-Dist: dataclasses-json (>=0.5.6,<0.6.0)
+Requires-Dist: djangorestframework (>=3.12.4,<4.0.0)
 Requires-Dist: djangorestframework-camel-case (>=1.2.0,<2.0.0)
 Requires-Dist: phonenumbers (>=8.12.37,<9.0.0)
-Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
-Requires-Dist: pyhumps (>=3.5.3,<4.0.0)
+Requires-Dist: pytest (>=6.2.5,<7.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: sentry-sdk (>=1.12.1,<2.0.0)
-Requires-Dist: shortuuid (>=1.0.9,<2.0.0)
```

