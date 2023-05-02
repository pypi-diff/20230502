# Comparing `tmp/autodocsumm-0.2.8.tar.gz` & `tmp/autodocsumm-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autodocsumm-0.2.8.tar", last modified: Tue Apr 19 11:25:43 2022, max compression
+gzip compressed data, was "autodocsumm-0.2.9.tar", last modified: Tue Aug  2 14:20:25 2022, max compression
```

## Comparing `autodocsumm-0.2.8.tar` & `autodocsumm-0.2.9.tar`

### file list

```diff
@@ -1,74 +1,17 @@
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.845777 autodocsumm-0.2.8/
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.837777 autodocsumm-0.2.8/.github/
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.837777 autodocsumm-0.2.8/.github/workflows/
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     1596 2022-04-19 11:20:00.000000 autodocsumm-0.2.8/.github/workflows/python-app.yml
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      827 2020-12-03 13:11:56.000000 autodocsumm-0.2.8/.gitignore
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      118 2021-05-09 11:10:09.000000 autodocsumm-0.2.8/.readthedocs.yml
--rw-r--r--   0 SommerP   (1000) psommer   (1000)    11357 2021-06-28 10:17:56.000000 autodocsumm-0.2.8/LICENSE
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       35 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/MANIFEST.in
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     6547 2022-04-19 11:25:43.845777 autodocsumm-0.2.8/PKG-INFO
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     4446 2022-04-18 05:56:34.000000 autodocsumm-0.2.8/README.rst
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.837777 autodocsumm-0.2.8/autodocsumm/
--rwxr-xr-x   0 SommerP   (1000) psommer   (1000)    24797 2022-04-19 11:20:05.000000 autodocsumm-0.2.8/autodocsumm/__init__.py
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.841777 autodocsumm-0.2.8/autodocsumm.egg-info/
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     6547 2022-04-19 11:25:43.000000 autodocsumm-0.2.8/autodocsumm.egg-info/PKG-INFO
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     1866 2022-04-19 11:25:43.000000 autodocsumm-0.2.8/autodocsumm.egg-info/SOURCES.txt
--rw-r--r--   0 SommerP   (1000) psommer   (1000)        1 2022-04-19 11:25:43.000000 autodocsumm-0.2.8/autodocsumm.egg-info/dependency_links.txt
--rw-r--r--   0 SommerP   (1000) psommer   (1000)        1 2020-02-13 10:10:49.000000 autodocsumm-0.2.8/autodocsumm.egg-info/not-zip-safe
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       17 2022-04-19 11:25:43.000000 autodocsumm-0.2.8/autodocsumm.egg-info/requires.txt
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       12 2022-04-19 11:25:43.000000 autodocsumm-0.2.8/autodocsumm.egg-info/top_level.txt
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      336 2021-06-28 11:16:42.000000 autodocsumm-0.2.8/conftest.py
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.841777 autodocsumm-0.2.8/docs/
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     7409 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/Makefile
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.841777 autodocsumm-0.2.8/docs/api/
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       95 2021-06-28 18:20:45.000000 autodocsumm-0.2.8/docs/api/autodocsumm.rst
--rwxr-xr-x   0 SommerP   (1000) psommer   (1000)      320 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/apigen.bash
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      750 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/call_demo.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)    13535 2021-06-28 18:29:50.000000 autodocsumm-0.2.8/docs/conf.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     4763 2021-06-28 18:21:33.000000 autodocsumm-0.2.8/docs/conf_settings.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       96 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/demo_class.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      103 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/demo_grouper.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       67 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/demo_module.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      384 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/dummy.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      384 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/dummy2.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     6227 2021-04-16 06:37:57.000000 autodocsumm-0.2.8/docs/examples.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     4903 2021-06-28 18:27:27.000000 autodocsumm-0.2.8/docs/index.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      288 2020-08-21 19:49:54.000000 autodocsumm-0.2.8/docs/inline_autoclasssumm.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       59 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/keep_data_demo.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       59 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/no_data_demo.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     8415 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/docs/objects.inv
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       66 2022-04-19 11:25:43.845777 autodocsumm-0.2.8/setup.cfg
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     1507 2022-04-19 11:20:09.000000 autodocsumm-0.2.8/setup.py
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.841777 autodocsumm-0.2.8/tests/
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.845777 autodocsumm-0.2.8/tests/test-root/
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     1135 2021-04-12 22:00:59.000000 autodocsumm-0.2.8/tests/test-root/conf.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     1971 2020-08-21 19:06:37.000000 autodocsumm-0.2.8/tests/test-root/dummy.py
-drwxr-xr-x   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 11:25:43.845777 autodocsumm-0.2.8/tests/test-root/dummy_submodule/
--rw-r--r--   0 SommerP   (1000) psommer   (1000)        0 2022-04-19 10:57:11.000000 autodocsumm-0.2.8/tests/test-root/dummy_submodule/__init__.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      153 2022-04-19 10:57:11.000000 autodocsumm-0.2.8/tests/test-root/dummy_submodule/submodule1.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      153 2022-04-19 10:57:11.000000 autodocsumm-0.2.8/tests/test-root/dummy_submodule/submodule2.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)     1354 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/tests/test-root/dummy_title.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      147 2020-12-03 13:11:56.000000 autodocsumm-0.2.8/tests/test-root/empty.py
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      456 2022-04-19 10:57:11.000000 autodocsumm-0.2.8/tests/test-root/index.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       94 2020-08-21 19:06:37.000000 autodocsumm-0.2.8/tests/test-root/test_autoclasssumm.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      127 2020-08-21 19:06:37.000000 autodocsumm-0.2.8/tests/test-root/test_autoclasssumm_inline.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      168 2020-08-21 19:06:37.000000 autodocsumm-0.2.8/tests/test-root/test_autoclasssumm_no_titles.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      206 2021-04-16 06:37:57.000000 autodocsumm-0.2.8/tests/test-root/test_autoclasssumm_nosignatures.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      196 2020-08-21 19:06:37.000000 autodocsumm-0.2.8/tests/test-root/test_autoclasssumm_some_sections.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       99 2020-08-21 19:06:37.000000 autodocsumm-0.2.8/tests/test-root/test_automodulesumm.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      211 2021-04-16 06:37:57.000000 autodocsumm-0.2.8/tests/test-root/test_automodulesumm_nosignatures.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      192 2020-08-21 19:06:37.000000 autodocsumm-0.2.8/tests/test-root/test_automodulesumm_some_sections.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       63 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/tests/test-root/test_class.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      176 2021-04-16 06:37:57.000000 autodocsumm-0.2.8/tests/test-root/test_class_nosignatures.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       91 2020-12-03 14:12:07.000000 autodocsumm-0.2.8/tests/test-root/test_class_order.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      157 2022-04-19 10:57:11.000000 autodocsumm-0.2.8/tests/test-root/test_class_submodule.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      137 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/tests/test-root/test_class_summary_only.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      133 2020-12-03 13:11:56.000000 autodocsumm-0.2.8/tests/test-root/test_empty.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      114 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/tests/test-root/test_inherited.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)       75 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/tests/test-root/test_module.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      135 2021-04-12 21:38:35.000000 autodocsumm-0.2.8/tests/test-root/test_module_no_nesting.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      187 2021-04-16 06:37:57.000000 autodocsumm-0.2.8/tests/test-root/test_module_nosignatures.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      142 2022-04-19 10:57:11.000000 autodocsumm-0.2.8/tests/test-root/test_module_submodule.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      148 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/tests/test-root/test_module_summary_only.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)      103 2020-01-14 22:03:25.000000 autodocsumm-0.2.8/tests/test-root/test_module_title.rst
--rw-r--r--   0 SommerP   (1000) psommer   (1000)    16945 2022-04-19 10:57:11.000000 autodocsumm-0.2.8/tests/test_autodocsumm.py
+drwxr-xr-x   0 bianca    (1000) bianca    (1000)        0 2022-08-02 14:20:25.646192 autodocsumm-0.2.9/
+-rw-r--r--   0 bianca    (1000) bianca    (1000)    11357 2022-08-02 14:19:59.000000 autodocsumm-0.2.9/LICENSE
+-rw-r--r--   0 bianca    (1000) bianca    (1000)       35 2022-08-02 14:19:59.000000 autodocsumm-0.2.9/MANIFEST.in
+-rw-r--r--   0 bianca    (1000) bianca    (1000)     5479 2022-08-02 14:20:25.645192 autodocsumm-0.2.9/PKG-INFO
+-rw-r--r--   0 bianca    (1000) bianca    (1000)     4460 2022-08-02 14:19:59.000000 autodocsumm-0.2.9/README.rst
+drwxr-xr-x   0 bianca    (1000) bianca    (1000)        0 2022-08-02 14:20:25.643192 autodocsumm-0.2.9/autodocsumm/
+-rwxr-xr-x   0 bianca    (1000) bianca    (1000)    24797 2022-08-02 14:19:59.000000 autodocsumm-0.2.9/autodocsumm/__init__.py
+drwxr-xr-x   0 bianca    (1000) bianca    (1000)        0 2022-08-02 14:20:25.645192 autodocsumm-0.2.9/autodocsumm.egg-info/
+-rw-r--r--   0 bianca    (1000) bianca    (1000)     5479 2022-08-02 14:20:24.000000 autodocsumm-0.2.9/autodocsumm.egg-info/PKG-INFO
+-rw-r--r--   0 bianca    (1000) bianca    (1000)      286 2022-08-02 14:20:25.000000 autodocsumm-0.2.9/autodocsumm.egg-info/SOURCES.txt
+-rw-r--r--   0 bianca    (1000) bianca    (1000)        1 2022-08-02 14:20:24.000000 autodocsumm-0.2.9/autodocsumm.egg-info/dependency_links.txt
+-rw-r--r--   0 bianca    (1000) bianca    (1000)        1 2022-08-02 14:20:24.000000 autodocsumm-0.2.9/autodocsumm.egg-info/not-zip-safe
+-rw-r--r--   0 bianca    (1000) bianca    (1000)       17 2022-08-02 14:20:25.000000 autodocsumm-0.2.9/autodocsumm.egg-info/requires.txt
+-rw-r--r--   0 bianca    (1000) bianca    (1000)       12 2022-08-02 14:20:25.000000 autodocsumm-0.2.9/autodocsumm.egg-info/top_level.txt
+-rw-r--r--   0 bianca    (1000) bianca    (1000)     1240 2022-08-02 14:19:59.000000 autodocsumm-0.2.9/pyproject.toml
+-rw-r--r--   0 bianca    (1000) bianca    (1000)       38 2022-08-02 14:20:25.646192 autodocsumm-0.2.9/setup.cfg
+-rw-r--r--   0 bianca    (1000) bianca    (1000)       38 2022-08-02 14:19:59.000000 autodocsumm-0.2.9/setup.py
```

### Comparing `autodocsumm-0.2.8/LICENSE` & `autodocsumm-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autodocsumm-0.2.8/PKG-INFO` & `autodocsumm-0.2.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,173 @@
 Metadata-Version: 2.1
 Name: autodocsumm
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extended sphinx autodoc including automatic autosummaries
 Home-page: https://github.com/Chilipp/autodocsumm
