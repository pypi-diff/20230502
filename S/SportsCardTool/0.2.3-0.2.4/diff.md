# Comparing `tmp/SportsCardTool-0.2.3.tar.gz` & `tmp/SportsCardTool-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SportsCardTool-0.2.3.tar", last modified: Tue Apr  4 22:24:08 2023, max compression
+gzip compressed data, was "SportsCardTool-0.2.4.tar", last modified: Tue May  2 20:48:27 2023, max compression
```

## Comparing `SportsCardTool-0.2.3.tar` & `SportsCardTool-0.2.4.tar`

### file list

```diff
@@ -1,114 +1,40 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.685140 SportsCardTool-0.2.3/
--rw-r--r--   0 travis    (1000) travis    (1000)      408 2023-04-04 22:23:47.000000 SportsCardTool-0.2.3/.bumpversion.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     4233 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 travis    (1000) travis    (1000)    11357 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/LICENSE
--rw-r--r--   0 travis    (1000) travis    (1000)      800 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     2272 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/Makefile
--rw-r--r--   0 travis    (1000) travis    (1000)    18521 2023-04-04 22:24:08.685140 SportsCardTool-0.2.3/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     4684 2023-04-04 19:40:23.000000 SportsCardTool-0.2.3/README.md
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.605140 SportsCardTool-0.2.3/SportsCardTool/
--rw-r--r--   0 travis    (1000) travis    (1000)      352 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/SportsCardTool/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      155 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/SportsCardTool/__main__.py
--rw-r--r--   0 travis    (1000) travis    (1000)       22 2023-04-04 22:23:47.000000 SportsCardTool-0.2.3/SportsCardTool/_version.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4152 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/SportsCardTool/bref_tool.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.605140 SportsCardTool-0.2.3/SportsCardTool/data/
--rw-r--r--   0 travis    (1000) travis    (1000)  4644780 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/SportsCardTool/data/bref_data.json
--rw-r--r--   0 travis    (1000) travis    (1000)    10043 2023-04-04 22:23:47.000000 SportsCardTool-0.2.3/SportsCardTool/scraping_tool.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3296 2023-04-04 19:40:23.000000 SportsCardTool-0.2.3/SportsCardTool/searching_tool.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.655140 SportsCardTool-0.2.3/SportsCardTool/tests/
--rw-r--r--   0 travis    (1000) travis    (1000)     3680 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/SportsCardTool/tests/test_all.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.605140 SportsCardTool-0.2.3/SportsCardTool.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)    18521 2023-04-04 22:24:08.000000 SportsCardTool-0.2.3/SportsCardTool.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     2938 2023-04-04 22:24:08.000000 SportsCardTool-0.2.3/SportsCardTool.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-04 22:24:08.000000 SportsCardTool-0.2.3/SportsCardTool.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      177 2023-04-04 22:24:08.000000 SportsCardTool-0.2.3/SportsCardTool.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       15 2023-04-04 22:24:08.000000 SportsCardTool-0.2.3/SportsCardTool.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.655140 SportsCardTool-0.2.3/docs/
--rw-r--r--   0 travis    (1000) travis    (1000)      634 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/Makefile
--rw-r--r--   0 travis    (1000) travis    (1000)      585 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/SportsCardTool.rst
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.595140 SportsCardTool-0.2.3/docs/_build/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.655140 SportsCardTool-0.2.3/docs/_build/doctrees/
--rw-r--r--   0 travis    (1000) travis    (1000)    81330 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/doctrees/SportsCardTool.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)   152382 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 travis    (1000) travis    (1000)     5000 2023-03-31 02:49:47.000000 SportsCardTool-0.2.3/docs/_build/doctrees/index.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)    10173 2023-03-31 02:59:03.000000 SportsCardTool-0.2.3/docs/_build/doctrees/install.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)     2706 2023-03-31 02:42:22.000000 SportsCardTool-0.2.3/docs/_build/doctrees/modules.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)     2361 2023-03-31 02:30:41.000000 SportsCardTool-0.2.3/docs/_build/doctrees/setup.doctree
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.665140 SportsCardTool-0.2.3/docs/_build/html/
--rw-r--r--   0 travis    (1000) travis    (1000)      230 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/.buildinfo
--rw-r--r--   0 travis    (1000) travis    (1000)    28238 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/SportsCardTool.html
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.665140 SportsCardTool-0.2.3/docs/_build/html/_sources/
--rw-r--r--   0 travis    (1000) travis    (1000)      585 2023-03-31 02:36:31.000000 SportsCardTool-0.2.3/docs/_build/html/_sources/SportsCardTool.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      484 2023-03-31 02:49:38.000000 SportsCardTool-0.2.3/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     3774 2023-03-31 02:58:56.000000 SportsCardTool-0.2.3/docs/_build/html/_sources/install.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       79 2023-03-31 02:37:58.000000 SportsCardTool-0.2.3/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      103 2023-03-31 02:25:27.000000 SportsCardTool-0.2.3/docs/_build/html/_sources/setup.rst.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.665140 SportsCardTool-0.2.3/docs/_build/html/_static/
--rw-r--r--   0 travis    (1000) travis    (1000)    11230 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 travis    (1000) travis    (1000)    14813 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/_static/basic.css
--rw-r--r--   0 travis    (1000) travis    (1000)       42 2023-03-31 02:20:26.000000 SportsCardTool-0.2.3/docs/_build/html/_static/custom.css
--rw-r--r--   0 travis    (1000) travis    (1000)     4472 2023-03-31 02:20:27.000000 SportsCardTool-0.2.3/docs/_build/html/_static/doctools.js
--rw-r--r--   0 travis    (1000) travis    (1000)      420 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 travis    (1000) travis    (1000)      286 2023-03-31 02:20:27.000000 SportsCardTool-0.2.3/docs/_build/html/_static/file.png
--rw-r--r--   0 travis    (1000) travis    (1000)     4758 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/_static/language_data.js
--rw-r--r--   0 travis    (1000) travis    (1000)       90 2023-03-31 02:20:27.000000 SportsCardTool-0.2.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 travis    (1000) travis    (1000)       90 2023-03-31 02:20:27.000000 SportsCardTool-0.2.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 travis    (1000) travis    (1000)     5327 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/_static/pygments.css
--rw-r--r--   0 travis    (1000) travis    (1000)    18215 2023-03-31 02:20:27.000000 SportsCardTool-0.2.3/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 travis    (1000) travis    (1000)     4712 2023-03-31 02:20:27.000000 SportsCardTool-0.2.3/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 travis    (1000) travis    (1000)     7826 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/genindex.html
--rw-r--r--   0 travis    (1000) travis    (1000)     4374 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/index.html
--rw-r--r--   0 travis    (1000) travis    (1000)    21242 2023-03-31 02:59:03.000000 SportsCardTool-0.2.3/docs/_build/html/install.html
--rw-r--r--   0 travis    (1000) travis    (1000)     7609 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/modules.html
--rw-r--r--   0 travis    (1000) travis    (1000)      522 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/objects.inv
--rw-r--r--   0 travis    (1000) travis    (1000)     3873 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/py-modindex.html
--rw-r--r--   0 travis    (1000) travis    (1000)     2923 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/search.html
--rw-r--r--   0 travis    (1000) travis    (1000)    10049 2023-03-31 09:38:47.000000 SportsCardTool-0.2.3/docs/_build/html/searchindex.js
--rw-r--r--   0 travis    (1000) travis    (1000)     3334 2023-03-31 02:30:41.000000 SportsCardTool-0.2.3/docs/_build/html/setup.html
--rw-r--r--   0 travis    (1000) travis    (1000)     1053 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/conf.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.675140 SportsCardTool-0.2.3/docs/html/
--rw-r--r--   0 travis    (1000) travis    (1000)      230 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/.buildinfo
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.675140 SportsCardTool-0.2.3/docs/html/.doctrees/
--rw-r--r--   0 travis    (1000) travis    (1000)    81330 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/.doctrees/SportsCardTool.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)   152373 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/.doctrees/environment.pickle
--rw-r--r--   0 travis    (1000) travis    (1000)     5000 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/.doctrees/index.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)    10173 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/.doctrees/install.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)     2706 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/.doctrees/modules.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)     2361 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/.doctrees/setup.doctree
--rw-r--r--   0 travis    (1000) travis    (1000)    28238 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/SportsCardTool.html
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.675140 SportsCardTool-0.2.3/docs/html/_sources/
--rw-r--r--   0 travis    (1000) travis    (1000)      585 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_sources/SportsCardTool.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      484 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_sources/index.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     3774 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_sources/install.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       79 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_sources/modules.rst.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      103 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_sources/setup.rst.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-04 22:24:08.685140 SportsCardTool-0.2.3/docs/html/_static/
--rw-r--r--   0 travis    (1000) travis    (1000)    11230 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/alabaster.css
--rw-r--r--   0 travis    (1000) travis    (1000)    14813 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/basic.css
--rw-r--r--   0 travis    (1000) travis    (1000)       42 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/custom.css
--rw-r--r--   0 travis    (1000) travis    (1000)     4472 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/doctools.js
--rw-r--r--   0 travis    (1000) travis    (1000)      420 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/documentation_options.js
--rw-r--r--   0 travis    (1000) travis    (1000)      286 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/file.png
--rw-r--r--   0 travis    (1000) travis    (1000)     4758 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/language_data.js
--rw-r--r--   0 travis    (1000) travis    (1000)       90 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/minus.png
--rw-r--r--   0 travis    (1000) travis    (1000)       90 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/plus.png
--rw-r--r--   0 travis    (1000) travis    (1000)     5327 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/pygments.css
--rw-r--r--   0 travis    (1000) travis    (1000)    18215 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/searchtools.js
--rw-r--r--   0 travis    (1000) travis    (1000)     4712 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/_static/sphinx_highlight.js
--rw-r--r--   0 travis    (1000) travis    (1000)     7826 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/genindex.html
--rw-r--r--   0 travis    (1000) travis    (1000)     4374 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/index.html
--rw-r--r--   0 travis    (1000) travis    (1000)    21242 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/install.html
--rw-r--r--   0 travis    (1000) travis    (1000)     7609 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/modules.html
--rw-r--r--   0 travis    (1000) travis    (1000)      522 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/objects.inv
--rw-r--r--   0 travis    (1000) travis    (1000)     3873 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/py-modindex.html
--rw-r--r--   0 travis    (1000) travis    (1000)     2923 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/search.html
--rw-r--r--   0 travis    (1000) travis    (1000)     9558 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/searchindex.js
--rw-r--r--   0 travis    (1000) travis    (1000)     3334 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/html/setup.html
--rw-r--r--   0 travis    (1000) travis    (1000)       65 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/index.html
--rw-r--r--   0 travis    (1000) travis    (1000)      484 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/index.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     3774 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/install.rst
--rw-r--r--   0 travis    (1000) travis    (1000)      800 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/make.bat
--rw-r--r--   0 travis    (1000) travis    (1000)       79 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/docs/modules.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     2254 2023-04-04 22:23:47.000000 SportsCardTool-0.2.3/pyproject.toml
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-04 22:24:08.685140 SportsCardTool-0.2.3/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)       39 2023-04-04 19:40:11.000000 SportsCardTool-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:48:27.487358 SportsCardTool-0.2.4/
+-rw-rw-rw-   0        0        0      425 2023-05-02 20:43:01.000000 SportsCardTool-0.2.4/.bumpversion.cfg
+-rw-rw-rw-   0        0        0     4326 2023-04-01 01:10:41.000000 SportsCardTool-0.2.4/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-04-01 01:10:41.000000 SportsCardTool-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      871 2023-04-27 17:41:42.000000 SportsCardTool-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2370 2023-04-01 01:10:41.000000 SportsCardTool-0.2.4/Makefile
+-rw-rw-rw-   0        0        0    19006 2023-05-02 20:48:27.486354 SportsCardTool-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4947 2023-04-27 02:26:29.000000 SportsCardTool-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 20:48:27.247218 SportsCardTool-0.2.4/SportsCardTool/
+-rw-rw-rw-   0        0        0      636 2023-05-02 17:09:06.000000 SportsCardTool-0.2.4/SportsCardTool/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-02 20:43:09.000000 SportsCardTool-0.2.4/SportsCardTool/_version.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 17:09:06.000000 SportsCardTool-0.2.4/SportsCardTool/bref_tool.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:48:27.329826 SportsCardTool-0.2.4/SportsCardTool/data/
+-rw-rw-rw-   0        0        0  4644780 2023-05-02 20:17:16.000000 SportsCardTool-0.2.4/SportsCardTool/data/bref_data.json
+-rw-rw-rw-   0        0        0      856 2023-05-02 16:45:45.000000 SportsCardTool-0.2.4/SportsCardTool/ebay_tool.py
+-rw-rw-rw-   0        0        0    12146 2023-05-02 20:43:48.000000 SportsCardTool-0.2.4/SportsCardTool/scraping_tool.py
+-rw-rw-rw-   0        0        0     3389 2023-05-02 16:45:45.000000 SportsCardTool-0.2.4/SportsCardTool/searching_tool.py
+-rw-rw-rw-   0        0        0     2692 2023-05-02 17:09:06.000000 SportsCardTool-0.2.4/SportsCardTool/statcast_tool.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:48:27.354811 SportsCardTool-0.2.4/SportsCardTool/tests/
+-rw-rw-rw-   0        0        0     6570 2023-05-02 17:09:06.000000 SportsCardTool-0.2.4/SportsCardTool/tests/test_all.py
+-rw-rw-rw-   0        0        0    12087 2023-05-02 19:41:25.000000 SportsCardTool-0.2.4/SportsCardTool/util.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:48:27.324849 SportsCardTool-0.2.4/SportsCardTool.egg-info/
+-rw-rw-rw-   0        0        0    19006 2023-05-02 20:48:26.000000 SportsCardTool-0.2.4/SportsCardTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-05-02 20:48:27.000000 SportsCardTool-0.2.4/SportsCardTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 20:48:26.000000 SportsCardTool-0.2.4/SportsCardTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-05-02 20:48:26.000000 SportsCardTool-0.2.4/SportsCardTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 20:48:26.000000 SportsCardTool-0.2.4/SportsCardTool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 20:48:27.483353 SportsCardTool-0.2.4/docs/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:10:26.000000 SportsCardTool-0.2.4/docs/.nojekyll
+-rw-rw-rw-   0        0        0      654 2023-04-04 22:40:32.000000 SportsCardTool-0.2.4/docs/Makefile
+-rw-rw-rw-   0        0        0      614 2023-04-04 22:40:32.000000 SportsCardTool-0.2.4/docs/SportsCardTool.rst
+-rw-rw-rw-   0        0        0     1084 2023-04-27 02:26:29.000000 SportsCardTool-0.2.4/docs/conf.py
+-rw-rw-rw-   0        0        0       72 2023-05-01 23:10:26.000000 SportsCardTool-0.2.4/docs/index.html
+-rw-rw-rw-   0        0        0      507 2023-04-04 22:40:32.000000 SportsCardTool-0.2.4/docs/index.rst
+-rw-rw-rw-   0        0        0     3910 2023-04-04 22:40:32.000000 SportsCardTool-0.2.4/docs/install.rst
+-rwxrwxrwx   0        0        0      800 2023-04-04 22:40:32.000000 SportsCardTool-0.2.4/docs/make.bat
+-rw-rw-rw-   0        0        0       86 2023-04-04 22:40:32.000000 SportsCardTool-0.2.4/docs/modules.rst
+-rw-rw-rw-   0        0        0     2377 2023-05-02 20:42:55.000000 SportsCardTool-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 20:48:27.488361 SportsCardTool-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-01 01:10:41.000000 SportsCardTool-0.2.4/setup.py
```

### Comparing `SportsCardTool-0.2.3/CONTRIBUTING.md` & `SportsCardTool-0.2.4/CONTRIBUTING.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-# Contributing
-
-When contributing to this repository, please first discuss the change you wish to make via issue,
-email, or any other method with the owners of this repository before making a change. 
-
-Please note we have a code of conduct, please follow it in all your interactions with the project.
-
-## Getting Started
-
-* In order to contribute to scraping tool, collection tooling, or search tooling simply install python 3.7+ and SportsCardTool via instructions in README
-
-## Pull Request Process
-
-1. Ensure all example data or csv files are removed and to create tests for new features prior to pull request
-2. Update the README.md with details of changes to the interface, this includes new environment 
-   variables, exposed ports, useful file locations and container parameters.
-3. You may merge the Pull Request in once you have the sign-off of one other developer
-
-## Code of Conduct
-
-### Our Pledge
-
-In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
-our community a harassment-free experience for everyone, regardless of age, body
-size, disability, ethnicity, gender identity and expression, level of experience,
-nationality, personal appearance, race, religion, or sexual identity and
-orientation.
-
-### Our Standards
-
-Examples of behavior that contributes to creating a positive environment
-include:
-
-* Using welcoming and inclusive language
-* Being respectful of differing viewpoints and experiences
-* Gracefully accepting constructive criticism
-* Focusing on what is best for the community
-* Showing empathy towards other community members
-
-Examples of unacceptable behavior by participants include:
-
-* The use of sexualized language or imagery and unwelcome sexual attention or
-advances
-* Trolling, insulting/derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or electronic
-  address, without explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
-  professional setting
-
-### Our Responsibilities
-
-Project maintainers are responsible for clarifying the standards of acceptable
-behavior and are expected to take appropriate and fair corrective action in
-response to any instances of unacceptable behavior.
-
-Project maintainers have the right and responsibility to remove, edit, or
-reject comments, commits, code, wiki edits, issues, and other contributions
-that are not aligned to this Code of Conduct, or to ban temporarily or
-permanently any contributor for other behaviors that they deem inappropriate,
-threatening, offensive, or harmful.
-
-### Scope
-
-This Code of Conduct applies both within project spaces and in public spaces
-when an individual is representing the project or its community. Examples of
-representing a project or community include using an official project e-mail
-address, posting via an official social media account, or acting as an appointed
-representative at an online or offline event. Representation of a project may be
-further defined and clarified by project maintainers.
-
-### Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported by contacting the project team at [INSERT EMAIL ADDRESS]. All
-complaints will be reviewed and investigated and will result in a response that
-is deemed necessary and appropriate to the circumstances. The project team is
-obligated to maintain confidentiality with regard to the reporter of an incident.
-Further details of specific enforcement policies may be posted separately.
-
-Project maintainers who do not follow or enforce the Code of Conduct in good
-faith may face temporary or permanent repercussions as determined by other
-members of the project's leadership.
-
-### Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
-available at [http://contributor-covenant.org/version/1/4][version]
-
-[homepage]: http://contributor-covenant.org
-[version]: http://contributor-covenant.org/version/1/4/
-
+# Contributing
+
+When contributing to this repository, please first discuss the change you wish to make via issue,
+email, or any other method with the owners of this repository before making a change. 
+
+Please note we have a code of conduct, please follow it in all your interactions with the project.
+
+## Getting Started
+
+* In order to contribute to scraping tool, collection tooling, or search tooling simply install python 3.7+ and SportsCardTool via instructions in README
+
+## Pull Request Process
+
+1. Ensure all example data or csv files are removed and to create tests for new features prior to pull request
+2. Update the README.md with details of changes to the interface, this includes new environment 
+   variables, exposed ports, useful file locations and container parameters.
+3. You may merge the Pull Request in once you have the sign-off of one other developer
+
+## Code of Conduct
+
+### Our Pledge
+
+In the interest of fostering an open and welcoming environment, we as
+contributors and maintainers pledge to making participation in our project and
+our community a harassment-free experience for everyone, regardless of age, body
+size, disability, ethnicity, gender identity and expression, level of experience,
+nationality, personal appearance, race, religion, or sexual identity and
+orientation.
+
+### Our Standards
+
+Examples of behavior that contributes to creating a positive environment
+include:
+
+* Using welcoming and inclusive language
+* Being respectful of differing viewpoints and experiences
+* Gracefully accepting constructive criticism
+* Focusing on what is best for the community
+* Showing empathy towards other community members
+
+Examples of unacceptable behavior by participants include:
+
+* The use of sexualized language or imagery and unwelcome sexual attention or
+advances
+* Trolling, insulting/derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or electronic
+  address, without explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+  professional setting
+
+### Our Responsibilities
+
+Project maintainers are responsible for clarifying the standards of acceptable
+behavior and are expected to take appropriate and fair corrective action in
+response to any instances of unacceptable behavior.
+
+Project maintainers have the right and responsibility to remove, edit, or
+reject comments, commits, code, wiki edits, issues, and other contributions
+that are not aligned to this Code of Conduct, or to ban temporarily or
+permanently any contributor for other behaviors that they deem inappropriate,
+threatening, offensive, or harmful.
+
+### Scope
+
+This Code of Conduct applies both within project spaces and in public spaces
+when an individual is representing the project or its community. Examples of
+representing a project or community include using an official project e-mail
+address, posting via an official social media account, or acting as an appointed
+representative at an online or offline event. Representation of a project may be
+further defined and clarified by project maintainers.
+
+### Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behavior may be
+reported by contacting the project team at [INSERT EMAIL ADDRESS]. All
+complaints will be reviewed and investigated and will result in a response that
+is deemed necessary and appropriate to the circumstances. The project team is
+obligated to maintain confidentiality with regard to the reporter of an incident.
+Further details of specific enforcement policies may be posted separately.
+
+Project maintainers who do not follow or enforce the Code of Conduct in good
+faith may face temporary or permanent repercussions as determined by other
+members of the project's leadership.
+
+### Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
+available at [http://contributor-covenant.org/version/1/4][version]
+
+[homepage]: http://contributor-covenant.org
+[version]: http://contributor-covenant.org/version/1/4/
+
 This contributing.md was adapted from PurpleBooth on github and can be found [here](https://gist.github.com/PurpleBooth/b24679402957c63ec426)
```

### Comparing `SportsCardTool-0.2.3/LICENSE` & `SportsCardTool-0.2.4/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `SportsCardTool-0.2.3/MANIFEST.in` & `SportsCardTool-0.2.4/MANIFEST.in`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-graft SportsCardsTool
-
-include LICENSE
-include *.md
-
-include .bumpversion.cfg
-include pyproject.toml
-include Makefile
-include SportsCardTool/data/bref_data.json
-include docs/Makefile
-include .nojekyll
-
-recursive-include docs *.bat
-recursive-include docs *.buildinfo
-recursive-include docs *.css
-recursive-include docs *.doctree
-recursive-include docs *.html
-recursive-include docs *.inv
-recursive-include docs *.js
-recursive-include docs *.pickle
-recursive-include docs *.png
-recursive-include docs *.py
-recursive-include docs *.rst
-recursive-include docs *.txt
-
-prune .github
-exclude .gitignore
-exclude .gitattributes
-
-# Patterns to exclude from any directory
-global-exclude *~
-global-exclude *.pyc
-global-exclude *.pyo
-global-exclude .git
-global-exclude .ipynb_checkpoints
-global-exclude .DS_Store
+graft SportsCardsTool
+
+include LICENSE
+include *.md
+
+include .bumpversion.cfg
+include pyproject.toml
+include Makefile
+include SportsCardTool/data/bref_data.json
+include docs/Makefile
+include .nojekyll
+
+recursive-include docs *.bat
+recursive-include docs *.buildinfo
+recursive-include docs *.css
+recursive-include docs *.doctree
+recursive-include docs *.html
+recursive-include docs *.inv
+recursive-include docs *.js
+recursive-include docs *.pickle
+recursive-include docs *.png
+recursive-include docs *.py
+recursive-include docs *.rst
+recursive-include docs *.txt
+recursive-include docs *.nojekyll
+
+prune .github
+exclude .gitignore
+exclude .gitattributes
+
+# Patterns to exclude from any directory
+global-exclude *~
+global-exclude *.pyc
+global-exclude *.pyo
+global-exclude .git
+global-exclude .ipynb_checkpoints
+global-exclude .DS_Store
```

### Comparing `SportsCardTool-0.2.3/Makefile` & `SportsCardTool-0.2.4/Makefile`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-#########
-# BUILD #
-#########
-develop:  ## install dependencies and build library
-	python -m pip install -e .[develop]
-
-build:  ## build the python library
-	python setup.py build build_ext --inplace
-
-install:  ## install library
-	python -m pip install .
-
-#########
-# LINTS #
-#########
-lint:  ## run static analysis with flake8
-	python -m black --check SportsCardTool setup.py
-	python -m flake8 SportsCardTool setup.py
-
-# Alias
-lints: lint
-
-format:  ## run autoformatting with black
-	python -m black SportsCardTool/ setup.py
-
-# alias
-fix: format
-
-check:  ## check assets for packaging
-	check-manifest -v
-
-# Alias
-checks: check
-
-annotate:  ## run type checking
-	python -m mypy ./SportsCardTool
-
-#########
-# TESTS #
-#########
-test: ## clean and run unit tests
-	python -m pytest -v SportsCardTool/tests
-
-coverage:  ## clean and run unit tests with coverage
-	python -m pytest -v SportsCardTool/tests --cov=SportsCardTool --cov-branch --cov-fail-under=70 --cov-report term-missing
-
-# Alias
-tests: test
-
-###########
-# VERSION #
-###########
-show-version:
-	bump2version --dry-run --allow-dirty setup.py --list | grep current | awk -F= '{print $2}'
-
-patch:
-	bump2version patch
-
-minor:
-	bump2version minor
-
-major:
-	bump2version major
-
-########
-# DIST #
-########
-dist-build:  # Build python dist
-	python setup.py sdist bdist_wheel
-
-dist-check:
-	python -m twine check dist/*
-
-dist: clean build dist-build dist-check  ## Build dists
-
-publish:  # Upload python assets
-	echo "would usually run python -m twine upload dist/* --skip-existing"
-
-#########
-# CLEAN #
-#########
-deep-clean: ## clean everything from the repository
-	git clean -fdx
-
-clean: ## clean the repository
-	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
-
-############################################################################################
-
-# Thanks to Francoise at marmelab.com for this
-.DEFAULT_GOAL := help
-help:
-	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
-
-print-%:
-	@echo '$*=$($*)'
-
-.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+#########
+# BUILD #
+#########
+develop:  ## install dependencies and build library
+	python -m pip install -e .[develop]
+
+build:  ## build the python library
+	python setup.py build build_ext --inplace
+
+install:  ## install library
+	python -m pip install .
+
+#########
+# LINTS #
+#########
+lint:  ## run static analysis with flake8
+	python -m black --check SportsCardTool setup.py
+	python -m flake8 SportsCardTool setup.py
+
+# Alias
+lints: lint
+
+format:  ## run autoformatting with black
+	python -m black SportsCardTool/ setup.py
+
+# alias
+fix: format
+
+check:  ## check assets for packaging
+	check-manifest -v
+
+# Alias
+checks: check
+
+annotate:  ## run type checking
+	python -m mypy ./SportsCardTool
+
+#########
+# TESTS #
+#########
+test: ## clean and run unit tests
+	python -m pytest -v SportsCardTool/tests
+
+coverage:  ## clean and run unit tests with coverage
+	python -m pytest -v SportsCardTool/tests --cov=SportsCardTool --cov-branch --cov-fail-under=70 --cov-report term-missing
+
+# Alias
+tests: test
+
+###########
+# VERSION #
+###########
+show-version:
+	bump2version --dry-run --allow-dirty setup.py --list | grep current | awk -F= '{print $2}'
+
+patch:
+	bump2version patch
+
+minor:
+	bump2version minor
+
+major:
+	bump2version major
+
+########
+# DIST #
+########
+dist-build:  # Build python dist
+	python setup.py sdist bdist_wheel
+
+dist-check:
+	python -m twine check dist/*
+
+dist: clean build dist-build dist-check  ## Build dists
+
+publish:  # Upload python assets
+	echo "would usually run python -m twine upload dist/* --skip-existing"
+
+#########
+# CLEAN #
+#########
+deep-clean: ## clean everything from the repository
+	git clean -fdx
+
+clean: ## clean the repository
+	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
+
+############################################################################################
+
+# Thanks to Francoise at marmelab.com for this
+.DEFAULT_GOAL := help
+help:
+	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
+
+print-%:
+	@echo '$*=$($*)'
+
+.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
```

### Comparing `SportsCardTool-0.2.3/PKG-INFO` & `SportsCardTool-0.2.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,375 +1,374 @@
-Metadata-Version: 2.1
-Name: SportsCardTool
-Version: 0.2.3
-Summary: A python tool for grabbing and tracking checklists for sports cards.
-Author-email: Travis Gibbs <travisgibbs.2019@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: repository, https://github.com/TravisGibbs/SportsCardTool
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
-# SportsCardTool
-
-[![Build Status](https://github.com/TravisGibbs/SportsCardTool/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/TravisGibbs/SportsCardTool/actions?query=workflow%3A%22Build+Status%22)
-[![codecov](https://codecov.io/gh/TravisGibbs/SportsCardTool/branch/main/graph/badge.svg)](https://codecov.io/gh/TravisGibbs/SportsCardTool)
-[![PyPI](https://img.shields.io/pypi/v/SportsCardTool)](https://pypi.org/project/SportsCardTool/)
-
-<img src="https://img.shields.io/badge/license-Apache--2.0-green"/>
-<img src="https://img.shields.io/github/issues/travisgibbs/SportsCardTool?style=plastic"/>
-
-SportsCardTool is designed to gather card data and track collections of cards. We hope to build the modern dynamic checklist and price book.
-
-Currently SportsCardTool provides the ability to gather all baseball card setlists and to search prescraped data via data API and Querybuilder tool.
-
-Potential contributors should check out [SportsCardToolServer](https://github.com/TravisGibbs/SportsCardToolServer).
-
-## Install it from PyPI
-
-```bash
-pip install SportsCardTool
-```
-
-## Usage
-
-Scraping a year of data:
-
-
-```py
-
-from SportsCardTool import grab_card_list, dump_data, grab_year_links
-
-# Find All Cards for 2023 Season, returned as list of dictionaries
-year_links = grab_year_links(["2023"])
-card_list = grab_card_list(year_link)
-
-# Create CSV to allow for manipulation via pandas
-dump_data(mock_data, "2023_cards.csv")
-
-```
-
-Grabbing cards from scraped data via code:
-Also accessible directly [here](https://travisapi.pythonanywhere.com/api/v1/sportscards/search?)!
-
-```py
-
-from SportsCardTool import QueryBuilder
-
-qb = QueryBuilder()
-
-# Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
-qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
-
-# Make request and return in form of tuple (list[dict], int)
-data = qb.grab_data()
-
-print(data[0])
-```
-```json
-[
-    {
-      "_id": "641f49185ee984b20a66ef77",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "fleer-ultra",
-      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "11",
-      "price": 0,
-      "rc": false,
-      "serial": 250,
-      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a66f5f4",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "fleer-ultra",
-      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "11",
-      "price": 0,
-      "rc": false,
-      "serial": 250,
-      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a674b2f",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "upper-deck",
-      "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
-      "mem": true,
-      "name": "Barry Bonds",
-      "number": "BB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a678e31",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "upper-deck-pros-and-prospects",
-      "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
-      "mem": true,
-      "name": "Barry Bonds",
-      "number": "BB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a67958c",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "sp-authentic",
-      "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "GBB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    }
-]
-```
-
-## Development
-
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
-### Attribution
-
-This README was adapted from an example [here](https://github.com/rochacbruno/python-project-template/blob/main/README.md)
+Metadata-Version: 2.1
+Name: SportsCardTool
+Version: 0.2.4
+Summary: A python tool for grabbing and tracking checklists for sports cards.
+Author-email: Travis Gibbs <travisgibbs.2019@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: repository, https://github.com/TravisGibbs/SportsCardTool
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
+# SportsCardTool
+
+[![Build Status](https://github.com/TravisGibbs/SportsCardTool/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/TravisGibbs/SportsCardTool/actions?query=workflow%3A%22Build+Status%22)
+[![codecov](https://codecov.io/gh/TravisGibbs/SportsCardToolLib/branch/main/graph/badge.svg?token=D45VY693WQ)](https://codecov.io/gh/TravisGibbs/SportsCardToolLib)[![PyPI](https://img.shields.io/pypi/v/SportsCardTool)](https://pypi.org/project/SportsCardTool/)
+
+<img src="https://img.shields.io/badge/license-Apache--2.0-green"/>
+<img src="https://img.shields.io/github/issues/travisgibbs/SportsCardTool?style=plastic"/>
+
+SportsCardTool is designed to gather card data and track collections of cards. We hope to build the modern dynamic checklist and price book.
+
+Currently SportsCardTool provides the ability to gather all baseball card setlists and to search prescraped data via data API and Querybuilder tool.
+
+Potential contributors should check out [SportsCardToolServer](https://github.com/TravisGibbs/SportsCardToolServer) and soon to launch [SportsCardToolApp](https://github.com/TravisGibbs/SportsCardToolApp).
+
+## Install it from PyPI
+
+```bash
+pip install SportsCardTool
+```
+
+## Usage
+
+Scraping a year of data:
+
+
+```py
+
+from SportsCardTool import grab_card_list, dump_data, grab_year_links
+
+# Find All Cards for 2023 Season, returned as list of dictionaries
+year_links = grab_year_links(["2023"])
+card_list = grab_card_list(year_link)
+
+# Create CSV to allow for manipulation via pandas
+dump_data(mock_data, "2023_cards.csv")
+
+```
+
+Grabbing cards from scraped data via code:
+Also accessible directly [here](https://travisapi.pythonanywhere.com/api/v1/sportscards/search?)!
+
+```py
+
+from SportsCardTool import QueryBuilder
+
+qb = QueryBuilder()
+
+# Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
+qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
+
+# Make request and return in form of tuple (list[dict], int)
+data = qb.grab_data()
+
+print(data[0])
+```
+```json
+[
+    {
+      "_id": "641f49185ee984b20a66ef77",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "fleer-ultra",
+      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "11",
+      "price": 0,
+      "rc": false,
+      "serial": 250,
+      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a66f5f4",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "fleer-ultra",
+      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "11",
+      "price": 0,
+      "rc": false,
+      "serial": 250,
+      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a674b2f",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "upper-deck",
+      "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
+      "mem": true,
+      "name": "Barry Bonds",
+      "number": "BB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a678e31",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "upper-deck-pros-and-prospects",
+      "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
+      "mem": true,
+      "name": "Barry Bonds",
+      "number": "BB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a67958c",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "sp-authentic",
+      "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "GBB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    }
+]
+```
+
+## Development
+
+Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+### Attribution
+
+This README was adapted from an example [here](https://github.com/rochacbruno/python-project-template/blob/main/README.md)
```

### Comparing `SportsCardTool-0.2.3/README.md` & `SportsCardTool-0.2.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,153 +1,152 @@
-# SportsCardTool
-
-[![Build Status](https://github.com/TravisGibbs/SportsCardTool/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/TravisGibbs/SportsCardTool/actions?query=workflow%3A%22Build+Status%22)
-[![codecov](https://codecov.io/gh/TravisGibbs/SportsCardTool/branch/main/graph/badge.svg)](https://codecov.io/gh/TravisGibbs/SportsCardTool)
-[![PyPI](https://img.shields.io/pypi/v/SportsCardTool)](https://pypi.org/project/SportsCardTool/)
-
-<img src="https://img.shields.io/badge/license-Apache--2.0-green"/>
-<img src="https://img.shields.io/github/issues/travisgibbs/SportsCardTool?style=plastic"/>
-
-SportsCardTool is designed to gather card data and track collections of cards. We hope to build the modern dynamic checklist and price book.
-
-Currently SportsCardTool provides the ability to gather all baseball card setlists and to search prescraped data via data API and Querybuilder tool.
-
-Potential contributors should check out [SportsCardToolServer](https://github.com/TravisGibbs/SportsCardToolServer).
-
-## Install it from PyPI
-
-```bash
-pip install SportsCardTool
-```
-
-## Usage
-
-Scraping a year of data:
-
-
-```py
-
-from SportsCardTool import grab_card_list, dump_data, grab_year_links
-
-# Find All Cards for 2023 Season, returned as list of dictionaries
-year_links = grab_year_links(["2023"])
-card_list = grab_card_list(year_link)
-
-# Create CSV to allow for manipulation via pandas
-dump_data(mock_data, "2023_cards.csv")
-
-```
-
-Grabbing cards from scraped data via code:
-Also accessible directly [here](https://travisapi.pythonanywhere.com/api/v1/sportscards/search?)!
-
-```py
-
-from SportsCardTool import QueryBuilder
-
-qb = QueryBuilder()
-
-# Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
-qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
-
-# Make request and return in form of tuple (list[dict], int)
-data = qb.grab_data()
-
-print(data[0])
-```
-```json
-[
-    {
-      "_id": "641f49185ee984b20a66ef77",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "fleer-ultra",
-      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "11",
-      "price": 0,
-      "rc": false,
-      "serial": 250,
-      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a66f5f4",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "fleer-ultra",
-      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "11",
-      "price": 0,
-      "rc": false,
-      "serial": 250,
-      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a674b2f",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "upper-deck",
-      "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
-      "mem": true,
-      "name": "Barry Bonds",
-      "number": "BB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a678e31",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "upper-deck-pros-and-prospects",
-      "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
-      "mem": true,
-      "name": "Barry Bonds",
-      "number": "BB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a67958c",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "sp-authentic",
-      "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "GBB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    }
-]
-```
-
-## Development
-
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
-### Attribution
-
-This README was adapted from an example [here](https://github.com/rochacbruno/python-project-template/blob/main/README.md)
+# SportsCardTool
+
+[![Build Status](https://github.com/TravisGibbs/SportsCardTool/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/TravisGibbs/SportsCardTool/actions?query=workflow%3A%22Build+Status%22)
+[![codecov](https://codecov.io/gh/TravisGibbs/SportsCardToolLib/branch/main/graph/badge.svg?token=D45VY693WQ)](https://codecov.io/gh/TravisGibbs/SportsCardToolLib)[![PyPI](https://img.shields.io/pypi/v/SportsCardTool)](https://pypi.org/project/SportsCardTool/)
+
+<img src="https://img.shields.io/badge/license-Apache--2.0-green"/>
+<img src="https://img.shields.io/github/issues/travisgibbs/SportsCardTool?style=plastic"/>
+
+SportsCardTool is designed to gather card data and track collections of cards. We hope to build the modern dynamic checklist and price book.
+
+Currently SportsCardTool provides the ability to gather all baseball card setlists and to search prescraped data via data API and Querybuilder tool.
+
+Potential contributors should check out [SportsCardToolServer](https://github.com/TravisGibbs/SportsCardToolServer) and soon to launch [SportsCardToolApp](https://github.com/TravisGibbs/SportsCardToolApp).
+
+## Install it from PyPI
+
+```bash
+pip install SportsCardTool
+```
+
+## Usage
+
+Scraping a year of data:
+
+
+```py
+
+from SportsCardTool import grab_card_list, dump_data, grab_year_links
+
+# Find All Cards for 2023 Season, returned as list of dictionaries
+year_links = grab_year_links(["2023"])
+card_list = grab_card_list(year_link)
+
+# Create CSV to allow for manipulation via pandas
+dump_data(mock_data, "2023_cards.csv")
+
+```
+
+Grabbing cards from scraped data via code:
+Also accessible directly [here](https://travisapi.pythonanywhere.com/api/v1/sportscards/search?)!
+
+```py
+
+from SportsCardTool import QueryBuilder
+
+qb = QueryBuilder()
+
+# Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
+qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
+
+# Make request and return in form of tuple (list[dict], int)
+data = qb.grab_data()
+
+print(data[0])
+```
+```json
+[
+    {
+      "_id": "641f49185ee984b20a66ef77",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "fleer-ultra",
+      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "11",
+      "price": 0,
+      "rc": false,
+      "serial": 250,
+      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a66f5f4",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "fleer-ultra",
+      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "11",
+      "price": 0,
+      "rc": false,
+      "serial": 250,
+      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a674b2f",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "upper-deck",
+      "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
+      "mem": true,
+      "name": "Barry Bonds",
+      "number": "BB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a678e31",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "upper-deck-pros-and-prospects",
+      "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
+      "mem": true,
+      "name": "Barry Bonds",
+      "number": "BB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a67958c",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "sp-authentic",
+      "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "GBB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    }
+]
+```
+
+## Development
+
+Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+### Attribution
+
+This README was adapted from an example [here](https://github.com/rochacbruno/python-project-template/blob/main/README.md)
```

### Comparing `SportsCardTool-0.2.3/SportsCardTool/bref_tool.py` & `SportsCardTool-0.2.4/SportsCardTool/bref_tool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,105 @@
-import requests
-from bs4 import BeautifulSoup
-from time import sleep
-from typing import Dict
-from typing import List
-
-
-"""
-This File contains tools for searching baseball reference.
-"""
-
-import unicodedata
-
-
-def remove_accents(input: str) -> str:
-    """Removes accent marks and capitlization from string.
-
-    Standardizing strings makes matching between cardlists and bref possible.
-    Credit To: https://stackoverflow.com/questions/517923
-
-    Args:
-        input: A string to be modified.
-
-    Returns:
-        An output string that is lowered and removes all non standard characthers.
-
-    """
-    nfkd_form = unicodedata.normalize('NFKD', input)
-    only_ascii = nfkd_form.encode('ASCII', 'ignore')
-    return only_ascii.decode()
-
-
-def grab_debut_year(year: str) -> Dict:
-    """Grabs bref info for all players who debuted in a given year.
-
-    Args:
-        year: A string containing a year to be searching on baseball reference
-        IE: "2017"
-
-    Returns:
-        A dictionary with the players stored in a dictionary keyed by their names.
-
-        Note this function sleeps between each call to respect baseball reference's
-        policies, please do not modify.
-
-    """
-    year_dictionary = {}
-    print("scraping year " + year)
-    url = "https://www.baseball-reference.com/leagues/majors/" + year + "-debuts.shtml"
-    # Sleep before firing requests to respect baseball reference guidelines
-    sleep(3)
-    r = requests.get(url)
-    soup = BeautifulSoup(r.content, features="lxml")
-    # Grab table containing all debuts
-    table = soup.find("tbody")
-    for row in table.find_all("tr"):
-        player = {"debut_year": year}
-        player['last_game'] = None
-        player['last_year'] = None
-        player["debut"] = None
-        player['short_name'] = None
-        player['href'] = None
-        player['draft_year'] = None
-        player['WAR'] = None
-        for col in row.find_all("td"):
-            col_name = col["data-stat"]
-            if col_name == "player":
-                player_link = col.find("a")
-                player['href'] = player_link['href']
-                name = remove_accents(player_link.get_text())
-                player['short_name'] = col['data-append-csv']
-            elif col_name == "debut":
-                link = col.find("a")
-                if link:
-                    link_text = link.get_text()
-                    if link_text != "" and link_text is not None:
-                        player['debut'] = link.get_text() + ", " + year
-            elif col_name == "final_game":
-                game_link = col.find("a")
-                if game_link:
-                    game_link_text = game_link.get_text()
-                    if game_link_text != "" and game_link_text is not None:
-                        player['last_game'] = game_link_text
-                        player['last_year'] = player['last_game'].split(" ")[2]
-            elif col_name == "WAR":
-                player['WAR'] = col.text
-            elif col_name == "draft":
-                if "in" in col.text:
-                    player['draft_year'] = col.text.split("in ")[1].split(" ")[0][:4]
-
-        year_dictionary[name] = player
-    return year_dictionary
-
-
-def grab_debut_dict(
-    years: List[str], allow_repeats: bool = False, dictionary: Dict = {"years": {}, "players": {}}
-) -> dict:
-    """Master function that allows users to search accross multiple years
-
-    Args:
-        years: A list of strings representing years.
-        IE: ["1940",  "1941"]
-
-        allow_repeats: If True will search a year again even if it
-        is already in passed in dictionary.
-
-        dictionary: A dict that defualts to two empty keyed dicts for years
-        and players.
-
-    Returns:
-        A dictionary in the same format as what is passed in
-        with player info from all debut years.
-
-    """
-    for year in years:
-        if year not in dictionary['years'] or allow_repeats:
-            year_dictionary = grab_debut_year(year)
-            dictionary['players'].update(year_dictionary)
-            # Flag year to avoid repeated searches
-            dictionary["years"][year] = True
-    return dictionary
+import requests
+from bs4 import BeautifulSoup
+from time import sleep
+from typing import Dict
+from typing import List
+
+from SportsCardTool.util import remove_accents
+
+
+"""
+This File contains tools for searching baseball reference.
+"""
+
+
+def grab_debut_year(year: str) -> Dict:
+    """Grabs bref info for all players who debuted in a given year.
+
+    Args:
+        year: A string containing a year to be searching on baseball reference
+        IE: "2017"
+
+    Returns:
+        A dictionary with the players stored in a dictionary keyed by their names.
+
+        Note this function sleeps between each call to respect baseball reference's
+        policies, please do not modify.
+
+    """
+    year_dictionary = {}
+    print("scraping year " + year)
+    url = "https://www.baseball-reference.com/leagues/majors/" + year + "-debuts.shtml"
+    # Sleep before firing requests to respect baseball reference guidelines
+    sleep(3)
+    r = requests.get(url)
+    soup = BeautifulSoup(r.content, features="lxml")
+    # Grab table containing all debuts
+    table = soup.find("tbody")
+    for row in table.find_all("tr"):
+        player = {"debut_year": year}
+        player["last_game"] = None
+        player["last_year"] = None
+        player["debut"] = None
+        player["short_name"] = None
+        player["href"] = None
+        player["draft_year"] = None
+        player["WAR"] = None
+        for col in row.find_all("td"):
+            col_name = col["data-stat"]
+            if col_name == "player":
+                player_link = col.find("a")
+                player["href"] = player_link["href"]
+                name = remove_accents(player_link.get_text())
+                player["short_name"] = col["data-append-csv"]
+            elif col_name == "debut":
+                link = col.find("a")
+                if link:
+                    link_text = link.get_text()
+                    if link_text != "" and link_text is not None:
+                        player["debut"] = link.get_text() + ", " + year
+            elif col_name == "final_game":
+                game_link = col.find("a")
+                if game_link:
+                    game_link_text = game_link.get_text()
+                    if game_link_text != "" and game_link_text is not None:
+                        player["last_game"] = game_link_text
+                        player["last_year"] = player["last_game"].split(" ")[2]
+            elif col_name == "WAR":
+                player["WAR"] = col.text
+            elif col_name == "draft":
+                if "in" in col.text:
+                    player["draft_year"] = col.text.split("in ")[1].split(" ")[0][:4]
+
+        year_dictionary[name] = player
+    return year_dictionary
+
+
+def grab_debut_dict(
+    years: List[str],
+    allow_repeats: bool = False,
+    dictionary: Dict = {"years": {}, "players": {}},
+) -> dict:
+    """Master function that allows users to search accross multiple years
+
+    Args:
+        years: A list of strings representing years.
+        IE: ["1940",  "1941"]
+
+        allow_repeats: If True will search a year again even if it
+        is already in passed in dictionary.
+
+        dictionary: A dict that defualts to two empty keyed dicts for years
+        and players.
+
+    Returns:
+        A dictionary in the same format as what is passed in
+        with player info from all debut years.
+
+    """
+    for year in years:
+        if year not in dictionary["years"] or allow_repeats:
+            year_dictionary = grab_debut_year(year)
+            dictionary["players"].update(year_dictionary)
+            # Flag year to avoid repeated searches
+            dictionary["years"][year] = True
+    return dictionary
```

### Comparing `SportsCardTool-0.2.3/SportsCardTool/data/bref_data.json` & `SportsCardTool-0.2.4/SportsCardTool/data/bref_data.json`

 * *Files identical despite different names*

### Comparing `SportsCardTool-0.2.3/SportsCardTool/searching_tool.py` & `SportsCardTool-0.2.4/SportsCardTool/searching_tool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import requests
-import json
-
-"""
-This file contains the query building class which helps users access data api.
-"""
-
-DEV_QUERY = "http://127.0.0.1:5000/api/v1/sportscards/search?"
-BASE_QUERY = "https://travisapi.pythonanywhere.com/api/v1/sportscards/search?"
-
-
-class query_builder:
-    """The query_builder class allows for quick queries to SportsCardTool's API
-
-    The API can also be accessed manually for now, but this class helps build queries progmatically.
-
-    Attributes:
-        query: A string containing the query to the API
-        terms: A int counting the number of terms in query
-
-    """
-
-    def __init__(
-        self,
-        base: str = BASE_QUERY,
-    ) -> None:
-        """Intializes the query builder object.
-
-        Args:
-            base: The base url of query, defaults to the where the API is currently hosted.
-            Do not recommend changing unless performing local development on server.
-        """
-        self.query = base
-        self.terms = 0
-
-    # Possible key value pairs: [name, team, group, set, year, serial, auto, mem, contains]
-    # Specify multiple item queries as comma seperated string IE {"name": "Rafael Devers,Juan Soto"}
-    # Searching via contains key checks if string is contained in the listing (non-case sensitive)
-    def add_item(self, filters: dict):
-        """Adds items from a dictionary of key value pairs to the query.
-
-        Key value pairs are parsed into url params. In the future we would like to support
-        clauses and conditionals, but currently we support the following:
-
-        Possible keys: [name, team, group, set, year, serial, auto, mem, contains]
-        Specify multi value queries as comma seperated string IE {"name": "Rafael Devers,Juan Soto"}
-        Searching via contains key checks if string is contained in the listing (non-case sensitive)
-
-        Args:
-            filters: A dictionary keyed by term and valued with a string containing all desired values.
-
-        """
-        for key, value in filters.items():
-            if self.terms == 0:
-                self.query += key + "=" + value
-            else:
-                self.query += "&" + key + "=" + value
-
-            self.terms += 1
-
-    def grab_data(self, min_results: int = 1000):
-        """Executes query as defined by class atribute.
-
-        Pages through results produced by query string untill
-        it hits the min results argument or runs out of data.
-
-        Args:
-            min_results: An int specifying how many results at
-            a minimum to return.
-
-        Returns:
-            A tuples where the first value is a list of dictionarties of results
-            and the second value is an int with the total number of results.
-
-        """
-        total_results = 0
-        results = []
-        page = 0
-
-        print("Fetching Results")
-        while True:
-            q = self.query + "&page=" + str(page)
-            r = requests.get(q)
-
-            data = json.loads(r.content)
-            results.extend(data['cards'])
-            total_results += len(data['cards'])
-
-            # If this is the last page we break
-            if data['total_results'] < data["entries_per_page"] or total_results >= min_results:
-                break
-
-            page += 1
-
-        return (results, total_results)
+import requests
+import json
+
+"""
+This file contains the query building class which helps users access data api.
+"""
+
+DEV_QUERY = "http://127.0.0.1:5000/api/v1/sportscards/search?"
+BASE_QUERY = "https://travisapi.pythonanywhere.com/api/v1/sportscards/search?"
+
+
+class query_builder:
+    """The query_builder class allows for quick queries to SportsCardTool's API
+
+    The API can also be accessed manually for now, but this class helps build queries progmatically.
+
+    Attributes:
+        query: A string containing the query to the API
+        terms: A int counting the number of terms in query
+
+    """
+
+    def __init__(
+        self,
+        base: str = BASE_QUERY,
+    ) -> None:
+        """Intializes the query builder object.
+
+        Args:
+            base: The base url of query, defaults to the where the API is currently hosted.
+            Do not recommend changing unless performing local development on server.
+        """
+        self.query = base
+        self.terms = 0
+
+    # Possible key value pairs: [name, team, group, set, year, serial, auto, mem, contains]
+    # Specify multiple item queries as comma seperated string IE {"name": "Rafael Devers,Juan Soto"}
+    # Searching via contains key checks if string is contained in the listing (non-case sensitive)
+    def add_item(self, filters: dict):
+        """Adds items from a dictionary of key value pairs to the query.
+
+        Key value pairs are parsed into url params. In the future we would like to support
+        clauses and conditionals, but currently we support the following:
+
+        Possible keys: [name, team, group, set, year, serial, auto, mem, contains]
+        Specify multi value queries as comma seperated string IE {"name": "Rafael Devers,Juan Soto"}
+        Searching via contains key checks if string is contained in the listing (non-case sensitive)
+
+        Args:
+            filters: A dictionary keyed by term and valued with a string containing all desired values.
+
+        """
+        for key, value in filters.items():
+            if self.terms == 0:
+                self.query += key + "=" + value
+            else:
+                self.query += "&" + key + "=" + value
+
+            self.terms += 1
+
+    def grab_data(self, min_results: int = 20):
+        """Executes query as defined by class atribute.
+
+        Pages through results produced by query string untill
+        it hits the min results argument or runs out of data.
+
+        Args:
+            min_results: An int specifying how many results at
+            a minimum to return.
+
+        Returns:
+            A tuples where the first value is a list of dictionarties of results
+            and the second value is an int with the total number of results.
+
+        """
+        total_results = 0
+        results = []
+        page = 0
+
+        print("Fetching Results")
+        while True:
+            q = self.query + "&page=" + str(page)
+            r = requests.get(q)
+
+            data = json.loads(r.content)
+            results.extend(data["cards"])
+            total_results += len(data["cards"])
+
+            # If this is the last page we break
+            if data["total_results"] < data["entries_per_page"] or total_results >= min_results:
+                break
+
+            page += 1
+
+        return (results, total_results)
```

### Comparing `SportsCardTool-0.2.3/SportsCardTool.egg-info/PKG-INFO` & `SportsCardTool-0.2.4/SportsCardTool.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,375 +1,374 @@
-Metadata-Version: 2.1
-Name: SportsCardTool
-Version: 0.2.3
-Summary: A python tool for grabbing and tracking checklists for sports cards.
-Author-email: Travis Gibbs <travisgibbs.2019@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: repository, https://github.com/TravisGibbs/SportsCardTool
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
-# SportsCardTool
-
-[![Build Status](https://github.com/TravisGibbs/SportsCardTool/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/TravisGibbs/SportsCardTool/actions?query=workflow%3A%22Build+Status%22)
-[![codecov](https://codecov.io/gh/TravisGibbs/SportsCardTool/branch/main/graph/badge.svg)](https://codecov.io/gh/TravisGibbs/SportsCardTool)
-[![PyPI](https://img.shields.io/pypi/v/SportsCardTool)](https://pypi.org/project/SportsCardTool/)
-
-<img src="https://img.shields.io/badge/license-Apache--2.0-green"/>
-<img src="https://img.shields.io/github/issues/travisgibbs/SportsCardTool?style=plastic"/>
-
-SportsCardTool is designed to gather card data and track collections of cards. We hope to build the modern dynamic checklist and price book.
-
-Currently SportsCardTool provides the ability to gather all baseball card setlists and to search prescraped data via data API and Querybuilder tool.
-
-Potential contributors should check out [SportsCardToolServer](https://github.com/TravisGibbs/SportsCardToolServer).
-
-## Install it from PyPI
-
-```bash
-pip install SportsCardTool
-```
-
-## Usage
-
-Scraping a year of data:
-
-
-```py
-
-from SportsCardTool import grab_card_list, dump_data, grab_year_links
-
-# Find All Cards for 2023 Season, returned as list of dictionaries
-year_links = grab_year_links(["2023"])
-card_list = grab_card_list(year_link)
-
-# Create CSV to allow for manipulation via pandas
-dump_data(mock_data, "2023_cards.csv")
-
-```
-
-Grabbing cards from scraped data via code:
-Also accessible directly [here](https://travisapi.pythonanywhere.com/api/v1/sportscards/search?)!
-
-```py
-
-from SportsCardTool import QueryBuilder
-
-qb = QueryBuilder()
-
-# Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
-qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
-
-# Make request and return in form of tuple (list[dict], int)
-data = qb.grab_data()
-
-print(data[0])
-```
-```json
-[
-    {
-      "_id": "641f49185ee984b20a66ef77",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "fleer-ultra",
-      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "11",
-      "price": 0,
-      "rc": false,
-      "serial": 250,
-      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a66f5f4",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "fleer-ultra",
-      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "11",
-      "price": 0,
-      "rc": false,
-      "serial": 250,
-      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a674b2f",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "upper-deck",
-      "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
-      "mem": true,
-      "name": "Barry Bonds",
-      "number": "BB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a678e31",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "upper-deck-pros-and-prospects",
-      "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
-      "mem": true,
-      "name": "Barry Bonds",
-      "number": "BB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    },
-    {
-      "_id": "641f49185ee984b20a67958c",
-      "auto": true,
-      "back_img": null,
-      "front_img": null,
-      "group": "sp-authentic",
-      "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
-      "mem": false,
-      "name": "Barry Bonds",
-      "number": "GBB",
-      "price": 0,
-      "rc": false,
-      "serial": 25,
-      "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
-      "team": "San Francisco Giants",
-      "year": 2000
-    }
-]
-```
-
-## Development
-
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
-
-### Attribution
-
-This README was adapted from an example [here](https://github.com/rochacbruno/python-project-template/blob/main/README.md)
+Metadata-Version: 2.1
+Name: SportsCardTool
+Version: 0.2.4
+Summary: A python tool for grabbing and tracking checklists for sports cards.
+Author-email: Travis Gibbs <travisgibbs.2019@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: repository, https://github.com/TravisGibbs/SportsCardTool
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
+# SportsCardTool
+
+[![Build Status](https://github.com/TravisGibbs/SportsCardTool/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/TravisGibbs/SportsCardTool/actions?query=workflow%3A%22Build+Status%22)
+[![codecov](https://codecov.io/gh/TravisGibbs/SportsCardToolLib/branch/main/graph/badge.svg?token=D45VY693WQ)](https://codecov.io/gh/TravisGibbs/SportsCardToolLib)[![PyPI](https://img.shields.io/pypi/v/SportsCardTool)](https://pypi.org/project/SportsCardTool/)
+
+<img src="https://img.shields.io/badge/license-Apache--2.0-green"/>
+<img src="https://img.shields.io/github/issues/travisgibbs/SportsCardTool?style=plastic"/>
+
+SportsCardTool is designed to gather card data and track collections of cards. We hope to build the modern dynamic checklist and price book.
+
+Currently SportsCardTool provides the ability to gather all baseball card setlists and to search prescraped data via data API and Querybuilder tool.
+
+Potential contributors should check out [SportsCardToolServer](https://github.com/TravisGibbs/SportsCardToolServer) and soon to launch [SportsCardToolApp](https://github.com/TravisGibbs/SportsCardToolApp).
+
+## Install it from PyPI
+
+```bash
+pip install SportsCardTool
+```
+
+## Usage
+
+Scraping a year of data:
+
+
+```py
+
+from SportsCardTool import grab_card_list, dump_data, grab_year_links
+
+# Find All Cards for 2023 Season, returned as list of dictionaries
+year_links = grab_year_links(["2023"])
+card_list = grab_card_list(year_link)
+
+# Create CSV to allow for manipulation via pandas
+dump_data(mock_data, "2023_cards.csv")
+
+```
+
+Grabbing cards from scraped data via code:
+Also accessible directly [here](https://travisapi.pythonanywhere.com/api/v1/sportscards/search?)!
+
+```py
+
+from SportsCardTool import QueryBuilder
+
+qb = QueryBuilder()
+
+# Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
+qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
+
+# Make request and return in form of tuple (list[dict], int)
+data = qb.grab_data()
+
+print(data[0])
+```
+```json
+[
+    {
+      "_id": "641f49185ee984b20a66ef77",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "fleer-ultra",
+      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "11",
+      "price": 0,
+      "rc": false,
+      "serial": 250,
+      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a66f5f4",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "fleer-ultra",
+      "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "11",
+      "price": 0,
+      "rc": false,
+      "serial": 250,
+      "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a674b2f",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "upper-deck",
+      "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
+      "mem": true,
+      "name": "Barry Bonds",
+      "number": "BB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a678e31",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "upper-deck-pros-and-prospects",
+      "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
+      "mem": true,
+      "name": "Barry Bonds",
+      "number": "BB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    },
+    {
+      "_id": "641f49185ee984b20a67958c",
+      "auto": true,
+      "back_img": null,
+      "front_img": null,
+      "group": "sp-authentic",
+      "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
+      "mem": false,
+      "name": "Barry Bonds",
+      "number": "GBB",
+      "price": 0,
+      "rc": false,
+      "serial": 25,
+      "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
+      "team": "San Francisco Giants",
+      "year": 2000
+    }
+]
+```
+
+## Development
+
+Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
+### Attribution
+
+This README was adapted from an example [here](https://github.com/rochacbruno/python-project-template/blob/main/README.md)
```

### Comparing `SportsCardTool-0.2.3/docs/Makefile` & `SportsCardTool-0.2.4/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `SportsCardTool-0.2.3/docs/SportsCardTool.rst` & `SportsCardTool-0.2.4/docs/SportsCardTool.rst`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-SportsCardTool package
-======================
-
-Submodules
-----------
-
-SportsCardTool.bref\_tool module
---------------------------------
-
-.. automodule:: SportsCardTool.bref_tool
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-SportsCardTool.scraping\_tool module
-------------------------------------
-
-.. automodule:: SportsCardTool.scraping_tool
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-SportsCardTool.searching\_tool module
--------------------------------------
-
-.. automodule:: SportsCardTool.searching_tool
-   :members:
-   :undoc-members:
-   :show-inheritance:
+SportsCardTool package
+======================
+
+Submodules
+----------
+
+SportsCardTool.bref\_tool module
+--------------------------------
+
+.. automodule:: SportsCardTool.bref_tool
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+SportsCardTool.scraping\_tool module
+------------------------------------
+
+.. automodule:: SportsCardTool.scraping_tool
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+SportsCardTool.searching\_tool module
+-------------------------------------
+
+.. automodule:: SportsCardTool.searching_tool
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `SportsCardTool-0.2.3/docs/_build/html/_sources/install.rst.txt` & `SportsCardTool-0.2.4/docs/install.rst`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-Getting Started
-===============
-
-Installation
-------------
-
-To use SportsCardTool, first install it using pip:
-
-.. code-block:: console
-
-   pip install SportsCardTool
-
-Usage
------
-
-Scraping a year of data:
-
-
-.. code-block:: python
-
-   from SportsCardTool import grab_card_list, dump_data, grab_year_links
-
-   # Find All Cards for 2023 Season, returned as list of dictionaries
-   year_links = grab_year_links(["2023"])
-   card_list = grab_card_list(year_link)
-
-   # Create CSV to allow for manipulation via pandas
-   dump_data(mock_data, "2023_cards.csv")
-
-
-Grabbing cards from scraped data
-
-.. code-block:: python
-
-   from SportsCardTool import QueryBuilder
-
-   qb = QueryBuilder()
-
-   # Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
-   qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
-
-   # Make request and return in form of tuple (list[dict], int)
-   data = qb.grab_data()
-
-   print(data[0])
-
-.. code-block:: json
-   
-
-   [
-      {
-         "_id": "641f49185ee984b20a66ef77",
-         "auto": true,
-         "back_img": null,
-         "front_img": null,
-         "group": "fleer-ultra",
-         "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-         "mem": false,
-         "name": "Barry Bonds",
-         "number": "11",
-         "price": 0,
-         "rc": false,
-         "serial": 250,
-         "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-         "team": "San Francisco Giants",
-         "year": 2000
-      },
-      {
-         "_id": "641f49185ee984b20a66f5f4",
-         "auto": true,
-         "back_img": null,
-         "front_img": null,
-         "group": "fleer-ultra",
-         "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
-         "mem": false,
-         "name": "Barry Bonds",
-         "number": "11",
-         "price": 0,
-         "rc": false,
-         "serial": 250,
-         "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
-         "team": "San Francisco Giants",
-         "year": 2000
-      },
-      {
-         "_id": "641f49185ee984b20a674b2f",
-         "auto": true,
-         "back_img": null,
-         "front_img": null,
-         "group": "upper-deck",
-         "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
-         "mem": true,
-         "name": "Barry Bonds",
-         "number": "BB",
-         "price": 0,
-         "rc": false,
-         "serial": 25,
-         "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
-         "team": "San Francisco Giants",
-         "year": 2000
-      },
-      {
-         "_id": "641f49185ee984b20a678e31",
-         "auto": true,
-         "back_img": null,
-         "front_img": null,
-         "group": "upper-deck-pros-and-prospects",
-         "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
-         "mem": true,
-         "name": "Barry Bonds",
-         "number": "BB",
-         "price": 0,
-         "rc": false,
-         "serial": 25,
-         "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
-         "team": "San Francisco Giants",
-         "year": 2000
-      },
-      {
-         "_id": "641f49185ee984b20a67958c",
-         "auto": true,
-         "back_img": null,
-         "front_img": null,
-         "group": "sp-authentic",
-         "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
-         "mem": false,
-         "name": "Barry Bonds",
-         "number": "GBB",
-         "price": 0,
-         "rc": false,
-         "serial": 25,
-         "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
-         "team": "San Francisco Giants",
-         "year": 2000
-      }
-   ]
+Getting Started
+===============
+
+Installation
+------------
+
+To use SportsCardTool, first install it using pip:
+
+.. code-block:: console
+
+   pip install SportsCardTool
+
+Usage
+-----
+
+Scraping a year of data:
+
+
+.. code-block:: python
+
+   from SportsCardTool import grab_card_list, dump_data, grab_year_links
+
+   # Find All Cards for 2023 Season, returned as list of dictionaries
+   year_links = grab_year_links(["2023"])
+   card_list = grab_card_list(year_link)
+
+   # Create CSV to allow for manipulation via pandas
+   dump_data(mock_data, "2023_cards.csv")
+
+
+Grabbing cards from scraped data
+
+.. code-block:: python
+
+   from SportsCardTool import QueryBuilder
+
+   qb = QueryBuilder()
+
+   # Construct query requesting Barry Bonds cards from 2000 with an autograph and a print run of 25 or 250
+   qb.add_item({"name": "Barry Bonds", "year": "2000", "auto": "True", "serial": "25,250"})
+
+   # Make request and return in form of tuple (list[dict], int)
+   data = qb.grab_data()
+
+   print(data[0])
+
+.. code-block:: json
+   
+
+   [
+      {
+         "_id": "641f49185ee984b20a66ef77",
+         "auto": true,
+         "back_img": null,
+         "front_img": null,
+         "group": "fleer-ultra",
+         "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+         "mem": false,
+         "name": "Barry Bonds",
+         "number": "11",
+         "price": 0,
+         "rc": false,
+         "serial": 250,
+         "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+         "team": "San Francisco Giants",
+         "year": 2000
+      },
+      {
+         "_id": "641f49185ee984b20a66f5f4",
+         "auto": true,
+         "back_img": null,
+         "front_img": null,
+         "group": "fleer-ultra",
+         "listing": "2000 Fleer Ultra Fresh Ink #11 Barry Bonds",
+         "mem": false,
+         "name": "Barry Bonds",
+         "number": "11",
+         "price": 0,
+         "rc": false,
+         "serial": 250,
+         "set": "fleer-ultra-fresh-ink-baseball-trading-card-checklist",
+         "team": "San Francisco Giants",
+         "year": 2000
+      },
+      {
+         "_id": "641f49185ee984b20a674b2f",
+         "auto": true,
+         "back_img": null,
+         "front_img": null,
+         "group": "upper-deck",
+         "listing": "2000 Upper Deck  Game Jersey Autograph Numbered #BB Barry Bonds",
+         "mem": true,
+         "name": "Barry Bonds",
+         "number": "BB",
+         "price": 0,
+         "rc": false,
+         "serial": 25,
+         "set": "upper-deck-game-jersey-autograph-numbered-baseball-trading-card-checklist",
+         "team": "San Francisco Giants",
+         "year": 2000
+      },
+      {
+         "_id": "641f49185ee984b20a678e31",
+         "auto": true,
+         "back_img": null,
+         "front_img": null,
+         "group": "upper-deck-pros-and-prospects",
+         "listing": "2000 Upper Deck Pros and Prospects Game Jersey Autograph Gold #BB Barry Bonds",
+         "mem": true,
+         "name": "Barry Bonds",
+         "number": "BB",
+         "price": 0,
+         "rc": false,
+         "serial": 25,
+         "set": "upper-deck-pros-and-prospects-game-jersey-autograph-gold-baseball-trading-card-checklist",
+         "team": "San Francisco Giants",
+         "year": 2000
+      },
+      {
+         "_id": "641f49185ee984b20a67958c",
+         "auto": true,
+         "back_img": null,
+         "front_img": null,
+         "group": "sp-authentic",
+         "listing": "2000 SP Authentic Chirography Gold #GBB Barry Bonds",
+         "mem": false,
+         "name": "Barry Bonds",
+         "number": "GBB",
+         "price": 0,
+         "rc": false,
+         "serial": 25,
+         "set": "sp-authentic-chirography-gold-baseball-trading-card-checklist",
+         "team": "San Francisco Giants",
+         "year": 2000
+      }
+   ]
```

### Comparing `SportsCardTool-0.2.3/docs/conf.py` & `SportsCardTool-0.2.4/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-import sys
-import os
-
-sys.path.insert(0, os.path.abspath(".."))
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = 'SportsCardTool'
-copyright = '2023, Travis Gibbs'
-author = 'Travis Gibbs'
-release = '0.2.1'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = ['sphinx.ext.autodoc']
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = 'alabaster'
-html_static_path = ['_static']
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+import sys
+import os
+
+sys.path.insert(0, os.path.abspath(".."))
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = 'SportsCardTool'
+copyright = '2023, Travis Gibbs'
+author = 'Travis Gibbs'
+release = '0.2.1'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = ['sphinx.ext.autodoc']
+
+templates_path = ['_templates']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+html_theme = 'alabaster'
+html_static_path = ['_static']
```

### Comparing `SportsCardTool-0.2.3/docs/make.bat` & `SportsCardTool-0.2.4/docs/make.bat`

 * *Files identical despite different names*

