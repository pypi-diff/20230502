# Comparing `tmp/django-bootstrap-modal-forms-2.2.1.tar.gz` & `tmp/django-bootstrap-modal-forms-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap-modal-forms-2.2.1.tar", last modified: Sun Mar  5 15:26:36 2023, max compression
+gzip compressed data, was "django-bootstrap-modal-forms-3.0.0.tar", last modified: Tue May  2 09:25:10 2023, max compression
```

## Comparing `django-bootstrap-modal-forms-2.2.1.tar` & `django-bootstrap-modal-forms-3.0.0.tar`

### file list

```diff
@@ -1,50 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.501241 django-bootstrap-modal-forms-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36008 2023-03-05 15:26:36.497241 django-bootstrap-modal-forms-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.493240 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.493240 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.497241 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.497241 django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36008 2023-03-05 15:26:36.000000 django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-05 15:26:36.000000 django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 15:26:36.000000 django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-05 15:26:36.000000 django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-05 15:26:36.000000 django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.497241 django-bootstrap-modal-forms-2.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.497241 django-bootstrap-modal-forms-2.2.1/examples/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/examples/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.497241 django-bootstrap-modal-forms-2.2.1/setup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/setup/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/setup/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/setup/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 15:26:36.501241 django-bootstrap-modal-forms-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:36.497241 django-bootstrap-modal-forms-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/tests/tests_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-03-05 15:26:22.000000 django-bootstrap-modal-forms-2.2.1/tests/tests_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.104624 django-bootstrap-modal-forms-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    36686 2023-05-02 09:25:10.104624 django-bootstrap-modal-forms-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35859 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.096624 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.092624 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.096624 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36686 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/examples/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:25:10.104624 django-bootstrap-modal-forms-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/tests_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/tests_unit.py
```

### Comparing `django-bootstrap-modal-forms-2.2.1/CHANGELOG.rst` & `django-bootstrap-modal-forms-3.0.0/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =========
 Changelog
 =========
 
+3.0.0 (2023-05-02)
+==================
+
+- deprecate support for python < 3.8
+- deprecate support for Django < 3.2
+- deprecate SuccessMessageMixin
+- add FormValidationMixin
+- add support for Chrome, Firefox, Edge and Safari drivers when running funtional tests
+- update examples to Django=4.2
+- update README.rst
+
 2.2.1 (2023-03-05)
 ==================
 
 - add support for Bootstrap5 without jQuery dependency
 - update documentation with Bootstrap5 examples
 
 2.2.0 (2021-04-27)
```

### Comparing `django-bootstrap-modal-forms-2.2.1/LICENSE.txt` & `django-bootstrap-modal-forms-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-2.2.1/PKG-INFO` & `django-bootstrap-modal-forms-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 2.2.1
+Version: 3.0.0
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
 
 ============================
 Django Bootstrap Modal Forms
 ============================
 
@@ -42,14 +37,21 @@
 This repository includes ``Dockerfile`` and ``docker-compose.yml`` files so you can easily setup and start to experiment with ``django-bootstrap-modal-forms`` running inside of a container on your local machine. Any changes you make in ``bootstrap_modal_forms``, ``examples`` and ``test`` folders are reflected in the container (see docker-compose.yml) and the data stored in sqlite3 database are persistent even if you remove stopped container. Follow the steps below to run the app::
 
     $ clone repository
     $ cd django-bootstrap-modal-forms
     $ docker compose up (use -d flag to run app in detached mode in the background)
     $ visit 0.0.0.0:8000
 
+Tests
+=====
+
+Run unit and functional tests inside of project folder::
+
+    $ python manage.py test
+
 Installation
 ============
 
 1. Install ``django-bootstrap-modal-forms``::
 
     $ pip install django-bootstrap-modal-forms
 
@@ -57,34 +59,34 @@
 
     INSTALLED_APPS = [
         ...
         'bootstrap_modal_forms',
         ...
     ]
 
-3. Include Bootstrap, jQuery and ``jquery.bootstrap.modal.forms.js`` on every page where you would like to set up the AJAX driven Django forms in Bootstrap modal.
-
-IMPORTANT: Adjust Bootstrap and jQuery file paths to match yours, but include ``jquery.bootstrap.modal.forms.js`` exactly as in code bellow.
+3. Include Bootstrap, jQuery and ``jquery.bootstrap(5).modal.forms.js`` on every page where you would like to set up the AJAX driven Django forms in Bootstrap modal. **IMPORTANT:** Adjust Bootstrap and jQuery file paths to match yours, but include ``jquery.bootstrap.modal.forms.js`` exactly as in code bellow.
 
 .. code-block:: html+django
 
     <head>
         <link rel="stylesheet" href="{% static 'assets/css/bootstrap.css' %}">
     </head>
 
     <body>
         <script src="{% static 'assets/js/bootstrap.js' %}"></script>
 
         <!-- Bootstrap 4 -->
-        <script src="{% static 'assets/js/jquery.js' %}"></script>
-        <script src="{% static 'js/jquery.bootstrap.modal.forms.js' %}"></script>
+        <script src="{% static 'assets/js/jquery-3.2.1.min.js' %}"></script>
+        <script src="{% static 'assets/js/popper.min.js' %}"></script>
+        <script src="{% static 'assets/js/bootstrap.min.js' %}"></script>
         <!-- You can alternatively load the minified version -->
-        <script src="{% static 'js/jquery.bootstrap.modal.forms.min.js' %}"></script>
+        <script src="{% static 'js/jquery.bootstrap.modal.forms.js' %}"></script>
 
         <!-- Bootstrap 5 -->
+        <script src="{% static 'assets/js/bootstrap.bundle.min.js' %}"></script>
         <script src="{% static 'js/bootstrap5.modal.forms.js' %}"></script>
         <!-- You can alternatively load the minified version -->
         <script src="{% static 'js/bootstrap5.modal.forms.min.js' %}"></script>
     </body>
 
 How it works?
 =============
