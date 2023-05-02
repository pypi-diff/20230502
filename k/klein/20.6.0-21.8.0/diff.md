# Comparing `tmp/klein-20.6.0.tar.gz` & `tmp/klein-21.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/klein-20.6.0.tar", last modified: Mon Jun  8 02:52:10 2020, max compression
+gzip compressed data, was "klein-21.8.0.tar", last modified: Sun Aug  8 18:33:34 2021, max compression
```

## Comparing `klein-20.6.0.tar` & `klein-21.8.0.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.841849 klein-20.6.0/
--rw-r--r--   0 wsanchez   (502) staff       (20)      244 2020-06-08 02:52:09.000000 klein-20.6.0/.coveragerc
--rw-r--r--   0 wsanchez   (502) staff       (20)      232 2020-06-08 02:52:09.000000 klein-20.6.0/AUTHORS
--rw-r--r--   0 wsanchez   (502) staff       (20)     4991 2020-06-08 02:52:09.000000 klein-20.6.0/CONTRIBUTING.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     1108 2020-06-08 02:52:09.000000 klein-20.6.0/LICENSE
--rw-r--r--   0 wsanchez   (502) staff       (20)      296 2020-06-08 02:52:09.000000 klein-20.6.0/MANIFEST.in
--rw-r--r--   0 wsanchez   (502) staff       (20)     3181 2020-06-08 02:52:09.000000 klein-20.6.0/NEWS.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     3846 2020-06-08 02:52:10.842006 klein-20.6.0/PKG-INFO
--rw-r--r--   0 wsanchez   (502) staff       (20)     2367 2020-06-08 02:52:09.000000 klein-20.6.0/README.rst
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.815702 klein-20.6.0/docs/
--rw-r--r--   0 wsanchez   (502) staff       (20)     5560 2020-06-08 02:52:09.000000 klein-20.6.0/docs/Makefile
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.815997 klein-20.6.0/docs/_extensions/
--rw-r--r--   0 wsanchez   (502) staff       (20)     1353 2020-06-08 02:52:09.000000 klein-20.6.0/docs/_extensions/apilinks.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1348 2020-06-08 02:52:09.000000 klein-20.6.0/docs/conf.py
--rw-r--r--   0 wsanchez   (502) staff       (20)       51 2020-06-08 02:52:09.000000 klein-20.6.0/docs/contributing.rst
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.818933 klein-20.6.0/docs/examples/
--rw-r--r--   0 wsanchez   (502) staff       (20)     2741 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/alternativerunning.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)      725 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/await.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)      702 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/deferreds.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     1940 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/disablingtracebacks.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     2505 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/handlingerrors.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     2012 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/handlingpost.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     1379 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/nonglobalstate.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)      822 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/staticfiles.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     1366 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/subroutes.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     1056 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/templates.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)      922 2020-06-08 02:52:09.000000 klein-20.6.0/docs/examples/twistd.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     1356 2020-06-08 02:52:09.000000 klein-20.6.0/docs/index.rst
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.824226 klein-20.6.0/docs/introduction/
--rw-r--r--   0 wsanchez   (502) staff       (20)     9256 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/1-gettingstarted.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)     2123 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/2-twistdtap.rst
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.827061 klein-20.6.0/docs/introduction/codeexamples/
--rw-r--r--   0 wsanchez   (502) staff       (20)     1496 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/forms.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      231 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/googleProxy.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      112 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/helloWorld.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      129 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/helloWorldClass.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      222 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/moreRoutes.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      245 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/orderMatters.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      177 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/staticFiles.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2652 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/template.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      127 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/twistdPlugin.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      164 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/variableRoutes.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      330 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/codeexamples/variableRoutesTypes.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      725 2020-06-08 02:52:09.000000 klein-20.6.0/docs/introduction/twistdwebman.txt
--rw-r--r--   0 wsanchez   (502) staff       (20)     1010 2020-06-08 02:52:09.000000 klein-20.6.0/docs/release.rst
--rw-r--r--   0 wsanchez   (502) staff       (20)      150 2020-06-08 02:52:09.000000 klein-20.6.0/pyproject.toml
--rw-r--r--   0 wsanchez   (502) staff       (20)       61 2020-06-08 02:52:10.842455 klein-20.6.0/setup.cfg
--rw-r--r--   0 wsanchez   (502) staff       (20)     1962 2020-06-08 02:52:09.000000 klein-20.6.0/setup.py
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.811216 klein-20.6.0/src/
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.833692 klein-20.6.0/src/klein/
--rw-r--r--   0 wsanchez   (502) staff       (20)     1267 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/__init__.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    14795 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_app.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     3567 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_decorators.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     4206 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_dihttp.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    26045 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_form.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     5122 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_headers.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2266 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_headers_compat.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      483 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_iapp.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      463 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_iform.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     5781 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_imessage.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1736 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_interfaces.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    12859 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_isession.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2058 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_message.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    10372 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_plating.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1286 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_request.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2879 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_request_compat.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     5692 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_requirer.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     9275 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_resource.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1179 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_response.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    12494 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_session.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2302 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_tubes.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      531 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_typing.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      254 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/_version.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      298 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/app.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2370 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/interfaces.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1657 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/resource.py
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.835723 klein-20.6.0/src/klein/storage/
--rw-r--r--   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/storage/__init__.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     4941 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/storage/_memory.py
--rw-r--r--   0 wsanchez   (502) staff       (20)      137 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/storage/memory.py
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.841626 klein-20.6.0/src/klein/test/
--rw-r--r--   0 wsanchez   (502) staff       (20)      299 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/__init__.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     8754 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/_strategies.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1796 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/_trial.py
--rw-r--r--   0 wsanchez   (502) staff       (20)   134586 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/idna-tables-properties.csv
--rw-r--r--   0 wsanchez   (502) staff       (20)     1677 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/py3_test_resource.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    17573 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_app.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1940 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_exports.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    27303 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_form.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    17165 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_headers.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2536 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_headers_compat.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     2375 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_memory.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     4893 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_message.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    19471 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_plating.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1743 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_request.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     5496 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_request_compat.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     5214 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_requirer.py
--rw-r--r--   0 wsanchez   (502) staff       (20)    37306 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_resource.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1562 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_response.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     8955 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_session.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     1529 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/test_trial.py
--rw-r--r--   0 wsanchez   (502) staff       (20)     3719 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein/test/util.py
-drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2020-06-08 02:52:10.835019 klein-20.6.0/src/klein.egg-info/
--rw-r--r--   0 wsanchez   (502) staff       (20)     3846 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein.egg-info/PKG-INFO
--rw-r--r--   0 wsanchez   (502) staff       (20)     2667 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein.egg-info/SOURCES.txt
--rw-r--r--   0 wsanchez   (502) staff       (20)        1 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein.egg-info/dependency_links.txt
--rw-r--r--   0 wsanchez   (502) staff       (20)      144 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein.egg-info/requires.txt
--rw-r--r--   0 wsanchez   (502) staff       (20)        6 2020-06-08 02:52:10.000000 klein-20.6.0/src/klein.egg-info/top_level.txt
--rw-r--r--   0 wsanchez   (502) staff       (20)    11786 2020-06-08 02:52:10.000000 klein-20.6.0/tox.ini
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.712772 klein-21.8.0/
+-rw-r--r--   0 wsanchez   (502) staff       (20)      352 2021-08-08 18:33:34.000000 klein-21.8.0/.codecov.yml
+-rw-r--r--   0 wsanchez   (502) staff       (20)      260 2021-08-08 18:33:34.000000 klein-21.8.0/.coveragerc
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1852 2021-08-08 18:33:34.000000 klein-21.8.0/.flake8
+-rw-r--r--   0 wsanchez   (502) staff       (20)      428 2021-08-08 18:33:34.000000 klein-21.8.0/.isort.cfg
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2463 2021-08-08 18:33:34.000000 klein-21.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 wsanchez   (502) staff       (20)      518 2021-08-08 18:33:34.000000 klein-21.8.0/.readthedocs.yml
+-rw-r--r--   0 wsanchez   (502) staff       (20)      233 2021-08-08 18:33:34.000000 klein-21.8.0/AUTHORS
+-rw-r--r--   0 wsanchez   (502) staff       (20)     5011 2021-08-08 18:33:34.000000 klein-21.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1108 2021-08-08 18:33:34.000000 klein-21.8.0/LICENSE
+-rw-r--r--   0 wsanchez   (502) staff       (20)      477 2021-08-08 18:33:34.000000 klein-21.8.0/MANIFEST.in
+-rw-r--r--   0 wsanchez   (502) staff       (20)     3940 2021-08-08 18:33:34.000000 klein-21.8.0/NEWS.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     3499 2021-08-08 18:33:34.712842 klein-21.8.0/PKG-INFO
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2404 2021-08-08 18:33:34.000000 klein-21.8.0/README.rst
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.702986 klein-21.8.0/docs/
+-rw-r--r--   0 wsanchez   (502) staff       (20)     5560 2021-08-08 18:33:34.000000 klein-21.8.0/docs/Makefile
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.703119 klein-21.8.0/docs/_extensions/
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1417 2021-08-08 18:33:34.000000 klein-21.8.0/docs/_extensions/apilinks.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1411 2021-08-08 18:33:34.000000 klein-21.8.0/docs/conf.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)       52 2021-08-08 18:33:34.000000 klein-21.8.0/docs/contributing.rst
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.704515 klein-21.8.0/docs/examples/
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2741 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/alternativerunning.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)      725 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/await.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)      702 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/deferreds.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1940 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/disablingtracebacks.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2484 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/handlingerrors.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1998 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/handlingpost.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1371 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/nonglobalstate.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1554 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/staticfiles.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1366 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/subroutes.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1056 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/templates.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)      922 2021-08-08 18:33:34.000000 klein-21.8.0/docs/examples/twistd.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1291 2021-08-08 18:33:34.000000 klein-21.8.0/docs/index.rst
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.704885 klein-21.8.0/docs/introduction/
+-rw-r--r--   0 wsanchez   (502) staff       (20)     9255 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/1-gettingstarted.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2123 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/2-twistdtap.rst
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.706278 klein-21.8.0/docs/introduction/codeexamples/
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1482 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/forms.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      236 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/googleProxy.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      114 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/helloWorld.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      133 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/helloWorldClass.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      227 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/moreRoutes.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      245 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/orderMatters.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      182 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/staticFiles.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2709 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/template.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      131 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/twistdPlugin.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      163 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/variableRoutes.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      321 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/codeexamples/variableRoutesTypes.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      725 2021-08-08 18:33:34.000000 klein-21.8.0/docs/introduction/twistdwebman.txt
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1010 2021-08-08 18:33:34.000000 klein-21.8.0/docs/release.rst
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1737 2021-08-08 18:33:34.000000 klein-21.8.0/mypy.ini
+-rw-r--r--   0 wsanchez   (502) staff       (20)      150 2021-08-08 18:33:34.000000 klein-21.8.0/pyproject.toml
+-rw-r--r--   0 wsanchez   (502) staff       (20)     8433 2021-08-08 18:33:34.000000 klein-21.8.0/release.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)       61 2021-08-08 18:33:34.713070 klein-21.8.0/setup.cfg
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2046 2021-08-08 18:33:34.000000 klein-21.8.0/setup.py
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.699601 klein-21.8.0/src/
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.709540 klein-21.8.0/src/klein/
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1386 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/__init__.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    19529 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_app.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     3439 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_decorators.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     4038 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_dihttp.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    25624 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_form.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     4842 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_headers.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2541 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_headers_compat.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      428 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_iform.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     5489 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_imessage.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      855 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_interfaces.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    12337 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_isession.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1789 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_message.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     9905 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_plating.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1130 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_request.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2557 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_request_compat.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     5134 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_requirer.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    10241 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_resource.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1040 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_response.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    11400 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_session.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1962 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_tubes.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      254 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/_version.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      298 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/app.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      770 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/interfaces.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1609 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/resource.py
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.710474 klein-21.8.0/src/klein/storage/
+-rw-r--r--   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/storage/__init__.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     4757 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/storage/_memory.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      138 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/storage/memory.py
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.712664 klein-21.8.0/src/klein/test/
+-rw-r--r--   0 wsanchez   (502) staff       (20)      343 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/__init__.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)      845 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/_trial.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    17548 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_app.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1845 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_exports.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    26159 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_form.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    17763 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_headers.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2476 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_headers_compat.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2276 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_memory.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     5031 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_message.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    19476 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_plating.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1669 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_request.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     5747 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_request_compat.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     5291 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_requirer.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)    43755 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_resource.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1516 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_response.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     8550 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_session.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     1429 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/test_trial.py
+-rw-r--r--   0 wsanchez   (502) staff       (20)     4491 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein/test/util.py
+drwxr-xr-x   0 wsanchez   (502) staff       (20)        0 2021-08-08 18:33:34.710170 klein-21.8.0/src/klein.egg-info/
+-rw-r--r--   0 wsanchez   (502) staff       (20)     3499 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein.egg-info/PKG-INFO
+-rw-r--r--   0 wsanchez   (502) staff       (20)     2644 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein.egg-info/SOURCES.txt
+-rw-r--r--   0 wsanchez   (502) staff       (20)        1 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein.egg-info/dependency_links.txt
+-rw-r--r--   0 wsanchez   (502) staff       (20)        1 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein.egg-info/not-zip-safe
+-rw-r--r--   0 wsanchez   (502) staff       (20)      117 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein.egg-info/requires.txt
+-rw-r--r--   0 wsanchez   (502) staff       (20)        6 2021-08-08 18:33:34.000000 klein-21.8.0/src/klein.egg-info/top_level.txt
+-rw-r--r--   0 wsanchez   (502) staff       (20)     8942 2021-08-08 18:33:34.000000 klein-21.8.0/tox.ini
```

### Comparing `klein-20.6.0/CONTRIBUTING.rst` & `klein-21.8.0/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 =====================
 Contributing to Klein
 =====================
 
 Klein is an open source project that welcomes contributions of all kinds coming from the community, including:
 
 - code patches,
-- `documentation <http://klein.readthedocs.org/>`_ improvements,
+- `documentation <https://klein.readthedocs.io/en/latest/>`_ improvements,
 - `bug reports <https://github.com/twisted/klein/issues>`_,
 - reviews for `contributed patches <https://github.com/twisted/klein/pulls>`_.
 
 
 Getting started
 ===============
 
-Here is a list of shell commands that will install the dependencies of Klein, run the test suite with Python 2.7 and the current version of Twisted, compile the documentation, and check for coding style issues with flake8.
+Here is a list of shell commands that will install the dependencies of Klein, run the test suite with Python 3.8 and the current version of Twisted, compile the documentation, and check for coding style issues with flake8.
 
 .. code-block:: shell
 
    pip install --user tox
-   tox -e py27-twcurrent
+   tox -e py38-twcurrent
    tox -e docs
    tox -e flake8
 
 `Tox <https://tox.readthedocs.io/en/latest/>`_ makes a virtualenv, installs Klein's dependencies into the virtualenv, and then runs a set of commands based on the ``-e`` (environment) argument.
 This strategy allows one to make and test changes to Klein without needing to change system-level Python packages.
 
 
@@ -30,39 +30,39 @@
 ==========
 
 Here are some suggestions to make the contributing process easier for everyone:
 
 Code
 ----
 
-- Use `Twisted's coding standards <http://twistedmatrix.com/documents/current/core/development/policy/coding-standard.html>`_ as a guideline for code changes you make.
+- Use `Twisted's coding standards <https://twistedmatrix.com/documents/current/core/development/policy/coding-standard.html>`_ as a guideline for code changes you make.
   Some parts of Klein (eg. ``klein.resource.ensure_utf8_bytes``) do not adhere to the Twisted style guide, but changing that would break public APIs, which is worse than breaking the style guidelines.
   Similarly, if you change existing code, following the Twisted style guide is good, but is less important than not breaking public APIs.
 - Compatibility across versions is important: here are `Twisted's compatibility guidelines <https://twistedmatrix.com/trac/wiki/CompatibilityPolicy>`_, which Klein shares.
 - If you're adding a new feature, please add a file with an example and some explanation to the `examples directory <https://github.com/twisted/klein/tree/master/docs/examples>`_, then add your example to ``/docs/index.rst``.
 - Please run ``tox -e flake8`` to check for style issues in changed code.
   Flake8 and similar tools expose many small-but-common errors early enough that it's easy to remedy the problem.
 - Code changes should have tests: untested code is buggy code.
-  Klein uses `Twisted Trial <http://twistedmatrix.com/documents/current/api/twisted.trial.html>`_ and `tox <https://tox.readthedocs.io/en/latest/>`_ for its tests.
+  Klein uses `Twisted Trial <https://twistedmatrix.com/documents/current/api/twisted.trial.html>`_ and `tox <https://tox.readthedocs.io/en/latest/>`_ for its tests.
   The command to run the full test suite is ``tox`` with no arguments.
   This will run tests against several versions of Python and Twisted, which can be time-consuming.
-  To run tests against only one or a few versions, pass a ``-e`` argument with an environment from the envlist in ``tox.ini``: for example, ``tox -e py35-twcurrent`` will run tests with Python 3.5 and the current released version of Twisted.
+  To run tests against only one or a few versions, pass a ``-e`` argument with an environment from the envlist in ``tox.ini``: for example, ``tox -e py38-twcurrent`` will run tests with Python 3.8 and the current released version of Twisted.
   To run only one or a few specific tests in the suite, add a filename or fully-qualified Python path to the end of the test invocation: for example, ``tox klein.test.test_app.KleinTestCase.test_foo`` will run only the ``test_foo()`` method of the ``KleinTestCase`` class in ``klein/test/test_app.py``.
   These two test shortcuts can be combined to give you a quick feedback cycle, but make sure to check on the full test suite from time to time to make sure changes haven't had unexpected side effects.
 - Show us your code changes through pull requests sent to `Klein's GitHub repo <https://github.com/twisted/klein>`_.
   This is the best way to make your code visible to others and to get feedback about it.
 - If your pull request is a work in progress, please put ``[WIP]`` in its title.
 - Add yourself to ``AUTHORS``.
   **Your contribution matters.**
 
 
 Documentation
 -------------
 
-Klein uses `Epydoc <http://epydoc.sourceforge.net/manual-epytext.html>`_ for docstrings in code and uses `Sphinx <https://sphinx.readthedocs.io/>`_ for standalone documentation.
+Klein uses `Epydoc <http://epydoc.sourceforge.net/manual-epytext.html>`_ for docstrings in code and uses `Sphinx <https://www.sphinx-doc.org/en/master/>`_ for standalone documentation.
 
 - In documents with headers, use this format and order for headers::
 
     ========
     Header 1
     ========
 
@@ -81,8 +81,8 @@
 
 Reviewing
 ---------
 
 All code changes added to Klein must be reviewed by at least one other person who is not an author of the code being added.
 This helps prevent bugs from slipping through the net, gives another source for improvements, and makes sure that the code productively follows guidelines.
 
-Reviewers should read `Glyph's mailing list post <http://twistedmatrix.com/pipermail/twisted-python/2014-January/027894.html>`_ on reviewing -- code and docs don't have to be *perfect*, only *better*.
+Reviewers should read `Glyph's mailing list post <https://twistedmatrix.com/pipermail/twisted-python/2014-January/027894.html>`_ on reviewing -- code and docs don't have to be *perfect*, only *better*.
```

### Comparing `klein-20.6.0/LICENSE` & `klein-21.8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 This is the MIT license.
 
-Copyright (c) 2011-2019, Klein Contributors (see AUTHORS)
+Copyright (c) 2011-2021, Klein Contributors (see AUTHORS)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `klein-20.6.0/NEWS.rst` & `klein-21.8.0/NEWS.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 NEWS
 ====
 
+NEXT
+-------------------
+ * Python 2 is no longer supported by Klein.
+ * Python 3.5 is no longer supported by Klein.
+ * Python 3.9 is now supported by Klein. [`#412 <https://github.com/twisted/klein/pull/412>`_]
+ * Fixed a compatibility issue with Twisted versions greater than 20.3.0 in Klein's test suite. [`#383 <https://github.com/twisted/klein/pull/383>`]
+ * Fixed a compatibility issue with Werkzeug versions greater than 2.0 in Klein's test suite. [`#499 <https://github.com/twisted/klein/pull/499>`]
+ * Klein has incomplete, but growing type hints, but ``py.typed`` is not installed, as they might not work well for most clients yet.
+ * ``Plating`` now sets the ``Content-Type`` header to ``application/json`` instead of ``text/json; charset=utf8``.
+
 20.6.0 - 2020-06-07
 -------------------
  * This is the last release of Klein expected to support Python 2.
  * This is the last release of Klein expected to support Python 3.5.
  * Python 3.4 is no longer supported by Klein. [`#284 <https://github.com/twisted/klein/pull/284>`_]
  * Python 3.8 is now supported by Klein. [`#303 <https://github.com/twisted/klein/pull/303>`_]
  * ``klein.app.subroute`` is now also available as ``klein.subroute``. [`#293 <https://github.com/twisted/klein/pull/293>`_]
```

### Comparing `klein-20.6.0/PKG-INFO` & `klein-21.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,85 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: klein
-Version: 20.6.0
+Version: 21.8.0
 Summary: werkzeug + twisted.web
 Home-page: https://github.com/twisted/klein
-Maintainer: Amber Brown (HawkOwl)
-Maintainer-email: hawkowl@twistedmatrix.com
+Maintainer: Twisted Matrix Laboratories
+Maintainer-email: twisted-python@twistedmatrix.com
 License: MIT
-Description: ============================
-        Klein, a Web Micro-Framework
-        ============================
-        
-        .. image:: https://travis-ci.org/twisted/klein.svg?branch=master
-            :target: http://travis-ci.org/twisted/klein
-            :alt: Build Status
-        .. image:: https://codecov.io/github/twisted/klein/coverage.svg?branch=master
-            :target: https://codecov.io/github/twisted/klein?branch=master
-            :alt: Code Coverage
-        .. image:: https://requires.io/github/twisted/klein/requirements.svg?branch=master
-            :target: https://requires.io/github/twisted/klein/requirements/?branch=master
-            :alt: Requirements Status
-        .. image:: https://img.shields.io/pypi/pyversions/klein.svg
-            :target: https://pypi.python.org/pypi/klein
-            :alt: Python Version Compatibility
-        
-        Klein is a micro-framework for developing production-ready web services with Python.
-        It is 'micro' in that it has an incredibly small API similar to `Bottle <http://bottlepy.org/docs/dev/index.html>`_ and `Flask <http://flask.pocoo.org/>`_.
-        It is not 'micro' in that it depends on things outside the standard library.
-        This is primarily because it is built on widely used and well tested components like `Werkzeug <http://werkzeug.pocoo.org/>`_ and `Twisted <http://twistedmatrix.com>`_.
-        
-        A `Klein bottle <https://en.wikipedia.org/wiki/Klein_bottle>`_ is an example of a non-orientable surface, and a glass Klein bottle looks like a twisted bottle or twisted flask.
-        This, of course, made it too good of a pun to pass up.
-        
-        Klein's documentation can be found at `Read The Docs <http://klein.readthedocs.org>`_.
-        
-        
-        Example
-        =======
-        
-        This is a sample Klein application that returns 'Hello, world!', running on port ``8080``.
-        
-        .. code-block:: python
-        
-            from klein import run, route
-        
-            @route('/')
-            def home(request):
-                return 'Hello, world!'
-        
-            run("localhost", 8080)
-        
-        
-        Contribute
-        ==========
-        
-        ``klein`` is hosted on `GitHub <http://github.com/twisted/klein>`_ and is an open source project that welcomes contributions of all kinds from the community, including:
-        
-        - code patches,
-        - `documentation <http://klein.readthedocs.org/>`_ improvements,
-        - `bug reports <https://github.com/twisted/klein/issues>`_,
-        - reviews for `contributed patches <https://github.com/twisted/klein/pulls>`_.
-        
-        For more information about contributing, see `the contributor guidelines <https://github.com/twisted/klein/tree/master/CONTRIBUTING.rst>`_.
-        
 Keywords: twisted flask werkzeug web
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
+============================
+Klein, a Web Micro-Framework
+============================
+
+.. image:: https://github.com/twisted/klein/workflows/CI%2fCD/badge.svg
+    :target: https://github.com/twisted/klein/actions
+    :alt: Build Status
+.. image:: https://codecov.io/github/twisted/klein/coverage.svg?branch=master
+    :target: https://codecov.io/github/twisted/klein?branch=master
+    :alt: Code Coverage
+.. image:: https://requires.io/github/twisted/klein/requirements.svg?branch=master
+    :target: https://requires.io/github/twisted/klein/requirements/?branch=master
+    :alt: Requirements Status
+.. image:: https://img.shields.io/pypi/pyversions/klein.svg
+    :target: https://pypi.org/project/klein
+    :alt: Python Version Compatibility
+
+Klein is a micro-framework for developing production-ready web services with Python.
+It is 'micro' in that it has an incredibly small API similar to `Bottle <https://bottlepy.org/docs/dev/index.html>`_ and `Flask <https://flask.palletsprojects.com/>`_.
+It is not 'micro' in that it depends on things outside the standard library.
+This is primarily because it is built on widely used and well tested components like `Werkzeug <https://werkzeug.palletsprojects.com/>`_ and `Twisted <https://twistedmatrix.com>`_.
+
+A `Klein bottle <https://en.wikipedia.org/wiki/Klein_bottle>`_ is an example of a non-orientable surface, and a glass Klein bottle looks like a twisted bottle or twisted flask.
+This, of course, made it too good of a pun to pass up.
+
+Klein's documentation can be found at `Read The Docs <https://klein.readthedocs.org>`_.
+
+
+Example
+========
+
+This is a sample Klein application that returns 'Hello, world!', running on port ``8080``.
+
+.. code-block:: python
+
+    from klein import run, route
+
+    @route('/')
+    def home(request):
+        return 'Hello, world!'
+
+    run("localhost", 8080)
+
+
+Contribute
+==========
+
+``klein`` is hosted on `GitHub <https://github.com/twisted/klein>`_ and is an open source project that welcomes contributions of all kinds from the community, including:
+
+- code patches,
+- `documentation <https://klein.readthedocs.org/>`_ improvements,
+- `bug reports <https://github.com/twisted/klein/issues>`_,
+- reviews for `contributed patches <https://github.com/twisted/klein/pulls>`_.
+
+For more information about contributing, see `the contributor guidelines <https://github.com/twisted/klein/tree/master/CONTRIBUTING.rst>`_.
+
+
```

### Comparing `klein-20.6.0/README.rst` & `klein-21.8.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 ============================
 Klein, a Web Micro-Framework
 ============================
 
-.. image:: https://travis-ci.org/twisted/klein.svg?branch=master
-    :target: http://travis-ci.org/twisted/klein
+.. image:: https://github.com/twisted/klein/workflows/CI%2fCD/badge.svg
+    :target: https://github.com/twisted/klein/actions
     :alt: Build Status
 .. image:: https://codecov.io/github/twisted/klein/coverage.svg?branch=master
     :target: https://codecov.io/github/twisted/klein?branch=master
     :alt: Code Coverage
 .. image:: https://requires.io/github/twisted/klein/requirements.svg?branch=master
     :target: https://requires.io/github/twisted/klein/requirements/?branch=master
     :alt: Requirements Status
 .. image:: https://img.shields.io/pypi/pyversions/klein.svg
-    :target: https://pypi.python.org/pypi/klein
+    :target: https://pypi.org/project/klein
     :alt: Python Version Compatibility
 
 Klein is a micro-framework for developing production-ready web services with Python.
-It is 'micro' in that it has an incredibly small API similar to `Bottle <http://bottlepy.org/docs/dev/index.html>`_ and `Flask <http://flask.pocoo.org/>`_.
+It is 'micro' in that it has an incredibly small API similar to `Bottle <https://bottlepy.org/docs/dev/index.html>`_ and `Flask <https://flask.palletsprojects.com/>`_.
 It is not 'micro' in that it depends on things outside the standard library.
-This is primarily because it is built on widely used and well tested components like `Werkzeug <http://werkzeug.pocoo.org/>`_ and `Twisted <http://twistedmatrix.com>`_.
+This is primarily because it is built on widely used and well tested components like `Werkzeug <https://werkzeug.palletsprojects.com/>`_ and `Twisted <https://twistedmatrix.com>`_.
 
 A `Klein bottle <https://en.wikipedia.org/wiki/Klein_bottle>`_ is an example of a non-orientable surface, and a glass Klein bottle looks like a twisted bottle or twisted flask.
 This, of course, made it too good of a pun to pass up.
 
-Klein's documentation can be found at `Read The Docs <http://klein.readthedocs.org>`_.
+Klein's documentation can be found at `Read The Docs <https://klein.readthedocs.org>`_.
 
 
 Example
-=======
+========
 
 This is a sample Klein application that returns 'Hello, world!', running on port ``8080``.
 
 .. code-block:: python
 
     from klein import run, route
 
@@ -41,15 +41,15 @@
 
     run("localhost", 8080)
 
 
 Contribute
 ==========
 
-``klein`` is hosted on `GitHub <http://github.com/twisted/klein>`_ and is an open source project that welcomes contributions of all kinds from the community, including:
+``klein`` is hosted on `GitHub <https://github.com/twisted/klein>`_ and is an open source project that welcomes contributions of all kinds from the community, including:
 
 - code patches,
-- `documentation <http://klein.readthedocs.org/>`_ improvements,
+- `documentation <https://klein.readthedocs.org/>`_ improvements,
 - `bug reports <https://github.com/twisted/klein/issues>`_,
 - reviews for `contributed patches <https://github.com/twisted/klein/pulls>`_.
 
 For more information about contributing, see `the contributor guidelines <https://github.com/twisted/klein/tree/master/CONTRIBUTING.rst>`_.
```

### Comparing `klein-20.6.0/docs/Makefile` & `klein-21.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/_extensions/apilinks.py` & `klein-21.8.0/docs/_extensions/apilinks.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,45 +6,59 @@
 
 for example::
 
     :api:`twisted.internet.defer.Deferred <Deferred>`
 
 """
 
+from types import MappingProxyType
 
 
-def make_api_link(name, rawtext, text, lineno, inliner,
-                  options={}, content=[]):
+emptyMapping = MappingProxyType({})
 
+
+def make_api_link(
+    name,
+    rawtext,
+    text,
+    lineno,
+    inliner,
+    options=emptyMapping,
+    content=(),
+):
     from docutils import nodes, utils
 
     # quick, dirty, and ugly...
-    if '<' in text and '>' in text:
-        full_name, label = text.split('<')
+    if "<" in text and ">" in text:
+        full_name, label = text.split("<")
         full_name = full_name.strip()
-        label = label.strip('>').strip()
+        label = label.strip(">").strip()
     else:
         full_name = text
 
-    #get the base url for api links from the config file
+    # get the base url for api links from the config file
     env = inliner.document.settings.env
-    base_url =  env.config.apilinks_base_url
+    base_url = env.config.apilinks_base_url
 
     # not really sufficient, but just testing...
     # ...hmmm, maybe this is good enough after all
-    ref = ''.join((base_url, full_name, '.html'))
+    ref = "".join((base_url, full_name, ".html"))
 
-    node = nodes.reference(rawtext, utils.unescape(label), refuri=ref,
-                           **options)
+    node = nodes.reference(
+        rawtext, utils.unescape(label), refuri=ref, **options
+    )
 
     nodes = [node]
     sys_msgs = []
     return nodes, sys_msgs
 
 
 # setup function to register the extension
 
+
 def setup(app):
-    app.add_config_value('apilinks_base_url',
-                         'http://twistedmatrix.com/documents/current/api/',
-                         'env')
-    app.add_role('api', make_api_link)
+    app.add_config_value(
+        "apilinks_base_url",
+        "http://twistedmatrix.com/documents/current/api/",
+        "env",
+    )
+    app.add_role("api", make_api_link)
```

### Comparing `klein-20.6.0/docs/examples/alternativerunning.rst` & `klein-21.8.0/docs/examples/alternativerunning.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/examples/await.rst` & `klein-21.8.0/docs/examples/await.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/examples/deferreds.rst` & `klein-21.8.0/docs/examples/deferreds.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/examples/disablingtracebacks.rst` & `klein-21.8.0/docs/examples/disablingtracebacks.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/examples/handlingerrors.rst` & `klein-21.8.0/docs/examples/handlingerrors.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 We can do this with ``Klein.handle_errors``.
 
 Below we have created a class that will translate ``NotFound`` exceptions into a custom 404 response.
 
 .. code-block:: python
 
     from klein import Klein
-    
+
     class NotFound(Exception):
         pass
 
 
-    class ItemStore(object):
+    class ItemStore:
         app = Klein()
 
         @app.handle_errors(NotFound)
         def notfound(self, request, failure):
             request.setResponseCode(404)
             return 'Not found, I say'
 
@@ -58,15 +58,15 @@
 
 A simple way to create a catch-all function, which serves every URL that doesn't match a route, is to use a ``path`` variable in the route.
 
 .. code-block:: python
 
     from klein import Klein
 
-    class OnlyOneRoute(object):
+    class OnlyOneRoute:
         app = Klein()
 
         @app.route('/api/<path:catchall>')
         def catchAll(self, request, catchall):
             request.redirect('/api')
 
         @app.route('/api')
@@ -92,8 +92,7 @@
    Version 1 - Home
 
    curl -L localhost:8080/api/another
    API Home
 
 
 This method can also be used on the root route, in which case it will catch every request which doesn't match a route.
-
```

### Comparing `klein-20.6.0/docs/examples/handlingpost.rst` & `klein-21.8.0/docs/examples/handlingpost.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,51 +14,51 @@
 So the ``POST`` handler must be defined before the handler with no ``methods``.
 
 .. code-block:: python
 
     from twisted.internet.defer import succeed
     from klein import run, route
 
-    name='world'
+    name = b"world"
 
-    @route('/', methods=['POST'])
+    @route("/", methods=["POST"])
     def setname(request):
         global name
-        name = request.args.get('name', ['world'])[0]
+        name = request.args.get(b'name', [b'world'])[0]
         request.redirect('/')
         return succeed(None)
 
     @route('/')
     def hello(request):
-        return "Hello, {0}!".format(name)
+        return b"Hello, %s!" % (name,)
 
     run("localhost", 8080)
 
 
 The following curl command can be used to test this behaviour::
 
     curl -v -L -d name='bob' http://localhost:8080/
 
 
 Accessing the request content
 =============================
 
 To read the content of the request use the ``read`` method of
-:api:`twisted.web.iweb.IRequest.content <IRequest.content>`
+:api:`twisted.web.iweb.IRequest <IRequest.content>`
 
 .. code-block:: python
 
     from klein import run, route
     import json
-    
+
     @route('/', methods=['POST'])
     def do_post(request):
         content = json.loads(request.content.read())
         response = json.dumps(dict(the_data=content), indent=4)
         return response
-    
+
     run("localhost", 8080)
- 
- 
+
+
 The following curl command can be used to test this behaviour::
- 
-	 curl -XPOST -v -H 'Content-Type: appliction/json' -d '{"name":"bob"}'  http://localhost:8080/
+
+     curl -XPOST -v -H 'Content-Type: appliction/json' -d '{"name":"bob"}'  http://localhost:8080/
```

### Comparing `klein-20.6.0/docs/examples/nonglobalstate.rst` & `klein-21.8.0/docs/examples/nonglobalstate.rst`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 .. code-block:: python
 
     import json
 
     from klein import Klein
 
 
-    class ItemStore(object):
+    class ItemStore:
         app = Klein()
 
         def __init__(self):
             self._items = {}
 
         @app.route('/')
         def items(self, request):
```

### Comparing `klein-20.6.0/docs/examples/staticfiles.rst` & `klein-21.8.0/docs/examples/staticfiles.rst`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,33 @@
     def static(request):
         return File("./static")
 
     @route('/')
     def home(request):
         return '<img src="/static/img.gif">'
 
-    run("localhost", 8080)
+    run("localhost", 8080)
+
+In production environments, you might want to disable directory listings so
+that you do not accidentally expose more information than you intend. To
+disable directory listings, override the ``directoryListing`` method for the
+:api:`twisted.web.static.File <t.w.static.File>` class.
+
+.. code-block:: python
+
+    from twisted.web.static import File
+    from klein import run, route
+    from werkzeug.exceptions import NotFound
+
+    @route('/static/', branch=True)
+    def static(request):
+        return FileNoDir("./static")
+
+    @route('/')
+    def home(request):
+        return '<img src="/static/img.gif">'
+
+    class FileNoDir(File):
+        def directoryListing(self):
+            raise NotFound()
+
+    run("localhost", 8080)
```

### Comparing `klein-20.6.0/docs/examples/subroutes.rst` & `klein-21.8.0/docs/examples/subroutes.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/examples/templates.rst` & `klein-21.8.0/docs/examples/templates.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/examples/twistd.rst` & `klein-21.8.0/docs/examples/twistd.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/index.rst` & `klein-21.8.0/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 ============================
 Klein, a Web Micro-Framework
 ============================
 
-.. image:: https://travis-ci.org/twisted/klein.png?branch=master
-
 Klein is a micro-framework for developing production-ready web services with Python.
 It's built on widely used and well tested components like Werkzeug and Twisted, and has near-complete test coverage.
 
 Klein is developed by a team of contributors `on GitHub <https://github.com/twisted/klein>`_.
-We're also commonly in ``#twisted.web`` on `Freenode <http://freenode.net>`_.
+We're also commonly in ``#twisted.web`` on `Freenode <https://freenode.net>`_.
 
 
 Introduction to Klein
 =====================
 
 This is an introduction to Klein, going through from creating a simple web site to something supporting AJAX and more.
```

### Comparing `klein-20.6.0/docs/introduction/1-gettingstarted.rst` & `klein-21.8.0/docs/introduction/1-gettingstarted.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 
 .. literalinclude:: codeexamples/moreRoutes.py
 
 
 Variable Routes
 ===============
 
-You can also make `variable routes`.
+You can also make variable routes.
 This gives your functions extra arguments which match up with the parts of the routes that you have specified.
-By using this, you can implement pages that change depending on this -- for example, by displaying users on a site, or documents in a repository. 
+By using this, you can implement pages that change depending on this -- for example, by displaying users on a site, or documents in a repository.
 
 .. literalinclude:: codeexamples/variableRoutes.py
 
 If you start the server and then visit ``http://localhost:8080/user/bob``, you should get ``Hi bob!`` in return.
 
 You can also define what types it should match.
 The three available types are ``string`` (default), ``int`` and ``float``.
@@ -127,15 +127,15 @@
 First, we'll create a top-level Plating for the site.  This takes a
 ``twisted.web.template`` template, defined with the objects from
 ``twisted.web.template.tags``, with one special slot, named
 ``Plating.CONTENT``, in the spot where you want the content of each page to
 appear.  That'll look something like this:
 
 .. literalinclude:: codeexamples/template.py
-    :lines: 13-24
+    :lines: 15-26
 
 Notice that we have defined a ``"pageTitle"`` slot in the template - individual
 pages must each provide a value for the title themselves in order to use the
 ``myStyle`` frame.  Nothing's special about ``"pageTitle"``, by the way; you
 may define whatever slots you want in your page template.
 
 You can also specify a dictionary of default values to fill slots with.
@@ -147,38 +147,38 @@
 must then return a dictionary of the values to populate the slots in the
 template with.
 
 Let's start with a really simple page that just has a static template to fill
 the content slot.
 
 .. literalinclude:: codeexamples/template.py
-    :lines: 26-37
+    :lines: 29-49
 
 This page generates some links to various sub-pages which we'll get to in a
 moment.  But first, if you load ``http://localhost:8080/``, you'll see that the
 template specified for ``root`` is inserted at the point in the template for
 ``myStyle`` specified the content should go.
 
 Next, we should actually try injecting some data.
 
 .. literalinclude:: codeexamples/template.py
-    :lines: 39-50
+    :lines: 52-67
 
 Here you can see the ``/foods/...`` route for showing information about a food.
 In the content template, we've got slots for ``"name"``, ``"rating"``, and
 ``"carbohydrates"``, the three primary properties which define a food.  The
 decorated function then returns a dictionary that returns values for each of
 those slots, as well as a value for ``"pageTitle"``.
 
 Each of these slots is only filled with a single item, though.  What if you
 need to put multiple items into the template?  The route for ``/places/...``
 can show us:
 
 .. literalinclude:: codeexamples/template.py
-    :lines: 52-68
+    :lines: 70-103
 
 Here you can see the special ``<slotname>:list`` renderer in use.  By
 specifying the ``render=`` attribute of a tag (in this case, a ``li`` tag) to
 be ``foods:list``, we invoke a ``twisted.web.template`` renderer that repeats
 the tag it is the renderer for, inserting each element of that list into the
 special ``"item"`` slot.
 
@@ -223,11 +223,11 @@
 
 Klein tries to do the right thing with what you return.
 You can return a result (which can be regular text, a :api:`twisted.web.resource.IResource <Resource>`, or a :api:`twisted.web.iweb.IRenderable <Renderable>`) synchronously (via ``return``) or asynchronously (via ``Deferred``).
 Just remember not to give Klein any ``unicode``, you have to encode it into ``bytes`` first.
 
 
 Onwards
-=======
+========
 
 That covers most of the general Klein concepts.
 The next chapter is about deploying your Klein application using Twisted's ``tap`` functionality.
```

#### html2text {}

```diff
@@ -20,16 +20,16 @@
 instance, then calling the ``run`` and ``route`` methods on it, you are able to
 make your routing not global. .. literalinclude:: codeexamples/
 helloWorldClass.py By not using the global Klein instance, you can have
 different Klein routers, each having different routes, if your application
 requires that in the future. Adding Routes ============= Add more decorated
 functions to add more routes to your Klein applications. .. literalinclude::
 codeexamples/moreRoutes.py Variable Routes =============== You can also make
-`variable routes`. This gives your functions extra arguments which match up
-with the parts of the routes that you have specified. By using this, you can
+variable routes. This gives your functions extra arguments which match up with
+the parts of the routes that you have specified. By using this, you can
 implement pages that change depending on this -- for example, by displaying
 users on a site, or documents in a repository. .. literalinclude::
 codeexamples/variableRoutes.py If you start the server and then visit ``http://
 localhost:8080/user/bob``, you should get ``Hi bob!`` in return. You can also
 define what types it should match. The three available types are ``string``
 (default), ``int`` and ``float``. .. literalinclude:: codeexamples/
 variableRoutesTypes.py If you run this example and visit ``http://localhost:
@@ -63,40 +63,40 @@
 fake (random) information about places you can go and foods you can get there.
 You can download the full example :download:`here
 emplate.py>` in order to run it. First, we'll create a top-level Plating for
 the site. This takes a ``twisted.web.template`` template, defined with the
 objects from ``twisted.web.template.tags``, with one special slot, named
 ``Plating.CONTENT``, in the spot where you want the content of each page to
 appear. That'll look something like this: .. literalinclude:: codeexamples/
-template.py :lines: 13-24 Notice that we have defined a ``"pageTitle"`` slot in
+template.py :lines: 15-26 Notice that we have defined a ``"pageTitle"`` slot in
 the template - individual pages must each provide a value for the title
 themselves in order to use the ``myStyle`` frame. Nothing's special about
 ``"pageTitle"``, by the way; you may define whatever slots you want in your
 page template. You can also specify a dictionary of default values to fill
 slots with. Next, you want to create a route that is plated with that
 ``Plating``, by using the ``Plating.routed`` decorator. ``@myStyle.routed``
 takes a route from the Klein instance, in this case ``app``, and then a
 template for the content portion (the ``Plating.CONTENT`` slot) of the page.
 The decorated function must then return a dictionary of the values to populate
 the slots in the template with. Let's start with a really simple page that just
 has a static template to fill the content slot. .. literalinclude::
-codeexamples/template.py :lines: 26-37 This page generates some links to
+codeexamples/template.py :lines: 29-49 This page generates some links to
 various sub-pages which we'll get to in a moment. But first, if you load
 ``http://localhost:8080/``, you'll see that the template specified for ``root``
 is inserted at the point in the template for ``myStyle`` specified the content
 should go. Next, we should actually try injecting some data. ..
-literalinclude:: codeexamples/template.py :lines: 39-50 Here you can see the
+literalinclude:: codeexamples/template.py :lines: 52-67 Here you can see the
 ``/foods/...`` route for showing information about a food. In the content
 template, we've got slots for ``"name"``, ``"rating"``, and
 ``"carbohydrates"``, the three primary properties which define a food. The
 decorated function then returns a dictionary that returns values for each of
 those slots, as well as a value for ``"pageTitle"``. Each of these slots is
 only filled with a single item, though. What if you need to put multiple items
 into the template? The route for ``/places/...`` can show us: ..
-literalinclude:: codeexamples/template.py :lines: 52-68 Here you can see the
+literalinclude:: codeexamples/template.py :lines: 70-103 Here you can see the
 special ``:list`` renderer in use. By specifying the ``render=`` attribute of a
 tag (in this case, a ``li`` tag) to be ``foods:list``, we invoke a
 ``twisted.web.template`` renderer that repeats the tag it is the renderer for,
 inserting each element of that list into the special ``"item"`` slot. You can
 view each of these pages in a web browser now, and you can see their contents;
 we've built a little website that generates random values for these types of
 data. But we've *also* built a JSON API. If you access, for example, ``http://
@@ -113,10 +113,10 @@
 literalinclude:: codeexamples/googleProxy.py This example here uses `treq
 github.com/dreid/treq>`_ (think Requests, but using Twisted) to implement a
 Google proxy. Return Anything =============== Klein tries to do the right thing
 with what you return. You can return a result (which can be regular text, a :
 api:`twisted.web.resource.IResource `, or a :api:`twisted.web.iweb.IRenderable
 `) synchronously (via ``return``) or asynchronously (via ``Deferred``). Just
 remember not to give Klein any ``unicode``, you have to encode it into
-``bytes`` first. Onwards ======= That covers most of the general Klein
+``bytes`` first. Onwards ======== That covers most of the general Klein
 concepts. The next chapter is about deploying your Klein application using
 Twisted's ``tap`` functionality.
```

### Comparing `klein-20.6.0/docs/introduction/2-twistdtap.rst` & `klein-21.8.0/docs/introduction/2-twistdtap.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/introduction/codeexamples/forms.py` & `klein-21.8.0/docs/introduction/codeexamples/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-from twisted.web.template import tags, slot
-from klein import Klein, Plating, Form, Field, Requirer, SessionProcurer
+from twisted.web.template import slot, tags
+
+from klein import Field, Form, Klein, Plating, Requirer, SessionProcurer
 from klein.interfaces import ISession
 from klein.storage.memory import MemorySessionStore
 
+
 app = Klein()
 
 sessions = MemorySessionStore()
 
 requirer = Requirer()
 
+
 @requirer.prerequisite([ISession])
 def procurer(request):
     return SessionProcurer(sessions).procureSession(request)
 
 
-style = Plating(tags=tags.html(
-    tags.head(tags.title("yay")),
-    tags.body(tags.div(slot(Plating.CONTENT))))
+style = Plating(
+    tags=tags.html(
+        tags.head(tags.title("yay")), tags.body(tags.div(slot(Plating.CONTENT)))
+    )
 )
 
+
 @requirer.require(
     style.routed(
         app.route("/", methods=["POST"]),
-        tags.h1('u did it: ', slot("an-form-arg"))
+        tags.h1("u did it: ", slot("an-form-arg")),
     ),
-    foo=Field.number(minimum=3, maximum=10), bar=Field.text(),
+    foo=Field.number(minimum=3, maximum=10),
+    bar=Field.text(),
 )
 def postHandler(foo, bar):
     return {"an-form-arg": foo}
 
+
 @requirer.require(
-    style.routed(
-        app.route("/", methods=["GET"]),
-        tags.div(slot("anForm"))
-    ),
-    theForm=Form.rendererFor(postHandler, action=u"/?post=yes")
+    style.routed(app.route("/", methods=["GET"]), tags.div(slot("anForm"))),
+    theForm=Form.rendererFor(postHandler, action="/?post=yes"),
 )
 def formRenderer(theForm):
     return {"anForm": theForm}
 
+
 @requirer.require(
-    style.routed(Form.onValidationFailureFor(postHandler),
-                 [tags.h1('invalid form'),
-                  tags.div(slot('the-invalid-form'))]),
-    renderer=Form.rendererFor(postHandler, action=u"/?post=yes"),
+    style.routed(
+        Form.onValidationFailureFor(postHandler),
+        [tags.h1("invalid form"), tags.div(slot("the-invalid-form"))],
+    ),
+    renderer=Form.rendererFor(postHandler, action="/?post=yes"),
 )
 def validationFailed(values, renderer):
     renderer.prevalidationValues = values.prevalidationValues
     renderer.validationErrors = values.validationErrors
-    return {'the-invalid-form': renderer}
+    return {"the-invalid-form": renderer}
 
 
 app.run("localhost", 8080)
```

### Comparing `klein-20.6.0/docs/introduction/twistdwebman.txt` & `klein-21.8.0/docs/introduction/twistdwebman.txt`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/docs/release.rst` & `klein-21.8.0/docs/release.rst`

 * *Files identical despite different names*

### Comparing `klein-20.6.0/src/klein/__init__.py` & `klein-21.8.0/src/klein/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,42 @@
-from __future__ import absolute_import, division
-
 from typing import TYPE_CHECKING
 
-from ._app import Klein, handle_errors, route, run, subroute, urlFor, url_for
+from ._app import (
+    Klein,
+    KleinErrorHandler,
+    KleinRenderable,
+    KleinRouteHandler,
+    handle_errors,
+    route,
+    run,
+    subroute,
+    url_for,
+    urlFor,
+)
 from ._dihttp import RequestComponent, RequestURL, Response
 from ._form import Field, FieldValues, Form, RenderableForm
 from ._plating import Plating
 from ._requirer import Requirer
 from ._session import Authorization, SessionProcurer
 from ._version import __version__ as _incremental_version
 
+
 if TYPE_CHECKING:
     # Inform mypy of import shenanigans.
     from .resource import _SpecialModuleObject
 
-    resource = _SpecialModuleObject()
+    resource = _SpecialModuleObject(None)
 else:
     from . import resource
 
 __all__ = (
     "Klein",
+    "KleinErrorHandler",
+    "KleinRenderable",
+    "KleinRouteHandler",
     "Plating",
     "Field",
     "FieldValues",
     "Form",
     "RequestComponent",
     "RequestURL",
     "Response",
@@ -46,8 +59,8 @@
 
 
 # Make it a str, for backwards compatibility
 __version__ = _incremental_version.base()
 
 __author__ = "The Klein contributors (see AUTHORS)"
 __license__ = "MIT"
-__copyright__ = "Copyright 2011-2019 {0}".format(__author__)
+__copyright__ = f"Copyright 2011-2021 {__author__}"
```

### Comparing `klein-20.6.0/src/klein/_app.py` & `klein-21.8.0/src/klein/_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,115 @@
 # -*- test-case-name: klein.test.test_app -*-
 """
 Applications are great.  Lets have more of them.
 """
 
-from __future__ import absolute_import, division
 
 import sys
-from collections import namedtuple
 from contextlib import contextmanager
+from inspect import iscoroutine
+from typing import (
+    IO,
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    cast,
+    overload,
+)
+from weakref import ref
+
 
 try:
-    from inspect import iscoroutine
+    from typing import Protocol
 except ImportError:
+    from typing_extensions import Protocol  # type: ignore[misc]
 
-    def iscoroutine(*args, **kwargs):  # type: ignore
-        return False
-
-
-from weakref import ref
+from werkzeug.routing import Map, MapAdapter, Rule, Submount
+from zope.interface import implementer
 
-from twisted.internet import endpoints, reactor
+from twisted.internet import reactor
+from twisted.internet.defer import ensureDeferred
+from twisted.internet.endpoints import serverFromString
 from twisted.python import log
 from twisted.python.components import registerAdapter
+from twisted.python.failure import Failure
+from twisted.web.iweb import IRenderable, IRequest
+from twisted.web.resource import IResource
 from twisted.web.server import Request, Site
 
-try:
-    from twisted.internet.defer import ensureDeferred
-except ImportError:
+from ._decorators import modified, named
+from ._interfaces import IKleinRequest, KleinQueryValue
+from ._resource import KleinResource
 
-    def ensureDeferred(*args, **kwagrs):
-        raise NotImplementedError("Coroutines support requires Twisted>=16.6")
 
+KleinSynchronousRenderable = Union[str, bytes, IResource, IRenderable]
+KleinRenderable = Union[
+    KleinSynchronousRenderable, Awaitable[KleinSynchronousRenderable]
+]
 
-from werkzeug.routing import Map, Rule, Submount
 
-from zope.interface import implementer
+class KleinRouteFunction(Protocol):
+    def __call__(_self, request: IRequest) -> KleinRenderable:
+        """
+        Function that, when decorated by L{Klein.route}, handles a Klein
+        request.
+        """
 
-from ._decorators import modified, named
-from ._interfaces import IKleinRequest
-from ._resource import KleinResource
+
+class KleinRouteMethod(Protocol):
+    def __call__(_self, self: Any, request: IRequest) -> KleinRenderable:
+        """
+        Method that, when decorated by L{Klein.route}, handles a Klein
+        request.
+        """
+
+
+class KleinErrorFunction(Protocol):
+    def __call__(
+        _self,
+        request: IRequest,
+        failure: Failure,
+    ) -> KleinRenderable:
+        """
+        Function that, when registered with L{Klein.handle_errors}, handles
+        errors raised during request routing.
+        """
 
 
-def _call(__klein_instance__, __klein_f__, *args, **kwargs):
+class KleinErrorMethod(Protocol):
+    def __call__(
+        _self,
+        self: Optional["Klein"],
+        request: IRequest,
+        failure: Failure,
+    ) -> KleinRenderable:
+        """
+        Method that, when registered with L{Klein.handle_errors}, handles
+        errors raised during request routing.
+        """
+
+
+KleinRouteHandler = Union[KleinRouteFunction, KleinRouteMethod]
+KleinErrorHandler = Union[KleinErrorFunction, KleinErrorMethod]
+
+
+def _call(
+    __klein_instance__: Optional["Klein"],
+    __klein_f__: Callable[..., KleinRenderable],
+    *args: Any,
+    **kwargs: Any,
+) -> KleinRenderable:
     """
     Call C{__klein_f__} with the given C{*args} and C{**kwargs}.
 
     Insert C{__klein_instance__} as the first positional argument to
     C{__klein_f__} if C{__klein_f__} is not decorated with
     L{klein._decorators.bindable}.
 
@@ -55,99 +119,143 @@
     """
     if __klein_instance__ is not None or getattr(
         __klein_f__, "__klein_bound__", False
     ):
         args = (__klein_instance__,) + args
     result = __klein_f__(*args, **kwargs)
     if iscoroutine(result):
-        result = ensureDeferred(result)
+        result = ensureDeferred(result)  # type: ignore[arg-type]
     return result
 
 
+def buildURL(
+    mapper: MapAdapter,
+    endpoint: str,
+    values: Optional[Mapping[str, KleinQueryValue]] = None,
+    method: Optional[str] = None,
+    force_external: bool = False,
+    append_unknown: bool = True,
+) -> str:
+    return mapper.build(
+        endpoint, values, method, force_external, append_unknown
+    )
+
+
 @implementer(IKleinRequest)
-class KleinRequest(object):
-    def __init__(self, request):
+class KleinRequest:
+    def __init__(self, request: Request) -> None:
         self.branch_segments = [""]
-        self.mapper = None
 
-    def url_for(self, *args, **kwargs):
-        return self.mapper.build(*args, **kwargs)
+        # Don't annotate as optional, since you should never set this to None
+        self.mapper: MapAdapter = None  # type: ignore[assignment]
+
+    def url_for(
+        self,
+        endpoint: str,
+        values: Optional[Mapping[str, KleinQueryValue]] = None,
+        method: Optional[str] = None,
+        force_external: bool = False,
+        append_unknown: bool = True,
+    ) -> str:
+        return buildURL(
+            self.mapper,
+            endpoint,
+            values,
+            method,
+            force_external,
+            append_unknown,
+        )
 
 
 registerAdapter(KleinRequest, Request, IKleinRequest)
 
 
-class Klein(object):
+ErrorHandlers = List[Tuple[List[Type[Exception]], KleinErrorHandler]]
+
+
+class Klein:
     """
     L{Klein} is an object which is responsible for maintaining the routing
     configuration of our application.
 
     @ivar _url_map: A C{werkzeug.routing.Map} object which will be used for
         routing resolution.
     @ivar _endpoints: A C{dict} mapping endpoint names to handler functions.
     """
 
     _subroute_segments = 0
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._url_map = Map()
-        self._endpoints = {}
-        self._error_handlers = []
-        self._instance = None
-        self._boundAs = None
+        self._endpoints: Dict[str, KleinRouteHandler] = {}
+        self._error_handlers: ErrorHandlers = []
+        self._instance: Optional[Klein] = None
+        self._boundAs: Optional[str] = None
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, Klein):
             return vars(self) == vars(other)
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         result = self.__eq__(other)
         if result is NotImplemented:
             return result
         return not result
 
     @property
-    def url_map(self):
+    def url_map(self) -> Map:
         """
         Read only property exposing L{Klein._url_map}.
         """
         return self._url_map
 
     @property
-    def endpoints(self):
+    def endpoints(self) -> Dict[str, KleinRouteHandler]:
         """
         Read only property exposing L{Klein._endpoints}.
         """
         return self._endpoints
 
-    def execute_endpoint(self, endpoint, *args, **kwargs):
+    def execute_endpoint(
+        self, endpoint: str, request: IRequest, *args: Any, **kwargs: Any
+    ) -> KleinRenderable:
         """
         Execute the named endpoint with all arguments and possibly a bound
         instance.
         """
         endpoint_f = self._endpoints[endpoint]
-        return endpoint_f(self._instance, *args, **kwargs)
+        # typing note: endpoint_f is a KleinRouteHandler, which is not defined
+        # as taking *args, **kwargs (because they aren't required), but we're
+        # going to pass them along here anyway.
+        return endpoint_f(
+            self._instance, request, *args, **kwargs  # type: ignore[arg-type]
+        )  # type: ignore[call-arg]
 
-    def execute_error_handler(self, handler, request, failure):
+    def execute_error_handler(
+        self,
+        handler: KleinErrorMethod,
+        request: IRequest,
+        failure: Failure,
+    ) -> KleinRenderable:
         """
         Execute the passed error handler, possibly with a bound instance.
         """
         return handler(self._instance, request, failure)
 
-    def resource(self):
+    def resource(self) -> KleinResource:
         """
         Return an L{IResource} which suitably wraps this app.
 
         @returns: An L{IResource}
         """
 
         return KleinResource(self)
 
-    def __get__(self, instance, owner):
+    def __get__(self, instance: Any, owner: object) -> "Klein":
         """
         Get an instance of L{Klein} bound to C{instance}.
         """
         if instance is None:
             return self
 
         if self._boundAs is None:
@@ -158,16 +266,18 @@
                 obj = getattr(owner, name, None)
                 if obj is self:
                     self._boundAs = name
                     break
             else:
                 self._boundAs = "unknown_" + str(id(self))
 
-        boundName = "__klein_bound_{}__".format(self._boundAs)
-        k = getattr(instance, boundName, lambda: None)()
+        boundName = f"__klein_bound_{self._boundAs}__"
+        k = cast(
+            Optional["Klein"], getattr(instance, boundName, lambda: None)()
+        )
 
         if k is None:
             k = self.__class__()
             k._url_map = self._url_map
             k._endpoints = self._endpoints
             k._error_handlers = self._error_handlers
             k._instance = instance
@@ -176,84 +286,101 @@
                 setattr(instance, boundName, kref)
             except AttributeError:
                 pass
 
         return k
 
     @staticmethod
-    def _segments_in_url(url):
+    def _segments_in_url(url: str) -> int:
         segment_count = url.count("/")
         if url.endswith("/"):
             segment_count -= 1
         return segment_count
 
-    def route(self, url, *args, **kwargs):
+    def route(
+        self, url: str, *args: Any, **kwargs: Any
+    ) -> Callable[[KleinRouteHandler], KleinRouteHandler]:
         """
         Add a new handler for C{url} passing C{args} and C{kwargs} directly to
         C{werkzeug.routing.Rule}.  The handler function will be passed at least
         one argument an L{twisted.web.server.Request} and any keyword arguments
         taken from the C{url} pattern.
 
         ::
             @app.route("/")
             def index(request):
                 return "Hello"
 
         @param url: A werkzeug URL pattern given to C{werkzeug.routing.Rule}.
-        @type url: str
-
         @param branch: A bool indiciated if a branch endpoint should
             be added that allows all child path segments that don't
             match some other route to be consumed.  Default C{False}.
-        @type branch: bool
-
 
         @returns: decorated handler function.
         """
         segment_count = self._segments_in_url(url) + self._subroute_segments
 
         @named("router for '" + url + "'")
-        def deco(f):
-            kwargs.setdefault("endpoint", f.__name__)
+        def deco(f: KleinRouteHandler) -> KleinRouteHandler:
+            kwargs.setdefault(
+                "endpoint",
+                f.__name__,  # type: ignore[union-attr]
+            )
             if kwargs.pop("branch", False):
                 branchKwargs = kwargs.copy()
                 branchKwargs["endpoint"] = branchKwargs["endpoint"] + "_branch"
 
-                @modified("branch route '{url}' executor".format(url=url), f)
-                def branch_f(instance, request, *a, **kw):
+                @modified(f"branch route '{url}' executor", f)
+                def branch_f(
+                    instance: Any,
+                    request: IRequest,
+                    *a: Any,
+                    **kw: Any,
+                ) -> KleinRenderable:
                     IKleinRequest(request).branch_segments = kw.pop(
                         "__rest__", ""
                     ).split("/")
                     return _call(instance, f, request, *a, **kw)
 
-                branch_f.segment_count = segment_count
+                branch_f = cast(KleinRouteHandler, branch_f)
+
+                branch_f.segment_count = (  # type: ignore[union-attr]
+                    segment_count
+                )
 
                 self._endpoints[branchKwargs["endpoint"]] = branch_f
                 self._url_map.add(
                     Rule(
                         url.rstrip("/") + "/" + "<path:__rest__>",
                         *args,
-                        **branchKwargs
+                        **branchKwargs,
                     )
                 )
 
-            @modified("route '{url}' executor".format(url=url), f)
-            def _f(instance, request, *a, **kw):
+            @modified(f"route '{url}' executor", f)
+            def _f(
+                instance: Any,
+                request: IRequest,
+                *a: Any,
+                **kw: Any,
+            ) -> KleinRenderable:
                 return _call(instance, f, request, *a, **kw)
 
-            _f.segment_count = segment_count
+            _f = cast(KleinRouteHandler, _f)
+
+            _f.segment_count = segment_count  # type: ignore[union-attr]
 
             self._endpoints[kwargs["endpoint"]] = _f
             self._url_map.add(Rule(url, *args, **kwargs))
             return f
 
         return deco
 
     @contextmanager
-    def subroute(self, prefix):
+    def subroute(self, prefix: str) -> Iterator["Klein"]:
         """
         Within this block, C{@route} adds rules to a
         C{werkzeug.routing.Submount}.
 
         This is implemented by tinkering with the instance's C{_url_map}
         variable. A context manager allows us to gracefully use the pattern of
         "change a variable, do some things with the new value, then put it back
@@ -265,38 +392,61 @@
         Usage:
         ::
             with app.subroute("/prefix") as app:
                 @app.route("/foo")
                 def foo_handler(request):
                     return 'I respond to /prefix/foo'
 
-        @type prefix: string
         @param prefix: The string that will be prepended to the paths of all
                        routes established during the with-block.
-        @return: Returns None.
         """
 
         _map_before_submount = self._url_map
 
         segments = self._segments_in_url(prefix)
 
-        submount_map = namedtuple("submount", ["rules", "add"])(
-            [], lambda r: submount_map.rules.append(r)
-        )
+        class SubmountMap:
+            def __init__(self) -> None:
+                self.rules: List[Rule] = []
+
+            def add(self, rule: Rule) -> None:
+                self.rules.append(rule)
+
+        submount_map = SubmountMap()
 
         try:
-            self._url_map = submount_map
+            self._url_map = cast(Map, submount_map)
             self._subroute_segments += segments
             yield self
             _map_before_submount.add(Submount(prefix, submount_map.rules))
         finally:
             self._url_map = _map_before_submount
             self._subroute_segments -= segments
 
-    def handle_errors(self, f_or_exception, *additional_exceptions):
+    @overload
+    def handle_errors(
+        self,
+        f_or_exception: KleinErrorHandler,
+        *additional_exceptions: Type[Exception],
+    ) -> Callable[[KleinErrorHandler], Callable]:
+        ...  # pragma: no cover
+
+    @overload
+    def handle_errors(
+        self,
+        f_or_exception: Type[Exception],
+        *additional_exceptions: Type[Exception],
+    ) -> Callable[[KleinErrorHandler], Callable]:
+        ...  # pragma: no cover
+
+    def handle_errors(
+        self,
+        f_or_exception: Union[KleinErrorHandler, Type[Exception]],
+        *additional_exceptions: Type[Exception],
+    ) -> Callable[[KleinErrorHandler], Callable]:
         """
         Register an error handler. This decorator supports two syntaxes. The
         simpler of these can be used to register a handler for all C{Exception}
         types::
 
             @app.handle_errors
             def error_handler(request, failure):
@@ -317,132 +467,137 @@
 
         If more than one error handler is registered, the handlers will be
         executed in the order in which they are defined, until a handler is
         encountered which completes successfully. If no handler completes
         successfully, L{twisted.web.server.Request}'s processingFailed() method
         will be called.
 
-        In addition to handling errors that occur within a route handler, error
-        handlers also handle any C{werkzeug.exceptions.HTTPException} which is
-        raised during routing. In particular, C{werkzeug.exceptions.NotFound}
-        will be raised if no matching route is found, so to return a custom 404
-        users can do the following::
+        In addition to handling errors that occur within a L{KleinRouteHandler},
+        error handlers also handle any L{werkzeug.exceptions.HTTPException}
+        which is raised during request routing.
+
+        In particular, C{werkzeug.exceptions.NotFound} will be raised if no
+        matching route is found, so to return a custom 404 users can do the
+        following::
 
             @app.handle_errors(NotFound)
             def error_handler(request, failure):
                 request.setResponseCode(404)
                 return 'Not found'
 
         @param f_or_exception: An error handler function, or an C{Exception}
             subclass to scope the decorated handler to.
-        @type f_or_exception: C{function} or C{Exception}
-
         @param additional_exceptions: Additional C{Exception} subclasses to
             scope the decorated function to.
-        @type additional_exceptions: C{list} of C{Exception}s
 
         @returns: decorated error handler function.
         """
         # Try to detect calls using the "simple" @app.handle_error syntax by
         # introspecting the first argument - if it isn't a type which
         # subclasses Exception we assume the simple syntax was used.
         if not isinstance(f_or_exception, type) or not issubclass(
             f_or_exception, Exception
         ):
-            return self.handle_errors(Exception)(f_or_exception)
+            # f_or_exception is a KleinErrorHandler
+            f = cast(KleinErrorHandler, f_or_exception)
+            return self.handle_errors(Exception)(f)
+
+        # f_or_exception is an Exception class
+        exceptions = [f_or_exception] + list(additional_exceptions)
 
-        def deco(f):
+        def deco(f: KleinErrorHandler) -> Callable:
             @modified("error handling wrapper", f)
-            def _f(instance, request, failure):
+            def _f(
+                instance: Optional["Klein"],
+                request: IRequest,
+                failure: Failure,
+            ) -> KleinRenderable:
                 return _call(instance, f, request, failure)
 
-            self._error_handlers.append(
-                ([f_or_exception] + list(additional_exceptions), _f)
-            )
-            return _f
+            self._error_handlers.append((exceptions, _f))
+
+            return cast(Callable, _f)
 
         return deco
 
     def urlFor(
         self,
-        request,
-        endpoint,
-        values=None,
-        method=None,
-        force_external=False,
-        append_unknown=True,
-    ):
+        request: IRequest,
+        endpoint: str,
+        values: Optional[Mapping[str, KleinQueryValue]] = None,
+        method: Optional[str] = None,
+        force_external: bool = False,
+        append_unknown: bool = True,
+    ) -> str:
         host = request.getHeader(b"host")
         if host is None:
             if force_external:
                 raise ValueError(
                     "Cannot build external URL if request"
                     " doesn't contain Host header"
                 )
             host = b""
-        return self.url_map.bind(host).build(
-            endpoint, values, method, force_external, append_unknown
+        return buildURL(
+            self.url_map.bind(host),
+            endpoint,
+            values,
+            method,
+            force_external,
+            append_unknown,
         )
 
     url_for = urlFor
 
     def run(
         self,
-        host=None,
-        port=None,
-        logFile=None,
-        endpoint_description=None,
-        displayTracebacks=True,
-    ):
+        host: Optional[str] = None,
+        port: Optional[int] = None,
+        logFile: Optional[IO] = None,
+        endpoint_description: Optional[str] = None,
+        displayTracebacks: bool = True,
+    ) -> None:
         """
         Run a minimal twisted.web server on the specified C{port}, bound to the
         interface specified by C{host} and logging to C{logFile}.
 
         This function will run the default reactor for your platform and so
         will block the main thread of your application.  It should be the last
         thing your klein application does.
 
         @param host: The hostname or IP address to bind the listening socket
             to.  "0.0.0.0" will allow you to listen on all interfaces, and
             "127.0.0.1" will allow you to listen on just the loopback
             interface.
-        @type host: str
 
         @param port: The TCP port to accept HTTP requests on.
-        @type port: int
 
         @param logFile: The file object to log to, by default C{sys.stdout}
-        @type logFile: file object
 
         @param endpoint_description: specification of endpoint. Must contain
              protocol, port and interface. May contain other optional arguments,
              e.g. to use SSL: "ssl:443:privateKey=key.pem:certKey=crt.pem"
-        @type endpoint_description: str
 
         @param displayTracebacks: Weather a processing error will result in
             a page displaying the traceback with debugging information or not.
-        @type displayTracebacks: bool
         """
         if logFile is None:
             logFile = sys.stdout
 
         log.startLogging(logFile)
 
         if not endpoint_description:
-            endpoint_description = "tcp:port={0}:interface={1}".format(
-                port, host
-            )
+            endpoint_description = f"tcp:port={port}:interface={host}"
 
-        endpoint = endpoints.serverFromString(reactor, endpoint_description)
+        endpoint = serverFromString(reactor, endpoint_description)
 
         site = Site(self.resource())
         site.displayTracebacks = displayTracebacks
 
         endpoint.listen(site)
-        reactor.run()
+        reactor.run()  # type: ignore[attr-defined]
 
 
 _globalKleinApp = Klein()
 
 route = _globalKleinApp.route
 run = _globalKleinApp.run
 subroute = _globalKleinApp.subroute
```

### Comparing `klein-20.6.0/src/klein/_decorators.py` & `klein-21.8.0/src/klein/_decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import wraps
-from typing import Callable, Optional, Text, TypeVar
+from typing import Callable, Optional, TypeVar
+
 
 C = TypeVar("C", bound=Callable)
 
 
-def bindable(bindable):
-    # type: (C) -> C
+def bindable(bindable: C) -> C:
     """
     Mark a method as a "bindable" method.
 
     If a L{Klein.app} resource is found on an instance object (i.e. is returned
     from C{YourObject().app.resource()}), it will pass C{self} from that
     instance to all of its routes, making a signature of 2 arguments: C{self}
     and C{request} However, if it's found globally (i.e. C{app = Klein()};
@@ -17,27 +17,26 @@
     C{request}.  However, for decorators that must be able to live between
     C{@route} and the user's function, but still need to manipulate the
     C{request} object, they need to be invoked with a consistent argument
     signature.  A method decorated with C{@bindable} will therefore always take
     C{instance, request} as its first two arguments, even if C{instance} is
     C{None} when the L{Klein} object is not bound to an instance.
 
-    @return: its argument, modified to mark it as unconditinally requiring an
+    @return: its argument, modified to mark it as unconditionally requiring an
         instance argument.
     """
     bindable.__klein_bound__ = True  # type: ignore[attr-defined]
     return bindable
 
 
 def modified(
-    modification,  # type: Text
-    original,  # type: Callable
-    modifier=None,  # type: Optional[Callable]
-):
-    # type: (...) -> Callable
+    modification: str,
+    original: Callable,
+    modifier: Optional[Callable] = None,
+) -> Callable:
     """
     Annotate a callable as a modified wrapper of an original callable.
 
     @param modification: A name for the type of modification, for example "form
         processor" or "request forwarder"; this will be tacked on to the name
         of the resulting function.
 
@@ -49,16 +48,15 @@
         to set attributes that will be visible at the top level.
 
     @return: A new callable; this may have a different argument signature or
         return value, and is only related to C{original} in the sense that it
         likely calls it.
     """
 
-    def decorator(wrapper):
-        # type: (Callable[..., C]) -> Callable[..., C]
+    def decorator(wrapper: Callable[..., C]) -> Callable[..., C]:
         result = named(modification + " for " + original.__name__)(
             wraps(original)(wrapper)
         )
         result.__original__ = original  # type: ignore[attr-defined]
         if modifier is not None:
             before = set(wrapper.__dict__.keys())
             result = modifier(result)
@@ -66,33 +64,30 @@
             for key in after - before:
                 setattr(original, key, wrapper.__dict__[key])
         return result
 
     return decorator
 
 
-def named(name):
-    # type: (Text) -> Callable[[C], C]
+def named(name: str) -> Callable[[C], C]:
     """
     Change the name of a function to the given name.
     """
 
-    def decorator(original):
-        # type: (C) -> C
+    def decorator(original: C) -> C:
         original.__name__ = str(name)
         original.__qualname__ = str(name)
         return original
 
     return decorator
 
 
-def originalName(function):
-    # type: (Callable) -> Text
+def originalName(function: Callable) -> str:
     """
     Get the original, user-specified name of C{function}, chasing back any
     wrappers applied with C{modified}.
     """
-    fnext = function  # type: Optional[Callable]
+    fnext: Optional[Callable] = function
     while fnext is not None:
         function = fnext
         fnext = getattr(function, "__original__", None)
     return function.__name__
```

### Comparing `klein-20.6.0/src/klein/_dihttp.py` & `klein-21.8.0/src/klein/_dihttp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,149 +1,151 @@
 """
 Dependency-Injected HTTP metadata.
 """
 
-from typing import Any, Dict, Mapping, Sequence, TYPE_CHECKING, Text, Union
+from typing import Any, Dict, Mapping, Sequence, Type, Union, cast
 
 import attr
-
 from hyperlink import DecodedURL
+from zope.interface import Interface, implementer, provider
 
-from six import text_type
-
-from zope.interface import implementer, provider
-from zope.interface.interfaces import IInterface
+from twisted.python.components import Componentized
+from twisted.web.iweb import IRequest
 
-from .interfaces import IDependencyInjector, IRequiredParameter
+from .interfaces import (
+    IDependencyInjector,
+    IRequestLifecycle,
+    IRequiredParameter,
+)
 
-if TYPE_CHECKING:  # pragma: no cover
-    from klein.interfaces import IRequestLifecycle
-    from twisted.web.iweb import IRequest
-    from twisted.python.components import Componentized
 
-
-def urlFromRequest(request):
-    # type: (IRequest) -> DecodedURL
+def urlFromRequest(request: IRequest) -> DecodedURL:
     sentHeader = request.getHeader(b"host")
     if sentHeader is not None:
         sentHeader = sentHeader.decode("charmap")
         if ":" in sentHeader:
             host, port = sentHeader.split(":")
             port = int(port)
         else:
             host = sentHeader
             port = None
     else:
-        host = request.client.host
-        port = request.client.port
-        if not isinstance(host, text_type):
-            host = host.decode("ascii")
+        client = request.client  # type: ignore[attr-defined]
+        host = client.host
+        port = client.port
 
     url = DecodedURL.fromText(request.uri.decode("charmap"))
     url = url.replace(
-        scheme=u"https" if request.isSecure() else u"http",
+        scheme="https" if request.isSecure() else "http",
         host=host,
         port=port,
     )
     return url
 
 
 @provider(IRequiredParameter, IDependencyInjector)
-class RequestURL(object):
+class RequestURL:
     """
     Require a hyperlink L{DecodedURL} object from a L{Requirer}.
 
     @since: Klein NEXT
     """
 
     @classmethod
     def registerInjector(
-        cls, injectionComponents, parameterName, requestLifecycle
-    ):
-        # type: (Componentized, str, IRequestLifecycle) -> IDependencyInjector
-        return cls()
+        cls,
+        injectionComponents: Componentized,
+        parameterName: str,
+        requestLifecycle: IRequestLifecycle,
+    ) -> IDependencyInjector:
+        # typing note: https://github.com/Shoobx/mypy-zope/issues/39
+        return cast(IDependencyInjector, cls())
 
     @classmethod
-    def injectValue(cls, instance, request, routeParams):
-        # type: (Any, IRequest, Dict[str, Any]) -> DecodedURL
+    def injectValue(
+        cls,
+        instance: Any,
+        request: IRequest,
+        routeParams: Dict[str, Any],
+    ) -> DecodedURL:
         return urlFromRequest(request)
 
     @classmethod
-    def finalize(cls):
-        # type: () -> None
+    def finalize(cls) -> None:
         "Nothing to do upon finalization."
 
 
 @implementer(IRequiredParameter, IDependencyInjector)
-@attr.s(frozen=True)
-class RequestComponent(object):
+@attr.frozen
+class RequestComponent:
     """
     Require a hyperlink L{DecodedURL} object from a L{Requirer}.
 
     @since: Klein NEXT
     """
 
-    interface = attr.ib(type=IInterface)
+    interface: Type[Interface]
 
     def registerInjector(
-        self, injectionComponents, parameterName, requestLifecycle
-    ):
-        # type: (Componentized, str, IRequestLifecycle) -> IDependencyInjector
+        self,
+        injectionComponents: Componentized,
+        parameterName: str,
+        requestLifecycle: IRequestLifecycle,
+    ) -> IDependencyInjector:
         return self
 
-    def injectValue(self, instance, request, routeParams):
-        # type: (Any, IRequest, Dict[str, Any]) -> DecodedURL
-        return request.getComponent(self.interface)
+    def injectValue(
+        self, instance: Any, request: IRequest, routeParams: Dict[str, Any]
+    ) -> DecodedURL:
+        return cast(
+            DecodedURL,
+            cast(Componentized, request).getComponent(self.interface),
+        )
 
-    def finalize(cls):
-        # type: () -> None
+    def finalize(cls) -> None:
         "Nothing to do upon finalization."
 
 
-@attr.s(frozen=True)
-class Response(object):
+@attr.s(auto_attribs=True, frozen=True)
+class Response:
     """
     Metadata about an HTTP response, with an object that Klein knows how to
     understand.
 
     This includes:
 
         - an HTTP response code
 
         - some HTTP headers
 
         - a body object, which can be anything else Klein understands; for
-          example, an IResource, an IRenderable, text, bytes, etc.
+          example, an IResource, an IRenderable, str, bytes, etc.
 
     @since: Klein NEXT
     """
 
-    code = attr.ib(type=int, default=200)
-    headers = attr.ib(
-        type=Mapping[
-            Union[Text, bytes], Union[Text, bytes, Sequence[Union[Text, bytes]]]
-        ],
-        default=attr.Factory(dict),
-    )
-    body = attr.ib(type=Any, default=u"")
+    code: int = 200
+    headers: Mapping[
+        Union[str, bytes], Union[str, bytes, Sequence[Union[str, bytes]]]
+    ] = attr.ib(factory=dict)
+    body: Any = ""
 
-    def _applyToRequest(self, request):
-        # type: (IRequest) -> Any
+    def _applyToRequest(self, request: IRequest) -> Any:
         """
         Apply this L{Response} to the given L{IRequest}, setting its response
         code and headers.
 
         Private because:
 
             - this should only ever be applied by Klein, and
 
             - hopefully someday soon this will be replaced with something that
               actually creates a txrequest-style response object.
         """
         request.setResponseCode(self.code)
         for headerName, headerValueOrValues in self.headers.items():
-            if not isinstance(headerValueOrValues, (text_type, bytes)):
+            if not isinstance(headerValueOrValues, (str, bytes)):
                 headerValues = headerValueOrValues
             else:
                 headerValues = [headerValueOrValues]
             request.responseHeaders.setRawHeaders(headerName, headerValues)
         return self.body
```

### Comparing `klein-20.6.0/src/klein/_form.py` & `klein-21.8.0/src/klein/_form.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,71 @@
 # -*- test-case-name: klein.test.test_form -*-
 
-from __future__ import print_function, unicode_literals
-
 import json
 from typing import (
     Any,
     AnyStr,
     Callable,
     Dict,
+    Generator,
     Iterable,
     List,
+    NoReturn,
     Optional,
     Sequence,
-    Text,
     Type,
     cast,
 )
 
 import attr
+from zope.interface import Attribute, Interface, implementer
 
 from twisted.internet.defer import Deferred, inlineCallbacks
 from twisted.python.components import Componentized, registerAdapter
 from twisted.web.error import MissingRenderMethod
 from twisted.web.http import FORBIDDEN
 from twisted.web.iweb import IRenderable, IRequest
 from twisted.web.resource import Resource
 from twisted.web.template import Element, Tag, TagLoader, tags
 
-from zope.interface import Interface, implementer
-
-from ._app import _call
+from ._app import KleinRenderable, _call
 from ._decorators import bindable
-from ._typing import DefaultNamedArg, NoReturn
 from .interfaces import (
     EarlyExit,
     IDependencyInjector,
     IRequestLifecycle,
     IRequiredParameter,
     ISession,
     SessionMechanism,
     ValidationError,
     ValueAbsent,
 )
 
 
-class CrossSiteRequestForgery(Resource, object):
+class CrossSiteRequestForgery(Resource):
     """
     Cross site request forgery detected.  Request aborted.
     """
 
-    def __init__(self, message):
-        # type: (str) -> None
-        super(CrossSiteRequestForgery, self).__init__()
+    def __init__(self, message: str) -> None:
+        super().__init__()
         self.message = message
 
-    def render(self, request):
-        # type: (IRequest) -> bytes
+    def render(self, request: IRequest) -> bytes:
         """
         For all HTTP methods, return a 403.
         """
         request.setResponseCode(FORBIDDEN, b"FAILURECSRF")
         return ("CSRF TOKEN FAILURE: " + self.message).encode("utf-8")
 
 
 CSRF_PROTECTION = "__csrf_protection__"
 
 
-def textConverter(value):
-    # type: (AnyStr) -> Text
+def textConverter(value: AnyStr) -> str:
     """
     Converter for form values (which may be any type of string) into text.
     """
     if isinstance(value, bytes):
         return value.decode("utf-8")
     else:
         return value
@@ -83,134 +77,135 @@
     """
 
     # TODO: how to allow applications to pass options to loads, such as
     # parse_float?
 
 
 @implementer(IRequiredParameter)
-@attr.s(frozen=True)
-class Field(object):
+@attr.s(auto_attribs=True, frozen=True)
+class Field:
     """
     A L{Field} is a static part of a L{Form}.
 
     @ivar converter: The converter.
     """
 
-    converter = attr.ib(type=Callable[[AnyStr], Any])
-    formInputType = attr.ib(type=str)
-    pythonArgumentName = attr.ib(type=Optional[str], default=None)
-    formFieldName = attr.ib(type=Optional[str], default=None)
-    formLabel = attr.ib(type=Optional[str], default=None)
-    default = attr.ib(type=Optional[Any], default=None, cmp=False)
-    required = attr.ib(type=bool, default=True)
-    noLabel = attr.ib(type=bool, default=False)
-    value = attr.ib(type=Text, default="")
-    error = attr.ib(type=ValidationError, default=None)
+    converter: Callable[[AnyStr], Any]
+    formInputType: str
+    pythonArgumentName: Optional[str] = None
+    formFieldName: Optional[str] = None
+    formLabel: Optional[str] = None
+    default: Optional[Any] = attr.ib(default=None, cmp=False)
+    required: bool = True
+    noLabel: bool = False
+    value: str = ""
+    error: Optional[ValidationError] = None
 
     # IRequiredParameter
     def registerInjector(
-        self, injectionComponents, parameterName, requestLifecycle
-    ):
-        # type: (Componentized, str, IRequestLifecycle) -> IDependencyInjector
+        self,
+        injectionComponents: Componentized,
+        parameterName: str,
+        requestLifecycle: IRequestLifecycle,
+    ) -> IDependencyInjector:
         """
         Register this form field as a dependency injector.
         """
         protoForm = IProtoForm(injectionComponents)
         return cast(
             IDependencyInjector,
             protoForm.addField(self.maybeNamed(parameterName)),
         )
 
-    def maybeNamed(self, name):
-        # type: (str) -> Field
+    def maybeNamed(self, name: str) -> "Field":
         """
         Create a new L{Field} like this one, but with all the name default
         values filled in.
 
         @param name: the name.
-        @type name: a native L{str}
         """
 
-        def maybe(it, that=name):
-            # type: (Optional[str], Optional[str]) -> Optional[str]
+        def maybe(
+            it: Optional[str], that: Optional[str] = name
+        ) -> Optional[str]:
             return that if it is None else it
 
         return attr.assoc(
             self,
             pythonArgumentName=maybe(self.pythonArgumentName),
             formFieldName=maybe(self.formFieldName),
             formLabel=maybe(
                 self.formLabel, name.capitalize() if not self.noLabel else None
             ),
         )
 
-    def asTags(self):
-        # type: () -> Iterable[Tag]
+    def asTags(self) -> Iterable[Tag]:
         """
         Convert this L{Field} into some stuff that can be rendered in a
         L{twisted.web.template}.
 
         @return: A new set of tags to include in a template.
-        @rtype: iterable of L{twisted.web.template.Tag}
         """
         value = self.value
         if value is None:
             value = ""  # type: ignore[unreachable]
         input_tag = tags.input(
-            type=self.formInputType, name=self.formFieldName, value=value
+            type=self.formInputType,
+            name=self.formFieldName,  # type: ignore[arg-type]
+            value=value,
         )
         error_tags = []
         if self.error:
             error_tags.append(
                 tags.div(class_="klein-form-validation-error")(
-                    self.error.message
+                    self.error.message  # type: ignore[arg-type]
                 )
             )
         if self.formLabel:
             yield tags.label(self.formLabel, ": ", input_tag, *error_tags)
         else:
             yield input_tag
-            yield error_tags
+            yield from error_tags
 
-    def extractValue(self, request):
-        # type: (IRequest) -> Any
+    def extractValue(self, request: IRequest) -> Any:
         """
         Extract a value from the request.
 
         In the case of key/value form posts, this attempts to reliably make the
-        value into Text.  In the case of a JSON post, however, it will simply
+        value into str.  In the case of a JSON post, however, it will simply
         extract the value from the top-level dictionary, which means it could
         be any arrangement of JSON-serializiable objects.
         """
         fieldName = self.formFieldName
         if fieldName is None:
             raise ValueError("Cannot extract unnamed form field.")
         contentType = request.getHeader(b"content-type")
         if contentType is not None and contentType.startswith(
             b"application/json"
         ):
             # TODO: parse only once, please.
-            parsed = request.getComponent(IParsedJSONBody)
+            parsed = cast(Componentized, request).getComponent(IParsedJSONBody)
             if parsed is None:
                 request.content.seek(0)
                 octets = request.content.read()
                 characters = octets.decode("utf-8")
                 parsed = json.loads(characters)
-                request.setComponent(IParsedJSONBody, parsed)
+                cast(Componentized, request).setComponent(
+                    IParsedJSONBody, parsed
+                )
             if fieldName not in parsed:
                 return None
             return parsed[fieldName]
         allValues = request.args.get(fieldName.encode("utf-8"))
         if allValues:
             return allValues[0].decode("utf-8")
         else:
             return None
 
-    def validateValue(self, value):
-        # type: (Any) -> Any
+    def validateValue(self, value: Any) -> Any:
         """
         Validate the given text and return a converted Python object to use, or
         fail with L{ValidationError}.
 
         @param value: The value that was extracted by L{Field.extractValue}.
 
         @return: The converted value.
@@ -222,124 +217,118 @@
                 return self.default
         try:
             return self.converter(value)
         except ValueError as ve:
             raise ValidationError(str(ve))
 
     @classmethod
-    def text(cls, **kw):  # type: (**Any) -> Field
+    def text(cls, **kw: Any) -> "Field":
         """
         Shorthand for a form field that contains a short string, and will be
         rendered as a plain <input>.
         """
         return cls(converter=textConverter, formInputType="text", **kw)
 
     @classmethod
-    def password(cls, **kw):  # type: (**Any) -> Field
+    def password(cls, **kw: Any) -> "Field":
         """
         Shorthand for a form field that, like L{text}, contains a short string,
         but should be obscured when typed (and, to the extent possible,
         obscured in other sensitive contexts, such as logging.)
         """
         return cls(converter=textConverter, formInputType="password", **kw)
 
     @classmethod
-    def hidden(cls, name, value, **kw):
-        # type: (str, Text, **Any) -> Field
+    def hidden(cls, name: str, value: str, **kw: Any) -> "Field":
         """
         Shorthand for a hidden field.
         """
         return cls(
             converter=textConverter,
             formInputType="hidden",
             noLabel=True,
             value=value,
-            **kw
+            **kw,
         ).maybeNamed(name)
 
     @classmethod
-    def number(cls, minimum=None, maximum=None, kind=float, **kw):
-        # type: (Optional[int], Optional[int], Type, **Any) -> Field
+    def number(
+        cls,
+        minimum: Optional[int] = None,
+        maximum: Optional[int] = None,
+        kind: Type = float,
+        **kw: Any,
+    ) -> "Field":
         """
         An integer within the range [minimum, maximum].
         """
 
-        def bounded_number(text):
-            # type: (AnyStr) -> Any
+        def bounded_number(text: AnyStr) -> Any:
             try:
                 value = kind(text)
             except (ValueError, ArithmeticError):
                 raise ValidationError("not a valid number")
             else:
                 if minimum is not None and value < minimum:
                     raise ValidationError("value must be >=" + repr(minimum))
                 if maximum is not None and value > maximum:
                     raise ValidationError("value must be <=" + repr(maximum))
                 return value
 
         return cls(converter=bounded_number, formInputType="number", **kw)
 
     @classmethod
-    def submit(cls, value):
-        # type: (Text) -> Field
+    def submit(cls, value: str) -> "Field":
         """
         A field representing a submit button, with a value (displayed on the
         button).
         """
         return cls(
             converter=textConverter,
             formInputType="submit",
             noLabel=True,
             default=value,
         )
 
 
 @implementer(IRenderable)
-@attr.s
-class RenderableForm(object):
+@attr.s(auto_attribs=True)
+class RenderableForm:
     """
     An L{IRenderable} representing a renderable form.
 
     @ivar prevalidationValues: a L{dict} mapping {L{Field}: L{list} of
-        L{Text}}, representing the value that each field received as part of
+        L{str}}, representing the value that each field received as part of
         the request.
 
     @ivar validationErrors: a L{dict} mapping {L{Field}: L{ValidationError}}
     """
 
-    _form = attr.ib(type="Form")
-    _session = attr.ib(type=ISession)
-    _action = attr.ib(type=str)
-    _method = attr.ib(type=str)
-    _enctype = attr.ib(type=str)
-    _encoding = attr.ib(type=str)
-    prevalidationValues = attr.ib(
-        type=Dict[Field, Optional[Text]],
-        default=cast(Dict[Field, Optional[Text]], attr.Factory(dict)),
-    )
-    validationErrors = attr.ib(
-        type=Dict[Field, ValidationError],
-        default=cast(Dict[Field, ValidationError], attr.Factory(dict)),
-    )
+    _form: "IForm"
+    _session: ISession
+    _action: str
+    _method: str
+    _enctype: str
+    _encoding: str
+    prevalidationValues: Dict[Field, Optional[str]] = attr.ib(factory=dict)
+    validationErrors: Dict[Field, ValidationError] = attr.ib(factory=dict)
 
     ENCTYPE_FORM_DATA = "multipart/form-data"
     ENCTYPE_URL_ENCODED = "application/x-www-form-urlencoded"
 
-    def _fieldForCSRF(self):
-        # type: () -> Field
+    def _fieldForCSRF(self) -> Field:
         """
         @return: A hidden L{Field} containing the cross-site request forgery
             protection token.
         """
         return Field.hidden(CSRF_PROTECTION, self._session.identifier)
 
-    def _fieldsToRender(self):
-        # type: () -> Iterable[Field]
+    def _fieldsToRender(self) -> Iterable[Field]:
         """
-        @return: an interable of L{Field} objects to include in the HTML
+        @return: an iterable of L{Field} objects to include in the HTML
             representation of this form.  This includes:
 
                 - all the user-specified fields in the form
 
                 - the CSRF protection hidden field
 
                 - if no "submit" buttons are included in the form, one
@@ -363,81 +352,72 @@
                 formFieldName="__klein_auto_submit__",
             )
         if self._method.lower() == "post":
             yield self._fieldForCSRF()
 
     # Public interface below.
 
-    def lookupRenderMethod(self, name):
-        # type: (str) -> NoReturn
+    def lookupRenderMethod(self, name: str) -> NoReturn:
         """
         Form renderers don't supply any render methods, so this just always
         raises L{MissingRenderMethod}.
         """
         raise MissingRenderMethod(self, name)
 
-    def render(self, request):
-        # type: (IRequest) -> Tag
+    def render(self, request: IRequest) -> Tag:  # type: ignore[override]
         """
         Render this form to the given request.
         """
         formAttributes = {
             "accept-charset": self._encoding,
             "class": "klein-form",
         }
         if self._method.lower() == "post":
             # Enctype has no meaning on method="GET" forms.
             formAttributes.update(enctype=self._enctype)
         return tags.form(
             action=self._action, method=self._method, **formAttributes
         )(field.asTags() for field in self._fieldsToRender())
 
-    def glue(self):
-        # type: () -> Iterable[Tag]
+    def glue(self) -> List[Tag]:
         """
         Provide any glue necessary to render this form; this must be dropped
         into the template within the C{<form>} tag.
 
         Presently, this glue includes only the CSRF token argument, but Klein
         reserves the right to add arbitrary HTML here.  This should not create
         any user-visible content, however.
 
         @return: some HTML elements in the form of renderable objects for
             L{twisted.web.template}
-        @rtype: L{twisted.web.template.Tag}, or L{list} thereof.
         """
-        return self._fieldForCSRF().asTags()
+        return list(self._fieldForCSRF().asTags())
 
 
 @bindable
 def defaultValidationFailureHandler(
-    instance,  # type: Optional[object]
-    request,  # type: IRequest
-    fieldValues,  # type: FieldValues
-):
-    # type: (...) -> Element
+    instance: Optional[object],
+    request: IRequest,
+    fieldValues: "FieldValues",
+) -> Element:
     """
     This is the default validation failure handler, which will be used by form
     handlers (i.e. any routes which use L{klein.Requirer} to require a field)
     in the case of any input validation failure when no other validation
     failure handler is registered via L{Form.onValidationFailureFor}.
 
     Its behavior is to simply return an HTML rendering of the form object,
     which includes inline information about fields which failed to validate.
 
     @param instance: The instance associated with the router that the form
         handler was handled on.
-    @type instance: L{object}
-
     @param request: The request including the form submission.
-    @type request: L{twisted.web.iweb.IRequest}
-
     @return: Any object acceptable from a Klein route.
     """
-    session = request.getComponent(ISession)
+    session = cast(Componentized, request).getComponent(ISession)
     request.setResponseCode(400)
     enctype = (
         (
             request.getHeader(b"content-type")
             or RenderableForm.ENCTYPE_URL_ENCODED.encode("ascii")
         )
         .split(b";")[0]
@@ -458,167 +438,197 @@
     )
 
     return Element(TagLoader(renderable))
 
 
 _requirerFunctionWithForm = Any
 _routeCallable = Any
-_routeDecorator = Callable[
-    [_routeCallable, DefaultNamedArg(Any, "__session__")], _routeCallable
-]
-_validationFailureHandler = Callable[
-    [Optional[object], IRequest, "Form", Dict[str, str]], Element
-]
-
-validationFailureHandlerAttribute = "__kleinFormValidationFailureHandlers__"
 
 
 class IProtoForm(Interface):
     """
     Marker interface for L{ProtoForm}.
     """
 
+    fields: Sequence[Field] = Attribute("Form fields")
+
+    def addField(field: Field) -> "FieldInjector":
+        """
+        Add the given field to the form ultimately created here.
+        """
+
 
 class IForm(Interface):
     """
     Marker interface for form attached to dependency injection components.
     """
 
+    fields: Sequence[Field] = Attribute("Form fields")
+
+    def populateRequestValues(
+        injectionComponents: Componentized,
+        instance: Any,
+        request: IRequest,
+    ) -> Deferred:
+        """
+        Extract the values present in this request and populate a
+        L{FieldValues} object.
+        """
+
 
 @implementer(IProtoForm)
-@attr.s
-class ProtoForm(object):
+@attr.s(auto_attribs=True)
+class ProtoForm:
     """
     Form-builder.
     """
 
-    _componentized = attr.ib(type=Componentized)
-    _lifecycle = attr.ib(type=IRequestLifecycle)
-    _fields = attr.ib(type=List[Field], default=attr.Factory(list))
+    _componentized: Componentized
+    _lifecycle: IRequestLifecycle
+    fields: List[Field] = attr.ib(factory=list)
 
     @classmethod
-    def fromComponentized(cls, componentized):
-        # type: (Componentized) -> ProtoForm
+    def fromComponentized(cls, componentized: Componentized) -> "ProtoForm":
         """
         Create a ProtoForm from a componentized object.
         """
-        rl = IRequestLifecycle(componentized)  # type: ignore[operator]
+        rl = IRequestLifecycle(componentized)
         assert rl is not None
         return cls(componentized, rl)
 
-    def addField(self, field):
-        # type: (Field) -> FieldInjector
-        """
-        Add the given field to the form ultimately created here.
-        """
-        self._fields.append(field)
+    def addField(self, field: Field) -> "FieldInjector":
+        self.fields.append(field)
         return FieldInjector(self._componentized, field, self._lifecycle)
 
 
 class IFieldValues(Interface):
     """
     Marker interface for parsed fields.
     """
 
+    form: IForm = Attribute("Form")
+    arguments: Dict[str, Any] = Attribute("Arguments")
+    prevalidationValues: Dict[Field, Optional[str]] = Attribute(
+        "Pre-validation values"
+    )
+    validationErrors: Dict[Field, ValidationError] = Attribute(
+        "Validation errors"
+    )
+
+    def validate(instance: Any, request: IRequest) -> Deferred:
+        """
+        If any validation errors have occurred, raise a relevant exception.
+        """
+
 
 @implementer(IFieldValues)
-@attr.s
-class FieldValues(object):
+@attr.s(auto_attribs=True)
+class FieldValues:
     """
     Reified post-parsing values for HTTP form submission.
     """
 
-    form = attr.ib(type="Form")
-    arguments = attr.ib(type=Dict[str, Any])
-    prevalidationValues = attr.ib(type=Dict[Field, Optional[Text]])
-    validationErrors = attr.ib(type=Dict[Field, ValidationError])
-    _injectionComponents = attr.ib(type=Componentized)
+    form: "Form"
+    arguments: Dict[str, Any]
+    prevalidationValues: Dict[Field, Optional[str]]
+    validationErrors: Dict[Field, ValidationError]
+    _injectionComponents: Componentized
 
     @inlineCallbacks
-    def validate(self, instance, request):
-        # type: (Any, IRequest) -> Deferred
-        """
-        If any validation errors have occurred, raise a relevant exception.
-        """
+    def validate(
+        self, instance: Any, request: IRequest
+    ) -> Generator[Any, object, None]:
         if self.validationErrors:
-            result = yield _call(
-                instance,
-                IValidationFailureHandler(
-                    self._injectionComponents, defaultValidationFailureHandler
+            result = cast(
+                KleinRenderable,
+                (
+                    yield _call(
+                        instance,
+                        IValidationFailureHandler(
+                            self._injectionComponents,
+                            defaultValidationFailureHandler,
+                        ),
+                        request,
+                        self,
+                    )
                 ),
-                request,
-                self,
             )
             raise EarlyExit(result)
 
 
 @implementer(IDependencyInjector)
-@attr.s
-class FieldInjector(object):
+@attr.s(auto_attribs=True)
+class FieldInjector:
     """
     Field injector.
     """
 
-    _componentized = attr.ib(type=Componentized)
-    _field = attr.ib(type=Field)
-    _lifecycle = attr.ib(type=IRequestLifecycle)
-
-    def injectValue(self, instance, request, routeParams):
-        # type: (Any, IRequest, Dict[str, Any]) -> Any
+    _componentized: Componentized
+    _field: Field
+    _lifecycle: IRequestLifecycle
+
+    def injectValue(
+        self, instance: Any, request: IRequest, routeParams: Dict[str, Any]
+    ) -> Any:
         """
         Inject the given value into the form.
         """
+        assert self._field.pythonArgumentName is not None
         return IFieldValues(request).arguments.get(
             self._field.pythonArgumentName
         )
 
-    def finalize(self):
-        # type: () -> None
+    def finalize(self) -> None:
         """
         Finalize this ProtoForm into a real form.
         """
         if IForm(self._componentized, None) is not None:
             return
 
-        finalForm = cast(IForm, Form(IProtoForm(self._componentized)._fields))
+        finalForm = cast(IForm, Form(IProtoForm(self._componentized).fields))
         self._componentized.setComponent(IForm, finalForm)
 
         # XXX set requiresComponents argument here to ISession if CSRF is
         # required; add flag somewhere to indicate if a form is
         # side-effect-free (like a search field) that can be handled even
         # without a CSRF token.
         @bindable
-        def populateValuesHook(instance, request):
-            # type: (Any, IRequest) -> Deferred
+        def populateValuesHook(instance: Any, request: IRequest) -> Deferred:
             return finalForm.populateRequestValues(
                 self._componentized, instance, request
             )
 
         self._lifecycle.addPrepareHook(
-            populateValuesHook, provides=[IFieldValues], requires=[ISession],
+            populateValuesHook,
+            provides=[IFieldValues],
+            requires=[ISession],
         )
 
 
 registerAdapter(ProtoForm.fromComponentized, Componentized, IProtoForm)
 
 
 class IValidationFailureHandler(Interface):
     """
     Validation failure handler callable interface.
     """
 
+    def __call__(request: IRequest) -> KleinRenderable:
+        """
+        Called to handle a validation failure.
+        """
+
 
-def checkCSRF(request):
-    # type: (IRequest) -> None
+def checkCSRF(request: IRequest) -> None:
     """
     Check the request for cross-site request forgery, raising an EarlyExit if
     it is found.
     """
     # TODO: optionalize CSRF protection for GET forms
-    session = ISession(request, None)  # type: ignore[operator]
+    session = ISession(request, None)
     token = None
     if request.method in (b"GET", b"HEAD"):
         # Idempotent requests don't require CRSF validation.  (Don't have
         # destructive GETs or bad stuff will happen to you in general!)
         return
     if session is not None:
         if session.authenticatedBy == SessionMechanism.Header:
@@ -632,30 +642,30 @@
             0
         ].decode("ascii")
         if token == session.identifier:
             # The token matches.  We're OK.
             return
     # leak only the value passed, not the actual token, just in
     # case there's some additional threat vector there
-    raise EarlyExit(
-        CrossSiteRequestForgery("Invalid CSRF token: {!r}".format(token))
-    )
+    raise EarlyExit(CrossSiteRequestForgery(f"Invalid CSRF token: {token!r}"))
 
 
-@attr.s(hash=False)
-class Form(object):
+@implementer(IForm)
+@attr.s(auto_attribs=True, hash=False)
+class Form:
     """
     A L{Form} is a collection of fields attached to a function.
     """
 
-    fields = attr.ib(type=Sequence[Field])
+    fields: Sequence[Field]
 
     @staticmethod
-    def onValidationFailureFor(handler):
-        # type: (_requirerFunctionWithForm) -> Callable[[Callable], Callable]
+    def onValidationFailureFor(
+        handler: _requirerFunctionWithForm,
+    ) -> Callable[[Callable], Callable]:
         """
         Register a function to be run in the event of a validation failure for
         the input to a particular form handler.
 
         Generally used like so::
 
             requirer = Requirer(...)
@@ -680,30 +690,29 @@
             L{Form.handler} - for which the decorated function will handle
             validation failures.
 
         @return: a decorator that decorates a function with the signature
             C{(request, form) -> thing klein can render}.
         """
 
-        def decorate(decoratee):
-            # type: (Callable) -> Callable
+        def decorate(decoratee: Callable) -> Callable:
             handler.injectionComponents.setComponent(
                 IValidationFailureHandler, decoratee
             )
             return decoratee
 
         return decorate
 
     @inlineCallbacks
-    def populateRequestValues(self, injectionComponents, instance, request):
-        # type: (Componentized, Any, IRequest) -> Deferred
-        """
-        Extract the values present in this request and populate a
-        L{FieldValues} object.
-        """
+    def populateRequestValues(
+        self,
+        injectionComponents: Componentized,
+        instance: Any,
+        request: IRequest,
+    ) -> Generator[Any, object, None]:
         assert IFieldValues(request, None) is None
 
         validationErrors = {}
         prevalidationValues = {}
         arguments = {}
 
         checkCSRF(request)
@@ -724,33 +733,32 @@
             self,
             arguments,
             prevalidationValues,
             validationErrors,
             injectionComponents,
         )
         yield values.validate(instance, request)
-        request.setComponent(IFieldValues, values)
+        cast(Componentized, request).setComponent(IFieldValues, values)
 
     @classmethod
     def rendererFor(
         cls,
-        decoratedFunction,  # type: _requirerFunctionWithForm
-        action,  # type: Text
-        method="POST",  # type: Text
-        enctype=RenderableForm.ENCTYPE_FORM_DATA,  # type: Text
-        encoding="utf-8",  # type: str
-    ):
-        # type: (...) -> RenderableFormParam
+        decoratedFunction: _requirerFunctionWithForm,
+        action: str,
+        method: str = "POST",
+        enctype: str = RenderableForm.ENCTYPE_FORM_DATA,
+        encoding: str = "utf-8",
+    ) -> "RenderableFormParam":
         """
         A form parameter that can render a form declared as a number of fields
         on another route.
 
         Use like so::
 
-            class MyFormApp(object):
+            class MyFormApp:
                 router = Klein()
                 requirer = Requirer()
 
                 @requirer.require(
                     router.route("/handle-form", methods=["POST"]),
                     name=Field.text(), value=Field.integer(),
                 )
@@ -763,56 +771,58 @@
                 )
                 def showForm(self, form):
                     return form
 
         As a L{RenderableForm} provides L{IRenderable}, you may return the
         parameter directly
         """
-        form = IForm(
+        form: Optional[IForm] = IForm(
             decoratedFunction.injectionComponents, None
-        )  # type: Optional[Form]
+        )
         if form is None:
             form = Form([])
         return RenderableFormParam(form, action, method, enctype, encoding)
 
 
 @implementer(IRequiredParameter, IDependencyInjector)
-@attr.s
-class RenderableFormParam(object):
+@attr.s(auto_attribs=True)
+class RenderableFormParam:
     """
     A L{RenderableFormParam} implements L{IRequiredParameter} and
     L{IDependencyInjector} to provide a L{RenderableForm} to your route.
     """
 
-    _form = attr.ib(type=Form)
-    _action = attr.ib(type=Text)
-    _method = attr.ib(type=Text)
-    _enctype = attr.ib(type=Text)
-    _encoding = attr.ib(type=Text)
+    _form: IForm
+    _action: str
+    _method: str
+    _enctype: str
+    _encoding: str
 
     def registerInjector(
-        self, injectionComponents, parameterName, requestLifecycle
-    ):
-        # type: (Componentized, str, IRequestLifecycle) -> RenderableFormParam
+        self,
+        injectionComponents: Componentized,
+        parameterName: str,
+        requestLifecycle: IRequestLifecycle,
+    ) -> "RenderableFormParam":
         return self
 
-    def injectValue(self, instance, request, routeParams):
-        # type: (Any, IRequest, Dict[str, Any]) -> RenderableForm
+    def injectValue(
+        self, instance: Any, request: IRequest, routeParams: Dict[str, Any]
+    ) -> RenderableForm:
         """
         Create the renderable form from the request.
         """
         return RenderableForm(
             self._form,
-            ISession(request),  # type: ignore[operator]
+            ISession(request),
             self._action,
             self._method,
             self._enctype,
             self._encoding,
             prevalidationValues={},
             validationErrors={},
         )
 
-    def finalize(self):
-        # type: () -> None
+    def finalize(self) -> None:
         """
         Nothing to do upon finalization.
         """
```

### Comparing `klein-20.6.0/src/klein/_headers.py` & `klein-21.8.0/src/klein/_headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,204 +1,200 @@
 # -*- test-case-name: klein.test.test_request -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 HTTP headers API.
 """
 
-from typing import AnyStr, Iterable, Text, Tuple, Union
+from typing import AnyStr, Iterable, Tuple, Union
 
 from attr import Factory, attrib, attrs
-
 from zope.interface import implementer
 
-from ._imessage import MutableRawHeaders, RawHeader, RawHeaders
-from ._interfaces import IHTTPHeaders, IMutableHTTPHeaders
+from ._imessage import (
+    IHTTPHeaders,
+    IMutableHTTPHeaders,
+    MutableRawHeaders,
+    RawHeader,
+    RawHeaders,
+)
 
 
 __all__ = ()
 
 
-String = Union[bytes, Text]
+String = Union[bytes, str]
 
 
 # Encoding/decoding header data
 
 HEADER_NAME_ENCODING = "iso-8859-1"
 HEADER_VALUE_ENCODING = "iso-8859-1"
 
 
-def headerNameAsBytes(name):
-    # type: (String) -> bytes
+def headerNameAsBytes(name: String) -> bytes:
     """
     Convert a header name to bytes if necessary.
     """
     if isinstance(name, bytes):
         return name
     else:
         return name.encode(HEADER_NAME_ENCODING)
 
 
-def headerNameAsText(name):
-    # type: (String) -> Text
+def headerNameAsText(name: String) -> str:
     """
-    Convert a header name to text if necessary.
+    Convert a header name to str if necessary.
     """
-    if isinstance(name, Text):
+    if isinstance(name, str):
         return name
     else:
         return name.decode(HEADER_NAME_ENCODING)
 
 
-def headerValueAsBytes(value):
-    # type: (String) -> bytes
+def headerValueAsBytes(value: String) -> bytes:
     """
     Convert a header value to bytes if necessary.
     """
     if isinstance(value, bytes):
         return value
     else:
         return value.encode(HEADER_VALUE_ENCODING)
 
 
-def headerValueAsText(value):
-    # type: (String) -> Text
+def headerValueAsText(value: String) -> str:
     """
-    Convert a header value to text if necessary.
+    Convert a header value to str if necessary.
     """
-    if isinstance(value, Text):
+    if isinstance(value, str):
         return value
     else:
         return value.decode(HEADER_VALUE_ENCODING)
 
 
-def normalizeHeaderName(name):
-    # type: (AnyStr) -> AnyStr
+def normalizeHeaderName(name: AnyStr) -> AnyStr:
     """
     Normalize a header name.
     """
     return name.lower()
 
 
 # Internal data representation
 
 
-def normalizeRawHeaders(headerPairs):
-    # type: (Iterable[Iterable[String]]) -> Iterable[RawHeader]
+def normalizeRawHeaders(
+    headerPairs: Iterable[Iterable[String]],
+) -> Iterable[RawHeader]:
     for pair in headerPairs:
         try:
             name, value = pair
         except ValueError:
             raise ValueError("header pair must be a 2-item iterable")
 
         name = normalizeHeaderName(headerNameAsBytes(name))
         value = headerValueAsBytes(value)
 
         yield (normalizeHeaderName(name), value)
 
 
-def normalizeRawHeadersFrozen(headerPairs):
-    # type: (Iterable[Iterable[bytes]]) -> RawHeaders
+def normalizeRawHeadersFrozen(
+    headerPairs: Iterable[Iterable[bytes]],
+) -> RawHeaders:
     return tuple(normalizeRawHeaders(headerPairs))
 
 
-def normalizeRawHeadersMutable(headerPairs):
-    # type: (Iterable[Iterable[bytes]]) -> MutableRawHeaders
+def normalizeRawHeadersMutable(
+    headerPairs: Iterable[Iterable[bytes]],
+) -> MutableRawHeaders:
     return list(normalizeRawHeaders(headerPairs))
 
 
-def getFromRawHeaders(rawHeaders, name):
-    # type: (RawHeaders, AnyStr) -> Iterable[AnyStr]
+def getFromRawHeaders(rawHeaders: RawHeaders, name: AnyStr) -> Iterable[AnyStr]:
     """
     Get a value from raw headers.
     """
     if isinstance(name, bytes):
         name = normalizeHeaderName(name)
         return (v for n, v in rawHeaders if name == n)
 
-    if isinstance(name, Text):
+    if isinstance(name, str):
         rawName = headerNameAsBytes(normalizeHeaderName(name))
         return (headerValueAsText(v) for n, v in rawHeaders if rawName == n)
 
-    raise TypeError("name {!r} must be text or bytes".format(name))
+    raise TypeError(f"name {name!r} must be str or bytes")
 
 
-def rawHeaderName(name):
-    # type: (String) -> bytes
+def rawHeaderName(name: String) -> bytes:
     if isinstance(name, bytes):
         return name
-    elif isinstance(name, Text):
+    elif isinstance(name, str):
         return headerNameAsBytes(name)
     else:
-        raise TypeError("name {!r} must be text or bytes".format(name))
+        raise TypeError(f"name {name!r} must be str or bytes")
 
 
-def rawHeaderNameAndValue(name, value):
-    # type: (String, String) -> Tuple[bytes, bytes]
+def rawHeaderNameAndValue(name: String, value: String) -> Tuple[bytes, bytes]:
     if isinstance(name, bytes):
         if not isinstance(value, bytes):
             raise TypeError(
                 "value {!r} must be bytes to match name {!r}".format(
                     value, name
                 )
             )
         return (name, value)
 
-    elif isinstance(name, Text):
-        if not isinstance(value, Text):
+    elif isinstance(name, str):
+        if not isinstance(value, str):
             raise TypeError(
-                "value {!r} must be text to match name {!r}".format(value, name)
+                f"value {value!r} must be str to match name {name!r}"
             )
         return (headerNameAsBytes(name), headerValueAsBytes(value))
 
     else:
-        raise TypeError("name {!r} must be text or bytes".format(name))
+        raise TypeError(f"name {name!r} must be str or bytes")
 
 
 # Implementation
 
 
 @implementer(IHTTPHeaders)
 @attrs(frozen=True)
-class FrozenHTTPHeaders(object):
+class FrozenHTTPHeaders:
     """
     Immutable HTTP entity headers.
     """
 
-    rawHeaders = attrib(
-        converter=normalizeRawHeadersFrozen, default=(),
-    )  # type: RawHeaders
+    rawHeaders: RawHeaders = attrib(
+        converter=normalizeRawHeadersFrozen,
+        default=(),
+    )
 
-    def getValues(self, name):
-        # type: (AnyStr) -> Iterable[AnyStr]
+    def getValues(self, name: AnyStr) -> Iterable[AnyStr]:
         return getFromRawHeaders(self.rawHeaders, name)
 
 
 @implementer(IMutableHTTPHeaders)
 @attrs(frozen=True)
-class MutableHTTPHeaders(object):
+class MutableHTTPHeaders:
     """
     Mutable HTTP entity headers.
     """
 
-    _rawHeaders = attrib(
-        converter=normalizeRawHeadersMutable, default=Factory(list),
-    )  # type: MutableRawHeaders
+    _rawHeaders: MutableRawHeaders = attrib(
+        converter=normalizeRawHeadersMutable,
+        default=Factory(list),
+    )
 
     @property
-    def rawHeaders(self):
-        # type: () -> RawHeaders
+    def rawHeaders(self) -> RawHeaders:
         return tuple(self._rawHeaders)
 
-    def getValues(self, name):
-        # type: (AnyStr) -> Iterable[AnyStr]
+    def getValues(self, name: AnyStr) -> Iterable[AnyStr]:
         return getFromRawHeaders(self._rawHeaders, name)
 
-    def remove(self, name):
-        # type: (String) -> None
+    def remove(self, name: String) -> None:
         rawName = rawHeaderName(name)
 
         self._rawHeaders[:] = [p for p in self._rawHeaders if p[0] != rawName]
 
-    def addValue(self, name, value):
-        # type: (AnyStr, AnyStr) -> None
+    def addValue(self, name: AnyStr, value: AnyStr) -> None:
         self._rawHeaders.append(rawHeaderNameAndValue(name, value))
```

### Comparing `klein-20.6.0/src/klein/_headers_compat.py` & `klein-21.8.0/src/klein/_headers_compat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- test-case-name: klein.test.test_headers -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Support for interoperability with L{twisted.web.http_headers.Headers}.
 """
 
-from typing import AnyStr, Iterable, Text, Tuple
+from typing import AnyStr, Iterable, Tuple, cast
 
 from attr import attrib, attrs
 from attr.validators import instance_of
+from zope.interface import implementer
 
 from twisted.web.http_headers import Headers
 
-from zope.interface import implementer
-
 from ._headers import (
     IMutableHTTPHeaders,
     RawHeaders,
     String,
     headerNameAsBytes,
     headerValueAsText,
     normalizeHeaderName,
@@ -27,57 +26,59 @@
 
 
 __all__ = ()
 
 
 @implementer(IMutableHTTPHeaders)
 @attrs(frozen=True)
-class HTTPHeadersWrappingHeaders(object):
+class HTTPHeadersWrappingHeaders:
     """
     HTTP entity headers.
 
     This is an L{IMutableHTTPHeaders} implementation that wraps a L{Headers}
     object.
     """
 
     # NOTE: In case Headers has different ideas about encoding text than we do,
-    # always interact with it using bytes, not text.
+    # always interact with it using bytes, not str.
 
-    _headers = attrib(validator=instance_of(Headers))  # type: Headers
+    _headers: Headers = attrib(validator=instance_of(Headers))
 
     @property
-    def rawHeaders(self):
-        # type: () -> RawHeaders
-        def pairs():
-            # type: () -> Iterable[Tuple[bytes, bytes]]
+    def rawHeaders(self) -> RawHeaders:
+        def pairs() -> Iterable[Tuple[bytes, bytes]]:
             for name, values in self._headers.getAllRawHeaders():
                 name = normalizeHeaderName(name)
                 for value in values:
                     yield (name, value)
 
         return tuple(pairs())
 
-    def getValues(self, name):
-        # type: (AnyStr) -> Iterable[AnyStr]
+    def getValues(self, name: AnyStr) -> Iterable[AnyStr]:
         if isinstance(name, bytes):
-            values = self._headers.getRawHeaders(name, default=())
-        elif isinstance(name, Text):
-            values = (
-                headerValueAsText(value)
-                for value in self._headers.getRawHeaders(
+            values = cast(
+                Iterable[AnyStr], self._headers.getRawHeaders(name, default=())
+            )
+        elif isinstance(name, str):
+            # typing note: getRawHeaders is typed to return an optional even if
+            # default is not None. We could assert not None, but are casting
+            # here so that if the hints for getRawHeaders are fixed later,
+            # mypy will tell us to remove the useless cast.
+            values = cast(
+                Iterable[str],
+                self._headers.getRawHeaders(
                     headerNameAsBytes(name), default=()
-                )
+                ),
             )
+            values = (headerValueAsText(value) for value in values)
         else:
-            raise TypeError("name {!r} must be text or bytes".format(name))
+            raise TypeError(f"name {name!r} must be str or bytes")
 
         return values
 
-    def remove(self, name):
-        # type: (String) -> None
+    def remove(self, name: String) -> None:
         self._headers.removeHeader(rawHeaderName(name))
 
-    def addValue(self, name, value):
-        # type: (AnyStr, AnyStr) -> None
+    def addValue(self, name: AnyStr, value: AnyStr) -> None:
         rawName, rawValue = rawHeaderNameAndValue(name, value)
 
         self._headers.addRawHeader(rawName, rawValue)
```

### Comparing `klein-20.6.0/src/klein/_imessage.py` & `klein-21.8.0/src/klein/_imessage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Interfaces related to HTTP messages.
 
 Do not import directly from here, except:
  - From _interfaces.py.
  - From implementations of these interfaces, but even then, import the
    zope.interface.Interface classes via _interfaces.py.
 
 This will ensure that type checking works.
 """
 
-from typing import AnyStr, Iterable, MutableSequence, Sequence, Text, Tuple
+from typing import AnyStr, Iterable, MutableSequence, Sequence, Tuple
 
 from hyperlink import DecodedURL
-
 from tubes.itube import IFount
-
-from twisted.internet.defer import Deferred
-
 from zope.interface import Attribute, Interface
 
-from ._typing import ifmethod
-
 
 __all__ = ()
 
 
 RawHeader = Tuple[bytes, bytes]
 RawHeaders = Sequence[RawHeader]
 MutableRawHeaders = MutableSequence[RawHeader]
@@ -64,83 +58,75 @@
     Note that header name bytes should be strictly encoded as ASCII; this
     interface uses ISO-8859-1 to provide interoperability with (naughty) HTTP
     implementations that send non-ASCII data.
     Because ISO-8859-1 is a superset of ASCII, this will still work for
     well-behaved implementations.
     """
 
-    rawHeaders = Attribute(
+    rawHeaders: RawHeaders = Attribute(
         """
         Raw header data as a tuple in the from: C{((name, value), ...)}.
         C{name} and C{value} are bytes.
         Headers are provided in the order that they were received.
         Headers with multiple values are provided as separate name and value
         pairs.
         """
-    )  # type: RawHeaders
+    )
 
-    @ifmethod
-    def getValues(name):
-        # type: (AnyStr) -> Iterable[AnyStr]
+    def getValues(name: AnyStr) -> Iterable[AnyStr]:
         """
         Get the values associated with the given header name.
 
         If the given name is L{bytes}, the value will be returned as the raw
         header L{bytes}.
 
-        If the given name is L{Text}, the name will be encoded as ISO-8859-1
+        If the given name is L{str}, the name will be encoded as ISO-8859-1
         and the value will be returned as text, by decoding the raw header
         value bytes with ISO-8859-1.
 
         @param name: The name of the header to look for.
 
         @return: The values of the header with the given name.
         """
 
 
 class IMutableHTTPHeaders(IHTTPHeaders):
     """
     Mutable HTTP entity headers.
     """
 
-    @ifmethod
-    def remove(name):
-        # type: (AnyStr) -> None
+    def remove(name: AnyStr) -> None:
         """
         Remove all header name/value pairs for the given header name.
 
-        If the given name is L{Text}, it will be encoded as ISO-8859-1 before
+        If the given name is L{str}, it will be encoded as ISO-8859-1 before
         comparing to the (L{bytes}) header names.
 
         @param name: The name of the header to remove.
         """
 
-    @ifmethod
-    def addValue(name, value):
-        # type: (AnyStr, AnyStr) -> None
+    def addValue(name: AnyStr, value: AnyStr) -> None:
         """
         Add the given header name/value pair.
 
         If the given name is L{bytes}, the value must also be L{bytes}.
 
-        If the given name is L{Text}, it will be encoded as ISO-8859-1, and the
-        value, which must also be L{Text}, will be encoded as ISO-8859-1.
+        If the given name is L{str}, it will be encoded as ISO-8859-1, and the
+        value, which must also be L{str}, will be encoded as ISO-8859-1.
         """
 
 
 class IHTTPMessage(Interface):
     """
     HTTP entity.
     """
 
-    headers = Attribute("Entity headers.")  # type: IHTTPHeaders
+    headers: IHTTPHeaders = Attribute("Entity headers.")
 
-    @ifmethod
-    def bodyAsFount():
-        # type: () -> IFount
+    def bodyAsFount() -> IFount:
         """
         The entity body, as a fount.
 
         @note: The fount may only be accessed once.
             It provides a mechanism for accessing the body as a stream of data,
             potentially as it is read from the network, without having to cache
             the entire body, which may be large.
@@ -148,17 +134,15 @@
             accessing the fount a second time.
             Attempting to do so will raise L{FountAlreadyAccessedError}.
 
         @raise FountAlreadyAccessedError: If the fount has previously been
             accessed.
         """
 
-    @ifmethod
-    def bodyAsBytes():
-        # type: () -> Deferred[bytes]
+    async def bodyAsBytes() -> bytes:
         """
         The entity body, as bytes.
 
         @note: This necessarily reads the entire entity body into memory,
             which may be a problem if the body is large.
 
         @note: This method caches the body, which means that unlike
@@ -176,17 +160,17 @@
 
 
 class IHTTPRequest(IHTTPMessage):
     """
     HTTP request.
     """
 
-    method = Attribute("Request method.")  # type: Text
-    uri = Attribute("Request URI.")  # type: DecodedURL
+    method: str = Attribute("Request method.")
+    uri: DecodedURL = Attribute("Request URI.")
 
 
 class IHTTPResponse(IHTTPMessage):
     """
     HTTP response.
     """
 
-    status = Attribute("Response status code.")  # type: int
+    status: int = Attribute("Response status code.")
```

### Comparing `klein-20.6.0/src/klein/_isession.py` & `klein-21.8.0/src/klein/_isession.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-from typing import Any, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Sequence, Type
 
 import attr
-
-try:
-    from constantly import NamedConstant, Names
-except ImportError:  # pragma: no cover
-    from twisted.python.constants import NamedConstant, Names
-
+from constantly import NamedConstant, Names
 from zope.interface import Attribute, Interface
 
-from ._typing import ifmethod
+from twisted.internet.defer import Deferred
+from twisted.python.components import Componentized
+from twisted.web.iweb import IRequest
+
 
-if TYPE_CHECKING:  # pragma: no cover
-    from twisted.internet.defer import Deferred
-    from twisted.python.components import Componentized
-    from typing import Dict, Iterable, Text, Sequence
-    from twisted.web.iweb import IRequest
-    from zope.interface.interfaces import IInterface
+if TYPE_CHECKING:
+    from ._app import KleinRenderable
 
 
 class NoSuchSession(Exception):
     """
     No such session could be found.
     """
 
@@ -33,32 +27,113 @@
 
 class TransactionEnded(Exception):
     """
     Exception raised when.
     """
 
 
+class SessionMechanism(Names):
+    """
+    Mechanisms which can be used to identify and authenticate a session.
+
+    @cvar Cookie: The Cookie session mechanism involves looking up the session
+        identifier via an HTTP cookie.  Session objects retrieved via this
+        mechanism may be vulnerable to U{CSRF attacks
+        <https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)>}
+        and therefore must have CSRF protections applied to them.
+
+    @cvar Header: The Header mechanism retrieves the session identifier via a
+        separate header such as C{"X-Auth-Token"}.  Since a different-origin
+        site in a browser can easily send a form submission including cookies,
+        but I{can't} easily put stuff into other arbitrary headers, this does
+        not require additional protections.
+    """
+
+    Cookie = NamedConstant()
+    Header = NamedConstant()
+
+
+class ISession(Interface):
+    """
+    An L{ISession} provider contains an identifier for the session, information
+    about how the session was negotiated with the client software, and
+    """
+
+    identifier = Attribute(
+        """
+        L{str} identifying a session.
+
+        This value should be:
+
+            1. I{unique} - no two sessions have the same identifier
+
+            2. I{unpredictable} - no one but the receipient of the session
+               should be able to guess what it is
+
+            3. I{opaque} - it should contain no interesting information
+        """
+    )
+
+    isConfidential = Attribute(
+        """
+        A L{bool} indicating whether this session mechanism transmitted over an
+        encrypted transport, i.e., HTTPS.  If C{True}, this means that this
+        session can be used for sensitive information; otherwise, the
+        information contained in it should be considered to be available to
+        attackers.
+        """
+    )
+
+    authenticatedBy = Attribute(
+        """
+        A L{SessionMechanism} indicating what mechanism was used to
+        authenticate this session.
+        """
+    )
+
+    def authorize(interfaces: Iterable[Type[Interface]]) -> Deferred:
+        """
+        Retrieve other objects from this session.
+
+        This method is how you can retrieve application-specific objects from
+        the general-purpose session; define interfaces for each facet of
+        something accessible to a session, then pass it here and to the
+        L{ISessionStore} implementation you're using.
+
+        @param interfaces: A list of interfaces.
+
+        @return: all of the providers that could be retrieved from the session.
+        @rtype: L{Deferred} firing with L{dict} mapping
+            L{zope.interface.interfaces.IInterface} to providers of each
+            interface.  Interfaces which cannot be authorized will not be
+            present as keys in this dictionary.
+        """
+
+
 class ISessionStore(Interface):
     """
     Backing storage for sessions.
     """
 
-    @ifmethod
-    def newSession(isConfidential, authenticatedBy):
-        # type: (bool, SessionMechanism) -> Deferred
+    def newSession(
+        isConfidential: bool,
+        authenticatedBy: SessionMechanism,
+    ) -> Deferred:
         """
         Create a new L{ISession}.
 
         @return: a new session with a new identifier.
         @rtype: L{Deferred} firing with L{ISession}.
         """
 
-    @ifmethod
-    def loadSession(identifier, isConfidential, authenticatedBy):
-        # type: (Text, bool, SessionMechanism) -> Deferred
+    def loadSession(
+        identifier: str,
+        isConfidential: bool,
+        authenticatedBy: SessionMechanism,
+    ) -> Deferred:
         """
         Load a session given the given identifier and security properties.
 
         As an optimization for session stores where the back-end can generate
         session identifiers when the presented one is not found in the same
         round-trip to a data store, this method may return a L{Session} object
         with an C{identifier} attribute that does not match C{identifier}.
@@ -69,17 +144,15 @@
         session should be valid already.
 
         @return: an existing session with the given identifier.
         @rtype: L{Deferred} firing with L{ISession} or failing with
             L{NoSuchSession}.
         """
 
-    @ifmethod
-    def sentInsecurely(identifiers):
-        # type: (Sequence[Text]) -> None
+    def sentInsecurely(identifiers: Sequence[str]) -> None:
         """
         The transport layer has detected that the given identifiers have been
         sent over an unauthenticated transport.
         """
 
 
 class ISimpleAccountBinding(Interface):
@@ -88,44 +161,36 @@
     accounts - i.e. those using username, password, and email address as a
     method to authenticate a user.
 
     This goes into a user-authentication-capable L{ISession} object's C{data}
     attribute as a component.
     """
 
-    @ifmethod
-    def bindIfCredentialsMatch(username, password):
-        # type: (Text, Text) -> None
+    def bindIfCredentialsMatch(username: str, password: str) -> None:
         """
         Attach the session this is a component of to an account with the given
         username and password, if the given username and password correctly
         authenticate a principal.
         """
 
-    @ifmethod
-    def boundAccounts():
-        # type: () -> Deferred
+    def boundAccounts() -> Deferred:
         """
         Retrieve the accounts currently associated with the session this is a
         component of.
 
         @return: L{Deferred} firing with a L{list} of L{ISimpleAccount}.
         """
 
-    @ifmethod
-    def unbindThisSession():
-        # type: () -> None
+    def unbindThisSession() -> None:
         """
         Disassociate the session this is a component of from any accounts it's
         logged in to.
         """
 
-    @ifmethod
-    def createAccount(username, email, password):
-        # type: (Text, Text, Text) -> None
+    def createAccount(username: str, email: str, password: str) -> None:
         """
         Create a new account with the given username, email and password.
         """
 
 
 class ISimpleAccount(Interface):
     """
@@ -140,51 +205,47 @@
 
     accountID = Attribute(
         """
         Unicode account-ID.
         """
     )
 
-    def bindSession(self, session):
-        # type: (ISession) -> None
+    def bindSession(session: ISession) -> None:
         """
         Bind the given session to this account; i.e. authorize the given
         session to act on behalf of this account.
         """
 
-    def changePassword(self, newPassword):
-        # type: (Text) -> None
+    def changePassword(newPassword: str) -> None:
         """
         Change the password of this account.
         """
 
 
 class ISessionProcurer(Interface):
     """
     An L{ISessionProcurer} wraps an L{ISessionStore} and can procure sessions
     that store, given HTTP request objects.
     """
 
-    def procureSession(self, request, forceInsecure=False):
-        # type: (IRequest, bool, bool) -> Deferred
+    def procureSession(
+        request: IRequest, forceInsecure: bool = False
+    ) -> Deferred:
         """
         Retrieve a session using whatever technique is necessary.
 
         If the request already identifies an existing session in the store,
         retrieve it.  If not, create a new session and retrieve that.
 
         @param request: The request to procure a session from.
-        @type request: L{twisted.web.server.Request}
-
         @param forceInsecure: Even if the request was transmitted securely
             (i.e. over HTTPS), retrieve the session that would be used by the
             same browser if it were sending an insecure (i.e. over HTTP)
             request; by default, this is False, and the session's security will
             match that of the request.
-        @type forceInsecure: L{bool}
 
         @return: a L{Deferred} that:
 
                 - fires with an L{ISession} provider if the request describes
                   an existing, valid session, or, if the intersection of the
                   data in the request and the configuration of this
                   L{ISessionProcurer} allow for a cookie to be set immediately,
@@ -196,109 +257,25 @@
                   authentication (and therefore does not want a new cookie set)
                   or if this procurer is configured not to automatically create
                   new sessions on the fly, or
 
                 - fails with L{TooLateForCookies} if the request bound to this
                   procurer has already sent the headers and therefore we can no
                   longer set a cookie, and we need to set a cookie.
-
-        @rtype: L{Session}
-        """
-
-
-class SessionMechanism(Names):
-    """
-    Mechanisms which can be used to identify and authenticate a session.
-
-    @cvar Cookie: The Cookie session mechanism involves looking up the session
-        identifier via an HTTP cookie.  Session objects retrieved via this
-        mechanism may be vulnerable to U{CSRF attacks
-        <https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)>}
-        and therefore must have CSRF protections applied to them.
-
-    @cvar Header: The Header mechanism retrieves the session identifier via a
-        separate header such as C{"X-Auth-Token"}.  Since a different-origin
-        site in a browser can easily send a form submission including cookies,
-        but I{can't} easily put stuff into other arbitrary headers, this does
-        not require additional protections.
-    """
-
-    Cookie = NamedConstant()
-    Header = NamedConstant()
-
-
-class ISession(Interface):
-    """
-    An L{ISession} provider contains an identifier for the session, information
-    about how the session was negotiated with the client software, and
-    """
-
-    identifier = Attribute(
-        """
-        L{unicode} identifying a session.
-
-        This value should be:
-
-            1. I{unique} - no two sessions have the same identifier
-
-            2. I{unpredictable} - no one but the receipient of the session
-               should be able to guess what it is
-
-            3. I{opaque} - it should contain no interesting information
-        """
-    )
-
-    isConfidential = Attribute(
-        """
-        A L{bool} indicating whether this session mechanism transmitted over an
-        encrypted transport, i.e., HTTPS.  If C{True}, this means that this
-        session can be used for sensitive information; otherwise, the
-        information contained in it should be considered to be available to
-        attackers.
-        """
-    )
-
-    authenticatedBy = Attribute(
-        """
-        A L{SessionMechanism} indicating what mechanism was used to
-        authenticate this session.
-        """
-    )
-
-    @ifmethod
-    def authorize(interfaces):
-        # type: (Iterable[IInterface]) -> Deferred
-        """
-        Retrieve other objects from this session.
-
-        This method is how you can retrieve application-specific objects from
-        the general-purpose session; define interfaces for each facet of
-        something accessible to a session, then pass it here and to the
-        L{ISessionStore} implementation you're using.
-
-        @param interfaces: A list of interfaces.
-        @type interfaces: L{iterable} of
-            L{zope.interface.interfaces.IInterface}
-
-        @return: all of the providers that could be retrieved from the session.
-        @rtype: L{Deferred} firing with L{dict} mapping
-            L{zope.interface.interfaces.IInterface} to providers of each
-            interface.  Interfaces which cannot be authorized will not be
-            present as keys in this dictionary.
         """
 
 
 class IDependencyInjector(Interface):
     """
     An injector for a given dependency.
     """
 
-    @ifmethod
-    def injectValue(instance, request, routeParams):
-        # type: (Any, IRequest, Dict[str, Any]) -> Any
+    def injectValue(
+        instance: Any, request: IRequest, routeParams: Dict[str, Any]
+    ) -> Any:
         """
         Return a value to be injected into the parameter name specified by the
         IRequiredParameter.  This may return a Deferred, or an object, or an
         object directly providing the relevant interface.
 
         @param instance: The instance to which the Klein router processing this
             request is bound.
@@ -306,41 +283,60 @@
         @param request: The request being processed.
 
         @param routeParams: A (read-only) copy of the the arguments passed to
             the route by the layer below dependency injection (for example, URL
             parameters).
         """
 
-    @ifmethod
-    def finalize():
-        # type: () -> None
+    def finalize() -> None:
         """
         Finalize this injector before allowing the route to be created.
 
         Finalization generally includes:
 
             - attaching any hooks to the request lifecycle object that need to
               be run before/after each request
 
             - attaching any finalized component objects to the
               injectionComponents originally passed along to the
               IRequiredParameter that created this IDependencyInjector.
+        """
+
+
+class IRequestLifecycle(Interface):
+    """
+    Interface for adding hooks to the phases of a request's lifecycle.
+    """
 
+    def addPrepareHook(
+        beforeHook: Callable,
+        requires: Sequence[Type[Interface]] = (),
+        provides: Sequence[Type[Interface]] = (),
+    ) -> None:
+        """
+        Add a hook that promises to prepare the request by supplying the given
+        interfaces as components on the request, and requires the given
+        requirements.
+
+        Prepare hooks are run I{before any} L{IDependencyInjector}s I{inject
+        their values}.
         """
 
 
 class IRequiredParameter(Interface):
     """
     A declaration that a given Python parameter is required to satisfy a given
     dependency at request-handling time.
     """
 
-    @ifmethod
-    def registerInjector(injectionComponents, parameterName, lifecycle):
-        # type: (Componentized, str, IRequestLifecycleT) -> IDependencyInjector
+    def registerInjector(
+        injectionComponents: Componentized,
+        parameterName: str,
+        lifecycle: IRequestLifecycle,
+    ) -> IDependencyInjector:
         """
         Register the given injector at method-decoration time, informing it of
         its Python parameter name.
 
         @note: this happens at I{route definition} time, after all other
             injectors have been registered by
             L{IRequiredParameter.registerInjector}.
@@ -352,34 +348,19 @@
             to those lists.  These hooks are supplied here rather than relying
             on C{injectValue} to run the requisite logic each time so that
             DependencyInjectors may cooperate on logic that needs to be
             duplicated, such as provisioning a session.
         """
 
 
-class IRequestLifecycle(Interface):
-    """
-    Interface for adding hooks to the phases of a request's lifecycle.
-    """
-
-
-if TYPE_CHECKING:  # pragma: no cover
-    from typing import Union
-    from ._requirer import RequestLifecycle
-
-    IRequestLifecycleT = Union[RequestLifecycle, IRequestLifecycle]
-
-
-@attr.s
+@attr.s(auto_attribs=True)
 class EarlyExit(Exception):
     """
     An L{EarlyExit} may be raised by any of the code that runs in the
     before-request dependency injection code path when using
     L{klein.Requirer.require}.
 
     @ivar alternateReturnValue: The return value which should instead be
         supplied as the route's response.
-    @type alternateReturnValue: Any type that's acceptable to return from a
-        Klein route.
     """
 
-    alternateReturnValue = attr.ib(type=Any)
+    alternateReturnValue: "KleinRenderable"
```

### Comparing `klein-20.6.0/src/klein/_message.py` & `klein-21.8.0/src/klein/_message.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 # -*- test-case-name: klein.test.test_message -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 HTTP message API.
 """
 
 from typing import Any, Optional, Union
 
 from attr import attrib, attrs
 from attr.validators import instance_of, optional
-
 from tubes.itube import IFount
 
-from twisted.internet.defer import Deferred, succeed
-
 from ._imessage import FountAlreadyAccessedError
 from ._tubes import bytesToFount, fountToBytes
 
 
 __all__ = ()
 
 
 InternalBody = Union[bytes, IFount]
 
 
 @attrs(frozen=False)
-class MessageState(object):
+class MessageState:
     """
     Internal mutable state for HTTP message implementations in L{klein}.
     """
 
-    cachedBody = attrib(
-        type=Optional[bytes],
-        validator=optional(instance_of(bytes)),
-        default=None,
-        init=False,
+    cachedBody: Optional[bytes] = attrib(
+        validator=optional(instance_of(bytes)), default=None, init=False
     )
 
-    fountExhausted = attrib(
-        type=bool, validator=instance_of(bool), default=False, init=False
+    fountExhausted: bool = attrib(
+        validator=instance_of(bool), default=False, init=False
     )
 
 
-def validateBody(instance, attribute, body):
-    # type: (Any, Any, InternalBody) -> None
+def validateBody(instance: Any, attribute: Any, body: InternalBody) -> None:
     """
     Validator for L{InternalBody}.
     """
 
     if not isinstance(body, bytes) and not IFount.providedBy(body):
         raise TypeError("body must be bytes or IFount")
 
 
-def bodyAsFount(body, state):
-    # type: (InternalBody, MessageState) -> IFount
+def bodyAsFount(body: InternalBody, state: MessageState) -> IFount:
     """
     Return a fount for a given L{InternalBody}.
     """
 
     if state.fountExhausted:
         raise FountAlreadyAccessedError()
     state.fountExhausted = True
@@ -66,29 +58,23 @@
         return bytesToFount(body)
 
     # assuming: IFount.providedBy(body)
 
     return body
 
 
-def bodyAsBytes(body, state):
-    # type: (InternalBody, MessageState) -> Deferred[bytes]
+async def bodyAsBytes(body: InternalBody, state: MessageState) -> bytes:
     """
     Return bytes for a given L{InternalBody}.
     """
 
     if isinstance(body, bytes):
-        return succeed(body)
+        return body
 
     # assuming: IFount.providedBy(body)
 
     if state.cachedBody is not None:
-        return succeed(state.cachedBody)
+        return state.cachedBody
+
+    state.cachedBody = await fountToBytes(body)
 
-    def cache(bodyBytes):
-        # type: (bytes) -> bytes
-        state.cachedBody = bodyBytes
-        return bodyBytes
-
-    d = fountToBytes(body)
-    d.addCallback(cache)
-    return d
+    return state.cachedBody
```

### Comparing `klein-20.6.0/src/klein/_plating.py` & `klein-21.8.0/src/klein/_plating.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,55 +3,46 @@
 """
 Templating wrapper support for Klein.
 """
 
 from functools import partial
 from json import dumps
 from operator import setitem
-from typing import Any, Callable, TYPE_CHECKING, Tuple, cast
+from typing import Any, Callable, Generator, List, Tuple, cast
 
 import attr
 
-from six import integer_types, string_types, text_type
-
-from twisted.internet.defer import inlineCallbacks, returnValue
+from twisted.internet.defer import inlineCallbacks
 from twisted.web.error import MissingRenderMethod
-from twisted.web.template import Element, TagLoader
+from twisted.web.iweb import IRequest
+from twisted.web.template import Element, Tag, TagLoader
 
 from ._app import _call
 from ._decorators import bindable, modified, originalName
 
-if TYPE_CHECKING:  # pragma: no cover
-    from twisted.internet.defer import Deferred
-    from twisted.web.iweb import IRequest
-    from twisted.web.template import Tag
-    from typing import List
 
-    Deferred, IRequest, Tag
-    StackType = List[Tuple[Any, Callable[[Any], None]]]
+StackType = List[Tuple[Any, Callable[[Any], None]]]
 
 # https://github.com/python/mypy/issues/224
 ATOM_TYPES = (
-    cast(Tuple[Any, ...], integer_types)
-    + cast(Tuple[Any, ...], string_types)
+    cast(Tuple[Any, ...], (int,))
+    + cast(Tuple[Any, ...], (str,))
     + cast(Tuple[Any, ...], (float, None.__class__))
 )
 
 
-def _should_return_json(request):
-    # type: (IRequest) -> bool
+def _should_return_json(request: IRequest) -> bool:
     """
     Should the given request result in a JSON entity-body?
     """
     return bool(request.args.get(b"json"))
 
 
 @inlineCallbacks
-def resolveDeferredObjects(root):
-    # type: (Any) -> Deferred
+def resolveDeferredObjects(root: Any) -> Generator[Any, object, Any]:
     """
     Wait on possibly nested L{Deferred}s that represent a JSON
     serializable object.
 
     @param root: JSON-serializable object that may contain
         L{Deferred}s that resolve to JSON-serializable objects, or a
         L{Deferred} that resolves to one.
@@ -59,26 +50,26 @@
     @return: A L{Deferred} that fires with a L{Deferred}-free version
         of C{root}, or that fails with the first exception
         encountered.
     """
 
     result = [None]
     setResult = partial(setitem, result, 0)
-    stack = [(root, setResult)]  # type: StackType
+    stack: StackType = [(root, setResult)]
 
     while stack:
         mightBeDeferred, setter = stack.pop()
         # inlineCallbacks pauses the generator only on yielded
         # Deferreds. It's resumed immediately with any other object.
         # Consequently coroutines must be wrapped in ensureDeferred.
         obj = yield mightBeDeferred
         if isinstance(obj, ATOM_TYPES):
             setter(obj)
         elif isinstance(obj, list):
-            parent = [None] * len(obj)  # type: Any
+            parent: Any = [None] * len(obj)
             setter(parent)
             stack.extend(
                 reversed(
                     [
                         (child, partial(setitem, parent, i))
                         for i, child in enumerate(obj)
                     ]
@@ -113,26 +104,27 @@
 
                 stack.append((value, setValue))
                 stack.append((key, setKey))
         elif isinstance(obj, PlatedElement):
             stack.append((obj._asJSON(), setter))
         else:
             raise TypeError(
-                obj, "{input} not JSON serializable".format(input=obj),
+                obj,
+                f"{obj} not JSON serializable",
             )
 
-    returnValue(result[0])
+    return result[0]
 
 
 def _extra_types(input):
     """
     Renderability for a few additional types.
     """
-    if isinstance(input, (float,) + integer_types):
-        return text_type(input)
+    if isinstance(input, (float, int)):
+        return str(input)
     return input
 
 
 class PlatedElement(Element):
     """
     The element type returned by L{Plating}.  This contains several utility
     renderers.
@@ -146,15 +138,15 @@
 
         @param preloaded: The pre-loaded data.
         """
         self.slot_data = slot_data
         self._boundInstance = boundInstance
         self._presentationSlots = presentationSlots
         self._renderers = renderers
-        super(PlatedElement, self).__init__(
+        super().__init__(
             loader=TagLoader(
                 preloaded.fillSlots(
                     **{k: _extra_types(v) for k, v in slot_data.items()}
                 )
             )
         )
 
@@ -171,16 +163,17 @@
         """
         @return: a renderer.
         """
         if name in self._renderers:
             wrapped = self._renderers[name]
 
             @modified("plated render wrapper", wrapped)
-            def renderWrapper(request, tag, *args, **kw):
-                # type: (IRequest, Tag, *Any, **Any) -> Any
+            def renderWrapper(
+                request: IRequest, tag: Tag, *args: Any, **kw: Any
+            ) -> Any:
                 return _call(
                     self._boundInstance, wrapped, request, tag, *args, **kw
                 )
 
             return renderWrapper
         if ":" not in name:
             raise MissingRenderMethod(self, name)
@@ -195,120 +188,115 @@
         }
         if type in types:
             return types[type]
         else:
             raise MissingRenderMethod(self, name)
 
 
-class Plating(object):
+class Plating:
     """
     A L{Plating} is a container which can be used to generate HTML from data.
 
     Its name is derived both from tem-I{plating} and I{chrome plating}.
     """
 
     CONTENT = "klein:plating:content"
 
     def __init__(self, defaults=None, tags=None, presentation_slots=()):
-        """
-        """
+        """ """
         self._defaults = {} if defaults is None else defaults
         self._loader = TagLoader(tags)
         self._presentationSlots = {self.CONTENT} | set(presentation_slots)
         self._renderers = {}
 
     def renderMethod(self, renderer):
         """
         Add a render method to this L{Plating} object that can be used in the
         top-level template.
 
         The name of the renderer to use within the template is the name of the
         decorated function.
         """
-        self._renderers[text_type(originalName(renderer))] = renderer
+        self._renderers[str(originalName(renderer))] = renderer
         return renderer
 
     def routed(self, routing, tags):
-        """
-        """
+        """ """
 
         def mydecorator(method):
             loader = TagLoader(tags)
 
             @modified("plating route renderer", method, routing)
             @bindable
             @inlineCallbacks
-            def mymethod(instance, request, *args, **kw):
-                # type: (Any, IRequest, *Any, **Any) -> Any
+            def mymethod(
+                instance: Any, request: IRequest, *args: Any, **kw: Any
+            ) -> Any:
                 data = yield _call(instance, method, request, *args, **kw)
                 if _should_return_json(request):
                     json_data = self._defaults.copy()
                     json_data.update(data)
                     for ignored in self._presentationSlots:
                         json_data.pop(ignored, None)
-                    text_type = u"json"
+                    request.setHeader(b"content-type", b"application/json")
                     ready = yield resolveDeferredObjects(json_data)
                     result = dumps(ready)
                 else:
                     data[self.CONTENT] = loader.load()
-                    text_type = u"html"
+                    request.setHeader(
+                        b"content-type", b"text/html; charset=utf-8"
+                    )
                     result = self._elementify(instance, data)
-                request.setHeader(
-                    b"content-type",
-                    (
-                        u"text/{format}; charset=utf-8".format(
-                            format=text_type
-                        ).encode("charmap")
-                    ),
-                )
-                returnValue(result)
+                return result
 
             return method
 
         return mydecorator
 
     def _elementify(self, instance, to_fill_with):
         """
         Convert this L{Plating} into a L{PlatedElement}.
         """
         slot_data = self._defaults.copy()
         slot_data.update(to_fill_with)
         [loaded] = self._loader.load()
-        loaded = loaded.clone()
+        loaded = loaded.clone()  # type: ignore[union-attr]
         return PlatedElement(
             slot_data=slot_data,
             preloaded=loaded,
             renderers=self._renderers,
             boundInstance=instance,
             presentationSlots=self._presentationSlots,
         )
 
-    @attr.s
-    class _Widget(object):
+    @attr.s(auto_attribs=True)
+    class _Widget:
         """
         Implementation of L{Plating.widgeted}.  This is a L{callable}
         descriptor that records the instance to which its wrapped
         function is bound, if any.  Its L{widget} method then passes
         that instance or L{None} and the result of invoking the
         function (or now bound method) to the creating L{Plating}
         instance's L{Plating._elementify} to construct a
         L{PlatedElement}.
         """
 
-        _plating = attr.ib(type="Plating")
-        _function = attr.ib(type=Callable[..., Any])
-        _instance = attr.ib(type=object)
+        _plating: "Plating"
+        _function: Callable[..., Any]
+        _instance: object
 
         def __call__(self, *args, **kwargs):
             return self._function(*args, **kwargs)
 
         def __get__(self, instance, owner=None):
             return self.__class__(
                 self._plating,
-                self._function.__get__(instance, owner),
+                self._function.__get__(  # type: ignore[attr-defined]
+                    instance, owner
+                ),
                 instance=instance,
             )
 
         def widget(self, *args, **kwargs):
             """
             Construct a L{PlatedElement} the rendering of this widget.
             """
```

### Comparing `klein-20.6.0/src/klein/_request.py` & `klein-21.8.0/src/klein/_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 # -*- test-case-name: klein.test.test_request -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 HTTP request API.
 """
 
-from typing import Text, Union
+from typing import Union
 
 from attr import Factory, attrib, attrs
 from attr.validators import instance_of, provides
-
 from hyperlink import DecodedURL
-
 from tubes.itube import IFount
-
-from twisted.internet.defer import Deferred
-
 from zope.interface import implementer
 
-from ._interfaces import IHTTPHeaders, IHTTPRequest
+from ._imessage import IHTTPHeaders, IHTTPRequest
 from ._message import MessageState, bodyAsBytes, bodyAsFount, validateBody
 
 
 __all__ = ()
 
 
 @implementer(IHTTPRequest)
 @attrs(frozen=True)
-class FrozenHTTPRequest(object):
+class FrozenHTTPRequest:
     """
     Immutable HTTP request.
     """
 
-    method = attrib(validator=instance_of(Text))  # type: Text
-    uri = attrib(validator=instance_of(DecodedURL))  # type: DecodedURL
-    headers = attrib(validator=provides(IHTTPHeaders))  # type: IHTTPHeaders
-
-    _body = attrib(validator=validateBody)  # type: Union[bytes, IFount]
-
-    _state = attrib(
-        default=Factory(MessageState), init=False
-    )  # type: MessageState
+    method: str = attrib(validator=instance_of(str))
+    uri: DecodedURL = attrib(validator=instance_of(DecodedURL))
+    headers: IHTTPHeaders = attrib(validator=provides(IHTTPHeaders))
+
+    _body: Union[bytes, IFount] = attrib(validator=validateBody)
+
+    _state: MessageState = attrib(default=Factory(MessageState), init=False)
 
-    def bodyAsFount(self):
-        # type: () -> IFount
+    def bodyAsFount(self) -> IFount:
         return bodyAsFount(self._body, self._state)
 
-    def bodyAsBytes(self):
-        # type: () -> Deferred[bytes]
-        return bodyAsBytes(self._body, self._state)
+    async def bodyAsBytes(self) -> bytes:
+        return await bodyAsBytes(self._body, self._state)
```

### Comparing `klein-20.6.0/src/klein/_request_compat.py` & `klein-21.8.0/src/klein/_request_compat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # -*- test-case-name: klein.test.test_irequest -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Support for interoperability with L{twisted.web.iweb.IRequest}.
 """
 
 from io import BytesIO
-from typing import Text
+from typing import cast
 
 from attr import Factory, attrib, attrs
 from attr.validators import provides
-
 from hyperlink import DecodedURL
-
 from tubes.itube import IFount
+from zope.interface import implementer
 
-from twisted.internet.defer import Deferred, succeed
 from twisted.python.compat import nativeString
 from twisted.web.iweb import IRequest
 
-from zope.interface import implementer
-
 from ._headers import IHTTPHeaders
 from ._headers_compat import HTTPHeadersWrappingHeaders
 from ._message import FountAlreadyAccessedError, MessageState
 from ._request import IHTTPRequest
 from ._tubes import IOFount, fountToBytes
 
 
@@ -32,84 +28,71 @@
 
 
 noneIO = BytesIO()
 
 
 @implementer(IHTTPRequest)
 @attrs(frozen=True)
-class HTTPRequestWrappingIRequest(object):
+class HTTPRequestWrappingIRequest:
     """
     HTTP request.
 
     This is an L{IHTTPRequest} implementation that wraps an L{IRequest} object.
     """
 
-    _request = attrib(validator=provides(IRequest))  # type: IRequest
+    _request: IRequest = attrib(validator=provides(IRequest))
 
-    _state = attrib(
-        default=Factory(MessageState), init=False
-    )  # type: MessageState
+    _state: MessageState = attrib(default=Factory(MessageState), init=False)
 
     @property
-    def method(self):
-        # type: () -> Text
-        return self._request.method.decode("ascii")
+    def method(self) -> str:
+        return cast(str, self._request.method.decode("ascii"))
 
     @property
-    def uri(self):
-        # type: () -> DecodedURL
+    def uri(self) -> DecodedURL:
         request = self._request
 
         # This code borrows from t.w.server.Request._prePathURL.
 
         if request.isSecure():
-            scheme = u"https"
+            scheme = "https"
         else:
-            scheme = u"http"
+            scheme = "http"
 
         netloc = nativeString(request.getRequestHostname())
 
         port = request.getHost().port
         if request.isSecure():
             default = 443
         else:
             default = 80
         if port != default:
-            netloc += u":{}".format(port)
+            netloc += f":{port}"
 
         path = nativeString(request.uri)
-        if path and path[0] == u"/":
+        if path and path[0] == "/":
             path = path[1:]
 
-        return DecodedURL.fromText(u"{}://{}/{}".format(scheme, netloc, path))
+        return DecodedURL.fromText(f"{scheme}://{netloc}/{path}")
 
     @property
-    def headers(self):
-        # type: () -> IHTTPHeaders
+    def headers(self) -> IHTTPHeaders:
         return HTTPHeadersWrappingHeaders(headers=self._request.requestHeaders)
 
-    def bodyAsFount(self):
-        # type: () -> IFount
+    def bodyAsFount(self) -> IFount:
         source = self._request.content
         if source is noneIO:
             raise FountAlreadyAccessedError()
 
         fount = IOFount(source=source)
 
         self._request.content = noneIO
 
         return fount
 
-    def bodyAsBytes(self):
-        # type: () -> Deferred[bytes]
+    async def bodyAsBytes(self) -> bytes:
         if self._state.cachedBody is not None:
-            return succeed(self._state.cachedBody)
-
-        def cache(bodyBytes):
-            # type: (bytes) -> bytes
-            self._state.cachedBody = bodyBytes
-            return bodyBytes
+            return self._state.cachedBody  # pragma: no cover
 
         fount = self.bodyAsFount()
-        d = fountToBytes(fount)
-        d.addCallback(cache)
-        return d
+        self._state.cachedBody = await fountToBytes(fount)
+        return self._state.cachedBody
```

### Comparing `klein-20.6.0/src/klein/_requirer.py` & `klein-21.8.0/src/klein/_requirer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-from typing import Any, Callable, List, TYPE_CHECKING
+from typing import Any, Callable, Dict, Generator, List, Sequence, Type
 
 import attr
+from zope.interface import Interface, implementer
 
-from twisted.internet.defer import inlineCallbacks, returnValue
+from twisted.internet.defer import inlineCallbacks
 from twisted.python.components import Componentized
-
-from zope.interface import implementer
+from twisted.web.iweb import IRequest
 
 from ._app import _call
 from ._decorators import bindable, modified
-from .interfaces import EarlyExit, IRequestLifecycle
-
-if TYPE_CHECKING:  # pragma: no cover
-    from typing import Dict, Sequence
-    from twisted.web.iweb import IRequest
-    from twisted.internet.defer import Deferred
-    from zope.interface.interfaces import IInterface
-    from .interfaces import IDependencyInjector, IRequiredParameter
+from .interfaces import (
+    EarlyExit,
+    IDependencyInjector,
+    IRequestLifecycle,
+    IRequiredParameter,
+)
 
 
 @implementer(IRequestLifecycle)
-@attr.s
-class RequestLifecycle(object):
+@attr.s(auto_attribs=True)
+class RequestLifecycle:
     """
     Mechanism to run hooks at the start of a request managed by a L{Requirer}.
     """
 
-    _prepareHooks = attr.ib(type=List, default=attr.Factory(list))
-
-    def addPrepareHook(self, beforeHook, requires=(), provides=()):
-        # type: (Callable, Sequence[IInterface], Sequence[IInterface]) -> None
-        """
-        Add a hook that promises to prepare the request by supplying the given
-        interfaces as components on the request, and requires the given
-        requirements.
+    _prepareHooks: List = attr.ib(factory=list)
 
-        Prepare hooks are run I{before any} L{IDependencyInjector}s I{inject
-        their values}.
-        """
+    def addPrepareHook(
+        self,
+        beforeHook: Callable,
+        requires: Sequence[Type[Interface]] = (),
+        provides: Sequence[Type[Interface]] = (),
+    ) -> None:
         # TODO: topological requirements sort
         self._prepareHooks.append(beforeHook)
 
     @inlineCallbacks
-    def runPrepareHooks(self, instance, request):
-        # type: (Any, IRequest) -> Deferred
+    def runPrepareHooks(
+        self, instance: Any, request: IRequest
+    ) -> Generator[Any, object, None]:
         """
         Execute all the hooks added with L{RequestLifecycle.addPrepareHook}.
         This is invoked by the L{requires} route machinery.
 
         @param instance: The instance bound to the Klein route.
 
         @param request: The IRequest being processed.
@@ -58,30 +53,27 @@
 
 _routeDecorator = Any  # a decorator like @route
 _routeT = Any  # a thing decorated by a decorator like @route
 
 _prerequisiteCallback = Callable[[IRequestLifecycle], None]
 
 
-@attr.s
-class Requirer(object):
+@attr.s(auto_attribs=True)
+class Requirer:
     """
     Dependency injection for required parameters.
     """
 
-    _prerequisites = attr.ib(
-        type=List[_prerequisiteCallback], default=attr.Factory(list)
-    )
+    _prerequisites: List[_prerequisiteCallback] = attr.ib(factory=list)
 
     def prerequisite(
         self,
-        providesComponents,  # type: Sequence[IInterface]
-        requiresComponents=(),  # type: Sequence[IInterface]
-    ):
-        # type: (...) -> Callable[[Callable], Callable]
+        providesComponents: Sequence[Type[Interface]],
+        requiresComponents: Sequence[Type[Interface]] = (),
+    ) -> Callable[[Callable], Callable]:
         """
         Specify a component that is a pre-requisite of every request routed
         through this requirer's C{require} method.  Used like so::
 
             requirer = Requirer()
 
             @requirer.prerequisite([IFoo])
@@ -91,42 +83,40 @@
 
         @note: C{requiresComponents} is, at this point, for the reader's
             interest only, the framework will not topologically sort
             dependencies; you must presently register prerequisites in the
             order you want them to be called.
         """
 
-        def decorator(prerequisiteMethod):
-            # type: (Callable) -> Callable
-            def oneHook(lifecycle):
-                # type: (IRequestLifecycle) -> None
+        def decorator(prerequisiteMethod: Callable) -> Callable:
+            def oneHook(lifecycle: IRequestLifecycle) -> None:
                 lifecycle.addPrepareHook(
                     prerequisiteMethod,
                     requires=requiresComponents,
                     provides=providesComponents,
                 )
 
             self._prerequisites.append(oneHook)
             return prerequisiteMethod
 
         return decorator
 
-    def require(self, routeDecorator, **requiredParameters):
-        # type: (_routeT, **IRequiredParameter) -> _routeDecorator
+    def require(
+        self, routeDecorator: _routeT, **requiredParameters: IRequiredParameter
+    ) -> _routeDecorator:
         """
         Inject the given dependencies while running the given route.
         """
 
-        def decorator(functionWithRequirements):
-            # type: (Callable) -> Callable
+        def decorator(functionWithRequirements: Callable) -> Callable:
             injectionComponents = Componentized()
             lifecycle = RequestLifecycle()
             injectionComponents.setComponent(IRequestLifecycle, lifecycle)
 
-            injectors = {}  # type: Dict[str, IDependencyInjector]
+            injectors: Dict[str, IDependencyInjector] = {}
 
             for parameterName, required in requiredParameters.items():
                 injectors[parameterName] = required.registerInjector(
                     injectionComponents, parameterName, lifecycle
                 )
 
             for prereq in self._prerequisites:
@@ -134,30 +124,31 @@
 
             for v in injectors.values():
                 v.finalize()
 
             @modified("dependency-injecting route", functionWithRequirements)
             @bindable
             @inlineCallbacks
-            def router(instance, request, *args, **routeParams):
-                # type: (Any, IRequest, *Any, **Any) -> Any
+            def router(
+                instance: Any, request: IRequest, *args: Any, **routeParams: Any
+            ) -> Any:
                 injected = routeParams.copy()
                 try:
                     yield lifecycle.runPrepareHooks(instance, request)
                     for (k, injector) in injectors.items():
                         injected[k] = yield injector.injectValue(
                             instance, request, routeParams
                         )
                 except EarlyExit as ee:
                     result = ee.alternateReturnValue
                 else:
                     result = yield _call(
                         instance, functionWithRequirements, *args, **injected
                     )
-                returnValue(result)
+                return result
 
             fWR, iC = functionWithRequirements, injectionComponents
             fWR.injectionComponents = iC  # type: ignore[attr-defined]
             routeDecorator(router)
             return functionWithRequirements
 
         return decorator
```

### Comparing `klein-20.6.0/src/klein/_resource.py` & `klein-21.8.0/src/klein/_resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,96 @@
 # -*- test-case-name: klein.test.test_resource -*-
 
-from __future__ import absolute_import, division
+from typing import TYPE_CHECKING, Any, Optional, Sequence, Tuple, Union, cast
+
+from werkzeug.exceptions import HTTPException
 
 from twisted.internet import defer
-from twisted.python import failure, log
-from twisted.python.compat import intToBytes, unicode
+from twisted.internet.defer import Deferred, maybeDeferred
+from twisted.python import log
+from twisted.python.failure import Failure
 from twisted.web import server
-from twisted.web.iweb import IRenderable
+from twisted.web.iweb import IRenderable, IRequest
 from twisted.web.resource import IResource, Resource, getChildForRequest
 from twisted.web.server import NOT_DONE_YET
 from twisted.web.template import renderElement
 
-from werkzeug.exceptions import HTTPException
-
 from ._dihttp import Response
 from ._interfaces import IKleinRequest
 
 
-def ensure_utf8_bytes(v):
+if TYPE_CHECKING:
+    from ._app import ErrorHandlers, Klein, KleinRenderable
+
+
+def ensure_utf8_bytes(v: Union[str, bytes]) -> bytes:
     """
-    Coerces a value which is either a C{unicode} or C{str} to a C{str}.
-    If ``v`` is a C{unicode} object it is encoded as utf-8.
+    Coerces a value which is either a C{str} or C{bytes} to a C{bytes}.
+    If ``v`` is a C{str} object it is encoded as utf-8.
     """
-    if isinstance(v, unicode):
+    if isinstance(v, str):
         v = v.encode("utf-8")
     return v
 
 
-class _StandInResource(object):
+class _StandInResource:
     """
     A standin for a Resource.
 
     This is a sentinel value for L{KleinResource}, to say that we are rendering
     a L{Resource}, which may close the connection itself later.
     """
 
 
-class _URLDecodeError(Exception):
+StandInResource = cast("KleinResource", _StandInResource())
+
+
+class URLDecodeError(Exception):
     """
     Raised if one or more string parts of the URL could not be decoded.
     """
 
     __slots__ = ["errors"]
 
-    def __init__(self, errors):
+    def __init__(self, errors: Sequence[Tuple[str, Failure]]) -> None:
         """
-        @param errors: List of decoding errors.
-        @type errors: L{list} of L{tuple} of L{str},
-            L{twisted.python.failure.Failure}
+        @param errors: Sequence of decoding errors, expressed as tuples
+            of names and an associated failure.
         """
         self.errors = errors
 
-    def __repr__(self):
-        return "<URLDecodeError(errors={0!r})>".format(self.errors)
+    def __repr__(self) -> str:
+        return f"<URLDecodeError(errors={self.errors!r})>"
 
 
-def _extractURLparts(request):
+def extractURLparts(request: IRequest) -> Tuple[str, str, int, str, str]:
     """
     Extracts and decodes URI parts from C{request}.
 
     All strings must be UTF8-decodable.
 
     @param request: A Twisted Web request.
-    @type request: L{twisted.web.iweb.IRequest}
 
     @raise URLDecodeError: If one of the parts could not be decoded as UTF-8.
 
     @return: L{tuple} of the URL scheme, the server name, the server port, the
         path info and the script name.
-    @rtype: L{tuple} of L{unicode}, L{unicode}, L{int}, L{unicode}, L{unicode}
     """
     server_name = request.getRequestHostname()
     if hasattr(request.getHost(), "port"):
         server_port = request.getHost().port
     else:
         server_port = 0
     if (bool(request.isSecure()), server_port) not in [
         (True, 443),
         (False, 80),
         (False, 0),
         (True, 0),
     ]:
-        server_name = server_name + b":" + intToBytes(server_port)
+        server_name = b"%s:%d" % (server_name, server_port)
 
     script_name = b""
     if request.prepath:
         script_name = b"/".join(request.prepath)
 
         if not script_name.startswith(b"/"):
             script_name = b"/" + script_name
@@ -93,71 +98,71 @@
     path_info = b""
     if request.postpath:
         path_info = b"/".join(request.postpath)
 
         if not path_info.startswith(b"/"):
             path_info = b"/" + path_info
 
-    url_scheme = u"https" if request.isSecure() else u"http"
+    url_scheme = "https" if request.isSecure() else "http"
 
     utf8Failures = []
     try:
         server_name = server_name.decode("utf-8")
     except UnicodeDecodeError:
-        utf8Failures.append(("SERVER_NAME", failure.Failure()))
+        utf8Failures.append(("SERVER_NAME", Failure()))
     try:
-        path_info = path_info.decode("utf-8")
+        path_text = path_info.decode("utf-8")
     except UnicodeDecodeError:
-        utf8Failures.append(("PATH_INFO", failure.Failure()))
+        utf8Failures.append(("PATH_INFO", Failure()))
     try:
-        script_name = script_name.decode("utf-8")
+        script_text = script_name.decode("utf-8")
     except UnicodeDecodeError:
-        utf8Failures.append(("SCRIPT_NAME", failure.Failure()))
+        utf8Failures.append(("SCRIPT_NAME", Failure()))
 
     if utf8Failures:
-        raise _URLDecodeError(utf8Failures)
+        raise URLDecodeError(utf8Failures)
 
-    return url_scheme, server_name, server_port, path_info, script_name
+    return url_scheme, server_name, server_port, path_text, script_text
 
 
 class KleinResource(Resource):
     """
     A ``Resource`` that can do URL routing.
     """
 
     isLeaf = True
 
-    def __init__(self, app):
+    def __init__(self, app: "Klein") -> None:
         Resource.__init__(self)
         self._app = app
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         if isinstance(other, KleinResource):
             return vars(self) == vars(other)
         return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         result = self.__eq__(other)
         if result is NotImplemented:
             return result
         return not result
 
-    def render(self, request):
+    def render(self, request: IRequest) -> "KleinRenderable":
         # Stuff we need to know for the mapper.
         try:
             (
                 url_scheme,
                 server_name,
                 server_port,
                 path_info,
                 script_name,
-            ) = _extractURLparts(request)
-        except _URLDecodeError as e:
+            ) = extractURLparts(request)
+        except URLDecodeError as e:
             for what, fail in e.errors:
-                log.err(fail, "Invalid encoding in {what}.".format(what=what))
+                log.err(fail, f"Invalid encoding in {what}.")
             request.setResponseCode(400)
             return b"Non-UTF-8 encoding in URL."
 
         # Bind our mapper.
         mapper = self._app.url_map.bind(
             server_name,
             script_name,
@@ -168,122 +173,140 @@
         # Make the mapper available to the view.
         kleinRequest = IKleinRequest(request)
         kleinRequest.mapper = mapper
 
         # Make sure we'll notice when the connection goes away unambiguously.
         request_finished = [False]
 
-        def _finish(result):
+        def _finish(result: object) -> None:
             request_finished[0] = True
 
-        def _execute():
+        def _execute() -> Deferred:
             # Actually doing the match right here. This can cause an exception
             # to percolate up. If that happens it will be handled below in
             # processing_failed, either by a user-registered error handler or
             # one of our defaults.
             (rule, kwargs) = mapper.match(return_rule=True)
             endpoint = rule.endpoint
 
             # Try pretty hard to fix up prepath and postpath.
-            segment_count = self._app.endpoints[endpoint].segment_count
+            segment_count = self._app.endpoints[
+                endpoint
+            ].segment_count  # type: ignore[union-attr]
             request.prepath.extend(request.postpath[:segment_count])
             request.postpath = request.postpath[segment_count:]
 
-            request.notifyFinish().addBoth(_finish)
+            request.notifyFinish().addBoth(  # type: ignore[attr-defined]
+                _finish,
+            )
 
             # Standard Twisted Web stuff. Defer the method action, giving us
             # something renderable or printable. Return NOT_DONE_YET and set up
             # the incremental renderer.
-            d = defer.maybeDeferred(
+            d = maybeDeferred(
                 self._app.execute_endpoint, endpoint, request, **kwargs
             )
 
-            request.notifyFinish().addErrback(lambda _: d.cancel())
+            request.notifyFinish().addErrback(  # type: ignore[attr-defined]
+                lambda _: d.cancel(),
+            )
 
             return d
 
-        d = defer.maybeDeferred(_execute)
+        d = maybeDeferred(_execute)
 
-        def process(r):
+        # typing note: returns Any because Response._applyToRequest returns Any
+        def process(r: object) -> Any:
             """
             Recursively go through r and any child Resources until something
             returns an IRenderable, then render it and let the result of that
             bubble back up.
             """
             if isinstance(r, Response):
                 r = r._applyToRequest(request)
 
             if IResource.providedBy(r):
-                request.render(getChildForRequest(r, request))
-                return _StandInResource
+                request.render(  # type: ignore[attr-defined]
+                    getChildForRequest(r, request)
+                )
+                return StandInResource
 
             if IRenderable.providedBy(r):
                 renderElement(request, r)
-                return _StandInResource
+                return StandInResource
 
             return r
 
         d.addCallback(process)
 
-        def processing_failed(failure, error_handlers):
+        def processing_failed(
+            failure: Failure, error_handlers: "ErrorHandlers"
+        ) -> Optional[Deferred]:
             # The failure processor writes to the request.  If the
             # request is already finished we should suppress failure
             # processing.  We don't return failure here because there
             # is no way to surface this failure to the user if the
             # request is finished.
             if request_finished[0]:
                 if not failure.check(defer.CancelledError):
                     log.err(failure, "Unhandled Error Processing Request.")
-                return
+                return None
 
             # If there are no more registered handlers, apply some defaults
             if len(error_handlers) == 0:
                 if failure.check(HTTPException):
                     he = failure.value
+                    assert isinstance(he, HTTPException)
                     request.setResponseCode(he.code)
                     resp = he.get_response({})
 
                     for header, value in resp.headers:
                         request.setHeader(
                             ensure_utf8_bytes(header), ensure_utf8_bytes(value)
                         )
 
-                    return ensure_utf8_bytes(b"".join(resp.iter_encoded()))
+                    return ensure_utf8_bytes(
+                        b"".join(
+                            resp.iter_encoded(),  # type: ignore[attr-defined]
+                        ),
+                    )  # type: ignore[attr-defined, return-value]
                 else:
-                    request.processingFailed(failure)
-                    return
+                    request.processingFailed(  # type: ignore[attr-defined]
+                        failure,
+                    )
+                    return None
 
             error_handler = error_handlers[0]
 
             # Each error handler is a tuple of
             # (list_of_exception_types, handler_fn)
             if failure.check(*error_handler[0]):
-                d = defer.maybeDeferred(
+                d = maybeDeferred(
                     self._app.execute_error_handler,
                     error_handler[1],
                     request,
                     failure,
                 )
 
                 d.addCallback(process)
 
                 return d.addErrback(processing_failed, error_handlers[1:])
 
             return processing_failed(failure, error_handlers[1:])
 
         d.addErrback(processing_failed, self._app._error_handlers)
 
-        def write_response(r):
-            if r is not _StandInResource:
-                if isinstance(r, unicode):
+        def write_response(r: object) -> None:
+            if r is not StandInResource:
+                if isinstance(r, str):
                     r = r.encode("utf-8")
 
                 if (r is not None) and (r != NOT_DONE_YET):
                     request.write(r)
 
                 if not request_finished[0]:
                     request.finish()
 
         d.addCallback(write_response)
         d.addErrback(log.err, _why="Unhandled Error writing response")
 
-        return server.NOT_DONE_YET
+        return server.NOT_DONE_YET  # type: ignore[return-value]
```

### Comparing `klein-20.6.0/src/klein/_response.py` & `klein-21.8.0/src/klein/_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,41 @@
 # -*- test-case-name: klein.test.test_response -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 HTTP response API.
 """
 
 from typing import Union
 
 from attr import Factory, attrib, attrs
 from attr.validators import instance_of, provides
-
 from tubes.itube import IFount
-
-from twisted.internet.defer import Deferred
-
 from zope.interface import implementer
 
-from ._interfaces import IHTTPHeaders, IHTTPResponse
+from ._imessage import IHTTPHeaders, IHTTPResponse
 from ._message import MessageState, bodyAsBytes, bodyAsFount, validateBody
 
 
 __all__ = ()
 
 
 @implementer(IHTTPResponse)
 @attrs(frozen=True)
-class FrozenHTTPResponse(object):
+class FrozenHTTPResponse:
     """
     Immutable HTTP response.
     """
 
-    status = attrib(validator=instance_of(int))  # type: int
+    status: int = attrib(validator=instance_of(int))
 
-    headers = attrib(validator=provides(IHTTPHeaders))  # type: IHTTPHeaders
+    headers: IHTTPHeaders = attrib(validator=provides(IHTTPHeaders))
 
-    _body = attrib(validator=validateBody)  # type: Union[bytes, IFount]
+    _body: Union[bytes, IFount] = attrib(validator=validateBody)
 
-    _state = attrib(
-        default=Factory(MessageState), init=False
-    )  # type: MessageState
+    _state: MessageState = attrib(default=Factory(MessageState), init=False)
 
-    def bodyAsFount(self):
-        # type: () -> IFount
+    def bodyAsFount(self) -> IFount:
         return bodyAsFount(self._body, self._state)
 
-    def bodyAsBytes(self):
-        # type: () -> Deferred[bytes]
-        return bodyAsBytes(self._body, self._state)
+    async def bodyAsBytes(self) -> bytes:
+        return await bodyAsBytes(self._body, self._state)
```

### Comparing `klein-20.6.0/src/klein/_session.py` & `klein-21.8.0/src/klein/_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # -*- test-case-name: klein.test.test_session -*-
 
-from typing import Any, Callable, Dict, Optional, Sequence, Text, Union
+from typing import Any, Callable, Dict, Optional, Sequence, Type, Union, cast
 
 import attr
+from zope.interface import Interface, implementer
 
-from twisted.internet.defer import inlineCallbacks, returnValue
+from twisted.internet.defer import inlineCallbacks
 from twisted.python.components import Componentized
 from twisted.python.reflect import qual
 from twisted.web.http import UNAUTHORIZED
 from twisted.web.iweb import IRequest
 from twisted.web.resource import Resource
 
-from zope.interface import implementer
-from zope.interface.interfaces import IInterface
-
-from ._typing import Arg, KwArg
 from .interfaces import (
     EarlyExit,
     IDependencyInjector,
     IRequestLifecycle,
     IRequiredParameter,
     ISession,
     ISessionProcurer,
@@ -26,108 +23,92 @@
     NoSuchSession,
     SessionMechanism,
     TooLateForCookies,
 )
 
 
 @implementer(ISessionProcurer)
-@attr.s
-class SessionProcurer(object):
+@attr.s(auto_attribs=True)
+class SessionProcurer:
     """
     A L{SessionProcurer} procures a session from a request and a store.
 
     @ivar _store: The session store to procure a session from.
-    @type _store: L{klein.interfaces.ISessionStore}
-
     @ivar _maxAge: The maximum age (in seconds) of the session cookie.
-    @type _maxAge: L{int}
-
     @ivar _secureCookie: The name of the cookie to use for sessions protected
         with TLS (i.e. HTTPS).
-    @type _secureCookie: L{bytes}
-
     @ivar _insecureCookie: The name of the cookie to use for sessions I{not}
         protected with TLS (i.e. HTTP).
-    @type _insecureCookie: L{bytes}
-
     @ivar _cookieDomain: If set, the domain name to restrict the session cookie
         to.
-    @type _cookieDomain: L{None} or L{bytes}
-
     @ivar _cookiePath: If set, the URL path to restrict the session cookie to.
-    @type _cookiePath: L{bytes}
-
     @ivar _secureTokenHeader: The name of the HTTPS header to try to extract a
         session token from; API clients should use this header, rather than a
         cookie.
-    @type _secureTokenHeader: L{bytes}
-
     @ivar _insecureTokenHeader: The name of the HTTP header to try to extract a
         session token from; API clients should use this header, rather than a
         cookie.
-    @type _insecureTokenHeader: L{bytes}
-
     @ivar _setCookieOnGET: Automatically request that the session store create
         a session if one is not already associated with the request and the
         request is a GET.
-    @type _setCookieOnGET: L{bool}
     """
 
-    _store = attr.ib(type=ISessionStore)
+    _store: ISessionStore
 
-    _maxAge = attr.ib(type=int, default=3600)
-    _secureCookie = attr.ib(type=bytes, default=b"Klein-Secure-Session")
-    _insecureCookie = attr.ib(type=bytes, default=b"Klein-INSECURE-Session")
-    _cookieDomain = attr.ib(type=Optional[bytes], default=None)
-    _cookiePath = attr.ib(type=bytes, default=b"/")
-
-    _secureTokenHeader = attr.ib(type=bytes, default=b"X-Auth-Token")
-    _insecureTokenHeader = attr.ib(type=bytes, default=b"X-INSECURE-Auth-Token")
-    _setCookieOnGET = attr.ib(type=bool, default=True)
+    _maxAge: int = 3600
+    _secureCookie: bytes = b"Klein-Secure-Session"
+    _insecureCookie: bytes = b"Klein-INSECURE-Session"
+    _cookieDomain: Optional[bytes] = None
+    _cookiePath: bytes = b"/"
+
+    _secureTokenHeader: bytes = b"X-Auth-Token"
+    _insecureTokenHeader: bytes = b"X-INSECURE-Auth-Token"
+    _setCookieOnGET: bool = True
 
     @inlineCallbacks
-    def procureSession(self, request, forceInsecure=False):
-        # type: (IRequest, bool) -> Any
-        alreadyProcured = request.getComponent(ISession)
+    def procureSession(
+        self, request: IRequest, forceInsecure: bool = False
+    ) -> Any:
+        alreadyProcured = cast(Componentized, request).getComponent(ISession)
         if alreadyProcured is not None:
             if not forceInsecure or not request.isSecure():
-                returnValue(alreadyProcured)
+                return alreadyProcured
 
         if request.isSecure():
             if forceInsecure:
                 tokenHeader = self._insecureTokenHeader
-                cookieName = self._insecureCookie  # type: Union[Text, bytes]
+                cookieName: Union[str, bytes] = self._insecureCookie
                 sentSecurely = False
             else:
                 tokenHeader = self._secureTokenHeader
                 cookieName = self._secureCookie
                 sentSecurely = True
         else:
             # Have we inadvertently disclosed a secure token over an insecure
             # transport, for example, due to a buggy client?
-            allPossibleSentTokens = sum(
-                [
+            allPossibleSentTokens: Sequence[str] = sum(
+                (
                     request.requestHeaders.getRawHeaders(header, [])
                     for header in [
                         self._secureTokenHeader,
                         self._insecureTokenHeader,
                     ]
-                ],
+                ),
                 [],
             ) + [
                 it
                 for it in [
                     request.getCookie(cookie)
                     for cookie in [self._secureCookie, self._insecureCookie]
                 ]
                 if it
-            ]  # type: Sequence[Text]
+            ]
             # Does it seem like this check is expensive? It sure is! Don't want
             # to do it? Turn on your dang HTTPS!
-            yield self._store.sentInsecurely(allPossibleSentTokens)
+            self._store.sentInsecurely(allPossibleSentTokens)
             tokenHeader = self._insecureTokenHeader
             cookieName = self._insecureCookie
             sentSecurely = False
             # Fun future feature: honeypot that does this over HTTPS, but sets
             # isSecure() to return false because it serves up a cert for the
             # wrong hostname or an invalid cert, to keep API clients honest
             # about chain validation.
@@ -148,94 +129,78 @@
                 if mechanism == SessionMechanism.Header:
                     raise
                 session = None
         if mechanism == SessionMechanism.Cookie and (
             session is None or session.identifier != sentCookie
         ):
             if session is None:
-                if request.startedWriting:
+                if request.startedWriting:  # type: ignore[attr-defined]
                     # At this point, if the mechanism is Header, we either have
                     # a valid session or we bailed after NoSuchSession above.
                     raise TooLateForCookies(
                         "You tried initializing a cookie-based session too"
                         " late in the request pipeline; the headers"
                         " were already sent."
                     )
                 if request.method != b"GET":
                     # Sessions should only ever be auto-created by GET
                     # requests; there's no way that any meaningful data
                     # manipulation could succeed (no CSRF token check could
                     # ever succeed, for example).
                     raise NoSuchSession(
-                        u"Can't initialize a session on a "
-                        u"{method} request.".format(
+                        "Can't initialize a session on a "
+                        "{method} request.".format(
                             method=request.method.decode("ascii")
                         )
                     )
                 if not self._setCookieOnGET:
                     # We don't have a session ID at all, and we're not allowed
                     # by policy to set a cookie on the client.
                     raise NoSuchSession(
-                        u"Cannot auto-initialize a session for this request."
+                        "Cannot auto-initialize a session for this request."
                     )
                 session = yield self._store.newSession(sentSecurely, mechanism)
             identifierInCookie = session.identifier
             if not isinstance(identifierInCookie, str):
                 identifierInCookie = identifierInCookie.encode("ascii")
             if not isinstance(cookieName, str):
                 cookieName = cookieName.decode("ascii")
-            request.addCookie(
+            request.addCookie(  # type: ignore[call-arg]
                 cookieName,
                 identifierInCookie,
                 max_age=str(self._maxAge),
                 domain=self._cookieDomain,
                 path=self._cookiePath,
                 secure=sentSecurely,
                 httpOnly=True,
             )
         if sentSecurely or not request.isSecure():
             # Do not cache the insecure session on the secure request, thanks.
-            request.setComponent(ISession, session)
-        returnValue(session)
+            cast(Componentized, request).setComponent(ISession, session)
+        return session
 
 
-_procureProcurerType = Union[
-    Callable[[Any], ISessionProcurer], Callable[[], ISessionProcurer]
-]
-
-_kleinRenderable = Any
-_routeCallable = Any
-_kleinCallable = Callable[..., _kleinRenderable]
-_kleinDecorator = Callable[[_kleinCallable], _kleinCallable]
-_requirerResult = Callable[
-    [Arg(_routeCallable, "route"), KwArg(Any)],
-    Callable[[_kleinCallable], _kleinCallable],
-]
-
-
-class AuthorizationDenied(Resource, object):
-    def __init__(self, interface, instance):
-        # type: (IInterface, Any) -> None
+class AuthorizationDenied(Resource):
+    def __init__(self, interface: Type[Interface], instance: Any) -> None:
         self._interface = interface
-        super(AuthorizationDenied, self).__init__()
+        super().__init__()
 
-    def render(self, request):
-        # type: (IRequest) -> bytes
+    def render(self, request: IRequest) -> bytes:
         request.setResponseCode(UNAUTHORIZED)
-        return "{} DENIED".format(qual(self._interface)).encode("utf-8")
+        return f"{qual(self._interface)} DENIED".encode()
 
 
 @implementer(IDependencyInjector, IRequiredParameter)
-@attr.s
-class Authorization(object):
+@attr.s(auto_attribs=True)
+class Authorization:
     """
     Declare that a C{require}-decorated function requires a certain interface
     be authorized from the session.
 
-    This is a dependnecy injector used in conjunction with a L{klein.Requirer},
+    This is a dependency injector used in conjunction with a L{klein.Requirer},
     like so::
 
         from klein import Requirer, SesssionProcurer
         from klein.interfaces import ISession
 
         from myapp import ISuperDuperAdmin
 
@@ -275,43 +240,45 @@
 
     @ivar _whenDenied: when this authorization is denied, what object - usually
         an IResource - should be returned to the route decorator that was
         passed to L{Requirer.require}?  Note that this will never be used if
         C{required} is set to C{False}.
     """
 
-    _interface = attr.ib(type=IInterface)
-    _required = attr.ib(type=bool, default=True)
-    _whenDenied = attr.ib(
-        type=Callable[[IInterface, Any], Any], default=AuthorizationDenied
-    )
-
-    def registerInjector(self, injectionComponents, parameterName, lifecycle):
-        # type: (Componentized, str, IRequestLifecycle) -> IDependencyInjector
+    _interface: Type[Interface]
+    _required: bool = True
+    _whenDenied: Callable[[Type[Interface], Any], Any] = AuthorizationDenied
+
+    def registerInjector(
+        self,
+        injectionComponents: Componentized,
+        parameterName: str,
+        lifecycle: IRequestLifecycle,
+    ) -> IDependencyInjector:
         """
         Register this authorization to inject a parameter.
         """
         return self
 
     @inlineCallbacks
-    def injectValue(self, instance, request, routeParams):
-        # type: (Any, IRequest, Dict[str, Any]) -> Any
+    def injectValue(
+        self, instance: Any, request: IRequest, routeParams: Dict[str, Any]
+    ) -> Any:
         """
         Inject a value by asking the request's session.
         """
         # TODO: this could be optimized to do fewer calls to 'authorize' by
         # collecting all the interfaces that are necessary and then using
         # addBeforeHook; the interface would not need to change.
-        session = ISession(request)  # type: ignore[operator]
+        session = ISession(request)
         provider = (yield session.authorize([self._interface])).get(
             self._interface
         )
         if self._required and provider is None:
             raise EarlyExit(self._whenDenied(self._interface, instance))
         # TODO: CSRF protection should probably go here
-        returnValue(provider)
+        return provider
 
-    def finalize(self):
-        # type: () -> None
+    def finalize(self) -> None:
         """
         Nothing to finalize when registering.
         """
```

### Comparing `klein-20.6.0/src/klein/_tubes.py` & `klein-21.8.0/src/klein/_tubes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,77 @@
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Extensions to Tubes.
 """
 
 from io import BytesIO
-from typing import BinaryIO, Iterable
+from typing import Any, BinaryIO
 
 from attr import attrib, attrs
 from attr.validators import instance_of, optional, provides
-
 from tubes.itube import IDrain, IFount, ISegment
 from tubes.kit import Pauser, beginFlowingTo
 from tubes.undefer import fountToDeferred
+from zope.interface import implementer
 
-from twisted.internet.defer import Deferred
 from twisted.python.failure import Failure
 
-from zope.interface import implementer
-
 
 __all__ = ()
 
 
 # See https://github.com/twisted/tubes/issues/60
-def fountToBytes(fount):
-    # type: (IFount) -> Deferred[bytes]
-    def collect(chunks):
-        # type: (Iterable[bytes]) -> bytes
-        return b"".join(chunks)
-
-    d = fountToDeferred(fount)
-    d.addCallback(collect)
-    return d
+async def fountToBytes(fount: IFount) -> bytes:
+    chunks = await fountToDeferred(fount)
+    return b"".join(chunks)
 
 
 # See https://github.com/twisted/tubes/issues/60
-def bytesToFount(data):
-    # type: (bytes) -> IFount
+def bytesToFount(data: bytes) -> IFount:
     return IOFount(source=BytesIO(data))
 
 
 # https://github.com/twisted/tubes/issues/61
 @implementer(IFount)
 @attrs(frozen=False)
-class IOFount(object):
+class IOFount:
     """
     Fount that reads from a file-like-object.
     """
 
     outputType = ISegment
 
-    _source = attrib()  # type: BinaryIO
+    _source: BinaryIO = attrib()
 
-    drain = attrib(
+    drain: IDrain = attrib(
         validator=optional(provides(IDrain)), default=None, init=False
-    )  # type: IDrain
+    )
     _paused = attrib(validator=instance_of(bool), default=False, init=False)
 
-    def __attrs_post_init__(self):
-        # type: () -> None
+    def __attrs_post_init__(self) -> None:
         self._pauser = Pauser(self._pause, self._resume)
 
-    def _flowToDrain(self):
-        # type: () -> None
+    def _flowToDrain(self) -> None:
         if self.drain is not None and not self._paused:
             data = self._source.read()
             if data:
                 self.drain.receive(data)
             self.drain.flowStopped(Failure(StopIteration()))
 
-    def flowTo(self, drain):
-        # type: (IDrain) -> IFount
+    def flowTo(self, drain: IDrain) -> IFount:
         result = beginFlowingTo(self, drain)
         self._flowToDrain()
         return result
 
-    def pauseFlow(self):
-        # type: () -> None
+    def pauseFlow(self) -> Any:
         return self._pauser.pause()
 
-    def stopFlow(self):
-        # type: () -> None
+    def stopFlow(self) -> Any:
         return self._pauser.resume()
 
-    def _pause(self):
-        # type: () -> None
+    def _pause(self) -> None:
         self._paused = True
 
-    def _resume(self):
-        # type: () -> None
+    def _resume(self) -> None:
         self._paused = False
         self._flowToDrain()
```

### Comparing `klein-20.6.0/src/klein/storage/_memory.py` & `klein-21.8.0/src/klein/storage/_memory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,162 +1,163 @@
 # -*- test-case-name: klein.test.test_memory -*-
 from binascii import hexlify
 from os import urandom
-from typing import Any, Callable, Dict, Iterable, List, Text, cast
+from typing import Any, Callable, Dict, Iterable, Type, cast
 
 import attr
-from attr import Factory
+from zope.interface import Interface, implementer
 
 from twisted.internet.defer import Deferred, fail, succeed
 from twisted.python.components import Componentized
 
-from zope.interface import implementer
-from zope.interface.interfaces import IInterface
-
 from klein.interfaces import (
     ISession,
     ISessionStore,
     NoSuchSession,
     SessionMechanism,
 )
 
-_authCB = Callable[[IInterface, ISession, Componentized], Any]
+
+_authCB = Callable[[Type[Interface], ISession, Componentized], Any]
 
 
 @implementer(ISession)
-@attr.s
-class MemorySession(object):
+@attr.s(auto_attribs=True)
+class MemorySession:
     """
     An in-memory session.
     """
 
-    identifier = attr.ib(type=Text)
-    isConfidential = attr.ib(type=bool)
-    authenticatedBy = attr.ib(type=SessionMechanism)
-    _authorizationCallback = attr.ib(type=_authCB)
-    _components = attr.ib(default=Factory(Componentized), type=Componentized)
+    identifier: str
+    isConfidential: bool
+    authenticatedBy: SessionMechanism
+    _authorizationCallback: _authCB
+    _components: Componentized = attr.ib(factory=Componentized)
 
-    def authorize(self, interfaces):
-        # type: (List[IInterface]) -> Deferred
+    def authorize(self, interfaces: Iterable[Type[Interface]]) -> Deferred:
         """
         Authorize each interface by calling back to the session store's
         authorization callback.
         """
         result = {}
         for interface in interfaces:
             provider = self._authorizationCallback(
                 interface, self, self._components
             )
             if provider is not None:
                 result[interface] = provider
         return succeed(result)
 
 
-class _MemoryAuthorizerFunction(object):
+class _MemoryAuthorizerFunction:
     """
     Type shadow for function with the given attribute.
     """
 
-    __memoryAuthInterface__ = None  # type: IInterface
+    __memoryAuthInterface__: Type[Interface] = None  # type: ignore[assignment]
 
-    def __call__(self, interface, session, data):
-        # type: (IInterface, ISession, Componentized) -> Any
+    def __call__(
+        self, interface: Type[Interface], session: ISession, data: Componentized
+    ) -> Any:
         """
         Return a provider of the given interface.
         """
 
 
-_authFn = Callable[[IInterface, ISession, Componentized], Any]
+_authFn = Callable[[Type[Interface], ISession, Componentized], Any]
 
 
-def declareMemoryAuthorizer(forInterface):
-    # type: (IInterface) -> Callable[[Callable], _MemoryAuthorizerFunction]
+def declareMemoryAuthorizer(
+    forInterface: Type[Interface],
+) -> Callable[[Callable], _MemoryAuthorizerFunction]:
     """
     Declare that the decorated function is an authorizer usable with a memory
     session store.
     """
 
-    def decorate(decoratee):
-        # type: (_authFn) -> _MemoryAuthorizerFunction
+    def decorate(decoratee: _authFn) -> _MemoryAuthorizerFunction:
         decoratee = cast(_MemoryAuthorizerFunction, decoratee)
         decoratee.__memoryAuthInterface__ = forInterface
         return decoratee
 
     return decorate
 
 
-def _noAuthorization(interface, session, data):
-    # type: (IInterface, ISession, Componentized) -> None
+def _noAuthorization(
+    interface: Type[Interface], session: ISession, data: Componentized
+) -> None:
     return None
 
 
 @implementer(ISessionStore)
-@attr.s
-class MemorySessionStore(object):
-    authorizationCallback = attr.ib(type=_authFn, default=_noAuthorization)
-    _secureStorage = attr.ib(
-        type=Dict[str, Any], default=cast(Dict[str, Any], Factory(dict))
-    )
-    _insecureStorage = attr.ib(
-        type=Dict[str, Any], default=cast(Dict[str, Any], Factory(dict))
-    )
+@attr.s(auto_attribs=True)
+class MemorySessionStore:
+    authorizationCallback: _authFn = _noAuthorization
+    _secureStorage: Dict[str, Any] = attr.ib(factory=dict)
+    _insecureStorage: Dict[str, Any] = attr.ib(factory=dict)
 
     @classmethod
-    def fromAuthorizers(cls, authorizers):
-        # type: (List[_MemoryAuthorizerFunction]) -> MemorySessionStore
+    def fromAuthorizers(
+        cls, authorizers: Iterable[_MemoryAuthorizerFunction]
+    ) -> "MemorySessionStore":
         """
         Create a L{MemorySessionStore} from a collection of callbacks which can
         do authorization.
         """
         interfaceToCallable = {}
         for authorizer in authorizers:
+            assert authorizer.__memoryAuthInterface__ is not None
             specifiedInterface = authorizer.__memoryAuthInterface__
             interfaceToCallable[specifiedInterface] = authorizer
 
-        def authorizationCallback(interface, session, data):
-            # type: (IInterface, ISession, Componentized) -> Any
+        def authorizationCallback(
+            interface: Type[Interface], session: ISession, data: Componentized
+        ) -> Any:
             return interfaceToCallable.get(interface, _noAuthorization)(
                 interface, session, data
             )
 
         return cls(authorizationCallback)
 
-    def _storage(self, isConfidential):
-        # type: (bool) -> Dict[str, Any]
+    def _storage(self, isConfidential: bool) -> Dict[str, Any]:
         """
         Return the storage appropriate to the isConfidential flag.
         """
         if isConfidential:
             return self._secureStorage
         else:
             return self._insecureStorage
 
-    def newSession(self, isConfidential, authenticatedBy):
-        # type: (bool, SessionMechanism) -> Deferred
+    def newSession(
+        self, isConfidential: bool, authenticatedBy: SessionMechanism
+    ) -> Deferred:
         storage = self._storage(isConfidential)
         identifier = hexlify(urandom(32)).decode("ascii")
         session = MemorySession(
             identifier,
             isConfidential,
             authenticatedBy,
             self.authorizationCallback,
         )
         storage[identifier] = session
         return succeed(session)
 
-    def loadSession(self, identifier, isConfidential, authenticatedBy):
-        # type: (str, bool, SessionMechanism) -> Deferred
+    def loadSession(
+        self,
+        identifier: str,
+        isConfidential: bool,
+        authenticatedBy: SessionMechanism,
+    ) -> Deferred:
         storage = self._storage(isConfidential)
         if identifier in storage:
             return succeed(storage[identifier])
         else:
             return fail(
                 NoSuchSession(
-                    u"Session not found in memory store {id!r}".format(
+                    "Session not found in memory store {id!r}".format(
                         id=identifier
                     )
                 )
             )
 
-    def sentInsecurely(self, tokens):
-        # type: (Iterable[str]) -> None
+    def sentInsecurely(self, tokens: Iterable[str]) -> None:
         return
```

### Comparing `klein-20.6.0/src/klein/test/test_app.py` & `klein-21.8.0/src/klein/test/test_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,43 @@
-from __future__ import absolute_import, division
+from sys import stdout
+from typing import cast
+from unittest.mock import Mock, patch
 
-import sys
-
-try:
-    from unittest.mock import Mock, patch
-except Exception:
-    from mock import Mock, patch  # type:ignore[misc]
+from zope.interface import implementer
 
 from twisted.python.components import registerAdapter
 from twisted.trial import unittest
+from twisted.web.iweb import IRequest
 
-from .test_resource import requestMock
-from .util import EqualityTestsMixin
 from .. import Klein
 from .._app import KleinRequest
 from .._decorators import bindable, modified, originalName
 from .._interfaces import IKleinRequest
+from .test_resource import MockRequest
+from .util import EqualityTestsMixin
 
 
-class DummyRequest(object):
+@implementer(IRequest)
+class DummyRequest:  # type: ignore[misc]  # incomplete interface
     def __init__(self, n):
         self.n = n
 
     def __eq__(self, other):
         return other.n == self.n
 
-    def __repr__(self):
-        return "<DummyRequest({n})>".format(n=self.n)
-
 
 registerAdapter(KleinRequest, DummyRequest, IKleinRequest)
 
 
 class KleinEqualityTestCase(unittest.TestCase, EqualityTestsMixin):
     """
     Tests for L{Klein}'s implementation of C{==} and C{!=}.
     """
 
-    class _One(object):
+    class _One:
         app = Klein()
 
         def __eq__(self, other):
             return True
 
         def __ne__(self, other):
             return False
@@ -59,15 +55,15 @@
         # equal to everything.
         return self._One().app
 
     def anotherInstance(self):
         return self._another
 
 
-class DuplicateHasher(object):
+class DuplicateHasher:
     """
     Every L{DuplicateHasher} has the same hash value and compares equal to
     every other L{DuplicateHasher}.
     """
 
     __slots__ = ("_identifier",)
 
@@ -151,24 +147,24 @@
 
     def test_kleinNotFoundOnClass(self):
         """
         When the Klein object can't find itself on the class it still preserves
         identity.
         """
 
-        class Wrap(object):
+        class Wrap:
             def __init__(self, wrapped):
                 self._wrapped = wrapped
 
             def __get__(self, instance, owner):
                 if instance is None:
                     return self
                 return self._wrapped.__get__(instance, owner)
 
-        class TwoRouters(object):
+        class TwoRouters:
 
             app1 = Wrap(Klein())
             app2 = Wrap(Klein())
 
         tr = TwoRouters()
 
         self.assertIs(tr.app1, tr.app1)
@@ -176,21 +172,21 @@
 
     def test_bindInstanceIgnoresBlankProperties(self):
         """
         L{Klein.__get__} doesn't propagate L{AttributeError} when
         searching for the bound L{Klein} instance.
         """
 
-        class ClassProperty(object):
+        class ClassProperty:
             def __get__(self, oself, owner):
                 raise AttributeError(
                     "you just don't have that special something"
                 )
 
-        class Oddment(object):
+        class Oddment:
             __something__ = ClassProperty()
             app = Klein()
 
         self.assertIsInstance(Oddment().app, Klein)
 
     def test_submountedRoute(self):
         """
@@ -248,19 +244,21 @@
         c = app.url_map.bind("foo")
         self.assertEqual(c.match("/foo/"), ("branchfunc", {}))
         self.assertEqual(
             c.match("/foo/bar"), ("branchfunc_branch", {"__rest__": "bar"})
         )
 
         self.assertEquals(
-            app.endpoints["branchfunc"].__name__,
+            app.endpoints["branchfunc"].__name__,  # type: ignore[union-attr]
             "route '/foo/' executor for branchfunc",
         )
         self.assertEquals(
-            app.endpoints["branchfunc_branch"].__name__,
+            app.endpoints[
+                "branchfunc_branch"
+            ].__name__,  # type: ignore[union-attr]
             "branch route '/foo/' executor for branchfunc",
         )
         self.assertEquals(
             app.execute_endpoint(
                 "branchfunc_branch", DummyRequest("looking for foo")
             ),
             "foo",
@@ -277,18 +275,18 @@
 
         @k.route("/test")
         @bindable
         def method(*args):
             calls.append(args)
             return 7
 
-        req = object()
+        req = cast(IRequest, object())
         k.execute_endpoint("method", req)
 
-        class BoundTo(object):
+        class BoundTo:
             app = k
 
         b = BoundTo()
         b.app.execute_endpoint("method", req)
 
         self.assertEquals(calls, [(None, req), (b, req)])
         self.assertEqual(originalName(method), "method")
@@ -307,26 +305,26 @@
             return a + b
 
         @modified("supersizer", add, modifier=annotate)
         def megaAdd(a, b):
             return add(a * 1000, b * 10000)
 
         self.assertEqual(megaAdd.supersized, True)
-        self.assertEqual(add.supersized, True)
+        self.assertEqual(add.supersized, True)  # type: ignore[attr-defined]
         self.assertIn("supersizer for add", str(megaAdd))
         self.assertEqual(megaAdd(3, 4), 43000)
 
     def test_classicalRoute(self):
         """
         L{Klein.route} may be used a method decorator when a L{Klein} instance
         is defined as a class variable.
         """
         bar_calls = []
 
-        class Foo(object):
+        class Foo:
             app = Klein()
 
             @app.route("/bar")
             def bar(self, request):
                 bar_calls.append((self, request))
                 return "bar"
 
@@ -342,15 +340,15 @@
     def test_classicalRouteWithTwoInstances(self):
         """
         Multiple instances of a class with a L{Klein} attribute and
         L{Klein.route}'d methods can be created and their L{Klein}s used
         independently.
         """
 
-        class Foo(object):
+        class Foo:
             app = Klein()
 
             def __init__(self):
                 self.bar_calls = []
 
             @app.route("/bar")
             def bar(self, request):
@@ -374,15 +372,15 @@
     def test_classicalRouteWithBranch(self):
         """
         Multiple instances of a class with a L{Klein} attribute and
         L{Klein.route}'d methods can be created and their L{Klein}s used
         independently.
         """
 
-        class Foo(object):
+        class Foo:
             app = Klein()
 
             def __init__(self):
                 self.bar_calls = []
 
             @app.route("/bar/", branch=True)
             def bar(self, request):
@@ -438,15 +436,15 @@
             8080, mock_site.return_value, backlog=50, interface="localhost"
         )
 
         reactor.run.assert_called_with()
 
         mock_site.assert_called_with(mock_kr.return_value)
         mock_kr.assert_called_with(app)
-        mock_log.startLogging.assert_called_with(sys.stdout)
+        mock_log.startLogging.assert_called_with(stdout)
 
     @patch("klein._app.KleinResource")
     @patch("klein._app.Site")
     @patch("klein._app.log")
     @patch("klein._app.reactor")
     def test_runWithLogFile(self, reactor, mock_log, mock_site, mock_kr):
         """
@@ -465,47 +463,47 @@
 
         mock_site.assert_called_with(mock_kr.return_value)
         mock_kr.assert_called_with(app)
         mock_log.startLogging.assert_called_with(logFile)
 
     @patch("klein._app.KleinResource")
     @patch("klein._app.log")
-    @patch("klein._app.endpoints.serverFromString")
+    @patch("klein._app.serverFromString")
     @patch("klein._app.reactor")
     def test_runTCP6(self, reactor, mock_sfs, mock_log, mock_kr):
         """
         L{Klein.run} called with tcp6 endpoint description.
         """
         app = Klein()
         interface = "2001\\:0DB8\\:f00e\\:eb00\\:\\:1"
-        spec = "tcp6:8080:interface={0}".format(interface)
+        spec = f"tcp6:8080:interface={interface}"
         app.run(endpoint_description=spec)
         reactor.run.assert_called_with()
         mock_sfs.assert_called_with(reactor, spec)
-        mock_log.startLogging.assert_called_with(sys.stdout)
+        mock_log.startLogging.assert_called_with(stdout)
         mock_kr.assert_called_with(app)
 
     @patch("klein._app.KleinResource")
     @patch("klein._app.log")
-    @patch("klein._app.endpoints.serverFromString")
+    @patch("klein._app.serverFromString")
     @patch("klein._app.reactor")
     def test_runSSL(self, reactor, mock_sfs, mock_log, mock_kr):
         """
         L{Klein.run} called with SSL endpoint specification.
         """
         app = Klein()
         key = "key.pem"
         cert = "cert.pem"
         dh_params = "dhparam.pem"
         spec_template = "ssl:443:privateKey={0}:certKey={1}"
         spec = spec_template.format(key, cert, dh_params)
         app.run(endpoint_description=spec)
         reactor.run.assert_called_with()
         mock_sfs.assert_called_with(reactor, spec)
-        mock_log.startLogging.assert_called_with(sys.stdout)
+        mock_log.startLogging.assert_called_with(stdout)
         mock_kr.assert_called_with(app)
 
     @patch("klein._app.KleinResource")
     def test_resource(self, mock_kr):
         """
         L{Klien.resource} returns a L{KleinResource}.
         """
@@ -524,60 +522,60 @@
         def userpage(req, name):
             return name
 
         @app.route("/post/<int:postid>", endpoint="bar")
         def foo(req, postid):
             return str(postid)
 
-        request = requestMock(b"/user/john")
+        request = MockRequest(b"/user/john")
         self.assertEqual(
             app.execute_endpoint("userpage", request, "john"), "john"
         )
         self.assertEqual(
-            app.execute_endpoint("bar", requestMock(b"/post/123"), 123), "123"
+            app.execute_endpoint("bar", MockRequest(b"/post/123"), 123), "123"
         )
 
-        request = requestMock(b"/addr")
+        request = MockRequest(b"/addr")
         self.assertEqual(
             app.urlFor(request, "userpage", {"name": "john"}), "/user/john"
         )
 
-        request = requestMock(b"/addr")
+        request = MockRequest(b"/addr")
         self.assertEqual(
             app.urlFor(
                 request, "userpage", {"name": "john"}, force_external=True
             ),
             "http://localhost:8080/user/john",
         )
 
-        request = requestMock(b"/addr", host=b"example.com", port=4321)
+        request = MockRequest(b"/addr", host=b"example.com", port=4321)
         self.assertEqual(
             app.urlFor(
                 request, "userpage", {"name": "john"}, force_external=True
             ),
             "http://example.com:4321/user/john",
         )
 
-        request = requestMock(b"/addr")
+        request = MockRequest(b"/addr")
         url = app.urlFor(
             request,
             "userpage",
             {"name": "john", "age": 29},
             append_unknown=True,
         )
         self.assertEqual(url, "/user/john?age=29")
 
-        request = requestMock(b"/addr")
+        request = MockRequest(b"/addr")
         self.assertEqual(
             app.urlFor(request, "bar", {"postid": 123}), "/post/123"
         )
 
-        request = requestMock(b"/addr")
+        request = MockRequest(b"/addr")
         request.requestHeaders.removeHeader(b"host")
         self.assertEqual(
             app.urlFor(request, "bar", {"postid": 123}), "/post/123"
         )
 
-        request = requestMock(b"/addr")
+        request = MockRequest(b"/addr")
         request.requestHeaders.removeHeader(b"host")
         with self.assertRaises(ValueError):
             app.urlFor(request, "bar", {"postid": 123}, force_external=True)
```

### Comparing `klein-20.6.0/src/klein/test/test_exports.py` & `klein-21.8.0/src/klein/test/test_exports.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,67 +6,62 @@
 
 
 class PublicSymbolsTestCase(unittest.TestCase):
     """
     Tests for public API modules.
     """
 
-    def test_klein(self):
-        # type: () -> None
+    def test_klein(self) -> None:
         """
         Test exports from L{klein}.
         """
         import klein as k
         import klein._app as a
         import klein._plating as p
 
         self.assertIdentical(k.Klein, a.Klein)
         self.assertIdentical(k.handle_errors, a.handle_errors)
         self.assertIdentical(k.route, a.route)
         self.assertIdentical(k.run, a.run)
 
         self.assertIdentical(k.Plating, p.Plating)
 
-    def test_klein_resource(self):
-        # type: () -> None
+    def test_klein_resource(self) -> None:
         """
         Test export of C{resource} from L{klein}.
         """
         import klein as k
         import klein._app as a
 
         self.assertIdentical(k.resource()._app, a.resource()._app)
 
-    def test_app(self):
-        # type: () -> None
+    def test_app(self) -> None:
         """
         Test exports from L{klein.app}.
         """
-        import klein.app as a
         import klein._app as _a
+        import klein.app as a
 
         self.assertIdentical(a.Klein, _a.Klein)
         self.assertIdentical(a.KleinRequest, _a.KleinRequest)
         self.assertIdentical(a.handle_errors, _a.handle_errors)
         self.assertIdentical(a.route, _a.route)
         self.assertIdentical(a.run, _a.run)
 
-    def test_interfaces(self):
-        # type: () -> None
+    def test_interfaces(self) -> None:
         """
         Test exports from L{klein.interfaces}.
         """
-        import klein.interfaces as i
         import klein._interfaces as _i
+        import klein.interfaces as i
 
         self.assertIdentical(i.IKleinRequest, _i.IKleinRequest)
 
-    def test_resource(self):
-        # type: () -> None
+    def test_resource(self) -> None:
         """
         Test exports from L{klein.resource}.
         """
-        import klein.resource as r
         import klein._resource as _r
+        import klein.resource as r
 
         self.assertIdentical(r.KleinResource, _r.KleinResource)
         self.assertIdentical(r.ensure_utf8_bytes, _r.ensure_utf8_bytes)
```

### Comparing `klein-20.6.0/src/klein/test/test_form.py` & `klein-21.8.0/src/klein/test/test_form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,54 @@
-from typing import List, TYPE_CHECKING, Text, cast
+from typing import Any, List, Tuple, cast
 from xml.etree import ElementTree
 
 import attr
-
 from treq import content
 from treq.testing import StubTreq
 
 from twisted.internet.defer import inlineCallbacks
 from twisted.python.compat import nativeString
 from twisted.trial.unittest import SynchronousTestCase
+from twisted.web.iweb import IRequest
 from twisted.web.template import Element, TagLoader, renderer, tags
 
-from klein import Field, Form, Klein, Requirer, SessionProcurer
+from klein import Field, Form, Klein, RenderableForm, Requirer, SessionProcurer
 from klein.interfaces import (
     ISession,
     ISessionStore,
     NoSuchSession,
     SessionMechanism,
     ValidationError,
 )
 from klein.storage.memory import MemorySessionStore
 
 from .._form import textConverter
 
-if TYPE_CHECKING:  # pragma: no cover
-    from typing import Any, Tuple
-    from twisted.web.iweb import IRequest
-    from klein import RenderableForm
-
 
 class DanglingField(Field):
     """
     A dangling field that, for some reason, doesn't remember its own name when
     told.
     """
 
-    def maybeNamed(self, name):
-        # type: (Text) -> Field
+    def maybeNamed(self, name: str) -> Field:
         return self
 
 
-@attr.s(hash=False)
-class TestObject(object):
-    sessionStore = attr.ib(type=ISessionStore)
-    calls = attr.ib(attr.Factory(list), type=List)
+@attr.s(auto_attribs=True, hash=False)
+class TestObject:
+    sessionStore: ISessionStore
+    calls: List = attr.ib(factory=list)
 
     router = Klein()
     requirer = Requirer()
 
     @requirer.prerequisite([ISession])
     @inlineCallbacks
-    def procureASession(self, request):
-        # type: (IRequest) -> Any
+    def procureASession(self, request: IRequest) -> Any:
         try:
             yield (
                 SessionProcurer(
                     self.sessionStore, secureTokenHeader=b"X-Test-Session"
                 ).procureSession(request)
             )
         except NoSuchSession:
@@ -64,189 +57,171 @@
             # component is present before proceeding.
             pass
 
     @requirer.require(
         router.route("/dangling-param", methods=["POST"]),
         dangling=DanglingField(lambda x: x, "text"),
     )
-    def danglingParameter(self, dangling):
-        # type: (str) -> None
+    def danglingParameter(self, dangling: str) -> None:
         "..."
 
     @requirer.require(
         router.route("/handle", methods=["POST"]),
         name=Field.text(),
         value=Field.number(),
     )
-    def handler(self, name, value):
-        # type: (Text, float) -> bytes
+    def handler(self, name: str, value: float) -> bytes:
         self.calls.append((name, value))
         return b"yay"
 
     @requirer.require(
         router.route("/handle-submit", methods=["POST"]),
         name=Field.text(),
-        button=Field.submit(u"OK"),
+        button=Field.submit("OK"),
     )
-    def handlerWithSubmit(self, name, button):
-        # type: (str, str) -> None
+    def handlerWithSubmit(self, name: str, button: str) -> None:
         """
         Form with a submit button.
         """
 
     @requirer.require(
         router.route("/password-field", methods=["POST"]), pw=Field.password()
     )
-    def gotPassword(self, pw):
-        # type: (Text) -> bytes
+    def gotPassword(self, pw: str) -> bytes:
         self.calls.append(("password", pw))
         return b"password received"
 
     @requirer.require(
         router.route("/notrequired", methods=["POST"]),
         name=Field.text(),
         value=Field.number(required=False, default=7.0),
     )
-    def notRequired(self, name, value):
-        # type: (IRequest, Text, float) -> bytes
+    def notRequired(self, name: str, value: float) -> bytes:
         self.calls.append((name, value))
         return b"okay"
 
     @requirer.require(
         router.route("/constrained", methods=["POST"]),
         goldilocks=Field.number(minimum=3, maximum=9),
     )
-    def constrained(self, goldilocks):
-        # type: (int) -> bytes
+    def constrained(self, goldilocks: int) -> bytes:
         self.calls.append(("constrained", goldilocks))
         return b"got it"
 
     @requirer.require(
         router.route("/render", methods=["GET"]),
-        form=Form.rendererFor(handler, action=u"/handle"),
+        form=Form.rendererFor(handler, action="/handle"),
     )
-    def renderer(self, form):
-        # type: (IRequest, Form) -> Form
+    def renderer(self, form: Form) -> Form:
         return form
 
     @requirer.require(
         router.route("/render-submit", methods=["GET"]),
-        form=Form.rendererFor(handlerWithSubmit, action=u"/handle-submit"),
+        form=Form.rendererFor(handlerWithSubmit, action="/handle-submit"),
     )
-    def submitRenderer(self, form):
-        # type: (IRequest, RenderableForm) -> RenderableForm
+    def submitRenderer(self, form: RenderableForm) -> RenderableForm:
         return form
 
     @requirer.require(
         router.route("/render-custom", methods=["GET"]),
-        form=Form.rendererFor(handler, action=u"/handle"),
+        form=Form.rendererFor(handler, action="/handle"),
     )
-    def customFormRender(self, form):
-        # type: (RenderableForm) -> Any
+    def customFormRender(self, form: RenderableForm) -> Any:
         """
         Include just the glue necessary for CSRF protection and let the
         application render the rest of the form.
         """
         return Element(loader=TagLoader(tags.html(tags.body(form.glue()))))
 
     @requirer.require(
         router.route("/render-cascade", methods=["GET"]),
-        form=Form.rendererFor(handler, action=u"/handle"),
+        form=Form.rendererFor(handler, action="/handle"),
     )
-    def cascadeRenderer(self, form):
-        # type: (RenderableForm) -> RenderableForm
-
+    def cascadeRenderer(self, form: RenderableForm) -> Element:
         class CustomElement(Element):
             @renderer
-            def customize(self, request, tag):
-                # type: (IRequest, Any) -> Any
+            def customize(self, request: IRequest, tag: Any) -> Any:
                 return tag("customized")
 
         form.validationErrors[form._form.fields[0]] = ValidationError(
             message=(tags.div(class_="checkme", render="customize"))
         )
 
         return CustomElement(loader=TagLoader(form))
 
     @requirer.require(
         router.route("/handle-validation", methods=["POST"]),
         value=Field.number(maximum=10),
     )
-    def customValidation(self, value):
-        # type: (int) -> None
+    def customValidation(self, value: int) -> None:
         """
         never called.
         """
 
     @requirer.require(Form.onValidationFailureFor(customValidation))
-    def customFailureHandling(self, values):
-        # type: (RenderableForm) -> bytes
+    def customFailureHandling(self, values: RenderableForm) -> bytes:
         """
         Handle validation failure.
         """
         self.calls.append(("validation", values))
         return b"~special~"
 
-    @requirer.require(router.route("/handle-empty", methods=["POST"]),)
-    def emptyHandler(self):
-        # type: () -> bytes
+    @requirer.require(
+        router.route("/handle-empty", methods=["POST"]),
+    )
+    def emptyHandler(self) -> bytes:
         """
         Empty form handler; just for testing rendering.
         """
 
     @requirer.require(
         router.route("/render-empty", methods=["GET"]),
-        form=Form.rendererFor(emptyHandler, action=u"/handle-empty"),
+        form=Form.rendererFor(emptyHandler, action="/handle-empty"),
     )
-    def emptyRenderer(self, form):
-        # type: (RenderableForm) -> RenderableForm
+    def emptyRenderer(self, form: RenderableForm) -> RenderableForm:
         return form
 
 
-def simpleFormRouter():
-    # type: () -> Tuple[Klein, List[Tuple[str, int]]]
+def simpleFormRouter() -> Tuple[Klein, List[Tuple[str, int]]]:
     """
     Create a simple router hooked up to a field handler.
     """
     router = Klein()
     requirer = Requirer()
     calls = []
 
     @requirer.require(
         router.route("/getme", methods=["GET"]),
         name=Field.text(),
         value=Field.number(),
         custom=Field(formInputType="number", converter=int, required=False),
     )
-    def justGet(name, value, custom):
-        # type: (str, int, int) -> bytes
+    def justGet(name: str, value: int, custom: int) -> bytes:
         calls.append((name, value or custom))
         return b"got"
 
     return router, calls
 
 
 class TestForms(SynchronousTestCase):
     """
     Tests for L{klein.Form} and associated tools.
     """
 
-    def test_textConverter(self):
-        # type: () -> None
+    def test_textConverter(self) -> None:
         """
         Convert a string of either type to text.
         """
-        text = u"f\xf6o"
+        text = "f\xf6o"
         for string in (text, text.encode("utf-8")):
             result = textConverter(string)  # type: ignore[type-var]
-            self.assertIsInstance(result, Text)
+            self.assertIsInstance(result, str)
             self.assertEqual(result, text)
 
-    def test_handling(self):
-        # type: () -> None
+    def test_handling(self) -> None:
         """
         A handler for a Form with Fields receives those fields as input, as
         passed by an HTTP client.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -260,18 +235,17 @@
                 "https://localhost/handle",
                 data=dict(name="hello", value="1234", ignoreme="extraneous"),
                 headers={b"X-Test-Session": session.identifier},
             )
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(self.successResultOf(content(response)), b"yay")
-        self.assertEqual(to.calls, [(u"hello", 1234)])
+        self.assertEqual(to.calls, [("hello", 1234)])
 
-    def test_handlingPassword(self):
-        # type: () -> None
+    def test_handlingPassword(self) -> None:
         """
         From the perspective of form handling, passwords are handled like
         strings.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -287,18 +261,17 @@
                 headers={b"X-Test-Session": session.identifier},
             )
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(
             self.successResultOf(content(response)), b"password received"
         )
-        self.assertEqual(to.calls, [(u"password", u"asdfjkl;")])
+        self.assertEqual(to.calls, [("password", "asdfjkl;")])
 
-    def test_numberConstraints(self):
-        # type: () -> None
+    def test_numberConstraints(self) -> None:
         """
         Number parameters have minimum and maximum validations and the object
         will not be called when the values exceed them.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -329,18 +302,17 @@
             )
         )
 
         self.assertEqual(tooHigh.code, 400)
         self.assertEqual(tooLow.code, 400)
         self.assertEqual(justRight.code, 200)
         self.assertEqual(self.successResultOf(content(justRight)), b"got it")
-        self.assertEqual(to.calls, [(u"constrained", 7)])
+        self.assertEqual(to.calls, [("constrained", 7)])
 
-    def test_missingRequiredParameter(self):
-        # type: () -> None
+    def test_missingRequiredParameter(self) -> None:
         """
         If required fields are missing, a default error form is presented and
         the form's handler is not called.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -359,16 +331,15 @@
         self.assertEqual(response.code, 400)
         self.assertIn(
             b"a value was required but none was supplied",
             self.successResultOf(content(response)),
         )
         self.assertEqual(to.calls, [])
 
-    def test_noName(self):
-        # type: () -> None
+    def test_noName(self) -> None:
         """
         A handler for a Form with a Field that doesn't have a name will return
         an error explaining the problem.
         """
         mem = MemorySessionStore()
         session = self.successResultOf(
             mem.newSession(True, SessionMechanism.Header)
@@ -385,16 +356,15 @@
         self.assertEqual(response.code, 500)
         errors = self.flushLoggedErrors(ValueError)
         self.assertEqual(len(errors), 1)
         self.assertIn(
             str(errors[0].value), "Cannot extract unnamed form field."
         )
 
-    def test_handlingGET(self):
-        # type: () -> None
+    def test_handlingGET(self) -> None:
         """
         A GET handler for a Form with Fields receives query parameters matching
         those field names as input.
         """
         router, calls = simpleFormRouter()
 
         stub = StubTreq(router.resource())
@@ -402,18 +372,17 @@
         response = self.successResultOf(
             stub.get(
                 b"https://localhost/getme?name=hello,%20big+world&value=4321"
             )
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(self.successResultOf(content(response)), b"got")
-        self.assertEqual(calls, [(u"hello, big world", 4321)])
+        self.assertEqual(calls, [("hello, big world", 4321)])
 
-    def test_validatingParameters(self):
-        # type: () -> None
+    def test_validatingParameters(self) -> None:
         """
         When a parameter fails to validate - for example, a non-number passed
         to a numeric Field, the request fails with a 400 and the default
         validation failure handler displays a form which explains the error.
         """
         router, calls = simpleFormRouter()
 
@@ -432,16 +401,15 @@
         responseDom = ElementTree.fromstring(responseForm)
         errors = responseDom.findall(
             ".//*[@class='klein-form-validation-error']"
         )
         self.assertEqual(len(errors), 1)
         self.assertEquals(errors[0].text, "not a valid number")
 
-    def test_customParameterValidation(self):
-        # type: () -> None
+    def test_customParameterValidation(self) -> None:
         """
         When a custom parameter fails to validate by raising ValueError - for
         example, a non-number passed to a numeric Field, the request fails with
         a 400 and the default validation failure handler displays a form which
         explains the error.
         """
         router, calls = simpleFormRouter()
@@ -461,23 +429,20 @@
         responseDom = ElementTree.fromstring(responseForm)
         errors = responseDom.findall(
             ".//*[@class='klein-form-validation-error']"
         )
         self.assertEqual(len(errors), 1)
         errorText = cast(str, errors[0].text)
         self.assertIsNot(errorText, None)
-        self.assertTrue(
-            errorText.startswith("invalid literal for int() with base 10: ")
+        self.assertEqual(
+            errorText,
+            "invalid literal for int() with base 10: 'not a number'",
         )
-        # Peculiar 2-step assert because pypy2 (invalidly) sticks a 'u' in
-        # there.
-        self.assertTrue(errorText.endswith("'not a number'"))
 
-    def test_handlingJSON(self):
-        # type: () -> None
+    def test_handlingJSON(self) -> None:
         """
         A handler for a form with Fields receives those fields as input, as
         passed by an HTTP client that submits a JSON POST body.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -486,23 +451,22 @@
 
         to = TestObject(mem)
         stub = StubTreq(to.router.resource())
         response = self.successResultOf(
             stub.post(
                 "https://localhost/handle",
                 json=dict(name="hello", value="1234", ignoreme="extraneous"),
-                headers={u"X-Test-Session": session.identifier},
+                headers={"X-Test-Session": session.identifier},
             )
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(self.successResultOf(content(response)), b"yay")
-        self.assertEqual(to.calls, [(u"hello", 1234)])
+        self.assertEqual(to.calls, [("hello", 1234)])
 
-    def test_missingOptionalParameterJSON(self):
-        # type: () -> None
+    def test_missingOptionalParameterJSON(self) -> None:
         """
         If a required Field is missing from the JSON body, its default value is
         used.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -525,18 +489,17 @@
                 headers={b"X-Test-Session": session.identifier},
             )
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(response2.code, 200)
         self.assertEqual(self.successResultOf(content(response)), b"okay")
         self.assertEqual(self.successResultOf(content(response2)), b"okay")
-        self.assertEqual(to.calls, [(u"one", 7.0), (u"two", 2.0)])
+        self.assertEqual(to.calls, [("one", 7.0), ("two", 2.0)])
 
-    def test_rendering(self):
-        # type: () -> None
+    def test_rendering(self) -> None:
         """
         When a route requires form fields, it renders a form with those fields.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
             mem.newSession(True, SessionMechanism.Header)
@@ -558,16 +521,15 @@
         )
         submitButton = responseDom.findall(".//*[@type='submit']")
         self.assertEqual(len(submitButton), 1)
         self.assertEqual(
             submitButton[0].attrib["name"], "__klein_auto_submit__"
         )
 
-    def test_renderingExplicitSubmit(self):
-        # type: () -> None
+    def test_renderingExplicitSubmit(self) -> None:
         """
         When a form renderer specifies a submit button, no automatic submit
         button is rendered.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -588,16 +550,15 @@
         responseDom = ElementTree.fromstring(
             self.successResultOf(content(response))
         )
         submitButton = responseDom.findall(".//*[@type='submit']")
         self.assertEqual(len(submitButton), 1)
         self.assertEqual(submitButton[0].attrib["name"], "button")
 
-    def test_renderingFormGlue(self):
-        # type: () -> None
+    def test_renderingFormGlue(self) -> None:
         """
         When a form renderer renders just the glue, none of the rest of the
         form is included.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -621,16 +582,15 @@
         submitButton = responseDom.findall(".//*[@type='submit']")
         self.assertEqual(len(submitButton), 0)
         protectionField = responseDom.findall(
             ".//*[@name='__csrf_protection__']"
         )
         self.assertEqual(protectionField[0].attrib["value"], session.identifier)
 
-    def test_renderingEmptyForm(self):
-        # type: () -> None
+    def test_renderingEmptyForm(self) -> None:
         """
         When a form renderer specifies a submit button, no automatic submit
         button is rendered.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -657,18 +617,17 @@
             submitButton[0].attrib["name"], "__klein_auto_submit__"
         )
         protectionField = responseDom.findall(
             ".//*[@name='__csrf_protection__']"
         )
         self.assertEqual(protectionField[0].attrib["value"], session.identifier)
 
-    def test_renderLookupError(self):
-        # type: () -> None
+    def test_renderLookupError(self) -> None:
         """
-        RenderableForm raises L{MissingRenderMethod} if anything attempst to
+        RenderableForm raises L{MissingRenderMethod} if anything attempts to
         look up a render method on it.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
             mem.newSession(True, SessionMechanism.Header)
         )
@@ -682,16 +641,15 @@
         )
         self.assertEqual(response.code, 200)
         # print(self.successResultOf(response.content()).decode('utf-8'))
         failures = self.flushLoggedErrors()
         self.assertEqual(len(failures), 1)
         self.assertIn("MissingRenderMethod", str(failures[0]))
 
-    def test_customValidationHandling(self):
-        # type: () -> None
+    def test_customValidationHandling(self) -> None:
         """
         L{Form.onValidationFailureFor} handles form validation failures by
         handing its thing a renderable form.
         """
         mem = MemorySessionStore()
 
         session = self.successResultOf(
@@ -717,33 +675,29 @@
             [
                 (k.pythonArgumentName, v)
                 for k, v in testobj.calls[-1][1].prevalidationValues.items()
             ],
             [("value", 300)],
         )
 
-    def test_renderingWithNoSessionYet(self):
-        # type: () -> None
+    def test_renderingWithNoSessionYet(self) -> None:
         """
         When a route is rendered with no session, it sets a cookie to establish
         a new session.
         """
         mem = MemorySessionStore()
         stub = StubTreq(TestObject(mem).router.resource())
         response = self.successResultOf(stub.get("https://localhost/render"))
         self.assertEqual(response.code, 200)
         setCookie = response.cookies()["Klein-Secure-Session"]
-        expected = 'value="{}"'.format(setCookie)
-        actual = self.successResultOf(content(response))
-        if not isinstance(expected, bytes):  # type: ignore[unreachable]
-            actual = actual.decode("utf-8")
+        expected = f'value="{setCookie}"'
+        actual = self.successResultOf(content(response)).decode("utf-8")
         self.assertIn(expected, actual)
 
-    def test_noSessionPOST(self):
-        # type: () -> None
+    def test_noSessionPOST(self) -> None:
         """
         An unauthenticated, CSRF-protected form will return a 403 Forbidden
         status code.
         """
         mem = MemorySessionStore()
         to = TestObject(mem)
         stub = StubTreq(to.router.resource())
@@ -753,16 +707,15 @@
                 data=dict(name="hello", value="1234"),
             )
         )
         self.assertEqual(to.calls, [])
         self.assertEqual(response.code, 403)
         self.assertIn(b"CSRF", self.successResultOf(content(response)))
 
-    def test_cookieNoToken(self):
-        # type: () -> None
+    def test_cookieNoToken(self) -> None:
         """
         A cookie-authenticated, CSRF-protected form will return a 403 Forbidden
         status code when a CSRF protection token is not supplied.
         """
         mem = MemorySessionStore()
         session = self.successResultOf(
             mem.newSession(True, SessionMechanism.Cookie)
@@ -778,16 +731,15 @@
                 },
             )
         )
         self.assertEqual(to.calls, [])
         self.assertEqual(response.code, 403)
         self.assertIn(b"CSRF", self.successResultOf(content(response)))
 
-    def test_cookieWithToken(self):
-        # type: () -> None
+    def test_cookieWithToken(self) -> None:
         """
         A cookie-authenticated, CRSF-protected form will call the form as
         expected.
         """
         mem = MemorySessionStore()
         session = self.successResultOf(
             mem.newSession(True, SessionMechanism.Cookie)
```

### Comparing `klein-20.6.0/src/klein/test/test_headers.py` & `klein-21.8.0/src/klein/test/test_headers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,133 @@
 # -*- test-case-name: klein.test.test_headers -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Tests for L{klein._headers}.
 """
 
+from abc import ABC, abstractmethod
 from collections import defaultdict
-from typing import AnyStr, Dict, Iterable, List, Optional, Text, Tuple, cast
+from string import ascii_letters
+from typing import (
+    AnyStr,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    cast,
+)
 
 from hypothesis import given
-from hypothesis.strategies import binary, iterables, text, tuples
+from hypothesis.strategies import (
+    binary,
+    characters,
+    composite,
+    iterables,
+    lists,
+    text,
+    tuples,
+)
 
-from ._strategies import ascii_text, latin1_text
-from ._trial import TestCase
 from .._headers import (
-    FrozenHTTPHeaders,
     HEADER_NAME_ENCODING,
     HEADER_VALUE_ENCODING,
+    FrozenHTTPHeaders,
     IHTTPHeaders,
     IMutableHTTPHeaders,
     MutableHTTPHeaders,
     RawHeaders,
     getFromRawHeaders,
     headerNameAsBytes,
     headerNameAsText,
     headerValueAsBytes,
     headerValueAsText,
     normalizeHeaderName,
     normalizeRawHeaders,
     normalizeRawHeadersFrozen,
 )
+from ._trial import TestCase
 
 
 __all__ = ()
 
 
-def encodeName(name):
-    # type: (Text) -> Optional[bytes]
+T = TypeVar("T")
+DrawCallable = Callable[[Callable[..., T]], T]
+
+
+@composite
+def ascii_text(
+    draw: DrawCallable,
+    min_size: Optional[int] = 0,
+    max_size: Optional[int] = None,
+) -> str:  # pragma: no cover
+    """
+    A strategy which generates ASCII-encodable text.
+
+    @param min_size: The minimum number of characters in the text.
+        C{None} is treated as C{0}.
+
+    @param max_size: The maximum number of characters in the text.
+        Use C{None} for an unbounded size.
+    """
+    return cast(
+        str,
+        draw(
+            text(min_size=min_size, max_size=max_size, alphabet=ascii_letters)
+        ),
+    )
+
+
+@composite  # pragma: no cover
+def latin1_text(
+    draw: DrawCallable,
+    min_size: Optional[int] = 0,
+    max_size: Optional[int] = None,
+) -> str:
+    """
+    A strategy which generates ISO-8859-1-encodable text.
+
+    @param min_size: The minimum number of characters in the text.
+        C{None} is treated as C{0}.
+
+    @param max_size: The maximum number of characters in the text.
+        Use C{None} for an unbounded size.
+    """
+    return "".join(
+        draw(
+            lists(
+                characters(max_codepoint=255),
+                min_size=min_size,
+                max_size=max_size,
+            )
+        )
+    )
+
+
+def encodeName(name: str) -> Optional[bytes]:
     return name.encode(HEADER_NAME_ENCODING)
 
 
-def encodeValue(name):
-    # type: (Text) -> Optional[bytes]
+def encodeValue(name: str) -> Optional[bytes]:
     return name.encode(HEADER_VALUE_ENCODING)
 
 
-def decodeName(name):
-    # type: (bytes) -> Text
+def decodeName(name: bytes) -> str:
     return name.decode(HEADER_NAME_ENCODING)
 
 
-def decodeValue(name):
-    # type: (bytes) -> Text
+def decodeValue(name: bytes) -> str:
     return name.decode(HEADER_VALUE_ENCODING)
 
 
-def headerValueSanitize(value):
-    # type: (AnyStr) -> AnyStr
+def headerValueSanitize(value: AnyStr) -> AnyStr:
     """
     Sanitize a header value by replacing linear whitespace with spaces.
     """
     if isinstance(value, bytes):
         lws = [b"\r\n", b"\r", b"\n"]
         space = b" "
     else:
@@ -73,100 +140,90 @@
 
 class EncodingTests(TestCase):
     """
     Tests for encoding support in L{klein._headers}.
     """
 
     @given(binary())
-    def test_headerNameAsBytesWithBytes(self, name):
-        # type: (bytes) -> None
+    def test_headerNameAsBytesWithBytes(self, name: bytes) -> None:
         """
         L{headerNameAsBytes} passes through L{bytes}.
         """
         self.assertIdentical(headerNameAsBytes(name), name)
 
     @given(latin1_text(min_size=1))
-    def test_headerNameAsBytesWithText(self, name):
-        # type: (Text) -> None
+    def test_headerNameAsBytesWithText(self, name: str) -> None:
         """
-        L{headerNameAsBytes} encodes L{Text} using L{HEADER_NAME_ENCODING}.
+        L{headerNameAsBytes} encodes L{str} using L{HEADER_NAME_ENCODING}.
         """
         rawName = encodeName(name)
         self.assertEqual(headerNameAsBytes(name), rawName)
 
     @given(binary())
-    def test_headerNameAsTextWithBytes(self, name):
-        # type: (bytes) -> None
+    def test_headerNameAsTextWithBytes(self, name: bytes) -> None:
         """
         L{headerNameAsText} decodes L{bytes} using L{HEADER_NAME_ENCODING}.
         """
         self.assertEqual(headerNameAsText(name), decodeName(name))
 
     @given(text(min_size=1))
-    def test_headerNameAsTextWithText(self, name):
-        # type: (Text) -> None
+    def test_headerNameAsTextWithText(self, name: str) -> None:
         """
-        L{headerNameAsText} passes through L{Text}.
+        L{headerNameAsText} passes through L{str}.
         """
         self.assertIdentical(headerNameAsText(name), name)
 
     @given(binary())
-    def test_headerValueAsBytesWithBytes(self, value):
-        # type: (bytes) -> None
+    def test_headerValueAsBytesWithBytes(self, value: bytes) -> None:
         """
         L{headerValueAsBytes} passes through L{bytes}.
         """
         self.assertIdentical(headerValueAsBytes(value), value)
 
     @given(latin1_text(min_size=1))
-    def test_headerValueAsBytesWithText(self, value):
-        # type: (Text) -> None
+    def test_headerValueAsBytesWithText(self, value: str) -> None:
         """
-        L{headerValueAsBytes} encodes L{Text} using L{HEADER_VALUE_ENCODING}.
+        L{headerValueAsBytes} encodes L{str} using L{HEADER_VALUE_ENCODING}.
         """
         rawValue = encodeValue(value)
         self.assertEqual(headerValueAsBytes(value), rawValue)
 
     @given(binary())
-    def test_headerValueAsTextWithBytes(self, value):
-        # type: (bytes) -> None
+    def test_headerValueAsTextWithBytes(self, value: bytes) -> None:
         """
         L{headerValueAsText} decodes L{bytes} using L{HEADER_VALUE_ENCODING}.
         """
         self.assertEqual(headerValueAsText(value), decodeValue(value))
 
     @given(text(min_size=1))
-    def test_headerValueAsTextWithText(self, value):
-        # type: (Text) -> None
+    def test_headerValueAsTextWithText(self, value: str) -> None:
         """
-        L{headerValueAsText} passes through L{Text}.
+        L{headerValueAsText} passes through L{str}.
         """
         self.assertIdentical(headerValueAsText(value), value)
 
 
 class HeaderNameNormalizationTests(TestCase):
     """
     Tests for header name normalization.
     """
 
-    def test_normalizeLowerCase(self):
-        # type: () -> None
+    def test_normalizeLowerCase(self) -> None:
         """
         L{normalizeHeaderName} normalizes header names to lower case.
         """
         self.assertEqual(normalizeHeaderName("FooBar"), "foobar")
 
 
 class RawHeadersConversionTests(TestCase):
     """
     Tests for L{normalizeRawHeaders}.
     """
 
-    def test_pairWrongLength(self):
-        # type: () -> None
+    def test_pairWrongLength(self) -> None:
         """
         L{normalizeRawHeaders} raises L{ValueError} if the C{headerPairs}
         argument is not an iterable of 2-item iterables.
         """
         for invalidPair in ((b"k",), (b"k", b"v", b"x")):
             e = self.assertRaises(
                 ValueError,
@@ -174,368 +231,352 @@
                 normalizeRawHeaders(
                     cast(Iterable[Iterable[bytes]], (invalidPair,))
                 ),
             )
             self.assertEqual(str(e), "header pair must be a 2-item iterable")
 
     @given(latin1_text())
-    def test_pairNameText(self, name):
-        # type: (Text) -> None
+    def test_pairNameText(self, name: str) -> None:
         """
         L{normalizeRawHeaders} converts ISO-8859-1-encodable text names into
         bytes.
         """
         rawHeaders = ((name, b"value"),)
         normalized = tuple(normalizeRawHeaders(rawHeaders))
 
         self.assertEqual(
             normalized,
             ((normalizeHeaderName(headerNameAsBytes(name)), b"value"),),
         )
 
     @given(latin1_text())
-    def test_pairValueText(self, value):
-        # type: (Text) -> None
+    def test_pairValueText(self, value: str) -> None:
         """
         L{normalizeRawHeaders} converts ISO-8859-1-encodable text values into
         bytes.
         """
         rawHeaders = ((b"name", value),)
         normalized = tuple(normalizeRawHeaders(rawHeaders))
 
         self.assertEqual(normalized, ((b"name", headerValueAsBytes(value)),))
 
 
-class GetValuesTestsMixIn(object):
+class GetValuesTestsMixIn(ABC):
     """
     Tests for utilities that access data from the C{RawHeaders} internal
     representation.
     """
 
-    def getValues(self, rawHeaders, name):
-        # type: (RawHeaders, AnyStr) -> Iterable[AnyStr]
+    @abstractmethod
+    def getValues(
+        self, rawHeaders: RawHeaders, name: AnyStr
+    ) -> Iterable[AnyStr]:
         """
         Look up the values for the given header name from the given raw
         headers.
 
         This is called by the other tests in this mix-in class to allow test
         cases that use it to specify how to perform this look-up in the
         implementation being tested.
         """
-        raise NotImplementedError(
-            "{} must implement getValues()".format(self.__class__)
-        )
 
-    def test_getBytesName(self):
-        # type: () -> None
+    def test_getBytesName(self) -> None:
         """
         C{getValues} returns an iterable of L{bytes} values for the
         given L{bytes} header name.
         """
         rawHeaders = ((b"a", b"1"), (b"b", b"2"), (b"c", b"3"), (b"B", b"TWO"))
 
-        normalized = defaultdict(list)  # type: Dict[bytes, List[bytes]]
+        normalized: Dict[bytes, List[bytes]] = defaultdict(list)
         for name, value in rawHeaders:
             normalized[normalizeHeaderName(name)].append(value)
 
         for name, values in normalized.items():
             cast(TestCase, self).assertEqual(
                 list(self.getValues(rawHeaders, name)),
                 values,
-                "header name: {!r}".format(name),
+                f"header name: {name!r}",
             )
 
-    def headerNormalize(self, value):
-        # type: (Text) -> Text
+    def headerNormalize(self, value: str) -> str:
         """
         Test hook for the normalization of header text values, which is a
         behavior Twisted has changed after version 18.9.0.
         """
         return value
 
     @given(iterables(tuples(ascii_text(min_size=1), latin1_text())))
-    def test_getTextName(self, textPairs):
-        # type: (Iterable[Tuple[Text, Text]]) -> None
+    def test_getTextName(self, textPairs: Iterable[Tuple[str, str]]) -> None:
         """
-        C{getValues} returns an iterable of L{Text} values for
-        the given L{Text} header name.
+        C{getValues} returns an iterable of L{str} values for
+        the given L{str} header name.
 
         This test only inserts Latin1 text into the header values, which is
         valid data.
         """
         textHeaders = tuple(
             (name, headerValueSanitize(value)) for name, value in textPairs
         )
 
-        textValues = defaultdict(list)  # type: Dict[Text, List[Text]]
+        textValues: Dict[str, List[str]] = defaultdict(list)
         for name, value in textHeaders:
             textValues[normalizeHeaderName(name)].append(value)
 
         rawHeaders = tuple(
             (headerNameAsBytes(name), headerValueAsBytes(value))
             for name, value in textHeaders
         )
 
         for name, _values in textValues.items():
             cast(TestCase, self).assertEqual(
                 list(self.getValues(rawHeaders, name)),
                 [self.headerNormalize(value) for value in _values],
-                "header name: {!r}".format(name),
+                f"header name: {name!r}",
             )
 
     @given(iterables(tuples(ascii_text(min_size=1), binary())))
-    def test_getTextNameBinaryValues(self, pairs):
-        # type: (Iterable[Tuple[Text, bytes]]) -> None
+    def test_getTextNameBinaryValues(
+        self, pairs: Iterable[Tuple[str, bytes]]
+    ) -> None:
         """
-        C{getValues} returns an iterable of L{Text} values for
-        the given L{Text} header name.
+        C{getValues} returns an iterable of L{str} values for
+        the given L{str} header name.
 
         This test only inserts binary data into the header values, which
         includes invalid data if you are a sane person, but arguably
         technically valid if you read the spec because the spec is unclear
         about header encodings, so we made sure that works also, if only sort
         of.
         """
         rawHeaders = tuple(
             (headerNameAsBytes(name), headerValueSanitize(value))
             for name, value in pairs
         )
 
-        binaryValues = defaultdict(list)  # type: Dict[Text, List[bytes]]
+        binaryValues: Dict[str, List[bytes]] = defaultdict(list)
         for name, value in rawHeaders:
             binaryValues[headerNameAsText(normalizeHeaderName(name))].append(
                 value
             )
 
         for textName, values in binaryValues.items():
             cast(TestCase, self).assertEqual(
                 tuple(self.getValues(rawHeaders, textName)),
                 tuple(
                     self.headerNormalize(headerValueAsText(value))
                     for value in values
                 ),
-                "header name: {!r}".format(textName),
+                f"header name: {textName!r}",
             )
 
-    def test_getInvalidNameType(self):
-        # type: () -> None
+    def test_getInvalidNameType(self) -> None:
         """
         C{getValues} raises L{TypeError} when the given header name is of an
         unknown type.
         """
         e = cast(TestCase, self).assertRaises(
             TypeError, self.getValues, (), object()
         )
         cast(TestCase, self).assertRegex(
-            str(e), "name <object object at 0x[0-9a-f]+> must be text or bytes"
+            str(e), "name <object object at 0x[0-9a-f]+> must be str or bytes"
         )
 
 
 class RawHeadersReadTests(GetValuesTestsMixIn, TestCase):
     """
     Tests for utilities that access data from the "headers tartare" internal
     representation.
     """
 
-    def getValues(self, rawHeaders, name):
-        # type: (RawHeaders, AnyStr) -> Iterable[AnyStr]
+    def getValues(
+        self, rawHeaders: RawHeaders, name: AnyStr
+    ) -> Iterable[AnyStr]:
         return getFromRawHeaders(normalizeRawHeadersFrozen(rawHeaders), name)
 
 
 class FrozenHTTPHeadersTests(GetValuesTestsMixIn, TestCase):
     """
     Tests for L{FrozenHTTPHeaders}.
     """
 
-    def getValues(self, rawHeaders, name):
-        # type: (RawHeaders, AnyStr) -> Iterable[AnyStr]
+    def getValues(
+        self, rawHeaders: RawHeaders, name: AnyStr
+    ) -> Iterable[AnyStr]:
         headers = FrozenHTTPHeaders(rawHeaders=rawHeaders)
         return headers.getValues(name=name)
 
-    def test_interface(self):
-        # type: () -> None
+    def test_interface(self) -> None:
         """
         L{FrozenHTTPHeaders} implements L{IHTTPHeaders}.
         """
         headers = FrozenHTTPHeaders(rawHeaders=())
         self.assertProvides(IHTTPHeaders, headers)
 
-    def test_defaultHeaders(self):
-        # type: () -> None
+    def test_defaultHeaders(self) -> None:
         """
         L{FrozenHTTPHeaders.rawHeaders} is empty by default.
         """
         headers = FrozenHTTPHeaders()
         self.assertEqual(headers.rawHeaders, ())
 
 
-class MutableHTTPHeadersTestsMixIn(GetValuesTestsMixIn):
+class MutableHTTPHeadersTestsMixIn(GetValuesTestsMixIn, ABC):
     """
     Tests for L{IMutableHTTPHeaders} implementations.
     """
 
-    def assertRawHeadersEqual(self, rawHeaders1, rawHeaders2):
-        # type: (RawHeaders, RawHeaders) -> None
+    def assertRawHeadersEqual(
+        self, rawHeaders1: RawHeaders, rawHeaders2: RawHeaders
+    ) -> None:
         cast(TestCase, self).assertEqual(rawHeaders1, rawHeaders2)
 
-    def headers(self, rawHeaders):
-        # type: (RawHeaders) -> IMutableHTTPHeaders
-        raise NotImplementedError(
-            "{} must implement headers()".format(self.__class__)
-        )
+    @abstractmethod
+    def headers(self, rawHeaders: RawHeaders) -> IMutableHTTPHeaders:
+        """
+        Given a L{RawHeaders}, return an L{IMutableHTTPHeaders}.
+        """
 
-    def getValues(self, rawHeaders, name):
-        # type: (RawHeaders, AnyStr) -> Iterable[AnyStr]
+    def getValues(
+        self, rawHeaders: RawHeaders, name: AnyStr
+    ) -> Iterable[AnyStr]:
         headers = self.headers(rawHeaders=rawHeaders)
         return headers.getValues(name=name)
 
-    def test_interface(self):
-        # type: () -> None
+    def test_interface(self) -> None:
         """
         Class implements L{IMutableHTTPHeaders}.
         """
         headers = self.headers(rawHeaders=())
         cast(TestCase, self).assertProvides(IMutableHTTPHeaders, headers)
 
-    def test_rawHeaders(self):
-        # type: () -> None
+    def test_rawHeaders(self) -> None:
         """
         L{IMutableHTTPHeaders.rawHeaders} equals the raw headers passed at init
         time as a tuple.
         """
         rawHeaders = [(b"a", b"1"), (b"b", b"2"), (b"c", b"3")]
         headers = self.headers(rawHeaders=rawHeaders)
         self.assertRawHeadersEqual(headers.rawHeaders, tuple(rawHeaders))
 
-    def test_removeBytesName(self):
-        # type: () -> None
+    def test_removeBytesName(self) -> None:
         """
         L{IMutableHTTPHeaders.remove} removes all values for the given L{bytes}
         header name.
         """
         rawHeaders = ((b"a", b"1"), (b"b", b"2a"), (b"c", b"3"), (b"b", b"2b"))
         headers = self.headers(rawHeaders=rawHeaders)
         headers.remove(name=b"b")
 
         self.assertRawHeadersEqual(
             headers.rawHeaders, ((b"a", b"1"), (b"c", b"3"))
         )
 
-    def test_removeTextName(self):
-        # type: () -> None
+    def test_removeTextName(self) -> None:
         """
-        L{IMutableHTTPHeaders.remove} removes all values for the given L{Text}
+        L{IMutableHTTPHeaders.remove} removes all values for the given L{str}
         header name.
         """
         rawHeaders = ((b"a", b"1"), (b"b", b"2a"), (b"c", b"3"), (b"b", b"2b"))
         headers = self.headers(rawHeaders=rawHeaders)
-        headers.remove(name=u"b")
+        headers.remove(name="b")
 
         self.assertRawHeadersEqual(
             headers.rawHeaders, ((b"a", b"1"), (b"c", b"3"))
         )
 
-    def test_removeInvalidNameType(self):
-        # type: () -> None
+    def test_removeInvalidNameType(self) -> None:
         """
         L{IMutableHTTPHeaders.remove} raises L{TypeError} when the given header
         name is of an unknown type.
         """
         headers = self.headers(rawHeaders=())
 
         e = cast(TestCase, self).assertRaises(
             TypeError, headers.remove, object()
         )
         cast(TestCase, self).assertRegex(
-            str(e), "name <object object at 0x[0-9a-f]+> must be text or bytes"
+            str(e), "name <object object at 0x[0-9a-f]+> must be str or bytes"
         )
 
-    def test_addValueBytesName(self):
-        # type: () -> None
+    def test_addValueBytesName(self) -> None:
         """
         L{IMutableHTTPHeaders.addValue} adds the given L{bytes} value for the
         given L{bytes} header name.
         """
         rawHeaders = ((b"a", b"1"), (b"b", b"2a"))
         headers = self.headers(rawHeaders=rawHeaders)
         headers.addValue(name=b"b", value=b"2b")
 
         self.assertRawHeadersEqual(
             headers.rawHeaders, ((b"a", b"1"), (b"b", b"2a"), (b"b", b"2b"))
         )
 
-    def test_addValueTextName(self):
-        # type: () -> None
+    def test_addValueTextName(self) -> None:
         """
-        L{IMutableHTTPHeaders.addValue} adds the given L{Text} value for the
-        given L{Text} header name.
+        L{IMutableHTTPHeaders.addValue} adds the given L{str} value for the
+        given L{str} header name.
         """
         rawHeaders = ((b"a", b"1"), (b"b", b"2a"))
         headers = self.headers(rawHeaders=rawHeaders)
-        headers.addValue(name=u"b", value=u"2b")
+        headers.addValue(name="b", value="2b")
 
         self.assertRawHeadersEqual(
             headers.rawHeaders, ((b"a", b"1"), (b"b", b"2a"), (b"b", b"2b"))
         )
 
-    def test_addValueBytesNameTextValue(self):
-        # type: () -> None
+    def test_addValueBytesNameTextValue(self) -> None:
         """
         L{IMutableHTTPHeaders.addValue} raises L{TypeError} when the given
-        header name is L{bytes} and the given value is L{Text}.
+        header name is L{bytes} and the given value is L{str}.
         """
         headers = self.headers(rawHeaders=())
 
         e = cast(TestCase, self).assertRaises(
-            TypeError, headers.addValue, b"a", u"1"
+            TypeError, headers.addValue, b"a", "1"
         )
         cast(TestCase, self).assertRegex(
             str(e), "value u?'1' must be bytes to match name b?'a'"
         )
 
-    def test_addValueTextNameBytesValue(self):
-        # type: () -> None
+    def test_addValueTextNameBytesValue(self) -> None:
         """
         L{IMutableHTTPHeaders.addValue} raises L{TypeError} when the given
-        header name is L{Text} and the given value is L{bytes}.
+        header name is L{str} and the given value is L{bytes}.
         """
         headers = self.headers(rawHeaders=())
 
         e = cast(TestCase, self).assertRaises(
-            TypeError, headers.addValue, u"a", b"1"
+            TypeError, headers.addValue, "a", b"1"
         )
         cast(TestCase, self).assertRegex(
-            str(e), "value b?'1' must be text to match name u?'a'"
+            str(e), "value b?'1' must be str to match name u?'a'"
         )
 
-    def test_addValueInvalidNameType(self):
-        # type: () -> None
+    def test_addValueInvalidNameType(self) -> None:
         """
         L{IMutableHTTPHeaders.addValue} raises L{TypeError} when the given
         header name is of an unknown type.
         """
         headers = self.headers(rawHeaders=())
 
         e = cast(TestCase, self).assertRaises(
             TypeError, headers.addValue, object(), b"1"
         )
         cast(TestCase, self).assertRegex(
-            str(e), "name <object object at 0x[0-9a-f]+> must be text or bytes"
+            str(e), "name <object object at 0x[0-9a-f]+> must be str or bytes"
         )
 
 
 class MutableHTTPHeadersTests(MutableHTTPHeadersTestsMixIn, TestCase):
     """
     Tests for L{MutableHTTPHeaders}.
     """
 
-    def headers(self, rawHeaders):
-        # type: (RawHeaders) -> IMutableHTTPHeaders
+    def headers(self, rawHeaders: RawHeaders) -> IMutableHTTPHeaders:
         return MutableHTTPHeaders(rawHeaders=rawHeaders)
 
-    def test_defaultHeaders(self):
-        # type: () -> None
+    def test_defaultHeaders(self) -> None:
         """
         L{MutableHTTPHeaders.rawHeaders} is empty by default.
         """
         headers = MutableHTTPHeaders()
         self.assertEqual(headers.rawHeaders, ())
```

### Comparing `klein-20.6.0/src/klein/test/test_headers_compat.py` & `klein-21.8.0/src/klein/test/test_headers_compat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,67 @@
 # -*- test-case-name: klein.test.test_headers_compat -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Tests for L{klein._headers}.
 """
 
-from typing import Text
-
 from twisted.web.http_headers import Headers
 
-from ._trial import TestCase
-from .test_headers import MutableHTTPHeadersTestsMixIn
 from .._headers import (
     IMutableHTTPHeaders,
     RawHeaders,
     normalizeRawHeadersFrozen,
 )
 from .._headers_compat import HTTPHeadersWrappingHeaders
+from ._trial import TestCase
+from .test_headers import MutableHTTPHeadersTestsMixIn
 
 
 try:
     from twisted.web.http_headers import _sanitizeLinearWhitespace
-except ImportError:
-    _sanitizeLinearWhitespace = None
+except ImportError:  # pragma: no cover
+    _sanitizeLinearWhitespace = None  # type: ignore[assignment]
 
 
-def _twistedHeaderNormalize(value):
-    # type: (Text) -> Text
+def _twistedHeaderNormalize(value: str) -> str:
     """
     Normalize the given header value according to the rules of the installed
     Twisted version.
     """
-    if _sanitizeLinearWhitespace is None:
-        return value
+    if _sanitizeLinearWhitespace is None:  # pragma: no cover
+        return value  # type: ignore[unreachable]
     else:
         return _sanitizeLinearWhitespace(value.encode("utf-8")).decode("utf-8")
 
 
 __all__ = ()
 
 
 class HTTPHeadersWrappingHeadersTests(MutableHTTPHeadersTestsMixIn, TestCase):
     """
     Tests for L{HTTPHeadersWrappingHeaders}.
     """
 
-    def assertRawHeadersEqual(self, rawHeaders1, rawHeaders2):
-        # type: (RawHeaders, RawHeaders) -> None
-        super(HTTPHeadersWrappingHeadersTests, self).assertRawHeadersEqual(
-            sorted(rawHeaders1), sorted(rawHeaders2)
-        )
+    def assertRawHeadersEqual(
+        self, rawHeaders1: RawHeaders, rawHeaders2: RawHeaders
+    ) -> None:
+        super().assertRawHeadersEqual(sorted(rawHeaders1), sorted(rawHeaders2))
 
-    def headerNormalize(self, value):
-        # type: (Text) -> Text
+    def headerNormalize(self, value: str) -> str:
         return _twistedHeaderNormalize(value)
 
-    def headers(self, rawHeaders):
-        # type: (RawHeaders) -> IMutableHTTPHeaders
+    def headers(self, rawHeaders: RawHeaders) -> IMutableHTTPHeaders:
         headers = Headers()
         for rawName, rawValue in rawHeaders:
             headers.addRawHeader(rawName, rawValue)
 
         return HTTPHeadersWrappingHeaders(headers=headers)
 
-    def test_rawHeaders(self):
-        # type: () -> None
+    def test_rawHeaders(self) -> None:
         """
         L{MutableHTTPHeaders.rawHeaders} equals raw headers matching the
         L{Headers} given at init time.
         """
         rawHeaders = ((b"b", b"2a"), (b"a", b"1"), (b"B", b"2b"))
         webHeaders = Headers()
         for name, value in rawHeaders:
```

### Comparing `klein-20.6.0/src/klein/test/test_memory.py` & `klein-21.8.0/src/klein/test/test_memory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 
-from twisted.trial.unittest import SynchronousTestCase
-
 from zope.interface import Interface
 from zope.interface.verify import verifyObject
 
+from twisted.trial.unittest import SynchronousTestCase
+
 from klein.interfaces import ISession, ISessionStore, SessionMechanism
 from klein.storage.memory import MemorySessionStore, declareMemoryAuthorizer
 
 
 class IFoo(Interface):
     """
     Testing interface 1.
@@ -22,58 +22,53 @@
 
 
 class MemoryTests(SynchronousTestCase):
     """
     Tests for memory-based session storage.
     """
 
-    def test_interfaceCompliance(self):
-        # type: () -> None
+    def test_interfaceCompliance(self) -> None:
         """
         Verify that the session store complies with the relevant interfaces.
         """
         store = MemorySessionStore()
         verifyObject(ISessionStore, store)
         verifyObject(
             ISession,
             self.successResultOf(
                 store.newSession(True, SessionMechanism.Header)
             ),
         )
 
-    def test_noAuthorizers(self):
-        # type: () -> None
+    def test_noAuthorizers(self) -> None:
         """
         By default, L{MemorySessionStore} contains no authorizers and the
         sessions it returns will authorize any supplied interfaces as None.
         """
         store = MemorySessionStore()
         session = self.successResultOf(
             store.newSession(True, SessionMechanism.Header)
         )
         self.assertEqual(
             self.successResultOf(session.authorize([IFoo, IBar])), {}
         )
 
-    def test_simpleAuthorization(self):
-        # type: () -> None
+    def test_simpleAuthorization(self) -> None:
         """
         L{MemorySessionStore.fromAuthorizers} takes a set of functions
         decorated with L{declareMemoryAuthorizer} and constructs a session
         store that can authorize for those interfaces.
         """
 
         @declareMemoryAuthorizer(IFoo)
-        def fooMe(interface, session, componentized):
-            # type: (Any, Any, Any) -> int
+        def fooMe(interface: Any, session: Any, componentized: Any) -> int:
             return 1
 
         @declareMemoryAuthorizer(IBar)
-        def barMe(interface, session, componentized):
-            # type: (Any, Any, Any) -> int
+        def barMe(interface: Any, session: Any, componentized: Any) -> int:
             return 2
 
         store = MemorySessionStore.fromAuthorizers([fooMe, barMe])
         session = self.successResultOf(
             store.newSession(False, SessionMechanism.Cookie)
         )
         self.assertEqual(
```

### Comparing `klein-20.6.0/src/klein/test/test_message.py` & `klein-21.8.0/src/klein/test/test_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,148 +1,152 @@
 # -*- test-case-name: klein.test.test_message -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Tests for L{klein._message}.
 """
 
+from abc import ABC, abstractmethod
 from typing import cast
 
 from hypothesis import given
 from hypothesis.strategies import binary
 
-from ._trial import TestCase
-from .._interfaces import IHTTPMessage
+from twisted.internet.defer import ensureDeferred
+
+from .._imessage import IHTTPMessage
 from .._message import FountAlreadyAccessedError, bytesToFount, fountToBytes
+from ._trial import TestCase
 
 
 __all__ = ()
 
 
-class FrozenHTTPMessageTestsMixIn(object):
+class FrozenHTTPMessageTestsMixIn(ABC):
     """
     Mix-In class for implementations of IHTTPMessage.
     """
 
     @classmethod
-    def messageFromBytes(cls, data=b""):
-        # type: (bytes) -> IHTTPMessage
+    @abstractmethod
+    def messageFromBytes(cls, data: bytes = b"") -> IHTTPMessage:
         """
         Return a new instance of an L{IHTTPMessage} implementation using the
         given bytes as the message body.
         """
-        raise NotImplementedError("{} must implement getValues()".format(cls))
 
     @classmethod
-    def messageFromFountFromBytes(cls, data=b""):
-        # type: (bytes) -> IHTTPMessage
+    def messageFromFountFromBytes(cls, data: bytes = b"") -> IHTTPMessage:
         """
         Return a new instance of an L{IHTTPMessage} implementation using a
         fount containing the given bytes as the message body.
         """
         return cls.messageFromBytes(bytesToFount(data))
 
-    def test_interface_message(self):
-        # type: () -> None
+    def test_interface_message(self) -> None:
         """
         Message instance implements L{IHTTPMessage}.
         """
         message = self.messageFromBytes()
         cast(TestCase, self).assertProvides(IHTTPMessage, message)
 
     @given(binary())
-    def test_bodyAsFountFromBytes(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsFountFromBytes(self, data: bytes) -> None:
         """
         C{bodyAsFount} returns a fount with the same bytes given to
         C{__init__}.
         """
         message = self.messageFromBytes(data)
         fount = message.bodyAsFount()
-        body = cast(TestCase, self).successResultOf(fountToBytes(fount))
+        body = cast(TestCase, self).successResultOf(
+            ensureDeferred(fountToBytes(fount))
+        )
 
         cast(TestCase, self).assertEqual(body, data)
 
     @given(binary())
-    def test_bodyAsFountFromBytesTwice(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsFountFromBytesTwice(self, data: bytes) -> None:
         """
         C{bodyAsFount} raises L{FountAlreadyAccessedError} if called more than
         once, when created from bytes.
         """
         message = self.messageFromBytes(data)
         message.bodyAsFount()
         cast(TestCase, self).assertRaises(
             FountAlreadyAccessedError, message.bodyAsFount
         )
 
     @given(binary())
-    def test_bodyAsFountFromFount(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsFountFromFount(self, data: bytes) -> None:
         """
         C{bodyAsBytes} returns the bytes from the fount given to C{__init__}.
         """
         message = self.messageFromFountFromBytes(data)
         fount = message.bodyAsFount()
-        body = cast(TestCase, self).successResultOf(fountToBytes(fount))
-
+        body = cast(TestCase, self).successResultOf(
+            ensureDeferred(fountToBytes(fount))
+        )
         cast(TestCase, self).assertEqual(body, data)
 
     @given(binary())
-    def test_bodyAsFountFromFountTwice(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsFountFromFountTwice(self, data: bytes) -> None:
         """
         C{bodyAsFount} raises L{FountAlreadyAccessedError} if called more than
         once, when created from a fount.
         """
         message = self.messageFromFountFromBytes(data)
         message.bodyAsFount()
         cast(TestCase, self).assertRaises(
             FountAlreadyAccessedError, message.bodyAsFount
         )
 
     @given(binary())
-    def test_bodyAsBytesFromBytes(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsBytesFromBytes(self, data: bytes) -> None:
         """
         C{bodyAsBytes} returns the same bytes given to C{__init__}.
         """
         message = self.messageFromBytes(data)
-        body = cast(TestCase, self).successResultOf(message.bodyAsBytes())
-
+        body = cast(TestCase, self).successResultOf(
+            ensureDeferred(message.bodyAsBytes())
+        )
         cast(TestCase, self).assertEqual(body, data)
 
     @given(binary())
-    def test_bodyAsBytesFromBytesCached(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsBytesFromBytesCached(self, data: bytes) -> None:
         """
         C{bodyAsBytes} called twice returns the same object both times, when
         created from bytes.
         """
         message = self.messageFromBytes(data)
-        body1 = cast(TestCase, self).successResultOf(message.bodyAsBytes())
-        body2 = cast(TestCase, self).successResultOf(message.bodyAsBytes())
-
+        body1 = cast(TestCase, self).successResultOf(
+            ensureDeferred(message.bodyAsBytes())
+        )
+        body2 = cast(TestCase, self).successResultOf(
+            ensureDeferred(message.bodyAsBytes())
+        )
         cast(TestCase, self).assertIdentical(body1, body2)
 
     @given(binary())
-    def test_bodyAsBytesFromFount(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsBytesFromFount(self, data: bytes) -> None:
         """
         C{bodyAsBytes} returns the bytes from the fount given to C{__init__}.
         """
         message = self.messageFromFountFromBytes(data)
-        body = cast(TestCase, self).successResultOf(message.bodyAsBytes())
+        body = cast(TestCase, self).successResultOf(
+            ensureDeferred(message.bodyAsBytes())
+        )
         cast(TestCase, self).assertEqual(body, data)
 
     @given(binary())
-    def test_bodyAsBytesFromFountCached(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsBytesFromFountCached(self, data: bytes) -> None:
         """
         C{bodyAsBytes} called twice returns the same object both times, when
         created from a fount.
         """
         message = self.messageFromFountFromBytes(data)
-        body1 = cast(TestCase, self).successResultOf(message.bodyAsBytes())
-        body2 = cast(TestCase, self).successResultOf(message.bodyAsBytes())
-
+        body1 = cast(TestCase, self).successResultOf(
+            ensureDeferred(message.bodyAsBytes())
+        )
+        body2 = cast(TestCase, self).successResultOf(
+            ensureDeferred(message.bodyAsBytes())
+        )
         cast(TestCase, self).assertIdentical(body1, body2)
```

### Comparing `klein-20.6.0/src/klein/test/test_plating.py` & `klein-21.8.0/src/klein/test/test_plating.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 """
 Tests for L{klein.plating}.
 """
 
-from __future__ import (
-    absolute_import,
-    division,
-    print_function,
-    unicode_literals,
-)
 
 import json
 from string import printable
+from typing import Any
 
 import attr
-
-from hypothesis import given, settings, strategies as st
+from hypothesis import given, settings
+from hypothesis import strategies as st
 
 from twisted.internet.defer import Deferred, succeed
-from twisted.trial.unittest import (
-    SynchronousTestCase,
-    TestCase as AsynchronousTestCase,
-)
+from twisted.trial.unittest import SynchronousTestCase
+from twisted.trial.unittest import TestCase as AsynchronousTestCase
 from twisted.web.error import FlattenerError, MissingRenderMethod
 from twisted.web.template import slot, tags
 
-from .test_resource import _render, requestMock
 from .. import Klein, Plating
 from .._plating import ATOM_TYPES, PlatedElement, resolveDeferredObjects
+from .test_resource import MockRequest, _render
 
 
 page = Plating(
     defaults={
         "title": "default title unchanged",
         Plating.CONTENT: "NEVER MIND THE CONTENT",
     },
@@ -41,16 +34,22 @@
             tags.div(slot(Plating.CONTENT), Class="content"),
             tags.div(id="rendermethod", render="registeredRenderMethod"),
         ),
     ),
 )
 
 element = Plating(
-    defaults={"a": "NO VALUE FOR A", "b": "NO VALUE FOR B",},
-    tags=tags.div(tags.span("a: ", slot("a")), tags.span("b: ", slot("b")),),
+    defaults={
+        "a": "NO VALUE FOR A",
+        "b": "NO VALUE FOR B",
+    },
+    tags=tags.div(
+        tags.span("a: ", slot("a")),
+        tags.span("b: ", slot("b")),
+    ),
 )
 
 
 @element.widgeted
 def enwidget(a, b):
     """
     Provide some values for the L{element} template.
@@ -74,15 +73,15 @@
     # Variable signature because since it's for testing, 'page' here has the
     # unusual property that is used in both bound (i.e. "has self") and unbound
     # contexts.
     tag = args[-1]
     return tag("(self)" if len(args) == 3 else "", "some text!")
 
 
-class InstanceWidget(object):
+class InstanceWidget:
     """
     A class with a method that's a L{Plating.widget}.
     """
 
     @element.widgeted
     def enwidget(self, a, b):
         """
@@ -94,26 +93,26 @@
     def deferredEnwidget(self, a, b):
         """
         Provide some L{Deferred} values for the L{element} template.
         """
         return {"a": succeed(a), "b": succeed(b)}
 
 
-@attr.s
-class DeferredValue(object):
+@attr.s(auto_attribs=True)
+class DeferredValue:
     """
     A value within a JSON serializable object that is deferred.
 
     @param value: The value.
 
     @param deferred: The L{Deferred} representing the value.
     """
 
-    value = attr.ib()  # type: object
-    deferred = attr.ib(attr.Factory(Deferred))  # type: Deferred
+    value: Any
+    deferred: Deferred = attr.ib(factory=Deferred)
 
     def resolve(self):
         """
         Resolve the L{Deferred} that represents the value with the
         value itself.
         """
         self.deferred.callback(self.value)
@@ -171,15 +170,15 @@
         elif isinstance(obj, tuple):
             return tuple(transformer(child) for child in obj)
         elif isinstance(obj, list):
             return [transformer(child) for child in obj]
         elif isinstance(obj, dict):
             return {transformer(k): transformer(v) for k, v in obj.items()}
         else:
-            raise AssertionError("Object of unknown type {!r}".format(obj))
+            raise AssertionError(f"Object of unknown type {obj!r}")
 
     return visit(jsonObject)
 
 
 class TransformJSONObjectTests(SynchronousTestCase):
     """
     Tests for L{transform_json_object}.
@@ -239,15 +238,16 @@
 class ResolveDeferredObjectsTests(SynchronousTestCase):
     """
     Tests for L{resolve_deferred_objects}.
     """
 
     @settings(max_examples=500)
     @given(
-        jsonObject=jsonObjects, data=st.data(),
+        jsonObject=jsonObjects,
+        data=st.data(),
     )
     def test_resolveObjects(self, jsonObject, data):
         """
         A JSON serializable object that may contain L{Deferred}s or a
         L{Deferred} that resolves to a JSON serializable object
         resolves to an object that contains no L{Deferred}s.
         """
@@ -258,26 +258,28 @@
             if data.draw(choose):
                 deferredValues.append(DeferredValue(value))
                 return deferredValues[-1].deferred
             else:
                 return value
 
         deferredJSONObject = transformJSONObject(
-            jsonObject, maybeWrapInDeferred,
+            jsonObject,
+            maybeWrapInDeferred,
         )
 
-        resolved = resolveDeferredObjects(deferredJSONObject)
+        resolved: "Deferred[Any]" = resolveDeferredObjects(deferredJSONObject)
 
         for value in deferredValues:
             value.resolve()
 
         self.assertEqual(self.successResultOf(resolved), jsonObject)
 
     @given(
-        jsonObject=jsonObjects, data=st.data(),
+        jsonObject=jsonObjects,
+        data=st.data(),
     )
     def test_elementSerialized(self, jsonObject, data):
         """
         A L{PlatedElement} within a JSON serializable object replaced
         by its JSON representation.
         """
         choose = st.booleans()
@@ -291,30 +293,31 @@
                     presentationSlots={},
                     renderers={},
                 )
             else:
                 return value
 
         withPlatingElements = transformJSONObject(
-            jsonObject, injectPlatingElements,
+            jsonObject,
+            injectPlatingElements,
         )
 
-        resolved = resolveDeferredObjects(withPlatingElements)
+        resolved: "Deferred[Any]" = resolveDeferredObjects(withPlatingElements)
 
         self.assertEqual(self.successResultOf(resolved), jsonObject)
 
     def test_unserializableObject(self):
         """
         An object that cannot be serialized causes the L{Deferred} to
         fail with an informative L{TypeError}.
 
         """
 
         @attr.s
-        class ConsistentRepr(object):
+        class ConsistentRepr:
             """
             Objects with a predictable repr
             """
 
         exception = self.failureResultOf(
             resolveDeferredObjects(ConsistentRepr())
         ).value
@@ -336,15 +339,15 @@
 
     def get(self, uri):
         """
         Issue a virtual GET request to the given path that is expected to
         succeed synchronously, and return the generated request object and
         written bytes.
         """
-        request = requestMock(uri)
+        request = MockRequest(uri)
         d = _render(self.kr, request)
         self.successResultOf(d)
         return request, request.getWrittenData()
 
     def test_template_html(self):
         """
         Rendering a L{Plating.routed} decorated route results in templated
@@ -362,15 +365,15 @@
 
     def test_selfhood(self):
         """
         Rendering a L{Plating.routed} decorated route on a method still results
         in the decorated method receiving the appropriate C{self}.
         """
 
-        class AppObj(object):
+        class AppObj:
             app = Klein()
 
             def __init__(self, x):
                 self.x = x
 
             @page.routed(app.route("/"), tags.span(slot("yeah")))
             def plateInstance(self, request):
@@ -393,15 +396,15 @@
         @page.routed(self.app.route("/"), tags.span(slot("ok")))
         def plateMe(request):
             return {"ok": "an-plating-test"}
 
         request, written = self.get(b"/?json=true")
         self.assertEqual(
             request.responseHeaders.getRawHeaders(b"content-type")[0],
-            b"text/json; charset=utf-8",
+            b"application/json",
         )
         self.assertEquals(
             {"ok": "an-plating-test", "title": "default title unchanged"},
             json.loads(written.decode("utf-8")),
         )
 
     def test_template_json_contains_deferred(self):
@@ -414,15 +417,15 @@
         @page.routed(self.app.route("/"), tags.span(slot("ok")))
         def plateMe(request):
             return {"ok": succeed("an-plating-test")}
 
         request, written = self.get(b"/?json=true")
         self.assertEqual(
             request.responseHeaders.getRawHeaders(b"content-type")[0],
-            b"text/json; charset=utf-8",
+            b"application/json",
         )
         self.assertEquals(
             {"ok": "an-plating-test", "title": "default title unchanged"},
             json.loads(written.decode("utf-8")),
         )
 
     def test_template_numbers(self):
```

### Comparing `klein-20.6.0/src/klein/test/test_request.py` & `klein-21.8.0/src/klein/test/test_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,58 @@
 # -*- test-case-name: klein.test.test_request -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Tests for L{klein._request}.
 """
 
 from hyperlink import DecodedURL
 
-from ._trial import TestCase
-from .test_message import FrozenHTTPMessageTestsMixIn
 from .._headers import FrozenHTTPHeaders
-from .._interfaces import IHTTPMessage
+from .._imessage import IHTTPMessage
 from .._request import FrozenHTTPRequest, IHTTPRequest
+from ._trial import TestCase
+from .test_message import FrozenHTTPMessageTestsMixIn
 
 
 __all__ = ()
 
 
 class FrozenHTTPRequestTests(FrozenHTTPMessageTestsMixIn, TestCase):
     """
     Tests for L{FrozenHTTPRequest}.
     """
 
     @staticmethod
-    def requestFromBytes(data=b""):
-        # type: (bytes) -> FrozenHTTPRequest
+    def requestFromBytes(data: bytes = b"") -> FrozenHTTPRequest:
         return FrozenHTTPRequest(
-            method=u"GET",
-            uri=DecodedURL.fromText(u"https://twistedmatrix.com/"),
+            method="GET",
+            uri=DecodedURL.fromText("https://twistedmatrix.com/"),
             headers=FrozenHTTPHeaders(rawHeaders=()),
             body=data,
         )
 
     @classmethod
-    def messageFromBytes(cls, data=b""):
-        # type: (bytes) -> IHTTPMessage
+    def messageFromBytes(cls, data: bytes = b"") -> IHTTPMessage:
         return cls.requestFromBytes(data)
 
-    def test_interface(self):
-        # type: () -> None
+    def test_interface(self) -> None:
         """
         L{FrozenHTTPRequest} implements L{IHTTPRequest}.
         """
         request = self.requestFromBytes()
         self.assertProvides(IHTTPRequest, request)
 
-    def test_initInvalidBodyType(self):
-        # type: () -> None
+    def test_initInvalidBodyType(self) -> None:
         """
         L{FrozenHTTPRequest} raises L{TypeError} when given a body of an
         unknown type.
         """
         e = self.assertRaises(
             TypeError,
             FrozenHTTPRequest,
-            method=u"GET",
-            uri=DecodedURL.fromText(u"https://twistedmatrix.com/"),
+            method="GET",
+            uri=DecodedURL.fromText("https://twistedmatrix.com/"),
             headers=FrozenHTTPHeaders(rawHeaders=()),
             body=object(),
         )
         self.assertEqual(str(e), "body must be bytes or IFount")
```

### Comparing `klein-20.6.0/src/klein/test/test_request_compat.py` & `klein-21.8.0/src/klein/test/test_request_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,172 +1,187 @@
 # -*- test-case-name: klein.test.test_request_compat -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Tests for L{klein._irequest}.
 """
 
+import functools
 from string import ascii_uppercase
-from typing import Optional, Text
+from types import MappingProxyType
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Coroutine,
+    Mapping,
+    Sequence,
+    TypeVar,
+)
 
 from hyperlink import DecodedURL, EncodedURL
-
+from hyperlink.hypothesis import decoded_urls
 from hypothesis import given
 from hypothesis.strategies import binary, text
 
-from twisted.web.http_headers import Headers
+from twisted.internet.defer import ensureDeferred
 from twisted.web.iweb import IRequest
 
-from ._strategies import decoded_urls
-from ._trial import TestCase
-from .test_resource import requestMock
 from .._headers import IHTTPHeaders
 from .._message import FountAlreadyAccessedError
 from .._request import IHTTPRequest
 from .._request_compat import HTTPRequestWrappingIRequest
+from ._trial import TestCase
+from .test_resource import MockRequest
 
 
 __all__ = ()
 
 
+emptyMapping: Mapping[Any, Any] = MappingProxyType({})
+
+_T = TypeVar("_T")
+_R = TypeVar("_R")
+
+
+def ensuringDeferred(
+    fn: Callable[[_T], Coroutine[Any, Any, _R]]
+) -> Callable[[_T], Awaitable[_R]]:
+    @functools.wraps(fn)
+    def wrapper(self: _T) -> Awaitable[_R]:
+        return ensureDeferred(fn(self))
+
+    return wrapper
+
+
 class HTTPRequestWrappingIRequestTests(TestCase):
     """
     Tests for L{HTTPRequestWrappingIRequest}.
     """
 
     def legacyRequest(
         self,
-        path=b"/",  # type: bytes
-        method=b"GET",  # type: bytes
-        host=b"localhost",  # type: bytes
-        port=8080,  # type: int
-        isSecure=False,  # type: bool
-        body=None,  # type: Optional[bytes]
-        headers=None,  # type: Optional[Headers]
-    ):
-        # type: (...) -> IRequest
-        return requestMock(
+        path: bytes = b"/",
+        method: bytes = b"GET",
+        host: bytes = b"localhost",
+        port: int = 8080,
+        isSecure: bool = False,
+        body: bytes = b"",
+        headers: Mapping[bytes, Sequence[bytes]] = emptyMapping,
+    ) -> IRequest:
+        return MockRequest(
             path=path,
             method=method,
             host=host,
             port=port,
             isSecure=isSecure,
             body=body,
             headers=headers,
         )
 
-    def test_interface(self):
-        # type: () -> None
+    def test_interface(self) -> None:
         """
         L{HTTPRequestWrappingIRequest} implements L{IHTTPRequest}.
         """
         request = HTTPRequestWrappingIRequest(request=self.legacyRequest())
         self.assertProvides(IHTTPRequest, request)
 
     @given(text(alphabet=ascii_uppercase, min_size=1))
-    def test_method(self, methodText):
-        # type: (Text) -> None
+    def test_method(self, methodText: str) -> None:
         """
         L{HTTPRequestWrappingIRequest.method} matches the underlying legacy
         request method.
         """
         legacyRequest = self.legacyRequest(method=methodText.encode("ascii"))
         request = HTTPRequestWrappingIRequest(request=legacyRequest)
         self.assertEqual(request.method, methodText)
 
     @given(decoded_urls())
-    def test_uri(self, url):
-        # type: (DecodedURL) -> None
+    def test_uri(self, url: DecodedURL) -> None:
         """
         L{HTTPRequestWrappingIRequest.uri} matches the underlying legacy
         request URI.
         """
         uri = url.asURI()  # Normalize as (computer-friendly) URI
 
         assert uri.port is not None  # Tells mypy it's not an Optional
 
         path = (
-            uri.replace(scheme=u"", host=u"", port=None)
-            .asText()
-            .encode("ascii")
+            uri.replace(scheme="", host="", port=None).asText().encode("ascii")
         )
         legacyRequest = self.legacyRequest(
-            isSecure=(uri.scheme == u"https"),
+            isSecure=(uri.scheme == "https"),
             host=uri.host.encode("ascii"),
             port=uri.port,
             path=path,
         )
         request = HTTPRequestWrappingIRequest(request=legacyRequest)
 
         uriNormalized = uri
         requestURINormalized = request.uri.asURI()
 
         # Needed because non-equal URLs can render as the same strings
-        def strURL(url):
-            # type: (EncodedURL) -> Text
+        def strURL(url: EncodedURL) -> str:
             return (
-                u"URL(scheme={url.scheme!r}, "
-                u"userinfo={url.userinfo!r}, "
-                u"host={url.host!r}, "
-                u"port={url.port!r}, "
-                u"path={url.path!r}, "
-                u"query={url.query!r}, "
-                u"fragment={url.fragment!r}, "
-                u"rooted={url.rooted})"
+                "URL(scheme={url.scheme!r}, "
+                "userinfo={url.userinfo!r}, "
+                "host={url.host!r}, "
+                "port={url.port!r}, "
+                "path={url.path!r}, "
+                "query={url.query!r}, "
+                "fragment={url.fragment!r}, "
+                "rooted={url.rooted})"
             ).format(url=url)
 
         self.assertEqual(
             requestURINormalized,
             uriNormalized,
             "{} != {}".format(
                 strURL(requestURINormalized), strURL(uriNormalized)
             ),
         )
 
-    def test_headers(self):
-        # type: () -> None
+    def test_headers(self) -> None:
         """
         L{HTTPRequestWrappingIRequest.headers} returns an
         L{HTTPRequestWrappingIRequest} containing the underlying legacy request
         headers.
         """
         legacyRequest = self.legacyRequest()
         request = HTTPRequestWrappingIRequest(request=legacyRequest)
         self.assertProvides(IHTTPHeaders, request.headers)
 
-    def test_bodyAsFountTwice(self):
-        # type: () -> None
+    def test_bodyAsFountTwice(self) -> None:
         """
         L{HTTPRequestWrappingIRequest.bodyAsFount} raises
         L{FountAlreadyAccessedError} if called more than once.
         """
         legacyRequest = self.legacyRequest()
         request = HTTPRequestWrappingIRequest(request=legacyRequest)
         request.bodyAsFount()
         self.assertRaises(FountAlreadyAccessedError, request.bodyAsFount)
 
     @given(binary())
-    def test_bodyAsBytes(self, data):
-        # type: (bytes) -> None
+    def test_bodyAsBytes(self, data: bytes) -> None:
         """
         L{HTTPRequestWrappingIRequest.bodyAsBytes} matches the underlying
         legacy request body.
         """
         legacyRequest = self.legacyRequest(body=data)
         request = HTTPRequestWrappingIRequest(request=legacyRequest)
-        body = self.successResultOf(request.bodyAsBytes())
+        body = self.successResultOf(ensureDeferred(request.bodyAsBytes()))
 
         self.assertEqual(body, data)
 
-    def test_bodyAsBytesCached(self):
-        # type: () -> None
+    @ensuringDeferred
+    async def test_bodyAsBytesCached(self) -> None:
         """
         L{HTTPRequestWrappingIRequest.bodyAsBytes} called twice returns the
         same object both times.
         """
         data = b"some data"
         legacyRequest = self.legacyRequest(body=data)
         request = HTTPRequestWrappingIRequest(request=legacyRequest)
-        body1 = self.successResultOf(request.bodyAsBytes())
-        body2 = self.successResultOf(request.bodyAsBytes())
+        body1 = await request.bodyAsBytes()
+        body2 = await request.bodyAsBytes()
 
         self.assertIdentical(body1, body2)
```

### Comparing `klein-20.6.0/src/klein/test/test_requirer.py` & `klein-21.8.0/src/klein/test/test_requirer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,81 @@
-from typing import Iterable, List, Text, Tuple
+from typing import Iterator, Sequence, Tuple, cast
 
 from hyperlink import DecodedURL
-
 from treq.testing import StubTreq
+from zope.interface import Interface
 
+from twisted.python.components import Componentized
 from twisted.trial.unittest import SynchronousTestCase
 from twisted.web.http_headers import Headers
 from twisted.web.iweb import IRequest
 
-from zope.interface import Interface
-
 from klein import Klein, RequestComponent, RequestURL, Requirer, Response
+from klein.interfaces import IRequiredParameter
 
 
 class BadlyBehavedHeaders(Headers):
     """
     Make L{Headers} lie, and refuse to return a Host header from
     getAllRequestHeaders.
     """
 
-    def getAllRawHeaders(self):
-        # type: () -> Iterable[Tuple[bytes, List[bytes]]]
+    def getAllRawHeaders(self) -> Iterator[Tuple[bytes, Sequence[bytes]]]:
         """
         Don't return a host header.
         """
-        for key, values in super(BadlyBehavedHeaders, self).getAllRawHeaders():
+        for key, values in super().getAllRawHeaders():
             if key != b"Host":
                 yield (key, values)
 
 
 router = Klein()
 requirer = Requirer()
 
 
 @requirer.require(
-    router.route("/hello/world", methods=["GET"]), url=RequestURL()
+    router.route("/hello/world", methods=["GET"]),
+    # typing note: https://github.com/Shoobx/mypy-zope/issues/39
+    url=cast(IRequiredParameter, RequestURL()),
 )
-def requiresURL(url):
-    # type: (DecodedURL) -> Text
+def requiresURL(url: DecodedURL) -> str:
     """
     This is a route that requires a URL.
     """
-    return url.child(u"hello/ world").asText()
+    text: str = url.child("hello/ world").asText()
+    return text
 
 
 class ISample(Interface):
     """
     Interface for testing.
     """
 
 
 @requirer.prerequisite([ISample])
-def provideSample(request):
-    # type: (IRequest) -> None
+def provideSample(request: IRequest) -> None:
     """
     This requirer prerequisite installs a string as the provider of ISample.
     """
-    request.setComponent(ISample, "sample component")
+    cast(Componentized, request).setComponent(ISample, "sample component")
 
 
 @requirer.require(
     router.route("/retrieve/component", methods=["GET"]),
     component=RequestComponent(ISample),
 )
-def needsComponent(component):
-    # type: (Text) -> Text
+def needsComponent(component: str) -> str:
     """
     This route requires and returns an L{ISample}.
     """
     return component
 
 
 @requirer.require(router.route("/set/headers"))
-def someHeaders():
-    # type: () -> Response
+def someHeaders() -> Response:
     """
     Set some response attributes.
     """
     return Response(
         209,
         {"x-single-header": b"one", "x-multi-header": [b"two", b"three"]},
         "this is the response body",
@@ -85,16 +83,15 @@
 
 
 class RequireURLTests(SynchronousTestCase):
     """
     Tests for RequestURL() required parameter.
     """
 
-    def test_requiresURL(self):
-        # type: () -> None
+    def test_requiresURL(self) -> None:
         """
         When RequestURL is specified to a requirer, a DecodedURL object will be
         passed in to the decorated route.
         """
         response = self.successResultOf(
             self.successResultOf(
                 StubTreq(router.resource()).get(
@@ -103,16 +100,15 @@
             ).text()
         )
 
         self.assertEqual(
             response, "https://example.com/hello/world/hello%2F%20world"
         )
 
-    def test_requiresURLNonStandardPort(self):
-        # type: () -> None
+    def test_requiresURLNonStandardPort(self) -> None:
         """
         When RequestURL is specified to a requirer, a DecodedURL object will be
         passed in to the decorated route.
         """
         response = self.successResultOf(
             self.successResultOf(
                 StubTreq(router.resource()).get(
@@ -121,16 +117,15 @@
             ).text()
         )
 
         self.assertEqual(
             response, "http://example.com:8080/hello/world/hello%2F%20world"
         )
 
-    def test_requiresURLBadlyBehavedClient(self):
-        # type: () -> None
+    def test_requiresURLBadlyBehavedClient(self) -> None:
         """
         requiresURL will press on in the face of badly-behaved client code.
         """
         response = self.successResultOf(
             self.successResultOf(
                 StubTreq(router.resource()).get(
                     "https://example.com/hello/world",
@@ -146,16 +141,15 @@
 
 
 class RequireComponentTests(SynchronousTestCase):
     """
     Tests for RequestComponent.
     """
 
-    def test_requestComponent(self):
-        # type: () -> None
+    def test_requestComponent(self) -> None:
         """
         Test for requiring a component installed on the request.
         """
         response = self.successResultOf(
             self.successResultOf(
                 StubTreq(router.resource()).get(
                     "https://example.com/retrieve/component",
@@ -166,23 +160,24 @@
 
 
 class ResponseTests(SynchronousTestCase):
     """
     Tests for L{klein.Response}.
     """
 
-    def test_basicResponse(self):
-        # type: () -> None
+    def test_basicResponse(self) -> None:
         """
         Since methods decorated with C{@require} don't receive the request and
         can't access it to set headers and response codes, instead, they can
         return a Response object that has those attributes.
         """
         response = self.successResultOf(
-            StubTreq(router.resource()).get("https://example.com/set/headers",)
+            StubTreq(router.resource()).get(
+                "https://example.com/set/headers",
+            )
         )
         self.assertEqual(response.code, 209)
         self.assertEqual(
             response.headers.getRawHeaders(b"X-Single-Header"), [b"one"]
         )
         self.assertEqual(
             response.headers.getRawHeaders(b"X-Multi-Header"),
```

### Comparing `klein-20.6.0/src/klein/test/test_response.py` & `klein-21.8.0/src/klein/test/test_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 # -*- test-case-name: klein.test.test_response -*-
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Tests for L{klein._response}.
 """
 
-from ._trial import TestCase
-from .test_message import FrozenHTTPMessageTestsMixIn
 from .._headers import FrozenHTTPHeaders
-from .._interfaces import IHTTPMessage
+from .._imessage import IHTTPMessage
 from .._response import FrozenHTTPResponse, IHTTPResponse
+from ._trial import TestCase
+from .test_message import FrozenHTTPMessageTestsMixIn
 
 
 __all__ = ()
 
 
 class FrozenHTTPResponseTests(FrozenHTTPMessageTestsMixIn, TestCase):
     """
     Tests for L{FrozenHTTPResponse}.
     """
 
     @staticmethod
-    def responseFromBytes(data=b""):
-        # type: (bytes) -> FrozenHTTPResponse
+    def responseFromBytes(data: bytes = b"") -> FrozenHTTPResponse:
         return FrozenHTTPResponse(
-            status=200, headers=FrozenHTTPHeaders(rawHeaders=()), body=data,
+            status=200,
+            headers=FrozenHTTPHeaders(rawHeaders=()),
+            body=data,
         )
 
     @classmethod
-    def messageFromBytes(cls, data=b""):
-        # type: (bytes) -> IHTTPMessage
+    def messageFromBytes(cls, data: bytes = b"") -> IHTTPMessage:
         return cls.responseFromBytes(data)
 
-    def test_interface(self):
-        # type: () -> None
+    def test_interface(self) -> None:
         """
         L{FrozenHTTPResponse} implements L{IHTTPResponse}.
         """
         response = self.responseFromBytes()
         self.assertProvides(IHTTPResponse, response)
 
-    def test_initInvalidBodyType(self):
-        # type: () -> None
+    def test_initInvalidBodyType(self) -> None:
         """
         L{FrozenHTTPResponse} raises L{TypeError} when given a body of an
         unknown type.
         """
         e = self.assertRaises(
             TypeError,
             FrozenHTTPResponse,
```

### Comparing `klein-20.6.0/src/klein/test/test_session.py` & `klein-21.8.0/src/klein/test/test_session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,227 +1,208 @@
 """
 Tests for L{klein._session}.
 """
 
-from typing import TYPE_CHECKING
+from typing import Any, Generator, List, Tuple, Type
 
 from treq.testing import StubTreq
+from zope.interface import Interface, implementer
 
-from twisted.internet.defer import inlineCallbacks, returnValue
+from twisted.internet.defer import Deferred, inlineCallbacks
+from twisted.python.components import Componentized
 from twisted.trial.unittest import SynchronousTestCase
-
-from zope.interface import Interface, implementer
+from twisted.web.iweb import IRequest
 
 from klein import Authorization, Klein, Requirer, SessionProcurer
-from klein._typing import ifmethod
 from klein.interfaces import ISession, NoSuchSession, TooLateForCookies
 from klein.storage.memory import MemorySessionStore, declareMemoryAuthorizer
 
-if TYPE_CHECKING:  # pragma: no cover
-    from twisted.web.iweb import IRequest
-    from twisted.internet.defer import Deferred
-    from twisted.python.components import Componentized
-    from zope.interface.interfaces import IInterface
-    from typing import Tuple, List
 
-    sessions = List[ISession]
-    errors = List[NoSuchSession]
+Sessions = List[ISession]
+Errors = List[NoSuchSession]
 
 
 class ISimpleTest(Interface):
     """
     Interface for testing.
     """
 
-    @ifmethod
-    def doTest():
-        # type: () -> None
+    def doTest() -> int:
         """
         Test method.
         """
 
 
 class IDenyMe(Interface):
     """
     Interface that is never provided.
     """
 
 
 @implementer(ISimpleTest)
-class SimpleTest(object):
+class SimpleTest:
     """
     Implementation of L{ISimpleTest} for testing.
     """
 
-    def doTest(self):
-        # type: () -> int
+    def doTest(self) -> int:
         """
         Implementation of L{ISimpleTest}.  Returns 3.
         """
         return 3
 
 
 @declareMemoryAuthorizer(ISimpleTest)
-def memoryAuthorizer(interface, session, data):
-    # type: (IInterface, ISession, Componentized) -> SimpleTest
+def memoryAuthorizer(
+    interface: Type[Interface], session: ISession, data: Componentized
+) -> SimpleTest:
     """
     Authorize the ISimpleTest interface; it always works.
     """
     return SimpleTest()
 
 
-def simpleSessionRouter():
-    # type: () -> Tuple[sessions, errors, str, str, StubTreq]
+def simpleSessionRouter() -> Tuple[Sessions, Errors, str, str, StubTreq]:
     """
     Construct a simple router.
     """
-    sessions = []
-    exceptions = []
+    sessions: Sessions = []
+    exceptions: Errors = []
     mss = MemorySessionStore.fromAuthorizers([memoryAuthorizer])
     router = Klein()
     token = "X-Test-Session-Token"
     cookie = "X-Test-Session-Cookie"
     sproc = SessionProcurer(
         mss,
         secureTokenHeader=b"X-Test-Session-Token",
         secureCookie=b"X-Test-Session-Cookie",
     )
 
     @router.route("/")
     @inlineCallbacks
-    def route(request):
-        # type: (IRequest) -> Deferred
+    def route(request: IRequest) -> Generator[Any, object, bytes]:
         try:
-            sessions.append((yield sproc.procureSession(request)))
+            sessions.append(
+                (yield sproc.procureSession(request)),  # type: ignore[arg-type]
+            )
         except NoSuchSession as nss:
             exceptions.append(nss)
-        returnValue(b"ok")
+        return b"ok"
 
     requirer = Requirer()
 
     @requirer.prerequisite([ISession])
-    def procure(request):
-        # type: (IRequest) -> Deferred
+    def procure(request: IRequest) -> Deferred:
         return sproc.procureSession(request)
 
     @requirer.require(router.route("/test"), simple=Authorization(ISimpleTest))
-    def testRoute(simple):
-        # type: (SimpleTest) -> str
+    def testRoute(simple: SimpleTest) -> str:
         return "ok: " + str(simple.doTest() + 4)
 
     @requirer.require(router.route("/denied"), nope=Authorization(IDenyMe))
-    def testDenied(nope):
-        # type: (IDenyMe) -> str
+    def testDenied(nope: IDenyMe) -> str:
         return "bad"
 
     treq = StubTreq(router.resource())
     return sessions, exceptions, token, cookie, treq
 
 
 class ProcurementTests(SynchronousTestCase):
     """
     Tests for L{klein.SessionProcurer}.
     """
 
-    def test_procurementSecurity(self):
-        # type: () -> None
+    def test_procurementSecurity(self) -> None:
         """
         Once a session is negotiated, it should be the identical object to
         avoid duplicate work - unless we are using forceInsecure to retrieve
         the insecure session from a secure request, in which case the result
         should not be cached.
         """
         sessions = []
         mss = MemorySessionStore()
         router = Klein()
 
         @router.route("/")
         @inlineCallbacks
-        def route(request):
-            # type: (IRequest) -> Deferred
+        def route(request: IRequest) -> Generator[Any, object, bytes]:
             sproc = SessionProcurer(mss)
             sessions.append((yield sproc.procureSession(request)))
             sessions.append((yield sproc.procureSession(request)))
             sessions.append(
                 (yield sproc.procureSession(request, forceInsecure=True))
             )
-            returnValue(b"sessioned")
+            return b"sessioned"
 
         treq = StubTreq(router.resource())
         self.successResultOf(treq.get("http://unittest.example.com/"))
         self.assertIs(sessions[0], sessions[1])
         self.assertIs(sessions[0], sessions[2])
         self.successResultOf(treq.get("https://unittest.example.com/"))
         self.assertIs(sessions[3], sessions[4])
         self.assertIsNot(sessions[3], sessions[5])
 
-    def test_procuredTooLate(self):
-        # type: () -> None
+    def test_procuredTooLate(self) -> None:
         """
         If you start writing stuff to the response before procuring the
         session, when cookies need to be set, you will get a comprehensible
         error.
         """
         mss = MemorySessionStore()
         router = Klein()
 
-        @router.route("/")
+        @router.route("/")  # type: ignore[arg-type]
         @inlineCallbacks
-        def route(request):
-            # type: (IRequest) -> Deferred
+        def route(request: IRequest) -> Generator[Any, object, None]:
             sproc = SessionProcurer(mss)
             request.write(b"oops...")
             with self.assertRaises(TooLateForCookies):
                 yield sproc.procureSession(request)
             request.write(b"bye")
             request.finish()
 
         treq = StubTreq(router.resource())
         result = self.successResultOf(treq.get("http://unittest.example.com/"))
         self.assertEqual(self.successResultOf(result.content()), b"oops...bye")
 
-    def test_cookiesTurnedOff(self):
-        # type: () -> None
+    def test_cookiesTurnedOff(self) -> None:
         """
         If cookies can't be set, then C{procureSession} raises
         L{NoSuchSession}.
         """
         mss = MemorySessionStore()
         router = Klein()
 
         @router.route("/")
         @inlineCallbacks
-        def route(request):
-            # type: (IRequest) -> Deferred
+        def route(request: IRequest) -> Generator[Any, object, bytes]:
             sproc = SessionProcurer(mss, setCookieOnGET=False)
             with self.assertRaises(NoSuchSession):
                 yield sproc.procureSession(request)
-            returnValue(b"no session")
+            return b"no session"
 
         treq = StubTreq(router.resource())
         result = self.successResultOf(treq.get("http://unittest.example.com/"))
         self.assertEqual(self.successResultOf(result.content()), b"no session")
 
-    def test_unknownSessionHeader(self):
-        # type: () -> None
+    def test_unknownSessionHeader(self) -> None:
         """
         Unknown session IDs in auth headers will be immediately rejected with
         L{NoSuchSession}.
         """
         sessions, exceptions, token, cookie, treq = simpleSessionRouter()
 
         response = self.successResultOf(
-            treq.get("https://unittest.example.com/", headers={token: u"bad"})
+            treq.get("https://unittest.example.com/", headers={token: "bad"})
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(len(sessions), 0)
         self.assertEqual(len(exceptions), 1)
 
-    def test_unknownSessionCookieGET(self):
-        # type: () -> None
+    def test_unknownSessionCookieGET(self) -> None:
         """
         Unknown session IDs in cookies will result in a new session being
         created.
         """
         badSessionID = "bad"
         sessions, exceptions, token, cookie, treq = simpleSessionRouter()
         response = self.successResultOf(
@@ -230,16 +211,15 @@
             )
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(len(exceptions), 0)
         self.assertEqual(len(sessions), 1)
         self.assertNotEqual(sessions[0].identifier, badSessionID)
 
-    def test_unknownSessionCookiePOST(self):
-        # type: () -> None
+    def test_unknownSessionCookiePOST(self) -> None:
         """
         Unknown session IDs in cookies for POST requests will result in a
         NoSuchSession error.
         """
         badSessionID = "bad"
         sessions, exceptions, token, cookie, treq = simpleSessionRouter()
         response = self.successResultOf(
@@ -247,28 +227,26 @@
                 "https://unittest.example.com/", cookies={cookie: badSessionID}
             )
         )
         self.assertEqual(response.code, 200)
         self.assertEqual(len(exceptions), 1)
         self.assertEqual(len(sessions), 0)
 
-    def test_authorization(self):
-        # type: () -> None
+    def test_authorization(self) -> None:
         """
         When L{Requirer.require} is used with L{Authorization} and the session
         knows how to supply that authorization, it is passed to the object.
         """
         sessions, exceptions, token, cookie, treq = simpleSessionRouter()
         response = self.successResultOf(
             treq.get("https://unittest.example.com/test")
         )
         self.assertEqual(self.successResultOf(response.content()), b"ok: 7")
 
-    def test_authorizationDenied(self):
-        # type: () -> None
+    def test_authorizationDenied(self) -> None:
         """
         When L{Requirer.require} is used with an L{Authorization} and the
         session does I{not} know how to supply that authorization, the callable
         is not invoked.
         """
         sessions, exceptions, token, cookie, treq = simpleSessionRouter()
         response = self.successResultOf(
```

### Comparing `klein-20.6.0/src/klein/test/test_trial.py` & `klein-21.8.0/src/klein/test/test_trial.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright (c) 2011-2019. See LICENSE for details.
+# Copyright (c) 2011-2021. See LICENSE for details.
 
 """
 Tests for L{klein.test._trial}.
 """
 
 from zope.interface import Interface, implementer
 
 from ._trial import TestCase
-from .._typing import ifmethod
 
 
 __all__ = ()
 
 
 class TestCaseTests(TestCase):
     """
@@ -19,49 +18,44 @@
     """
 
     class IFrobbable(Interface):
         """
         Frobbable object.
         """
 
-        @ifmethod
-        def frob():
-            # type: () -> None
+        def frob() -> None:
             """
             Frob the object.
             """
 
     @implementer(IFrobbable)
-    class Frobbable(object):
+    class Frobbable:
         """
         Implements L{IFrobbable}.
         """
 
-        def frob(self):
-            # type: () -> None
+        def frob(self) -> None:
             pass
 
     @implementer(IFrobbable)
-    class NotFrobbable(object):
+    class NotFrobbable:  # type: ignore[misc]  # …intentional for test
         """
         Does not implement L{IFrobbable}, despite declaring.
         """
 
-    def test_assertProvidesPass(self):
-        # type: () -> None
+    def test_assertProvidesPass(self) -> None:
         """
         L{TestCase.assertProvides} does not raise when C{interface} is provided
         by C{obj}.
         """
         frobbable = self.Frobbable()
         self.assertProvides(self.IFrobbable, frobbable)
         frobbable.frob()  # Coverage
 
-    def test_assertProvidesFail(self):
-        # type: () -> None
+    def test_assertProvidesFail(self) -> None:
         """
         L{TestCase.assertProvides} does not raise when C{interface} is not
         provided by C{obj}.
         """
         self.assertRaises(
             self.failureException,
             self.assertProvides,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `klein-20.6.0/src/klein.egg-info/PKG-INFO` & `klein-21.8.0/src/klein.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,85 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: klein
-Version: 20.6.0
+Version: 21.8.0
 Summary: werkzeug + twisted.web
 Home-page: https://github.com/twisted/klein
-Maintainer: Amber Brown (HawkOwl)
-Maintainer-email: hawkowl@twistedmatrix.com
+Maintainer: Twisted Matrix Laboratories
+Maintainer-email: twisted-python@twistedmatrix.com
 License: MIT
-Description: ============================
-        Klein, a Web Micro-Framework
-        ============================
-        
-        .. image:: https://travis-ci.org/twisted/klein.svg?branch=master
-            :target: http://travis-ci.org/twisted/klein
-            :alt: Build Status
-        .. image:: https://codecov.io/github/twisted/klein/coverage.svg?branch=master
-            :target: https://codecov.io/github/twisted/klein?branch=master
-            :alt: Code Coverage
-        .. image:: https://requires.io/github/twisted/klein/requirements.svg?branch=master
-            :target: https://requires.io/github/twisted/klein/requirements/?branch=master
-            :alt: Requirements Status
-        .. image:: https://img.shields.io/pypi/pyversions/klein.svg
-            :target: https://pypi.python.org/pypi/klein
-            :alt: Python Version Compatibility
-        
-        Klein is a micro-framework for developing production-ready web services with Python.
-        It is 'micro' in that it has an incredibly small API similar to `Bottle <http://bottlepy.org/docs/dev/index.html>`_ and `Flask <http://flask.pocoo.org/>`_.
-        It is not 'micro' in that it depends on things outside the standard library.
-        This is primarily because it is built on widely used and well tested components like `Werkzeug <http://werkzeug.pocoo.org/>`_ and `Twisted <http://twistedmatrix.com>`_.
-        
-        A `Klein bottle <https://en.wikipedia.org/wiki/Klein_bottle>`_ is an example of a non-orientable surface, and a glass Klein bottle looks like a twisted bottle or twisted flask.
-        This, of course, made it too good of a pun to pass up.
-        
-        Klein's documentation can be found at `Read The Docs <http://klein.readthedocs.org>`_.
-        
-        
-        Example
-        =======
-        
-        This is a sample Klein application that returns 'Hello, world!', running on port ``8080``.
-        
-        .. code-block:: python
-        
-            from klein import run, route
-        
-            @route('/')
-            def home(request):
-                return 'Hello, world!'
-        
-            run("localhost", 8080)
-        
-        
-        Contribute
-        ==========
-        
-        ``klein`` is hosted on `GitHub <http://github.com/twisted/klein>`_ and is an open source project that welcomes contributions of all kinds from the community, including:
-        
-        - code patches,
-        - `documentation <http://klein.readthedocs.org/>`_ improvements,
-        - `bug reports <https://github.com/twisted/klein/issues>`_,
-        - reviews for `contributed patches <https://github.com/twisted/klein/pulls>`_.
-        
-        For more information about contributing, see `the contributor guidelines <https://github.com/twisted/klein/tree/master/CONTRIBUTING.rst>`_.
-        
 Keywords: twisted flask werkzeug web
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
+============================
+Klein, a Web Micro-Framework
+============================
+
+.. image:: https://github.com/twisted/klein/workflows/CI%2fCD/badge.svg
+    :target: https://github.com/twisted/klein/actions
+    :alt: Build Status
+.. image:: https://codecov.io/github/twisted/klein/coverage.svg?branch=master
+    :target: https://codecov.io/github/twisted/klein?branch=master
+    :alt: Code Coverage
+.. image:: https://requires.io/github/twisted/klein/requirements.svg?branch=master
+    :target: https://requires.io/github/twisted/klein/requirements/?branch=master
+    :alt: Requirements Status
+.. image:: https://img.shields.io/pypi/pyversions/klein.svg
+    :target: https://pypi.org/project/klein
+    :alt: Python Version Compatibility
+
+Klein is a micro-framework for developing production-ready web services with Python.
+It is 'micro' in that it has an incredibly small API similar to `Bottle <https://bottlepy.org/docs/dev/index.html>`_ and `Flask <https://flask.palletsprojects.com/>`_.
+It is not 'micro' in that it depends on things outside the standard library.
+This is primarily because it is built on widely used and well tested components like `Werkzeug <https://werkzeug.palletsprojects.com/>`_ and `Twisted <https://twistedmatrix.com>`_.
+
+A `Klein bottle <https://en.wikipedia.org/wiki/Klein_bottle>`_ is an example of a non-orientable surface, and a glass Klein bottle looks like a twisted bottle or twisted flask.
+This, of course, made it too good of a pun to pass up.
+
+Klein's documentation can be found at `Read The Docs <https://klein.readthedocs.org>`_.
+
+
+Example
+========
+
+This is a sample Klein application that returns 'Hello, world!', running on port ``8080``.
+
+.. code-block:: python
+
+    from klein import run, route
+
+    @route('/')
+    def home(request):
+        return 'Hello, world!'
+
+    run("localhost", 8080)
+
+
+Contribute
+==========
+
+``klein`` is hosted on `GitHub <https://github.com/twisted/klein>`_ and is an open source project that welcomes contributions of all kinds from the community, including:
+
+- code patches,
+- `documentation <https://klein.readthedocs.org/>`_ improvements,
+- `bug reports <https://github.com/twisted/klein/issues>`_,
+- reviews for `contributed patches <https://github.com/twisted/klein/pulls>`_.
+
+For more information about contributing, see `the contributor guidelines <https://github.com/twisted/klein/tree/master/CONTRIBUTING.rst>`_.
+
+
```

### Comparing `klein-20.6.0/src/klein.egg-info/SOURCES.txt` & `klein-21.8.0/src/klein.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+.codecov.yml
 .coveragerc
+.flake8
+.isort.cfg
+.pre-commit-config.yaml
+.readthedocs.yml
 AUTHORS
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 NEWS.rst
 README.rst
+mypy.ini
 pyproject.toml
+release.py
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
@@ -43,46 +50,42 @@
 src/klein/__init__.py
 src/klein/_app.py
 src/klein/_decorators.py
 src/klein/_dihttp.py
 src/klein/_form.py
 src/klein/_headers.py
 src/klein/_headers_compat.py
-src/klein/_iapp.py
 src/klein/_iform.py
 src/klein/_imessage.py
 src/klein/_interfaces.py
 src/klein/_isession.py
 src/klein/_message.py
 src/klein/_plating.py
 src/klein/_request.py
 src/klein/_request_compat.py
 src/klein/_requirer.py
 src/klein/_resource.py
 src/klein/_response.py
 src/klein/_session.py
 src/klein/_tubes.py
-src/klein/_typing.py
 src/klein/_version.py
 src/klein/app.py
 src/klein/interfaces.py
 src/klein/resource.py
 src/klein.egg-info/PKG-INFO
 src/klein.egg-info/SOURCES.txt
 src/klein.egg-info/dependency_links.txt
+src/klein.egg-info/not-zip-safe
 src/klein.egg-info/requires.txt
 src/klein.egg-info/top_level.txt
 src/klein/storage/__init__.py
 src/klein/storage/_memory.py
 src/klein/storage/memory.py
 src/klein/test/__init__.py
-src/klein/test/_strategies.py
 src/klein/test/_trial.py
-src/klein/test/idna-tables-properties.csv
-src/klein/test/py3_test_resource.py
 src/klein/test/test_app.py
 src/klein/test/test_exports.py
 src/klein/test/test_form.py
 src/klein/test/test_headers.py
 src/klein/test/test_headers_compat.py
 src/klein/test/test_memory.py
 src/klein/test/test_message.py
```

### Comparing `klein-20.6.0/tox.ini` & `klein-21.8.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,49 @@
 [tox]
 
 envlist =
-    flake8, black, mypy
-    coverage-py{27,35,36,37,38,py2,py3}-tw{184,192,current,trunk}
+    lint, mypy
+    coverage-py{36,37,38,39,310,py3}-tw{192,203,current,trunk}
     coverage_report
     docs, docs-linkcheck
     packaging
 
 skip_missing_interpreters = {tty:True:False}
 
 
 [default]
 
-basepython = python3.8
+basepython = python3.9
 
 deps =
-    tw160: Twisted==16.0.0
-    tw161: Twisted==16.1.1
-    tw162: Twisted==16.2.0
-    tw163: Twisted==16.3.2
-    tw164: Twisted==16.4.1
-    tw165: Twisted==16.5.0
-    tw166: Twisted==16.6.0
-    tw171: Twisted==17.1.0
-    tw175: Twisted==17.5.0
-    tw179: Twisted==17.9.0
-    tw184: Twisted==18.4.0
-    tw187: Twisted==18.7.0
-    tw189: Twisted==18.9.0
     tw192: Twisted==19.2.1
     tw197: Twisted==19.7.0
     tw1910: Twisted==19.10.0
     tw203: Twisted==20.3.0
+    tw212: Twisted==21.2.0
     twcurrent: Twisted
-    twtrunk: https://github.com/twisted/twisted/archive/trunk.zip
-
-    attrs==19.3.0
-    hyperlink==19.0.0
-    incremental==17.5.0
-    six==1.15.0
+    # See https://github.com/twisted/klein/issues/486
+    twtrunk: --use-deprecated=legacy-resolver
+    twtrunk: https://github.com/twisted/twisted/tarball/trunk#egg=Twisted
+
+    attrs==21.2.0
+    Automat==20.2.0
+    characteristic==14.3.0
+    constantly==15.1.0
+    hyperlink==21.0.0
+    incremental==21.3.0
+    PyHamcrest==2.0.2
+    six==1.16.0
     Tubes==0.2.0
-    Werkzeug==1.0.1
-    zope.interface==5.1.0
+    Werkzeug==2.0.1
+    zope.interface==5.4.0
 
-    {test,coverage}: treq==20.3.0
-    {test,coverage}-py{27,py2}: hypothesis==4.57.1
-    {test,coverage}-py{35,36,37,38,py3}: hypothesis==5.8.6
-    {test,coverage}: idna==2.8
-    {test,coverage}-py{27,py2}: mock==3.0.5  # rq.filter: <4
-    {test,coverage}-py{27,py2}: typing==3.7.4.1
+    {test,coverage}: treq==21.5.0
+    {test,coverage}: hypothesis==6.14.6
+    {test,coverage}: idna==3.2
 
     coverage: {[testenv:coverage_report]deps}
 
 setenv =
     PY_MODULE=klein
 
     PYTHONPYCACHEPREFIX={envtmpdir}/pycache
@@ -63,340 +54,185 @@
 ##
 
 [testenv]
 
 description = run tests
 
 basepython =
-    py27: python2.7
-    py35: python3.5
+    py: python
+
     py36: python3.6
     py37: python3.7
     py38: python3.8
     py39: python3.9
+    py310: python3.10
 
-    pypy2: pypy
     pypy3: pypy3
 
 deps = {[default]deps}
 
 setenv =
     {[default]setenv}
 
     coverage: COVERAGE_FILE={toxworkdir}/coverage.{envname}
+    coverage: COVERAGE_PROCESS_START={toxinidir}/.coveragerc
+
+    TRIAL_JOBS={env:TRIAL_JOBS:--jobs=2}
+    HYPOTHESIS_STORAGE_DIRECTORY={toxworkdir}/hypothesis
 
 commands =
     # Run trial without coverage
-    test: trial --random=0 --logfile="{envlogdir}/trial.log" --temp-directory="{envlogdir}/trial.d" {posargs:{env:PY_MODULE}}
+    test: trial --random=0 {env:TRIAL_JOBS} --logfile="{envlogdir}/trial.log" --temp-directory="{envlogdir}/trial.d" {posargs:{env:PY_MODULE}}
 
     # Run trial with coverage
-    coverage: coverage run --source {env:PY_MODULE} "{envdir}/bin/trial" --random=0 --logfile="{envlogdir}/trial.log" --temp-directory="{envlogdir}/trial.d" {posargs:{env:PY_MODULE}}
+    # Notes:
+    #  - Because we run tests in parallel, which uses multiple subprocesses,
+    #      we need to drop in a .pth file that causes coverage to start when
+    #      Python starts. See:
+    #      https://coverage.readthedocs.io/en/coverage-5.5/subprocess.html
+    #  - We use coverage in parallel mode, then combine here to get the results
+    #      to get a unified result for the current test environment.
+    #  - Use `tox -e coverage_report` to generate a report for all environments.
+    coverage: python -c 'f=open("{envsitepackagesdir}/zz_coverage.pth", "w"); f.write("import coverage; coverage.process_startup()\n")'
+    coverage: coverage erase
+    coverage: coverage run --source="{env:PY_MODULE}" "{envdir}/bin/trial" --random=0 {env:TRIAL_JOBS} --logfile="{envlogdir}/trial.log" --temp-directory="{envlogdir}/trial.d" {posargs:{env:PY_MODULE}}
+    coverage: coverage combine
+    coverage: coverage xml
 
     # Run coverage reports, ignore exit status
     coverage: - coverage report --skip-covered
 
 
 ##
-# Black code formatting
+# Lint
 ##
 
-[testenv:black]
+[testenv:lint]
 
-description = run Black (linter)
+description = run all linters
 
 basepython = {[default]basepython}
 
 skip_install = True
 
 deps =
-    black==19.10b0
-
-setenv =
-    BLACK_LINT_ARGS=--check
+    pre-commit==2.14.0
 
 commands =
-    black {env:BLACK_LINT_ARGS:} {posargs:release.py src}
-
-
-[testenv:black-reformat]
-
-description  = {[testenv:black]description} and reformat
-basepython   = {[testenv:black]basepython}
-skip_install = {[testenv:black]skip_install}
-deps         = {[testenv:black]deps}
-commands     = {[testenv:black]commands}
+    pre-commit run {posargs:--all-files}
 
 
 ##
-# Flake8 linting
+# Black code formatting
 ##
 
-[testenv:flake8]
+[testenv:black]
 
-description = run Flake8 (linter)
+description = run Black (linter)
 
 basepython = {[default]basepython}
 
 skip_install = True
 
 deps =
-    flake8-bugbear==20.1.4
-    flake8-docstrings==1.5.0
-    flake8-import-order==0.18.1
-    flake8-mutable==1.2.0
-    flake8-pep3101==1.3.0
-    flake8==3.8.2
-    mccabe==0.6.1
-    pep8-naming==0.10.0
-    pycodestyle==2.6.0
-    pydocstyle==5.0.2
-    # pin pyflakes pending a release with https://github.com/PyCQA/pyflakes/pull/455
-    git+git://github.com/PyCQA/pyflakes@ffe9386#egg=pyflakes
-
-commands =
-    flake8 {posargs:release.py setup.py src/{env:PY_MODULE}}
-
-
-[flake8]
-
-# !!! BRING THE PAIN !!!
-select = A,B,B9,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z
-
-show-source = True
-doctests    = True
-
-max-line-length = 80
-
-# Codes: http://flake8.pycqa.org/en/latest/user/error-codes.html
-ignore =
-    ######## WARNINGS BELOW SHOULD BE FIXED ########
-
-    # Missing docstring in public module
-    D100,
-
-    # Missing docstring in public class
-    D101,
-
-    # Missing docstring in public method
-    D102,
-
-    # Missing docstring in public function
-    D103,
-
-    # Missing docstring in public package
-    D104,
-
-    # Missing docstring in magic method
-    D105,
-
-    # Missing docstring in __init__
-    D107,
-
-    # Use """triple double quotes"""
-    D300,
-
-    # First word of the first line should be properly capitalized
-    D403,
-
-    # Additional newline in a group of imports
-    I202,
-
-    ######## WARNINGS ABOVE SHOULD BE FIXED ########
-
-    # Invalid first argument used for instance method
-    B902,
-
-    # One-line docstring should fit on one line with quotes
-    D200,
-
-    # No blank lines allowed after function docstring
-    D202,
-
-    # 1 blank line required between summary line and description
-    D205,
-
-    # First line should end with a period
-    D400,
-
-    # First line should be in imperative mood
-    D401,
-
-    # missing whitespace after ','
-    E231,
-
-    # function name should be lowercase
-    N802,
+    black==21.7b0
 
-    # argument name should be lowercase
-    N803,
-
-    # first argument of a method should be named 'self'
-    N805,
-
-    # variable in function should be lowercase
-    N806,
-
-    # lowercase imported as non lowercase
-    N812,
-
-    # variable in class scope should not be mixedCase
-    N815,
-
-    # variable in global scope should not be mixedCase
-    N816,
+setenv =
+    BLACK_LINT_ARGS=--check
 
-    # line break before binary operator
-    W503,
+commands =
+    black {env:BLACK_LINT_ARGS:} {posargs:release.py setup.py src}
 
-    # End of list (allows last item to end with trailing ',')
-    EOL
 
-# flake8-import-order: local module name space
-application-import-names = klein
+[testenv:black-reformat]
 
-# McCabe complexity checker
-max-complexity = 60
+description  = {[testenv:black]description} and reformat
+basepython   = {[testenv:black]basepython}
+skip_install = {[testenv:black]skip_install}
+deps         = {[testenv:black]deps}
+commands     = {[testenv:black]commands}
 
 
 ##
 # Mypy static type checking
 ##
 
 [testenv:mypy]
 
 description = run Mypy (static type checker)
 
 basepython = {[default]basepython}
 
 deps =
-    mypy==0.780
-    mypy_extensions==0.4.3
+    # Note: mypy-zope pins the mypy version
+    mypy==0.910
+    mypy-zope==0.3.2
+    types-click==7.1.4
 
     {[default]deps}
 
 commands =
     mypy                                       \
-        --config-file="{toxinidir}/tox.ini"    \
         --cache-dir="{toxworkdir}/mypy_cache"  \
         {tty:--pretty:}                        \
         {posargs:release.py setup.py src}
 
 
-[mypy]
-
-# Global settings
-
-disallow_untyped_defs    = True
-show_column_numbers      = True
-show_error_codes         = True
-strict_optional          = True
-warn_no_return           = True
-warn_redundant_casts     = True
-warn_unreachable         = True
-warn_unused_ignores      = True
-
-# Enable these over time
-
-check_untyped_defs       = False
-disallow_incomplete_defs = False
-no_implicit_optional     = False
-warn_return_any          = False
-
-# Disable some checks until effected files fully adopt mypy
-
-[mypy-klein._app]
-allow_untyped_defs = True
-
-[mypy-klein._decorators]
-allow_untyped_defs = True
-
-[mypy-klein._iapp]
-allow_untyped_defs = True
-
-[mypy-klein._plating]
-allow_untyped_defs = True
-
-[mypy-klein._resource]
-allow_untyped_defs = True
-
-[mypy-klein.test._trial]
-allow_untyped_defs = True
-
-[mypy-klein.test.py3_test_resource]
-allow_untyped_defs = True
-
-[mypy-klein.test.test_app]
-allow_untyped_defs = True
-
-[mypy-klein.test.test_plating]
-allow_untyped_defs = True
-
-[mypy-klein.test.test_resource]
-allow_untyped_defs = True
-
-[mypy-klein.test.util]
-allow_untyped_defs = True
-
-# Don't complain about dependencies known to lack type hints
-
-[mypy-constantly]
-ignore_missing_imports = True
-
-[mypy-git.*]
-ignore_missing_imports = True
-
-[mypy-hyperlink]
-ignore_missing_imports = True
-
-[mypy-incremental]
-ignore_missing_imports = True
-
-[mypy-zope.interface]
-[mypy-zope.interface.*]
-ignore_missing_imports = True
+##
+# pyupgrade
+##
 
-[mypy-treq]
-ignore_missing_imports = True
-[mypy-treq.*]
-ignore_missing_imports = True
+[testenv:pyupgrade]
 
-[mypy-hypothesis]
-ignore_missing_imports = True
-[mypy-hypothesis.*]
-ignore_missing_imports = True
+description = Run pyupgrade
 
-[mypy-idna]
-ignore_missing_imports = True
+basepython = {[default]basepython}
 
-[mypy-setuptools]
-ignore_missing_imports = True
+skip_install = True
+recreate = True
 
-[mypy-tubes.*]
-ignore_missing_imports = True
+deps = pyupgrade==2.23.3
 
-[mypy-twisted.*]
-ignore_missing_imports = True
+allowlist_externals =
+    find
+    xargs
+
+commands =
+    find '{toxinidir}' \
+        '!' '(' -type d '(' \
+            -name .eggs -o \
+            -name .git -o \
+            -name .tox -o \
+            -name _build -o \
+            -name dist -o \
+            -name htmlcov -o \
+            -name htmldocs \
+        ')' -prune ')' \
+        -name '*.py' \
+        -exec pyupgrade --py36-plus '\{}' ';'
 
 
 ##
 # Coverage report
 ##
 
 [testenv:coverage_report]
 
 description = generate coverage report
 
-depends = {test,coverage}-py{27,35,36,37,38,py2,py3}-tw{171,184,current,trunk}
+depends =
+    coverage-py{36,37,38,39,310,py3}-tw{1,2}{0,1,2,3,4,5,6,7,8,9}{0,1,2,3,4,5,6,7,8,9}
+    coverage-py{36,37,38,39,310,py3}-tw{current,trunk}
 
 basepython = {[default]basepython}
 
 skip_install = True
 
 deps =
-    coverage==5.1
+    coverage==5.5
 
 setenv =
     {[default]setenv}
 
     COVERAGE_FILE={toxworkdir}/coverage
 
 commands =
@@ -411,21 +247,19 @@
 
 [testenv:codecov]
 
 description = upload coverage to Codecov
 
 depends = {[coverage_report]depends}
 
-basepython = python
-
 skip_install = True
 
 deps =
     {[testenv:coverage_report]deps}
-    codecov==2.1.4
+    codecov==2.1.12
 
 passenv =
     # See https://github.com/codecov/codecov-python/blob/master/README.md#using-tox
     # And CI-specific docs:
     #   https://help.github.com/en/articles/virtual-environments-for-github-actions#default-environment-variables
     #   https://docs.travis-ci.com/user/environment-variables#default-environment-variables
     #   https://www.appveyor.com/docs/environment-variables/
@@ -433,20 +267,20 @@
     GITHUB_*
     TRAVIS TRAVIS_*
     APPVEYOR APPVEYOR_*
 
 setenv =
     {[testenv:coverage_report]setenv}
 
-    COVERAGE_XML={envlogdir}/coverage_report.xml
+    COVERAGE_XML={envlogdir}/coverage.xml
 
 commands =
     # Note documentation for CI variables in passenv above
     coverage combine
-    coverage xml --ignore-errors -o "{env:COVERAGE_XML}"
+    coverage xml -o "{env:COVERAGE_XML}"
     codecov --file="{env:COVERAGE_XML}" --env                 \
         GITHUB_REF GITHUB_COMMIT GITHUB_USER GITHUB_WORKFLOW  \
         TRAVIS_BRANCH TRAVIS_BUILD_WEB_URL                    \
         TRAVIS_COMMIT TRAVIS_COMMIT_MESSAGE                   \
         APPVEYOR_REPO_BRANCH APPVEYOR_REPO_COMMIT             \
         APPVEYOR_REPO_COMMIT_AUTHOR_EMAIL                     \
         APPVEYOR_REPO_COMMIT_MESSAGE_EXTENDED
@@ -459,16 +293,16 @@
 [testenv:docs]
 
 description = build documentation
 
 basepython = {[default]basepython}
 
 deps =
-    sphinx==3.0.4
-    sphinx_rtd_theme==0.4.3
+    Sphinx==4.1.2
+    sphinx-rtd-theme==0.5.2
 
 commands =
     sphinx-build                           \
         -b html -d "{envtmpdir}/doctrees"  \
         "{toxinidir}/docs"                 \
         "{toxinidir}/htmldocs"
 
@@ -477,30 +311,30 @@
 
 description = build documentation and rebuild automatically
 
 basepython = {[default]basepython}
 
 deps =
     {[testenv:docs]deps}
-    sphinx-autobuild==0.7.1
+    sphinx-autobuild==2021.3.14
 
 commands =
     sphinx-autobuild                       \
         -b html -d "{envtmpdir}/doctrees"  \
         --host=localhost                   \
         "{toxinidir}/docs"                 \
         "{toxinidir}/htmldocs"
 
 
 [testenv:apidocs]
 
-basepython = python3.8
+basepython = {[testenv:docs]basepython}
 
 deps =
-    git+git://github.com/twisted/pydoctor@c74016b#egg=pydoctor
+    pydoctor>=20.12.1
 
 commands =
     pydoctor                                               \
         --project-name=klein                               \
         --project-url="https://github.com/twisted/klein/"  \
         --project-base-dir="{toxinidir}"                   \
         --add-package="{toxinidir}/src/klein"              \
@@ -512,42 +346,43 @@
 # Check for broken links in documentation
 ##
 
 [testenv:docs-linkcheck]
 
 description = check for broken links in documentation
 
-basepython = {[default]basepython}
+basepython = {[testenv:docs]basepython}
 
-deps = {[testenv:docs]deps}
+deps =
+    {[testenv:docs]deps}
 
 commands =
     sphinx-build -b html -d "{envtmpdir}/doctrees" docs docs/_build/html
     sphinx-build -b linkcheck docs docs/_build/html
 
 
 ##
 # Packaging
 ##
 
 [testenv:packaging]
 
 description = check for potential packaging problems
 
+depends = {[coverage_report]depends}
+
 basepython = {[default]basepython}
 
 skip_install = True
 
 deps =
-   check-manifest==0.42
-   readme-renderer==26.0
-   twine==3.1.1
+   readme-renderer==29.0
+   twine==3.4.2
 
 commands =
-   check-manifest
    pip wheel --wheel-dir "{envtmpdir}/dist" --no-deps {toxinidir}
    twine check "{envtmpdir}/dist/"*
 
 
 ##
 # Print dependencies
 ##
@@ -557,17 +392,22 @@
 description = print dependencies
 
 basepython = {[default]basepython}
 
 recreate = true
 
 deps =
+    pipdeptree
 
 commands =
-    pip freeze
+    python -c 'print()'
+    pip freeze --exclude="{env:PY_MODULE}" --exclude=pipdeptree
+
+    python -c 'print()'
+    pipdeptree
 
 
 ##
 # Release
 ##
 
 [testenv:release]
@@ -575,17 +415,17 @@
 description = invoke tool to manage a release branch
 
 basepython = {[default]basepython}
 
 skip_install = True
 
 deps =
-    click==7.1.2
-    GitPython==3.1.0
+    click==8.0.1
+    GitPython==3.1.20
     incremental[scripts]==17.5.0
-    twine==3.1.1
+    twine==3.3.0
 
 passenv =
     SSH_AUTH_SOCK
 
 commands =
     python "{toxinidir}/release.py" {posargs}
```

