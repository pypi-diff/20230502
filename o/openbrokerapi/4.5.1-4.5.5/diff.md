# Comparing `tmp/openbrokerapi-4.5.1.tar.gz` & `tmp/openbrokerapi-4.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbrokerapi-4.5.1.tar", max compression
+gzip compressed data, was "openbrokerapi-4.5.5.tar", max compression
```

## Comparing `openbrokerapi-4.5.1.tar` & `openbrokerapi-4.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1065 2023-04-26 09:13:32.818504 openbrokerapi-4.5.1/LICENSE
--rw-r--r--   0        0        0     6596 2023-04-26 09:13:32.818504 openbrokerapi-4.5.1/README.rst
--rw-r--r--   0        0        0     1375 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/__init__.py
--rw-r--r--   0        0        0    25386 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/api.py
--rw-r--r--   0        0        0     1830 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/auth.py
--rw-r--r--   0        0        0     2328 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/catalog.py
--rw-r--r--   0        0        0      333 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/constants.py
--rw-r--r--   0        0        0     2051 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/errors.py
--rw-r--r--   0        0        0     1009 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/helper.py
--rw-r--r--   0        0        0     1057 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/log_util.py
--rw-r--r--   0        0        0     2762 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/request_filter.py
--rw-r--r--   0        0        0     2641 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/response.py
--rw-r--r--   0        0        0     4148 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/router.py
--rw-r--r--   0        0        0    17197 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/service_broker.py
--rw-r--r--   0        0        0      400 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/settings.py
--rw-r--r--   0        0        0     2358 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/pyproject.toml
--rw-r--r--   0        0        0     8267 1970-01-01 00:00:00.000000 openbrokerapi-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-02 07:24:07.988857 openbrokerapi-4.5.5/LICENSE
+-rw-r--r--   0        0        0     6821 2023-05-02 07:24:07.988857 openbrokerapi-4.5.5/README.rst
+-rw-r--r--   0        0        0     1375 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/__init__.py
+-rw-r--r--   0        0        0    25386 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/api.py
+-rw-r--r--   0        0        0     1830 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/auth.py
+-rw-r--r--   0        0        0     2328 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/catalog.py
+-rw-r--r--   0        0        0      333 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/constants.py
+-rw-r--r--   0        0        0     2051 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/errors.py
+-rw-r--r--   0        0        0     1009 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/helper.py
+-rw-r--r--   0        0        0     1057 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/log_util.py
+-rw-r--r--   0        0        0     2762 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/request_filter.py
+-rw-r--r--   0        0        0     2641 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/response.py
+-rw-r--r--   0        0        0     4148 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/router.py
+-rw-r--r--   0        0        0    17197 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/service_broker.py
+-rw-r--r--   0        0        0      400 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/openbrokerapi/settings.py
+-rw-r--r--   0        0        0     2358 2023-05-02 07:24:07.992857 openbrokerapi-4.5.5/pyproject.toml
+-rw-r--r--   0        0        0     8492 1970-01-01 00:00:00.000000 openbrokerapi-4.5.5/PKG-INFO
```

### Comparing `openbrokerapi-4.5.1/LICENSE` & `openbrokerapi-4.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/README.rst` & `openbrokerapi-4.5.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|Build Status| |Coverage Status| |Known Vulnerabilities| |PYUP|
+|Build Status| |Coverage Status| |Known Vulnerabilities| |PYUP| |OpenSSF Best Practices|
 
 Open Broker API
 ===============
 
 A Python package for building Service Brokers supporting API version 2.13+.
 
 Following `Open Service Broker
@@ -17,15 +17,15 @@
 `Platform Compatibility for OSBAPI <https://github.com/openservicebrokerapi/servicebroker/blob/master/compatibility.md>`__
 
  Not all features are supported with this library due to conflicting features.
 
 Installation
 ------------
 
-This package is available for Python 3.6+.
+This package is available for Python 3.8+.
 
 .. code:: bash
 
     pip3 install openbrokerapi
 
     # including gevent as server
     pip3 install openbrokerapi[gevent]
@@ -159,19 +159,19 @@
 
     - Use a new branch for every Pull Request
     - Include just related commits in this branch
     - Less commits are better, one would be the best (You can squash them.)
     - Always add tests for your feature, if you are not familiar with writing tests, ask for help.
     - Hint: To update your fork with the newest changes, follow `these instructions <https://stackoverflow.com/a/7244456/2947505>`_.
 
-[ ~ Dependencies scanned by PyUp.io ~ ]
-
 .. _Github Issues: https://github.com/eruvanos/openbrokerapi/issues
 
 .. |Build Status| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml/badge.svg
     :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/eruvanos/openbrokerapi/badge.svg?branch=master
    :target: https://coveralls.io/github/eruvanos/openbrokerapi?branch=main
 .. |Known Vulnerabilities| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml/badge.svg
    :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml
 .. |PYUP| image:: https://pyup.io/repos/github/eruvanos/openbrokerapi/shield.svg
      :target: https://pyup.io/repos/github/eruvanos/openbrokerapi/