@@ -465,41 +467,47 @@
 
 Mixins
 ======
 
 Import mixins with ``from bootstrap_modal_forms.mixins import PassRequestMixin``.
 
 PassRequestMixin
-    Puts the request into the form's kwargs.
+    Form Mixin which puts the request into the form's kwargs. Note: Using this mixin requires you to pop the `request` kwarg out of the dict in the super of your form's `__init__`. See PopRequestMixin.
 
 PopRequestMixin
-    Pops request out of the kwargs and attaches it to the form's instance.
+    Form Mixin which pops request out of the kwargs and attaches it to the form's instance. Note: This mixin must precede forms.ModelForm/forms.Form. The form is not expecting these kwargs to be passed in, so they must be popped off before anything else is done.
 
 CreateUpdateAjaxMixin
-    Saves or doesn't save the object based on the request type.
+    ModelForm Mixin which passes or saves object based on request type.
 
 DeleteMessageMixin
-    Deletes object if request is not ajax request.
+    Generic View Mixin which adds message to BSModalDeleteView and only calls the post method if request is not ajax request. In case request is ajax post method calls delete method, which redirects to success url.
+
+FormValidationMixin
+    Generic View Mixin which saves object and redirects to success_url if request is not ajax request. Otherwise response 204 No content is returned.
 
 LoginAjaxMixin
-    Authenticates user if request is not ajax request.
+    Generic View Mixin which authenticates user if request is not ajax request.
 
 Generic views
 =============
 
 Import generic views with ``from bootstrap_modal_forms.generic import BSModalFormView``.
 
+BSModalLoginView
+    Inhertis LoginAjaxMixin and Django's LoginView.
+
 BSModalFormView
     Inherits PassRequestMixin and Django's generic.FormView.
 
 BSModalCreateView
-    Inherits PassRequestMixin and Django's SuccessMessageMixin and generic.CreateView.
+    Inherits PassRequestMixin, FormValidationMixin and generic.CreateView.
 
 BSModalUpdateView
-    Inherits PassRequestMixin and Django's SuccessMessageMixin and generic.UpdateView.
+    Inherits PassRequestMixin, FormValidationMixin and generic.UpdateView.
 
 BSModalReadView
     Inherits Django's generic.DetailView.
 
 BSModalDeleteView
     Inherits DeleteMessageMixin and Django's generic.DeleteView.
 
@@ -510,21 +518,14 @@
 
     $ git clone https://github.com/trco/django-bootstrap-modal-forms.git
     $ cd django-bootstrap-modal-forms
     $ pip install -r requirements.txt
     $ python manage.py migrate
     $ python manage.py runserver
 
-Tests
-=====
-
-Run unit and functional tests inside of project folder::
-
-    $ python manage.py test
-
 Example 1: Signup form in Bootstrap modal
 *****************************************
 
 For explanation how all the parts of the code work together see paragraph **Usage**. To test the working solution presented here clone and run **Examples**.
 
 .. code-block:: python
```

### Comparing `django-bootstrap-modal-forms-2.2.1/README.rst` & `django-bootstrap-modal-forms-3.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 This repository includes ``Dockerfile`` and ``docker-compose.yml`` files so you can easily setup and start to experiment with ``django-bootstrap-modal-forms`` running inside of a container on your local machine. Any changes you make in ``bootstrap_modal_forms``, ``examples`` and ``test`` folders are reflected in the container (see docker-compose.yml) and the data stored in sqlite3 database are persistent even if you remove stopped container. Follow the steps below to run the app::
 
     $ clone repository
     $ cd django-bootstrap-modal-forms
     $ docker compose up (use -d flag to run app in detached mode in the background)
     $ visit 0.0.0.0:8000
 
+Tests
+=====
+
+Run unit and functional tests inside of project folder::
+
+    $ python manage.py test
+
 Installation
 ============
 
 1. Install ``django-bootstrap-modal-forms``::
 
     $ pip install django-bootstrap-modal-forms
 
@@ -32,34 +39,34 @@
 
     INSTALLED_APPS = [
         ...
         'bootstrap_modal_forms',
         ...
     ]
 
-3. Include Bootstrap, jQuery and ``jquery.bootstrap.modal.forms.js`` on every page where you would like to set up the AJAX driven Django forms in Bootstrap modal.
-
-IMPORTANT: Adjust Bootstrap and jQuery file paths to match yours, but include ``jquery.bootstrap.modal.forms.js`` exactly as in code bellow.
+3. Include Bootstrap, jQuery and ``jquery.bootstrap(5).modal.forms.js`` on every page where you would like to set up the AJAX driven Django forms in Bootstrap modal. **IMPORTANT:** Adjust Bootstrap and jQuery file paths to match yours, but include ``jquery.bootstrap.modal.forms.js`` exactly as in code bellow.
 
 .. code-block:: html+django
 
     <head>
         <link rel="stylesheet" href="{% static 'assets/css/bootstrap.css' %}">
     </head>
 
     <body>
         <script src="{% static 'assets/js/bootstrap.js' %}"></script>
 
         <!-- Bootstrap 4 -->
-        <script src="{% static 'assets/js/jquery.js' %}"></script>
-        <script src="{% static 'js/jquery.bootstrap.modal.forms.js' %}"></script>
+        <script src="{% static 'assets/js/jquery-3.2.1.min.js' %}"></script>
+        <script src="{% static 'assets/js/popper.min.js' %}"></script>
+        <script src="{% static 'assets/js/bootstrap.min.js' %}"></script>
         <!-- You can alternatively load the minified version -->
-        <script src="{% static 'js/jquery.bootstrap.modal.forms.min.js' %}"></script>
+        <script src="{% static 'js/jquery.bootstrap.modal.forms.js' %}"></script>
 
         <!-- Bootstrap 5 -->
+        <script src="{% static 'assets/js/bootstrap.bundle.min.js' %}"></script>
         <script src="{% static 'js/bootstrap5.modal.forms.js' %}"></script>
         <!-- You can alternatively load the minified version -->
         <script src="{% static 'js/bootstrap5.modal.forms.min.js' %}"></script>
     </body>
 
 How it works?
 =============
