# Comparing `tmp/invocations-3.0.2.tar.gz` & `tmp/invocations-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpubuqxkl9/dist/invocations-3.0.2.tar", last modified: Fri Apr 28 15:17:15 2023, max compression
+gzip compressed data, was "/tmp/tmpaphn4xr8/dist/invocations-3.1.0.tar", last modified: Tue May  2 21:15:20 2023, max compression
```

## Comparing `invocations-3.0.2.tar` & `invocations-3.1.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     3271 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      307 2023-01-16 22:33:01.000000 invocations-3.0.2/dev-requirements.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/invocations/packaging/
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.0.2/invocations/packaging/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/packaging/vendorize.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-16 22:33:01.000000 invocations-3.0.2/invocations/packaging/semantic_version_monkey.py
--rw-r--r--   0 jforcier  (1000) users      (100)    34040 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/packaging/release.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1982 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/checks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-16 22:33:01.000000 invocations-3.0.2/invocations/console.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.0.2/invocations/pytest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.0.2/invocations/watch.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/autodoc.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6534 2023-04-12 22:47:06.000000 invocations-3.0.2/invocations/docs.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.0.2/invocations/ci.py
--rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.0.2/invocations/environment.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.2/invocations/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-28 15:17:14.000000 invocations-3.0.2/invocations/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-16 22:33:01.000000 invocations-3.0.2/invocations/testing.py
--rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.0.2/invocations/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-28 15:17:15.000000 invocations-3.0.2/setup.cfg
--rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.0.2/README.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)    12161 2023-04-28 15:17:11.000000 invocations-3.0.2/docs/changelog.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/packaging.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.0.2/docs/api/ci.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/pytest.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/docs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/environment.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/console.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/api/autodoc.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.0.2/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.0.2/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2737 2023-04-28 15:16:14.000000 invocations-3.0.2/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.0.2/LICENSE
--rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-04-28 15:17:15.000000 invocations-3.0.2/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.0.2/MANIFEST.in
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/environment.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/
--rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/autodoc/base.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/autodoc/_support/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/api.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/index.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/
--rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/api.html
--rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/py-modindex.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_sources/
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/searchindex.js
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/language_data.js
--rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/basic.css
--rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/plus.png
--rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/minus.png
--rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/documentation_options.js
--rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/pygments.css
--rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/custom.css
--rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/searchtools.js
--rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/alabaster.css
--rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
--rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery.js
--rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/doctools.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/file.png
--rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/index.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/
--rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/objects.inv
--rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/.buildinfo
--rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/genindex.html
--rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.0.2/tests/autodoc/_support/docs/_build/search.html
--rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/autodoc/_support/mytasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/pytest_.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1066 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/console.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/packaging/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/packaging/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/unreleased_1.x_features.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/no_unreleased_1.x_features.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 15:17:15.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/otherversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/noversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/fakepackage/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/no_unreleased_1.1_bugs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.0.2/tests/packaging/_support/unreleased_1.1_bugs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    48944 2022-12-31 22:11:11.000000 invocations-3.0.2/tests/packaging/release.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3243 2022-10-29 02:26:37.000000 invocations-3.0.2/tests/checks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.1.0/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-02 21:15:20.000000 invocations-3.1.0/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)      295 2023-04-28 19:13:24.000000 invocations-3.1.0/dev-requirements.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3303 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/dependency_links.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations/
+-rw-r--r--   0 jforcier  (1000) users      (100)     6534 2023-04-12 22:47:06.000000 invocations-3.1.0/invocations/docs.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/autodoc.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.1.0/invocations/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-16 22:33:01.000000 invocations-3.1.0/invocations/testing.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.1.0/invocations/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations/packaging/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-16 22:33:01.000000 invocations-3.1.0/invocations/packaging/semantic_version_monkey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.1.0/invocations/packaging/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/packaging/vendorize.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    34493 2023-05-02 21:11:34.000000 invocations-3.1.0/invocations/packaging/release.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/ci.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.1.0/invocations/watch.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.1.0/invocations/environment.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-02 20:50:00.000000 invocations-3.1.0/invocations/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.1.0/invocations/pytest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1982 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/checks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-16 22:33:01.000000 invocations-3.1.0/invocations/console.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3243 2022-10-29 02:26:37.000000 invocations-3.1.0/tests/checks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/api.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_sources/
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/objects.inv
+-rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/py-modindex.html
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/pygments.css
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/minus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/alabaster.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/basic.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/file.png
+-rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/documentation_options.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/language_data.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/custom.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/searchtools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/doctools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/plus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/search.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/genindex.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/api.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/index.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/searchindex.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.buildinfo
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/
+-rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/mytasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/autodoc/_support/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/autodoc/base.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/packaging/
+-rw-r--r--   0 jforcier  (1000) users      (100)    73728 2023-05-02 21:11:42.000000 invocations-3.1.0/tests/packaging/.release.py.swp
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/packaging/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/unreleased_1.x_features.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/no_unreleased_1.1_bugs.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/otherversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/noversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/no_unreleased_1.x_features.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/unreleased_1.1_bugs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    50230 2023-05-02 21:11:45.000000 invocations-3.1.0/tests/packaging/release.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/console.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/environment.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1066 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/pytest_.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-02 21:15:20.000000 invocations-3.1.0/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     2737 2023-04-28 15:16:14.000000 invocations-3.1.0/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.1.0/LICENSE
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/docs/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.1.0/docs/api/ci.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/pytest.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/environment.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/packaging.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/autodoc.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/docs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/console.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.1.0/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12475 2023-05-02 21:15:20.000000 invocations-3.1.0/docs/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.1.0/MANIFEST.in
```

### Comparing `invocations-3.0.2/invocations.egg-info/PKG-INFO` & `invocations-3.1.0/invocations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.0.2
+Version: 3.1.0
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
```

### Comparing `invocations-3.0.2/invocations.egg-info/SOURCES.txt` & `invocations-3.1.0/invocations.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 tests/autodoc/_support/docs/_build/_static/minus.png
 tests/autodoc/_support/docs/_build/_static/plus.png
 tests/autodoc/_support/docs/_build/_static/pygments.css
 tests/autodoc/_support/docs/_build/_static/searchtools.js
 tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
 tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
 tests/autodoc/_support/docs/_build/_static/underscore.js
