# Comparing `tmp/pydoctor-22.9.1.tar.gz` & `tmp/pydoctor-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoctor-22.9.1.tar", last modified: Sun Sep 18 21:39:52 2022, max compression
+gzip compressed data, was "pydoctor-23.4.0.tar", last modified: Tue May  2 21:02:32 2023, max compression
```

## Comparing `pydoctor-22.9.1.tar` & `pydoctor-23.4.0.tar`

### file list

```diff
@@ -1,332 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.098701 pydoctor-22.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     5380 2022-09-18 21:39:48.000000 pydoctor-22.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-18 21:39:48.000000 pydoctor-22.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    18037 2022-09-18 21:39:52.098701 pydoctor-22.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16713 2022-09-18 21:39:48.000000 pydoctor-22.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/docs/epytext_demo/
--rw-r--r--   0 runner    (1001) docker     (121)     5193 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/epytext_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/epytext_demo/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4954 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/epytext_demo/demo_epytext_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/docs/google_demo/
--rw-r--r--   0 runner    (1001) docker     (121)     9329 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/google_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/docs/numpy_demo/
--rw-r--r--   0 runner    (1001) docker     (121)     9516 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/numpy_demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/restructuredtext_demo/
--rw-r--r--   0 runner    (1001) docker     (121)     6840 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/restructuredtext_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/restructuredtext_demo/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5385 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/restructuredtext_demo/demo_restructuredtext_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/sample_template/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/sample_template/extra.css
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/sample_template/header.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13924 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/codedoc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6149 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7607 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/contrib.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/custom_template_demo/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/custom_template_demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/custom_template_demo/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     9284 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/customize.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/docformat/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/docformat/epytext/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/epytext/epytext_demo.rst
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/epytext.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/docformat/google/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/google/google_demo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/google-numpy.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7304 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/list-restructuredtext-support.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/docformat/numpy/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/numpy/numpy_demo.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/source/docformat/restructuredtext/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/restructuredtext/restructuredtext_demo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4909 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/docformat/restructuredtext.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3923 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/help.rst
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/publish-github-action.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4522 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/sphinx-integration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/source/transition.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.078700 pydoctor-22.9.1/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/tests/test-search.html
--rw-r--r--   0 runner    (1001) docker     (121)     9922 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/tests/test_python_igraph_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/tests/test_standard_library_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-09-18 21:39:48.000000 pydoctor-22.9.1/docs/tests/test_twisted_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18979 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/_configparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    48158 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/astbuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)    11846 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/astutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6539 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/epydoc/
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7391 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/doctest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/docutils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/epydoc/markup/
--rw-r--r--   0 runner    (1001) docker     (121)    17761 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/_napoleon.py
--rw-r--r--   0 runner    (1001) docker     (121)    42874 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/_pyval_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     8205 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    56958 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/epytext.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/google.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/plaintext.py
--rw-r--r--   0 runner    (1001) docker     (121)    20692 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/markup/restructuredtext.py
--rw-r--r--   0 runner    (1001) docker     (121)    38150 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc/sre_parse36.py
--rw-r--r--   0 runner    (1001) docker     (121)    37281 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/epydoc2stan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)     6562 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6501 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/extensions/attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6781 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/extensions/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (121)    14017 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/extensions/zopeinterface.py
--rw-r--r--   0 runner    (1001) docker     (121)     3643 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    19310 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/linker.py
--rw-r--r--   0 runner    (1001) docker     (121)    55454 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4302 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/mro.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/napoleon/
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/napoleon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    59464 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/napoleon/docstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/napoleon/iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)    11608 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/node2stan.py
--rw-r--r--   0 runner    (1001) docker     (121)    19315 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/qnmatch.py
--rw-r--r--   0 runner    (1001) docker     (121)    12913 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/sphinx_ext/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/sphinx_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5608 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/sphinx_ext/build_apidocs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/stanutils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/templatewriter/
--rw-r--r--   0 runner    (1001) docker     (121)    16987 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor/templatewriter/pages/
--rw-r--r--   0 runner    (1001) docker     (121)    19937 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/pages/attributechild.py
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/pages/functionchild.py
--rw-r--r--   0 runner    (1001) docker     (121)    16408 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/pages/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/pages/table.py
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/search.py
--rw-r--r--   0 runner    (1001) docker     (121)    12066 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     7627 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     6010 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/templatewriter/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.086701 pydoctor-22.9.1/pydoctor/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.086701 pydoctor-22.9.1/pydoctor/test/epydoc/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5220 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/epytext.doctest
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/restructuredtext.doctest
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/test_epytext.py
--rw-r--r--   0 runner    (1001) docker     (121)    11254 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/test_epytext2html.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/test_epytext2node.py
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/test_google_numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/test_parsed_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)    40603 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/test_pyval_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)    11648 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/epydoc/test_restructuredtext.py
--rw-r--r--   0 runner    (1001) docker     (121)    69930 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_astbuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3509 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_colorize.py
--rw-r--r--   0 runner    (1001) docker     (121)     8304 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_commandline.py
--rw-r--r--   0 runner    (1001) docker     (121)    25534 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_configparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_cyclic_imports_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    56753 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_epydoc2stan.py
--rw-r--r--   0 runner    (1001) docker     (121)    14986 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8883 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_mro.py
--rw-r--r--   0 runner    (1001) docker     (121)    85527 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_napoleon_docstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    11945 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_napoleon_iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4559 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_node2stan.py
--rw-r--r--   0 runner    (1001) docker     (121)     9007 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     7016 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_qnmatch.py
--rw-r--r--   0 runner    (1001) docker     (121)    22015 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (121)    28766 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_templatewriter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_twisted_python_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (121)    15931 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_type_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    19793 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/test_zopeinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.086701 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/allok/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/allok/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/allok/pydoctor.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/casing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.086701 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/casing/test1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/casing/test1/nav.HTML
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.086701 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/casing/test2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/casing/test2/nav.Html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.086701 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/casing/test3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/casing/test3/nav.htmL
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/header.html
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/pydoctor.js
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/random.html
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/subheader.html
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/summary.html
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/table.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/foo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/atemplate.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/static/fonts/bar.svg
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/static/fonts/foo.svg
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/static/info.svg
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testcustomtemplates/subfolders/static/lol.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.074700 pydoctor-22.9.1/pydoctor/test/testpackages/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/allgames/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/allgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/allgames/mod1.py
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/allgames/mod2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/basic/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/basic/_private_mod.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/basic/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/codeininit/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/codeininit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports/a.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports/b.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/a.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/cyclic_imports_base_classes/b.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/importingfrompackage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/importingfrompackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/importingfrompackage/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/importingfrompackage/subpack/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/importingfrompackage/subpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/importingfrompackage/subpack/submod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceallgames/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceallgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceallgames/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceallgames/implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceallgames/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceclass/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/interfaceclass/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/liveobject/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/liveobject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/liveobject/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/modnamedafterbuiltin/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/multipleinheritance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/multipleinheritance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/multipleinheritance/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/nestedconfusion/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/nestedconfusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/nestedconfusion/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/package_module_name_clash/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/package_module_name_clash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.090700 pydoctor-22.9.1/pydoctor/test/testpackages/package_module_name_clash/pack/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/package_module_name_clash/pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/package_module_name_clash/pack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/test/testpackages/relativeimporttest/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/relativeimporttest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/relativeimporttest/mod1.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/relativeimporttest/mod2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/test/testpackages/reparented_module/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparented_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparented_module/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_crash/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_crash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_crash/reparenting_crash.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_crash_alt/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_crash_alt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_crash_alt/_impl.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_crash_alt/reparenting_crash_alt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/_myotherthing.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/_mything.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/reparenting_follows_aliases/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/test/testpackages/report_trigger/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/report_trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/report_trigger/report_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/test/testpackages/syntax_error/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/test/testpackages/syntax_error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/themes/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/themes/base/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/ajax.js
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/all-documents.html
--rw-r--r--   0 runner    (1001) docker     (121)    22015 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/apidocs.css
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/attribute-child.html
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/common.html
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/themes/base/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/fonts/info.svg
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/fonts/x-circle.svg
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/function-child.html
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/head.html
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/header.html
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/index.html
--rw-r--r--   0 runner    (1001) docker     (121)   113673 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/lunr.js
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/nameIndex.html
--rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/pydoctor.js
--rw-r--r--   0 runner    (1001) docker     (121)    14604 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/search.js
--rw-r--r--   0 runner    (1001) docker     (121)    13916 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/searchlib.js
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/sidebar-list.html
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/sidebartoggle.js
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/subheader.html
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/summary.html
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/base/table.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.094700 pydoctor-22.9.1/pydoctor/themes/classic/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/classic/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (121)   117305 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/classic/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/classic/head.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.098701 pydoctor-22.9.1/pydoctor/themes/readthedocs/
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/common.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.098701 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    67312 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    66444 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/book.svg
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/home.svg
--rw-r--r--   0 runner    (1001) docker     (121)   184912 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   182708 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/minus-square-o.svg
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/plus-square-o.svg
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/head.html
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/themes/readthedocs/readthedocstheme.css
--rw-r--r--   0 runner    (1001) docker     (121)     3495 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10818 2022-09-18 21:39:48.000000 pydoctor-22.9.1/pydoctor/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 21:39:52.082700 pydoctor-22.9.1/pydoctor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18037 2022-09-18 21:39:52.000000 pydoctor-22.9.1/pydoctor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10597 2022-09-18 21:39:52.000000 pydoctor-22.9.1/pydoctor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 21:39:52.000000 pydoctor-22.9.1/pydoctor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-18 21:39:52.000000 pydoctor-22.9.1/pydoctor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-09-18 21:39:52.000000 pydoctor-22.9.1/pydoctor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-18 21:39:52.000000 pydoctor-22.9.1/pydoctor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-09-18 21:39:52.098701 pydoctor-22.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-09-18 21:39:48.000000 pydoctor-22.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.227754 pydoctor-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-02 21:02:21.000000 pydoctor-23.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 21:02:21.000000 pydoctor-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-05-02 21:02:32.227754 pydoctor-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-02 21:02:21.000000 pydoctor-23.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/epytext_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/epytext_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/epytext_demo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/epytext_demo/demo_epytext_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/google_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/google_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/numpy_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/numpy_demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/restructuredtext_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/restructuredtext_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/restructuredtext_demo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/restructuredtext_demo/demo_restructuredtext_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/sample_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/sample_template/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/sample_template/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.191754 pydoctor-23.4.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/codedoc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/contrib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.195754 pydoctor-23.4.0/docs/source/custom_template_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/custom_template_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/custom_template_demo/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/customize.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.195754 pydoctor-23.4.0/docs/source/docformat/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/epytext.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.195754 pydoctor-23.4.0/docs/source/docformat/epytext_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/epytext_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/google-numpy.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.195754 pydoctor-23.4.0/docs/source/docformat/google_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/google_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/list-restructuredtext-support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.195754 pydoctor-23.4.0/docs/source/docformat/numpy_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/numpy_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/restructuredtext.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.195754 pydoctor-23.4.0/docs/source/docformat/restructuredtext_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/docformat/restructuredtext_demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/publish-github-action.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/sphinx-integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/source/transition.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.195754 pydoctor-23.4.0/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/tests/test-search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/tests/test_python_igraph_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/tests/test_standard_library_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-02 21:02:21.000000 pydoctor-23.4.0/docs/tests/test_twisted_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.199754 pydoctor-23.4.0/pydoctor/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50698 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/astbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/astutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.199754 pydoctor-23.4.0/pydoctor/epydoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/docutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.203754 pydoctor-23.4.0/pydoctor/epydoc/markup/
+-rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/_napoleon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43757 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/_pyval_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56006 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/epytext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/plaintext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/markup/restructuredtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/sre_constants36.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc/sre_parse36.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/epydoc2stan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.203754 pydoctor-23.4.0/pydoctor/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/extensions/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/extensions/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/extensions/zopeinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60628 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/mro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.203754 pydoctor-23.4.0/pydoctor/napoleon/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/napoleon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59464 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/napoleon/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/napoleon/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/node2stan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/qnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.203754 pydoctor-23.4.0/pydoctor/sphinx_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/sphinx_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/sphinx_ext/build_apidocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/stanutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.203754 pydoctor-23.4.0/pydoctor/templatewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.203754 pydoctor-23.4.0/pydoctor/templatewriter/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/pages/attributechild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/pages/functionchild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/pages/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/pages/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/templatewriter/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.207754 pydoctor-23.4.0/pydoctor/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.207754 pydoctor-23.4.0/pydoctor/test/epydoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/epytext.doctest
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/restructuredtext.doctest
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/test_epytext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/test_epytext2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/test_epytext2node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/test_google_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/test_parsed_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41723 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/test_pyval_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/epydoc/test_restructuredtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79854 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_astbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_commandline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_cyclic_imports_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59584 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_epydoc2stan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_mro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85527 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_napoleon_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_napoleon_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_node2stan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_qnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29820 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_templatewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_twisted_python_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_type_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/test_zopeinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.187754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.207754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/allok/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/allok/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/allok/pydoctor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.187754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/casing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.207754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/casing/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/casing/test1/nav.HTML
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.207754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/casing/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/casing/test2/nav.Html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.207754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/casing/test3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/casing/test3/nav.htmL
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/pydoctor.js
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/random.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/subheader.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.187754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/overridesubfolders/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.187754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/overridesubfolders/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/overridesubfolders/static/fonts/foo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/atemplate.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/static/fonts/bar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/static/fonts/foo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/static/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testcustomtemplates/subfolders/static/lol.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.187754 pydoctor-23.4.0/pydoctor/test/testpackages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testpackages/allgames/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/allgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/allgames/mod1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/allgames/mod2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testpackages/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/basic/_private_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/basic/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_invalid_text_signature/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_invalid_text_signature/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.211754 pydoctor-23.4.0/pydoctor/test/testpackages/codeininit/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/codeininit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports/b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports_base_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports_base_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports_base_classes/a.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/cyclic_imports_base_classes/b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/importingfrompackage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/importingfrompackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/importingfrompackage/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/importingfrompackage/subpack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/importingfrompackage/subpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/importingfrompackage/subpack/submod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceallgames/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceallgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceallgames/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceallgames/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceallgames/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceclass/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/interfaceclass/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/liveobject/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/liveobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/liveobject/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/modnamedafterbuiltin/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/modnamedafterbuiltin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/modnamedafterbuiltin/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/modnamedafterbuiltin/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/multipleinheritance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/multipleinheritance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/multipleinheritance/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/nestedconfusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/nestedconfusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/nestedconfusion/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/package_module_name_clash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/package_module_name_clash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/package_module_name_clash/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/package_module_name_clash/pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/package_module_name_clash/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.215754 pydoctor-23.4.0/pydoctor/test/testpackages/relativeimporttest/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/relativeimporttest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/relativeimporttest/mod1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/relativeimporttest/mod2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.219754 pydoctor-23.4.0/pydoctor/test/testpackages/reparented_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparented_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparented_module/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.219754 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_crash/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_crash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_crash/reparenting_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.219754 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_crash_alt/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_crash_alt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_crash_alt/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_crash_alt/reparenting_crash_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.219754 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_follows_aliases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_follows_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_follows_aliases/_myotherthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_follows_aliases/_mything.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/reparenting_follows_aliases/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.219754 pydoctor-23.4.0/pydoctor/test/testpackages/report_trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/report_trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/report_trigger/report_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.219754 pydoctor-23.4.0/pydoctor/test/testpackages/syntax_error/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/test/testpackages/syntax_error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.219754 pydoctor-23.4.0/pydoctor/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.223754 pydoctor-23.4.0/pydoctor/themes/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/all-documents.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/apidocs.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/attribute-child.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/common.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.223754 pydoctor-23.4.0/pydoctor/themes/base/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/fonts/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/fonts/x-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/function-child.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   113673 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/lunr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/nameIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/pydoctor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/searchlib.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/sidebar-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/sidebartoggle.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/subheader.html
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/base/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.223754 pydoctor-23.4.0/pydoctor/themes/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/classic/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)   117305 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/classic/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/classic/head.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.223754 pydoctor-23.4.0/pydoctor/themes/readthedocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/common.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.223754 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/minus-square-o.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/plus-square-o.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16297 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/themes/readthedocs/readthedocstheme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-05-02 21:02:21.000000 pydoctor-23.4.0/pydoctor/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:32.199754 pydoctor-23.4.0/pydoctor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-05-02 21:02:32.000000 pydoctor-23.4.0/pydoctor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-05-02 21:02:32.000000 pydoctor-23.4.0/pydoctor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:02:32.000000 pydoctor-23.4.0/pydoctor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 21:02:32.000000 pydoctor-23.4.0/pydoctor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-02 21:02:32.000000 pydoctor-23.4.0/pydoctor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 21:02:32.000000 pydoctor-23.4.0/pydoctor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-02 21:02:32.227754 pydoctor-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-02 21:02:21.000000 pydoctor-23.4.0/setup.py
```

### Comparing `pydoctor-22.9.1/LICENSE.txt` & `pydoctor-23.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/PKG-INFO` & `pydoctor-23.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoctor
-Version: 22.9.1
+Version: 23.4.0
 Summary: API doc generator.
 Home-page: https://github.com/twisted/pydoctor
 Author: Michael Hudson-Doyle
 Author-email: micahel@gmail.com
 Maintainer: Maarten ter Huurne
 Maintainer-email: maarten@boxingbeetle.com
 License: MIT/X11
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
@@ -34,16 +35,16 @@
 
 pydoctor
 --------
 
 .. image:: https://img.shields.io/pypi/pyversions/pydoctor.svg
   :target: https://pypi.python.org/pypi/pydoctor
 
-.. image:: https://travis-ci.org/twisted/pydoctor.svg?branch=tox-travis-2
-  :target: https://travis-ci.org/twisted/pydoctor
+.. image:: https://github.com/twisted/pydoctor/actions/workflows/unit.yaml/badge.svg
+  :target: https://github.com/twisted/pydoctor/actions/workflows/unit.yaml
 
 .. image:: https://codecov.io/gh/twisted/pydoctor/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/twisted/pydoctor
 
 .. image:: https://img.shields.io/badge/-documentation-blue
   :target: https://pydoctor.readthedocs.io/
 
@@ -103,16 +104,35 @@
 __ https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard
 
 You can select a different format using the ``--docformat`` option or the ``__docformat__`` module variable. 
 
 What's New?
 ~~~~~~~~~~~
 
-in development
-^^^^^^^^^^^^^^
+pydoctor 23.4.0
+^^^^^^^^^^^^^^^
+
+* Add support for Python 3.11
+* Add support for the ``@overload`` decorator.
+* Show type annotations in function's signatures.
+* If none of a function's parameters have documentation, do not render the parameter table.
+* Themes have been adjusted to render annotations more concisely.
+* Fix a rare crash in the type inference. 
+  Invalid python code like a set of lists would raise a uncaught TypeError in the evaluation.
+* Support when source path lies outside base directory (``--project-base-dir``).
+  Since pydoctor support generating docs for multiple packages, 
+  it is not certain that all of the source is even viewable below a single URL. 
+  We now allow to add arbitrary paths to the system, 
+  but only the objects inside a module wich path is relative to
+  the base directory can have a source control link generated.
+* Cache the default docutils settings on docutils>=0.19 to improve performance.
+* Improve the search bar user experience by automatically appending wildcard to each query terms
+  when no terms already contain a wildcard. 
+* Link recognized constructors in class page.
+* An invalid epytext docstring will be rederered as plaintext, just like invalid restructuredtext docstrings (finally).
 
 pydoctor 22.9.1
 ^^^^^^^^^^^^^^^
 * ``pydoctor --help`` works again.
 
 pydoctor 22.9.0
 ^^^^^^^^^^^^^^^
```

### Comparing `pydoctor-22.9.1/README.rst` & `pydoctor-23.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pydoctor
 --------
 
 .. image:: https://img.shields.io/pypi/pyversions/pydoctor.svg
   :target: https://pypi.python.org/pypi/pydoctor
 
-.. image:: https://travis-ci.org/twisted/pydoctor.svg?branch=tox-travis-2
-  :target: https://travis-ci.org/twisted/pydoctor
+.. image:: https://github.com/twisted/pydoctor/actions/workflows/unit.yaml/badge.svg
+  :target: https://github.com/twisted/pydoctor/actions/workflows/unit.yaml
 
 .. image:: https://codecov.io/gh/twisted/pydoctor/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/twisted/pydoctor
 
 .. image:: https://img.shields.io/badge/-documentation-blue
   :target: https://pydoctor.readthedocs.io/
 
@@ -69,16 +69,35 @@
 __ https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard
 
 You can select a different format using the ``--docformat`` option or the ``__docformat__`` module variable. 
 
 What's New?
 ~~~~~~~~~~~
 
-in development
-^^^^^^^^^^^^^^
+pydoctor 23.4.0
+^^^^^^^^^^^^^^^
+
+* Add support for Python 3.11
+* Add support for the ``@overload`` decorator.
+* Show type annotations in function's signatures.
+* If none of a function's parameters have documentation, do not render the parameter table.
+* Themes have been adjusted to render annotations more concisely.
+* Fix a rare crash in the type inference. 
+  Invalid python code like a set of lists would raise a uncaught TypeError in the evaluation.
+* Support when source path lies outside base directory (``--project-base-dir``).
+  Since pydoctor support generating docs for multiple packages, 
+  it is not certain that all of the source is even viewable below a single URL. 
+  We now allow to add arbitrary paths to the system, 
+  but only the objects inside a module wich path is relative to
+  the base directory can have a source control link generated.
+* Cache the default docutils settings on docutils>=0.19 to improve performance.
+* Improve the search bar user experience by automatically appending wildcard to each query terms
+  when no terms already contain a wildcard. 
+* Link recognized constructors in class page.
+* An invalid epytext docstring will be rederered as plaintext, just like invalid restructuredtext docstrings (finally).
 
 pydoctor 22.9.1
 ^^^^^^^^^^^^^^^
 * ``pydoctor --help`` works again.
 
 pydoctor 22.9.0
 ^^^^^^^^^^^^^^^
```

### Comparing `pydoctor-22.9.1/docs/Makefile` & `pydoctor-23.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/epytext_demo/__init__.py` & `pydoctor-23.4.0/docs/epytext_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/epytext_demo/constants.py` & `pydoctor-23.4.0/docs/epytext_demo/constants.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/epytext_demo/demo_epytext_module.py` & `pydoctor-23.4.0/docs/epytext_demo/demo_epytext_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This is a module demonstrating epydoc code documentation features.
 
 Most part of this documentation is using Python type hinting.
 """
 
 from abc import ABC
 import math
-from typing import AnyStr, Dict, Generator, List, Union, Callable, Tuple, TYPE_CHECKING
+from typing import overload, AnyStr, Dict, Generator, List, Union, Callable, Tuple, TYPE_CHECKING
 from somelib import SomeInterface
 import zope.interface
 import zope.schema
 from typing import Sequence, Optional
 from incremental import Version
 from twisted.python.deprecate import deprecated, deprecatedProperty
 
@@ -77,14 +77,34 @@
 
     If you wish to use the name of the Python object as the text for the link, you can simply write C{LE{lb}objectE{rb}}.
 
         - L{demo_typing_arguments}
         - L{Custom name <demo_typing_arguments>}
     """
 
+@overload
+def demo_overload(s: str) -> str:
+    ...
+
+@overload
+def demo_overload(s: bytes) -> bytes:
+    ...
+
+def demo_overload(s: Union[str, bytes]) -> Union[str, bytes]:
+    """
+    Overload signatures appear without the main signature and with C{@overload} decorator.
+
+    @param s: Some string or bytes param.
+    @return: Some string or bytes result.
+    """
+    raise NotImplementedError
+
+def demo_undocumented(s: str) -> str:
+    raise NotImplementedError
+
 
 class _PrivateClass:
     """
     This is the docstring of a private class.
     """
 
     def method_inside_private(self) -> bool:
```

### Comparing `pydoctor-22.9.1/docs/google_demo/__init__.py` & `pydoctor-23.4.0/docs/google_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/make.bat` & `pydoctor-23.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/numpy_demo/__init__.py` & `pydoctor-23.4.0/docs/numpy_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/restructuredtext_demo/__init__.py` & `pydoctor-23.4.0/docs/restructuredtext_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/restructuredtext_demo/constants.py` & `pydoctor-23.4.0/docs/restructuredtext_demo/constants.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/restructuredtext_demo/demo_restructuredtext_module.py` & `pydoctor-23.4.0/docs/restructuredtext_demo/demo_restructuredtext_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Most part of this documentation is using Python type hinting.
 """
 from abc import ABC
 from ast import Tuple
 import math
 import zope.interface
 import zope.schema
-from typing import Callable, Sequence, Optional, AnyStr, Generator, Union, List, Dict, TYPE_CHECKING
+from typing import overload, Callable, Sequence, Optional, AnyStr, Generator, Union, List, Dict, TYPE_CHECKING
 from incremental import Version
 from twisted.python.deprecate import deprecated, deprecatedProperty
 
 if TYPE_CHECKING:
     from typing_extensions import Final
 
 Parser = Callable[[str], Tuple[int, bytes, bytes]]
@@ -85,14 +85,33 @@
     'text' is the text that should be displayed for the link, and 'object' is the name of the Python object that should be linked to.
 
     If you wish to use the name of the Python object as the text for the link, you can simply write ```object``` -> `object`.
 
     - `demo_typing_arguments`
     """
 
+@overload
+def demo_overload(s: str) -> str:
+    ...
+
+@overload
+def demo_overload(s: bytes) -> bytes:
+    ...
+
+def demo_overload(s: Union[str, bytes]) -> Union[str, bytes]:
+    """
+    Overload signatures appear without the main signature and with ``@overload`` decorator.
+
+    :param s: Some string or bytes param.
+    :return: Some string or bytes result.
+    """
+    raise NotImplementedError
+
+def demo_undocumented(s: str) -> str:
+    raise NotImplementedError
 
 
 class _PrivateClass:
     """
     This is the docstring of a private class.
     """
```

### Comparing `pydoctor-22.9.1/docs/sample_template/header.html` & `pydoctor-23.4.0/docs/sample_template/header.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/codedoc.rst` & `pydoctor-23.4.0/docs/source/codedoc.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/conf.py` & `pydoctor-23.4.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,44 +111,44 @@
         f'--project-version={version}',
         f'--template-dir={_pydoctor_root}/docs/sample_template',
         f'{_pydoctor_root}/pydoctor',
         ] + _common_args + 
             [f'--config={_pydoctor_root}/docs/source/custom_template_demo/pyproject.toml',
               '-qqq' ], # we don't want to hear any warnings from this custom template demo.
     'epydoc_demo': [
-        '--html-output={outdir}/docformat/epytext',
+        '--html-output={outdir}/docformat/epytext_demo',
         '--project-name=pydoctor-epytext-demo',
         '--project-version=1.3.0',
         '--docformat=epytext',
         '--sidebar-toc-depth=3',
         '--project-url=../epytext.html',
         '--theme=readthedocs',
         f'{_pydoctor_root}/docs/epytext_demo',
         ] + _common_args,
     'restructuredtext_demo': [
-        '--html-output={outdir}/docformat/restructuredtext',
+        '--html-output={outdir}/docformat/restructuredtext_demo',
         '--project-name=pydoctor-restructuredtext-demo',
         '--project-version=1.0.0',
         '--docformat=restructuredtext',
         '--sidebar-toc-depth=3',
         '--project-url=../restructuredtext.html',
         '--process-types',
         f'{_pydoctor_root}/docs/restructuredtext_demo',
         ] + _common_args,
     'numpy_demo': [ # no need to pass --docformat here, we use __docformat__
-        '--html-output={outdir}/docformat/numpy',
+        '--html-output={outdir}/docformat/numpy_demo',
         '--project-name=pydoctor-numpy-style-demo',
         '--project-version=1.0.0',
         '--project-url=../google-numpy.html',
         '--theme=readthedocs',
         f'{_pydoctor_root}/docs/numpy_demo',
         f'{_pydoctor_root}/pydoctor/napoleon'
         ] + _common_args,
     'google_demo': [
-        '--html-output={outdir}/docformat/google',
+        '--html-output={outdir}/docformat/google_demo',
         '--project-name=pydoctor-google-style-demo',
         '--project-version=1.0.0',
         '--docformat=google',
         '--project-url=../google-numpy.html',
         '--theme=readthedocs',
         f'{_pydoctor_root}/docs/google_demo',
         ] + _common_args,
```

### Comparing `pydoctor-22.9.1/docs/source/contrib.rst` & `pydoctor-23.4.0/docs/source/contrib.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/customize.rst` & `pydoctor-23.4.0/docs/source/customize.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/docformat/epytext.rst` & `pydoctor-23.4.0/docs/source/docformat/epytext.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Epytext
 =======
 
 .. toctree::
     :maxdepth: 1
 
-    epytext/epytext_demo
+    epytext_demo/index
 
 Read the `the epytext manual <http://epydoc.sourceforge.net/manual-epytext.html>`_
 for full documentation.
 
 Pydoctor has extended ``epydoc``'s parser and uses it as a
 library to parse epytext formatted docstrings.
```

### Comparing `pydoctor-22.9.1/docs/source/docformat/google-numpy.rst` & `pydoctor-23.4.0/docs/source/docformat/google-numpy.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Google and Numpy
 ================
 
 .. toctree::
     :maxdepth: 1
     
-    google/google_demo
-    numpy/numpy_demo
+    google_demo/index
+    numpy_demo/index
 
 Pydoctor now supports numpydoc and google style docstrings!
 
 Docstrings will be first converted to reStructuredText and then parsed with ``docutils``. 
 Any supported `reST markup <restructuredtext.html>`_ can be use to supplement google-style or numpy-style markup. 
 
 The main difference between the two styles is that Google uses indentation to separate sections,
```

### Comparing `pydoctor-22.9.1/docs/source/docformat/index.rst` & `pydoctor-23.4.0/docs/source/docformat/index.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/docformat/list-restructuredtext-support.rst` & `pydoctor-23.4.0/docs/source/docformat/list-restructuredtext-support.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/docformat/restructuredtext.rst` & `pydoctor-23.4.0/docs/source/docformat/restructuredtext.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 reStructuredText
 ================
 
 .. toctree::
     :maxdepth: 1
 
-    restructuredtext/restructuredtext_demo
+    restructuredtext_demo/index
 
 For the language syntax documentation, read the `ReST docutils syntax reference <https://docutils.sourceforge.io/docs/user/rst/quickref.html>`_.
 
 Fields
 ------
 
 See :ref:`fields section <codedoc-fields>`.
```

### Comparing `pydoctor-22.9.1/docs/source/faq.rst` & `pydoctor-23.4.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/help.rst` & `pydoctor-23.4.0/docs/source/help.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/publish-github-action.rst` & `pydoctor-23.4.0/docs/source/publish-github-action.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/quickstart.rst` & `pydoctor-23.4.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/sphinx-integration.rst` & `pydoctor-23.4.0/docs/source/sphinx-integration.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/source/transition.rst` & `pydoctor-23.4.0/docs/source/transition.rst`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/tests/test-search.html` & `pydoctor-23.4.0/docs/tests/test-search.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/tests/test.py` & `pydoctor-23.4.0/docs/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def test_rtd_pydoctor_multiple_call():
     """
     With the pydoctor Sphinx extension can call pydoctor for more than one
     API doc source.
     """
-    with open(BASE_DIR / 'docformat' / 'epytext' / 'index.html', 'r') as stream:
+    with open(BASE_DIR / 'docformat' / 'epytext_demo' / 'index.html', 'r') as stream:
         page = stream.read()
         assert '<a href="../epytext.html" class="projecthome">pydoctor-epytext-demo</a>' in page, page
 
 
 def test_rtd_extension_inventory():
     """
     The Sphinx inventory is available during normal sphinx-build.
@@ -72,15 +72,15 @@
 
 
 def test_sphinx_object_inventory_version_epytext_demo():
     """
     The Sphinx inventory for demo/showcase code has a fixed version and name,
     passed via docs/source/conf.py.
     """
-    with open(BASE_DIR / 'docformat' / 'epytext' / 'objects.inv', 'rb') as stream:
+    with open(BASE_DIR / 'docformat' / 'epytext_demo' / 'objects.inv', 'rb') as stream:
         page = stream.read()
         assert page.startswith(
             b'# Sphinx inventory version 2\n'
             b'# Project: pydoctor-epytext-demo\n'
             b'# Version: 1.3.0\n'
             ), page
```

### Comparing `pydoctor-22.9.1/docs/tests/test_python_igraph_docs.py` & `pydoctor-23.4.0/docs/tests/test_python_igraph_docs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/tests/test_standard_library_docs.py` & `pydoctor-23.4.0/docs/tests/test_standard_library_docs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/docs/tests/test_twisted_docs.py` & `pydoctor-23.4.0/docs/tests/test_twisted_docs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/__init__.py` & `pydoctor-23.4.0/pydoctor/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/_configparser.py` & `pydoctor-23.4.0/pydoctor/_configparser.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/astbuilder.py` & `pydoctor-23.4.0/pydoctor/astbuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     Any, Callable, Collection, Dict, Iterable, Iterator, List, Mapping, Optional, Sequence, Tuple,
     Type, TypeVar, Union, cast
 )
 
 import astor
 from pydoctor import epydoc2stan, model, node2stan, extensions
 from pydoctor.epydoc.markup._pyval_repr import colorize_inline_pyval