@@ -440,41 +447,47 @@
 
 Mixins
 ======
 
 Import mixins with ``from bootstrap_modal_forms.mixins import PassRequestMixin``.
 
 PassRequestMixin
-    Puts the request into the form's kwargs.
+    Form Mixin which puts the request into the form's kwargs. Note: Using this mixin requires you to pop the `request` kwarg out of the dict in the super of your form's `__init__`. See PopRequestMixin.
 
 PopRequestMixin
-    Pops request out of the kwargs and attaches it to the form's instance.
+    Form Mixin which pops request out of the kwargs and attaches it to the form's instance. Note: This mixin must precede forms.ModelForm/forms.Form. The form is not expecting these kwargs to be passed in, so they must be popped off before anything else is done.
 
 CreateUpdateAjaxMixin
-    Saves or doesn't save the object based on the request type.
+    ModelForm Mixin which passes or saves object based on request type.
 
 DeleteMessageMixin
-    Deletes object if request is not ajax request.
+    Generic View Mixin which adds message to BSModalDeleteView and only calls the post method if request is not ajax request. In case request is ajax post method calls delete method, which redirects to success url.
+
+FormValidationMixin
+    Generic View Mixin which saves object and redirects to success_url if request is not ajax request. Otherwise response 204 No content is returned.
 
 LoginAjaxMixin
-    Authenticates user if request is not ajax request.
+    Generic View Mixin which authenticates user if request is not ajax request.
 
 Generic views
 =============
 
 Import generic views with ``from bootstrap_modal_forms.generic import BSModalFormView``.
 
+BSModalLoginView
+    Inhertis LoginAjaxMixin and Django's LoginView.
+
 BSModalFormView
     Inherits PassRequestMixin and Django's generic.FormView.
 
 BSModalCreateView
-    Inherits PassRequestMixin and Django's SuccessMessageMixin and generic.CreateView.
+    Inherits PassRequestMixin, FormValidationMixin and generic.CreateView.
 
 BSModalUpdateView
-    Inherits PassRequestMixin and Django's SuccessMessageMixin and generic.UpdateView.
+    Inherits PassRequestMixin, FormValidationMixin and generic.UpdateView.
 
 BSModalReadView
     Inherits Django's generic.DetailView.
 
 BSModalDeleteView
     Inherits DeleteMessageMixin and Django's generic.DeleteView.
 
@@ -485,21 +498,14 @@
 
     $ git clone https://github.com/trco/django-bootstrap-modal-forms.git
     $ cd django-bootstrap-modal-forms
     $ pip install -r requirements.txt
     $ python manage.py migrate
     $ python manage.py runserver
 
-Tests
-=====
-
-Run unit and functional tests inside of project folder::
-
-    $ python manage.py test
-
 Example 1: Signup form in Bootstrap modal
 *****************************************
 
 For explanation how all the parts of the code work together see paragraph **Usage**. To test the working solution presented here clone and run **Examples**.
 
 .. code-block:: python
```

### Comparing `django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/compatibility.py` & `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/mixins.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,96 @@
-from django.conf import settings
-from django.contrib.auth import REDIRECT_FIELD_NAME, get_user_model, login as auth_login
-from django.contrib.auth.forms import AuthenticationForm
-from django.contrib.sites.shortcuts import get_current_site
-from django.http import HttpResponseRedirect
-from django.shortcuts import resolve_url
-from django.utils.decorators import method_decorator
-from django.utils.http import is_safe_url
-from django.views.decorators.cache import never_cache
-from django.views.decorators.csrf import csrf_protect
-from django.views.decorators.debug import sensitive_post_parameters
-from django.views.generic.edit import FormView
-
-
-class SuccessURLAllowedHostsMixin:
-    success_url_allowed_hosts = set()
-
-    def get_success_url_allowed_hosts(self):
-        return {self.request.get_host(), *self.success_url_allowed_hosts}
-
-
-class LoginView(SuccessURLAllowedHostsMixin, FormView):
-    """
-    Display the login form and handle the login action.
-    """
-    form_class = AuthenticationForm
-    authentication_form = None
-    redirect_field_name = REDIRECT_FIELD_NAME
-    template_name = 'registration/login.html'
-    redirect_authenticated_user = False
-    extra_context = None
-
-    @method_decorator(sensitive_post_parameters())
-    @method_decorator(csrf_protect)
-    @method_decorator(never_cache)
-    def dispatch(self, request, *args, **kwargs):
-        if self.redirect_authenticated_user and self.request.user.is_authenticated:
-            redirect_to = self.get_success_url()
-            if redirect_to == self.request.path:
-                raise ValueError(
-                    'Redirection loop for authenticated user detected. Check that '
-                    'your LOGIN_REDIRECT_URL doesn\'t point to a login page.'
-                )
-            return HttpResponseRedirect(redirect_to)
-        return super().dispatch(request, *args, **kwargs)
-
-    def get_success_url(self):
-        url = self.get_redirect_url()
-        return url or resolve_url(settings.LOGIN_REDIRECT_URL)
-
-    def get_redirect_url(self):
-        """Return the user-originating redirect URL if it's safe."""
-        redirect_to = self.request.POST.get(
-            self.redirect_field_name,
-            self.request.GET.get(self.redirect_field_name, '')
-        )
-        url_is_safe = is_safe_url(
-            url=redirect_to
-        )
-        return redirect_to if url_is_safe else ''
+from django.contrib import messages
+from django.contrib.auth import login as auth_login
+from django.http import HttpResponseRedirect, HttpResponse
 
-    def get_form_class(self):
-        return self.authentication_form or self.form_class
+class PassRequestMixin:
+    """
+    Form Mixin which puts the request into the form's kwargs.
+
+    Note: Using this mixin requires you to pop the `request` kwarg
+    out of the dict in the super of your form's `__init__`.
+    """
 
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
         kwargs['request'] = self.request
         return kwargs
 