+tests/packaging/.release.py.swp
 tests/packaging/release.py
 tests/packaging/_support/conf.py
 tests/packaging/_support/index.rst
 tests/packaging/_support/no_unreleased_1.1_bugs.rst
 tests/packaging/_support/no_unreleased_1.x_features.rst
 tests/packaging/_support/unreleased_1.1_bugs.rst
 tests/packaging/_support/unreleased_1.x_features.rst
```

### Comparing `invocations-3.0.2/invocations/packaging/vendorize.py` & `invocations-3.1.0/invocations/packaging/vendorize.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/packaging/semantic_version_monkey.py` & `invocations-3.1.0/invocations/packaging/semantic_version_monkey.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/packaging/release.py` & `invocations-3.1.0/invocations/packaging/release.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import os
 import re
 import sys
 import venv
 from functools import partial
 from glob import glob
 from io import StringIO
+from pathlib import Path
 from shutil import rmtree
 
 from invoke.vendor.lexicon import Lexicon
 
 from blessings import Terminal
 from docutils.utils import Reporter
 from enum import Enum
@@ -533,14 +534,16 @@
     Uses the ``packaging.package`` config setting if defined. If not defined,
     fallback is to look for a single top-level Python package (directory
     containing ``__init__.py``). (This search ignores a small blacklist of
     directories like ``tests/``, ``vendor/`` etc.)
     """
     # TODO: is there a way to get this from the same place setup.py does w/o
     # setup.py barfing (since setup() runs at import time and assumes CLI use)?
+    # TODO Python 3.7: seems like a job for the then-in-stdlib
+    # importlib.metadata?
     configured_value = c.get("packaging", {}).get("package", None)
     if configured_value:
         return configured_value
     # TODO: tests covering this stuff here (most logic tests simply supply
     # config above)
     packages = [
         path
@@ -765,22 +768,25 @@
         # dry run)
         test_install(c, directory=tmp)
         # Do the thing! (Maybe.)
         upload(c, directory=tmp, index=index, sign=sign, dry_run=dry_run)
 
 
 @task
-def test_install(c, directory, verbose=False):
+def test_install(c, directory, verbose=False, skip_import=False):
     """
     Test installation of build artifacts found in ``$directory``.
 
     Directory should either be a ``dist`` directory itself, or the parent of
     one.
 
     Uses the `venv` module to build temporary virtualenvs.
