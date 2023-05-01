# Comparing `tmp/django_zana-0.3.0a0.tar.gz` & `tmp/django_zana-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_zana-0.3.0a0.tar", max compression
+gzip compressed data, was "django_zana-0.3.0a1.tar", max compression
```

## Comparing `django_zana-0.3.0a0.tar` & `django_zana-0.3.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1786 2023-04-30 02:54:51.599699 django_zana-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/__init__.py
--rw-r--r--   0        0        0      187 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/apps.py
--rw-r--r--   0        0        0      165 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/__init__.py
--rw-r--r--   0        0        0      159 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/__init__.pyi
--rw-r--r--   0        0        0    18179 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/_xaliases.py
--rw-r--r--   0        0        0     1386 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/fields/__init__.py
--rw-r--r--   0        0        0    41199 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/fields/aliases.py
--rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 django_zana-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1897 2023-05-01 23:03:11.650687 django_zana-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 23:03:11.654687 django_zana-0.3.0a1/zana/django/__init__.py
+-rw-r--r--   0        0        0      187 2023-05-01 23:03:11.654687 django_zana-0.3.0a1/zana/django/apps.py
+-rw-r--r--   0        0        0      165 2023-05-01 23:03:11.654687 django_zana-0.3.0a1/zana/django/models/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-01 23:03:11.654687 django_zana-0.3.0a1/zana/django/models/__init__.pyi
+-rw-r--r--   0        0        0    18179 2023-05-01 23:03:11.654687 django_zana-0.3.0a1/zana/django/models/_xaliases.py
+-rw-r--r--   0        0        0     1386 2023-05-01 23:03:11.654687 django_zana-0.3.0a1/zana/django/models/fields/__init__.py
+-rw-r--r--   0        0        0    41199 2023-05-01 23:03:11.654687 django_zana-0.3.0a1/zana/django/models/fields/aliases.py
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 django_zana-0.3.0a1/PKG-INFO
```

### Comparing `django_zana-0.3.0a0/pyproject.toml` & `django_zana-0.3.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Django-Zana"
-version = "0.3.0a0"
+version = "0.3.0a1"
 description = "A `django` extension for `zana`."
 packages = [
     { include="zana" },
 ]
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 classifiers = [
@@ -30,26 +30,31 @@
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 ipython = "^8.10.0"
 django-polymorphic = "^3.1.0"
 tox = "^4.4.8"
+psycopg = "^3.1.8"
+mysqlclient = "^2.1.1"
 
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "^0.20.3"
 pytest-cov = {version = "^4.0.0", extras = ["toml"]}
 pytest-django = "^4.5.2"
 django-polymorphic = "^3.1.0"
 tox = "^4.4.8"
+mysqlclient = "^2.1.1"
+psycopg = "^3.1.8"
+django-environ = "^0.10.0"
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "*"
```

### Comparing `django_zana-0.3.0a0/zana/django/models/_xaliases.py` & `django_zana-0.3.0a1/zana/django/models/_xaliases.py`

 * *Files identical despite different names*

### Comparing `django_zana-0.3.0a0/zana/django/models/fields/__init__.py` & `django_zana-0.3.0a1/zana/django/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django_zana-0.3.0a0/zana/django/models/fields/aliases.py` & `django_zana-0.3.0a1/zana/django/models/fields/aliases.py`

 * *Files identical despite different names*

### Comparing `django_zana-0.3.0a0/PKG-INFO` & `django_zana-0.3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-zana
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: A `django` extension for `zana`.
 License: MIT
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