-from pydoctor.astutils import (is_typing_annotation, is_using_annotations, is_using_typing_final, node2dottedname, node2fullname, 
-                               is__name__equals__main__, unstring_annotation, iterassign, 
+from pydoctor.astutils import (is_none_literal, is_typing_annotation, is_using_annotations, is_using_typing_final, node2dottedname, node2fullname, 
+                               is__name__equals__main__, unstring_annotation, iterassign, extract_docstring_linenum,  
                                NodeVisitor)
 
 def parseFile(path: Path) -> ast.Module:
     """Parse the contents of a Python source file."""
     with open(path, 'rb') as f:
         src = f.read() + b'\n'
     return _parse(src, filename=str(path))
@@ -765,46 +765,71 @@
 
         func_name = node.name
 
         # determine the function's kind
         is_property = False
         is_classmethod = False
         is_staticmethod = False
-        if isinstance(parent, model.Class) and node.decorator_list:
+        is_overload_func = False
+        if node.decorator_list:
             for d in node.decorator_list:
                 if isinstance(d, ast.Call):
                     deco_name = node2dottedname(d.func)
                 else:
                     deco_name = node2dottedname(d)
                 if deco_name is None:
                     continue
-                if deco_name[-1].endswith('property') or deco_name[-1].endswith('Property'):
-                    is_property = True
-                elif deco_name == ['classmethod']:
-                    is_classmethod = True
-                elif deco_name == ['staticmethod']:
-                    is_staticmethod = True
-                elif len(deco_name) >= 2 and deco_name[-1] in ('setter', 'deleter'):
-                    # Rename the setter/deleter, so it doesn't replace
-                    # the property object.
-                    func_name = '.'.join(deco_name[-2:])
+                if isinstance(parent, model.Class):
+                    if deco_name[-1].endswith('property') or deco_name[-1].endswith('Property'):
+                        is_property = True
+                    elif deco_name == ['classmethod']:
+                        is_classmethod = True
+                    elif deco_name == ['staticmethod']:
+                        is_staticmethod = True
+                    elif len(deco_name) >= 2 and deco_name[-1] in ('setter', 'deleter'):
+                        # Rename the setter/deleter, so it doesn't replace
+                        # the property object.
+                        func_name = '.'.join(deco_name[-2:])
+                # Determine if the function is decorated with overload
+                if parent.expandName('.'.join(deco_name)) in ('typing.overload', 'typing_extensions.overload'):
+                    is_overload_func = True
 
         if is_property:
             # handle property and skip child nodes.
             attr = self._handlePropertyDef(node, docstring, lineno)
             if is_classmethod:
                 attr.report(f'{attr.fullName()} is both property and classmethod')
             if is_staticmethod:
                 attr.report(f'{attr.fullName()} is both property and staticmethod')
             raise self.SkipNode()
 
-        func = self.builder.pushFunction(func_name, lineno)
+        # Check if it's a new func or exists with an overload
+        existing_func = parent.contents.get(func_name)
+        if isinstance(existing_func, model.Function) and existing_func.overloads:
+            # If the existing function has a signature and this function is an
+            # overload, then the overload came _after_ the primary function
+            # which we do not allow. This also ensures that func will have
+            # properties set for the primary function and not overloads.
+            if existing_func.signature and is_overload_func:
+                existing_func.report(f'{existing_func.fullName()} overload appeared after primary function', lineno_offset=lineno-existing_func.linenumber)
+                raise self.SkipNode()
+            # Do not recreate function object, just re-push it
+            self.builder.push(existing_func, lineno)
+            func = existing_func
+        else:
+            func = self.builder.pushFunction(func_name, lineno)
+
         func.is_async = is_async
         if docstring is not None:
-            func.setDocstring(docstring)
+            # Docstring not allowed on overload
+            if is_overload_func:
+                docline = extract_docstring_linenum(docstring)
+                func.report(f'{func.fullName()} overload has docstring, unsupported', lineno_offset=docline-func.linenumber)
+            else:
+                func.setDocstring(docstring)
         func.decorators = node.decorator_list
         if is_staticmethod:
             if is_classmethod:
                 func.report(f'{func.fullName()} is both classmethod and staticmethod')
             else:
                 func.kind = model.DocumentableKind.STATIC_METHOD
         elif is_classmethod:
@@ -812,23 +837,26 @@
 
         # Position-only arguments were introduced in Python 3.8.
         posonlyargs: Sequence[ast.arg] = getattr(node.args, 'posonlyargs', ())
 
         num_pos_args = len(posonlyargs) + len(node.args.args)
         defaults = node.args.defaults
         default_offset = num_pos_args - len(defaults)
+        annotations = self._annotations_from_function(node)
+
         def get_default(index: int) -> Optional[ast.expr]:
             assert 0 <= index < num_pos_args, index
             index -= default_offset
             return None if index < 0 else defaults[index]
 
         parameters: List[Parameter] = []
         def add_arg(name: str, kind: Any, default: Optional[ast.expr]) -> None:
             default_val = Parameter.empty if default is None else _ValueFormatter(default, ctx=func)
-            parameters.append(Parameter(name, kind, default=default_val))
+            annotation = Parameter.empty if annotations.get(name) is None else _AnnotationValueFormatter(annotations[name], ctx=func)
+            parameters.append(Parameter(name, kind, default=default_val, annotation=annotation))
 
         for index, arg in enumerate(posonlyargs):
             add_arg(arg.arg, Parameter.POSITIONAL_ONLY, get_default(index))
 
         for index, arg in enumerate(node.args.args, start=len(posonlyargs)):
             add_arg(arg.arg, Parameter.POSITIONAL_OR_KEYWORD, get_default(index))
 
@@ -840,23 +868,30 @@
         for arg, default in zip(node.args.kwonlyargs, node.args.kw_defaults):
             add_arg(arg.arg, Parameter.KEYWORD_ONLY, default)
 
         kwarg = node.args.kwarg
         if kwarg is not None:
             add_arg(kwarg.arg, Parameter.VAR_KEYWORD, None)
 
+        return_type = annotations.get('return')
+        return_annotation = Parameter.empty if return_type is None or is_none_literal(return_type) else _AnnotationValueFormatter(return_type, ctx=func)
         try:
-            signature = Signature(parameters)
+            signature = Signature(parameters, return_annotation=return_annotation)
         except ValueError as ex:
             func.report(f'{func.fullName()} has invalid parameters: {ex}')
             signature = Signature()
 
-        func.signature = signature
-        func.annotations = self._annotations_from_function(node)
-    
+        func.annotations = annotations
+
+        # Only set main function signature if it is a non-overload
+        if is_overload_func:
+            func.overloads.append(model.FunctionOverload(primary=func, signature=signature, decorators=node.decorator_list))
+        else:
+            func.signature = signature
+
     def depart_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:
         self.builder.popFunction()
 
     def depart_FunctionDef(self, node: ast.FunctionDef) -> None:
         self.builder.popFunction()
 
     def _handlePropertyDef(self,
@@ -957,22 +992,33 @@
         Without the englobing <code> tags.
         """
         # Using node2stan.node2html instead of flatten(to_stan()). 
         # This avoids calling flatten() twice, 
         # but potential XML parser errors caused by XMLString needs to be handled later.
         return ''.join(node2stan.node2html(self._colorized.to_node(), self._linker))
 
+class _AnnotationValueFormatter(_ValueFormatter):
+    """
+    Special L{_ValueFormatter} for annotations.
+    """
+    def __repr__(self) -> str:
+        """
+        Present the annotation wrapped inside <code> tags.
+        """
+        return '<code>%s</code>' % super().__repr__()
+
+
 def _infer_type(expr: ast.expr) -> Optional[ast.expr]:
     """Infer an expression's type.
     @param expr: The expression's AST.
     @return: A type annotation, or None if the expression has no obvious type.
     """
     try:
         value: object = ast.literal_eval(expr)
-    except ValueError:
+    except (ValueError, TypeError):
         return None
     else:
         ann = _annotation_for_value(value)
         if ann is None:
             return None
         else:
             return ast.fix_missing_locations(ast.copy_location(ann, expr))
```

### Comparing `pydoctor-22.9.1/pydoctor/astutils.py` & `pydoctor-23.4.0/pydoctor/astutils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Various bits of reusable code related to L{ast.AST} node processing.
 """
 
+import inspect
+import platform
 import sys
 from numbers import Number
-from typing import Iterator, Optional, List, Iterable, Sequence, TYPE_CHECKING, Union
+from typing import Iterator, Optional, List, Iterable, Sequence, TYPE_CHECKING, Tuple, Union
 from inspect import BoundArguments, Signature
 import ast
 
 from pydoctor import visitor
 
 if TYPE_CHECKING:
     from pydoctor import model
@@ -142,14 +144,20 @@
     def get_num_value(expr:ast.expr) -> Optional[Number]:
         if isinstance(expr, ast.Num):
             return expr.n
         return None
     def _is_str_constant(expr: ast.expr, s: str) -> bool:
         return isinstance(expr, ast.Str) and expr.s == s
 
+def get_int_value(expr: ast.expr) -> Optional[int]:
+    num = get_num_value(expr)
+    if isinstance(num, int):
+        return num # type:ignore[unreachable]
+    return None
+
 def is__name__equals__main__(cmp: ast.Compare) -> bool:
     """
     Returns whether or not the given L{ast.Compare} is equal to C{__name__ == '__main__'}.
     """
     return isinstance(cmp.left, ast.Name) \
     and cmp.left.id == '__name__' \
     and len(cmp.ops) == 1 \
@@ -179,14 +187,18 @@
         if isinstance(expr.value, (ast.Name, ast.Attribute)):
             value = expr.value
             full_name = node2fullname(value, ctx)
             if full_name in annotations:
                 return True
     return False
 
+def is_none_literal(node: ast.expr) -> bool:
+    """Does this AST node represent the literal constant None?"""
+    return isinstance(node, (ast.Constant, ast.NameConstant)) and node.value is None
+    
 def unstring_annotation(node: ast.expr, ctx:'model.Documentable') -> ast.expr:
     """Replace all strings in the given expression by parsed versions.
     @return: The unstringed node. If parsing fails, an error is logged
         and the original node is returned.
     """
     try:
         expr = _AnnotationStringParser().visit(node)
@@ -341,7 +353,53 @@
 def is_typing_annotation(node: ast.AST, ctx: 'model.Documentable') -> bool:
     """
     Whether this annotation node refers to a typing alias.
     """
     return is_using_annotations(node, TYPING_ALIAS, ctx) or \
             is_using_annotations(node, SUBSCRIPTABLE_CLASSES_PEP585, ctx)
 
+
+_string_lineno_is_end = sys.version_info < (3,8) \
+                    and platform.python_implementation() != 'PyPy'
+"""True iff the 'lineno' attribute of an AST string node points to the last
+line in the string, rather than the first line.
+"""
+
+def extract_docstring_linenum(node: ast.Str) -> int:
+    r"""
+    In older CPython versions, the AST only tells us the end line
+    number and we must approximate the start line number.
+    This approximation is correct if the docstring does not contain
+    explicit newlines ('\n') or joined lines ('\' at end of line).
+
+    Leading blank lines are stripped by cleandoc(), so we must
+    return the line number of the first non-blank line.
+    """
+    doc = node.s
+    lineno = node.lineno
+    if _string_lineno_is_end:
+        # In older CPython versions, the AST only tells us the end line
+        # number and we must approximate the start line number.
+        # This approximation is correct if the docstring does not contain
+        # explicit newlines ('\n') or joined lines ('\' at end of line).
+        lineno -= doc.count('\n')
+
+    # Leading blank lines are stripped by cleandoc(), so we must
+    # return the line number of the first non-blank line.
+    for ch in doc:
+        if ch == '\n':
+            lineno += 1
+        elif not ch.isspace():
+            break
+    
+    return lineno
+
+def extract_docstring(node: ast.Str) -> Tuple[int, str]:
+    """
+    Extract docstring information from an ast node that represents the docstring.
+
+    @returns: 
+        - The line number of the first non-blank line of the docsring. See L{extract_docstring_linenum}.
+        - The docstring to be parsed, cleaned by L{inspect.cleandoc}.
+    """
+    lineno = extract_docstring_linenum(node)
+    return lineno, inspect.cleandoc(node.s)
```

### Comparing `pydoctor-22.9.1/pydoctor/driver.py` & `pydoctor-23.4.0/pydoctor/driver.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/__init__.py` & `pydoctor-23.4.0/pydoctor/epydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/doctest.py` & `pydoctor-23.4.0/pydoctor/epydoc/doctest.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/docutils.py` & `pydoctor-23.4.0/pydoctor/epydoc/docutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 """
 Collection of helper functions and classes related to the creation and processing of L{docutils} nodes.
 """
 from typing import Iterable, Iterator, Optional
 
-from docutils import nodes
+import optparse
+
+from docutils import nodes, utils, frontend, __version_info__ as docutils_version_info
 from docutils.transforms import parts
 
 __docformat__ = 'epytext en'
 
+_DEFAULT_DOCUTILS_SETTINGS: Optional[optparse.Values] = None
+
+def new_document(source_path: str, settings: Optional[optparse.Values] = None) -> nodes.document:
+    """
+    Create a new L{nodes.document} using the provided settings or cached default settings.
+
+    @returns: L{nodes.document}
+    """
+    global _DEFAULT_DOCUTILS_SETTINGS
+    # If we have docutils >= 0.19 we use get_default_settings to calculate and cache
+    # the default settings. Otherwise we let new_document figure it out.
+    if settings is None and docutils_version_info >= (0,19):
+        if _DEFAULT_DOCUTILS_SETTINGS is None:
+            _DEFAULT_DOCUTILS_SETTINGS = frontend.get_default_settings() # type:ignore[attr-defined]
+
+        settings = _DEFAULT_DOCUTILS_SETTINGS
+
+    return utils.new_document(source_path, settings)
+
 def _set_nodes_parent(nodes: Iterable[nodes.Node], parent: nodes.Element) -> Iterator[nodes.Node]:
     """
     Set the L{nodes.Node.parent} attribute of the C{nodes} to the defined C{parent}. 
     
     @returns: An iterator containing the modified nodes.
     """
     for node in nodes:
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/__init__.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 from typing import Callable, ContextManager, List, Optional, Sequence, Iterator, TYPE_CHECKING
 import abc
 import sys
 import re
 from importlib import import_module
 from inspect import getmodulename
 
-from docutils import nodes, utils
+from docutils import nodes
 from twisted.web.template import Tag, tags
 
 from pydoctor import node2stan
-from pydoctor.epydoc.docutils import set_node_attributes, build_table_of_content
+from pydoctor.epydoc.docutils import set_node_attributes, build_table_of_content, new_document
 
 
 # In newer Python versions, use importlib.resources from the standard library.
 # On older versions, a compatibility package must be installed from PyPI.
 if sys.version_info < (3, 9):
     import importlib_resources
 else:
@@ -64,36 +64,62 @@
 #
 # 1. ParsedDocstring abstract base class
 # 2. Field class
 # 3. Docstring Linker
 # 4. ParseError exceptions
 #
 
+ParserFunction = Callable[[str, List['ParseError']], 'ParsedDocstring']
+
 def get_supported_docformats() -> Iterator[str]:
     """
     Get the list of currently supported docformat.
     """
     for fileName in (path.name for path in importlib_resources.files('pydoctor.epydoc.markup').iterdir()):
         moduleName = getmodulename(fileName)
         if moduleName is None or moduleName.startswith("_"):
             continue
         else:
             yield moduleName
 
-def get_parser_by_name(docformat: str, obj: Optional['Documentable'] = None) -> Callable[[str, List['ParseError'], bool], 'ParsedDocstring']:
+def get_parser_by_name(docformat: str, obj: Optional['Documentable'] = None) -> ParserFunction:
     """
     Get the C{parse_docstring(str, List[ParseError], bool) -> ParsedDocstring} function based on a parser name. 
 
     @raises ImportError: If the parser could not be imported, probably meaning that your are missing a dependency
         or it could be that the docformat name do not match any know L{pydoctor.epydoc.markup} submodules.
     """
     mod = import_module(f'pydoctor.epydoc.markup.{docformat}')
     # We can safely ignore this mypy warning, since we can be sure the 'get_parser' function exist and is "correct".
     return mod.get_parser(obj) # type:ignore[no-any-return]
 
+def processtypes(parse:ParserFunction) -> ParserFunction:
+    """
+    Wraps a docstring parser function to provide option --process-types.
+    """
+    
+    def _processtypes(doc: 'ParsedDocstring', errs: List['ParseError']) -> None:
+        """
+        Mutates the type fields of the given parsed docstring to replace 
+        their body by parsed version with type auto-linking.
+        """
+        from pydoctor.epydoc.markup._types import ParsedTypeDocstring
+        for field in doc.fields:
+            if field.tag() in ParsedTypeDocstring.FIELDS:
+                body = ParsedTypeDocstring(field.body().to_node(), lineno=field.lineno)
+                append_warnings(body.warnings, errs, lineno=field.lineno+1)
+                field.replace_body(body)
+    
+    def parse_and_processtypes(doc:str, errs:List['ParseError']) -> 'ParsedDocstring':
+        parsed_doc = parse(doc, errs)
+        _processtypes(parsed_doc, errs)
+        return parsed_doc
+
+    return parse_and_processtypes
+
 ##################################################
 ## ParsedDocstring
 ##################################################
 class ParsedDocstring(abc.ABC):
     """
     A standard intermediate representation for parsed docstrings that
     can be used to generate output.  Parsed docstrings are produced by
@@ -113,15 +139,14 @@
         """
         A list of L{Field}s, each of which encodes a single field.
         The field's bodies are encoded as C{ParsedDocstring}s.
         """
 
         self._stan: Optional[Tag] = None
         self._summary: Optional['ParsedDocstring'] = None
-        self._compact = True
 
     @abc.abstractproperty
     def has_body(self) -> bool:
         """
         Does this docstring have a non-empty body?
 
         The body is the part of the docstring that remains after the fields
@@ -133,50 +158,38 @@
         The table of contents of the docstring if titles are defined or C{None}.
         """
         try:
             document = self.to_node()
         except NotImplementedError:
             return None
         contents = build_table_of_content(document, depth=depth)
-        docstring_toc = utils.new_document('toc')
+        docstring_toc = new_document('toc')
         if contents:
             docstring_toc.extend(contents)
             from pydoctor.epydoc.markup.restructuredtext import ParsedRstDocstring
             return ParsedRstDocstring(docstring_toc, ())
         else:
             return None
 
-    def to_stan(self, docstring_linker: 'DocstringLinker', compact:bool=True) -> Tag:
+    def to_stan(self, docstring_linker: 'DocstringLinker') -> Tag:
         """
         Translate this docstring to a Stan tree.
 
         @note: The default implementation relies on functionalities 
             provided by L{node2stan.node2stan} and L{ParsedDocstring.to_node()}.
 
         @param docstring_linker: An HTML translator for crossreference
             links into and out of the docstring.
         @return: The docstring presented as a stan tree.
         @raises Exception: If something went wrong. Callers should generally catch C{Exception}
             when calling L{to_stan()}.
         """
-        # The following three lines is a hack in order to still show p tags 
-        # around docstrings content when there is only a single line text
-        # and arguement compact=False is passed. We clear cached stan if required.
-        if compact != self._compact and self._stan is not None:
-            self._stan = None
-        self._compact = compact
-
         if self._stan is not None:
-            return self._stan      
-
-        docstring_stan = node2stan.node2stan(self.to_node(), 
-                                        docstring_linker, 
-                                        compact=compact)
-
-        self._stan = Tag('', children=docstring_stan.children)
+            return self._stan
+        self._stan = Tag('', children=node2stan.node2stan(self.to_node(), docstring_linker).children)
         return self._stan
     
     @abc.abstractmethod
     def to_node(self) -> nodes.document:
         """
         Translate this docstring to a L{nodes.document}.
 
@@ -246,14 +259,17 @@
         return self._arg
 
     def body(self) -> ParsedDocstring:
         """
         @return: This field's body.
         """
         return self._body
+    
+    def replace_body(self, newbody:ParsedDocstring) -> None:
+        self._body = newbody
 
     def __repr__(self) -> str:
         if self._arg is None:
             return f'<Field @{self._tag}: ...>'
         else:
             return f'<Field @{self._tag} {self._arg}: ...>'
 
@@ -301,25 +317,29 @@
         This will resolve the identifier like Python itself would.
 
         @param identifier: The name of the Python identifier that
             should be linked to.
         @return: The URL of the target, or L{None} if not found.
         """
         raise NotImplementedError()
-    
-    def disable_same_page_optimazation(self) -> ContextManager[None]:
+
+    def switch_context(self, ob:Optional['Documentable']) -> ContextManager[None]:
         """
-        By default, when linkng to an object on the same page, the linker will generate 
-        an URL that links to the anchor only, this will avoid reloading the page needlessly. But sometimes 
-        we're using a linker to present the content on another page. This context manager will 
-        make the linker always generate full URLs.
+        Switch the context of the linker, keeping the same underlying lookup rules.
+
+        Useful to resolve links with the right L{Documentable} context but
+        create correct - absolute or relative - links to be clicked on from another page 
+        rather than the initial page of the context. "Cannot find link target" errors will be reported
+        relatively to the new context object.
+
+        Pass C{None} to always generate full URLs (for summaries for example), 
+        in this case error will NOT be reported at all.
         """
         raise NotImplementedError()
 
-
 ##################################################
 ## ParseError exceptions
 ##################################################
 
 def append_warnings(warns:List[str], errs:List['ParseError'], lineno:int) -> None:
     """
     Utility method to create non fatal L{ParseError}s and append them to the provided list.
@@ -423,15 +443,15 @@
 
     def visit_paragraph(self, node: nodes.Node) -> None:
         if self.summary is not None:
             # found a paragraph after the first one
             self.other_docs = True
             raise nodes.StopTraversal()
 
-        summary_doc = utils.new_document('summary')
+        summary_doc = new_document('summary')
         summary_pieces = []
 
         # Extract the first sentences from the first paragraph until maximum number 
         # of characters is reach or until the end of the paragraph.
         char_count = 0
 
         for child in node:
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/_napoleon.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/_napoleon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains a class to wrap shared behaviour between 
 L{pydoctor.epydoc.markup.numpy} and L{pydoctor.epydoc.markup.google}. 
 """
 from typing import List, Optional, Type
 
-from pydoctor.epydoc.markup import ParsedDocstring, ParseError
+from pydoctor.epydoc.markup import ParsedDocstring, ParseError, processtypes
 from pydoctor.epydoc.markup import restructuredtext
 from pydoctor.napoleon.docstring import GoogleDocstring, NumpyDocstring
 from pydoctor.model import Attribute, Documentable
 
 
 class NapoelonDocstringParser:
     """
@@ -25,38 +25,37 @@
     def __init__(self, obj: Optional[Documentable] = None):
         """
         @param obj: Documentable object we're parsing the docstring for.
         """
         self.obj = obj
 
     def parse_google_docstring(
-        self, docstring: str, errors: List[ParseError], processtypes: bool = True
+        self, docstring: str, errors: List[ParseError]
     ) -> ParsedDocstring:
         """
         Parse the given docstring, which is formatted as Google style docstring.
         Return a L{ParsedDocstring} representation of its contents.
 
         @param docstring: The docstring to parse
         @param errors: A list where any errors generated during parsing
             will be stored.
         """
         return self._parse_docstring(
             docstring, errors, GoogleDocstring, )
 
     def parse_numpy_docstring(
-        self, docstring: str, errors: List[ParseError], processtypes: bool = True
+        self, docstring: str, errors: List[ParseError]
     ) -> ParsedDocstring:
         """
         Parse the given docstring, which is formatted as NumPy style docstring.
         Return a L{ParsedDocstring} representation of its contents.
 
         @param docstring: The docstring to parse
         @param errors: A list where any errors generated during parsing
             will be stored.
-        @param processtypes: processtypes is always ``True`` for google and numpy docstrings.
         """
         return self._parse_docstring(
             docstring, errors, NumpyDocstring, )
 
     def _parse_docstring(
         self,
         docstring: str,
@@ -79,8 +78,8 @@
         """
         Helper method to parse L{GoogleDocstring} or L{NumpyDocstring} objects.
         """
         # log any warnings
         for warn, lineno in docstring_obj.warnings:
             errors.append(ParseError(warn, lineno, is_fatal=False))
         # Get the converted reST string and parse it with docutils
-        return restructuredtext.parse_docstring(str(docstring_obj), errors, processtypes=True)
+        return processtypes(restructuredtext.parse_docstring)(str(docstring_obj), errors)
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/_pyval_repr.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/_pyval_repr.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,27 +35,26 @@
 
 __docformat__ = 'epytext en'
 
 import re
 import ast
 import functools
 import sys
-import sre_constants
 from inspect import signature
 from typing import Any, AnyStr, Union, Callable, Dict, Iterable, Sequence, Optional, List, Tuple, cast
 
 import attr
 import astor.op_util
-from docutils import nodes, utils
+from docutils import nodes
 from twisted.web.template import Tag
 
-from pydoctor.epydoc import sre_parse36
+from pydoctor.epydoc import sre_parse36, sre_constants36 as sre_constants
 from pydoctor.epydoc.markup import DocstringLinker
 from pydoctor.epydoc.markup.restructuredtext import ParsedRstDocstring
-from pydoctor.epydoc.docutils import set_node_attributes, wbr, obj_reference
+from pydoctor.epydoc.docutils import set_node_attributes, wbr, obj_reference, new_document
 from pydoctor.astutils import node2dottedname, bind_args
 
 def decode_with_backslashreplace(s: bytes) -> str:
     r"""
     Convert the given 8-bit string into unicode, treating any
     character c such that ord(c)<128 as an ascii character, and
     converting any c such that ord(c)>128 into a backslashed escape
@@ -185,17 +184,17 @@
         super().__init__(document, ())
         self.is_complete = is_complete
         self.warnings = warnings
         """
         List of warnings
         """
     
-    def to_stan(self, docstring_linker: DocstringLinker, compact:bool=False) -> Tag:
+    def to_stan(self, docstring_linker: DocstringLinker) -> Tag:
         return Tag('code')(super().to_stan(docstring_linker))
-
+    
 def colorize_pyval(pyval: Any, linelen:Optional[int], maxlines:int, linebreakok:bool=True) -> ColorizedPyvalRepr:
     """
     @return: A L{ColorizedPyvalRepr} describing the given pyval.
     """
     return PyvalColorizer(linelen=linelen, maxlines=maxlines, linebreakok=linebreakok).colorize(pyval)
 
 def colorize_inline_pyval(pyval: Any) -> ColorizedPyvalRepr:
@@ -309,15 +308,15 @@
                 self._trim_result(state.result, 3)
                 state.result.append(self.ELLIPSIS)
             is_complete = False
         else:
             is_complete = True
         
         # Put it all together.
-        document = utils.new_document('pyval_repr')
+        document = new_document('pyval_repr')
         # This ensure the .parent and .document attributes of the child nodes are set correcly.
         set_node_attributes(document, children=[set_node_attributes(node, document=document) for node in state.result])
         return ColorizedPyvalRepr(document, is_complete, state.warnings)
     
     def _colorize(self, pyval: Any, state: _ColorizerState) -> None:
 
         pyvaltype = type(pyval)
@@ -713,15 +712,16 @@
         self._output('(', self.GROUP_TAG, state)
         indent = state.charpos
         
         try:
             # Can raise ValueError or re.error
             # Value of type variable "AnyStr" cannot be "Union[bytes, str]": Yes it can.
             self._colorize_re_pattern_str(pat, state) #type:ignore[type-var]
-        except (ValueError, re.error) as e:
+        except (ValueError, sre_constants.error) as e:
+            # Make sure not to swallow control flow errors.
             # Colorize the ast.Call as any other node if the pattern parsing fails.
             state.restore(mark)
             state.warnings.append(f"Cannot colorize regular expression, error: {str(e)}")
             self._colorize_ast_call_generic(node, state)
             return
 
         ast_flags = args.arguments.get('flags')
@@ -809,15 +809,15 @@
         if len(tree) > 1 and not noparen:
             self._output('(', self.RE_GROUP_TAG, state)
 
         for elt in tree:
             op = elt[0]
             args = elt[1]
 
-            if op == sre_constants.LITERAL:
+            if op == sre_constants.LITERAL: #type:ignore[attr-defined]
                 c = chr(cast(int, args))
                 # Add any appropriate escaping.
                 if c in '.^$\\*+?{}[]|()\'': 
                     c = '\\' + c
                 elif c == '\t': 
                     c = r'\t'
                 elif c == '\r': 
@@ -831,75 +831,75 @@
                 # Keep unicode chars as is, so do nothing if ord(c) > 65535
                 elif ord(c) > 255 and ord(c) <= 65535: 
                    c = rb'\u%04x' % ord(c) # type:ignore[assignment]
                 elif (ord(c)<32 or ord(c)>=127) and ord(c) <= 65535: 
                     c = rb'\x%02x' % ord(c) # type:ignore[assignment]
                 self._output(c, self.RE_CHAR_TAG, state)
 
-            elif op == sre_constants.ANY:
+            elif op == sre_constants.ANY: #type:ignore[attr-defined]
                 self._output('.', self.RE_CHAR_TAG, state)
 
-            elif op == sre_constants.BRANCH:
+            elif op == sre_constants.BRANCH: #type:ignore[attr-defined]
                 if args[0] is not None:
                     raise ValueError('Branch expected None arg but got %s'
                                      % args[0])
                 for i, item in enumerate(args[1]):
                     if i > 0:
                         self._output('|', self.RE_OP_TAG, state)
                     self._colorize_re_tree(item, state, True, groups)
 
-            elif op == sre_constants.IN:
-                if (len(args) == 1 and args[0][0] == sre_constants.CATEGORY):
+            elif op == sre_constants.IN: #type:ignore[attr-defined]
+                if (len(args) == 1 and args[0][0] == sre_constants.CATEGORY): #type:ignore[attr-defined]
                     self._colorize_re_tree(args, state, False, groups)
                 else:
                     self._output('[', self.RE_GROUP_TAG, state)
                     self._colorize_re_tree(args, state, True, groups)
                     self._output(']', self.RE_GROUP_TAG, state)
 
-            elif op == sre_constants.CATEGORY:
-                if args == sre_constants.CATEGORY_DIGIT: val = r'\d'
-                elif args == sre_constants.CATEGORY_NOT_DIGIT: val = r'\D'
-                elif args == sre_constants.CATEGORY_SPACE: val = r'\s'
-                elif args == sre_constants.CATEGORY_NOT_SPACE: val = r'\S'
-                elif args == sre_constants.CATEGORY_WORD: val = r'\w'
-                elif args == sre_constants.CATEGORY_NOT_WORD: val = r'\W'
+            elif op == sre_constants.CATEGORY: #type:ignore[attr-defined]
+                if args == sre_constants.CATEGORY_DIGIT: val = r'\d' #type:ignore[attr-defined]
+                elif args == sre_constants.CATEGORY_NOT_DIGIT: val = r'\D' #type:ignore[attr-defined]
+                elif args == sre_constants.CATEGORY_SPACE: val = r'\s' #type:ignore[attr-defined]
+                elif args == sre_constants.CATEGORY_NOT_SPACE: val = r'\S' #type:ignore[attr-defined]
+                elif args == sre_constants.CATEGORY_WORD: val = r'\w' #type:ignore[attr-defined]
+                elif args == sre_constants.CATEGORY_NOT_WORD: val = r'\W' #type:ignore[attr-defined]
                 else: raise ValueError('Unknown category %s' % args)
                 self._output(val, self.RE_CHAR_TAG, state)
 
-            elif op == sre_constants.AT:
-                if args == sre_constants.AT_BEGINNING_STRING: val = r'\A'
-                elif args == sre_constants.AT_BEGINNING: val = '^'
-                elif args == sre_constants.AT_END: val = '$'
-                elif args == sre_constants.AT_BOUNDARY: val = r'\b'
-                elif args == sre_constants.AT_NON_BOUNDARY: val = r'\B'
-                elif args == sre_constants.AT_END_STRING: val = r'\Z'
+            elif op == sre_constants.AT: #type:ignore[attr-defined]
+                if args == sre_constants.AT_BEGINNING_STRING: val = r'\A' #type:ignore[attr-defined]
+                elif args == sre_constants.AT_BEGINNING: val = '^' #type:ignore[attr-defined]
+                elif args == sre_constants.AT_END: val = '$' #type:ignore[attr-defined]
+                elif args == sre_constants.AT_BOUNDARY: val = r'\b' #type:ignore[attr-defined]
+                elif args == sre_constants.AT_NON_BOUNDARY: val = r'\B' #type:ignore[attr-defined]
+                elif args == sre_constants.AT_END_STRING: val = r'\Z' #type:ignore[attr-defined]
                 else: raise ValueError('Unknown position %s' % args)
                 self._output(val, self.RE_CHAR_TAG, state)
 
-            elif op in (sre_constants.MAX_REPEAT, sre_constants.MIN_REPEAT):
+            elif op in (sre_constants.MAX_REPEAT, sre_constants.MIN_REPEAT): #type:ignore[attr-defined]
                 minrpt = args[0]
                 maxrpt = args[1]
                 if maxrpt == sre_constants.MAXREPEAT:
                     if minrpt == 0:   val = '*'
                     elif minrpt == 1: val = '+'
                     else: val = '{%d,}' % (minrpt)
                 elif minrpt == 0:
                     if maxrpt == 1: val = '?'
                     else: val = '{,%d}' % (maxrpt)
                 elif minrpt == maxrpt:
                     val = '{%d}' % (maxrpt)
                 else:
                     val = '{%d,%d}' % (minrpt, maxrpt)
-                if op == sre_constants.MIN_REPEAT:
+                if op == sre_constants.MIN_REPEAT: #type:ignore[attr-defined]
                     val += '?'
 
                 self._colorize_re_tree(args[2], state, False, groups)
                 self._output(val, self.RE_OP_TAG, state)
 
-            elif op == sre_constants.SUBPATTERN:
+            elif op == sre_constants.SUBPATTERN: #type:ignore[attr-defined]
                 if args[0] is None:
                     self._output(r'(?:', self.RE_GROUP_TAG, state)
                 elif args[0] in groups:
                     self._output(r'(?P<', self.RE_GROUP_TAG, state)
                     self._output(groups[args[0]], self.RE_REF_TAG, state)
                     self._output('>', self.RE_GROUP_TAG, state)
                 elif isinstance(args[0], int):
@@ -908,50 +908,50 @@
                 else:
                     self._output('(?P<', self.RE_GROUP_TAG, state)
                     self._output(args[0], self.RE_REF_TAG, state)
                     self._output('>', self.RE_GROUP_TAG, state)
                 self._colorize_re_tree(args[3], state, True, groups)
                 self._output(')', self.RE_GROUP_TAG, state)
 
-            elif op == sre_constants.GROUPREF:
+            elif op == sre_constants.GROUPREF: #type:ignore[attr-defined]
                 self._output('\\%d' % args, self.RE_REF_TAG, state)
 
-            elif op == sre_constants.RANGE:
-                self._colorize_re_tree( ((sre_constants.LITERAL, args[0]),),
+            elif op == sre_constants.RANGE: #type:ignore[attr-defined]
+                self._colorize_re_tree( ((sre_constants.LITERAL, args[0]),), #type:ignore[attr-defined]
                                         state, False, groups )
                 self._output('-', self.RE_OP_TAG, state)
-                self._colorize_re_tree( ((sre_constants.LITERAL, args[1]),),
+                self._colorize_re_tree( ((sre_constants.LITERAL, args[1]),), #type:ignore[attr-defined]
                                         state, False, groups )
 
-            elif op == sre_constants.NEGATE:
+            elif op == sre_constants.NEGATE: #type:ignore[attr-defined]
                 self._output('^', self.RE_OP_TAG, state)
 
-            elif op == sre_constants.ASSERT:
+            elif op == sre_constants.ASSERT: #type:ignore[attr-defined]
                 if args[0] > 0:
                     self._output('(?=', self.RE_GROUP_TAG, state)
                 else:
                     self._output('(?<=', self.RE_GROUP_TAG, state)
                 self._colorize_re_tree(args[1], state, True, groups)
                 self._output(')', self.RE_GROUP_TAG, state)
 
-            elif op == sre_constants.ASSERT_NOT:
+            elif op == sre_constants.ASSERT_NOT: #type:ignore[attr-defined]
                 if args[0] > 0:
                     self._output('(?!', self.RE_GROUP_TAG, state)
                 else:
                     self._output('(?<!', self.RE_GROUP_TAG, state)
                 self._colorize_re_tree(args[1], state, True, groups)
                 self._output(')', self.RE_GROUP_TAG, state)
 
-            elif op == sre_constants.NOT_LITERAL:
+            elif op == sre_constants.NOT_LITERAL: #type:ignore[attr-defined]
                 self._output('[^', self.RE_GROUP_TAG, state)
-                self._colorize_re_tree( ((sre_constants.LITERAL, args),),
+                self._colorize_re_tree( ((sre_constants.LITERAL, args),), #type:ignore[attr-defined]
                                         state, False, groups )
                 self._output(']', self.RE_GROUP_TAG, state)
             else:
-                raise RuntimeError(f"Error colorizing regexp, unknown element :{elt}")
+                raise ValueError(f"Unsupported element :{elt}")
         if len(tree) > 1 and not noparen:
             self._output(')', self.RE_GROUP_TAG, state)
 
     #////////////////////////////////////////////////////////////
     # Output function
     #////////////////////////////////////////////////////////////
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/_types.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def to_node(self) -> nodes.document:
         """
         Not implemented.
         """
         raise NotImplementedError()
 
-    def to_stan(self, docstring_linker: DocstringLinker, compact:bool=False) -> Tag:
+    def to_stan(self, docstring_linker: DocstringLinker) -> Tag:
         """
         Present the type as a stan tree. 
         """
         return self._convert_type_spec_to_stan(docstring_linker)
 
     def _tokenize_node_type_spec(self, spec: nodes.document) -> List[Union[str, nodes.Node]]:
         
@@ -161,16 +161,16 @@
 
         converters: Dict[TokenType, Callable[[Union[str, Tag]], Union[str, Tag]]] = {
             TokenType.LITERAL:      lambda _token: tags.span(_token, class_="literal"),
             TokenType.CONTROL:      lambda _token: tags.em(_token),
             # We don't use safe_to_stan() here, if these converter functions raise an exception, 
             # the whole type docstring will be rendered as plaintext.
             # it does not crash on invalid xml entities
-            TokenType.REFERENCE:    lambda _token: get_parser_by_name('restructuredtext')(_token, warnings, False).to_stan(docstring_linker) if isinstance(_token, str) else _token, 
-            TokenType.UNKNOWN:      lambda _token: get_parser_by_name('restructuredtext')(_token, warnings, False).to_stan(docstring_linker) if isinstance(_token, str) else _token, 
+            TokenType.REFERENCE:    lambda _token: get_parser_by_name('restructuredtext')(_token, warnings).to_stan(docstring_linker) if isinstance(_token, str) else _token, 
+            TokenType.UNKNOWN:      lambda _token: get_parser_by_name('restructuredtext')(_token, warnings).to_stan(docstring_linker) if isinstance(_token, str) else _token, 
             TokenType.OBJ:          lambda _token: _token, # These convertions (OBJ and DELIMITER) are done in _convert_obj_tokens_to_stan().
             TokenType.DELIMITER:    lambda _token: _token, 
             TokenType.ANY:          lambda _token: _token, 
         }
 
         for w in warnings:
             self.warnings.append(w.descr())
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/epytext.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/epytext.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,24 +128,23 @@
 # Code organization..
 #   1. parse()
 #   2. tokenize()
 #   3. colorize()
 #   4. helpers
 #   5. testing
 
-from typing import Any, Callable, Iterable, List, Optional, Sequence, Set, Union, cast, overload
+from typing import Any, Iterable, List, Optional, Sequence, Set, Union, cast
 import re
 import unicodedata
 
-from docutils import utils, nodes
+from docutils import nodes
 from twisted.web.template import Tag
 
-from pydoctor.epydoc.markup import Field, ParseError, ParsedDocstring, append_warnings
-from pydoctor.epydoc.markup._types import ParsedTypeDocstring
-from pydoctor.epydoc.docutils import set_node_attributes
+from pydoctor.epydoc.markup import Field, ParseError, ParsedDocstring, ParserFunction
+from pydoctor.epydoc.docutils import set_node_attributes, new_document
 from pydoctor.model import Documentable
 
 ##################################################
 ## Helper functions
 ##################################################
 
 def gettext(node: Union[str, 'Element', List[Union[str, 'Element']]]) -> List[str]:
@@ -279,43 +278,30 @@
 # Which tags can use "link syntax" (e.g., U{Python<www.python.org>})?
 _LINK_COLORIZING_TAGS = ['link', 'uri']
 
 ##################################################
 ## Structuring (Top Level)
 ##################################################
 
-@overload
-def parse(text: str) -> Element: ...
-
-@overload
-def parse(text: str, errors: List[ParseError]) -> Optional[Element]: ...
-
-def parse(text: str, errors: Optional[List[ParseError]] = None) -> Optional[Element]:
+def parse(text: str, errors: List[ParseError]) -> Optional[Element]:
     """
     Return a DOM tree encoding the contents of an epytext string.  Any
     errors generated during parsing will be stored in C{errors}.
 
     @param text: The epytext string to parse.
     @param errors: A list where any errors generated during parsing
         will be stored.  If no list is specified, then fatal errors
         will generate exceptions, and non-fatal errors will be
         ignored.
     @return: a DOM tree encoding the contents of an epytext string,
         or C{None} if non-fatal errors were encountered and no C{errors}
         accumulator was provided.
     @raise ParseError: If C{errors} is C{None} and an error is
         encountered while parsing.
-    """
-    # Initialize errors list.
-    if errors is None:
-        errors = []
-        raise_on_error = True
-    else:
-        raise_on_error = False
-    
+    """    
     # Preprocess the string.
     text = re.sub('\015\012', '\012', text)
     text = text.expandtabs()
 
     # Tokenize the input string.
     tokens = _tokenize(text, errors)
 
@@ -376,19 +362,18 @@
         elif encountered_field:
             if len(stack) <= 3:
                 estr = ("Fields must be the final elements in an "+
                         "epytext string.")
                 errors.append(StructuringError(estr, token.startline))
 
     # If there was an error, then signal it!
-    if any(e.is_fatal() for e in errors):
-        if raise_on_error:
-            raise errors[0]
-        else:
-            return None
+    try:
+        raise next(e for e in errors if e.is_fatal())
+    except StopIteration:
+        pass
 
     # Return the top-level epytext DOM element.
     return doc
 
 def _pop_completed_blocks(
         token: 'Token',
         stack: List[Element],
@@ -1264,23 +1249,22 @@
                      + '...')
         return f"{self._descr}\n\n{left}{right}\n{' '*len(left)}^"
 
 #################################################################
 ##                    SUPPORT FOR EPYDOC
 #################################################################
 
-def parse_docstring(docstring: str, errors: List[ParseError], processtypes: bool = False) -> ParsedDocstring:
+def parse_docstring(docstring: str, errors: List[ParseError]) -> ParsedDocstring:
     """
     Parse the given docstring, which is formatted using epytext; and
     return a L{ParsedDocstring} representation of its contents.
 
     @param docstring: The docstring to parse
     @param errors: A list where any errors generated during parsing
         will be stored.
-    @param processtypes: Use L{ParsedTypeDocstring} to parsed 'type' fields.
     """
     tree = parse(docstring, errors)
     if tree is None:
         return ParsedEpytextDocstring(None, ())
 
     tree_children = cast(List[Element], tree.children)
 
@@ -1299,33 +1283,25 @@
                 arg: Optional[str] = \
                     cast(str, cast(Element, field.children.pop(0)).children[0])
             else:
                 arg = None
 
             # Process the field.
             field.tag = 'epytext'
-
             field_parsed_doc: ParsedDocstring = ParsedEpytextDocstring(field, ())
-
             lineno = int(field.attribs['lineno'])
-            
-            # This allows epytext markup to use TypeDocstring as well with a CLI option: --process-types
-            if processtypes and tag in ParsedTypeDocstring.FIELDS:
-                field_parsed_doc = ParsedTypeDocstring(field_parsed_doc.to_node(), lineno=lineno)
-                append_warnings(field_parsed_doc.warnings, errors, lineno=lineno)
-            
             fields.append(Field(tag, arg, field_parsed_doc, lineno))
 
     # Save the remaining docstring as the description.
     if tree_children and tree_children[0].children:
         return ParsedEpytextDocstring(tree, fields)
     else:
         return ParsedEpytextDocstring(None, fields)
 
-def get_parser(obj: Optional[Documentable]) -> Callable[[str, List[ParseError], bool], ParsedDocstring]:
+def get_parser(obj: Optional[Documentable]) -> ParserFunction:
     """
     Get the L{parse_docstring} function. 
     """
     return parse_docstring
 
 class ParsedEpytextDocstring(ParsedDocstring):
     SYMBOL_TO_CODEPOINT = {
@@ -1399,17 +1375,17 @@
         self._section_slugs.add(s)
         return s
 
     def to_node(self) -> nodes.document:
 
         if self._document is not None:
             return self._document
-        
-        self._document = utils.new_document('epytext')
-        
+
+        self._document = new_document('epytext')
+
         if self._tree is not None:
             node, = self._to_node(self._tree)
             # The contents is encapsulated inside a section node. 
             # Reparent the contents of the second level to the root level. 
             self._document = set_node_attributes(self._document, children=node.children)
         
         return self._document
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/google.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/google.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Parser for google-style docstrings. 
 
 @See: L{pydoctor.epydoc.markup.numpy}
 @See: L{pydoctor.epydoc.markup._napoleon}
 """
-from typing import Callable, List, Optional
+from typing import Optional
 from pydoctor.model import Documentable
-from pydoctor.epydoc.markup import ParseError, ParsedDocstring
+from pydoctor.epydoc.markup import ParserFunction
 from pydoctor.epydoc.markup._napoleon import NapoelonDocstringParser
 
 
-def get_parser(obj: Optional[Documentable]) -> Callable[[str, List[ParseError], bool], ParsedDocstring]:
+def get_parser(obj: Optional[Documentable]) -> ParserFunction:
     """
     Returns the parser function. Behaviour will depend on the documentable type and system options.
     """
     return NapoelonDocstringParser(obj).parse_google_docstring
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/numpy.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/numpy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Parser for numpy-style docstrings. 
 
 @See: L{pydoctor.epydoc.markup.google}
 @See: L{pydoctor.epydoc.markup._napoleon}
 """
-from typing import Callable, List, Optional
+from typing import Optional
 from pydoctor.model import Documentable
-from pydoctor.epydoc.markup import ParseError, ParsedDocstring
+from pydoctor.epydoc.markup import ParserFunction
 from pydoctor.epydoc.markup._napoleon import NapoelonDocstringParser
 
 
-def get_parser(obj: Optional[Documentable]) -> Callable[[str, List[ParseError], bool], ParsedDocstring]:
+def get_parser(obj: Optional[Documentable]) -> ParserFunction:
     """
     Returns the parser function. Behaviour will depend on the documentable type and system options.
     """
     return NapoelonDocstringParser(obj).parse_numpy_docstring
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/plaintext.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/plaintext.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 
 """
 Parser for plaintext docstrings.  Plaintext docstrings are rendered as
 verbatim output, preserving all whitespace.
 """
 __docformat__ = 'epytext en'
 
-from typing import List, Callable, Optional
+from typing import List, Optional
 
-from docutils import nodes, utils
+from docutils import nodes
 from twisted.web.template import Tag, tags
 
-from pydoctor.epydoc.markup import DocstringLinker, ParsedDocstring, ParseError
+from pydoctor.epydoc.markup import DocstringLinker, ParsedDocstring, ParseError, ParserFunction
 from pydoctor.model import Documentable
-from pydoctor.epydoc.docutils import set_node_attributes
+from pydoctor.epydoc.docutils import set_node_attributes, new_document
 
-def parse_docstring(docstring: str, errors: List[ParseError], processtypes: bool = False) -> ParsedDocstring:
+def parse_docstring(docstring: str, errors: List[ParseError]) -> ParsedDocstring:
     """
     Parse the given docstring, which is formatted as plain text; and
     return a L{ParsedDocstring} representation of its contents.
 
     @param docstring: The docstring to parse
     @param errors: A list where any errors generated during parsing
         will be stored.
     """
     return ParsedPlaintextDocstring(docstring)
 
-def get_parser(obj: Optional[Documentable]) -> Callable[[str, List[ParseError], bool], ParsedDocstring]:
+def get_parser(obj: Optional[Documentable]) -> ParserFunction:
     """
     Just return the L{parse_docstring} function. 
     """
     return parse_docstring
 
 class ParsedPlaintextDocstring(ParsedDocstring):
 
@@ -49,25 +49,25 @@
     def has_body(self) -> bool:
         return bool(self._text)
     
     # plaintext parser overrides the default to_stan() method for performance and design reasons. 
     # We don't want to use docutils to process the plaintext format because we won't 
     # actually use the document tree ,it does not contains any additionnalt information compared to the raw docstring. 
     # Also, the consolidated fields handling in restructuredtext.py relies on this "pre" class.
-    def to_stan(self, docstring_linker: DocstringLinker, compact:bool=False) -> Tag:
+    def to_stan(self, docstring_linker: DocstringLinker) -> Tag:
         return tags.p(self._text, class_='pre')
     
     def to_node(self) -> nodes.document:
         # This code is mainly used to generate summary of plaintext docstrings.
 
         if self._document is not None:
             return self._document
         else:
             # create document
-            _document = utils.new_document('plaintext')
+            _document = new_document('plaintext')
 
             # split text into paragraphs
             paragraphs = [set_node_attributes(nodes.paragraph('',''), children=[
                             set_node_attributes(nodes.Text(p.strip('\n')), document=_document, lineno=0)], 
                             document=_document, lineno=0)
                                 for p in self._text.split('\n\n')]
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/markup/restructuredtext.py` & `pydoctor-23.4.0/pydoctor/epydoc/markup/restructuredtext.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,29 +37,29 @@
 fields into individual fields.  The keys of C{CONSOLIDATED_FIELDS} are
 the names of possible consolidated fields; and the values are the
 names of the field tags that should be used for individual entries in
 the list.
 """
 __docformat__ = 'epytext en'
 
-from typing import Callable, Iterable, List, Optional, Sequence, Set, cast
+from typing import Iterable, List, Optional, Sequence, Set, cast
 import re
 from docutils import nodes
 
 from docutils.core import publish_string
 from docutils.writers import Writer
 from docutils.parsers.rst.directives.admonitions import BaseAdmonition # type: ignore[import]
 from docutils.readers.standalone import Reader as StandaloneReader
-from docutils.utils import Reporter, new_document
+from docutils.utils import Reporter
 from docutils.parsers.rst import Directive, directives
 from docutils.transforms import Transform, frontmatter
 
-from pydoctor.epydoc.markup import Field, ParseError, ParsedDocstring, append_warnings
+from pydoctor.epydoc.markup import Field, ParseError, ParsedDocstring, ParserFunction
 from pydoctor.epydoc.markup.plaintext import ParsedPlaintextDocstring
-from pydoctor.epydoc.markup._types import ParsedTypeDocstring
+from pydoctor.epydoc.docutils import new_document
 from pydoctor.model import Documentable
 
 #: A dictionary whose keys are the "consolidated fields" that are
 #: recognized by epydoc; and whose values are the corresponding epydoc
 #: field names that should be used for the individual fields.
 CONSOLIDATED_FIELDS = {
     'parameters': 'param',
@@ -77,25 +77,23 @@
 #: definition list, rather than a bulleted list.  For these fields, the
 #: 'classifier' for each term in the definition list is translated into
 #: a @type field.
 CONSOLIDATED_DEFLIST_FIELDS = ['param', 'arg', 'var', 'ivar', 'cvar', 'keyword']
 
 def parse_docstring(docstring: str, 
                     errors: List[ParseError], 
-                    processtypes: bool = False,
                     ) -> ParsedDocstring:
     """
     Parse the given docstring, which is formatted using
     ReStructuredText; and return a L{ParsedDocstring} representation
     of its contents.
 
     @param docstring: The docstring to parse
     @param errors: A list where any errors generated during parsing
         will be stored.
-    @param processtypes: Use L{ParsedTypeDocstring} to parsed 'type' fields.
     """
     writer = _DocumentPseudoWriter()
     reader = _EpydocReader(errors) # Outputs errors to the list.
 
     # Credits: mhils - Maximilian Hils from the pdoc repository https://github.com/mitmproxy/pdoc
     # Strip Sphinx interpreted text roles for code references: :obj:`foo` -> `foo`
     docstring = re.sub(
@@ -104,20 +102,20 @@
 
     publish_string(docstring, writer=writer, reader=reader,
                    settings_overrides={'report_level':10000,
                                        'halt_level':10000,
                                        'warning_stream':None})
 
     document = writer.document
-    visitor = _SplitFieldsTranslator(document, errors, processtypes=processtypes)
+    visitor = _SplitFieldsTranslator(document, errors)
     document.walk(visitor)
 
     return ParsedRstDocstring(document, visitor.fields)
 
-def get_parser(obj:Documentable) -> Callable[[str, List[ParseError], bool], ParsedDocstring]:
+def get_parser(obj:Documentable) -> ParserFunction:
     """
     Get the L{parse_docstring} function. 
     """
     return parse_docstring
 
 class OptimizedReporter(Reporter):
     """A reporter that ignores all debug messages.  This is used to
@@ -219,20 +217,19 @@
     ALLOW_UNMARKED_ARG_IN_CONSOLIDATED_FIELD = True
     """If true, then consolidated fields are not required to mark
     arguments with C{`backticks`}.  (This is currently only
     implemented for consolidated fields expressed as definition lists;
     consolidated fields expressed as unordered lists still require
     backticks for now."""
 
-    def __init__(self, document: nodes.document, errors: List[ParseError], processtypes: bool = False):
+    def __init__(self, document: nodes.document, errors: List[ParseError]):
         nodes.NodeVisitor.__init__(self, document)
         self._errors = errors
         self.fields: List[Field] = []
         self._newfields: Set[str] = set()
-        self._processtypes = processtypes
 
     def visit_document(self, node: nodes.Node) -> None:
         self.fields = []
 
     def visit_field(self, node: nodes.Node) -> None:
         # Remove the field from the tree.
         node.parent.remove(node)
@@ -277,22 +274,15 @@
             arg: Optional[str],
             fbody: Iterable[nodes.Node],
             lineno: int
             ) -> None:
         field_doc = self.document.copy()
         for child in fbody: 
             field_doc.append(child)
-
-        # This allows restructuredtext markup to use TypeDocstring as well with a CLI option: --process-types
-        field_parsed_doc: ParsedDocstring
-        if self._processtypes and tagname in ParsedTypeDocstring.FIELDS:
-            field_parsed_doc = ParsedTypeDocstring(field_doc)
-            append_warnings(field_parsed_doc.warnings, self._errors, lineno=lineno)
-        else:
-            field_parsed_doc = ParsedRstDocstring(field_doc, ())
+        field_parsed_doc = ParsedRstDocstring(field_doc, ())
         self.fields.append(Field(tagname, arg, field_parsed_doc, lineno - 1))
 
     def visit_field_list(self, node: nodes.Node) -> None:
         # Remove the field list from the tree.  The visitor will still walk
         # over the node's children.
         node.parent.remove(node)
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc/sre_parse36.py` & `pydoctor-23.4.0/pydoctor/epydoc/sre_parse36.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 # See the sre.py file for information on usage and redistribution.
 #
 
 """Internal support module for sre"""
 
 # XXX: show string offset and offending character for all errors
 
-from sre_constants import *
+from .sre_constants36 import *
 
 SPECIAL_CHARS = ".\\[{()*+?^$|"
 REPEAT_CHARS = "*+?{"
 
 DIGITS = frozenset("0123456789")
 
 OCTDIGITS = frozenset("01234567")
```

### Comparing `pydoctor-22.9.1/pydoctor/epydoc2stan.py` & `pydoctor-23.4.0/pydoctor/epydoc2stan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Convert L{pydoctor.epydoc} parsed markup into renderable content.
 """
 
 from collections import defaultdict
+import enum
 from typing import (
-    TYPE_CHECKING, Any, Callable, ClassVar, DefaultDict, Dict, Generator, 
-    Iterator, List, Mapping, Optional, Sequence, Tuple, 
+    TYPE_CHECKING, Any, Callable, ClassVar, DefaultDict, Dict, Generator,
+    Iterator, List, Mapping, Optional, Sequence, Tuple,
 )
 import ast
 import re
 
 import attr
 
 from pydoctor import model, linker, node2stan
-from pydoctor.epydoc.markup import Field as EpydocField, ParseError, get_parser_by_name
+from pydoctor.astutils import is_none_literal
+from pydoctor.epydoc.markup import Field as EpydocField, ParseError, get_parser_by_name, processtypes
 from twisted.web.template import Tag, tags
 from pydoctor.epydoc.markup import ParsedDocstring, DocstringLinker
 import pydoctor.epydoc.markup.plaintext
 from pydoctor.epydoc.markup._pyval_repr import colorize_pyval, colorize_inline_pyval
 
 if TYPE_CHECKING:
     from twisted.web.template import Flattenable
@@ -25,56 +27,27 @@
 taglink = linker.taglink
 """
 Alias to L{pydoctor.linker.taglink()}.
 """
 
 BROKEN = tags.p(class_="undocumented")('Broken description')
 
-def get_parser(obj: model.Documentable) -> Callable[[str, List[ParseError], bool], ParsedDocstring]:
+def _get_docformat(obj: model.Documentable) -> str:
     """
-    Get the C{parse_docstring(str, List[ParseError], bool) -> ParsedDocstring} function. 
-    """    
-    # Use module's __docformat__ if specified, else use system's. 
+    Returns the docformat to use to parse the docstring of this object.
+    """
+    # Use module's __docformat__ if specified, else use system's.
     # Except if system's docformat is plaintext, in this case, use plaintext.
     # See https://github.com/twisted/pydoctor/issues/503 for the reason
-    # of this behavior. 
+    # of this behavior.
     if obj.system.options.docformat == 'plaintext':
-        return pydoctor.epydoc.markup.plaintext.parse_docstring
+        return 'plaintext'
     # the docstring should be parsed using the format of the module it was inherited from
     docformat = obj.module.docformat or obj.system.options.docformat
-    
-    try:
-        return get_parser_by_name(docformat, obj)
-    except ImportError as e:
-        msg = 'Error trying to import %r parser:\n\n    %s: %s\n\nUsing plain text formatting only.'%(
-            docformat, e.__class__.__name__, e)
-        obj.system.msg('epydoc2stan', msg, thresh=-1, once=True)
-        return pydoctor.epydoc.markup.plaintext.parse_docstring
-
-
-def get_docstring(
-        obj: model.Documentable
-        ) -> Tuple[Optional[str], Optional[model.Documentable]]:
-    """
-    Fetch the docstring for a documentable. 
-    Treat empty docstring as undocumented.
-
-    :returns: 
-        - C{(docstring, source)} if the object is documented.
-        - C{(None, None)} if the object has no docstring (even inherited).
-        - C{(None, source)} if the object has an empty docstring.
-    """
-    for source in obj.docsources():
-        doc = source.docstring
-        if doc:
-            return doc, source
-        if doc is not None:
-            # Treat empty docstring as undocumented.
-            return None, source
-    return None, None
+    return docformat
 
 @attr.s(auto_attribs=True)
 class FieldDesc:
     """
     Combines informations from multiple L{Field} objects into one.
 
     Example::
@@ -121,14 +94,19 @@
             #  <name>: <type> | <desc>
             yield tags.td(class_="fieldArgContainer")(*fieldNameTd)
             yield tags.td(class_="fieldArgDesc")(formatted)
         else:
             #  <desc>
             yield tags.td(formatted, colspan="2")
 
+@attr.s(auto_attribs=True)
+class SignatureDesc(FieldDesc):
+    type_origin: Optional['FieldOrigin'] = None
+
+
 class RaisesDesc(FieldDesc):
     """Description of an exception that can be raised by function/method."""
 
     def format(self) -> Generator[Tag, None, None]:
         assert self.type is not None  # TODO: Why can't it be None?
         yield tags.td(tags.code(self.type), class_="fieldArgContainer")
         yield tags.td(self.body or self._UNDOCUMENTED)
@@ -199,15 +177,15 @@
             source=source,
             lineno=field.lineno,
             body=field.body()
             )
 
     def format(self) -> Tag:
         """Present this field's body as HTML."""
-        return safe_to_stan(self.body, self.source.docstring_linker, self.source, compact=True, 
+        return safe_to_stan(self.body, self.source.docstring_linker, self.source,
                     # the parsed docstring maybe doesn't support to_node(), i.e. ParsedTypeDocstring,
                     # so we can only show the broken text.
                     fallback=lambda _, __, ___:BROKEN)
 
     def report(self, message: str) -> None:
         self.source.report(message, lineno_offset=self.lineno, section='docstring')
 
@@ -236,108 +214,121 @@
     for field in fields:
         row = tags.tr()
         row(tags.td(colspan="2")(field.format()))
         yield row
 
 class VariableArgument(str):
     """
-    Encapsulate the name of C{vararg} parameters.
+    Encapsulate the name of C{vararg} parameters in L{Function.annotations} mapping keys.
     """
 
 class KeywordArgument(str):
     """
-    Encapsulate the name of C{kwarg} parameters.
+    Encapsulate the name of C{kwarg} parameters in L{Function.annotations} mapping keys.
     """
 
+class FieldOrigin(enum.Enum):
+    FROM_AST = 0
+    FROM_DOCSTRING = 1
+
+@attr.s(auto_attribs=True)
+class ParamType:
+    stan: Tag
+    origin: FieldOrigin
+
 class FieldHandler:
 
     def __init__(self, obj: model.Documentable):
         self.obj = obj
         self._linker = self.obj.docstring_linker
 
-        self.types: Dict[str, Optional[Tag]] = {}
+        self.types: Dict[str, Optional[ParamType]] = {}
 
-        self.parameter_descs: List[FieldDesc] = []
-        self.return_desc: Optional[FieldDesc] = None
-        self.yields_desc: Optional[FieldDesc] = None 
+        self.parameter_descs: List[SignatureDesc] = []
+        self.return_desc: Optional[SignatureDesc] = None
+        self.yields_desc: Optional[FieldDesc] = None
         self.raise_descs: List[RaisesDesc] = []
-        self.warns_desc: List[FieldDesc] = [] 
+        self.warns_desc: List[FieldDesc] = []
         self.seealsos: List[Field] = []
         self.notes: List[Field] = []
         self.authors: List[Field] = []
         self.sinces: List[Field] = []
         self.unknowns: DefaultDict[str, List[FieldDesc]] = defaultdict(list)
 
     def set_param_types_from_annotations(
             self, annotations: Mapping[str, Optional[ast.expr]]
             ) -> None:
         formatted_annotations = {
             name: None if value is None
-                       else safe_to_stan(colorize_inline_pyval(value), self.obj.docstring_linker, 
-                                self.obj, compact=True, fallback=colorized_pyval_fallback, section='annotation')
+                       else ParamType(safe_to_stan(colorize_inline_pyval(value), self.obj.docstring_linker,
+                                self.obj, fallback=colorized_pyval_fallback, section='annotation', report=False),
+                                # don't spam the log, invalid annotation are going to be reported when the signature gets colorized
+                                origin=FieldOrigin.FROM_AST)
+
             for name, value in annotations.items()
             }
         ret_type = formatted_annotations.pop('return', None)
         self.types.update(formatted_annotations)
         if ret_type is not None:
             # In most cases 'None' is not an actual return type, but the absence
             # of a returned value. Not storing it is the easiest way to prevent
             # it from being presented.
             ann_ret = annotations['return']
             assert ann_ret is not None  # ret_type would be None otherwise
-            if not _is_none_literal(ann_ret):
-                self.return_desc = FieldDesc(type=ret_type)
+            if not is_none_literal(ann_ret):
+                self.return_desc = SignatureDesc(type=ret_type.stan, type_origin=ret_type.origin)
 
     @staticmethod
     def _report_unexpected_argument(field:Field) -> None:
         if field.arg is not None:
             field.report('Unexpected argument in %s field' % (field.tag,))
 
     def handle_return(self, field: Field) -> None:
         self._report_unexpected_argument(field)
         if not self.return_desc:
-            self.return_desc = FieldDesc()
+            self.return_desc = SignatureDesc()
         self.return_desc.body = field.format()
     handle_returns = handle_return
 
     def handle_yield(self, field: Field) -> None:
         self._report_unexpected_argument(field)
         if not self.yields_desc:
             self.yields_desc = FieldDesc()
         self.yields_desc.body = field.format()
     handle_yields = handle_yield
 
     def handle_returntype(self, field: Field) -> None:
         self._report_unexpected_argument(field)
         if not self.return_desc:
-            self.return_desc = FieldDesc()
+            self.return_desc = SignatureDesc()
         self.return_desc.type = field.format()
+        self.return_desc.type_origin = FieldOrigin.FROM_DOCSTRING
     handle_rtype = handle_returntype
 
     def handle_yieldtype(self, field: Field) -> None:
         self._report_unexpected_argument(field)
         if not self.yields_desc:
             self.yields_desc = FieldDesc()
         self.yields_desc.type = field.format()
     handle_ytype = handle_yieldtype
 
     def _handle_param_name(self, field: Field) -> Optional[str]:
         name = field.arg
         if name is None:
             field.report('Parameter name missing')
             return None
-        
+
         name = name.lstrip('*')
         annotations = None
         if isinstance(field.source, model.Function):
             annotations = field.source.annotations
         elif isinstance(field.source, model.Class):
             # Constructor parameters can be documented on the class.
             annotations = field.source.constructor_params
-        # This might look useless, but it's needed in order to keep the 
+        # This might look useless, but it's needed in order to keep the
         # right str type: str, VariableArgument or KeyowrdArgument. And then add the stars accordingly.
         if annotations is not None:
             for param_name, _ in annotations.items():
                 if param_name == name:
                     name = param_name
         return name
 
@@ -379,32 +370,32 @@
             # Note: extract_fields() will issue warnings about missing field
             #       names, so we can silently ignore them here.
             # TODO: Processing the fields once in extract_fields() and again
             #       in format_docstring() adds complexity and can cause
             #       inconsistencies.
             name = field.arg
         if name is not None:
-            self.types[name] = field.format()
+            self.types[name] = ParamType(field.format(), origin=FieldOrigin.FROM_DOCSTRING)
 
     def handle_param(self, field: Field) -> None:
         name = self._handle_param_name(field)
         if name is not None:
             if any(desc.name == name for desc in self.parameter_descs):
                 field.report('Parameter "%s" was already documented' % (name,))
-            self.parameter_descs.append(FieldDesc(name=name, body=field.format()))
+            self.parameter_descs.append(SignatureDesc(name=name, body=field.format()))
             if name not in self.types:
                 self._handle_param_not_found(name, field)
 
     handle_arg = handle_param
 
     def handle_keyword(self, field: Field) -> None:
         name = self._handle_param_name(field)
         if name is not None:
             # TODO: How should this be matched to the type annotation?
-            self.parameter_descs.append(FieldDesc(name=name, body=field.format()))
+            self.parameter_descs.append(SignatureDesc(name=name, body=field.format()))
             if name in self.types:
                 field.report('Parameter "%s" is documented as keyword' % (name,))
 
 
     def handled_elsewhere(self, field: Field) -> None:
         # Some fields are handled by extract_fields below.
         pass
@@ -420,24 +411,24 @@
             typ_fmt = tags.span(class_='undocumented')("Unknown exception")
         else:
             typ_fmt = self._linker.link_to(name, name)
         self.raise_descs.append(RaisesDesc(type=typ_fmt, body=field.format()))
     handle_raise = handle_raises
     handle_except = handle_raises
 
-    # Warns is just like raises but the syntax is more relax i.e. warning type not required. 
+    # Warns is just like raises but the syntax is more relax i.e. warning type not required.
     def handle_warns(self, field: Field) -> None:
         if field.arg is None:
             typ_fmt = None
         else:
             typ_fmt = self._linker.link_to(field.arg, field.arg)
         self.warns_desc.append(FieldDesc(type=typ_fmt, body=field.format()))
 
     handle_warn = handle_warns
-    
+
     def handle_seealso(self, field: Field) -> None:
         self.seealsos.append(field)
     handle_see = handle_seealso
 
     def handle_note(self, field: Field) -> None:
         self.notes.append(field)
 
@@ -460,47 +451,60 @@
         """Merge information from 'param' fields and AST analysis."""
 
         params = {param.name: param for param in self.parameter_descs}
         any_info = bool(params)
 
         # We create a new parameter_descs list to ensure the parameter order
         # matches the AST order.
-        new_parameter_descs = []
-        for index, (name, type_doc) in enumerate(self.types.items()):
+        new_parameter_descs: List[SignatureDesc] = []
+        for index, (name, param_type) in enumerate(self.types.items()):
             try:
                 param = params.pop(name)
             except KeyError:
+                # parameter is not documented with @param.
+
                 if index == 0:
                     # Strip 'self' or 'cls' from parameter table when it semantically makes sens.
                     if name=='self' and self.obj.kind is model.DocumentableKind.METHOD:
                         continue
                     if name=='cls' and self.obj.kind is model.DocumentableKind.CLASS_METHOD:
                         continue
-                    
-                param = FieldDesc(name=name, type=type_doc)
-                any_info |= type_doc is not None
+
+                param = SignatureDesc(name=name,
+                    type=param_type.stan if param_type else None,
+                    type_origin=param_type.origin if param_type else None,)
+
+                any_info |= param_type is not None
             else:
-                param.type = type_doc
+                param.type = param_type.stan if param_type else None
+                param.type_origin = param_type.origin if param_type else None
+
             new_parameter_descs.append(param)
 
         # Add any leftover parameters, which includes documented **kwargs keywords
         # and non-existing (but documented) parameters.
         new_parameter_descs += params.values()
 
-        # Only replace the descriptions if at least one parameter is documented
+        # Only update the descriptions if at least one parameter is documented
         # or annotated.
         if any_info:
             self.parameter_descs = new_parameter_descs
 
     def format(self) -> Tag:
         r: List[Tag] = []
 
-        r += format_desc_list('Parameters', self.parameter_descs)
-        if self.return_desc:
+        # Only include parameter or return sections if any are documented or any type are documented from @type fields.
+        include_params = False
+        if any((p.body or p.type_origin is FieldOrigin.FROM_DOCSTRING) for p in self.parameter_descs):
+            r += format_desc_list('Parameters', self.parameter_descs)
+            include_params = True
+
+        if self.return_desc and (include_params or self.return_desc.body or self.return_desc.type_origin is FieldOrigin.FROM_DOCSTRING):
             r += format_desc_list('Returns', [self.return_desc])
+
         if self.yields_desc:
             r += format_desc_list('Yields', [self.yields_desc])
 
         r += format_desc_list("Raises", self.raise_descs)
         r += format_desc_list("Warns", self.warns_desc)
         for s_p_l in (('Author', 'Authors', self.authors),
                       ('See Also', 'See Also', self.seealsos),
@@ -511,40 +515,35 @@
             r += format_desc_list(f"Unknown Field: {kind}", fieldlist)
 
         if any(r):
             return tags.table(class_='fieldTable')(r)
         else:
             return tags.transparent
 
-
-def _is_none_literal(node: ast.expr) -> bool:
-    """Does this AST node represent the literal constant None?"""
-    return isinstance(node, (ast.Constant, ast.NameConstant)) and node.value is None
-
 def reportWarnings(obj: model.Documentable, warns: Sequence[str], **kwargs:Any) -> None:
     for message in warns:
         obj.report(message, **kwargs)
 
 def reportErrors(obj: model.Documentable, errs: Sequence[ParseError], section:str='docstring') -> None:
     if not errs:
         return
-    
+
     errors = obj.system.parse_errors[section]
 
     if obj.fullName() not in errors:
         errors.add(obj.fullName())
-        
+
         for err in errs:
             obj.report(
                 f'bad {section}: ' + err.descr(),
                 lineno_offset=(err.linenum() or 1) - 1,
                 section=section
                 )
 
-
+_docformat_skip_processtypes = ('google', 'numpy', 'plaintext')
 def parse_docstring(
         obj: model.Documentable,
         doc: str,
         source: model.Documentable,
         markup: Optional[str]=None,
         section: str='docstring',
         ) -> ParsedDocstring:
@@ -554,39 +553,60 @@
     @param source: The object on which the docstring is defined.
         This can differ from C{obj} if the docstring is inherited.
     @param markup: Parse the docstring with the given markup, ignoring system's options.
         Useful for creating L{ParsedDocstring}s from restructuredtext for instance.
     @param section: A custom section to use.
     """
 
-    parser = get_parser(source) if not markup else get_parser_by_name(markup, obj)
+    docformat = _get_docformat(source) if not markup else markup
+
+    # fetch the parser function
+    try:
+        parser = get_parser_by_name(docformat, obj)
+    except ImportError as e:
+        _err = 'Error trying to import %r parser:\n\n    %s: %s\n\nUsing plain text formatting only.'%(
+            docformat, e.__class__.__name__, e)
+        obj.system.msg('epydoc2stan', _err, thresh=-1, once=True)
+        parser = pydoctor.epydoc.markup.plaintext.parse_docstring
+
+    # type processing is always enabled for google and numpy docformat,
+    # it's already part of the specification, doing it now would process types twice.
+    if obj.system.options.processtypes and docformat not in _docformat_skip_processtypes:
+        # This allows epytext and restructuredtext markup to use TypeDocstring as well with a CLI option: --process-types.
+        # It's still technically part of the parsing process, so we use a wrapper function.
+        parser = processtypes(parser)
+
     errs: List[ParseError] = []
     try:
-        parsed_doc = parser(doc, errs, obj.system.options.processtypes)
+        # parse docstring
+        parsed_doc = parser(doc, errs)
+    except ParseError:
+        # this error should already by stored in the errs list
+        parsed_doc = pydoctor.epydoc.markup.plaintext.parse_docstring(doc, errs)
     except Exception as e:
         errs.append(ParseError(f'{e.__class__.__name__}: {e}', 1))
         parsed_doc = pydoctor.epydoc.markup.plaintext.parse_docstring(doc, errs)
     if errs:
         reportErrors(source, errs, section=section)
     return parsed_doc
 
 def ensure_parsed_docstring(obj: model.Documentable) -> Optional[model.Documentable]:
     """
     Currently, it's not 100% clear at what point the L{Documentable.parsed_docstring} attribute is set.
     It can be set from the ast builder or later processing step.
-    
-    This function ensures that the C{parsed_docstring} attribute of a documentable is set to it's final value. 
 
-    @returns: 
-        - If the C{obj.parsed_docstring} is set to a L{ParsedDocstring} instance: 
-          The source object of the docstring (might be different 
+    This function ensures that the C{parsed_docstring} attribute of a documentable is set to it's final value.
+
+    @returns:
+        - If the C{obj.parsed_docstring} is set to a L{ParsedDocstring} instance:
+          The source object of the docstring (might be different
           from C{obj} if the documentation is inherited).
         - If the object is undocumented: C{None}.
     """
-    doc, source = get_docstring(obj)
+    doc, source = model.get_docstring(obj)
 
     # Use cached or split version if possible.
     parsed_doc = obj.parsed_docstring
 
     if source is None and parsed_doc is not None:
         # No docstring found
         # A split field is documented by its parent: meaning the parsed_docstring
@@ -595,87 +615,89 @@
         source = obj.parent
 
     if parsed_doc is None and doc is not None:
         # The parsed_docstring has not been initialized yet
         assert source is not None
         parsed_doc = parse_docstring(obj, doc, source)
         obj.parsed_docstring = parsed_doc
-    
+
     if obj.parsed_docstring is not None:
         return source
     else:
         return None
 
 
 class ParsedStanOnly(ParsedDocstring):
     """
     A L{ParsedDocstring} directly constructed from stan, for caching purposes.
-    
-    L{to_stan} method simply returns back what's given to L{ParsedStanOnly.__init__}. 
+
+    L{to_stan} method simply returns back what's given to L{ParsedStanOnly.__init__}.
     """
     def __init__(self, stan: Tag):
         super().__init__(fields=[])
         self._fromstan = stan
+
+    @property
     def has_body(self) -> bool:
         return True
-    def to_stan(self, docstring_linker: Any, compact:bool=False) -> Tag:
+
+    def to_stan(self, docstring_linker: Any) -> Tag:
         return self._fromstan
+
     def to_node(self) -> Any:
         raise NotImplementedError()
 
 def _get_parsed_summary(obj: model.Documentable) -> Tuple[Optional[model.Documentable], ParsedDocstring]:
     """
-    Ensures that the L{model.Documentable.parsed_summary} attribute of a documentable is set to it's final value. 
+    Ensures that the L{model.Documentable.parsed_summary} attribute of a documentable is set to it's final value.
     Do not generate summary twice.
-    
+
     @returns: Tuple: C{source}, C{parsed docstring}
     """
     source = ensure_parsed_docstring(obj)
-    
+
     if obj.parsed_summary is not None:
         return (source, obj.parsed_summary)
 
     if source is None:
         summary_parsed_doc: ParsedDocstring = ParsedStanOnly(format_undocumented(obj))
     else:
         # Tell mypy that if we found a docstring, we also have its source.
         assert obj.parsed_docstring is not None
         summary_parsed_doc = obj.parsed_docstring.get_summary()
-    
+
     obj.parsed_summary = summary_parsed_doc
 
     return (source, summary_parsed_doc)
 
 def get_to_stan_error(e: Exception) -> ParseError:
     return ParseError(f"{e.__class__.__name__}: {e}", 0)
 
-def safe_to_stan(parsed_doc: ParsedDocstring, 
+def safe_to_stan(parsed_doc: ParsedDocstring,
                  linker: 'DocstringLinker',
-                 ctx: model.Documentable, 
-                 compact: bool,
+                 ctx: model.Documentable,
                  fallback: Callable[[List[ParseError], ParsedDocstring, model.Documentable], Tag],
                  report: bool = True,
                  section:str='docstring') -> Tag:
     """
     Wraps L{ParsedDocstring.to_stan()} to catch exception and handle them in C{fallback}.
     This is used to convert docstrings as well as other colorized AST values to stan.
 
     @param parsed_doc: The L{ParsedDocstring} to "stanify".
     @param linker: The L{DocstringLinker} to use to resolve links.
     @param ctx: The documentable context to use to report errors, passed to the C{fallback} function.
-    @param compact: Whether the generated html should be compact.
     @param fallback: A callable that returns a fallback stan if the convertion failed.
         It can also be used to set some state on the documentable context.
         Signature::
             (errs:List[ParseError], doc:ParsedDocstring, ctx:model.Documentable) -> Tag
     @param report: Whether to report errors.
     @param section: Used for error messages.
     """
     try:
-        stan = parsed_doc.to_stan(linker, compact=compact)
+        stan = parsed_doc.to_stan(linker)
     except Exception as e:
         errs = [get_to_stan_error(e)]
         stan = fallback(errs, parsed_doc, ctx)
         if report:
             reportErrors(ctx, errs, section=section)
     return stan
 
@@ -683,31 +705,56 @@
     if ctx.docstring is None:
         stan = BROKEN
     else:
         parsed_doc_plain = pydoctor.epydoc.markup.plaintext.parse_docstring(ctx.docstring, errs)
         stan = parsed_doc_plain.to_stan(ctx.docstring_linker)
     return stan
 
+def _wrap_in_paragraph(body:Sequence["Flattenable"]) -> bool:
+    """
+    Whether to wrap the given docstring stan body inside a paragraph. 
+    """
+    has_paragraph = False
+    for e in body:
+        if isinstance(e, Tag) and e.tagName == 'p':
+            has_paragraph = True
+        # only check the first element of the body
+        break
+    return bool(len(body)>0 and not has_paragraph)
+
+def unwrap_docstring_stan(stan:Tag) -> "Flattenable":
+    """
+    Unwrap the body of the given C{Tag} instance if it has a non-empty tag name and 
+    ensure there is at least one paragraph. 
+
+    @note: This is the counterpart of what we're doing in L{HTMLTranslator.should_be_compact_paragraph()}.
+        Since the L{HTMLTranslator} is generic for all parsed docstrings types, it always generates compact paragraphs.
+
+        But for docstrings, we want to have at least one paragraph for consistency.
+    """
+    if stan.tagName:
+        return stan
+    body = stan.children
+    if _wrap_in_paragraph(body):
+        return tags.p(*body)
+    else:
+        return body
+
 def format_docstring(obj: model.Documentable) -> Tag:
     """Generate an HTML representation of a docstring"""
 
     source = ensure_parsed_docstring(obj)
 
     ret: Tag = tags.div
     if source is None:
         ret(tags.p(class_='undocumented')("Undocumented"))
     else:
         assert obj.parsed_docstring is not None, "ensure_parsed_docstring() did not do it's job"
-        stan = safe_to_stan(obj.parsed_docstring, source.docstring_linker, source, 
-                            compact=False, fallback=format_docstring_fallback)
-        
-        if stan.tagName:
-            ret(stan)
-        else:
-            ret(*stan.children)
+        stan = safe_to_stan(obj.parsed_docstring, source.docstring_linker, source, fallback=format_docstring_fallback)
+        ret(unwrap_docstring_stan(stan))
 
     fh = FieldHandler(obj)
     if isinstance(obj, model.Function):
         fh.set_param_types_from_annotations(obj.annotations)
     if source is not None:
         assert obj.parsed_docstring is not None, "ensure_parsed_docstring() did not do it's job"
         for field in obj.parsed_docstring.fields:
@@ -725,21 +772,21 @@
 
 def format_summary(obj: model.Documentable) -> Tag:
     """Generate an shortened HTML representation of a docstring."""
 
     source, parsed_doc = _get_parsed_summary(obj)
     if not source:
         source = obj
-
-    # Disallow same_page_optimization in order to make sure we're not
-    # breaking links when including the summaries on other pages.
-    with source.docstring_linker.disable_same_page_optimazation():
+    
+    # do not optimize url in order to make sure we're always generating full urls.
+    # avoids breaking links when including the summaries on other pages.
+    with source.docstring_linker.switch_context(None):
         # ParserErrors will likely be reported by the full docstring as well,
         # so don't spam the log, pass report=False.
-        stan = safe_to_stan(parsed_doc, source.docstring_linker, source, compact=True, report=False,
+        stan = safe_to_stan(parsed_doc, source.docstring_linker, source, report=False,
                 fallback=format_summary_fallback)
 
     return stan
 
 
 def format_undocumented(obj: model.Documentable) -> Tag:
     """Generate an HTML representation for an object lacking a docstring."""
@@ -751,60 +798,60 @@
         if kind is not None:
             sub_objects_total_count[kind] += 1
             if sub_ob.docstring is not None:
                 sub_objects_with_docstring_count[kind] += 1
 
     tag: Tag = tags.span(class_='undocumented')
     if sub_objects_with_docstring_count:
-        
+
         kind = obj.kind
         assert kind is not None # if kind is None, object is invisible
         tag(
             "No ", format_kind(kind).lower(), " docstring; ",
             ', '.join(
                 f"{sub_objects_with_docstring_count[kind]}/{sub_objects_total_count[kind]} "
                 f"{format_kind(kind, plural=sub_objects_with_docstring_count[kind]>=2).lower()}"
-                
+
                 for kind in sorted(sub_objects_total_count, key=(lambda x:x.value))
                 ),
             " documented"
             )
     else:
         tag("Undocumented")
     return tag
 
 
 def type2stan(obj: model.Documentable) -> Optional[Tag]:
     parsed_type = get_parsed_type(obj)
     if parsed_type is None:
         return None
     else:
-        return safe_to_stan(parsed_type, obj.docstring_linker, obj, compact=True, 
+        return safe_to_stan(parsed_type, obj.docstring_linker, obj,
             fallback=colorized_pyval_fallback, section='annotation')
 
 def get_parsed_type(obj: model.Documentable) -> Optional[ParsedDocstring]:
     parsed_type = obj.parsed_type
     if parsed_type is not None:
         return parsed_type
 
     annotation: Optional[ast.expr] = getattr(obj, 'annotation', None)
     if annotation is not None:
         return colorize_inline_pyval(annotation)
 
     return None
 
 def format_toc(obj: model.Documentable) -> Optional[Tag]:
-    # Load the parsed_docstring if it's not already done. 
+    # Load the parsed_docstring if it's not already done.
     ensure_parsed_docstring(obj)
 
     if obj.parsed_docstring:
         if obj.system.options.sidebartocdepth > 0:
             toc = obj.parsed_docstring.get_toc(depth=obj.system.options.sidebartocdepth)
             if toc:
-                return safe_to_stan(toc, obj.docstring_linker, obj, compact=True, report=False,
+                return safe_to_stan(toc, obj.docstring_linker, obj, report=False,
                     fallback=lambda _,__,___:BROKEN)
     return None
 
 
 field_name_to_kind = {
     'ivar': model.DocumentableKind.INSTANCE_VARIABLE,
     'cvar': model.DocumentableKind.CLASS_VARIABLE,
@@ -842,15 +889,15 @@
                 attrobj.parsed_type = field.body()
             else:
                 attrobj.parsed_docstring = field.body()
                 attrobj.kind = field_name_to_kind[tag]
 
 def format_kind(kind: model.DocumentableKind, plural: bool = False) -> str:
     """
-    Transform a `model.DocumentableKind` Enum value to string. 
+    Transform a `model.DocumentableKind` Enum value to string.
     """
     names = {
         model.DocumentableKind.PACKAGE         : 'Package',
         model.DocumentableKind.MODULE          : 'Module',
         model.DocumentableKind.INTERFACE       : 'Interface',
         model.DocumentableKind.CLASS           : 'Class',
         model.DocumentableKind.CLASS_METHOD    : 'Class Method',
@@ -865,15 +912,15 @@
         model.DocumentableKind.SCHEMA_FIELD    : 'Attribute',
         model.DocumentableKind.CONSTANT        : 'Constant',
         model.DocumentableKind.EXCEPTION       : 'Exception',
         model.DocumentableKind.TYPE_ALIAS      : 'Type Alias',
         model.DocumentableKind.TYPE_VARIABLE   : 'Type Variable',
     }
     plurals = {
-        model.DocumentableKind.CLASS           : 'Classes', 
+        model.DocumentableKind.CLASS           : 'Classes',
         model.DocumentableKind.PROPERTY        : 'Properties',
         model.DocumentableKind.TYPE_ALIAS      : 'Type Aliases',
     }
     if plural:
         return plurals.get(kind, names[kind] + 's')
     else:
         return names[kind]
@@ -887,20 +934,20 @@
 def _format_constant_value(obj: model.Attribute) -> Iterator["Flattenable"]:
 
     # yield the table title, "Value"
     row = tags.tr(class_="fieldStart")
     row(tags.td(class_="fieldName")("Value"))
     # yield the first row.
     yield row
-    
-    doc = colorize_pyval(obj.value, 
+
+    doc = colorize_pyval(obj.value,
         linelen=obj.system.options.pyvalreprlinelen,
         maxlines=obj.system.options.pyvalreprmaxlines)
-    
-    value_repr = safe_to_stan(doc, obj.docstring_linker, obj, compact=True, 
+
+    value_repr = safe_to_stan(doc, obj.docstring_linker, obj,
         fallback=colorized_pyval_fallback, section='rendering of constant')
 
     # Report eventual warnings. It warns when a regex failed to parse.
     reportWarnings(obj, doc.warnings, section='colorize constant')
 
     # yield the value repr.
     row = tags.tr()
@@ -920,39 +967,39 @@
         # We use \u200b as temp token to hack a split that passes the tests.
         return text.replace(sep, '\u200b'+sep).split('\u200b')
 
     match = re.match('(_{1,2})?(.*?)(_{1,2})?$', indentifier)
     assert match is not None # the regex always matches
     prefix, text, suffix = match.groups(default='')
     text_parts = []
-    
+
     if text.islower() or text.isupper():
         # We assume snake_case or SCREAMING_SNAKE_CASE.
         text_parts = split(text, '_')
     else:
         # We assume camelCase.  We're not using a regex because we also want it
         # to work with non-ASCII characters (and the Python re module does not
         # support checking for Unicode properties using something like \p{Lu}).
         current_part = ''
         previous_was_upper = False
         for c in text:
 
             if c.isupper() and not previous_was_upper:
                 text_parts.append(current_part)
                 current_part = ''
-            
+
             current_part += c
             previous_was_upper = c.isupper()
-        
+
         if current_part:
             text_parts.append(current_part)
 
     if not text_parts: # the name is composed only by underscores
         text_parts = ['']
-    
+
     if prefix:
         text_parts[0] = prefix + text_parts[0]
     if suffix:
         text_parts[-1] = text_parts[-1] + suffix
 
     return text_parts
 
@@ -963,20 +1010,87 @@
     word break opportunities.
 
     :note: It support full dotted names and will add a wbr tag after each dot.
     """
 
     # We use tags.wbr instead of zero-width spaces because
     # zero-width spaces can interfer in subtle ways when copy/pasting a name.
-    
+
     r: List['Flattenable'] = []
     parts = text.split('.')
     for i,t in enumerate(parts):
         _parts = _split_indentifier_parts_on_case(t)
         for i_,p in enumerate(_parts):
             r += [p]
             if i_ != len(_parts)-1:
                 r += [tags.wbr()]
         if i != len(parts)-1:
             r += [tags.wbr(), '.']
     return tags.transparent(*r)
 
+def format_constructor_short_text(constructor: model.Function, forclass: model.Class) -> str:
+    """
+    Returns a simplified signature of the constructor.
+    C{forclass} is not always the function's parent, it can be a subclass.
+    """
+    args = ''
+    # for signature with more than 5 parameters, 
+    # we just show the elipsis after the fourth parameter
+    annotations = constructor.annotations.items()
+    many_param = len(annotations) > 6
+    
+    for index, (name, ann) in enumerate(annotations):
+        if name=='return':
+            continue
+
+        if many_param and index > 4:
+            args += ', ...'
+            break
+        
+        # Special casing __new__ because it's actually a static method
+        if index==0 and (constructor.name in ('__new__', '__init__') or 
+                         constructor.kind is model.DocumentableKind.CLASS_METHOD):
+            # Omit first argument (self/cls) from simplified signature.
+            continue
+        star = ''
+        if isinstance(name, VariableArgument):
+            star='*'
+        elif isinstance(name, KeywordArgument):
+            star='**'
+        
+        if args:
+            args += ', '
+        
+        args += f"{star}{name}"
+    
+    # display innner classes with their name starting at the top level class.
+    _current:model.CanContainImportsDocumentable = forclass
+    class_name = [] 
+    while isinstance(_current, model.Class):
+        class_name.append(_current.name)
+        _current = _current.parent
+    
+    callable_name = '.'.join(reversed(class_name))
+
+    if constructor.name not in ('__new__', '__init__'):
+        # We assume that the constructor is a method accessible in the Class.
+
+        callable_name += f'.{constructor.name}'
+
+    return f"{callable_name}({args})"
+
+def populate_constructors_extra_info(cls:model.Class) -> None:
+    """
+    Adds an extra information to be rendered based on Class constructors.
+    """
+    from pydoctor.templatewriter import util
+    constructors = cls.public_constructors
+    if constructors:
+        plural = 's' if len(constructors)>1 else ''
+        extra_epytext = f'Constructor{plural}: '
+        for i, c in enumerate(sorted(constructors, key=util.objects_order)):
+            if i != 0:
+                extra_epytext += ', '
+            short_text = format_constructor_short_text(c, cls)
+            extra_epytext += '`%s <%s>`' % (short_text, c.fullName())
+        
+        cls.extra_info.append(parse_docstring(cls, extra_epytext, cls, 'restructuredtext', section='constructor extra'))
```

### Comparing `pydoctor-22.9.1/pydoctor/extensions/__init__.py` & `pydoctor-23.4.0/pydoctor/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/extensions/attrs.py` & `pydoctor-23.4.0/pydoctor/extensions/attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Support for L{attrs <attr>}.
+Support for L{attrs}.
 """
 
 import ast
 import inspect
 
 from typing import Optional, Union
 
@@ -161,14 +161,14 @@
 
 class AttrsClass(extensions.ClassMixin, model.Class):
     
     def setup(self) -> None:
         super().setup()
         self.auto_attribs: bool = False
         """
-        L{True} if this class uses the C{auto_attribs} feature of the L{attrs <attr>}
+        L{True} if this class uses the C{auto_attribs} feature of the L{attrs}
         library to automatically convert annotated fields into attributes.
         """
 
 def setup_pydoctor_extension(r:extensions.ExtRegistrar) -> None:
     r.register_astbuilder_visitor(ModuleVisitor)
     r.register_mixin(AttrsClass)
```

### Comparing `pydoctor-22.9.1/pydoctor/extensions/deprecate.py` & `pydoctor-23.4.0/pydoctor/extensions/deprecate.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 """
 Support for L{twisted.python.deprecate}.
 """
 
 import ast
 import inspect
-from numbers import Number
 from typing import Optional, Sequence, Tuple, Union, TYPE_CHECKING
 
 from pydoctor import astbuilder, model, epydoc2stan, astutils, extensions
 
 from twisted.python.deprecate import deprecated
 from incremental import Version
 
@@ -82,21 +81,24 @@
     Change an AST C{Version()} to a real one.
 
     @note: Only use required arguments, ignores arguments release_candidate, prerelease, post, dev.
     @raises ValueError: If the incremental.Version call is invalid.
     """
     bound_args = astutils.bind_args(_incremental_Version_signature, version)
     package = astutils.get_str_value(bound_args.arguments['package'])
-    major: Union[Number, str, None] = astutils.get_num_value(bound_args.arguments['major']) or \
+    major: Union[int, str, None] = astutils.get_int_value(bound_args.arguments['major']) or \
         astutils.get_str_value(bound_args.arguments['major'])
-    if isinstance(major, str) and major != "NEXT": 
+    if major is None or (isinstance(major, str) and major != "NEXT"): 
         raise ValueError("Invalid call to incremental.Version(), 'major' should be an int or 'NEXT'.")
-    return Version(package, major, 
-        minor=astutils.get_num_value(bound_args.arguments['minor']),
-        micro=astutils.get_num_value(bound_args.arguments['micro']),)
+    assert isinstance(major, (int, str))
+    minor = astutils.get_int_value(bound_args.arguments['minor'])
+    micro = astutils.get_int_value(bound_args.arguments['micro'])
+    if minor is None or micro is None:
+        raise ValueError("Invalid call to incremental.Version(), 'minor' and 'micro' should be an ints.")
+    return Version(package, major, minor=minor, micro=micro) # type:ignore[arg-type]
 
 _deprecation_text_with_replacement_template = "``{name}`` was deprecated in {package} {version}; please use `{replacement}` instead."
 _deprecation_text_without_replacement_template = "``{name}`` was deprecated in {package} {version}."
 
 _deprecated_signature = inspect.signature(deprecated)
 def deprecatedToUsefulText(ctx:model.Documentable, name:str, deprecated:ast.Call) -> Tuple[str, str]:
     """
```

### Comparing `pydoctor-22.9.1/pydoctor/extensions/zopeinterface.py` & `pydoctor-23.4.0/pydoctor/extensions/zopeinterface.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/factory.py` & `pydoctor-23.4.0/pydoctor/factory.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/model.py` & `pydoctor-23.4.0/pydoctor/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 (subclasses of) L{Documentable} represent the documentable 'things' in the
 system being documented.  An instance of L{System} represents the whole system
 being documented -- a System is a bad of Documentables, in some sense.
 """
 
 import abc
 import ast
+import attr
 from collections import defaultdict
 import datetime
 import importlib
-import inspect
 import platform
 import sys
 import textwrap
 import types
 from enum import Enum
 from inspect import signature, Signature
 from pathlib import Path
@@ -27,19 +27,19 @@
 
 from pydoctor.options import Options
 from pydoctor import factory, qnmatch, utils, linker, astutils, mro
 from pydoctor.epydoc.markup import ParsedDocstring
 from pydoctor.sphinx import CacheT, SphinxInventory
 
 if TYPE_CHECKING:
-    from typing_extensions import Literal
+    from typing_extensions import Literal, Protocol
     from pydoctor.astbuilder import ASTBuilder, DocumentableT
 else:
     Literal = {True: bool, False: bool}
-    ASTBuilder = object
+    ASTBuilder = Protocol = object
 
 
 # originally when I started to write pydoctor I had this idea of a big
 # tree of Documentables arranged in an almost arbitrary tree.
 #
 # this was misguided.  the tree structure is important, to be sure,
 # but the arrangement of the tree is far from arbitrary and there is
@@ -155,32 +155,16 @@
         return self
 
     def setup(self) -> None:
         self.contents: Dict[str, Documentable] = {}
         self._linker: Optional['linker.DocstringLinker'] = None
 
     def setDocstring(self, node: ast.Str) -> None:
-        doc = node.s
-        lineno = node.lineno
-        if _string_lineno_is_end:
-            # In older CPython versions, the AST only tells us the end line
-            # number and we must approximate the start line number.
-            # This approximation is correct if the docstring does not contain
-            # explicit newlines ('\n') or joined lines ('\' at end of line).
-            lineno -= doc.count('\n')
-
-        # Leading blank lines are stripped by cleandoc(), so we must
-        # return the line number of the first non-blank line.
-        for ch in doc:
-            if ch == '\n':
-                lineno += 1
-            elif not ch.isspace():
-                break
-
-        self.docstring = inspect.cleandoc(doc)
+        lineno, doc = astutils.extract_docstring(node)
+        self.docstring = doc
         self.docstring_lineno = lineno
 
     def setLineNumber(self, lineno: int) -> None:
         if not self.linenumber:
             self.linenumber = lineno
             parentMod = self.parentMod
             if parentMod is not None:
@@ -401,19 +385,19 @@
             f'{self.description}:{linenumber}: {descr}',
             thresh=thresh)
 
     @property
     def docstring_linker(self) -> 'linker.DocstringLinker':
         """
         Returns an instance of L{DocstringLinker} suitable for resolving names
-        in the context of the object scope. 
+        in the context of the object. 
         """
         if self._linker is not None:
             return self._linker
-        self._linker = linker._CachedEpydocLinker(self)
+        self._linker = linker._EpydocLinker(self)
         return self._linker
 
 
 class CanContainImportsDocumentable(Documentable):
     def setup(self) -> None:
         super().setup()
         self._localNameToFullName_map: Dict[str, str] = {}
@@ -581,41 +565,102 @@
         if isinstance(o, str):
             return []
         return list(localbases(o))
 
     init_finalbaseobjects(cls)
     return mro.mro(cls, getbases)
 
+def _find_dunder_constructor(cls:'Class') -> Optional['Function']:
+    """
+    Find the a non-default python-powered dunder constructor.
+    Returns C{None} if neither C{__new__} or C{__init__} are defined.
+
+    @note: C{__new__} takes precedence orver C{__init__}. 
+        More infos: U{https://docs.python.org/3/reference/datamodel.html#object.__new__}
+    """
+    _new = cls.find('__new__')
+    if isinstance(_new, Function):
+        return _new
+    elif _new is None:
+        _init = cls.find('__init__')
+        if isinstance(_init, Function):
+            return _init
+    return None
+
 class Class(CanContainImportsDocumentable):
     kind = DocumentableKind.CLASS
     parent: CanContainImportsDocumentable
     decorators: Sequence[Tuple[str, Optional[Sequence[ast.expr]]]]
-    
+
     # set in post-processing:
     _finalbaseobjects: Optional[List[Optional['Class']]] = None 
     _finalbases: Optional[List[str]] = None
     _mro: Optional[List[Union['Class', str]]] = None
 
     def setup(self) -> None:
         super().setup()
         self.rawbases: Sequence[Tuple[str, ast.expr]] = []
         self.raw_decorators: Sequence[ast.expr] = []
         self.subclasses: List[Class] = []
+        self.constructors: List[Function] = []
+        """
+        List of constructors.
+
+        Makes the assumption that the constructor name is available in the locals of the class
+        it's supposed to create. Typically with C{__init__} and C{__new__} it's always the case. 
+        It means that no regular function can be interpreted as a constructor for a given class.
+        """
         self._initialbases: List[str] = []
         self._initialbaseobjects: List[Optional['Class']] = []
     
     def _init_mro(self) -> None:
         """
         Compute the correct value of the method resolution order returned by L{mro()}.
         """
         try:
             self._mro = compute_mro(self)
         except ValueError as e:
             self.report(str(e), 'mro')
             self._mro = list(self.allbases(True))
+    
+    def _init_constructors(self) -> None:
+        """
+        Initiate the L{Class.constructors} list. A constructor MUST be a method accessible 
+        in the locals of the class.
+        """
+        # Look for python language powered constructors.
+        # If __new__ is defined, then it takes precedence over __init__
+        # Blind spot: we don't understand when a Class is using a metaclass that overrides __call__.
+        dunder_constructor = _find_dunder_constructor(self)
+        if dunder_constructor:
+            self.constructors.append(dunder_constructor)
+        
+        # Then look for staticmethod/classmethod constructors,
+        # This only happens at the local scope level (i.e not looking in super-classes).
+        for fun in self.contents.values():
+            if not isinstance(fun, Function):
+                continue
+            # Only static methods and class methods can be recognized as constructors
+            if not fun.kind in (DocumentableKind.STATIC_METHOD, DocumentableKind.CLASS_METHOD):
+                continue
+            # get return annotation, if it returns the same type as self, it's a constructor method.
+            if not 'return' in fun.annotations:
+                # we currently only support constructor detection trought explicit annotations.
+                continue 
+            
+            # annotation should be resolved at the module scope
+            return_ann = astutils.node2fullname(fun.annotations['return'], self.module)
+            
+            # pydoctor understand explicit annotation as well as the Self-Type.
+            if return_ann == self.fullName() or \
+               return_ann in ('typing.Self', 'typing_extensions.Self'):
+                self.constructors.append(fun)
+        
+        from pydoctor import epydoc2stan
+        epydoc2stan.populate_constructors_extra_info(self)
 
     @overload
     def mro(self, include_external:'Literal[True]', include_self:bool=True) -> List[Union['Class', str]]:...
     @overload
     def mro(self, include_external:'Literal[False]'=False, include_self:bool=True) -> List['Class']:...
     def mro(self, include_external:bool=False, include_self:bool=True) -> List[Union['Class', str]]: # type:ignore[misc]
         """
@@ -654,14 +699,40 @@
             It's computed another time in post-processing to try to resolve the names that could not be resolved the first time. This is needed when there are import cycles. 
             
             Meaning depending on the state of the system, this property can return either the initial objects or the final objects
         """
         return self._finalbaseobjects if \
             self._finalbaseobjects is not None else self._initialbaseobjects
     
+    @property
+    def public_constructors(self) -> Sequence['Function']:
+        """
+        Yields public constructors for this class.
+        A public constructor must not be hidden and have
+        arguments or have a docstring.
+        """
+        r = []
+        for c in self.constructors:
+            if not c.isVisible:
+                continue
+            args = list(c.annotations)
+            try: args.remove('return')
+            except ValueError: pass
+            if c.kind in (DocumentableKind.CLASS_METHOD, 
+                          DocumentableKind.METHOD):
+                try:
+                    args.pop(0)
+                except IndexError:
+                    pass
+            if (len(args)==0 and get_docstring(c)[0] is None and 
+                c.name in ('__init__', '__new__')):
+                continue
+            r.append(c)
+        return r
+
     def allbases(self, include_self: bool = False) -> Iterator['Class']:
         """
         Iterate on all base objects of this class and it's super classes. Doesn't comply with MRO.
         """
         if include_self:
             yield self
         for b in self.baseobjects:
@@ -691,19 +762,20 @@
     @property
     def constructor_params(self) -> Mapping[str, Optional[ast.expr]]:
         """A mapping of constructor parameter names to their type annotation.
         If a parameter is not annotated, its value is L{None}.
         """
 
         # We assume that the constructor parameters are the same as the
-        # __init__() parameters. This is incorrect if __new__() or the class
-        # call have different parameters.
-        init = self.find('__init__')
-        if isinstance(init, Function):
-            return init.annotations
+        # __new__()/__init__() parameters. This is incorrect if the metaclass
+        # __call__() have different parameters or __init__/__new__ is using
+        # signature changing decorators.
+        constructor = _find_dunder_constructor(self)
+        if constructor is not None:
+            return constructor.annotations
         else:
             return {}
 
 
 class Inheritable(Documentable):
     documentation_location = DocLocation.PARENT_PAGE
 
@@ -722,19 +794,31 @@
 
 class Function(Inheritable):
     kind = DocumentableKind.FUNCTION
     is_async: bool
     annotations: Mapping[str, Optional[ast.expr]]
     decorators: Optional[Sequence[ast.expr]]
     signature: Optional[Signature]
+    overloads: List['FunctionOverload']
 
     def setup(self) -> None:
         super().setup()
         if isinstance(self.parent, Class):
             self.kind = DocumentableKind.METHOD
+        self.signature = None
+        self.overloads = []
+
+@attr.s(auto_attribs=True)
+class FunctionOverload:
+    """
+    @note: This is not an actual documentable type. 
+    """
+    primary: Function
+    signature: Signature
+    decorators: Sequence[ast.expr]
 
 class Attribute(Inheritable):
     kind: Optional[DocumentableKind] = DocumentableKind.ATTRIBUTE
     annotation: Optional[ast.expr]
     decorators: Optional[Sequence[ast.expr]] = None
     value: Optional[ast.expr] = None
     """
@@ -1059,18 +1143,26 @@
     #  http://divmod.org/trac/browser/trunk
     #                          ~/src/Divmod/Nevow/nevow/flat/ten.py
 
     def setSourceHref(self, mod: _ModuleT, source_path: Path) -> None:
         if self.sourcebase is None:
             mod.sourceHref = None
         else:
+            # pydoctor supports generating documentation covering more than one package, 
+            # in which case it is not certain that all of the source is even viewable below a single URL.
+            # We ignore this limitation by not assigning sourceHref for now, but it would be good to add support for it.
             projBaseDir = mod.system.options.projectbasedirectory
             assert projBaseDir is not None
-            relative = source_path.relative_to(projBaseDir).as_posix()
-            mod.sourceHref = f'{self.sourcebase}/{relative}'
+            try:
+                relative = source_path.relative_to(projBaseDir).as_posix()
+            except ValueError:
+                # The links cannot be computed because the source path lies outside base directory.
+                pass
+            else:
+                mod.sourceHref = f'{self.sourcebase}/{relative}'
 
     @overload
     def analyzeModule(self,
             modpath: Path,
             modname: str,
             parentPackage: Optional[_PackageT],
             is_package: Literal[False] = False
@@ -1319,18 +1411,20 @@
         without the risk of drawing incorrect conclusions because modules
         were not fully processed yet.
         """
 
         # default post-processing includes:
         # - Processing of subclasses
         # - MRO computing.
+        # - Lookup of constructors
         # - Checking whether the class is an exception
         for cls in self.objectsOfType(Class):
             
             cls._init_mro()
+            cls._init_constructors()
             
             for b in cls.baseobjects:
                 if b is not None:
                     b.subclasses.append(cls)
             
             if is_exception(cls):
                 cls.kind = DocumentableKind.EXCEPTION
@@ -1342,14 +1436,35 @@
     def fetchIntersphinxInventories(self, cache: CacheT) -> None:
         """
         Download and parse intersphinx inventories based on configuration.
         """
         for url in self.options.intersphinx:
             self.intersphinx.update(cache, url)
 
+def get_docstring(
+        obj: Documentable
+        ) -> Tuple[Optional[str], Optional[Documentable]]:
+    """
+    Fetch the docstring for a documentable.
+    Treat empty docstring as undocumented.
+
+    :returns:
+        - C{(docstring, source)} if the object is documented.
+        - C{(None, None)} if the object has no docstring (even inherited).
+        - C{(None, source)} if the object has an empty docstring.
+    """
+    for source in obj.docsources():
+        doc = source.docstring
+        if doc:
+            return doc, source
+        if doc is not None:
+            # Treat empty docstring as undocumented.
+            return None, source
+    return None, None
+
 class SystemBuildingError(Exception):
     """
     Raised when there is a (handled) fatal error while adding modules to the builder.
     """
 
 class ISystemBuilder(abc.ABC):
     """
@@ -1389,21 +1504,27 @@
         self.system = system
         self._added: Set[Path] = set()
 
     def addModule(self, path: Path, parent_name: Optional[str] = None, ) -> None:
         if path in self._added:
             return
         # Path validity check
-        if self.system.options.projectbasedirectory is not None:
+        projBaseDir = self.system.options.projectbasedirectory
+        if projBaseDir is not None:
             # Note: Path.is_relative_to() was only added in Python 3.9,
             #       so we have to use this workaround for now.
             try:
-                path.relative_to(self.system.options.projectbasedirectory)
-            except ValueError as ex:
-                raise SystemBuildingError(f"Source path lies outside base directory: {ex}")
+                path.relative_to(projBaseDir)
+            except ValueError:
+                if self.system.options.htmlsourcebase:  
+                    # We now support building documentation when the source path is outside of the build directory.
+                    # We simply leave a warning and skip the sourceHref attribute.
+                    # https://github.com/twisted/pydoctor/issues/658
+                    _warn_msg = f"No source links can be generated for module {path}: source path lies outside base directory {projBaseDir}"
+                    self.system.msg('addPackage', _warn_msg, once=True)
         parent: Optional[Package] = None
         if parent_name:
             _p = self.system.allobjects[parent_name]
             assert isinstance(_p, Package)
             parent = _p
         if path.is_dir():
             self.system.msg('addPackage', f"adding directory {path}")
```

### Comparing `pydoctor-22.9.1/pydoctor/mro.py` & `pydoctor-23.4.0/pydoctor/mro.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/napoleon/__init__.py` & `pydoctor-23.4.0/pydoctor/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/napoleon/docstring.py` & `pydoctor-23.4.0/pydoctor/napoleon/docstring.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/napoleon/iterators.py` & `pydoctor-23.4.0/pydoctor/napoleon/iterators.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/node2stan.py` & `pydoctor-23.4.0/pydoctor/node2stan.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,37 @@
     from twisted.web.template import Flattenable
     from pydoctor.epydoc.markup import DocstringLinker
 
 from pydoctor.epydoc.docutils import get_lineno
 from pydoctor.epydoc.doctest import colorize_codeblock, colorize_doctest
 from pydoctor.stanutils import flatten, html2stan
 
-def node2html(node: nodes.Node, docstring_linker: 'DocstringLinker', compact:bool=True) -> List[str]:
+def node2html(node: nodes.Node, docstring_linker: 'DocstringLinker') -> List[str]:
     """
     Convert a L{docutils.nodes.Node} object to HTML strings.
     """
-    visitor = HTMLTranslator(node.document, docstring_linker, compact=compact)
+    visitor = HTMLTranslator(node.document, docstring_linker)
     node.walkabout(visitor)
     return visitor.body
 
-def node2stan(node: Union[nodes.Node, Iterable[nodes.Node]], docstring_linker: 'DocstringLinker', compact:bool=True) -> Tag:
+def node2stan(node: Union[nodes.Node, Iterable[nodes.Node]], docstring_linker: 'DocstringLinker') -> Tag:
     """
     Convert L{docutils.nodes.Node} objects to a Stan tree.
 
     @param node: An docutils document or a fragment of document.
     @return: The element as a stan tree.
     @note:  Any L{nodes.Node} can be passed to that function, the only requirement is 
         that the node's L{nodes.Node.document} attribute is set to a valid L{nodes.document} object.
     """
     html = []
     if isinstance(node, nodes.Node):
-        html += node2html(node, docstring_linker, compact)
+        html += node2html(node, docstring_linker)
     else:
         for child in node:
-            html += node2html(child, docstring_linker, compact)
+            html += node2html(child, docstring_linker)
     return html2stan(''.join(html))
 
 
 def gettext(node: Union[nodes.Node, List[nodes.Node]]) -> List[str]:
     """Return the text inside the node(s)."""
     filtered: List[str] = []
     if isinstance(node, (nodes.Text)):
@@ -66,16 +66,15 @@
     """
     
     settings: ClassVar[Optional[optparse.Values]] = None
     body: List[str]
 
     def __init__(self,
             document: nodes.document,
-            docstring_linker: 'DocstringLinker',
-            compact: bool = False, 
+            docstring_linker: 'DocstringLinker'
             ):
         self._linker = docstring_linker
 
         # Set the document's settings.
         if self.settings is None:
             if docutils_version_info >= (0,19):
                 # Direct access to OptionParser is deprecated from Docutils 0.19
@@ -91,15 +90,14 @@
         document.settings = self.settings
 
         super().__init__(document)
 
         # don't allow <h1> tags, start at <h2>
         # h1 is reserved for the page nodes.title. 
         self.section_level += 1
-        self._compact = compact
 
     # Handle interpreted text (crossreferences)
     def visit_title_reference(self, node: nodes.Node) -> None:
         lineno = get_lineno(node)
         self._handle_reference(node, link_func=lambda target, label: self._linker.link_xref(target, label, lineno))
     
     # Handle internal references
@@ -123,21 +121,15 @@
         if target.endswith('()'):
             target = target[:len(target)-2]
 
         self.body.append(flatten(link_func(target, label)))
         raise nodes.SkipNode()
 
     def should_be_compact_paragraph(self, node: nodes.Node) -> bool:
-
-        # HTMLTranslator.should_be_compact_paragraph() used to always remove the
-        # p tag when there is only one element in the document. This is a good behaviour
-        # for colorizing AST values, etc, but for the docstring, we want to have at least
-        # one paragraph (for a better margin, so we use option compact=False). 
-
-        if self._compact is True and self.document.children == [node]:
+        if self.document.children == [node]:
             return True
         else:
             return super().should_be_compact_paragraph(node)  # type: ignore[no-any-return]
 
     def visit_document(self, node: nodes.Node) -> None:
         pass
```

### Comparing `pydoctor-22.9.1/pydoctor/options.py` & `pydoctor-23.4.0/pydoctor/options.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/qnmatch.py` & `pydoctor-23.4.0/pydoctor/qnmatch.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/sphinx.py` & `pydoctor-23.4.0/pydoctor/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/sphinx_ext/build_apidocs.py` & `pydoctor-23.4.0/pydoctor/sphinx_ext/build_apidocs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/stanutils.py` & `pydoctor-23.4.0/pydoctor/stanutils.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/__init__.py` & `pydoctor-23.4.0/pydoctor/templatewriter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import warnings
 import sys
 from xml.dom import minidom
 
 # Newer APIs from importlib_resources should arrive to stdlib importlib.resources in Python 3.9.
 if TYPE_CHECKING:
     if sys.version_info >= (3, 9):
-        from importlib.abc import Traversable
+        from importlib.resources.abc import Traversable
     else:
         Traversable = Any
 else:
     Traversable = object
 
 from twisted.web.iweb import ITemplateLoader
 from twisted.web.template import TagLoader, XMLString, Element, tags
```

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/pages/__init__.py` & `pydoctor-23.4.0/pydoctor/templatewriter/pages/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,49 +41,83 @@
         if kind == model.DocumentableKind.PACKAGE:
             # packages and modules should be listed together
             return model.DocumentableKind.MODULE
         return kind
 
     return (-o.privacyClass.value, -map_kind(o.kind).value if o.kind else 0, o.fullName().lower())
 
-def format_decorators(obj: Union[model.Function, model.Attribute]) -> Iterator["Flattenable"]:
+def format_decorators(obj: Union[model.Function, model.Attribute, model.FunctionOverload]) -> Iterator["Flattenable"]:
+    # Since we use this function to colorize the FunctionOverload decorators and it's not an actual Documentable subclass, we use the overload's 
+    # primary function for parts that requires an interface to Documentable methods or attributes
+    documentable_obj = obj if not isinstance(obj, model.FunctionOverload) else obj.primary
+
     for dec in obj.decorators or ():
         if isinstance(dec, ast.Call):
-            fn = node2fullname(dec.func, obj)
+            fn = node2fullname(dec.func, documentable_obj)
             # We don't want to show the deprecated decorator;
             # it shows up as an infobox.
             if fn in ("twisted.python.deprecate.deprecated",
                       "twisted.python.deprecate.deprecatedProperty"):
                 break
 
         # Colorize decorators!
         doc = colorize_inline_pyval(dec)
-
-        stan = epydoc2stan.safe_to_stan(doc, obj.docstring_linker, obj, compact=True, 
+        stan = epydoc2stan.safe_to_stan(doc, documentable_obj.docstring_linker, documentable_obj,
             fallback=epydoc2stan.colorized_pyval_fallback, 
             section='rendering of decorators')
         
-        # Report eventual warnings. It warns when a regex failed to parse or the html2stan() function fails.
-        epydoc2stan.reportWarnings(obj, doc.warnings, section='colorize decorator')
+        # Report eventual warnings. It warns when we can't colorize the expression for some reason.
+        epydoc2stan.reportWarnings(documentable_obj, doc.warnings, section='colorize decorator')
         yield '@', stan.children, tags.br()
 
-def format_signature(function: model.Function) -> "Flattenable":
+def format_signature(func: Union[model.Function, model.FunctionOverload]) -> "Flattenable":
     """
     Return a stan representation of a nicely-formatted source-like function signature for the given L{Function}.
     Arguments default values are linked to the appropriate objects when possible.
     """
     broken = "(...)"
     try:
-        return html2stan(str(function.signature)) if function.signature else broken
+        return html2stan(str(func.signature)) if func.signature else broken
     except Exception as e:
         # We can't use safe_to_stan() here because we're using Signature.__str__ to generate the signature HTML.
-        epydoc2stan.reportErrors(function, 
+        epydoc2stan.reportErrors(func.primary if isinstance(func, model.FunctionOverload) else func, 
             [epydoc2stan.get_to_stan_error(e)], section='signature')
         return broken
 
+
+def format_overloads(func: model.Function) -> Iterator["Flattenable"]:
+    """
+    Format a function overloads definitions as nice HTML signatures.
+    """
+    for overload in func.overloads:
+        yield from format_decorators(overload)
+        yield tags.div(format_function_def(func.name, func.is_async, overload))
+
+def format_function_def(func_name: str, is_async: bool, 
+                        func: Union[model.Function, model.FunctionOverload]) -> List["Flattenable"]:
+    """
+    Format a function definition as nice HTML signature. 
+    
+    If the function is overloaded, it will return an empty list. We use L{format_overloads} for these.
+    """
+    r:List["Flattenable"] = []
+    # If this is a function with overloads, we do not render the principal signature because the overloaded signatures will be shown instead.
+    if isinstance(func, model.Function) and func.overloads:
+        return r
+    def_stmt = 'async def' if is_async else 'def'
+    if func_name.endswith('.setter') or func_name.endswith('.deleter'):
+        func_name = func_name[:func_name.rindex('.')]
+    r.extend([
+        tags.span(def_stmt, class_='py-keyword'), ' ',
+        tags.span(func_name, class_='py-defname'), 
+        tags.span(format_signature(func), class_='function-signature'), ':',
+    ])
+    return r
+    
+
 class Nav(TemplateElement):
     """
     Common navigation header.
     """
 
     filename = 'nav.html'
 
@@ -217,15 +251,15 @@
             return ()
         return tag(href=sourceHref)
 
     @renderer
     def inhierarchy(self, request: object, tag: Tag) -> "Flattenable":
         return ()
 
-    def extras(self) -> List[Tag]:
+    def extras(self) -> List["Flattenable"]:
         return self.objectExtras(self.ob)
 
     def docstring(self) -> "Flattenable":
         return self.docgetter.get(self.ob)
 
     def children(self) -> Sequence[model.Documentable]:
         return sorted(
@@ -266,22 +300,23 @@
                 r.append(FunctionChild(self.docgetter, c, self.objectExtras(c), func_loader))
             elif isinstance(c, model.Attribute):
                 r.append(AttributeChild(self.docgetter, c, self.objectExtras(c), attr_loader))
             else:
                 assert False, type(c)
         return r
 
-    def objectExtras(self, ob: model.Documentable) -> List[Tag]:
+    def objectExtras(self, ob: model.Documentable) -> List["Flattenable"]:
         """
         Flatten each L{model.Documentable.extra_info} list item.
         """
-        r: List[Tag] = []
+        r: List["Flattenable"] = []
         for extra in ob.extra_info:
-            r.append(epydoc2stan.safe_to_stan(extra, ob.docstring_linker, ob, compact=False, 
-                fallback = lambda _,__,___:epydoc2stan.BROKEN, section='extra'))
+            r.append(epydoc2stan.unwrap_docstring_stan(
+                epydoc2stan.safe_to_stan(extra, ob.docstring_linker, ob,
+                fallback = lambda _,__,___:epydoc2stan.BROKEN, section='extra')))
         return r
 
 
     def functionBody(self, ob: model.Documentable) -> "Flattenable":
         return self.docgetter.get(ob)
 
     @renderer
@@ -309,16 +344,16 @@
         )
         return slot_map
 
 
 class ModulePage(CommonPage):
     ob: model.Module
 
-    def extras(self) -> List[Tag]:
-        r: List[Tag] = []
+    def extras(self) -> List["Flattenable"]:
+        r: List["Flattenable"] = []
 
         sourceHref = util.srclink(self.ob)
         if sourceHref:
             r.append(tags.a("(source)", href=sourceHref, class_="sourceLink"))
 
         r.extend(super().extras())
         return r
@@ -389,28 +424,28 @@
             ob: model.Documentable,
             template_lookup: TemplateLookup,
             docgetter: Optional[util.DocGetter] = None
             ):
         super().__init__(ob, template_lookup, docgetter)
         self.baselists = util.class_members(self.ob)
 
-    def extras(self) -> List[Tag]:
-        r: List[Tag] = []
+    def extras(self) -> List["Flattenable"]:
+        r: List["Flattenable"] = []
 
         sourceHref = util.srclink(self.ob)
         source: "Flattenable"
         if sourceHref:
             source = (" ", tags.a("(source)", href=sourceHref, class_="sourceLink"))
         else:
             source = tags.transparent
         r.append(tags.p(tags.code(
             tags.span("class", class_='py-keyword'), " ",
             tags.span(self.ob.name, class_='py-defname'),
             self.classSignature(), ":", source
-            )))
+            ), class_='class-signature'))
 
         subclasses = sorted(self.ob.subclasses, key=util.objects_order)
         if subclasses:
             p = assembleList(self.ob.system, "Known subclasses: ",
                             [o.fullName() for o in subclasses], self.page_url)
             if p is not None:
                 r.append(tags.p(p))
@@ -422,24 +457,23 @@
 
         r: List["Flattenable"] = []
         # Here, we should use the parent's linker because a base name
         # can't be define in the class itself.
         _linker = self.ob.parent.docstring_linker
         if self.ob.rawbases:
             r.append('(')
-            with _linker.disable_same_page_optimazation():
+            with _linker.switch_context(None):
             
                 for idx, (_, base_node) in enumerate(self.ob.rawbases):
                     if idx != 0:
                         r.append(', ')
 
                     # link to external class or internal class, using the colorizer here
                     # to link to classes with generics (subscripts and other AST expr).
                     stan = epydoc2stan.safe_to_stan(colorize_inline_pyval(base_node), _linker, self.ob, 
-                        compact=True, 
                         fallback=epydoc2stan.colorized_pyval_fallback, 
                         section='rendering of class signature')
                     r.extend(stan.children)
                     
             r.append(')')
         return r
 
@@ -473,20 +507,20 @@
             for b in reversed(bases_to_mention):
                 tail.append(tags.code(epydoc2stan.taglink(b, page_url, b.name)))
                 tail.append(', ')
             del tail[-1]
             r.extend([' (via ', tail, ')'])
         return r
 
-    def objectExtras(self, ob: model.Documentable) -> List[Tag]:
-        r = list(get_override_info(self.ob, ob.name, self.page_url))
+    def objectExtras(self, ob: model.Documentable) -> List["Flattenable"]:
+        r: List["Flattenable"] = list(get_override_info(self.ob, ob.name, self.page_url))
         r.extend(super().objectExtras(ob))
         return r
 
-def get_override_info(cls:model.Class, member_name:str, page_url:Optional[str]=None) -> Iterator[Tag]:
+def get_override_info(cls:model.Class, member_name:str, page_url:Optional[str]=None) -> Iterator["Flattenable"]:
     page_url = page_url or cls.page_object.url
     for b in cls.mro(include_self=False):
         if member_name not in b.contents:
             continue
         overridden = b.contents[member_name]
         yield tags.div(class_="interfaceinfo")(
             'overrides ', tags.code(epydoc2stan.taglink(overridden, page_url)))
@@ -499,15 +533,15 @@
         if l is not None:
             yield tags.div(class_="interfaceinfo")(l)
     
 
 class ZopeInterfaceClassPage(ClassPage):
     ob: zopeinterface.ZopeInterfaceClass
 
-    def extras(self) -> List[Tag]:
+    def extras(self) -> List["Flattenable"]:
         r = super().extras()
         if self.ob.isinterface:
             namelist = [o.fullName() for o in 
                         sorted(self.ob.implementedby_directly, key=util.objects_order)]
             label = 'Known implementations: '
         else:
             namelist = sorted(self.ob.implements_directly, key=lambda x:x.lower())
@@ -526,17 +560,17 @@
                 assert isinstance(io, zopeinterface.ZopeInterfaceClass)
                 for io2 in io.mro():
                     method: Optional[model.Documentable] = io2.contents.get(methname)
                     if method is not None:
                         return method
         return None
 
-    def objectExtras(self, ob: model.Documentable) -> List[Tag]:
+    def objectExtras(self, ob: model.Documentable) -> List["Flattenable"]:
         imeth = self.interfaceMeth(ob.name)
-        r: List[Tag] = []
+        r: List["Flattenable"] = []
         if imeth:
             iface = imeth.parent
             assert iface is not None
             r.append(tags.div(class_="interfaceinfo")('from ', tags.code(
                 epydoc2stan.taglink(imeth, self.page_url, iface.fullName())
                 )))
         r.extend(super().objectExtras(ob))
```

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/pages/attributechild.py` & `pydoctor-23.4.0/pydoctor/templatewriter/pages/attributechild.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class AttributeChild(TemplateElement):
 
     filename = 'attribute-child.html'
 
     def __init__(self,
             docgetter: util.DocGetter,
             ob: Attribute,
-            extras: List[Tag],
+            extras: List["Flattenable"],
             loader: ITemplateLoader
             ):
         super().__init__(loader)
         self.docgetter = docgetter
         self.ob = ob
         self._functionExtras = extras
 
@@ -63,15 +63,15 @@
     def sourceLink(self, request: object, tag: Tag) -> "Flattenable":
         if self.ob.sourceHref:
             return tag.fillSlots(sourceHref=self.ob.sourceHref)
         else:
             return ()
 
     @renderer
-    def objectExtras(self, request: object, tag: Tag) -> List[Tag]:
+    def objectExtras(self, request: object, tag: Tag) -> List["Flattenable"]:
         return self._functionExtras
 
     @renderer
     def functionBody(self, request: object, tag: Tag) -> "Flattenable":
         return self.docgetter.get(self.ob)
 
     @renderer
```

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/pages/functionchild.py` & `pydoctor-23.4.0/pydoctor/templatewriter/pages/table.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,91 @@
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, Collection
 
 from twisted.web.iweb import ITemplateLoader
-from twisted.web.template import Tag, renderer, tags
+from twisted.web.template import Element, Tag, TagLoader, renderer, tags
 
-from pydoctor.model import Function
+from pydoctor import epydoc2stan
+from pydoctor.model import Documentable, Function
 from pydoctor.templatewriter import TemplateElement, util
-from pydoctor.templatewriter.pages import format_decorators, format_signature
 
 if TYPE_CHECKING:
     from twisted.web.template import Flattenable
 
 
-class FunctionChild(TemplateElement):
-
-    filename = 'function-child.html'
+class TableRow(Element):
 
     def __init__(self,
+            loader: ITemplateLoader,
             docgetter: util.DocGetter,
-            ob: Function,
-            extras: List[Tag],
-            loader: ITemplateLoader
+            ob: Documentable,
+            child: Documentable,
             ):
         super().__init__(loader)
         self.docgetter = docgetter
         self.ob = ob
-        self._functionExtras = extras
+        self.child = child
 
     @renderer
     def class_(self, request: object, tag: Tag) -> "Flattenable":
-        class_ = util.css_class(self.ob)
-        if self.ob.parent is not self.ob:
+        class_ = util.css_class(self.child)
+        if self.child.parent is not self.ob:
             class_ = 'base' + class_
         return class_
 
     @renderer
-    def functionAnchor(self, request: object, tag: Tag) -> "Flattenable":
-        return self.ob.fullName()
+    def kind(self, request: object, tag: Tag) -> Tag:
+        child = self.child
+        kind = child.kind
+        assert kind is not None  # 'kind is None' makes the object invisible
+        kind_name = epydoc2stan.format_kind(kind)
+        if isinstance(child, Function) and child.is_async:
+            # The official name is "coroutine function", but that is both
+            # a bit long and not as widely recognized.
+            kind_name = f'Async {kind_name}'
 
-    @renderer
-    def shortFunctionAnchor(self, request: object, tag: Tag) -> str:
-        return self.ob.name
-    
-    @renderer
-    def anchorHref(self, request: object, tag: Tag) -> str:
-        name = self.shortFunctionAnchor(request, tag)
-        return f'#{name}'
+        return tag.clear()(kind_name)
 
     @renderer
-    def decorator(self, request: object, tag: Tag) -> "Flattenable":
-        return list(format_decorators(self.ob))
+    def name(self, request: object, tag: Tag) -> Tag:
+        return tag.clear()(tags.code(
+            epydoc2stan.taglink(self.child, self.ob.url, epydoc2stan.insert_break_points(self.child.name))
+            ))
 
     @renderer
-    def functionDef(self, request: object, tag: Tag) -> "Flattenable":
-        def_stmt = 'async def' if self.ob.is_async else 'def'
-        name = self.ob.name
-        if name.endswith('.setter') or name.endswith('.deleter'):
-            name = name[:name.rindex('.')]
-        return [
-            tags.span(def_stmt, class_='py-keyword'), ' ',
-            tags.span(name, class_='py-defname'), 
-            format_signature(self.ob), ':'
-            ]
+    def summaryDoc(self, request: object, tag: Tag) -> Tag:
+        return tag.clear()(self.docgetter.get(self.child, summary=True))
 
-    @renderer
-    def sourceLink(self, request: object, tag: Tag) -> "Flattenable":
-        if self.ob.sourceHref:
-            return tag.fillSlots(sourceHref=self.ob.sourceHref)
-        else:
-            return ()
 
-    @renderer
-    def objectExtras(self, request: object, tag: Tag) -> List[Tag]:
-        return self._functionExtras
+class ChildTable(TemplateElement):
+
+    last_id = 0
+
+    filename = 'table.html'
+
+    def __init__(self,
+            docgetter: util.DocGetter,
+            ob: Documentable,
+            children: Collection[Documentable],
+            loader: ITemplateLoader,
+            ):
+        super().__init__(loader)
+        self.children = children
+        ChildTable.last_id += 1
+        self._id = ChildTable.last_id
+        self.ob = ob
+        self.docgetter = docgetter
 
     @renderer
-    def functionBody(self, request: object, tag: Tag) -> "Flattenable":
-        return self.docgetter.get(self.ob)
+    def id(self, request: object, tag: Tag) -> str:
+        return f'id{self._id}'
 
+    @renderer
+    def rows(self, request: object, tag: Tag) -> "Flattenable":
+        return [
+            TableRow(
+                TagLoader(tag),
+                self.docgetter,
+                self.ob,
+                child)
+            for child in self.children
+            if child.isVisible
+            ]
```

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/pages/sidebar.py` & `pydoctor-23.4.0/pydoctor/templatewriter/pages/sidebar.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/search.py` & `pydoctor-23.4.0/pydoctor/templatewriter/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import attr
 
 from pydoctor.templatewriter.pages import Page
 from pydoctor import model, epydoc2stan, node2stan
 
 from twisted.web.template import Tag, renderer
-from lunr import lunr, get_default_builder, stop_word_filter, stemmer
+from lunr import lunr, get_default_builder
 
 if TYPE_CHECKING:
     from twisted.web.template import Flattenable
 
 def get_all_documents_flattenable(system: model.System) -> List[Dict[str, "Flattenable"]]:
     """
     Get the all data to be writen into ``all-documents.html`` file.
@@ -53,21 +53,26 @@
     """
     
     output_file: Path
     system: model.System
     fields: List[str]
 
     _BOOSTS = {
-                'name':4,
-                'names': 2,
-                'qname':1,
+                'name':6,
+                'names': 1,
+                'qname':2,
                 'docstring':1,
                 'kind':-1
               }
-
+    
+    # For all pipeline functions, stop_word_filter, stemmer and trimmer, skip their action expect for the
+    # docstring field.
+    _SKIP_PIPELINES = list(_BOOSTS)
+    _SKIP_PIPELINES.remove('docstring')
+    
     @staticmethod
     def get_ob_boost(ob: model.Documentable) -> int:
         # Advantage container types because they hold more informations.
         if isinstance(ob, (model.Class, model.Module)):
             return 2
         else:
             return 1
@@ -127,22 +132,21 @@
 
         builder = get_default_builder()
 
         # Skip some pipelines for better UX
         # https://lunr.readthedocs.io/en/latest/customisation.html#skip-a-pipeline-function-for-specific-field-names
         
         # We want classes named like "For" to be indexed with their name, even if it's matching stop words.
-        builder.pipeline.skip(stop_word_filter.stop_word_filter, ["qname", "name", "kind", "names"])  
-
-        # We don't want "name" and related fields to be stemmed since the field "names"
-        # contains all cased breaked combinaisons and will be stemmed.
-        builder.pipeline.skip(stemmer.stemmer, ["name", "kind", "qname"])
+        # We don't want "name" and related fields to be stemmed since we're stemming ourselves the name.
+        # see https://github.com/twisted/pydoctor/issues/648 for why.
+        for pipeline_function in builder.pipeline.registered_functions.values():
+            builder.pipeline.skip(pipeline_function, self._SKIP_PIPELINES)  
 
         # Removing the stemmer from the search pipeline, see https://github.com/yeraydiazdiaz/lunr.py/issues/112
-        builder.search_pipeline.remove(stemmer.stemmer)
+        builder.search_pipeline.reset()
 
         index = lunr(
             ref='qname',
             fields=[{'field_name':name, 'boost':self._BOOSTS[name]} for name in self.fields],
             documents=self.get_corpus(), 
             builder=builder)   
         
@@ -165,15 +169,22 @@
         ).write()
 
     LunrIndexWriter(output_dir / "fullsearchindex.json", 
         system=system, 
         fields=["name", "names", "qname", "docstring", "kind"]
         ).write()
 
+
 def stem_identifier(identifier: str) -> Iterator[str]:
+    # we are stemming the identifier ourselves because
+    # lunr is removing too much of important data. 
+    # See issue https://github.com/twisted/pydoctor/issues/648
+    yielded = set()
     parts = epydoc2stan._split_indentifier_parts_on_case(identifier)
     for p in parts:
         p = p.strip('_')
-        if p and p.lower() not in stop_word_filter.WORDS: 
-            yield p
+        if p:
+            if p not in yielded:
+                yielded.add(p)
+                yield p
 
 searchpages: List[Type[Page]] = [AllDocuments]
```

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/summary.py` & `pydoctor-23.4.0/pydoctor/templatewriter/summary.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/util.py` & `pydoctor-23.4.0/pydoctor/templatewriter/util.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/templatewriter/writer.py` & `pydoctor-23.4.0/pydoctor/templatewriter/writer.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/__init__.py` & `pydoctor-23.4.0/pydoctor/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/__init__.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,13 +3,21 @@
 # Copyright (C) 2005 Edward Loper
 # Author: Edward Loper <edloper@loper.org>
 # URL: <http://epydoc.sf.net>
 #
 
 from typing import List
 from pydoctor.epydoc.markup import ParseError, ParsedDocstring, get_parser_by_name
+import pydoctor.epydoc.markup
 
 def parse_docstring(doc: str, markup: str, processtypes: bool = False) -> ParsedDocstring:
+    
+    parse = get_parser_by_name(markup)
+    if processtypes:
+        if markup in ('google','numpy'):
+            raise AssertionError("don't process types twice.")
+        parse = pydoctor.epydoc.markup.processtypes(parse)
+    
     errors: List[ParseError] = []
-    parsed = get_parser_by_name(markup)(doc, errors, processtypes)
+    parsed = parse(doc, errors)
     assert not errors, [f"{e.linenum()}:{e.descr()}" for e in errors]
     return parsed
```

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/epytext.doctest` & `pydoctor-23.4.0/pydoctor/test/epydoc/epytext.doctest`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     <para>field</para></field></fieldlist>
 
     >>> print(testparse("""\nParagraph\n@foo: field"""))
     <para>Paragraph</para>
     <fieldlist><field lineno='2'><tag>foo</tag>
     <para>field</para></field></fieldlist>
 
-Make sure thta unindented lists are not allowed:
+Make sure that unindented lists are not allowed:
 
     >>> print(testparse("""
     ...     This is a paragraph.
     ...
     ...     - This is a list item."""))
     Traceback (most recent call last):
     StructuringError: Line 4: Lists must be indented.
```

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/restructuredtext.doctest` & `pydoctor-23.4.0/pydoctor/test/epydoc/restructuredtext.doctest`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/test_epytext.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/test_epytext.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,21 @@
     v = flatten(epytext.parse_docstring(s, errs).to_stan(linker))
     if errs:
         raise errs[0]
     return (v or '').rstrip()
 
 
 def parse(s: str) -> str:
-    # this strips off the <epytext>...</epytext>
-    return ''.join(str(n) for n in epytext.parse(s).children)
+    errors: List[ParseError] = []
+    element = epytext.parse(s, errors)
+    if element is None:
+        raise errors[0]
+    else:
+        # this strips off the <epytext>...</epytext>
+        return ''.join(str(n) for n in element.children)
 
 
 def test_basic_list() -> None:
     P1 = "This is a paragraph."
     P2 = "This is a \nparagraph."
     LI1 = "  - This is a list item."
     LI2 = "\n  - This is a list item."
```

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/test_epytext2html.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/test_epytext2html.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/test_epytext2node.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/test_epytext2node.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/test_google_numpy.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/test_google_numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         parse_docstring = get_google_parser(obj)
 
         docstring = """\
 numpy.ndarray: super-dooper attribute"""
 
         errors: List[ParseError] = []
 
-        actual = flatten(parse_docstring(docstring, errors, False).fields[-1].body().to_stan(NotFoundLinker()))
+        parsed_doc = parse_docstring(docstring, errors)
+
+        actual = flatten(parsed_doc.fields[-1].body().to_stan(NotFoundLinker()))
         
         expected = """<code>numpy.ndarray</code>"""
 
         self.assertEqual(expected, actual)
         self.assertEqual(errors, [])
 
     def test_get_google_parser_not_attribute(self) -> None:
@@ -35,31 +37,33 @@
         parse_docstring = get_google_parser(obj)
 
         docstring = """\
 numpy.ndarray: super-dooper attribute"""
 
         errors: List[ParseError] = []
 
-        assert not parse_docstring(docstring, errors, False).fields
+        assert not parse_docstring(docstring, errors).fields
 
     # the numpy inline attribute parsing is the same as google-style
     # as shown in the example_numpy.py from Sphinx docs
     def test_get_numpy_parser_attribute(self) -> None:
 
         obj = Attribute(system = System(), name='attr1')
 
         parse_docstring = get_numpy_parser(obj)
 
         docstring = """\
 numpy.ndarray: super-dooper attribute"""
 
         errors: List[ParseError] = []
-
-        actual = flatten(parse_docstring(docstring, errors, False).fields[-1].body().to_stan(NotFoundLinker()))
         
+        parsed_doc = parse_docstring(docstring, errors)
+
+        actual = flatten(parsed_doc.fields[-1].body().to_stan(NotFoundLinker()))
+
         expected = """<code>numpy.ndarray</code>"""
 
         self.assertEqual(expected, actual)
         self.assertEqual(errors, [])
 
     def test_get_numpy_parser_not_attribute(self) -> None:
 
@@ -68,15 +72,15 @@
         parse_docstring = get_numpy_parser(obj)
 
         docstring = """\
 numpy.ndarray: super-dooper attribute"""
 
         errors: List[ParseError] = []
 
-        assert not parse_docstring(docstring, errors, False).fields
+        assert not parse_docstring(docstring, errors).fields
 
 
 class TestWarnings(TestCase):
 
     def test_warnings(self) -> None:
         
         obj = Function(system = System(), name='func')
@@ -111,15 +115,15 @@
 Note
 ----
 Some more text.
 """
 
         errors: List[ParseError] = []
 
-        parse_docstring(docstring, errors, False)
+        parse_docstring(docstring, errors)
         
         self.assertEqual(len(errors), 3)
         
         self.assertIn("malformed string literal (missing closing quote)", errors[2].descr())
         self.assertIn("invalid value set (missing closing brace)", errors[1].descr())
         self.assertIn("malformed string literal (missing opening quote)", errors[0].descr())
```

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/test_parsed_docstrings.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/test_parsed_docstrings.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/test_pyval_repr.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/test_pyval_repr.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     colorizer = PyvalColorizer(linelen=linelen, linebreakok=linebreakok, maxlines=maxlines)
     parsed_doc = colorizer.colorize(v)
     return parsed_doc.to_node().pformat() #type: ignore
 
 def colorhtml(v: Any, linebreakok:bool=True, maxlines:int=5, linelen:int=40) -> str:
     colorizer = PyvalColorizer(linelen=linelen, linebreakok=linebreakok, maxlines=maxlines)
     parsed_doc = colorizer.colorize(v)
-    return flatten(parsed_doc.to_stan(NotFoundLinker(), compact=True))
+    return flatten(parsed_doc.to_stan(NotFoundLinker()))
 
 def test_simple_types() -> None:
     """
     Integers, floats, None, and complex numbers get printed using str,
     with no syntax highlighting.
     """
     assert color(1) == """<document source="pyval_repr">
@@ -1219,25 +1219,40 @@
 def color_re(s: Union[bytes, str], 
              check_roundtrip:bool=True) -> str:
 
     colorizer = PyvalColorizer(linelen=55, maxlines=5)
     val = colorizer.colorize(extract_expr(ast.parse(f"re.compile({repr(s)})")))
 
     if check_roundtrip:
-
+        raw_text = ''.join(gettext(val.to_node()))
         re_begin = 13
+        raw_string = True
+
+        if raw_text[11] != 'r':
+            # the regex has failed to be colorized since we can't find the r prefix
+            # meaning the string has been rendered as plaintext instead.
+            raw_string = False
+            re_begin -= 1
+        
         if isinstance(s, bytes):
             re_begin += 1
         re_end = -2
 
-        round_trip: Union[bytes, str] = ''.join(gettext(val.to_node()))[re_begin:re_end]
+        round_trip: Union[bytes, str] = raw_text[re_begin:re_end]
         if isinstance(s, bytes):
             assert isinstance(round_trip, str)
             round_trip = bytes(round_trip, encoding='utf-8')
-        assert round_trip == s, "%s != %s" % (repr(round_trip), repr(s))
+        
+        expected = s
+        if not raw_string:
+            assert isinstance(expected, str) 
+            # we only test invalid regexes with strings currently
+            expected = expected.replace('\\', '\\\\')
+        
+        assert round_trip == expected, "%s != %s" % (repr(round_trip), repr(s))
     
     return flatten(val.to_stan(NotFoundLinker()))[17:-8]
 
 
 def test_re_literals() -> None:
     # Literal characters
     assert color_re(r'abc \t\r\n\f\v \xff \uffff', False) == r"""r<span class="rst-variable-quote">'</span>abc \t\r\n\f\v \xff \uffff<span class="rst-variable-quote">'</span>"""
@@ -1340,14 +1355,35 @@
 
     assert color_re(b"(?Limstx)^Food") == """rb<span class="rst-variable-quote">'</span><span class="rst-re-flags">(?Limstx)</span>^Food<span class="rst-variable-quote">'</span>"""
     
     assert color_re(r"(?imstux)^Food") == """r<span class="rst-variable-quote">'</span><span class="rst-re-flags">(?imstux)</span>^Food<span class="rst-variable-quote">'</span>"""
      
     assert color_re(r"(?x)This   is   verbose", False) == """r<span class="rst-variable-quote">'</span><span class="rst-re-flags">(?ux)</span>Thisisverbose<span class="rst-variable-quote">'</span>"""
 
+def test_unsupported_regex_features() -> None:
+    """
+    Because pydoctor uses the regex engine of python 3.6, it does not support the 
+    latest features introduced in python3.11 like atomic groupping and possesive qualifiers.
+
+    But still, we should not crash.
+    """
+    regexes = ['e*+e',
+        '(e?){2,4}+a',
+        r"^(\w){1,2}+$",
+        # "^x{}+$", this one fails to round-trip :/
+        r'a++',
+        r'(?:ab)++',
+        r'(?:ab){1,3}+',
+        r'(?>x++)x',
+        r'(?>a{1,3})',
+        r'(?>(?:ab){1,3})',
+        ]
+    for r in regexes:
+        color_re(r)
+
 def test_re_not_literal() -> None:
 
     assert color_re(r"[^0-9]") == """r<span class="rst-variable-quote">'</span><span class="rst-re-group">[</span><span class="rst-re-op">^</span>0<span class="rst-re-op">-</span>9<span class="rst-re-group">]</span><span class="rst-variable-quote">'</span>"""
 
 def test_re_named_groups() -> None:
     # This regex triggers some weird behaviour: it adds the &crarr; element at the end where it should not be...
     # The regex is 42 caracters long, so more than 40, maybe that's why?
```

### Comparing `pydoctor-22.9.1/pydoctor/test/epydoc/test_restructuredtext.py` & `pydoctor-23.4.0/pydoctor/test/epydoc/test_restructuredtext.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         Return a fully qualified name for the possibly-dotted name.
 
         To explain what this means, consider the following modules... blabla""",
         "Return a fully qualified name for the possibly-dotted name.")
     ]
     for src, summary_text in cases:
         errors: List[ParseError] = []
-        pdoc = get_parser_by_name(markup)(dedent(src), errors, False)
+        pdoc = get_parser_by_name(markup)(dedent(src), errors)
         assert not errors
         assert pdoc.get_summary() == pdoc.get_summary() # summary is cached inside ParsedDocstring as well.
         assert flatten_text(pdoc.get_summary().to_stan(NotFoundLinker())) == summary_text
 
 
 # From docutils 0.18 the toc entries uses different ids.
 @pytest.mark.skipif(docutils_version_info < (0,18), reason="HTML ids in toc tree changed in docutils 0.18.0.")
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_astbuilder.py` & `pydoctor-23.4.0/pydoctor/test/test_astbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Tuple, Type, List, overload, cast
 import ast
 
 import astor
 
 
 from pydoctor import astbuilder, astutils, model
+from pydoctor import epydoc2stan
 from pydoctor.epydoc.markup import DocstringLinker, ParsedDocstring
 from pydoctor.options import Options
 from pydoctor.stanutils import flatten, html2stan, flatten_text
 from pydoctor.epydoc.markup.epytext import Element, ParsedEpytextDocstring
 from pydoctor.epydoc2stan import format_summary, get_parsed_type
 from pydoctor.test.test_packages import processPackage
 from pydoctor.utils import partialclass
@@ -1614,14 +1615,51 @@
         var = 1
         """Local variable."""
     ''', systemcls=systemcls)
     outer = mod.contents['outer']
     assert not outer.contents
 
 @systemcls_param
+def test_overload(systemcls: Type[model.System], capsys: CapSys) -> None:
+    # Confirm decorators retained on overloads, docstring ignored for overloads,
+    # and that overloads after the primary function are skipped
+    mod = fromText("""
+        from typing import overload, Union
+        def dec(fn):
+            pass
+        @dec
+        @overload
+        def parse(s:str)->str:
+            ...
+        @overload
+        def parse(s:bytes)->bytes:
+            '''Ignored docstring'''
+            ...
+        def parse(s:Union[str, bytes])->Union[str, bytes]:
+            pass
+        @overload
+        def parse(s:str)->bytes:
+            ...
+        """, systemcls=systemcls)
+    func = mod.contents['parse']
+    assert isinstance(func, model.Function)
+    # Work around different space arrangements in Signature.__str__ between python versions
+    assert flatten_text(html2stan(str(func.signature).replace(' ', ''))) == '(s:Union[str,bytes])->Union[str,bytes]'
+    assert [astbuilder.node2dottedname(d) for d in (func.decorators or ())] == []
+    assert len(func.overloads) == 2
+    assert [astbuilder.node2dottedname(d) for d in func.overloads[0].decorators] == [['dec'], ['overload']]
+    assert [astbuilder.node2dottedname(d) for d in func.overloads[1].decorators] == [['overload']]
+    assert flatten_text(html2stan(str(func.overloads[0].signature).replace(' ', ''))) == '(s:str)->str'
+    assert flatten_text(html2stan(str(func.overloads[1].signature).replace(' ', ''))) == '(s:bytes)->bytes'
+    assert capsys.readouterr().out.splitlines() == [
+        '<test>:11: <test>.parse overload has docstring, unsupported',
+        '<test>:15: <test>.parse overload appeared after primary function',
+    ]
+
+@systemcls_param
 def test_constant_module(systemcls: Type[model.System]) -> None:
     """
     Module variables with all-uppercase names are recognized as constants.
     """
     mod = fromText('''
     LANG = 'FR'
     ''', systemcls=systemcls)
@@ -2111,7 +2149,234 @@
         assert isinstance(system.allobjects['lib.pack'], model.Package)
         assert isinstance(system.allobjects['lib.pack.basic.mod.C'], model.Class)
         assert 'basic' not in system.allobjects
     
     finally:
         systemcls.systemBuilder = _builderT_init
 
+def getConstructorsText(cls: model.Documentable) -> str:
+    assert isinstance(cls, model.Class)
+    return '\n'.join(
+        epydoc2stan.format_constructor_short_text(c, cls) for c in cls.public_constructors)
+
+@systemcls_param
+def test_crash_type_inference_unhashable_type(systemcls: Type[model.System], capsys:CapSys) -> None:
+    """
+    This test is about not crashing.
+
+    A TypeError is raised by ast.literal_eval() in some cases, when we're trying to do a set of lists or a dict with list keys.
+    We do not bother reporting it because pydoctor is not a checker.
+    """
+
+    src = '''
+    # Unhashable type, will raise an error in ast.literal_eval()
+    x = {[1, 2]}
+    class C:
+        v = {[1,2]:1}
+        def __init__(self):
+            self.y = [{'str':2}, {[1,2]:1}]
+    Y = [{'str':2}, {{[1, 2]}:1}]
+    '''
+
+    mod = fromText(src, systemcls=systemcls, modname='m')
+    for obj in ['m.x', 'm.C.v', 'm.C.y', 'm.Y']:
+        o = mod.system.allobjects[obj]
+        assert isinstance(o, model.Attribute)
+        assert o.annotation is None
+    assert not capsys.readouterr().out
+
+
+@systemcls_param
+def test_constructor_signature_init(systemcls: Type[model.System]) -> None:
+    
+    src = '''\
+    class Person(object):
+        # pydoctor can infer the constructor to be: "Person(name, age)"
+        def __init__(self, name, age):
+            self.name = name
+            self.age = age
+
+    class Citizen(Person):
+        # pydoctor can infer the constructor to be: "Citizen(nationality, *args, **kwargs)"
+        def __init__(self, nationality, *args, **kwargs):
+            self.nationality = nationality
+            super(Citizen, self).__init__(*args, **kwargs)
+        '''
+    mod = fromText(src, systemcls=systemcls)
+
+    # Like "Available constructor: ``Person(name, age)``" that links to Person.__init__ documentation.
+    assert getConstructorsText(mod.contents['Person']) == "Person(name, age)"
+    
+    # Like "Available constructor: ``Citizen(nationality, *args, **kwargs)``" that links to Citizen.__init__ documentation.
+    assert getConstructorsText(mod.contents['Citizen']) == "Citizen(nationality, *args, **kwargs)"
+
+@systemcls_param
+def test_constructor_signature_new(systemcls: Type[model.System]) -> None:
+    src = '''\
+    class Animal(object):
+        # pydoctor can infer the constructor to be: "Animal(name)"
+        def __new__(cls, name):
+            obj = super().__new__(cls)
+            # assignation not recognized by pydoctor, attribute 'name' will not be documented
+            obj.name = name 
+            return obj
+    '''
+
+    mod = fromText(src, systemcls=systemcls)
+
+    assert getConstructorsText(mod.contents['Animal']) == "Animal(name)"
+
+@systemcls_param
+def test_constructor_signature_init_and_new(systemcls: Type[model.System]) -> None:
+    """
+    Pydoctor can't infer the constructor signature when both __new__ and __init__ are defined. 
+    __new__ takes the precedence over __init__ because it's called first. Trying to infer what are the complete 
+    constructor signature when __new__ is defined might be very hard because the method can return an instance of 
+    another class, calling another __init__ method. We're not there yet in term of static analysis.
+    """
+
+    src = '''\
+    class Animal(object):
+        # both __init__ and __new__ are defined, pydoctor only looks at the __new__ method
+        # pydoctor infers the constructor to be: "Animal(*args, **kw)"
+        def __new__(cls, *args, **kw):
+            print('__new__() called.')
+            print('args: ', args, ', kw: ', kw)
+            return super().__new__(cls)
+
+        def __init__(self, name):
+            print('__init__() called.')
+            self.name = name
+            
+    class Cat(Animal):
+        # Idem, but __new__ is inherited.
+        # pydoctor infers the constructor to be: "Cat(*args, **kw)"
+        # This is why it's important to still document __init__ as a regular method.
+        def __init__(self, name, owner):
+            super().__init__(name)
+            self.owner = owner
+    '''
+
+    mod = fromText(src, systemcls=systemcls)
+
+    assert getConstructorsText(mod.contents['Animal']) == "Animal(*args, **kw)"
+    assert getConstructorsText(mod.contents['Cat']) == "Cat(*args, **kw)"
+
+@systemcls_param
+def test_constructor_signature_classmethod(systemcls: Type[model.System]) -> None:
+
+    src = '''\
+    
+    def get_default_options() -> 'Options':
+        """
+        This is another constructor for class 'Options'. 
+        But it's not recognized by pydoctor because it's not defined in the locals of Options.
+        """
+        return Options()
+
+    class Options:
+        a,b,c = None, None, None
+
+        @classmethod
+        def create_no_hints(cls):
+            """
+            Pydoctor can't deduce that this method is a constructor as well,
+            because there is no type annotation.
+            """
+            return cls()
+        
+        # thanks to type hints, 
+        # pydoctor can infer the constructor to be: "Options.create()"
+        @staticmethod
+        def create(important_arg) -> 'Options':
+            # the fictional constructor is not detected by pydoctor, because it doesn't exists actually.
+            return Options(1,2,3)
+        
+        # thanks to type hints, 
+        # pydoctor can infer the constructor to be: "Options.create_from_num(num)"
+        @classmethod
+        def create_from_num(cls, num) -> 'Options':
+            c = cls.create()
+            c.a = num
+            return c
+        '''
+
+    mod = fromText(src, systemcls=systemcls)
+
+    assert getConstructorsText(mod.contents['Options']) == "Options.create(important_arg)\nOptions.create_from_num(num)"
+
+@systemcls_param
+def test_constructor_inner_class(systemcls: Type[model.System]) -> None:
+    src = '''\
+    from typing import Self
+    class Animal(object):
+        class Bar(object):
+            # pydoctor can infer the constructor to be: "Animal.Bar(name)"
+            def __new__(cls, name):
+                ...
+            class Foo(object):
+                # pydoctor can infer the constructor to be: "Animal.Bar.Foo.create(name)"
+                @classmethod
+                def create(cls, name) -> 'Self':
+                    c = cls.create()
+                    c.a = num
+                    return c
+    '''
+    mod = fromText(src, systemcls=systemcls)
+    assert getConstructorsText(mod.contents['Animal'].contents['Bar']) == "Animal.Bar(name)"
+    assert getConstructorsText(mod.contents['Animal'].contents['Bar'].contents['Foo']) == "Animal.Bar.Foo.create(name)"
+
+@systemcls_param
+def test_constructor_many_parameters(systemcls: Type[model.System]) -> None:
+    src = '''\
+    class Animal(object):
+        def __new__(cls, name, lastname, age, spec, extinct, group, friends):
+            ...
+    '''
+    mod = fromText(src, systemcls=systemcls)
+
+    assert getConstructorsText(mod.contents['Animal']) == "Animal(name, lastname, age, spec, ...)"
+
+@systemcls_param
+def test_constructor_five_paramters(systemcls: Type[model.System]) -> None:
+    src = '''\
+    class Animal(object):
+        def __new__(cls, name, lastname, age, spec, extinct):
+            ...
+    '''
+    mod = fromText(src, systemcls=systemcls)
+
+    assert getConstructorsText(mod.contents['Animal']) == "Animal(name, lastname, age, spec, extinct)"
+
+@systemcls_param
+def test_default_constructors(systemcls: Type[model.System]) -> None:
+    src = '''\
+    class Animal(object):
+        def __init__(self):
+            ...
+        def __new__(cls):
+            ...
+        @classmethod
+        def new(cls) -> 'Animal':
+            ...
+        '''
+
+    mod = fromText(src, systemcls=systemcls)
+    assert getConstructorsText(mod.contents['Animal']) == "Animal.new()"
+
+    src = '''\
+    class Animal(object):
+        def __init__(self):
+            ...
+        '''
+
+    mod = fromText(src, systemcls=systemcls)
+    assert getConstructorsText(mod.contents['Animal']) == ""
+
+    src = '''\
+    class Animal(object):
+        def __init__(self):
+            "thing"
+        '''
+
+    mod = fromText(src, systemcls=systemcls)
+    assert getConstructorsText(mod.contents['Animal']) == "Animal()"
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_attrs.py` & `pydoctor-23.4.0/pydoctor/test/test_attrs.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_colorize.py` & `pydoctor-23.4.0/pydoctor/test/test_colorize.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_commandline.py` & `pydoctor-23.4.0/pydoctor/test/test_commandline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from contextlib import redirect_stdout
 from io import StringIO
 from pathlib import Path
+import re
 import sys
 
-from pytest import raises
-
 from pydoctor.options import Options
 from pydoctor import driver
 
 from . import CapSys
 
 
 def geterrtext(*options: str) -> str:
@@ -222,23 +221,38 @@
         f'{link}/pydoctor/test/testpackages/basic/'
         ])
     assert exit_code == 0
 
 
 def test_main_source_outside_basedir(capsys: CapSys) -> None:
     """
-    If a --project-base-dir is given, all package and module paths must
-    be located inside that base directory.
-    """
-    with raises(SystemExit):
-        driver.main(args=[
-            '--project-base-dir=docs',
-            'pydoctor/test/testpackages/basic/'
-            ])
-    assert "Source path lies outside base directory:" in capsys.readouterr().err
+    If a --project-base-dir is given, all package and module paths should
+    be located inside that base directory if source links wants to be generated.
+    Otherwise it's OK, but no source links will be genrated
+    """
+    assert driver.main(args=[
+        '--html-viewsource-base=notnone',
+        '--project-base-dir=docs',
+        'pydoctor/test/testpackages/basic/'
+        ]) == 0
+    re.match("No source links can be generated for module .+/pydoctor/test/testpackages/basic/: source path lies outside base directory .+/docs\n", 
+        capsys.readouterr().out)
+
+    assert driver.main(args=[
+        '--project-base-dir=docs',
+        'pydoctor/test/testpackages/basic/'
+        ]) == 0
+    assert "No source links can be generated" not in capsys.readouterr().out
+
+    assert driver.main(args=[
+        '--html-viewsource-base=notnone',
+        '--project-base-dir=pydoctor/test/testpackages/',
+        'pydoctor/test/testpackages/basic/'
+        ]) == 0
+    assert "No source links can be generated" not in capsys.readouterr().out
 
 
 def test_make_intersphix(tmp_path: Path) -> None:
     """
     --make-intersphinx without --make-html will only produce the Sphinx inventory object.
 
     This is also an integration test for the Sphinx inventory writer.
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_configparser.py` & `pydoctor-23.4.0/pydoctor/test/test_configparser.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_cyclic_imports_base_classes.py` & `pydoctor-23.4.0/pydoctor/test/test_cyclic_imports_base_classes.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_epydoc2stan.py` & `pydoctor-23.4.0/pydoctor/test/test_epydoc2stan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from typing import List, Optional, cast, TYPE_CHECKING
+from typing import List, Optional, Type, cast, TYPE_CHECKING
 import re
 
 from pytest import mark, raises
 import pytest
 from twisted.web.template import Tag, tags
 
 from pydoctor import epydoc2stan, model, linker
-from pydoctor.epydoc.markup import DocstringLinker
+from pydoctor.epydoc.markup import DocstringLinker, get_supported_docformats
 from pydoctor.stanutils import flatten, flatten_text
 from pydoctor.epydoc.markup.epytext import ParsedEpytextDocstring
 from pydoctor.sphinx import SphinxInventory
 from pydoctor.test.test_astbuilder import fromText, unwrap
 from pydoctor.test import CapSys
 from pydoctor.templatewriter.search import stem_identifier
-from pydoctor.utils import partialclass
 
 if TYPE_CHECKING:
     from twisted.web.template import Flattenable
 
 
 def test_multiple_types() -> None:
     mod = fromText('''
@@ -67,19 +66,45 @@
     else:
         # Summaries are now generated without englobing <span> when we don't need one. 
         assert stan.tagName == '', stan
     return flatten(stan.children)
 
 
 def test_html_empty_module() -> None:
+    # checks the presence of at least one paragraph on all docstrings
     mod = fromText('''
     """Empty module."""
     ''')
     assert docstring2html(mod) == "<div>\n<p>Empty module.</p>\n</div>"
 
+    mod = fromText('''
+    """
+    Empty module.
+    
+    Another paragraph.
+    """
+    ''')
+    assert docstring2html(mod) == "<div>\n<p>Empty module.</p>\n<p>Another paragraph.</p>\n</div>"
+
+    mod = fromText('''
+    """C{thing}"""
+    ''', modname='module')
+    assert docstring2html(mod) == '<div>\n<p>\n<tt class="rst-docutils literal">thing</tt>\n</p>\n</div>'
+
+    mod = fromText('''
+    """My C{thing}."""
+    ''', modname='module')
+    assert docstring2html(mod) == '<div>\n<p>My <tt class="rst-docutils literal">thing</tt>.</p>\n</div>'
+
+    mod = fromText('''
+    """
+    @note: There is no paragraph here. 
+    """
+    ''')
+    assert '<p>' not in docstring2html(mod)
 
 def test_xref_link_not_found() -> None:
     """A linked name that is not found is output as text."""
     mod = fromText('''
     """This link leads L{nowhere}."""
     ''', modname='test')
     html = docstring2html(mod)
@@ -160,34 +185,77 @@
     func = mod.contents['nop']
     lines = docstring2html(func).split('\n')
     assert '<td class="fieldName">Returns</td>' not in lines
 
 
 def test_func_undocumented_return_something() -> None:
     """When the returned value is undocumented (no 'return' field) and its type
-    annotation is not None, include the "Returns" entry in the output.
+    annotation is not None, do not include the "Returns" entry in the field
+    table. It will be shown in the signature.
     """
     mod = fromText('''
     def get_answer() -> int:
         return 42
     ''')
     func = mod.contents['get_answer']
     lines = docstring2html(func).splitlines()
     expected_html = [
-        '<div>', '<p class="undocumented">Undocumented</p>',
-        '<table class="fieldTable">',
+        '<div>',
+        '<p class="undocumented">Undocumented</p>',
+        '</div>',
+    ]
+    assert lines == expected_html, str(lines)
+
+def test_func_only_single_param_doc() -> None:
+    """When only a single parameter is documented, all parameters show with
+    undocumented parameters marked as such.
+    """
+    mod = fromText('''
+    def f(x, y):
+        """
+        @param x: Actual documentation.
+        """
+    ''')
+    lines = docstring2html(mod.contents['f']).splitlines()
+    expected_html = [
+        '<div>', '<table class="fieldTable">',
         '<tr class="fieldStart">',
-        '<td class="fieldName" colspan="2">Returns</td>',
-        '</tr>',
-        '<tr>', '<td class="fieldArgContainer">', '<code>int</code>',
-        '</td>',
-        '<td class="fieldArgDesc">',
+        '<td class="fieldName" colspan="2">Parameters</td>',
+        '</tr>', '<tr>',
+        '<td class="fieldArgContainer">',
+        '<span class="fieldArg">x</span>',
+        '</td>', '<td class="fieldArgDesc">Actual documentation.</td>',
+        '</tr>', '<tr>',
+        '<td class="fieldArgContainer">',
+        '<span class="fieldArg">y</span>',
+        '</td>', '<td class="fieldArgDesc">',
         '<span class="undocumented">Undocumented</span>',
-        '</td>', '</tr>', '</table>', '</div>'
-        ]
+        '</td>', '</tr>', '</table>', '</div>',
+    ]
+    assert lines == expected_html, str(lines)
+
+def test_func_only_return_doc() -> None:
+    """When only return is documented but not parameters, only the return
+    section is visible.
+    """
+    mod = fromText('''
+    def f(x: str):
+        """
+        @return: Actual documentation.
+        """
+    ''')
+    lines = docstring2html(mod.contents['f']).splitlines()
+    expected_html = [
+        '<div>', '<table class="fieldTable">',
+        '<tr class="fieldStart">',
+        '<td class="fieldName" colspan="2">Returns</td>',
+        '</tr>', '<tr>',
+        '<td colspan="2">Actual documentation.</td>',
+        '</tr>', '</table>', '</div>',
+    ]
     assert lines == expected_html, str(lines)
 
 # These 3 tests fails because AnnotationDocstring is not using node2stan() yet.
 
 @pytest.mark.xfail
 def test_func_arg_and_ret_annotation() -> None:
     annotation_mod = fromText('''
@@ -235,34 +303,68 @@
         @rtype: C{bool}
         """
     ''')
     annotation_fmt = docstring2html(annotation_mod.contents['f'])
     classic_fmt = docstring2html(classic_mod.contents['f'])
     assert annotation_fmt == classic_fmt
 
-@pytest.mark.xfail
-def test_func_arg_when_doc_missing() -> None:
+def test_func_arg_when_doc_missing_ast_types() -> None:
+    """
+    Type hints are now included in the signature, so no need to 
+    docucument them twice in the param table, only if non of them has documentation.
+    """
     annotation_mod = fromText('''
     def f(a: List[str], b: int) -> bool:
         """
         Today I will not document details
         """
     ''')
-    classic_mod = fromText('''
-    def f(a):
-        """
-        Today I will not document details
+    annotation_fmt = docstring2html(annotation_mod.contents['f'])
+    
+    assert 'fieldTable' not in annotation_fmt
+    assert 'b:' not in annotation_fmt
+
+def _get_test_func_arg_when_doc_missing_docstring_fields_types_cases() -> List[str]:
+    case1="""
         @type a: C{List[str]}
         @type b: C{int}
-        @rtype: C{bool}
+        @rtype: C{bool}"""
+    
+    case2="""
+        Args
+        ----
+        a: List[str]
+        b: int
+        
+        Returns
+        -------
+        bool:"""
+    return [case1,case2]
+
+@pytest.mark.parametrize('sig', ['(a)', '(a:List[str])', '(a) -> bool', '(a:List[str], b:int) -> bool'])
+@pytest.mark.parametrize('doc', _get_test_func_arg_when_doc_missing_docstring_fields_types_cases())
+def test_func_arg_when_doc_missing_docstring_fields_types(sig:str, doc:str) -> None:
+    """
+    When type fields are present (whether they are coming from napoleon extension or epytext), always show the param table.
+    """
+    
+    classic_mod = fromText(f'''
+    __docformat__ = "{'epytext' if '@type' in doc else 'numpy'}"
+    def f{sig}:
+        """
+        Today I will not document details
+        {doc}
         """
     ''')
-    annotation_fmt = docstring2html(annotation_mod.contents['f'])
+
     classic_fmt = docstring2html(classic_mod.contents['f'])
-    assert annotation_fmt == classic_fmt
+    assert 'fieldTable' in classic_fmt
+    assert '<span class="fieldArg' in classic_fmt
+    assert 'Parameters' in classic_fmt
+    assert 'Returns' in classic_fmt
 
 def test_func_param_duplicate(capsys: CapSys) -> None:
     """Warn when the same parameter is documented more than once."""
     mod = fromText('''
     def f(x, y):
         """
         @param x: Actual documentation.
@@ -589,41 +691,14 @@
     
     for part in expected_parts:
         assert part in epy_with_asterixes_fmt
     
     captured = capsys.readouterr().out
     assert not captured
 
-def test_func_starargs_no_docstring(capsys: CapSys) -> None:
-    """
-    Star arguments, even if there are not docstring attached, will be rendered with stars.
-
-    @note: This test might not pass anymore when we include the annotations inside the signatures.
-    """
-
-    mod = fromText('''
-    def f(args:str, kwargs:str, *a:Any, **kwa:Any) -> None:
-        """
-        Do something with var-positional and var-keyword arguments.
-        """
-    ''', modname='<great>')
-
-    mod_fmt = docstring2html(mod.contents['f'])
-    
-    expected_parts = ['<span class="fieldArg">args:</span>', 
-                      '<span class="fieldArg">kwargs:</span>',
-                      '<span class="fieldArg">*a:</span>',
-                      '<span class="fieldArg">**kwa:</span>',]
-    
-    for part in expected_parts:
-        assert part in mod_fmt, mod_fmt
-    
-    captured = capsys.readouterr().out
-    assert not captured
-
 def test_summary() -> None:
     mod = fromText('''
     def single_line_summary():
         """
         Lorem Ipsum
 
         Ipsum Lorem
@@ -770,23 +845,123 @@
     ''', modname='test')
     a = mod.contents['a']
     assert isinstance(a, model.Attribute)
     epydoc2stan.format_docstring(a)
     captured = capsys.readouterr().out
     assert captured == "test:5: Field in variable docstring should not include a name\n"
 
+@pytest.mark.parametrize('linkercls', [linker._EpydocLinker])
+def test_EpydocLinker_switch_context(linkercls:Type[linker._EpydocLinker]) -> None:
+    """
+    Test for switching the page context of the EpydocLinker.
+    """
+    mod = fromText('''
+    v=0
+    class Klass:
+        class InnerKlass(Klass):
+            def f():...
+            Klass = 'not this one!'
+            class v: 
+                'not this one!'
+    ''', modname='test')
+    Klass = mod.contents['Klass']
+    assert isinstance(Klass, model.Class)
+    InnerKlass = Klass.contents['InnerKlass']
+    assert isinstance(InnerKlass, model.Class)
+    
+    # patch with the linkercls
+    mod._linker = linkercls(mod)
+    Klass._linker = linkercls(Klass)
+    InnerKlass._linker = linkercls(InnerKlass)
+
+    # Evaluating the name of the base classes must be done in the upper scope
+    # in order to avoid the following to happen:
+    assert 'href="#Klass"' in flatten(InnerKlass.docstring_linker.link_to('Klass', 'Klass'))
+    
+    with Klass.docstring_linker.switch_context(InnerKlass):
+        assert 'href="test.Klass.html"' in flatten(Klass.docstring_linker.link_to('Klass', 'Klass'))
+    
+    assert 'href="#v"' in flatten(mod.docstring_linker.link_to('v', 'v'))
+    
+    with mod.docstring_linker.switch_context(InnerKlass):
+        assert 'href="index.html#v"' in flatten(mod.docstring_linker.link_to('v', 'v'))
+
+@pytest.mark.parametrize('linkercls', [linker._EpydocLinker])
+def test_EpydocLinker_switch_context_is_reentrant(linkercls:Type[linker._EpydocLinker], capsys:CapSys) -> None:
+    """
+    We can nest several calls to switch_context(), and links will still be valid and warnings line will be correct.
+    """
+    
+    mod = fromText('''
+    "L{thing.notfound}"
+    v=0
+    class Klass:
+        "L{thing.notfound}"
+        ...
+    ''', modname='test')
+    
+    Klass = mod.contents['Klass']
+    assert isinstance(Klass, model.Class)
+    
+    for ob in mod.system.allobjects.values():
+        epydoc2stan.ensure_parsed_docstring(ob)
+    
+    # patch with the linkercls
+    mod._linker = linkercls(mod)
+    Klass._linker = linkercls(Klass)
+
+    with Klass.docstring_linker.switch_context(mod):
+        assert 'href="#v"' in flatten(Klass.docstring_linker.link_to('v', 'v'))
+        with Klass.docstring_linker.switch_context(Klass):
+            assert 'href="index.html#v"' in flatten(Klass.docstring_linker.link_to('v', 'v'))
+    
+    assert capsys.readouterr().out == ''
+
+    mod.parsed_docstring.to_stan(mod.docstring_linker) #type:ignore
+    mod.parsed_docstring.get_summary().to_stan(mod.docstring_linker) # type:ignore
+
+    warnings = ['test:2: Cannot find link target for "thing.notfound" (you can link to external docs with --intersphinx)']
+    if linkercls is linker._EpydocLinker:
+        warnings = warnings * 2
+    assert capsys.readouterr().out.strip().splitlines() == warnings
+
+    # This is wrong:
+    Klass.parsed_docstring.to_stan(mod.docstring_linker) # type:ignore
+    Klass.parsed_docstring.get_summary().to_stan(mod.docstring_linker) # type:ignore
+    
+    # Because the warnings will be reported on line 2
+    warnings = ['test:2: Cannot find link target for "thing.notfound" (you can link to external docs with --intersphinx)']
+    warnings = warnings * 2
+    
+    assert capsys.readouterr().out.strip().splitlines() == warnings
+
+    # assert capsys.readouterr().out == ''
+
+    # Reset stan and summary, because they are supposed to be cached.
+    Klass.parsed_docstring._stan = None # type:ignore
+    Klass.parsed_docstring._summary = None # type:ignore
+
+    # This is better:
+    with mod.docstring_linker.switch_context(Klass):
+        Klass.parsed_docstring.to_stan(mod.docstring_linker) # type:ignore
+        Klass.parsed_docstring.get_summary().to_stan(mod.docstring_linker) # type:ignore
 
+    warnings = ['test:5: Cannot find link target for "thing.notfound" (you can link to external docs with --intersphinx)']
+    warnings = warnings * 2
+    
+    assert capsys.readouterr().out.strip().splitlines() == warnings
+    
 def test_EpydocLinker_look_for_intersphinx_no_link() -> None:
     """
     Return None if inventory had no link for our markup.
     """
     system = model.System()
     target = model.Module(system, 'ignore-name')
     sut = target.docstring_linker
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    assert isinstance(sut, linker._EpydocLinker)
 
     result = sut.look_for_intersphinx('base.module')
 
     assert None is result
 
 
 def test_EpydocLinker_look_for_intersphinx_hit() -> None:
@@ -795,15 +970,15 @@
     """
     system = model.System()
     inventory = SphinxInventory(system.msg)
     inventory._links['base.module.other'] = ('http://tm.tld', 'some.html')
     system.intersphinx = inventory
     target = model.Module(system, 'ignore-name')
     sut = target.docstring_linker
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    assert isinstance(sut, linker._EpydocLinker)
 
     result = sut.look_for_intersphinx('base.module.other')
 
     assert 'http://tm.tld/some.html' == result
 
 def test_EpydocLinker_adds_intersphinx_link_css_class() -> None:
     """
@@ -811,15 +986,15 @@
     """
     system = model.System()
     inventory = SphinxInventory(system.msg)
     inventory._links['base.module.other'] = ('http://tm.tld', 'some.html')
     system.intersphinx = inventory
     target = model.Module(system, 'ignore-name')
     sut = target.docstring_linker
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    assert isinstance(sut, linker._EpydocLinker)
 
     result1 = sut.link_xref('base.module.other', 'base.module.other', 0).children[0] # wrapped in a code tag
     result2 = sut.link_to('base.module.other', 'base.module.other')
     
     res = flatten(result2)
     assert flatten(result1) == res
     assert 'class="intersphinx-link"' in res
@@ -832,15 +1007,15 @@
     """
     system = model.System()
     inventory = SphinxInventory(system.msg)
     inventory._links['base.module.other'] = ('http://tm.tld', 'some.html')
     system.intersphinx = inventory
     target = model.Module(system, 'ignore-name')
     sut = target.docstring_linker
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    assert isinstance(sut, linker._EpydocLinker)
 
     url = sut.resolve_identifier('base.module.other')
     url_xref = sut._resolve_identifier_xref('base.module.other', 0)
 
     assert "http://tm.tld/some.html" == url
     assert "http://tm.tld/some.html" == url_xref
 
@@ -858,15 +1033,15 @@
     # Here we set up the target module as it would have this import.
     # from ext_package import ext_module
     ext_package = model.Module(system, 'ext_package')
     target.contents['ext_module'] = model.Module(
         system, 'ext_module', parent=ext_package)
 
     sut = target.docstring_linker
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    assert isinstance(sut, linker._EpydocLinker)
 
     # This is called for the L{ext_module<Pretty Text>} markup.
     url = sut.resolve_identifier('ext_module')
     url_xref = sut._resolve_identifier_xref('ext_module', 0)
 
     assert "http://tm.tld/some.html" == url
     assert "http://tm.tld/some.html" == url_xref
@@ -883,15 +1058,15 @@
     target = model.Module(system, 'ignore-name')
     # Here we set up the target module as it would have this import.
     # from ext_package import ext_module
     ext_package = model.Module(system, 'ext_package')
     target.contents['ext_module'] = model.Module(
         system, 'ext_module', parent=ext_package)
     sut = target.docstring_linker
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    assert isinstance(sut, linker._EpydocLinker)
 
     # This is called for the L{ext_module} markup.
     assert sut.resolve_identifier('ext_module') is None
     assert not capsys.readouterr().out
     with raises(LookupError):
         sut._resolve_identifier_xref('ext_module', 0)
 
@@ -923,15 +1098,15 @@
 
     mod = fromText('''
     class C:
         socket = None
     ''')
     mod.system.intersphinx = cast(SphinxInventory, InMemoryInventory())
     _linker = mod.docstring_linker
-    assert isinstance(_linker, linker._CachedEpydocLinker)
+    assert isinstance(_linker, linker._EpydocLinker)
 
     url = _linker.resolve_identifier('socket.socket')
     url_xref = _linker._resolve_identifier_xref('socket.socket', 0)
 
     assert 'https://docs.python.org/3/library/socket.html#socket.socket' == url
     assert 'https://docs.python.org/3/library/socket.html#socket.socket' == url_xref
     assert not capsys.readouterr().out
@@ -946,204 +1121,84 @@
         pass
     ''', modname='internal_module')
     system = int_mod.system
 
     # Dummy module that we want to link from.
     target = model.Module(system, 'ignore-name')
     sut = target.docstring_linker
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    assert isinstance(sut, linker._EpydocLinker)
     url = sut.resolve_identifier('internal_module.C')
     xref = sut._resolve_identifier_xref('internal_module.C', 0)
 
     assert "internal_module.C.html" == url
     assert int_mod.contents['C'] is xref
 
-def test_CachedEpydocLinker() -> None:
+def test_EpydocLinker_None_context() -> None:
     """
-    The CachedEpydocLinker returns the same Tag object without resolving the name and re-creating the link tag all the time.
-    """
-    system = model.System()
-    inventory = SphinxInventory(system.msg)
-    inventory._links['base.module.other'] = ('http://tm.tld', 'some.html')
-    system.intersphinx = inventory
-    target = model.Module(system, 'ignore-name')
-    
-    sut = _TestCachedEpydocLinker(target, max_lookups=1)
-
-    result2 = sut.link_to('base.module.other', 'base.module.other')
-    assert 'base.module.other' in sut._link_to_cache
-    assert len(sut._link_to_cache['base.module.other'][True])==1
-    result1 = sut.link_xref('base.module.other', 'base.module.other', 0).children[0] # wrapped in a code tag
-    assert len(sut._link_xref_cache['base.module.other'][True])==0
-    assert len(sut._link_to_cache['base.module.other'][True])==1
-    result3 = sut.link_to('base.module.other', 'other')
-    assert len(sut._link_to_cache['base.module.other'][True])==2
-    result4 = sut.link_xref('base.module.other', 'other', 0).children[0]
-    assert len(sut._link_to_cache['base.module.other'][True])==2
-    assert len(sut._link_xref_cache['base.module.other'][True])==0
-
-    res = flatten(result2)
-    assert flatten(result1) == res == '<a href="http://tm.tld/some.html" class="intersphinx-link">base.module.other</a>'
-    assert flatten(result3) == flatten(result4) == '<a href="http://tm.tld/some.html" class="intersphinx-link">other</a>'
-
-class _TestCachedEpydocLinker(linker._CachedEpydocLinker):
-    """
-    Docstring linker for testing the caching of results.
-    """
-    
-    def __init__(self, obj: model.Documentable, max_lookups:int, same_page_optimization:bool=True) -> None:
-        super().__init__(obj, same_page_optimization)
-        self.lookups = 0
-        self.max_lookups = max_lookups
-
-    def link_to(self, target: str, label: "Flattenable") -> Tag:
-        link = self._lookup_cached_link_to(target, label)
-        if link is None: 
-            if self.lookups<self.max_lookups:
-                self.lookups+=1
-                link = super().link_to(target, label)
-            else:
-                raise AssertionError(f"Should not lookup link to {target!r}. Max lookups reached ({self.max_lookups} lookups). ")
-        return link
-    
-    def link_xref(self, target: str, label: "Flattenable", lineno:int) -> Tag:
-        link = self._lookup_cached_link_xref(target, label, lineno)
-        if link is None: 
-            if self.lookups<self.max_lookups:
-                self.lookups+=1
-                link = super().link_xref(target, label, lineno)
-            else:
-                raise AssertionError(f"Should not lookup link to {target!r}. Max lookups reached ({self.max_lookups} lookups). ")
-        else:
-            link = tags.code(link)
-        return link
-
-def test_TestCachedEpydocLinker() -> None:
-    """
-    A test case for the testing linker L{_TestCachedEpydocLinker}. 
-    The test linker is initialized with a maximum number of non-cached requests it can make
-    and an AssertionError is raised if it makes too many requests.
-    """
-    system = model.System()
-    inventory = SphinxInventory(system.msg)
-    inventory._links['base.module.other'] = ('http://tm.tld', 'some.html')
-    system.intersphinx = inventory
-    target = model.Module(system, 'ignore-name')
-    
-    sut = _TestCachedEpydocLinker(target, 2)
-    sut.link_xref('base.module.other', 'other', 1)
-    assert sut.lookups==1
-    assert len(sut._link_xref_cache['base.module.other'][True])==1
-    sut.link_xref('notfound', 'notfound', 1)
-    assert sut.lookups==2
-    assert len(sut._link_xref_cache['notfound'][True])==1
+    When the linker context is None, 
 
-    with pytest.raises(AssertionError):
-        sut.link_xref('anothername', 'again notfound', 1)
-
-def test_CachedEpydocLinker_same_page_optimization() -> None:
-    """
-    When _CachedEpydocLinker.same_page_optimization is True, the linker will create URLs with only the anchor
+    The linker will create URLs with only the anchor
     if we're lnking to an object on the same page. 
     
     Otherwise it will always use return a URL with a filename, this is used to generate the summaries.
     """
     mod = fromText('''
     base=1
     class someclass: ...
     ''', modname='module')
-    sut = _TestCachedEpydocLinker(mod, 3) # Raise if it makes more than 3 lookups.
-    assert isinstance(sut, linker._CachedEpydocLinker)
+    sut = mod.docstring_linker
+    assert isinstance(sut, linker._EpydocLinker)
     
-    sut.same_page_optimization=False
-    assert sut.link_to('base','module.base').attributes['href']=='index.html#base'
-    assert len(sut._link_to_cache['base'][False])==1, repr(sut._link_to_cache['base'][False])
-    assert sut.link_to('base','base').attributes['href']=='index.html#base'
-    assert len(sut._link_to_cache['base'][False])==2, sut._link_to_cache['base'][False]
-    assert sut.link_to('someclass','some random name').attributes['href']=='module.someclass.html'
-
-    sut.same_page_optimization=True
-    assert sut.link_to('base','base').attributes['href']=='#base'
-    assert sut.link_to('base','base').attributes['href']=='#base'
-    assert len(sut._link_to_cache['base'][True])==1
-    assert sut.link_to('base', tags.transparent('module.base')).attributes['href']=='#base'
-    assert sut.link_to('base', tags.transparent('module.base')).attributes['href']=='#base' 
-    # Tags are not properly understood right now but that's ok since these are only used
-    # when inserting a link with nested markup like L{B{driver} <pydoctor.driver>}
-    assert len(sut._link_to_cache['base'][False])==2
-    assert len(sut._link_to_cache['base'][True])==3
-
-    assert sut.link_to('someclass','some other name').attributes['href']=='module.someclass.html'
-    assert sut.link_to('someclass','a third name').attributes['href']=='module.someclass.html'
-    assert len(sut._link_to_cache['someclass'][False])==1
-    assert len(sut._link_to_cache['someclass'][True])==2
-
-    assert sut.link_to('notfound', 'notfound').children[0] == 'notfound'
-    assert sut.link_to('notfound', 'notfound.notfound').children[0] == 'notfound.notfound'
-    assert len(sut._link_to_cache['notfound'][True])==2
+    assert sut.page_url == mod.url == cast(linker._EpydocLinker,mod.contents['base'].docstring_linker).page_url
+    
+    with sut.switch_context(None):
+        assert sut.page_url ==''
+        
+        assert sut.link_to('base','module.base').attributes['href']=='index.html#base'
+        assert sut.link_to('base','module.base').children[0]=='module.base'
+        
+        assert sut.link_to('base','base').attributes['href']=='index.html#base'
+        assert sut.link_to('base','base').children[0]=='base'
+        
+        assert sut.link_to('someclass','some random name').attributes['href']=='module.someclass.html'
+        assert sut.link_to('someclass','some random name').children[0]=='some random name'
 
-def test_CachedEpydocLinker_warnings(capsys: CapSys) -> None:
+def test_EpydocLinker_warnings(capsys: CapSys) -> None:
     """
     Warnings should be reported only once per invalid name per line, 
     no matter the number of times we call summary2html() or docstring2html() or the order we call these functions.
     """
-    _default_class = linker._CachedEpydocLinker
-    try:
-        linker._CachedEpydocLinker = partialclass(_TestCachedEpydocLinker, max_lookups=2) # type:ignore
-        src = '''
-        """
-        L{base} L{regular text <notfound>} L{notfound} 
-
-        L{regular text <base>} L{B{look at the base} <base>} L{I{Important class} <notfound>}  L{notfound} 
-        """
-        base=1
-        '''
-
-        mod = fromText(src, modname='module')
-        assert isinstance(mod.docstring_linker, _TestCachedEpydocLinker)
-        assert mod.docstring_linker.max_lookups==2
-        assert 'href="#base"' in docstring2html(mod)
-        captured = capsys.readouterr().out
-
-        # Here, we can see that the warning got reported only 2 times but 
-        # the error is present 4 times in the docstring. This is because 
-        # links are on the same line.
+    src = '''
+    """
+    L{base} L{regular text <notfound>} L{notfound} 
 
-        # The rationale about xref warnings is now the following: 
-        # - Warns only once per unresolved identifier per line. 
+    L{regular text <base>} L{B{look at the base} <base>} L{I{Important class} <notfound>}  L{notfound} 
+    """
+    base=1
+    '''
 
-        assert captured == 'module:3: Cannot find link target for "notfound"\nmodule:5: Cannot find link target for "notfound"\n'
+    mod = fromText(src, modname='module')
 
-        assert 'href="index.html#base"' in summary2html(mod)
-        summary2html(mod); docstring2html(mod)
-        
-        captured = capsys.readouterr().out
+    assert 'href="#base"' in docstring2html(mod)
+    captured = capsys.readouterr().out
 
-        # Other warnings are not logged if running summary2html and docstring2html multiple times.
-        assert captured == ''
+    # The rationale about xref warnings is to warn when the target cannot be found.
 
-        mod = fromText(src, modname='module')
-        assert isinstance(mod.docstring_linker, _TestCachedEpydocLinker)
-        assert mod.docstring_linker.max_lookups==2
-        assert 'href="index.html#base"' in summary2html(mod)
-        captured = capsys.readouterr().out
+    assert captured == ('module:3: Cannot find link target for "notfound"'
+                        '\nmodule:3: Cannot find link target for "notfound"'
+                        '\nmodule:5: Cannot find link target for "notfound"'
+                        '\nmodule:5: Cannot find link target for "notfound"\n')
 
-        assert captured == 'module:3: Cannot find link target for "notfound"\n'
-        
-        html = docstring2html(mod)
-        captured = capsys.readouterr().out
-        assert captured == 'module:5: Cannot find link target for "notfound"\n'
-        assert 'href="#base"' in html
-        
-        docstring2html(mod); summary2html(mod)
-        captured = capsys.readouterr().out
-        assert captured == ''
+    assert 'href="index.html#base"' in summary2html(mod)
+    summary2html(mod)
     
-    finally:
-        linker._CachedEpydocLinker = _default_class # type:ignore
+    captured = capsys.readouterr().out
+
+    # No warnings are logged when generating the summary.
+    assert captured == ''
 
 def test_xref_not_found_epytext(capsys: CapSys) -> None:
     """
     When a link in an epytext docstring cannot be resolved, the reference
     and the line number of the link should be reported.
     """
 
@@ -1529,20 +1584,26 @@
 def test_insert_break_points_dotted_name() -> None:
     assert insert_break_points('mod.__some_very_long_name__') == 'mod<wbr></wbr>.__some<wbr></wbr>_very<wbr></wbr>_long<wbr></wbr>_name__'
     assert insert_break_points('_mod.__SOME_VERY_LONG_NAME__') == '_mod<wbr></wbr>.__SOME<wbr></wbr>_VERY<wbr></wbr>_LONG<wbr></wbr>_NAME__'
     assert insert_break_points('pack.mod.__someVeryLongName__') == 'pack<wbr></wbr>.mod<wbr></wbr>.__some<wbr></wbr>Very<wbr></wbr>Long<wbr></wbr>Name__'
     assert insert_break_points('pack._mod_.__einÜberlangerName__') == 'pack<wbr></wbr>._mod_<wbr></wbr>.__ein<wbr></wbr>Überlanger<wbr></wbr>Name__'
 
 def test_stem_identifier() -> None:
-    assert list(stem_identifier('__some_very_long_name__')) == [
-        'very', 'long', 'name'  # 'some' has been filtered out because it's part of the stop words.
-    ] 
+    assert list(stem_identifier('__some_very_long_name__')) == list(stem_identifier('__some_very_very_long_name__')) == [
+        'some', 'very', 'long', 'name',]
+    
+    assert list(stem_identifier('transitivity_maximum')) == [
+        'transitivity', 'maximum',]
+    
+    assert list(stem_identifier('ForEach')) == [
+        'For', 'Each',]
+
     assert list(stem_identifier('__someVeryLongName__')) == [
-        'Very', 'Long', 'Name'
-    ]
+        'some', 'Very', 'Long', 'Name', ]
+    
     assert list(stem_identifier('_name')) == ['name']
     assert list(stem_identifier('name')) == ['name']
     assert list(stem_identifier('processModuleAST')) == ['process', 'Module', 'AST']
 
 def test_self_cls_in_function_params(capsys: CapSys) -> None:
     """
     'self' and 'cls' in parameter table of regular function should appear because 
@@ -1632,7 +1693,111 @@
     assert '<span class="fieldArg">self</span>' in html_bar
     assert '<span class="fieldArg">self</span>' in html_watch
     assert '<span class="fieldArg">cls</span>' in html_leave
 
     assert '<span class="fieldArg">cls</span>' not in html_which
     assert '<span class="fieldArg">self</span>' not in html_init
     assert '<span class="fieldArg">self</span>' in html_bool
+
+
+def test_not_found_annotation_does_not_create_link() -> None:
+    """
+    The docstring linker cache does not create empty <a> tags.
+    """
+
+    
+    from pydoctor.test.test_templatewriter import getHTMLOf
+
+    src = '''\
+    __docformat__ = 'numpy'
+
+    def link_to(identifier, label: NotFound):
+        """
+        :param label: the lable of the link.
+        :type identifier: Union[str, NotFound]
+        """
+
+    '''
+
+    mod = fromText(src)
+
+    html = getHTMLOf(mod)
+
+    assert '<a>NotFound</a>' not in html
+
+def test_docformat_skip_processtypes() -> None:
+    assert all([d in get_supported_docformats() for d in epydoc2stan._docformat_skip_processtypes])
+
+def test_returns_undocumented_still_show_up_if_params_documented() -> None:
+    """
+    The returns section will show up if any of the 
+    parameter are documented and the fucntion has a return annotation.
+    """
+    src = '''
+    def f(c:int) -> bool:
+        """
+        @param c: stuff
+        """
+    def g(c) -> bool:
+        """
+        @type c: int
+        """
+    def h(c):
+        """
+        @param c: stuff
+        """
+    def i(c) -> None:
+        """
+        @param c: stuff
+        """
+    '''
+
+    mod = fromText(src)
+
+    html_f = docstring2html(mod.contents['f'])
+    html_g = docstring2html(mod.contents['g'])
+    html_h = docstring2html(mod.contents['h'])
+    html_i = docstring2html(mod.contents['i'])
+
+    assert 'Returns</td>' in html_f
+    assert 'Returns</td>' in html_g
+
+    assert 'Returns</td>' not in html_h
+    assert 'Returns</td>' not in html_i
+
+def test_invalid_epytext_renders_as_plaintext(capsys: CapSys) -> None:
+    """
+    An invalid epytext docstring will be rederered as plaintext.
+    """
+
+    mod = fromText(''' 
+    def func():
+        """
+            Title
+            ~~~~~
+            
+
+            Hello
+            ~~~~~
+        """
+        pass
+    
+    ''', modname='invalid')
+
+    expected = """<div>
+<p class="pre">Title
+~~~~~
+
+
+Hello
+~~~~~</p>
+</div>"""
+    
+    actual = docstring2html(mod.contents['func'])
+    captured = capsys.readouterr().out
+    assert captured == ('invalid:4: bad docstring: Wrong underline character for heading.\n'
+                        'invalid:8: bad docstring: Wrong underline character for heading.\n')
+    assert actual  == expected
+
+    assert docstring2html(mod.contents['func'], docformat='plaintext') == expected
+    captured = capsys.readouterr().out
+    assert captured == ''
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_model.py` & `pydoctor-23.4.0/pydoctor/test/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,14 +164,17 @@
         log.append((part, msg))
     sut.msg = log_msg # type: ignore[assignment]
 
     class Cache(CacheT):
         """Avoid touching the network."""
         def get(self, url: str) -> bytes:
             return url_content[url]
+        def close(self) -> None:
+            return None
+        
 
     sut.fetchIntersphinxInventories(Cache())
 
     assert [] == log
     assert (
         'http://sphinx/sp.html' ==
         sut.intersphinx.getLink('sphinx.module')
@@ -231,14 +234,29 @@
         pass
     '''
     mod = fromText(src)
     C = mod.contents['C']
     assert isinstance(C, model.Class)
     assert C.constructor_params.keys() == {'self', 'a', 'b'}
 
+def test_constructor_params_new() -> None:
+    src = '''
+    class A:
+        def __new__(cls, **kwargs):
+            pass
+    class B:
+        def __init__(self, a: int, b: str):
+            pass
+    class C(A, B):
+        pass
+    '''
+    mod = fromText(src)
+    C = mod.contents['C']
+    assert isinstance(C, model.Class)
+    assert C.constructor_params.keys() == {'cls', 'kwargs'}
 
 def test_docstring_lineno() -> None:
     src = '''
     def f():
         """
         This is a long docstring.
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_mro.py` & `pydoctor-23.4.0/pydoctor/test/test_mro.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_napoleon_docstring.py` & `pydoctor-23.4.0/pydoctor/test/test_napoleon_docstring.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_napoleon_iterators.py` & `pydoctor-23.4.0/pydoctor/test/test_napoleon_iterators.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_node2stan.py` & `pydoctor-23.4.0/pydoctor/test/test_node2stan.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_options.py` & `pydoctor-23.4.0/pydoctor/test/test_options.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_packages.py` & `pydoctor-23.4.0/pydoctor/test/test_packages.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_pydantic_fields.py` & `pydoctor-23.4.0/pydoctor/test/test_pydantic_fields.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_qnmatch.py` & `pydoctor-23.4.0/pydoctor/test/test_qnmatch.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_sphinx.py` & `pydoctor-23.4.0/pydoctor/test/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_templatewriter.py` & `pydoctor-23.4.0/pydoctor/test/test_templatewriter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from io import BytesIO
-from typing import Callable, Union, Any, cast, TYPE_CHECKING
+import re
+from typing import Callable, Union, Any, cast, Type, TYPE_CHECKING
 import pytest
 import warnings
 import sys
 import tempfile
 import os
 from pathlib import Path, PurePath
 
 from pydoctor import model, templatewriter, stanutils, __version__, epydoc2stan
 from pydoctor.templatewriter import (FailedToCreateTemplate, StaticTemplate, pages, writer, util,
                                      TemplateLookup, Template, 
                                      HtmlTemplate, UnsupportedTemplateVersion, 
                                      OverrideTemplateNotAllowed)
 from pydoctor.templatewriter.pages.table import ChildTable
 from pydoctor.templatewriter.summary import isClassNodePrivate, isPrivate, moduleSummary
-from pydoctor.test.test_astbuilder import fromText
+from pydoctor.test.test_astbuilder import fromText, systemcls_param
 from pydoctor.test.test_packages import processPackage, testpackages
 from pydoctor.test import CapSys
 from pydoctor.themes import get_themes
 
 if TYPE_CHECKING:
     from twisted.web.template import Flattenable
 
@@ -517,26 +518,50 @@
         pass
     ''')
     assert not isClassNodePrivate(cast(model.Class, mod.contents['Public']))
     assert isClassNodePrivate(cast(model.Class, mod.contents['_Private']))
     assert not isClassNodePrivate(cast(model.Class, mod.contents['_BaseForPublic']))
     assert isClassNodePrivate(cast(model.Class, mod.contents['_BaseForPrivate']))
 
+@systemcls_param
+def test_format_function_def_overloads(systemcls: Type[model.System]) -> None:
+    mod = fromText("""
+        from typing import overload, Union
+        @overload
+        def parse(s: str) -> str:
+            ...
+        @overload
+        def parse(s: bytes) -> bytes:
+            ...
+        def parse(s: Union[str, bytes]) -> Union[str, bytes]:
+            pass
+        """, systemcls=systemcls)
+    func = mod.contents['parse']
+    assert isinstance(func, model.Function)
+    
+    # We intentionally remove spaces before comparing
+    overloads_html = stanutils.flatten_text(list(pages.format_overloads(func))).replace(' ','')
+    assert '''(s:str)->str:''' in overloads_html
+    assert '''(s:bytes)->bytes:''' in overloads_html
+
+    # Confirm the actual function definition is not rendered
+    function_def_html = stanutils.flatten_text(list(pages.format_function_def(func.name, func.is_async, func)))
+    assert function_def_html == ''
+
 def test_format_signature() -> None:
     """Test C{pages.format_signature}. 
     
     @note: This test will need to be adapted one we include annotations inside signatures.
     """
     mod = fromText(r'''
     def func(a:Union[bytes, str]=_get_func_default(str), b:Any=re.compile(r'foo|bar'), *args:str, **kwargs:Any) -> Iterator[Union[str, bytes]]:
         ...
     ''')
-    assert ("""(a=_get_func_default(<wbr></wbr>str), b=re.compile("""
-            """r<span class="rst-variable-quote">'</span>foo<span class="rst-re-op">|</span>"""
-            """bar<span class="rst-variable-quote">'</span>), *args, **kwargs)""") in flatten(pages.format_signature(cast(model.Function, mod.contents['func'])))
+    assert ("""(a:Union[bytes,str]=_get_func_default(str),b:Any=re.compile(r'foo|bar'),*args:str,**kwargs:Any)->Iterator[Union[str,bytes]]""") in \
+        stanutils.flatten_text(pages.format_signature(cast(model.Function, mod.contents['func']))).replace(' ','')
 
 def test_format_decorators() -> None:
     """Test C{pages.format_decorators}"""
     mod = fromText(r'''
     @string_decorator(set('\\/:*?"<>|\f\v\t\r\n'))
     @simple_decorator(max_examples=700, deadline=None, option=range(10))
     def func():
@@ -682,32 +707,31 @@
     mod = fromText(src_crash_xml_entities, system=system, modname='test')
     for o in mod.system.allobjects.values():
         epydoc2stan.ensure_parsed_docstring(o)
     getHTMLOf(mod)
     getHTMLOf(mod.contents['C'])
     out = capsys.readouterr().out
     warnings = '''\
-test:2: bad docstring: SAXParseException: <unknown>:2:25: undefined entity
-test:25: bad signature: SAXParseException: <unknown>:1:88: undefined entity
-test:25: bad annotation: SAXParseException: <unknown>:1:104: undefined entity
-test:17: bad rendering of decorators: SAXParseException: <unknown>:1:102: undefined entity
-test:21: bad annotation: SAXParseException: <unknown>:1:104: undefined entity
-test:30: bad docstring: SAXParseException: <unknown>:1:6: undefined entity
-test:8: bad annotation: SAXParseException: <unknown>:1:104: undefined entity
-test:10: bad rendering of constant: SAXParseException: <unknown>:1:112: undefined entity
-test:14: bad docstring: SAXParseException: <unknown>:1:13: undefined entity
-test:36: bad rendering of class signature: SAXParseException: <unknown>:1:104: undefined entity
+test:2: bad docstring: SAXParseException: <unknown>.+ undefined entity
+test:25: bad signature: SAXParseException: <unknown>.+ undefined entity
+test:17: bad rendering of decorators: SAXParseException: <unknown>.+ undefined entity
+test:21: bad signature: SAXParseException: <unknown>.+ undefined entity
+test:30: bad docstring: SAXParseException: <unknown>.+ undefined entity
+test:8: bad annotation: SAXParseException: <unknown>:.+ undefined entity
+test:10: bad rendering of constant: SAXParseException: <unknown>.+ undefined entity
+test:14: bad docstring: SAXParseException: <unknown>.+ undefined entity
+test:36: bad rendering of class signature: SAXParseException: <unknown>.+ undefined entity
 '''.splitlines()
     
     # Some how the type processing get rid of the non breaking spaces, but it's more an implementation
     # detail rather than a fix for the bug.
     if processtypes is True:
-        warnings.remove('test:30: bad docstring: SAXParseException: <unknown>:1:6: undefined entity')
+        warnings.remove('test:30: bad docstring: SAXParseException: <unknown>.+ undefined entity')
     
-    assert out == '\n'.join(warnings)+'\n'
+    assert re.match('\n'.join(warnings), out)
 
 @pytest.mark.parametrize('processtypes', [True, False])
 def test_crash_xmlstring_entities_rst(capsys:CapSys, processtypes:bool) -> None:
     """Idem for RST"""
     system = model.System()
     system.options.verbosity = -1
     system.options.processtypes=processtypes
@@ -715,25 +739,37 @@
     mod = fromText(src_crash_xml_entities.replace('@type', ':type').replace('@rtype', ':rtype').replace('==', "--"), modname='test', system=system)
     for o in mod.system.allobjects.values():
         epydoc2stan.ensure_parsed_docstring(o)
     getHTMLOf(mod)
     getHTMLOf(mod.contents['C'])
     out = capsys.readouterr().out
     warn_str = '''\
-test:2: bad docstring: SAXParseException: <unknown>:1:13: undefined entity
-test:25: bad signature: SAXParseException: <unknown>:1:88: undefined entity
-test:25: bad annotation: SAXParseException: <unknown>:1:104: undefined entity
-test:17: bad rendering of decorators: SAXParseException: <unknown>:1:102: undefined entity
-test:21: bad annotation: SAXParseException: <unknown>:1:104: undefined entity
-test:30: bad docstring: SAXParseException: <unknown>:1:6: undefined entity
-test:8: bad annotation: SAXParseException: <unknown>:1:104: undefined entity
-test:10: bad rendering of constant: SAXParseException: <unknown>:1:112: undefined entity
-test:14: bad docstring: SAXParseException: <unknown>:1:13: undefined entity
-test:36: bad rendering of class signature: SAXParseException: <unknown>:1:104: undefined entity
+test:2: bad docstring: SAXParseException: <unknown>.+ undefined entity
+test:25: bad signature: SAXParseException: <unknown>.+ undefined entity
+test:17: bad rendering of decorators: SAXParseException: <unknown>.+ undefined entity
+test:21: bad signature: SAXParseException: <unknown>.+ undefined entity
+test:30: bad docstring: SAXParseException: <unknown>.+ undefined entity
+test:8: bad annotation: SAXParseException: <unknown>.+ undefined entity
+test:10: bad rendering of constant: SAXParseException: <unknown>.+ undefined entity
+test:14: bad docstring: SAXParseException: <unknown>.+ undefined entity
+test:36: bad rendering of class signature: SAXParseException: <unknown>.+ undefined entity
 '''
     warnings = warn_str.splitlines()
 
     if processtypes is True:
-        warnings.remove('test:30: bad docstring: SAXParseException: <unknown>:1:6: undefined entity')
+        warnings.remove('test:30: bad docstring: SAXParseException: <unknown>.+ undefined entity')
     
-    assert out == '\n'.join(warnings)+'\n'
+    assert re.match('\n'.join(warnings), out)
+
+def test_constructor_renders(capsys:CapSys) -> None:
+    ...
+    src = '''\
+    class Animal(object):
+        # pydoctor can infer the constructor to be: "Animal(name)"
+        def __new__(cls, name):
+            ...
+    '''
 
+    mod = fromText(src)
+    html = getHTMLOf(mod.contents['Animal'])
+    assert 'Constructor: ' in html
+    assert 'Animal(name)' in html
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_twisted_python_deprecate.py` & `pydoctor-23.4.0/pydoctor/test/test_twisted_python_deprecate.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         name='_bar', package='Twisted', version=r'16\.0\.0'
     ), mod_html_text, re.DOTALL), mod_html_text
 
     _class = mod.contents['Baz']
     assert len(_class.extra_info)==1
     assert re.match(_html_template_with_replacement.format(
         name='Baz', package='Twisted', version=r'14\.2\.3', replacement='stuff'
-    ), flatten_text(_class.extra_info[0].to_stan(mod.docstring_linker, False)).strip(), re.DOTALL)
+    ), flatten_text(_class.extra_info[0].to_stan(mod.docstring_linker)).strip(), re.DOTALL)
 
     assert re.match(_html_template_with_replacement.format(
         name='Baz', package='Twisted', version=r'14\.2\.3', replacement='stuff'
     ), class_html_text, re.DOTALL), class_html_text
 
     assert re.match(_html_template_with_replacement.format(
         name='foom', package='Twisted', version=r'NEXT', replacement='faam'
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_type_fields.py` & `pydoctor-23.4.0/pydoctor/test/test_type_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pydoctor.test import NotFoundLinker, CapSys
 from pydoctor.test.epydoc import parse_docstring
 from pydoctor.test.test_epydoc2stan import docstring2html
 from pydoctor.test.test_astbuilder import fromText
 from pydoctor.stanutils import flatten
 from pydoctor.napoleon.docstring import TokenType
 from pydoctor.epydoc.markup._types import ParsedTypeDocstring
+import pydoctor.epydoc.markup
 from pydoctor import model
 from twisted.web.template import Tag
 
 
 def doc2html(doc: str, markup: str, processtypes: bool = False) -> str:
     return ''.join(prettify(flatten(parse_docstring(doc, markup, processtypes).to_stan(NotFoundLinker()))).splitlines())
 
@@ -53,15 +54,15 @@
     for tokens_types, expected_token_types in convert_obj_tokens_cases:
 
         assert str(ann._convert_obj_tokens_to_stan(tokens_types, NotFoundLinker()))==str(expected_token_types)
 
 
 def typespec2htmlvianode(s: str, markup: str) -> str:
     err: List[ParseError] = []
-    parsed_doc = get_parser_by_name(markup)(s, err, False)
+    parsed_doc = get_parser_by_name(markup)(s, err)
     assert not err
     ann = ParsedTypeDocstring(parsed_doc.to_node(), warns_on_unknown_tokens=True)
     html = flatten(ann.to_stan(NotFoundLinker()))
     assert not ann.warnings
     return html
 
 def typespec2htmlviastr(s: str) -> str:
@@ -309,24 +310,24 @@
         >>> print('example')
     """
 
     expected = """<code>complicated string</code> or <code>strIO</code>, <em>optional</em>"""
     
     # Test epytext
     epy_errors: List[ParseError] = []
-    epy_parsed = get_parser_by_name('epytext')(epy_string, epy_errors, True)
+    epy_parsed = pydoctor.epydoc.markup.processtypes(get_parser_by_name('epytext'))(epy_string, epy_errors)
 
     assert len(epy_errors)==1
     assert "Unexpected element in type specification field: element 'doctest_block'" in epy_errors.pop().descr()
 
     assert flatten(epy_parsed.fields[-1].body().to_stan(NotFoundLinker())).replace('\n', '') == expected
     
     # Test restructuredtext
     rst_errors: List[ParseError] = []
-    rst_parsed = get_parser_by_name('restructuredtext')(rst_string, rst_errors, True)
+    rst_parsed = pydoctor.epydoc.markup.processtypes(get_parser_by_name('restructuredtext'))(rst_string, rst_errors)
 
     assert len(rst_errors)==1
     assert "Unexpected element in type specification field: element 'doctest_block'" in rst_errors.pop().descr()
 
     assert flatten(rst_parsed.fields[-1].body().to_stan(NotFoundLinker())).replace('\n', ' ') == expected
 
 def test_napoleon_types_warnings(capsys: CapSys) -> None:
```

### Comparing `pydoctor-22.9.1/pydoctor/test/test_utils.py` & `pydoctor-23.4.0/pydoctor/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_visitor.py` & `pydoctor-23.4.0/pydoctor/test/test_visitor.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/test_zopeinterface.py` & `pydoctor-23.4.0/pydoctor/test/test_zopeinterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from typing import Type, cast
+from typing import Any, Dict, Iterable, List, Type, cast
 from pydoctor.test.test_astbuilder import fromText, type2html, ZopeInterfaceSystem
 from pydoctor.test.test_packages import processPackage
 from pydoctor.test.test_templatewriter import getHTMLOf
 from pydoctor.extensions.zopeinterface import ZopeInterfaceClass
 from pydoctor.epydoc.markup import ParsedDocstring
 from pydoctor import model
 from pydoctor.stanutils import flatten
@@ -554,12 +554,63 @@
     
     assert 'Known implementations:' in ifoo_html
     assert 'zi.Foo' in ifoo_html
 
     assert 'Implements interfaces:' in foo_html
     assert 'zi.IFoo' in foo_html
 
+
+def _get_modules_test_zope_interface_imports_cycle_proof() -> List[Iterable[Dict[str, Any]]]:
+    src_inteface = '''\
+    from zope.interface import Interface
+    from top.impl import Address
+
+    class IAddress(Interface):
+        ...
+    '''
+
+    src_impl = '''\
+    from zope.interface import implementer
+    from top.interface import IAddress
+    
+    @implementer(IAddress)
+    class Address(object):
+        ...  
+    '''
+
+    mod_interface = {'modname': 'interface', 'text': src_inteface, 'parent_name':'top'}
+    mod_top = {'modname':'top', 'text': 'pass', 'is_package': True}
+    mod_impl = {'modname': 'impl', 'text': src_impl, 'parent_name':'top'}
+
+    return [
+        (mod_top,mod_interface,mod_impl),
+        (mod_top,mod_impl,mod_interface),
+        ]
+
+@pytest.mark.parametrize('modules', _get_modules_test_zope_interface_imports_cycle_proof())
+@zope_interface_systemcls_param
+def test_zope_interface_imports_cycle_proof(systemcls: Type[model.System], modules:Iterable[Dict[str, Any]]) -> None:
+    """
+    Zope interface informations is collected no matter the cyclics imports and the order of processing of modules.
+    This test only check some basic cyclic imports examples.
+    """
+    system = systemcls()
+    builder = system.systemBuilder(system)
+    for m in modules:
+        builder.addModuleString(**m)
     
+    builder.buildModules()
+
+    interface = system.objForFullName('top.interface.IAddress')
+    impl = system.objForFullName('top.impl.Address')
 
+    assert isinstance(interface, model.Class)
+    assert isinstance(impl, model.Class)
+
+    ihtml = getHTMLOf(interface)
+    html = getHTMLOf(impl)
+    
+    assert 'top.impl.Address' in ihtml
+    assert 'top.interface.IAddress' in html
```

### Comparing `pydoctor-22.9.1/pydoctor/test/testcustomtemplates/allok/nav.html` & `pydoctor-23.4.0/pydoctor/test/testcustomtemplates/allok/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/testcustomtemplates/faketemplate/nav.html` & `pydoctor-23.4.0/pydoctor/test/testcustomtemplates/faketemplate/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/testpackages/basic/mod.py` & `pydoctor-23.4.0/pydoctor/test/testpackages/basic/mod.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c` & `pydoctor-23.4.0/pydoctor/test/testpackages/c_module_invalid_text_signature/mymod/base.c`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c` & `pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.c`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py` & `pydoctor-23.4.0/pydoctor/test/testpackages/c_module_python_module_name_clash/mymod/base.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/test/testpackages/multipleinheritance/mod.py` & `pydoctor-23.4.0/pydoctor/test/testpackages/multipleinheritance/mod.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/__init__.py` & `pydoctor-23.4.0/pydoctor/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/ajax.js` & `pydoctor-23.4.0/pydoctor/themes/base/ajax.js`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/all-documents.html` & `pydoctor-23.4.0/pydoctor/themes/base/all-documents.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/apidocs.css` & `pydoctor-23.4.0/pydoctor/themes/base/apidocs.css`

 * *Files 1% similar despite different names*

```diff
@@ -390,14 +390,23 @@
 
 .functionBody > .undocumented {
 
     margin-top: 6px;
     margin-bottom: 6px;
 }
 
+/* Use a slightly more compact presentation for signatures */
+.function-signature {
+    word-spacing: -5px;
+}
+
+.function-signature code {
+    padding: 2px 1px;
+}
+
 /*
 - Links to class/function/etc names are nested like this:
     <code><a>label</a></code>
   
 - 'functionHeader' is used for lines like `def func():` and `var =`
 */
 code, .literal, .pre, #childList > div .functionHeader,
```

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/attribute-child.html` & `pydoctor-23.4.0/pydoctor/themes/base/attribute-child.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/common.html` & `pydoctor-23.4.0/pydoctor/themes/base/common.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/footer.html` & `pydoctor-23.4.0/pydoctor/themes/base/footer.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/function-child.html` & `pydoctor-23.4.0/pydoctor/themes/base/function-child.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 <div xmlns:t="http://twistedmatrix.com/ns/twisted.web.template/0.1">
-  <meta name="pydoctor-template-version" content="3" />
+  <meta name="pydoctor-template-version" content="4" />
   <t:attr name="class" t:render="class_" />
   <a>
     <t:attr name="name" t:render="functionAnchor" />
   </a>
   <a>
     <t:attr name="name" t:render="shortFunctionAnchor" />
   </a>
   <div class="functionHeader">
+    <t:transparent t:render="overloads" />
     <t:transparent t:render="decorator" />
     <t:transparent t:render="functionDef">
       def functionName():
     </t:transparent>
     <a class="sourceLink" t:render="sourceLink">
       <t:attr name="href"><t:slot name="sourceHref" /></t:attr>
       (source)
```

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/head.html` & `pydoctor-23.4.0/pydoctor/themes/base/head.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/index.html` & `pydoctor-23.4.0/pydoctor/themes/base/index.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/lunr.js` & `pydoctor-23.4.0/pydoctor/themes/base/lunr.js`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/nameIndex.html` & `pydoctor-23.4.0/pydoctor/themes/base/nameIndex.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/nav.html` & `pydoctor-23.4.0/pydoctor/themes/base/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/pydoctor.js` & `pydoctor-23.4.0/pydoctor/themes/base/pydoctor.js`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/search.js` & `pydoctor-23.4.0/pydoctor/themes/base/search.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -161,18 +161,19 @@
         document.getElementById('search-clear-button').style.display = 'none';
     }
 }
 
 //////// SEARCH WARPPER FUNCTIONS /////////
 
 // Values configuring the search-as-you-type feature.
-const SEARCH_DEFAULT_DELAY = 100; // in miliseconds
-const SEARCH_INCREASED_DELAY = 200;
-const SEARCH_INDEX_SIZE_TRESH_INCREASE_DELAY = 10; // in MB
-const SEARCH_INDEX_SIZE_TRESH_DISABLE_SEARCH_AS_YOU_TYPE = 20;
+var SEARCH_DEFAULT_DELAY = 100; // in miliseconds
+var SEARCH_INCREASED_DELAY = 200;
+var SEARCH_INDEX_SIZE_TRESH_INCREASE_DELAY = 10; // in MB
+var SEARCH_INDEX_SIZE_TRESH_DISABLE_SEARCH_AS_YOU_TYPE = 20;
+var SEARCH_AUTO_WILDCARD = true;
 
 // Search delay depends on index size.
 function _getIndexSizePromise(indexURL) {
     return httpGetPromise(indexURL).then((responseText) => {
         if (responseText == null) {
             return 0;
         }
@@ -285,15 +286,15 @@
 
     // Get search delay, wait the all search resources to be cached and actually launch the search 
     return _getSearchDelayPromise(indexURL).then((searchDelay) => {
         if (isSearchReadyPromise == null) {
             isSearchReadyPromise = _getIsSearchReadyPromise()
         }
         return isSearchReadyPromise.then((r) => {
-            return lunrSearch(_query, indexURL, _fields, "lunr.js", !noDelay ? searchDelay : 0).then((lunrResults) => {
+            return lunrSearch(_query, indexURL, _fields, "lunr.js", !noDelay ? searchDelay : 0, SEARCH_AUTO_WILDCARD).then((lunrResults) => {
 
                 // outdated query results
                 if (_searchStartTime != _lastSearchStartTime) {
                     return;
                 }
 
                 if (!lunrResults) {
@@ -352,24 +353,16 @@
  */
 function displaySearchResults(_query, documentResults, lunrResults) {
     resetResultList();
     documentResults.forEach((dobj) => {
         results_list.appendChild(buildSearchResult(dobj));
     });
 
-    if (lunrResults[0].score <= 5) {
-        if (lunrResults.length > 500) {
-            setWarning("Your search yielded a lot of results! and there aren't many great matches. Maybe try with other terms?");
-        } else {
-            setWarning("Unfortunately, it looks like there aren't many great matches for your search. Maybe try with other terms?");
-        }
-    } else {
-        if (lunrResults.length > 500) {
-            setWarning("Your search yielded a lot of results! Maybe try with other terms?");
-        }
+    if (lunrResults.length > 500) {
+        setWarning("Your search yielded a lot of results! Maybe try with other terms?");
     }
 
     let publicResults = documentResults.filter(function(value) {
         return !value.querySelector('.privacy').innerHTML.includes("PRIVATE");
     })
 
     if (publicResults.length == 0) {
```

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/searchlib.js` & `pydoctor-23.4.0/pydoctor/themes/base/searchlib.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -10,46 +10,75 @@
 // old promise will never resolves and the searhc worker will be restarted.
 
 // Hacky way to make the worker code inline with the rest of the source file handling the search.
 // Worker message params are the following: 
 // - query: string
 // - indexJSONData: dict
 // - defaultFields: list of strings
+// - autoWildcard: boolean
 let _lunrWorkerCode = `
 
 // The lunr.js code will be inserted here.
 
 onmessage = (message) => {
     if (!message.data.query) {
         throw new Error('No search query provided.');
     }
     if (!message.data.indexJSONData) {
         throw new Error('No index data provided.');
     }
     if (!message.data.defaultFields) {
         throw new Error('No default fields provided.');
     }
+    if (!message.data.hasOwnProperty('autoWildcard')){
+        throw new Error('No value for auto wildcard provided.');
+    }
     // Create index
     let index = lunr.Index.load(message.data.indexJSONData);
     
     // Declare query function building 
     function _queryfn(_query){ // _query is the Query object
         // Edit the parsed query clauses that are applicable for all fields (default) in order
         // to remove the field 'kind' from the clause since this it's only useful when specifically requested.
         var parser = new lunr.QueryParser(message.data.query, _query)
         parser.parse()
+        var hasTraillingWildcard = false;
         _query.clauses.forEach(clause => {
             if (clause.fields == _query.allFields){
                 // we change the query fields when they are applicable to all fields
                 // to a list of predefined fields because we might include additional filters (like kind:)
                 // which should not be matched by default.
                 clause.fields = message.data.defaultFields;
             }
-            // TODO: If fuzzy match is greater than 20 throw an error.
+            // clause.wildcard is actually always NONE due to https://github.com/olivernn/lunr.js/issues/495
+            // But this works...
+            if (clause.term.slice(-1) == '*'){
+                // we want to avoid the auto wildcard system only if a trailling wildcard is already added
+                // not if a leading wildcard exists
+                hasTraillingWildcard = true
+            }
+        });
+        // Auto wilcard feature, see issue https://github.com/twisted/pydoctor/issues/648
+        var new_clauses = [];
+        if ((message.data.autoWildcard == true) && (hasTraillingWildcard == false)){
+            _query.clauses.forEach(clause => {
+                // Setting clause.wildcard is useless.
+                // But this works...
+                let new_clause = {...clause}
+                new_clause.term = new_clause.term + '*'
+                clause.boost = 2
+                new_clause.boost = 0
+                new_clauses.push(new_clause)
+            });
+        }
+        new_clauses.forEach(clause => {
+            _query.clauses.push(clause)
         });
+        console.log('Parsed query:')
+        console.dir(_query.clauses)
     }
 
     // Launch the search
     let results = index.query(_queryfn)
     
     // Post message with results
     postMessage({'results':results});
@@ -144,16 +173,17 @@
  * Old promise never resolves if calling lunrSearch() again while already running.
  * @param query: Query string.
  * @param indexURL: URL pointing to the Lunr search index, generated by pydoctor.
  * @param defaultFields: List of strings: default fields to apply to query clauses when none is specified. ["name", "names", "qname"] for instance.
  * @param lunrJsURL: URL pointing to a copy of lunr.js.
  * @param searchDelay: Number of miliseconds to wait before actually launching the query. This is useful to set for "search as you type" kind of search box
  *                     because it let a chance to users to continue typing without triggering useless searches (because previous search is aborted on launching a new one).
+ * @param autoWildcard: Whether to automatically append wildcards to all query clauses when no wildcard is already specified. boolean.
  */
-function lunrSearch(query, indexURL, defaultFields, lunrJsURL, searchDelay) {
+function lunrSearch(query, indexURL, defaultFields, lunrJsURL, searchDelay, autoWildcard) {
     // Abort ongoing search
     abortSearch();
 
     // Register abort procedure.
     var _aborted = false;
     searchEventsEnv.addEventListener('abortSearch', (ev) => {
         _aborted = true;
@@ -187,15 +217,16 @@
                                 worker.onerror = function(error) {
                                     reject(error);
                                 };
                             });
                             let _msgData = {
                                 'query': query,
                                 'indexJSONData': lunrIndexData,
-                                'defaultFields': defaultFields
+                                'defaultFields': defaultFields,
+                                'autoWildcard': autoWildcard,
                             }
 
                             if (!_aborted) {
                                 console.log(`Posting query "${query}" to worker:`)
                                 console.dir(_msgData)
                                 worker.postMessage(_msgData);
                                 searchEventsEnv.dispatchEvent(
```

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/sidebar-list.html` & `pydoctor-23.4.0/pydoctor/themes/base/sidebar-list.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/sidebar.html` & `pydoctor-23.4.0/pydoctor/themes/base/sidebar.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/sidebartoggle.js` & `pydoctor-23.4.0/pydoctor/themes/base/sidebartoggle.js`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/base/summary.html` & `pydoctor-23.4.0/pydoctor/themes/base/summary.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/classic/bootstrap.min.css` & `pydoctor-23.4.0/pydoctor/themes/classic/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/classic/head.html` & `pydoctor-23.4.0/pydoctor/themes/classic/head.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/common.html` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/common.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/book.svg` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/book.svg`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/lato-bold.woff2` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/lato-normal.woff2` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/fonts/plus-square-o.svg` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/fonts/plus-square-o.svg`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/footer.html` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/footer.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/head.html` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/head.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/nav.html` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/nav.html`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor/themes/readthedocs/readthedocstheme.css` & `pydoctor-23.4.0/pydoctor/themes/readthedocs/readthedocstheme.css`

 * *Files 3% similar despite different names*

```diff
@@ -60,58 +60,58 @@
     margin-top: 0;
     padding: 5px 0 5px 0;
     position: relative;
 }
 
 /* xref stlyles */
 
-code > a {
-    background: rgb(255, 255, 255);
-    font-family: Menlo, Monaco, Consolas, "Courier New", monospace;
-    border: 1px solid rgb(225, 228, 229);
-    padding: 1px 2px;
-    font-size: 14px;
-}
 
 .sourceLink {
     font-size: 14px;
     border: 0;
     font-family: Menlo, Monaco, Consolas, "Courier New", monospace;
 }
 
 code, .pre, #childList > div .functionHeader,
 #splitTables > table tr td:nth-child(2), .fieldArg {
     font-family: Menlo, Monaco, Consolas, "Courier New", monospace;
 }
 
-code {
-    background: transparent;
+code, .literal {
+    border-radius:2px;
+    font-size: 14px;
+}
+
+#main code, .literal {
+    border: 1px solid rgb(225, 228, 229);
+    padding:1px 2px;
+}
+
+/* special cases where pydoctor's default theme renders ok with the background,
+but doesn't render nicely with this theme. */
+.class-signature > code, h1 > code, pre code{
+    background-color: transparent;
+    border: none !important;
 }
 
 /* Header */ 
 
-.page-header > h1 {
+h1 {
     margin-top: 15px;
     font-size: 28px;
 }
 
-.page-header > h1 code {
-    padding: 0;
-    font-size: 16px;
+h1 code {
+    font-size: 20px;
 }
 
-.page-header > h1 > code {
-    display: block;
+h1 > code {
     line-height: 1.6;
 }
 
-.page-header > h1 code > a {
-    font-size: 18px;
-}
-
 /* Titles */
 
 p.caption, h1, h2, h3, h4, h5, h6, legend, .categoryHeader, #search-status{
 
     font-weight: bold;
     font-family: "Roboto Slab",Georgia,Arial,sans-serif;
 }
@@ -243,14 +243,15 @@
 
 #childList > div .functionHeader {
     background: rgb(240, 240, 240);
     border-left: 3px solid rgb(204, 204, 204);
     border-width: 0px 0px 0px 3px;
     margin: 0px 0px 6px;
     padding: 6px;
+    font-size: 15px;
 }
 
 .functionBody{
     margin-left: 30px;
 }
 
 /* Class definition block */
```

### Comparing `pydoctor-22.9.1/pydoctor/utils.py` & `pydoctor-23.4.0/pydoctor/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def findClassFromDottedName(
         dottedname: str,
         optionname: str,
         base_class: Union[str, Type[T]]
         ) -> Type[T]:
     """
     Looks up a class by full name.
-    
+
     @raises ValueError: If can't find the class.
     """
     if '.' not in dottedname:
         raise ValueError(f"{optionname} takes a dotted name")
     parts = dottedname.rsplit('.', 1)
     try:
         mod = __import__(parts[0], globals(), locals(), parts[1])
@@ -92,14 +92,12 @@
     else:
         return (priv, parts[1].strip())
 
 def partialclass(cls: Type[Any], *args: Any, **kwds: Any) -> Type[Any]:
     """
     Bind a class to be created with some predefined __init__ arguments.
     """
-    # mypy gets errors: - Variable "cls" is not valid as a type
-    #                   - Invalid base class "cls" 
-    class NewPartialCls(cls): #type: ignore
+    class NewPartialCls(cls):
         __init__ = functools.partialmethod(cls.__init__, *args, **kwds) #type: ignore
         __class__ = cls
     assert isinstance(NewPartialCls, type)
     return NewPartialCls
```

### Comparing `pydoctor-22.9.1/pydoctor/visitor.py` & `pydoctor-23.4.0/pydoctor/visitor.py`

 * *Files identical despite different names*

### Comparing `pydoctor-22.9.1/pydoctor.egg-info/PKG-INFO` & `pydoctor-23.4.0/pydoctor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoctor
-Version: 22.9.1
+Version: 23.4.0
 Summary: API doc generator.
 Home-page: https://github.com/twisted/pydoctor
 Author: Michael Hudson-Doyle
 Author-email: micahel@gmail.com
 Maintainer: Maarten ter Huurne
 Maintainer-email: maarten@boxingbeetle.com
 License: MIT/X11
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
@@ -34,16 +35,16 @@
 
 pydoctor
 --------
 
 .. image:: https://img.shields.io/pypi/pyversions/pydoctor.svg
   :target: https://pypi.python.org/pypi/pydoctor
 
-.. image:: https://travis-ci.org/twisted/pydoctor.svg?branch=tox-travis-2
-  :target: https://travis-ci.org/twisted/pydoctor
+.. image:: https://github.com/twisted/pydoctor/actions/workflows/unit.yaml/badge.svg
+  :target: https://github.com/twisted/pydoctor/actions/workflows/unit.yaml
 
 .. image:: https://codecov.io/gh/twisted/pydoctor/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/twisted/pydoctor
 
 .. image:: https://img.shields.io/badge/-documentation-blue
   :target: https://pydoctor.readthedocs.io/
 
@@ -103,16 +104,35 @@
 __ https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard
 
 You can select a different format using the ``--docformat`` option or the ``__docformat__`` module variable. 
 
 What's New?
 ~~~~~~~~~~~
 
-in development
-^^^^^^^^^^^^^^
+pydoctor 23.4.0
+^^^^^^^^^^^^^^^
+
+* Add support for Python 3.11
+* Add support for the ``@overload`` decorator.
+* Show type annotations in function's signatures.
+* If none of a function's parameters have documentation, do not render the parameter table.
+* Themes have been adjusted to render annotations more concisely.
+* Fix a rare crash in the type inference. 
+  Invalid python code like a set of lists would raise a uncaught TypeError in the evaluation.
+* Support when source path lies outside base directory (``--project-base-dir``).
+  Since pydoctor support generating docs for multiple packages, 
+  it is not certain that all of the source is even viewable below a single URL. 
+  We now allow to add arbitrary paths to the system, 
+  but only the objects inside a module wich path is relative to
+  the base directory can have a source control link generated.
+* Cache the default docutils settings on docutils>=0.19 to improve performance.
+* Improve the search bar user experience by automatically appending wildcard to each query terms
+  when no terms already contain a wildcard. 
+* Link recognized constructors in class page.
+* An invalid epytext docstring will be rederered as plaintext, just like invalid restructuredtext docstrings (finally).
 
 pydoctor 22.9.1
 ^^^^^^^^^^^^^^^
 * ``pydoctor --help`` works again.
 
 pydoctor 22.9.0
 ^^^^^^^^^^^^^^^
```

### Comparing `pydoctor-22.9.1/pydoctor.egg-info/SOURCES.txt` & `pydoctor-23.4.0/pydoctor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 docs/source/custom_template_demo/index.rst
 docs/source/custom_template_demo/pyproject.toml
 docs/source/docformat/epytext.rst
 docs/source/docformat/google-numpy.rst
 docs/source/docformat/index.rst
 docs/source/docformat/list-restructuredtext-support.rst
 docs/source/docformat/restructuredtext.rst
-docs/source/docformat/epytext/epytext_demo.rst
-docs/source/docformat/google/google_demo.rst
-docs/source/docformat/numpy/numpy_demo.rst
-docs/source/docformat/restructuredtext/restructuredtext_demo.rst
+docs/source/docformat/epytext_demo/index.rst
+docs/source/docformat/google_demo/index.rst
+docs/source/docformat/numpy_demo/index.rst
+docs/source/docformat/restructuredtext_demo/index.rst
 docs/tests/__init__.py
 docs/tests/test-search.html
 docs/tests/test.py
 docs/tests/test_python_igraph_docs.py
 docs/tests/test_standard_library_docs.py
 docs/tests/test_twisted_docs.py
 pydoctor/__init__.py
@@ -69,14 +69,15 @@
 pydoctor.egg-info/dependency_links.txt
 pydoctor.egg-info/entry_points.txt
 pydoctor.egg-info/requires.txt
 pydoctor.egg-info/top_level.txt
 pydoctor/epydoc/__init__.py
 pydoctor/epydoc/doctest.py
 pydoctor/epydoc/docutils.py
+pydoctor/epydoc/sre_constants36.py
 pydoctor/epydoc/sre_parse36.py
 pydoctor/epydoc/markup/__init__.py
 pydoctor/epydoc/markup/_napoleon.py
 pydoctor/epydoc/markup/_pyval_repr.py
 pydoctor/epydoc/markup/_types.py
 pydoctor/epydoc/markup/epytext.py
 pydoctor/epydoc/markup/google.py
```

### Comparing `pydoctor-22.9.1/setup.cfg` & `pydoctor-23.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoctor
-version = 22.9.1
+version = 23.4.0
 author = Michael Hudson-Doyle
 author_email = micahel@gmail.com
 maintainer = Maarten ter Huurne
 maintainer_email = maarten@boxingbeetle.com
 description = API doc generator.
 long_description_content_type = text/x-rst
 license = MIT/X11
@@ -20,14 +20,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Documentation
 	Topic :: Software Development :: Documentation
 
 [options]
 packages = find:
```