+
+    :param bool verbose: Whether to print subprocess output.
+    :param bool skip_import: If True, don't try importing the installed module.
     """
     # TODO: wants contextmanager or similar for only altering a setting within
     # a given scope or block - this may pollute subsequent subroutine calls
     if verbose:
         old_hide = c.config.run.hide
         c.config.run.hide = False
 
@@ -791,25 +797,29 @@
     for archive in archives:
         with tmpdir() as tmp:
             # Make temp venv
             builder.create(tmp)
             # Obligatory: make inner pip match outer pip (version obtained from
             # this file's executable env, up in import land); very frequently
             # venv-made envs have a bundled, older pip :(
-            pip = os.path.join(tmp, "bin", "pip")
+            envbin = Path(tmp) / "bin"
+            pip = envbin / "pip"
             c.run("{} install pip=={}".format(pip, pip_version))
             # Does the package under test install cleanly?
-            # TODO: might be nice to have a further 'can you import whatever it
-            # was' test
             c.run(
                 "{} install --disable-pip-version-check {}".format(
                     pip, archive
                 )
             )
-            # TODO: install wheel and try again to make sure wheels work ok?
+            # Can we actually import it? (Will catch certain classes of
+            # import-time-but-not-install-time explosions, eg busted dependency
+            # specifications or imports).
+            if not skip_import:
+                package = _find_package(c)
+                c.run(f"{envbin / 'python'} -c 'import {package}'")
 
     if verbose:
         c.config.run.hide = old_hide
 
 
 def get_archives(directory):
     # Obtain list of archive filenames, then ensure any wheels come first
```

### Comparing `invocations-3.0.2/invocations/checks.py` & `invocations-3.1.0/invocations/checks.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/console.py` & `invocations-3.1.0/invocations/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/pytest.py` & `invocations-3.1.0/invocations/pytest.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/watch.py` & `invocations-3.1.0/invocations/watch.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/autodoc.py` & `invocations-3.1.0/invocations/autodoc.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/docs.py` & `invocations-3.1.0/invocations/docs.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/ci.py` & `invocations-3.1.0/invocations/ci.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/environment.py` & `invocations-3.1.0/invocations/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/testing.py` & `invocations-3.1.0/invocations/testing.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/invocations/util.py` & `invocations-3.1.0/invocations/util.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/README.rst` & `invocations-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/docs/changelog.rst` & `invocations-3.1.0/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+- :release:`3.1.0 <2023-05-02>`
+- :feature:`-` Updated ``packaging.release.test_install`` to attempt imports of
+  freshly test-installed packages, to catch import-time errors on top of
+  install-time ones. This can be opted out of by giving the ``skip_import``
+  kwarg (aka the ``--skip-import`` flag on the CLI).
 - :release:`3.0.2 <2023-04-28>`
 - :support:`- backported` Unpin ``tabulate`` in our install requirements, it's
   had many more releases since we instituted a defensive pin vs some bugs in
   its later 0.7 line!
 - :release:`3.0.1 <2023-01-06>`
 - :bug:`-` We neglected to remove references to ``six`` in a few spots -
   including some that utilized Invoke's old vendor of same; this causes issues
```

### Comparing `invocations-3.0.2/docs/conf.py` & `invocations-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/setup.py` & `invocations-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/LICENSE` & `invocations-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/PKG-INFO` & `invocations-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.0.2
+Version: 3.1.0
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
```

### Comparing `invocations-3.0.2/tests/environment.py` & `invocations-3.1.0/tests/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/base.py` & `invocations-3.1.0/tests/autodoc/base.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/api.html` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/api.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/py-modindex.html` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/searchindex.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/language_data.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/basic.css` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/pygments.css` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/searchtools.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/alabaster.css` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/jquery.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/underscore.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/doctools.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/index.html` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/api.doctree` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/.doctrees/index.doctree` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/genindex.html` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/autodoc/_support/docs/_build/search.html` & `invocations-3.1.0/tests/autodoc/_support/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/pytest_.py` & `invocations-3.1.0/tests/pytest_.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/conftest.py` & `invocations-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/console.py` & `invocations-3.1.0/tests/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.0.2/tests/packaging/release.py` & `invocations-3.1.0/tests/packaging/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,14 @@
 
     def undefined_always_returns_None_and_empty_list(self):
         skip()
 
 
 class find_package_:
     def can_be_short_circuited_with_config_value(self):
-        # TODO: should we just bundle this + the version part into one
-        # function and setting? do we ever peep into the package for anything
-        # else besides version module?
         skip()
 
     def seeks_directories_with_init_py_in_em(self):
         skip()
 
     def blacklists_common_non_public_modules(self):
         skip()
@@ -352,15 +349,15 @@
             parts = dict(
                 changelog=Changelog.NEEDS_RELEASE.value,
                 version=VersionFile.NEEDS_BUMP.value,
                 tag=Tag.NEEDS_CUTTING.value,
             )
             for part in parts:
                 parts[part] = re.escape(parts[part])
-            parts["header_footer"] = r"-+ +-+"
+            parts["header_footer"] = r"-+( +-+)?"
             # NOTE: forces impl to follow specific order, which is good
             regex = r"""
 {header_footer}
 Changelog +{changelog}
 Version +{version}
 Tag +{tag}
 {header_footer}