+
+class PopRequestMixin:
+    """
+    Form Mixin which pops request out of the kwargs and attaches it to the form's
+    instance.
+
+    Note: This mixin must precede forms.ModelForm/forms.Form. The form is not
+    expecting these kwargs to be passed in, so they must be popped off before
+    anything else is done.
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        self.request = kwargs.pop('request', None)
+        super().__init__(*args, **kwargs)
+
+
+class CreateUpdateAjaxMixin:
+    """
+    ModelForm Mixin which passes or saves object based on request type.
+    """
+
+    def save(self, commit=True):
+        isAjaxRequest = is_ajax(self.request.META)
+        asyncUpdate = self.request.POST.get('asyncUpdate') == 'True'
+
+        if not isAjaxRequest or asyncUpdate:
+            return super().save(commit=commit)
+        if isAjaxRequest:
+            return super().save(commit=False)
+
+
+class DeleteMessageMixin:
+    """
+    Generic View Mixin which adds message to BSModalDeleteView and only calls the post method if request
+    is not ajax request. In case request is ajax post method calls delete method, which redirects to success url.
+    """
+
+    def post(self, request, *args, **kwargs):
+        if not is_ajax(request.META):
+            messages.success(request, self.success_message)
+            return super().post(request, *args, **kwargs)
+        else:
+            self.object = self.get_object()
+            return HttpResponseRedirect(self.get_success_url())
+
+
+class LoginAjaxMixin:
+    """
+    Generic View Mixin which authenticates user if request is not ajax request.
+    """
+
     def form_valid(self, form):
-        """Security check complete. Log the user in."""
-        auth_login(self.request, form.get_user())
+        if not is_ajax(self.request.META):
+            auth_login(self.request, form.get_user())
+            messages.success(self.request, self.success_message)
         return HttpResponseRedirect(self.get_success_url())
 
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-        current_site = get_current_site(self.request)
-        context.update({
-            self.redirect_field_name: self.get_redirect_url(),
-            'site': current_site,
-            'site_name': current_site.name,
-            **(self.extra_context or {})
-        })
-        return context
+
+class FormValidationMixin:
+    """
+    Generic View Mixin which saves object and redirects to success_url if request is not ajax request. Otherwise response 204 No content is returned.
+    """
+        
+    def form_valid(self, form):
+        isAjaxRequest = is_ajax(self.request.META)
+        asyncUpdate = self.request.POST.get('asyncUpdate') == 'True'
+
+        if isAjaxRequest:
+            if asyncUpdate:
+                form.save()
+            return HttpResponse(status=204)
+        
+        form.save()
+        messages.success(self.request, self.success_message)
+        return HttpResponseRedirect(self.success_url)   
+
+
+def is_ajax(meta):
+    return 'HTTP_X_REQUESTED_WITH' in meta and meta['HTTP_X_REQUESTED_WITH'] == 'XMLHttpRequest'
```

### Comparing `django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/generic.py` & `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/generic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-import django
-from django.contrib.messages.views import SuccessMessageMixin
 from django.views import generic
-from .mixins import PassRequestMixin, DeleteMessageMixin, LoginAjaxMixin
+from django.contrib.auth.views import LoginView
 
-DJANGO_VERSION = django.get_version().split('.')
-DJANGO_MAJOR_VERSION = DJANGO_VERSION[0]
-DJANGO_MINOR_VERSION = DJANGO_VERSION[1]
+from .mixins import PassRequestMixin, DeleteMessageMixin, LoginAjaxMixin, FormValidationMixin
 
-# Import custom LoginView for Django versions < 1.11
-if DJANGO_MAJOR_VERSION == '1' and '11' not in DJANGO_MINOR_VERSION:
-    from .compatibility import LoginView
-else:
-    from django.contrib.auth.views import LoginView
 
-
-class BSModalLoginView(LoginAjaxMixin, SuccessMessageMixin, LoginView):
+class BSModalLoginView(LoginAjaxMixin, LoginView):
     pass
 
 
 class BSModalFormView(PassRequestMixin, generic.FormView):
     pass
 
 
-class BSModalCreateView(PassRequestMixin, SuccessMessageMixin, generic.CreateView):
+class BSModalCreateView(PassRequestMixin, FormValidationMixin, generic.CreateView):
     pass
 
 
-class BSModalUpdateView(PassRequestMixin, SuccessMessageMixin, generic.UpdateView):
+class BSModalUpdateView(PassRequestMixin, FormValidationMixin, generic.UpdateView):
     pass
 
 
 class BSModalReadView(generic.DetailView):
     pass
```

### Comparing `django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js` & `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 2.2.1
+version : 3.0.0
 Copyright (c) 2023 Marcel Rupp
 */
 
 // Open modal & load the form at formURL to the modalContent element
 const modalFormCallback = function(settings) {
     let modal = document.querySelector(settings.modalID);
     let content = modal.querySelector(settings.modalContent);
@@ -21,15 +21,15 @@
     }).then(data => {
         content.innerHTML = data;
     }).then(() => {
         modalInstance.show();
 
         let form = modal.querySelector(settings.modalForm);
         if (form) {
-            form.action = settings.formURL;
+            form.setAttribute("action", settings.formURL);
             addEventHandlers(modal, form, settings)
         }
     });
 };
 
 const addEventHandlers = function(modal, form, settings) {
     form.addEventListener('submit', (event) => {
@@ -53,31 +53,31 @@
     let modal = document.querySelector(settings.modalID);
     let form = modal.querySelector(settings.modalForm);
     const headers = new Headers();
     headers.append('X-Requested-With', 'XMLHttpRequest');
 
     let btnSubmit = modal.querySelector('button[type="submit"]');
     btnSubmit.disabled = true;
-    fetch(form.action, {
+    fetch(form.getAttribute("action"), {
         headers: headers,
-        method: form.method,
+        method: form.getAttribute("method"),
         body: new FormData(form),
     }).then(res => {
         return res.text();
     }).then(data => {
         if (data.includes(settings.errorClass)) {
             modal.querySelector(settings.modalContent).innerHTML = data;
 
             form = modal.querySelector(settings.modalForm);
             if (!form) {
                 console.error('no form present in response')
                 return;
             }
 
-            form.action = settings.formURL;
+            form.setAttribute("action", settings.formURL);
             addEventHandlers(modal, form, settings)
         } else {
             callback(settings);
         }
     });
 };
 
@@ -93,16 +93,16 @@
         if (asyncSettingsValid) {
             let asyncSettings = settings.asyncSettings;
             // Serialize form data
             let formData = new FormData(form);
             // Add asyncUpdate and check for it in save method of CreateUpdateAjaxMixin
             formData.append("asyncUpdate", "True");
 
-            fetch(form.action, {
-                method: form.method,
+            fetch(form.getAttribute("action"), {
+                method: form.getAttribute("method"),
                 body: formData,
             }).then(res => {
                 return res.text();
             }).then(data => {
                 let body = document.body;
                 if (body === undefined) {
                     console.error("django-bootstrap-modal-forms: <body> element missing in your html.");
@@ -138,29 +138,28 @@
 
                                 form = modal.querySelector(settings.modalForm);
                                 if (!form) {
                                     console.error('no form present in response')
                                     return;
                                 }
 
-                                form.action = settings.formURL;
+                                form.setAttribute("action", settings.formURL);
                                 addEventHandlers(modal, form, settings)
                             });
                         }
                     });
                 } else if (asyncSettings.closeOnSubmit) {
                     bootstrap.Modal.getInstance(modal).hide();
                 }
             });
         }
     }
 };
 
 const validateAsyncSettings = function(settings) {
-    console.log(settings)
     var missingSettings = [];
 
     if (!settings.successMessage) {
         missingSettings.push("successMessage");
         console.error("django-bootstrap-modal-forms: 'successMessage' in asyncSettings is missing.");
     }
     if (!settings.dataUrl) {
```

### Comparing `django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js` & `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 2.2.1
+version : 3.0.0
 Copyright (c) 2023 Uroš Trstenjak
 https://github.com/trco/django-bootstrap-modal-forms
 */
 
 (function($) {
 
     // Open modal & load the form at formURL to the modalContent element
```

### Comparing `django-bootstrap-modal-forms-2.2.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js` & `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/PKG-INFO` & `django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 2.2.1
+Version: 3.0.0
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
 
 ============================
 Django Bootstrap Modal Forms
 ============================
 
@@ -42,14 +37,21 @@
 This repository includes ``Dockerfile`` and ``docker-compose.yml`` files so you can easily setup and start to experiment with ``django-bootstrap-modal-forms`` running inside of a container on your local machine. Any changes you make in ``bootstrap_modal_forms``, ``examples`` and ``test`` folders are reflected in the container (see docker-compose.yml) and the data stored in sqlite3 database are persistent even if you remove stopped container. Follow the steps below to run the app::
 
     $ clone repository
     $ cd django-bootstrap-modal-forms
     $ docker compose up (use -d flag to run app in detached mode in the background)
     $ visit 0.0.0.0:8000
 
+Tests
+=====
+
+Run unit and functional tests inside of project folder::
+
+    $ python manage.py test
+
 Installation
 ============
 
 1. Install ``django-bootstrap-modal-forms``::
 
     $ pip install django-bootstrap-modal-forms
 
@@ -57,34 +59,34 @@
 
     INSTALLED_APPS = [
         ...
         'bootstrap_modal_forms',
         ...
     ]
 
-3. Include Bootstrap, jQuery and ``jquery.bootstrap.modal.forms.js`` on every page where you would like to set up the AJAX driven Django forms in Bootstrap modal.
-
-IMPORTANT: Adjust Bootstrap and jQuery file paths to match yours, but include ``jquery.bootstrap.modal.forms.js`` exactly as in code bellow.
+3. Include Bootstrap, jQuery and ``jquery.bootstrap(5).modal.forms.js`` on every page where you would like to set up the AJAX driven Django forms in Bootstrap modal. **IMPORTANT:** Adjust Bootstrap and jQuery file paths to match yours, but include ``jquery.bootstrap.modal.forms.js`` exactly as in code bellow.
 
 .. code-block:: html+django
 
     <head>
         <link rel="stylesheet" href="{% static 'assets/css/bootstrap.css' %}">
     </head>
 
     <body>
         <script src="{% static 'assets/js/bootstrap.js' %}"></script>
 
         <!-- Bootstrap 4 -->
-        <script src="{% static 'assets/js/jquery.js' %}"></script>
-        <script src="{% static 'js/jquery.bootstrap.modal.forms.js' %}"></script>
+        <script src="{% static 'assets/js/jquery-3.2.1.min.js' %}"></script>
+        <script src="{% static 'assets/js/popper.min.js' %}"></script>
+        <script src="{% static 'assets/js/bootstrap.min.js' %}"></script>
         <!-- You can alternatively load the minified version -->
-        <script src="{% static 'js/jquery.bootstrap.modal.forms.min.js' %}"></script>
+        <script src="{% static 'js/jquery.bootstrap.modal.forms.js' %}"></script>
 
         <!-- Bootstrap 5 -->
+        <script src="{% static 'assets/js/bootstrap.bundle.min.js' %}"></script>
         <script src="{% static 'js/bootstrap5.modal.forms.js' %}"></script>
         <!-- You can alternatively load the minified version -->
         <script src="{% static 'js/bootstrap5.modal.forms.min.js' %}"></script>
     </body>
 
 How it works?
 =============
@@ -465,41 +467,47 @@
 
 Mixins
 ======
 
 Import mixins with ``from bootstrap_modal_forms.mixins import PassRequestMixin``.
 
 PassRequestMixin
-    Puts the request into the form's kwargs.
+    Form Mixin which puts the request into the form's kwargs. Note: Using this mixin requires you to pop the `request` kwarg out of the dict in the super of your form's `__init__`. See PopRequestMixin.
 
 PopRequestMixin
-    Pops request out of the kwargs and attaches it to the form's instance.
+    Form Mixin which pops request out of the kwargs and attaches it to the form's instance. Note: This mixin must precede forms.ModelForm/forms.Form. The form is not expecting these kwargs to be passed in, so they must be popped off before anything else is done.
 
 CreateUpdateAjaxMixin
-    Saves or doesn't save the object based on the request type.
+    ModelForm Mixin which passes or saves object based on request type.
 
 DeleteMessageMixin
-    Deletes object if request is not ajax request.
+    Generic View Mixin which adds message to BSModalDeleteView and only calls the post method if request is not ajax request. In case request is ajax post method calls delete method, which redirects to success url.
+
+FormValidationMixin
+    Generic View Mixin which saves object and redirects to success_url if request is not ajax request. Otherwise response 204 No content is returned.
 
 LoginAjaxMixin
-    Authenticates user if request is not ajax request.
+    Generic View Mixin which authenticates user if request is not ajax request.
 
 Generic views
 =============
 
 Import generic views with ``from bootstrap_modal_forms.generic import BSModalFormView``.
 
+BSModalLoginView
+    Inhertis LoginAjaxMixin and Django's LoginView.
+
 BSModalFormView
     Inherits PassRequestMixin and Django's generic.FormView.
 
 BSModalCreateView
-    Inherits PassRequestMixin and Django's SuccessMessageMixin and generic.CreateView.
+    Inherits PassRequestMixin, FormValidationMixin and generic.CreateView.
 
 BSModalUpdateView
-    Inherits PassRequestMixin and Django's SuccessMessageMixin and generic.UpdateView.
+    Inherits PassRequestMixin, FormValidationMixin and generic.UpdateView.
 
 BSModalReadView
     Inherits Django's generic.DetailView.
 
 BSModalDeleteView
     Inherits DeleteMessageMixin and Django's generic.DeleteView.
 
@@ -510,21 +518,14 @@
 
     $ git clone https://github.com/trco/django-bootstrap-modal-forms.git
     $ cd django-bootstrap-modal-forms
     $ pip install -r requirements.txt
     $ python manage.py migrate
     $ python manage.py runserver
 
-Tests
-=====
-
-Run unit and functional tests inside of project folder::
-
-    $ python manage.py test
-
 Example 1: Signup form in Bootstrap modal
 *****************************************
 
 For explanation how all the parts of the code work together see paragraph **Usage**. To test the working solution presented here clone and run **Examples**.
 
 .. code-block:: python
```

### Comparing `django-bootstrap-modal-forms-2.2.1/django_bootstrap_modal_forms.egg-info/SOURCES.txt` & `django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 CHANGELOG.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
 bootstrap_modal_forms/__init__.py
-bootstrap_modal_forms/compatibility.py
 bootstrap_modal_forms/forms.py
 bootstrap_modal_forms/generic.py
 bootstrap_modal_forms/mixins.py
-bootstrap_modal_forms/utils.py
 bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
 bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
 bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
 bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
 django_bootstrap_modal_forms.egg-info/PKG-INFO
 django_bootstrap_modal_forms.egg-info/SOURCES.txt
 django_bootstrap_modal_forms.egg-info/dependency_links.txt
 django_bootstrap_modal_forms.egg-info/requires.txt
 django_bootstrap_modal_forms.egg-info/top_level.txt
 examples/__init__.py
-examples/admin.py
 examples/apps.py
 examples/forms.py
 examples/models.py
-examples/tests.py
 examples/urls.py
 examples/views.py
 examples/migrations/0001_initial.py
 examples/migrations/__init__.py
 setup/__init__.py
 setup/settings.py
 setup/urls.py
```

### Comparing `django-bootstrap-modal-forms-2.2.1/examples/forms.py` & `django-bootstrap-modal-forms-3.0.0/examples/forms.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
         model = User
         fields = ['username', 'password1', 'password2']
 
 
 class CustomAuthenticationForm(AuthenticationForm):
     class Meta:
         model = User
-        fields = ['username', 'password']
+        fields = ['username', 'password']
```

### Comparing `django-bootstrap-modal-forms-2.2.1/examples/migrations/0001_initial.py` & `django-bootstrap-modal-forms-3.0.0/examples/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 2.1 on 2019-03-30 16:15
+# Generated by Django 3.2 on 2023-04-09 15:22
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
@@ -10,15 +10,15 @@
     dependencies = [
     ]
 
     operations = [
         migrations.CreateModel(
             name='Book',
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('title', models.CharField(max_length=50)),
                 ('publication_date', models.DateField(null=True)),
                 ('author', models.CharField(blank=True, max_length=30)),
                 ('price', models.DecimalField(decimal_places=2, max_digits=5)),
                 ('pages', models.IntegerField(blank=True, null=True)),
                 ('book_type', models.PositiveSmallIntegerField(choices=[(1, 'Hardcover'), (2, 'Paperback'), (3, 'E-book')])),
                 ('timestamp', models.DateField(auto_now_add=True)),
```

### Comparing `django-bootstrap-modal-forms-2.2.1/examples/models.py` & `django-bootstrap-modal-forms-3.0.0/examples/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     title = models.CharField(max_length=50)
     publication_date = models.DateField(null=True)
     author = models.CharField(max_length=30, blank=True)
     price = models.DecimalField(max_digits=5, decimal_places=2)
     pages = models.IntegerField(blank=True, null=True)
     book_type = models.PositiveSmallIntegerField(choices=BOOK_TYPES)
 
-    timestamp = models.DateField(auto_now_add=True, auto_now=False)
+    timestamp = models.DateField(auto_now_add=True, auto_now=False)
```

### Comparing `django-bootstrap-modal-forms-2.2.1/examples/urls.py` & `django-bootstrap-modal-forms-3.0.0/examples/urls.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
     path('create/', views.BookCreateView.as_view(), name='create_book'),
     path('update/<int:pk>', views.BookUpdateView.as_view(), name='update_book'),
     path('read/<int:pk>', views.BookReadView.as_view(), name='read_book'),
     path('delete/<int:pk>', views.BookDeleteView.as_view(), name='delete_book'),
     path('books/', views.books, name='books'),
     path('signup/', views.SignUpView.as_view(), name='signup'),
     path('login/', views.CustomLoginView.as_view(), name='login'),
-]
+]
```

### Comparing `django-bootstrap-modal-forms-2.2.1/examples/views.py` & `django-bootstrap-modal-forms-3.0.0/examples/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from django.http import JsonResponse
 from django.template.loader import render_to_string
-from django.contrib.messages.views import SuccessMessageMixin
 from django.urls import reverse_lazy
 from django.views import generic
 
 from bootstrap_modal_forms.generic import (
     BSModalLoginView,
     BSModalFormView,
     BSModalCreateView,
@@ -85,16 +84,16 @@
     authentication_form = CustomAuthenticationForm
     template_name = 'examples/login.html'
     success_message = 'Success: You were successfully logged in.'
     success_url = reverse_lazy('index')
 
 
 def books(request):
-    data = dict()
+    data = {}
     if request.method == 'GET':
         books = Book.objects.all()
         data['table'] = render_to_string(
             '_books_table.html',
             {'books': books},
             request=request
         )
-        return JsonResponse(data)
+        return JsonResponse(data)
```

### Comparing `django-bootstrap-modal-forms-2.2.1/setup/settings.py` & `django-bootstrap-modal-forms-3.0.0/setup/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
+from pathlib import Path
 
-
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+BASE_DIR = Path(__file__).resolve().parent.parent
 SECRET_KEY = 'ke2rim3a=ukld9cjh6$d$fb%ztgobvrs807i^d!_whg%@n^%v#'
 DEBUG = True
 
 ALLOWED_HOSTS = ['*']
 
 INSTALLED_APPS = [
     'django.contrib.admin',
@@ -28,20 +28,17 @@
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
 ]
 
 ROOT_URLCONF = 'setup.urls'
 
-PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
-
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [os.path.join(BASE_DIR, 'examples/templates'), ],
         'APP_DIRS': True,
         'OPTIONS': {
             'context_processors': [
                 'django.template.context_processors.debug',
                 'django.template.context_processors.request',
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
@@ -51,51 +48,37 @@
 ]
 
 WSGI_APPLICATION = 'setup.wsgi.application'
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': os.path.join(BASE_DIR, 'database/db.sqlite3'),
+        'NAME': str(Path(BASE_DIR, 'db.sqlite3')),
     }
 }
 
-AUTH_PASSWORD_VALIDATORS = [
-    {
-        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
-    },
-]
+DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
+
+# No password rules in development
+AUTH_PASSWORD_VALIDATORS = []
+# Simple (and unsecure) but fast password hasher in development
+PASSWORD_HASHERS = ['django.contrib.auth.hashers.MD5PasswordHasher']
 
 LOGIN_REDIRECT_URL = '/'
 LOGOUT_REDIRECT_URL = '/'
 
 LANGUAGE_CODE = 'en-us'
-
 TIME_ZONE = 'UTC'
 
-USE_I18N = True
-
-USE_L10N = True
-
-USE_TZ = True
+# No internationalization for this project
+USE_I18N = False
+USE_L10N = False
+USE_TZ = False
 
 STATICFILES_FINDERS = [
     # searches in STATICFILES_DIRS
     'django.contrib.staticfiles.finders.FileSystemFinder',
     # searches in STATIC subfolder of each app
     'django.contrib.staticfiles.finders.AppDirectoriesFinder',
 ]
 
 STATIC_URL = '/static/'
-
-STATICFILES_DIRS = [
-    os.path.join(BASE_DIR, 'static'),
-]
```

### Comparing `django-bootstrap-modal-forms-2.2.1/tests/tests_functional.py` & `django-bootstrap-modal-forms-3.0.0/tests/tests_functional.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from examples.models import Book
 from .base import FunctionalTest
 
 
 class SignUpLoginTest(FunctionalTest):
     def test_signup_login(self):
         # User visits homepage and checks the content
-        self.browser.get(self.live_server_url)
-        self.assertIn('django-bootstrap-modal-forms', self.browser.title)
-        header_text = self.browser.find_element_by_tag_name('h1').text
+        self.BROWSER.get(self.live_server_url)
+        self.assertIn('django-bootstrap-modal-forms', self.BROWSER.title)
+        header_text = self.BROWSER.find_element_by_tag_name('h1').text
         self.assertIn('django-bootstrap-modal-forms', header_text)
 
         # User clicks Sign up button
-        self.browser.find_element_by_id('signup-btn').click()
+        self.BROWSER.find_element_by_id('signup-btn').click()
 
         # Sign up modal opens
         modal = self.wait_for(element_id='modal')
 
         # User fills in and submits sign up form with misspelled second password
         form = modal.find_element_by_tag_name('form')
         username_field = form.find_element_by_id('id_username')
@@ -37,22 +37,22 @@
         password1_field = form.find_element_by_id('id_password1')
         password2_field = form.find_element_by_id('id_password2')
         password1_field.send_keys('pass12345')
         password2_field.send_keys('pass12345')
         form.submit()
 
         # User sees success message after page redirection
-        redirect_url = self.browser.current_url
+        redirect_url = self.BROWSER.current_url
         self.assertRegex(redirect_url, '/')
         # Slice removes '\nx' since alert is dismissible and contains 'times' button
         success_msg = self.wait_for(class_name='alert').text[:-2]
         self.assertEqual(success_msg, 'Success: Sign up succeeded. You can now Log in.')
 
         # User clicks log in button
-        self.browser.find_element_by_id('login-btn').click()
+        self.BROWSER.find_element_by_id('login-btn').click()
 
         # Log in modal opens
         modal = self.wait_for(element_id='modal')
 
         # User fills in and submits log in form with misspelled username
         form = modal.find_element_by_tag_name('form')
         username_field = form.find_element_by_id('id_username')
@@ -76,15 +76,15 @@
         username_field.send_keys('user')
         password_field.send_keys('pass12345')
         form.submit()
 
         # User sees log out button after page redirection
         logout_btn_txt = self.wait_for(element_id='logout-btn').text
         self.assertEqual(logout_btn_txt, 'Log out')
-        redirect_url = self.browser.current_url
+        redirect_url = self.BROWSER.current_url
         self.assertRegex(redirect_url, '/')
 
 
 class CRUDActionsTest(FunctionalTest):
     def setUp(self):
         super().setUp()
         self.book = Book.objects.create(
@@ -94,18 +94,18 @@
             price=19,
             pages=477,
             book_type=1,
         )
 
     def test_create_object(self):
         # User visits homepage
-        self.browser.get(self.live_server_url)
+        self.BROWSER.get(self.live_server_url)
 
         # User clicks create book button
-        self.browser.find_element_by_id('create-book-sync').click()
+        self.BROWSER.find_element_by_id('create-book-sync').click()
 
         # Create book modal opens
         modal = self.wait_for(element_id='create-modal')
 
         # User fills in and submits the form with wrong date format
         form = self.wait_for(tag='form')
 
@@ -136,15 +136,15 @@
         publication_date_field = form.find_element_by_id('id_publication_date')
         publication_date_field.clear()
         publication_date_field.send_keys('2019-01-01')
         
         form.submit()
 
         # User sees success message after page redirection
-        redirect_url = self.browser.current_url
+        redirect_url = self.BROWSER.current_url
         self.assertRegex(redirect_url, '/')
 
         # Slice removes '\nx' since alert is dismissible and contains 'times' button
         success_msg = self.wait_for(class_name='alert').text[:-2]
         self.assertEqual(success_msg, 'Success: Book was created.')
 
         # User sees created book in table
@@ -156,42 +156,42 @@
             table_entries[1],
             7,
             ['Life of Jane Doe', 'Jane Doe', 'Hardcover', 'Jan. 1, 2019', '464', '21.00', None],
         )
 
     def test_filter_object(self):
         # User visits homepage
-        self.browser.get(self.live_server_url)
+        self.BROWSER.get(self.live_server_url)
 
         # User clicks filter book button
         self.wait_for(element_id='filter-book').click()
 
         # Update filter modal opens
         modal = self.wait_for(element_id='modal')
 
         # User changes book type
         form = modal.find_element_by_tag_name('form')   
         
-        book_type = self.browser.find_element_by_id("id_type")
+        book_type = self.BROWSER.find_element_by_id("id_type")
         book_type_select = Select(book_type)
         book_type_select.select_by_index(0)
 
         form.submit()
 
         # User is redirected to the homepage with a querystring with the filter
         self.wait_for(class_name='filtered-books')
-        redirect_url = self.browser.current_url
+        redirect_url = self.BROWSER.current_url
         self.assertRegex(redirect_url, '/?type=1$')
 
     def test_update_object(self):
         # User visits homepage
-        self.browser.get(self.live_server_url)
+        self.BROWSER.get(self.live_server_url)
 
         # User clicks update book button
-        self.browser.find_element_by_class_name('update-book').click()
+        self.BROWSER.find_element_by_class_name('update-book').click()
 
         # Update book modal opens
         modal = self.wait_for(element_id='modal')
 
         # User changes price and book type
         form = modal.find_element_by_tag_name('form')
         
@@ -202,15 +202,15 @@
 
         title_field.send_keys('Life of Jane and John Doe')
         book_type_select.select_by_index(2)
 
         form.submit()
 
         # User sees success message after page redirection
-        redirect_url = self.browser.current_url
+        redirect_url = self.BROWSER.current_url
         self.assertRegex(redirect_url, '/')
 
         # Slice removes '\nx' since alert is dismissible and contains 'times' button
         success_msg = self.wait_for(class_name='alert').text[:-2]
         self.assertEqual(success_msg, 'Success: Book was updated.')
 
         # User sees updated book in table
@@ -230,18 +230,18 @@
                 '19.00',
                 None,
             ],
         )
 
     def test_read_object(self):
         # User visits homepage
-        self.browser.get(self.live_server_url)
+        self.BROWSER.get(self.live_server_url)
 
         # User clicks Read book button
-        self.browser.find_element_by_class_name('read-book').click()
+        self.BROWSER.find_element_by_class_name('read-book').click()
 
         # Read book modal opens
         modal = self.wait_for(element_id='modal')
 
         # User sees book content
         modal_body = modal.find_element_by_class_name('modal-body')
         divs = modal_body.find_elements_by_tag_name('div')
@@ -250,32 +250,32 @@
         self.assertEqual(divs[2].text, 'Price: 19.00 €')
         self.assertEqual(divs[3].text, 'Pages: 477')
         self.assertEqual(divs[4].text, 'Type: Hardcover')
         self.assertEqual(divs[5].text, 'Publication date: Feb. 2, 2017')
 
     def test_delete_object(self):
         # User visits homepage
-        self.browser.get(self.live_server_url)
+        self.BROWSER.get(self.live_server_url)
 
         # User clicks Delete book button
-        self.browser.find_element_by_class_name('delete-book').click()
+        self.BROWSER.find_element_by_class_name('delete-book').click()
 
         # Delete book modal opens
         modal = self.wait_for(element_id='modal')
         delete_text = modal.find_element_by_class_name('delete-text').text
         self.assertEqual(
             delete_text, 'Are you sure you want to delete book with title Life of John Doe?'
         )
 
         # User clicks delete button
         delete_btn = modal.find_element_by_id('delete-btn')
         delete_btn.click()
 
         # User sees success message after page redirection
-        redirect_url = self.browser.current_url
+        redirect_url = self.BROWSER.current_url
         self.assertRegex(redirect_url, '/')
 
         # Slice removes '\nx' since alert is dismissible and contains 'times' button
         alert = self.wait_for(class_name='alert')
         self.assertEqual(alert.text[:-2], 'Success: Book was deleted.')
 
         # There is no books in database anymore
```

### Comparing `django-bootstrap-modal-forms-2.2.1/tests/tests_unit.py` & `django-bootstrap-modal-forms-3.0.0/tests/tests_unit.py`

 * *Files identical despite different names*