-Author: Philipp S. Sommer
-Author-email: philipp.sommer@hereon.de
+Author-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
-Description: ==============================================
-        Extending your autodoc API docs with a summary
-        ==============================================
-        
-        .. start-badges
-        
-        .. list-table::
-            :stub-columns: 1
-            :widths: 10 90
-        
-            * - docs
-              - |docs|
-            * - tests
-              - |github-action| |requires| |codecov|
-            * - package
-              - |version| |supported-versions| |supported-implementations|
-        
-        .. |docs| image:: http://readthedocs.org/projects/autodocsumm/badge/?version=latest
-            :alt: Documentation Status
-            :target: http://autodocsumm.readthedocs.io/en/latest/?badge=latest
-        
-        .. |github-action| image:: https://github.com/Chilipp/autodocsumm/workflows/Tests/badge.svg
-            :alt: Tests
-            :target: https://github.com/Chilipp/autodocsumm/actions?query=workflow%3A%22Tests%22
-        
-        .. |codecov| image:: https://codecov.io/gh/Chilipp/autodocsumm/branch/master/graph/badge.svg?token=I9wlZyhI4Y
-            :alt: Codecov
-            :target: https://codecov.io/gh/Chilipp/autodocsumm
-        
-        .. |requires| image:: https://requires.io/github/Chilipp/autodocsumm/requirements.svg?branch=master
-            :alt: Requirements Status
-            :target: https://requires.io/github/Chilipp/autodocsumm/requirements/?branch=master
-        
-        .. |version| image:: https://img.shields.io/pypi/v/autodocsumm.svg?style=flat
-            :alt: PyPI Package latest release
-            :target: https://pypi.python.org/pypi/autodocsumm
-        
-        .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/autodocsumm.svg?style=flat
-            :alt: Supported versions
-            :target: https://pypi.python.org/pypi/autodocsumm
-        
-        .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/autodocsumm.svg?style=flat
-            :alt: Supported implementations
-            :target: https://pypi.python.org/pypi/autodocsumm
-        
-        
-        .. end-badges
-        
-        Welcome! This sphinx extension provides some useful extensions to the Sphinxs
-        autodoc_ extension. Those are
-        
-        1. It creates a *Table of Contents* in the style of the autosummary_ extension
-           with methods, classes, functions and attributes
-        2. As you can include the ``__init__`` method documentation for via the
-           autoclass_content_ configuration value,
-           we provide the *autodata_content* configuration value to include
-           the documentation from the ``__call__`` method
-        3. You can exclude the string representation of specific objects. E.g. if you
-           have a large dictionary using the *not_document_data* configuration
-           value.
-        
-        See the `Documentation on Readthedocs`_ for more details.
-        
-        .. _autodoc: http://www.sphinx-doc.org/en/stable/ext/autodoc.html
-        .. _autoclass_content: http://www.sphinx-doc.org/en/stable/ext/autodoc.html#confval-autoclass_content
-        .. _autosummary: http://www.sphinx-doc.org/en/stable/ext/autosummary.html
-        .. _Documentation on Readthedocs: http://autodocsumm.readthedocs.io/en/latest/
-        
-        
-        
-        Installation
-        ============
-        Simply install it via ``pip``::
-        
-            $ pip install autodocsumm
-        
-        Or you install it via::
-        
-            $ python setup.py install
-        
-        from the `source on GitHub`_.
-        
-        
-        .. _source on GitHub: https://github.com/Chilipp/autodocsumm
-        
-        
-        Requirements
-        ============
-        The package only requires Sphinx_ to be installed. It has been tested for
-        versions higher than 1.3.
-        
-        
-        .. _Sphinx: http://www.sphinx-doc.org/en/master
-        
-        
-        Quickstart
-        ==========
-        
-        In order to activate the autodocsumm extension, you have to list it in your
-        ``conf.py``:
-        
-        .. code-block:: python
-        
-            extensions = [
-                'sphinx.ext.autodoc',
-                ...,
-                'autodocsumm',
-            ]
-        
-        Once this is done, you can use the ``:autosummary:`` option for autodoc
-        directives to generate a table at the top, e.g.:
-        
-        .. code-block:: rst
-        
-            .. automodule:: my.awesome.module
-                :autosummary:
-        
-        Optionally, you can make autodocsumm active by default for all autodoc
-        directives by adding in ``conf.py``:
-        
-        .. code-block:: python
-        
-            autodoc_default_options = {
-                'autosummary': True,
-            }
-        
-        
-        Disclaimer
-        ==========
-        Copyright 2016-2019, Philipp S. Sommer
-        
-        Copyright 2020-2021, Helmholtz-Zentrum Hereon
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-            http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-Keywords: sphinx autodoc autosummary content table
+Project-URL: homepage, https://github.com/Chilipp/autodocsumm
+Keywords: sphinx,autodoc,autosummary,content,table
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==============================================
+Extending your autodoc API docs with a summary
+==============================================
+
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+    :widths: 10 90
+
+    * - docs
+      - |docs|
+    * - tests
+      - |github-action| |requires| |codecov|
+    * - package
+      - |version| |supported-versions| |supported-implementations|
+
+.. |docs| image:: http://readthedocs.org/projects/autodocsumm/badge/?version=latest
+    :alt: Documentation Status
+    :target: http://autodocsumm.readthedocs.io/en/latest/?badge=latest
+
+.. |github-action| image:: https://github.com/Chilipp/autodocsumm/workflows/Tests/badge.svg
+    :alt: Tests
+    :target: https://github.com/Chilipp/autodocsumm/actions?query=workflow%3A%22Tests%22
+
+.. |codecov| image:: https://codecov.io/gh/Chilipp/autodocsumm/branch/master/graph/badge.svg?token=I9wlZyhI4Y
+    :alt: Codecov
+    :target: https://codecov.io/gh/Chilipp/autodocsumm
+
+.. |requires| image:: https://requires.io/github/Chilipp/autodocsumm/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/Chilipp/autodocsumm/requirements/?branch=master
+
+.. |version| image:: https://img.shields.io/pypi/v/autodocsumm.svg?style=flat
+    :alt: PyPI Package latest release
+    :target: https://pypi.python.org/pypi/autodocsumm
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/autodocsumm.svg?style=flat
+    :alt: Supported versions
+    :target: https://pypi.python.org/pypi/autodocsumm
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/autodocsumm.svg?style=flat
+    :alt: Supported implementations
+    :target: https://pypi.python.org/pypi/autodocsumm
+
+
+.. end-badges
+
+Welcome! This sphinx extension provides some useful extensions to the Sphinxs
+autodoc_ extension. Those are
+
+1. It creates a *Table of Contents* in the style of the autosummary_ extension
+   with methods, classes, functions and attributes
+2. As you can include the ``__init__`` method documentation for via the
+   autoclass_content_ configuration value,
+   we provide the *autodata_content* configuration value to include
+   the documentation from the ``__call__`` method
+3. You can exclude the string representation of specific objects. E.g. if you
+   have a large dictionary using the *not_document_data* configuration
+   value.
+
+See the `Documentation on Readthedocs`_ for more details.
+
+.. _autodoc: http://www.sphinx-doc.org/en/stable/ext/autodoc.html
+.. _autoclass_content: http://www.sphinx-doc.org/en/stable/ext/autodoc.html#confval-autoclass_content
+.. _autosummary: http://www.sphinx-doc.org/en/stable/ext/autosummary.html
+.. _Documentation on Readthedocs: http://autodocsumm.readthedocs.io/en/latest/
+
+
+
+Installation
+============
+Simply install it via ``pip``::
+
+    $ pip install autodocsumm
+
+
+Local development
+^^^^^^^^^^^^^^^^^
+
+Use ``pip`` on the `source on GitHub`_::
+
+    $ pip install .
+
+
+.. _source on GitHub: https://github.com/Chilipp/autodocsumm
+
+
+Requirements
+============
+The package only requires Sphinx_ to be installed. It has been tested for
+versions higher than 1.3.
+
+
+.. _Sphinx: http://www.sphinx-doc.org/en/master
+
+
+Quickstart
+==========
+
+In order to activate the autodocsumm extension, you have to list it in your
+``conf.py``:
+
+.. code-block:: python
+
+    extensions = [
+        'sphinx.ext.autodoc',
+        ...,
+        'autodocsumm',
+    ]
+
+Once this is done, you can use the ``:autosummary:`` option for autodoc
+directives to generate a table at the top, e.g.:
+
+.. code-block:: rst
+
+    .. automodule:: my.awesome.module
+        :autosummary:
+
+Optionally, you can make autodocsumm active by default for all autodoc
+directives by adding in ``conf.py``:
+
+.. code-block:: python
+
+    autodoc_default_options = {
+        'autosummary': True,
+    }
+
+
+Disclaimer
+==========
+Copyright 2016-2019, Philipp S. Sommer
+
+Copyright 2020-2021, Helmholtz-Zentrum Hereon
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+
```

### Comparing `autodocsumm-0.2.8/README.rst` & `autodocsumm-0.2.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -70,19 +70,21 @@
 
 Installation
 ============
 Simply install it via ``pip``::
 
     $ pip install autodocsumm
 