@@ -1206,14 +1203,15 @@
 
 class test_install_:
     @patch("invocations.packaging.release.pip_version", "lmao")
     @patch("invocations.packaging.release.get_archives")
     @patch("invocations.util.mkdtemp")
     @patch("invocations.util.rmtree", Mock("rmtree"))  # Just a neuter
     @patch("venv.EnvBuilder")
+    @patch("invocations.packaging.release._find_package", lambda c: "foo")
     def installs_all_archives_in_fresh_venv_with_matching_pip(
         self, builder, mkdtemp, get_archives
     ):
         # Setup & run
         c = MockContext(run=True, repeat=True)
         mkdtemp.return_value = "tmpdir"
         get_archives.return_value = ["foo.tgz", "foo.whl"]
@@ -1229,20 +1227,50 @@
         pip_base = "tmpdir/bin/pip install --disable-pip-version-check"
         c.run.assert_has_calls(
             [
                 # Pip installed to same version as running interpreter's pip
                 call("tmpdir/bin/pip install pip==lmao"),
                 # Archives installed into venv
                 call("{} foo.tgz".format(pip_base)),
+                # Import attempt was made
+                call("tmpdir/bin/python -c 'import foo'"),
                 # And repeat
                 call("tmpdir/bin/pip install pip==lmao"),
                 call("{} foo.whl".format(pip_base)),
+                call("tmpdir/bin/python -c 'import foo'"),
             ]
         )
 
+    @patch("invocations.packaging.release.pip_version", "lmao")
+    @patch("invocations.packaging.release.get_archives")
+    @patch("invocations.util.mkdtemp")
+    @patch("invocations.util.rmtree", Mock("rmtree"))  # Just a neuter
+    @patch("invocations.packaging.release._find_package", lambda c: "foo")
+    def skips_import_test_when_asked_to(self, mkdtemp, get_archives):
+        # Setup & run
+        c = MockContext(run=True, repeat=True)
+        mkdtemp.return_value = "tmpdir"
+        get_archives.return_value = ["foo.tgz", "foo.whl"]
+        install_test_task(c, directory="whatever", skip_import=True)
+        pip_base = "tmpdir/bin/pip install --disable-pip-version-check"
+        c.run.assert_has_calls(
+            [
+                # Pip installed to same version as running interpreter's pip
+                call("tmpdir/bin/pip install pip==lmao"),
+                # Archives installed into venv
+                call("{} foo.tgz".format(pip_base)),
+                # And repeat
+                call("tmpdir/bin/pip install pip==lmao"),
+                call("{} foo.whl".format(pip_base)),
+            ]
+        )
+        assert (
+            call("tmpdir/bin/python -c 'import foo'") not in c.run.mock_calls
+        )
+
 
 class push_:
     def pushes_with_follow_tags(self):
         "git-pushes with --follow-tags"
         c = MockContext(run=True)
         push(c)
         c.run.assert_called_once_with("git push --follow-tags --no-verify")
```

### Comparing `invocations-3.0.2/tests/checks.py` & `invocations-3.1.0/tests/checks.py`

 * *Files identical despite different names*