+.. |OpenSSF Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/7220/badge
+     :target: https://bestpractices.coreinfrastructure.org/projects/7220/badge)](https://bestpractices.coreinfrastructure.org/projects/7220
```

### Comparing `openbrokerapi-4.5.1/openbrokerapi/__init__.py` & `openbrokerapi-4.5.5/openbrokerapi/__init__.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/api.py` & `openbrokerapi-4.5.5/openbrokerapi/api.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/auth.py` & `openbrokerapi-4.5.5/openbrokerapi/auth.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/catalog.py` & `openbrokerapi-4.5.5/openbrokerapi/catalog.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/errors.py` & `openbrokerapi-4.5.5/openbrokerapi/errors.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/helper.py` & `openbrokerapi-4.5.5/openbrokerapi/helper.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/log_util.py` & `openbrokerapi-4.5.5/openbrokerapi/log_util.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/request_filter.py` & `openbrokerapi-4.5.5/openbrokerapi/request_filter.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/response.py` & `openbrokerapi-4.5.5/openbrokerapi/response.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/router.py` & `openbrokerapi-4.5.5/openbrokerapi/router.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/openbrokerapi/service_broker.py` & `openbrokerapi-4.5.5/openbrokerapi/service_broker.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.1/pyproject.toml` & `openbrokerapi-4.5.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbrokerapi"
-version = "4.5.1"
+version = "4.5.5"
 description = "A python package for the V2 CF Service Broker API and Open Broker API (version 2.13+)"
 authors = ["Maic Siemering <maic@siemering.tech>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://openbrokerapi.readthedocs.io/"
 documentation = "https://openbrokerapi.readthedocs.io/"
 repository = "https://github.com/eruvanos/openbrokerapi"
@@ -50,19 +50,19 @@
 Sphinx = {version = "^6.1.3", optional = true}
 sphinx-rtd-theme = {version = "^1.2.0", optional = true}
 gevent = {version = "^22.10.2", optional = true}
 gunicorn = {version = "^20.1.0", optional = true}
 
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3.1"
 Flask-Testing = "^0.8.1"
 requests = "^2.28.2"
-black = "^23.1.0"
-pre-commit = "^3.0.4"
+black = "^23.3.0"
+pre-commit = "^3.2.2"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx_rtd_theme"]
 gevent = ["gevent"]
 gunicorn = ["gunicorn"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `openbrokerapi-4.5.1/PKG-INFO` & `openbrokerapi-4.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbrokerapi
-Version: 4.5.1
+Version: 4.5.5
 Summary: A python package for the V2 CF Service Broker API and Open Broker API (version 2.13+)
 Home-page: https://openbrokerapi.readthedocs.io/
 License: MIT
 Keywords: cloudfoundry,cfbrokerapi,openbrokerapi,openservicebrokerapi,servicebroker,flask,kubernetes,k8s
 Author: Maic Siemering
 Author-email: maic@siemering.tech
 Requires-Python: >=3.8,<4.0
@@ -31,15 +31,15 @@
 Requires-Dist: gevent (>=22.10.2,<23.0.0) ; extra == "gevent"
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "gunicorn"
 Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0) ; extra == "docs"
 Project-URL: Documentation, https://openbrokerapi.readthedocs.io/
 Project-URL: Repository, https://github.com/eruvanos/openbrokerapi
 Description-Content-Type: text/x-rst
 
-|Build Status| |Coverage Status| |Known Vulnerabilities| |PYUP|
+|Build Status| |Coverage Status| |Known Vulnerabilities| |PYUP| |OpenSSF Best Practices|
 
 Open Broker API
 ===============
 
 A Python package for building Service Brokers supporting API version 2.13+.
 
 Following `Open Service Broker
@@ -54,15 +54,15 @@
 `Platform Compatibility for OSBAPI <https://github.com/openservicebrokerapi/servicebroker/blob/master/compatibility.md>`__
 
  Not all features are supported with this library due to conflicting features.
 
 Installation
 ------------
 
-This package is available for Python 3.6+.
+This package is available for Python 3.8+.
 
 .. code:: bash
 
     pip3 install openbrokerapi
 
     # including gevent as server
     pip3 install openbrokerapi[gevent]
@@ -196,20 +196,20 @@
 
     - Use a new branch for every Pull Request
     - Include just related commits in this branch
     - Less commits are better, one would be the best (You can squash them.)
     - Always add tests for your feature, if you are not familiar with writing tests, ask for help.
     - Hint: To update your fork with the newest changes, follow `these instructions <https://stackoverflow.com/a/7244456/2947505>`_.
 
-[ ~ Dependencies scanned by PyUp.io ~ ]
-
 .. _Github Issues: https://github.com/eruvanos/openbrokerapi/issues
 
 .. |Build Status| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml/badge.svg
     :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/eruvanos/openbrokerapi/badge.svg?branch=master
    :target: https://coveralls.io/github/eruvanos/openbrokerapi?branch=main
 .. |Known Vulnerabilities| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml/badge.svg
    :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml
 .. |PYUP| image:: https://pyup.io/repos/github/eruvanos/openbrokerapi/shield.svg
      :target: https://pyup.io/repos/github/eruvanos/openbrokerapi/
+.. |OpenSSF Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/7220/badge
+     :target: https://bestpractices.coreinfrastructure.org/projects/7220/badge)](https://bestpractices.coreinfrastructure.org/projects/7220
```

