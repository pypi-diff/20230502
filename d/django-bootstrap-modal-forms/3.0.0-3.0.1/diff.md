# Comparing `tmp/django-bootstrap-modal-forms-3.0.0.tar.gz` & `tmp/django-bootstrap-modal-forms-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap-modal-forms-3.0.0.tar", last modified: Tue May  2 09:25:10 2023, max compression
+gzip compressed data, was "django-bootstrap-modal-forms-3.0.1.tar", last modified: Tue May  2 13:06:29 2023, max compression
```

## Comparing `django-bootstrap-modal-forms-3.0.0.tar` & `django-bootstrap-modal-forms-3.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.104624 django-bootstrap-modal-forms-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36686 2023-05-02 09:25:10.104624 django-bootstrap-modal-forms-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35859 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.096624 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.092624 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.096624 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36686 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 09:25:10.000000 django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/examples/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/examples/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/setup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:25:10.104624 django-bootstrap-modal-forms-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:25:10.100624 django-bootstrap-modal-forms-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/tests_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-02 09:24:58.000000 django-bootstrap-modal-forms-3.0.0/tests/tests_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.401183 django-bootstrap-modal-forms-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-05-02 13:06:29.401183 django-bootstrap-modal-forms-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36236 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.397183 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.397183 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.397183 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.397183 django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-05-02 13:06:29.000000 django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 13:06:29.000000 django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:06:29.000000 django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 13:06:29.000000 django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 13:06:29.000000 django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.397183 django-bootstrap-modal-forms-3.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.401183 django-bootstrap-modal-forms-3.0.1/examples/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/examples/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.401183 django-bootstrap-modal-forms-3.0.1/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/setup/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/setup/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/setup/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:06:29.401183 django-bootstrap-modal-forms-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:29.401183 django-bootstrap-modal-forms-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/tests/tests_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-02 13:06:20.000000 django-bootstrap-modal-forms-3.0.1/tests/tests_unit.py
```

### Comparing `django-bootstrap-modal-forms-3.0.0/CHANGELOG.rst` & `django-bootstrap-modal-forms-3.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+3.0.1 (2023-05-02)
+==================
+
+- fix redirect in FormValidationMixin
+
 3.0.0 (2023-05-02)
 ==================
 
 - deprecate support for python < 3.8
 - deprecate support for Django < 3.2
 - deprecate SuccessMessageMixin
 - add FormValidationMixin
```

### Comparing `django-bootstrap-modal-forms-3.0.0/LICENSE.txt` & `django-bootstrap-modal-forms-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/PKG-INFO` & `django-bootstrap-modal-forms-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -20,21 +20,39 @@
 
 ============================
 Django Bootstrap Modal Forms
 ============================
 
 A Django plugin for creating AJAX driven forms in Bootstrap modal.
 
+.. contents:: **Table of Contents**
+   :depth: 2
+   :local:
+   :backlinks: none
+
 Live Demo
 =========
 
 Demo_
 
 .. _Demo: http://trco.silkym.com/dbmf/
 
+
+General information
+===================
+
+Opening an issue
+****************
+When reporting an issue for ``django-bootstrap-modal-forms`` package, please prepare a publicly available repository having the issue you are reporting. The clear reproduce is the optimal way towards resolution.
+
+Contribute
+**********
+This is an Open Source project and any contribution is highly appreciated.
+
+
 Test and experiment on your machine
 ===================================
 
 This repository includes ``Dockerfile`` and ``docker-compose.yml`` files so you can easily setup and start to experiment with ``django-bootstrap-modal-forms`` running inside of a container on your local machine. Any changes you make in ``bootstrap_modal_forms``, ``examples`` and ``test`` folders are reflected in the container (see docker-compose.yml) and the data stored in sqlite3 database are persistent even if you remove stopped container. Follow the steps below to run the app::
 
     $ clone repository
     $ cd django-bootstrap-modal-forms
@@ -1137,16 +1155,11 @@
           $("#filter-book").each(function () {
               $(this).modalForm({formURL: $(this).data('form-url')});
           });
           ...
         });
       </script>
 
-Contribute
-==========
-
-This is an Open Source project and any contribution is appreciated.
-
 License
 =======
 
 This project is licensed under the MIT License.
```

### Comparing `django-bootstrap-modal-forms-3.0.0/README.rst` & `django-bootstrap-modal-forms-3.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,38 @@
 ============================
 Django Bootstrap Modal Forms
 ============================
 
 A Django plugin for creating AJAX driven forms in Bootstrap modal.
 
+.. contents:: **Table of Contents**
+   :depth: 2
+   :local:
+   :backlinks: none
+
 Live Demo
 =========
 
 Demo_
 
 .. _Demo: http://trco.silkym.com/dbmf/
 
+
+General information
+===================
+
+Opening an issue
+****************
+When reporting an issue for ``django-bootstrap-modal-forms`` package, please prepare a publicly available repository having the issue you are reporting. The clear reproduce is the optimal way towards resolution.
+
+Contribute
+**********
+This is an Open Source project and any contribution is highly appreciated.
+
+
 Test and experiment on your machine
 ===================================
 
 This repository includes ``Dockerfile`` and ``docker-compose.yml`` files so you can easily setup and start to experiment with ``django-bootstrap-modal-forms`` running inside of a container on your local machine. Any changes you make in ``bootstrap_modal_forms``, ``examples`` and ``test`` folders are reflected in the container (see docker-compose.yml) and the data stored in sqlite3 database are persistent even if you remove stopped container. Follow the steps below to run the app::
 
     $ clone repository
     $ cd django-bootstrap-modal-forms