-Or you install it via::
 
-    $ python setup.py install
+Local development
+^^^^^^^^^^^^^^^^^
 
-from the `source on GitHub`_.
+Use ``pip`` on the `source on GitHub`_::
+
+    $ pip install .
 
 
 .. _source on GitHub: https://github.com/Chilipp/autodocsumm
 
 
 Requirements
 ============
```

### Comparing `autodocsumm-0.2.8/autodocsumm/__init__.py` & `autodocsumm-0.2.9/autodocsumm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 __license__ = "Apache-2.0"
 
 __maintainer__ = "Philipp S. Sommer"
 __email__ = "philipp.sommer@hereon.de"
 
 __status__ = "Production"
 
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 from itertools import chain
 
 from sphinx.util import logging
 import re
 
 from docutils import nodes
```

### Comparing `autodocsumm-0.2.8/autodocsumm.egg-info/PKG-INFO` & `autodocsumm-0.2.9/autodocsumm.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,173 @@
 Metadata-Version: 2.1
 Name: autodocsumm
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extended sphinx autodoc including automatic autosummaries
 Home-page: https://github.com/Chilipp/autodocsumm
-Author: Philipp S. Sommer
-Author-email: philipp.sommer@hereon.de
+Author-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
-Description: ==============================================
-        Extending your autodoc API docs with a summary
-        ==============================================
-        
-        .. start-badges
-        
-        .. list-table::
-            :stub-columns: 1
-            :widths: 10 90
-        
-            * - docs
-              - |docs|
-            * - tests
-              - |github-action| |requires| |codecov|
-            * - package
-              - |version| |supported-versions| |supported-implementations|
-        
-        .. |docs| image:: http://readthedocs.org/projects/autodocsumm/badge/?version=latest
-            :alt: Documentation Status
-            :target: http://autodocsumm.readthedocs.io/en/latest/?badge=latest
-        
-        .. |github-action| image:: https://github.com/Chilipp/autodocsumm/workflows/Tests/badge.svg
-            :alt: Tests
-            :target: https://github.com/Chilipp/autodocsumm/actions?query=workflow%3A%22Tests%22
-        
-        .. |codecov| image:: https://codecov.io/gh/Chilipp/autodocsumm/branch/master/graph/badge.svg?token=I9wlZyhI4Y
-            :alt: Codecov
-            :target: https://codecov.io/gh/Chilipp/autodocsumm
-        
-        .. |requires| image:: https://requires.io/github/Chilipp/autodocsumm/requirements.svg?branch=master
-            :alt: Requirements Status
-            :target: https://requires.io/github/Chilipp/autodocsumm/requirements/?branch=master
-        
-        .. |version| image:: https://img.shields.io/pypi/v/autodocsumm.svg?style=flat
-            :alt: PyPI Package latest release
-            :target: https://pypi.python.org/pypi/autodocsumm
-        
-        .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/autodocsumm.svg?style=flat
-            :alt: Supported versions
-            :target: https://pypi.python.org/pypi/autodocsumm
-        
-        .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/autodocsumm.svg?style=flat
-            :alt: Supported implementations
-            :target: https://pypi.python.org/pypi/autodocsumm
-        
-        
-        .. end-badges
-        
-        Welcome! This sphinx extension provides some useful extensions to the Sphinxs
-        autodoc_ extension. Those are
-        
-        1. It creates a *Table of Contents* in the style of the autosummary_ extension
-           with methods, classes, functions and attributes
-        2. As you can include the ``__init__`` method documentation for via the
-           autoclass_content_ configuration value,
-           we provide the *autodata_content* configuration value to include
-           the documentation from the ``__call__`` method
-        3. You can exclude the string representation of specific objects. E.g. if you
-           have a large dictionary using the *not_document_data* configuration
-           value.
-        
-        See the `Documentation on Readthedocs`_ for more details.
-        
-        .. _autodoc: http://www.sphinx-doc.org/en/stable/ext/autodoc.html
-        .. _autoclass_content: http://www.sphinx-doc.org/en/stable/ext/autodoc.html#confval-autoclass_content
-        .. _autosummary: http://www.sphinx-doc.org/en/stable/ext/autosummary.html
-        .. _Documentation on Readthedocs: http://autodocsumm.readthedocs.io/en/latest/
-        
-        
-        
-        Installation
-        ============
-        Simply install it via ``pip``::
-        
-            $ pip install autodocsumm
-        
-        Or you install it via::
-        
-            $ python setup.py install
-        
-        from the `source on GitHub`_.
-        
-        
-        .. _source on GitHub: https://github.com/Chilipp/autodocsumm
-        
-        
-        Requirements
-        ============
-        The package only requires Sphinx_ to be installed. It has been tested for
-        versions higher than 1.3.
-        
-        
-        .. _Sphinx: http://www.sphinx-doc.org/en/master
-        
-        
-        Quickstart
-        ==========
-        
-        In order to activate the autodocsumm extension, you have to list it in your
-        ``conf.py``:
-        
-        .. code-block:: python
-        
-            extensions = [
-                'sphinx.ext.autodoc',
-                ...,
-                'autodocsumm',
-            ]
-        
-        Once this is done, you can use the ``:autosummary:`` option for autodoc
-        directives to generate a table at the top, e.g.:
-        
-        .. code-block:: rst
-        
-            .. automodule:: my.awesome.module
-                :autosummary:
-        
-        Optionally, you can make autodocsumm active by default for all autodoc
-        directives by adding in ``conf.py``:
-        
-        .. code-block:: python
-        
-            autodoc_default_options = {
-                'autosummary': True,
-            }
-        
-        
-        Disclaimer
-        ==========
-        Copyright 2016-2019, Philipp S. Sommer
-        
-        Copyright 2020-2021, Helmholtz-Zentrum Hereon
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-            http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-Keywords: sphinx autodoc autosummary content table
+Project-URL: homepage, https://github.com/Chilipp/autodocsumm
+Keywords: sphinx,autodoc,autosummary,content,table
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==============================================
+Extending your autodoc API docs with a summary
+==============================================
+
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+    :widths: 10 90
+
+    * - docs
+      - |docs|
+    * - tests
+      - |github-action| |requires| |codecov|
+    * - package
+      - |version| |supported-versions| |supported-implementations|
+
+.. |docs| image:: http://readthedocs.org/projects/autodocsumm/badge/?version=latest
+    :alt: Documentation Status
+    :target: http://autodocsumm.readthedocs.io/en/latest/?badge=latest
+
+.. |github-action| image:: https://github.com/Chilipp/autodocsumm/workflows/Tests/badge.svg
+    :alt: Tests
+    :target: https://github.com/Chilipp/autodocsumm/actions?query=workflow%3A%22Tests%22
+
+.. |codecov| image:: https://codecov.io/gh/Chilipp/autodocsumm/branch/master/graph/badge.svg?token=I9wlZyhI4Y
+    :alt: Codecov
+    :target: https://codecov.io/gh/Chilipp/autodocsumm
+
+.. |requires| image:: https://requires.io/github/Chilipp/autodocsumm/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/Chilipp/autodocsumm/requirements/?branch=master
+
+.. |version| image:: https://img.shields.io/pypi/v/autodocsumm.svg?style=flat
+    :alt: PyPI Package latest release
+    :target: https://pypi.python.org/pypi/autodocsumm
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/autodocsumm.svg?style=flat
+    :alt: Supported versions
+    :target: https://pypi.python.org/pypi/autodocsumm
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/autodocsumm.svg?style=flat
+    :alt: Supported implementations
+    :target: https://pypi.python.org/pypi/autodocsumm
+
+
+.. end-badges
+
+Welcome! This sphinx extension provides some useful extensions to the Sphinxs
+autodoc_ extension. Those are
+
+1. It creates a *Table of Contents* in the style of the autosummary_ extension
+   with methods, classes, functions and attributes
+2. As you can include the ``__init__`` method documentation for via the
+   autoclass_content_ configuration value,
+   we provide the *autodata_content* configuration value to include
+   the documentation from the ``__call__`` method
+3. You can exclude the string representation of specific objects. E.g. if you
+   have a large dictionary using the *not_document_data* configuration
+   value.
+
+See the `Documentation on Readthedocs`_ for more details.
+
+.. _autodoc: http://www.sphinx-doc.org/en/stable/ext/autodoc.html
+.. _autoclass_content: http://www.sphinx-doc.org/en/stable/ext/autodoc.html#confval-autoclass_content
+.. _autosummary: http://www.sphinx-doc.org/en/stable/ext/autosummary.html
+.. _Documentation on Readthedocs: http://autodocsumm.readthedocs.io/en/latest/
+
+
+
+Installation
+============
+Simply install it via ``pip``::
+
+    $ pip install autodocsumm
+
+
+Local development
+^^^^^^^^^^^^^^^^^
+
+Use ``pip`` on the `source on GitHub`_::
+
+    $ pip install .
+
+
+.. _source on GitHub: https://github.com/Chilipp/autodocsumm
+
+
+Requirements
+============
+The package only requires Sphinx_ to be installed. It has been tested for
+versions higher than 1.3.
+
+
+.. _Sphinx: http://www.sphinx-doc.org/en/master
+
+
+Quickstart
+==========
+
+In order to activate the autodocsumm extension, you have to list it in your
+``conf.py``:
+
+.. code-block:: python
+
+    extensions = [
+        'sphinx.ext.autodoc',
+        ...,
+        'autodocsumm',
+    ]
+
+Once this is done, you can use the ``:autosummary:`` option for autodoc
+directives to generate a table at the top, e.g.:
+
+.. code-block:: rst
+
+    .. automodule:: my.awesome.module
+        :autosummary:
+
+Optionally, you can make autodocsumm active by default for all autodoc
+directives by adding in ``conf.py``:
+
+.. code-block:: python
+
+    autodoc_default_options = {
+        'autosummary': True,
+    }
+
+
+Disclaimer
+==========
+Copyright 2016-2019, Philipp S. Sommer
+
+Copyright 2020-2021, Helmholtz-Zentrum Hereon
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+
```

### Comparing `autodocsumm-0.2.8/setup.py` & `autodocsumm-0.2.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from setuptools import setup, find_packages
-import sys
+[build-system]
+build-backend = 'setuptools.build_meta'
+requires = ['setuptools >= 61.0']
 
-needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
-pytest_runner = ['pytest-runner'] if needs_pytest else []
+[project]
+name = 'autodocsumm'
+version = '0.2.9'
+description = 'Extended sphinx autodoc including automatic autosummaries'
+readme = 'README.rst'
+keywords = ['sphinx', 'autodoc', 'autosummary', 'content', 'table']
+urls.homepage = 'https://github.com/Chilipp/autodocsumm'
+authors = [
+    { name = 'Philipp S. Sommer', email = 'philipp.sommer@hereon.de' },
+]
+license = { text = 'Apache-2.0' }
 
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Developers',
+    'Topic :: Documentation',
+    'License :: OSI Approved :: Apache Software License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Operating System :: OS Independent',
+]
 
-def readme():
-    with open('README.rst') as f:
-        return f.read()
-
-
-setup(name='autodocsumm',
-      version='0.2.8',
-      description='Extended sphinx autodoc including automatic autosummaries',
-      long_description=readme(),
-      long_description_content_type='text/x-rst',
-      classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Documentation',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Operating System :: OS Independent',
-      ],
-      keywords='sphinx autodoc autosummary content table',
-      python_requires=">=3.6",
-      url='https://github.com/Chilipp/autodocsumm',
-      author='Philipp S. Sommer',
-      author_email='philipp.sommer@hereon.de',
-      license="Apache-2.0",
-      packages=find_packages(exclude=['docs', 'tests*', 'examples']),
-      install_requires=[
-          'Sphinx>=2.2,<5.0',
-      ],
-      setup_requires=pytest_runner,
-      tests_require=['pytest'],
-      zip_safe=False)
+requires-python = '>= 3.7'
+dependencies = [
+    'Sphinx >= 2.2, < 6.0',
+]
+
+[tool.setuptools]
+zip-safe = false
+
+[tool.setuptools.packages.find]
+namespaces = false
+exclude = ['docs', 'tests*', 'examples']
+
+[tool.pytest.ini_options]
+addopts = '-v'
```