@@ -1117,16 +1135,11 @@
           $("#filter-book").each(function () {
               $(this).modalForm({formURL: $(this).data('form-url')});
           });
           ...
         });
       </script>
 
-Contribute
-==========
-
-This is an Open Source project and any contribution is appreciated.
-
 License
 =======
 
 This project is licensed under the MIT License.
```

### Comparing `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/generic.py` & `django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/generic.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/mixins.py` & `django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,12 +85,12 @@
         if isAjaxRequest:
             if asyncUpdate:
                 form.save()
             return HttpResponse(status=204)
         
         form.save()
         messages.success(self.request, self.success_message)
-        return HttpResponseRedirect(self.success_url)   
+        return HttpResponseRedirect(self.get_success_url())
 
 
 def is_ajax(meta):
     return 'HTTP_X_REQUESTED_WITH' in meta and meta['HTTP_X_REQUESTED_WITH'] == 'XMLHttpRequest'
```

### Comparing `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js` & `django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 3.0.0
+version : 3.0.1
 Copyright (c) 2023 Marcel Rupp
 */
 
 // Open modal & load the form at formURL to the modalContent element
 const modalFormCallback = function(settings) {
     let modal = document.querySelector(settings.modalID);
     let content = modal.querySelector(settings.modalContent);
```

### Comparing `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js` & `django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js` & `django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 3.0.0
+version : 3.0.1
 Copyright (c) 2023 Uroš Trstenjak
 https://github.com/trco/django-bootstrap-modal-forms
 */
 
 (function($) {
 
     // Open modal & load the form at formURL to the modalContent element
```

### Comparing `django-bootstrap-modal-forms-3.0.0/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js` & `django-bootstrap-modal-forms-3.0.1/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/PKG-INFO` & `django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -20,21 +20,39 @@
 
 ============================
 Django Bootstrap Modal Forms
 ============================
 
 A Django plugin for creating AJAX driven forms in Bootstrap modal.
 
+.. contents:: **Table of Contents**
+   :depth: 2
+   :local:
+   :backlinks: none
+
 Live Demo
 =========
 
 Demo_
 
 .. _Demo: http://trco.silkym.com/dbmf/
 
+
+General information
+===================
+
+Opening an issue
+****************
+When reporting an issue for ``django-bootstrap-modal-forms`` package, please prepare a publicly available repository having the issue you are reporting. The clear reproduce is the optimal way towards resolution.
+
+Contribute
+**********
+This is an Open Source project and any contribution is highly appreciated.
+
+
 Test and experiment on your machine
 ===================================
 
 This repository includes ``Dockerfile`` and ``docker-compose.yml`` files so you can easily setup and start to experiment with ``django-bootstrap-modal-forms`` running inside of a container on your local machine. Any changes you make in ``bootstrap_modal_forms``, ``examples`` and ``test`` folders are reflected in the container (see docker-compose.yml) and the data stored in sqlite3 database are persistent even if you remove stopped container. Follow the steps below to run the app::
 
     $ clone repository
     $ cd django-bootstrap-modal-forms
@@ -1137,16 +1155,11 @@
           $("#filter-book").each(function () {
               $(this).modalForm({formURL: $(this).data('form-url')});
           });
           ...
         });
       </script>
 
-Contribute
-==========
-
-This is an Open Source project and any contribution is appreciated.
-
 License
 =======
 
 This project is licensed under the MIT License.
```

### Comparing `django-bootstrap-modal-forms-3.0.0/django_bootstrap_modal_forms.egg-info/SOURCES.txt` & `django-bootstrap-modal-forms-3.0.1/django_bootstrap_modal_forms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/examples/forms.py` & `django-bootstrap-modal-forms-3.0.1/examples/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/examples/migrations/0001_initial.py` & `django-bootstrap-modal-forms-3.0.1/examples/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/examples/models.py` & `django-bootstrap-modal-forms-3.0.1/examples/models.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/examples/urls.py` & `django-bootstrap-modal-forms-3.0.1/examples/urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/examples/views.py` & `django-bootstrap-modal-forms-3.0.1/examples/views.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/setup/settings.py` & `django-bootstrap-modal-forms-3.0.1/setup/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/setup.py` & `django-bootstrap-modal-forms-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     README = readme_file.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-bootstrap-modal-forms',
-    version='3.0.0',
+    version='3.0.1',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A Django plugin for creating AJAX driven forms in Bootstrap modal.',
     long_description=README,
     url='https://github.com/trco/django-bootstrap-modal-forms',
     author='Uros Trstenjak',
```

### Comparing `django-bootstrap-modal-forms-3.0.0/tests/base.py` & `django-bootstrap-modal-forms-3.0.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/tests/tests_functional.py` & `django-bootstrap-modal-forms-3.0.1/tests/tests_functional.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.0/tests/tests_unit.py` & `django-bootstrap-modal-forms-3.0.1/tests/tests_unit.py`

 * *Files identical despite different names*

