# Comparing `tmp/ms3-1.2.7.tar.gz` & `tmp/ms3-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms3-1.2.7.tar", last modified: Fri Apr 28 13:53:30 2023, max compression
+gzip compressed data, was "ms3-1.2.8.tar", last modified: Tue May  2 15:36:47 2023, max compression
```

## Comparing `ms3-1.2.7.tar` & `ms3-1.2.8.tar`

### file list

```diff
@@ -1,317 +1,317 @@
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.185244 ms3-1.2.7/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      586 2020-05-03 17:52:04.000000 ms3-1.2.7/.coveragerc
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.091909 ms3-1.2.7/.github/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.095243 ms3-1.2.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      752 2023-03-18 08:04:35.000000 ms3-1.2.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      599 2023-03-18 08:04:35.000000 ms3-1.2.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.095243 ms3-1.2.7/.github/workflows/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      669 2023-01-28 14:33:36.000000 ms3-1.2.7/.github/workflows/draft-pdf.yml
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      541 2023-03-23 18:04:33.000000 ms3-1.2.7/.gitignore
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2020-07-06 00:26:02.000000 ms3-1.2.7/AUTHORS.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    23156 2023-04-28 13:53:00.000000 ms3-1.2.7/CHANGELOG.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    34500 2020-05-07 11:55:51.000000 ms3-1.2.7/LICENSE.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-04-28 13:53:30.185244 ms3-1.2.7/PKG-INFO
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4026 2023-03-21 14:17:58.000000 ms3-1.2.7/README.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2094 2022-12-15 11:35:36.000000 ms3-1.2.7/codemeta.json
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/.nojekyll
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7593 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/Makefile
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-01-28 14:33:36.000000 ms3-1.2.7/docs/README.md
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/_intersphinx/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      646 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/_intersphinx/bs4_objects.inv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1799 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/_intersphinx/bs4_objects.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/_static/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       18 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/_static/.gitignore
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/authors.rst
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.098576 ms3-1.2.7/docs/build/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.buildinfo
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.108576 ms3-1.2.7/docs/build/.doctrees/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.108576 ms3-1.2.7/docs/build/.doctrees/api/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2579 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/api/modules.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   619252 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/api/ms3.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3406 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/authors.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6354 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/changelog.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 10423401 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/environment.pickle
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14745 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/index.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7547 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/install.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4679 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/intro.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96686 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/license.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35413 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/manual.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4590 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.doctrees/quick.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/.nojekyll
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.121910 ms3-1.2.7/docs/build/doctrees/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4366 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/README.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3594 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/authors.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154262 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/changelog.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 13487965 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/environment.pickle
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35248 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/index.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7812 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/install.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97335 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/license.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.135243 ms3-1.2.7/docs/build/doctrees/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 14283956 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/manual/index.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.145243 ms3-1.2.7/docs/build/doctrees/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79212 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/old_src/quick_old.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    78946 2023-03-23 18:04:33.000000 ms3-1.2.7/docs/build/doctrees/quick.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 17416423 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/doctrees/reference.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.148577 ms3-1.2.7/docs/build/html/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/.buildinfo
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2023-03-18 10:45:36.000000 ms3-1.2.7/docs/build/html/.nojekyll
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15846 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/README.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.148577 ms3-1.2.7/docs/build/html/_modules/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15440 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/index.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.151910 ms3-1.2.7/docs/build/html/_modules/ms3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   121982 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/annotations.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   562760 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/bs4_parser.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   585871 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/corpus.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   119721 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/expand_dcml.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   299877 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/parse.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   337630 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/piece.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   326103 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/score.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   264338 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/transformations.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   930043 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/utils.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   139939 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/ms3/view.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    63215 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_modules/re.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.155243 ms3-1.2.7/docs/build/html/_sources/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/README.md.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/html/_sources/authors.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.7/docs/build/html/_sources/install.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/build/html/_sources/license.rst.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.155243 ms3-1.2.7/docs/build/html/_sources/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/manual/index.md.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.155243 ms3-1.2.7/docs/build/html/_sources/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/old_src/quick_old.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_sources/quick.md.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-03-21 14:17:58.000000 ms3-1.2.7/docs/build/html/_sources/reference.rst.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4418 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14621 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/basic.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4472 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/doctools.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      439 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      286 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/file.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   288580 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    89501 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/jquery.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/jupyter-sphinx.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4758 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/language_data.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/minus.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    39364 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/plus.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14668 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/pygments.css
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/scripts/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    86398 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5229 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18215 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/searchtools.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4712 2023-01-21 10:04:25.000000 ms3-1.2.7/docs/build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/styles/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   144661 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    58614 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      106 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/styles/theme.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    68420 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19530 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/underscore.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.091909 ms3-1.2.7/docs/build/html/_static/vendor/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.091909 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7427 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   101709 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   181264 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   105112 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60236 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24028 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   389948 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154840 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10084 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4776 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1845 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16465 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/authors.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    69269 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/changelog.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79722 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/genindex.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    31724 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19975 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/install.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    53099 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/license.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.158577 ms3-1.2.7/docs/build/html/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   338361 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/manual/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7352 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/objects.inv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/build/html/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60388 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/old_src/quick_old.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17021 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/py-modindex.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    47347 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/quick.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1763633 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/reference.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15656 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/search.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130526 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/html/searchindex.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/build/jupyter_execute/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/build/jupyter_execute/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   346220 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/jupyter_execute/manual/index.ipynb
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    49220 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/build/jupyter_execute/quick.ipynb
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/changelog.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      135 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/columns.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10588 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/conf.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   137117 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/cujus.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/examples/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      134 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/access_score_info.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       47 2021-10-16 12:40:03.000000 ms3-1.2.7/docs/examples/parse_directory.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       64 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_directory_mscx.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       58 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_directory_xml.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      199 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_key.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      173 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_other_directory.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-01-02 20:31:46.000000 ms3-1.2.7/docs/examples/parse_single_score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       71 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/index.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.7/docs/install.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/license.rst
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      715 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/corpus_after
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      174 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/corpus_before
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/index.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      488 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/manual/out
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9940 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/ms3_architecture.drawio
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   218314 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/ms3_architecture.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96827 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/o_quam.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/docs/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15949 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/old_src/quick_old.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/old_src/quick_old.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   163542 2020-11-02 16:20:48.000000 ms3-1.2.7/docs/quae.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/quick.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-03-21 14:17:58.000000 ms3-1.2.7/docs/reference.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       86 2023-03-23 18:04:34.000000 ms3-1.2.7/docs/requirements.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   115684 2021-10-20 14:43:53.000000 ms3-1.2.7/docs/stabat.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.161910 ms3-1.2.7/new_tests/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7378 2023-04-28 13:53:19.000000 ms3-1.2.7/new_tests/conftest.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.095243 ms3-1.2.7/new_tests/inferred_labels/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.165243 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19047 2022-12-15 11:35:36.000000 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   332296 2022-12-15 11:35:36.000000 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317949 2022-12-15 11:35:36.000000 ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      466 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/parse_script.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-04-28 13:53:00.000000 ms3-1.2.7/new_tests/test_cli.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      403 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_docs_examples.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    12424 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_extract.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6352 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3744 2023-01-02 20:31:46.000000 ms3-1.2.7/new_tests/test_score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      823 2023-01-17 21:52:55.000000 ms3-1.2.7/new_tests/test_transformations.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.171910 ms3-1.2.7/old_tests/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   388689 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/05_symph_fant_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      959 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/05_symph_fant_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   100539 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/05_symph_fant_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   488895 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7268 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2636 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   155973 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/76CASM34A33UM_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4361 2023-01-02 20:31:46.000000 ms3-1.2.7/old_tests/ALL_WARNINGS
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   256806 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/BWV_0815_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/BWV_0815_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/BWV_0815_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16417 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/D973deutscher01_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/D973deutscher01_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/D973deutscher01_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1490215 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      330 2023-01-02 20:31:46.000000 ms3-1.2.7/old_tests/IGNORED_WARNINGS
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   431522 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14480 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4560 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96112 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/K281-3_notes.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.175244 ms3-1.2.7/old_tests/MS3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1041665 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/05_symph_fant.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1034028 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/76CASM34A33UM.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   787637 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/BWV_0815.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    54002 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/D973deutscher01.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   701525 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   807371 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/MS3/K281-3.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   259369 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/MS3/stabat_03_coloured.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      624 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/README.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      224 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/conftest.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.175244 ms3-1.2.7/old_tests/harmonies/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9855 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    21459 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3905 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/harmonies/stabat_03_coloured.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.178577 ms3-1.2.7/old_tests/measures/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      889 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/05_symph_fant.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6504 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/BWV_0815.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      684 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/D973deutscher01.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2706 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4411 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/measures/stabat_03_coloured.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5885 2023-03-23 18:04:34.000000 ms3-1.2.7/old_tests/metadata.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.178577 ms3-1.2.7/old_tests/notes/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    74055 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/05_symph_fant.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   112389 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   102317 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/BWV_0815.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6173 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/D973deutscher01.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   230316 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    70952 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/notes/stabat_03_coloured.tsv
--rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)       45 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/parse_original.sh
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      750 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/paths1.json
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      844 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/paths2.json
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.178577 ms3-1.2.7/old_tests/repeat_dummies/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6909 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/repeat_dummies/repeats0.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6493 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/repeat_dummies/repeats1.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7376 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/repeat_dummies/repeats2.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   135170 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4822 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/stabat_03_coloured_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2207 2023-02-18 19:40:30.000000 ms3-1.2.7/old_tests/test_parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      712 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_repeats.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.181911 ms3-1.2.7/old_tests/test_results/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      921 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/05_symph_fant_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    98388 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/05_symph_fant_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7089 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/76CASM34A33UM_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2536 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/76CASM34A33UM_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   152525 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/76CASM34A33UM_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/BWV_0815_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/BWV_0815_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/D973deutscher01_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/D973deutscher01_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14099 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/K281-3_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4391 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/K281-3_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    94030 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/K281-3_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4731 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/stabat_03_coloured_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      758 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/stabat_03_coloured_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24478 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_results/stabat_03_coloured_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4777 2022-12-15 11:35:36.000000 ms3-1.2.7/old_tests/test_score.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.181911 ms3-1.2.7/paper/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17950 2023-03-21 14:17:58.000000 ms3-1.2.7/paper/paper.bib
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4605 2023-03-21 14:17:58.000000 ms3-1.2.7/paper/paper.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   200690 2023-01-28 14:33:36.000000 ms3-1.2.7/paper/paper.pdf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1364 2023-04-28 13:53:30.188577 ms3-1.2.7/setup.cfg
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      567 2020-05-03 17:52:04.000000 ms3-1.2.7/setup.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.181911 ms3-1.2.7/src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:27:59.000000 ms3-1.2.7/src/__init__.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.185244 ms3-1.2.7/src/ms3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1006 2023-02-18 19:40:30.000000 ms3-1.2.7/src/ms3/__init__.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2402 2023-02-18 19:40:30.000000 ms3-1.2.7/src/ms3/_typing.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24943 2023-01-12 10:36:52.000000 ms3-1.2.7/src/ms3/annotations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41608 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/bs4_measures.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130482 2023-04-26 16:41:43.000000 ms3-1.2.7/src/ms3/bs4_parser.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41211 2023-04-28 13:53:00.000000 ms3-1.2.7/src/ms3/cli.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   151734 2023-04-19 06:50:23.000000 ms3-1.2.7/src/ms3/corpus.py
--rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)    26692 2023-01-02 20:31:46.000000 ms3-1.2.7/src/ms3/expand_dcml.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8416 2023-01-02 20:31:46.000000 ms3-1.2.7/src/ms3/ferocious_names.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18415 2023-03-18 08:04:35.000000 ms3-1.2.7/src/ms3/logger.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15645 2023-04-28 13:53:00.000000 ms3-1.2.7/src/ms3/operations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    83765 2023-04-26 16:41:43.000000 ms3-1.2.7/src/ms3/parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    82901 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/piece.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97681 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    67393 2023-03-23 18:04:34.000000 ms3-1.2.7/src/ms3/transformations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   219679 2023-04-28 13:53:00.000000 ms3-1.2.7/src/ms3/utils.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    29853 2023-04-26 16:41:43.000000 ms3-1.2.7/src/ms3/view.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-04-28 13:53:30.185244 ms3-1.2.7/src/ms3.egg-info/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/PKG-INFO
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9420 2023-04-28 13:53:30.000000 ms3-1.2.7/src/ms3.egg-info/SOURCES.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/dependency_links.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       36 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/entry_points.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/not-zip-safe
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/requires.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        4 2023-04-28 13:53:29.000000 ms3-1.2.7/src/ms3.egg-info/top_level.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      318 2020-05-03 17:52:04.000000 ms3-1.2.7/tox.ini
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.910134 ms3-1.2.8/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      586 2020-05-03 17:52:04.000000 ms3-1.2.8/.coveragerc
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/.github/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.703466 ms3-1.2.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      752 2023-05-02 08:27:28.000000 ms3-1.2.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      599 2023-05-02 08:27:28.000000 ms3-1.2.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.706799 ms3-1.2.8/.github/workflows/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      669 2023-01-28 14:33:36.000000 ms3-1.2.8/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      541 2023-05-02 08:27:28.000000 ms3-1.2.8/.gitignore
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2020-07-06 00:26:02.000000 ms3-1.2.8/AUTHORS.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    23371 2023-05-02 15:33:29.000000 ms3-1.2.8/CHANGELOG.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    34500 2020-05-07 11:55:51.000000 ms3-1.2.8/LICENSE.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-05-02 15:36:47.910134 ms3-1.2.8/PKG-INFO
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4026 2023-05-01 12:14:08.000000 ms3-1.2.8/README.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2094 2022-12-15 11:35:36.000000 ms3-1.2.8/codemeta.json
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.713466 ms3-1.2.8/docs/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/.nojekyll
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7593 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/Makefile
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-01-28 14:33:36.000000 ms3-1.2.8/docs/README.md
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.713466 ms3-1.2.8/docs/_intersphinx/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      646 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/_intersphinx/bs4_objects.inv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1799 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/_intersphinx/bs4_objects.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.713466 ms3-1.2.8/docs/_static/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       18 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/_static/.gitignore
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/authors.rst
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.716799 ms3-1.2.8/docs/build/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.buildinfo
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.736800 ms3-1.2.8/docs/build/.doctrees/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.736800 ms3-1.2.8/docs/build/.doctrees/api/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2579 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/api/modules.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   619252 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/api/ms3.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3406 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/authors.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6354 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/changelog.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 10423401 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14745 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/index.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7547 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/install.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4679 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/intro.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96686 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/license.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35413 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/manual.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4590 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/quick.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.nojekyll
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.760133 ms3-1.2.8/docs/build/doctrees/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4366 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/README.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3594 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/authors.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154262 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/changelog.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 13487965 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35248 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/index.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7812 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/install.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97335 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/license.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.783466 ms3-1.2.8/docs/build/doctrees/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 14283956 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/manual/index.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.806800 ms3-1.2.8/docs/build/doctrees/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79212 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/old_src/quick_old.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    78946 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/quick.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 17416423 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/reference.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.813467 ms3-1.2.8/docs/build/html/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/.buildinfo
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2023-03-18 10:45:36.000000 ms3-1.2.8/docs/build/html/.nojekyll
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15846 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/README.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.816800 ms3-1.2.8/docs/build/html/_modules/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15440 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/index.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.826800 ms3-1.2.8/docs/build/html/_modules/ms3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   121982 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/annotations.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   562760 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/bs4_parser.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   585871 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/corpus.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   119721 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/expand_dcml.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   299877 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/parse.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   337630 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/piece.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   326103 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/score.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   264338 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/transformations.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   930043 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/utils.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   139939 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/view.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    63215 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/re.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.826800 ms3-1.2.8/docs/build/html/_sources/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_sources/README.md.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/html/_sources/authors.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.8/docs/build/html/_sources/install.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/html/_sources/license.rst.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.830133 ms3-1.2.8/docs/build/html/_sources/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/manual/index.md.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.830133 ms3-1.2.8/docs/build/html/_sources/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/old_src/quick_old.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/quick.md.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-05-01 12:14:08.000000 ms3-1.2.8/docs/build/html/_sources/reference.rst.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.836800 ms3-1.2.8/docs/build/html/_static/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4418 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14621 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_static/basic.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4472 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/doctools.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      439 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      286 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/file.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   288580 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    89501 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/jquery.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/jupyter-sphinx.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4758 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/language_data.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/minus.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    39364 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/plus.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14668 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/pygments.css
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.836800 ms3-1.2.8/docs/build/html/_static/scripts/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    86398 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5229 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18215 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4712 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.840133 ms3-1.2.8/docs/build/html/_static/styles/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   144661 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    58614 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      106 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    68420 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19530 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/underscore.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/docs/build/html/_static/vendor/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.840133 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7427 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.840133 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   101709 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.843467 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   181264 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   105112 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60236 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24028 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   389948 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154840 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10084 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4776 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1845 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16465 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/authors.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    69269 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/changelog.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79722 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/genindex.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    31724 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19975 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/install.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    53099 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/license.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.843467 ms3-1.2.8/docs/build/html/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   338361 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/manual/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7352 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/objects.inv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.846800 ms3-1.2.8/docs/build/html/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60388 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/old_src/quick_old.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17021 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/py-modindex.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    47347 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/quick.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1763633 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/reference.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15656 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/search.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130526 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/searchindex.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.846800 ms3-1.2.8/docs/build/jupyter_execute/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.846800 ms3-1.2.8/docs/build/jupyter_execute/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   346220 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/jupyter_execute/manual/index.ipynb
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    49220 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/jupyter_execute/quick.ipynb
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/changelog.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      135 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/columns.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10588 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/conf.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   137117 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/cujus.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.850133 ms3-1.2.8/docs/examples/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      134 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/access_score_info.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       47 2021-10-16 12:40:03.000000 ms3-1.2.8/docs/examples/parse_directory.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       64 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_directory_mscx.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       58 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_directory_xml.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      199 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_key.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      173 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_other_directory.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_single_score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       71 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/index.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.8/docs/install.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/license.rst
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.850133 ms3-1.2.8/docs/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      715 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/corpus_after
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      174 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/corpus_before
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/index.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      488 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/out
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9940 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/ms3_architecture.drawio
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   218314 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/ms3_architecture.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96827 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/o_quam.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.850133 ms3-1.2.8/docs/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15949 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/old_src/quick_old.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/old_src/quick_old.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   163542 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/quae.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/quick.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-05-01 12:14:08.000000 ms3-1.2.8/docs/reference.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       86 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/requirements.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   115684 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/stabat.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.853467 ms3-1.2.8/new_tests/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7378 2023-05-02 08:27:28.000000 ms3-1.2.8/new_tests/conftest.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/new_tests/inferred_labels/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.856800 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19047 2022-12-15 11:35:36.000000 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   332296 2022-12-15 11:35:36.000000 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317949 2022-12-15 11:35:36.000000 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      466 2023-05-01 13:23:04.000000 ms3-1.2.8/new_tests/parse_script.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-05-02 08:27:28.000000 ms3-1.2.8/new_tests/test_cli.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      403 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_docs_examples.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    12424 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_extract.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6352 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3744 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      823 2023-01-17 21:52:55.000000 ms3-1.2.8/new_tests/test_transformations.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.873467 ms3-1.2.8/old_tests/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   388689 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/05_symph_fant_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      959 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/05_symph_fant_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   100539 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/05_symph_fant_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   488895 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7268 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2636 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   155973 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4361 2023-01-02 20:31:46.000000 ms3-1.2.8/old_tests/ALL_WARNINGS
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   256806 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/BWV_0815_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/BWV_0815_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/BWV_0815_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16417 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/D973deutscher01_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/D973deutscher01_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/D973deutscher01_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1490215 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      330 2023-01-02 20:31:46.000000 ms3-1.2.8/old_tests/IGNORED_WARNINGS
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   431522 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14480 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4560 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96112 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_notes.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.883467 ms3-1.2.8/old_tests/MS3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1041665 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/05_symph_fant.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1034028 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/76CASM34A33UM.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   787637 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/BWV_0815.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    54002 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/D973deutscher01.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   701525 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   807371 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/MS3/K281-3.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   259369 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/stabat_03_coloured.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      624 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/README.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      224 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/conftest.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.886800 ms3-1.2.8/old_tests/harmonies/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9855 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    21459 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3905 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/stabat_03_coloured.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.886800 ms3-1.2.8/old_tests/measures/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      889 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/05_symph_fant.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6504 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/BWV_0815.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      684 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/D973deutscher01.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2706 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4411 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/stabat_03_coloured.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5885 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/metadata.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.890133 ms3-1.2.8/old_tests/notes/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    74055 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/05_symph_fant.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   112389 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   102317 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/BWV_0815.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6173 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/D973deutscher01.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   230316 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    70952 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/stabat_03_coloured.tsv
+-rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)       45 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/parse_original.sh
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      750 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/paths1.json
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      844 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/paths2.json
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.893467 ms3-1.2.8/old_tests/repeat_dummies/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6909 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/repeat_dummies/repeats0.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6493 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/repeat_dummies/repeats1.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7376 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/repeat_dummies/repeats2.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   135170 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4822 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2207 2023-02-18 19:40:30.000000 ms3-1.2.8/old_tests/test_parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      712 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_repeats.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.900134 ms3-1.2.8/old_tests/test_results/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      921 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/05_symph_fant_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    98388 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/05_symph_fant_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7089 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/76CASM34A33UM_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2536 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/76CASM34A33UM_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   152525 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/76CASM34A33UM_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/BWV_0815_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/BWV_0815_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/D973deutscher01_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/D973deutscher01_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14099 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/K281-3_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4391 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/K281-3_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    94030 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/K281-3_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4731 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/stabat_03_coloured_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      758 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/stabat_03_coloured_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24478 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/stabat_03_coloured_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4777 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_score.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.900134 ms3-1.2.8/paper/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17950 2023-05-01 12:14:08.000000 ms3-1.2.8/paper/paper.bib
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4605 2023-05-01 12:14:08.000000 ms3-1.2.8/paper/paper.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   200690 2023-01-28 14:33:36.000000 ms3-1.2.8/paper/paper.pdf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1364 2023-05-02 15:36:47.910134 ms3-1.2.8/setup.cfg
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      567 2020-05-03 17:52:04.000000 ms3-1.2.8/setup.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.900134 ms3-1.2.8/src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:27:59.000000 ms3-1.2.8/src/__init__.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.906800 ms3-1.2.8/src/ms3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1006 2023-02-18 19:40:30.000000 ms3-1.2.8/src/ms3/__init__.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2402 2023-02-18 19:40:30.000000 ms3-1.2.8/src/ms3/_typing.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24943 2023-01-12 10:36:52.000000 ms3-1.2.8/src/ms3/annotations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41608 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/bs4_measures.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130482 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/bs4_parser.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41211 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/cli.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   151740 2023-05-02 15:30:05.000000 ms3-1.2.8/src/ms3/corpus.py
+-rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)    26692 2023-01-02 20:31:46.000000 ms3-1.2.8/src/ms3/expand_dcml.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8416 2023-01-02 20:31:46.000000 ms3-1.2.8/src/ms3/ferocious_names.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18415 2023-03-18 08:04:35.000000 ms3-1.2.8/src/ms3/logger.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15652 2023-05-02 15:30:05.000000 ms3-1.2.8/src/ms3/operations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    83765 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    82901 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/piece.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97681 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    67393 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/transformations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   219679 2023-05-02 15:33:29.000000 ms3-1.2.8/src/ms3/utils.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    29890 2023-05-02 15:30:05.000000 ms3-1.2.8/src/ms3/view.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.910134 ms3-1.2.8/src/ms3.egg-info/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/PKG-INFO
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9420 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/SOURCES.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/dependency_links.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       36 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/entry_points.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-28 13:53:29.000000 ms3-1.2.8/src/ms3.egg-info/not-zip-safe
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/requires.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        4 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/top_level.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      318 2020-05-03 17:52:04.000000 ms3-1.2.8/tox.ini
```

### Comparing `ms3-1.2.7/.coveragerc` & `ms3-1.2.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/.github/ISSUE_TEMPLATE/bug_report.md` & `ms3-1.2.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/.github/ISSUE_TEMPLATE/feature_request.md` & `ms3-1.2.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/.github/workflows/draft-pdf.yml` & `ms3-1.2.8/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/.gitignore` & `ms3-1.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/CHANGELOG.rst` & `ms3-1.2.8/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 1.2.8
+=============
+
+* operations.insert_labels_into_score() filters pieces exactly one facet to be inserted (e.g. ``labels``),
+  not a fuzzy regex (e.g., which would include ``form_labels`` in the filter)
+
 Version 1.2.7
 =============
 
 * warning files omit system-dependend information from warning headers (6764476)
 * bugfixes
 
 Version 1.2.6
```

### Comparing `ms3-1.2.7/LICENSE.txt` & `ms3-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/PKG-INFO` & `ms3-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms3
-Version: 1.2.7
+Version: 1.2.8
 Summary: A parser for annotated MuseScore 3 files.
 Home-page: https://github.com/johentsch/ms3
 Author: Johannes Hentschel
 Author-email: johannes.hentschel@epfl.ch
 License: gpl3
 Project-URL: Documentation, https://johentsch.github.io/ms3/
 Platform: any
```

### Comparing `ms3-1.2.7/README.rst` & `ms3-1.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/codemeta.json` & `ms3-1.2.8/codemeta.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/Makefile` & `ms3-1.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/_intersphinx/bs4_objects.inv` & `ms3-1.2.8/docs/_intersphinx/bs4_objects.inv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/_intersphinx/bs4_objects.txt` & `ms3-1.2.8/docs/_intersphinx/bs4_objects.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/api/modules.doctree` & `ms3-1.2.8/docs/build/.doctrees/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/api/ms3.doctree` & `ms3-1.2.8/docs/build/.doctrees/api/ms3.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/authors.doctree` & `ms3-1.2.8/docs/build/.doctrees/authors.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/changelog.doctree` & `ms3-1.2.8/docs/build/.doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/environment.pickle` & `ms3-1.2.8/docs/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/index.doctree` & `ms3-1.2.8/docs/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/install.doctree` & `ms3-1.2.8/docs/build/.doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/intro.doctree` & `ms3-1.2.8/docs/build/.doctrees/intro.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/license.doctree` & `ms3-1.2.8/docs/build/.doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/manual.doctree` & `ms3-1.2.8/docs/build/.doctrees/manual.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/.doctrees/quick.doctree` & `ms3-1.2.8/docs/build/.doctrees/quick.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/README.doctree` & `ms3-1.2.8/docs/build/doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/authors.doctree` & `ms3-1.2.8/docs/build/doctrees/authors.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/changelog.doctree` & `ms3-1.2.8/docs/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/environment.pickle` & `ms3-1.2.8/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/index.doctree` & `ms3-1.2.8/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/install.doctree` & `ms3-1.2.8/docs/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/license.doctree` & `ms3-1.2.8/docs/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/manual/index.doctree` & `ms3-1.2.8/docs/build/doctrees/manual/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/old_src/quick_old.doctree` & `ms3-1.2.8/docs/build/doctrees/old_src/quick_old.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/quick.doctree` & `ms3-1.2.8/docs/build/doctrees/quick.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/doctrees/reference.doctree` & `ms3-1.2.8/docs/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/README.html` & `ms3-1.2.8/docs/build/html/README.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/index.html` & `ms3-1.2.8/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/annotations.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/annotations.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/bs4_parser.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/bs4_parser.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/corpus.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/corpus.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/expand_dcml.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/expand_dcml.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/parse.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/parse.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/piece.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/piece.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/score.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/score.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/transformations.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/transformations.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/utils.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/utils.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/ms3/view.html` & `ms3-1.2.8/docs/build/html/_modules/ms3/view.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_modules/re.html` & `ms3-1.2.8/docs/build/html/_modules/re.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_sources/index.rst.txt` & `ms3-1.2.8/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_sources/install.rst.txt` & `ms3-1.2.8/docs/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_sources/manual/index.md.txt` & `ms3-1.2.8/docs/build/html/_sources/manual/index.md.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_sources/old_src/quick_old.rst.txt` & `ms3-1.2.8/docs/build/html/_sources/old_src/quick_old.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_sources/quick.md.txt` & `ms3-1.2.8/docs/build/html/_sources/quick.md.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_sources/reference.rst.txt` & `ms3-1.2.8/docs/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `ms3-1.2.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/basic.css` & `ms3-1.2.8/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/doctools.js` & `ms3-1.2.8/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/jquery-3.6.0.js` & `ms3-1.2.8/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/jquery.js` & `ms3-1.2.8/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/jupyter-sphinx.css` & `ms3-1.2.8/docs/build/html/_static/jupyter-sphinx.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/language_data.js` & `ms3-1.2.8/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `ms3-1.2.8/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/pygments.css` & `ms3-1.2.8/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/scripts/bootstrap.js` & `ms3-1.2.8/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `ms3-1.2.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/searchtools.js` & `ms3-1.2.8/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/sphinx_highlight.js` & `ms3-1.2.8/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/styles/bootstrap.css` & `ms3-1.2.8/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `ms3-1.2.8/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/underscore-1.13.1.js` & `ms3-1.2.8/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/underscore.js` & `ms3-1.2.8/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/_static/webpack-macros.html` & `ms3-1.2.8/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/authors.html` & `ms3-1.2.8/docs/build/html/authors.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/changelog.html` & `ms3-1.2.8/docs/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/genindex.html` & `ms3-1.2.8/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/index.html` & `ms3-1.2.8/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/install.html` & `ms3-1.2.8/docs/build/html/install.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/license.html` & `ms3-1.2.8/docs/build/html/license.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/manual/index.html` & `ms3-1.2.8/docs/build/html/manual/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/objects.inv` & `ms3-1.2.8/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/old_src/quick_old.html` & `ms3-1.2.8/docs/build/html/old_src/quick_old.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/py-modindex.html` & `ms3-1.2.8/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/quick.html` & `ms3-1.2.8/docs/build/html/quick.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/reference.html` & `ms3-1.2.8/docs/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/search.html` & `ms3-1.2.8/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/html/searchindex.js` & `ms3-1.2.8/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/jupyter_execute/manual/index.ipynb` & `ms3-1.2.8/docs/build/jupyter_execute/manual/index.ipynb`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/build/jupyter_execute/quick.ipynb` & `ms3-1.2.8/docs/build/jupyter_execute/quick.ipynb`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/conf.py` & `ms3-1.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/cujus.mscx` & `ms3-1.2.8/docs/cujus.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/index.rst` & `ms3-1.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/install.rst` & `ms3-1.2.8/docs/install.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/manual/corpus_after` & `ms3-1.2.8/docs/manual/corpus_after`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/manual/index.md` & `ms3-1.2.8/docs/manual/index.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/ms3_architecture.drawio` & `ms3-1.2.8/docs/ms3_architecture.drawio`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/ms3_architecture.png` & `ms3-1.2.8/docs/ms3_architecture.png`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/o_quam.mscx` & `ms3-1.2.8/docs/o_quam.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/old_src/quick_old.md` & `ms3-1.2.8/docs/old_src/quick_old.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/old_src/quick_old.rst` & `ms3-1.2.8/docs/old_src/quick_old.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/quae.mscx` & `ms3-1.2.8/docs/quae.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/quick.md` & `ms3-1.2.8/docs/quick.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/reference.rst` & `ms3-1.2.8/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/docs/stabat.mscx` & `ms3-1.2.8/docs/stabat.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/conftest.py` & `ms3-1.2.8/new_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv` & `ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv` & `ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv` & `ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/test_cli.py` & `ms3-1.2.8/new_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/test_extract.py` & `ms3-1.2.8/new_tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/test_parse.py` & `ms3-1.2.8/new_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/test_score.py` & `ms3-1.2.8/new_tests/test_score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/new_tests/test_transformations.py` & `ms3-1.2.8/new_tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/05_symph_fant_events.tsv` & `ms3-1.2.8/old_tests/05_symph_fant_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/05_symph_fant_measures.tsv` & `ms3-1.2.8/old_tests/05_symph_fant_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/05_symph_fant_notes.tsv` & `ms3-1.2.8/old_tests/05_symph_fant_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/76CASM34A33UM_events.tsv` & `ms3-1.2.8/old_tests/76CASM34A33UM_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/76CASM34A33UM_labels.tsv` & `ms3-1.2.8/old_tests/76CASM34A33UM_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/76CASM34A33UM_measures.tsv` & `ms3-1.2.8/old_tests/76CASM34A33UM_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/76CASM34A33UM_notes.tsv` & `ms3-1.2.8/old_tests/76CASM34A33UM_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/ALL_WARNINGS` & `ms3-1.2.8/old_tests/ALL_WARNINGS`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/BWV_0815_events.tsv` & `ms3-1.2.8/old_tests/BWV_0815_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/BWV_0815_measures.tsv` & `ms3-1.2.8/old_tests/BWV_0815_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/BWV_0815_notes.tsv` & `ms3-1.2.8/old_tests/BWV_0815_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/D973deutscher01_events.tsv` & `ms3-1.2.8/old_tests/D973deutscher01_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/D973deutscher01_measures.tsv` & `ms3-1.2.8/old_tests/D973deutscher01_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/D973deutscher01_notes.tsv` & `ms3-1.2.8/old_tests/D973deutscher01_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv` & `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv` & `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv` & `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv` & `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/K281-3_events.tsv` & `ms3-1.2.8/old_tests/K281-3_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/K281-3_labels.tsv` & `ms3-1.2.8/old_tests/K281-3_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/K281-3_measures.tsv` & `ms3-1.2.8/old_tests/K281-3_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/K281-3_notes.tsv` & `ms3-1.2.8/old_tests/K281-3_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/MS3/05_symph_fant.mscx` & `ms3-1.2.8/old_tests/MS3/05_symph_fant.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/MS3/76CASM34A33UM.mscx` & `ms3-1.2.8/old_tests/MS3/76CASM34A33UM.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/MS3/BWV_0815.mscx` & `ms3-1.2.8/old_tests/MS3/BWV_0815.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/MS3/D973deutscher01.mscx` & `ms3-1.2.8/old_tests/MS3/D973deutscher01.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx` & `ms3-1.2.8/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/MS3/K281-3.mscx` & `ms3-1.2.8/old_tests/MS3/K281-3.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/MS3/stabat_03_coloured.mscx` & `ms3-1.2.8/old_tests/MS3/stabat_03_coloured.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/README.md` & `ms3-1.2.8/old_tests/README.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/harmonies/76CASM34A33UM.tsv` & `ms3-1.2.8/old_tests/harmonies/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.8/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/harmonies/K281-3.tsv` & `ms3-1.2.8/old_tests/harmonies/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/harmonies/stabat_03_coloured.tsv` & `ms3-1.2.8/old_tests/harmonies/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/measures/05_symph_fant.tsv` & `ms3-1.2.8/old_tests/measures/05_symph_fant.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/measures/76CASM34A33UM.tsv` & `ms3-1.2.8/old_tests/measures/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/measures/BWV_0815.tsv` & `ms3-1.2.8/old_tests/measures/BWV_0815.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/measures/D973deutscher01.tsv` & `ms3-1.2.8/old_tests/measures/D973deutscher01.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.8/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/measures/K281-3.tsv` & `ms3-1.2.8/old_tests/measures/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/measures/stabat_03_coloured.tsv` & `ms3-1.2.8/old_tests/measures/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/metadata.tsv` & `ms3-1.2.8/old_tests/metadata.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/notes/05_symph_fant.tsv` & `ms3-1.2.8/old_tests/notes/05_symph_fant.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/notes/76CASM34A33UM.tsv` & `ms3-1.2.8/old_tests/notes/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/notes/BWV_0815.tsv` & `ms3-1.2.8/old_tests/notes/BWV_0815.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/notes/D973deutscher01.tsv` & `ms3-1.2.8/old_tests/notes/D973deutscher01.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.8/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/notes/K281-3.tsv` & `ms3-1.2.8/old_tests/notes/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/notes/stabat_03_coloured.tsv` & `ms3-1.2.8/old_tests/notes/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/paths1.json` & `ms3-1.2.8/old_tests/paths1.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/paths2.json` & `ms3-1.2.8/old_tests/paths2.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/repeat_dummies/repeats0.mscx` & `ms3-1.2.8/old_tests/repeat_dummies/repeats0.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/repeat_dummies/repeats1.mscx` & `ms3-1.2.8/old_tests/repeat_dummies/repeats1.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/repeat_dummies/repeats2.mscx` & `ms3-1.2.8/old_tests/repeat_dummies/repeats2.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/stabat_03_coloured_events.tsv` & `ms3-1.2.8/old_tests/stabat_03_coloured_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/stabat_03_coloured_labels.tsv` & `ms3-1.2.8/old_tests/stabat_03_coloured_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/stabat_03_coloured_measures.tsv` & `ms3-1.2.8/old_tests/stabat_03_coloured_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/stabat_03_coloured_notes.tsv` & `ms3-1.2.8/old_tests/stabat_03_coloured_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_parse.py` & `ms3-1.2.8/old_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_repeats.py` & `ms3-1.2.8/old_tests/test_repeats.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/05_symph_fant_measures.tsv` & `ms3-1.2.8/old_tests/test_results/05_symph_fant_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/05_symph_fant_notes.tsv` & `ms3-1.2.8/old_tests/test_results/05_symph_fant_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/76CASM34A33UM_labels.tsv` & `ms3-1.2.8/old_tests/test_results/76CASM34A33UM_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/76CASM34A33UM_measures.tsv` & `ms3-1.2.8/old_tests/test_results/76CASM34A33UM_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/76CASM34A33UM_notes.tsv` & `ms3-1.2.8/old_tests/test_results/76CASM34A33UM_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/BWV_0815_measures.tsv` & `ms3-1.2.8/old_tests/test_results/BWV_0815_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/BWV_0815_notes.tsv` & `ms3-1.2.8/old_tests/test_results/BWV_0815_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/D973deutscher01_measures.tsv` & `ms3-1.2.8/old_tests/test_results/D973deutscher01_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/D973deutscher01_notes.tsv` & `ms3-1.2.8/old_tests/test_results/D973deutscher01_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv` & `ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv` & `ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv` & `ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/K281-3_labels.tsv` & `ms3-1.2.8/old_tests/test_results/K281-3_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/K281-3_measures.tsv` & `ms3-1.2.8/old_tests/test_results/K281-3_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/K281-3_notes.tsv` & `ms3-1.2.8/old_tests/test_results/K281-3_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/stabat_03_coloured_labels.tsv` & `ms3-1.2.8/old_tests/test_results/stabat_03_coloured_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/stabat_03_coloured_measures.tsv` & `ms3-1.2.8/old_tests/test_results/stabat_03_coloured_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_results/stabat_03_coloured_notes.tsv` & `ms3-1.2.8/old_tests/test_results/stabat_03_coloured_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/old_tests/test_score.py` & `ms3-1.2.8/old_tests/test_score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/paper/paper.bib` & `ms3-1.2.8/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/paper/paper.md` & `ms3-1.2.8/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/paper/paper.pdf` & `ms3-1.2.8/paper/paper.pdf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/setup.cfg` & `ms3-1.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/setup.py` & `ms3-1.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/__init__.py` & `ms3-1.2.8/src/ms3/__init__.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/_typing.py` & `ms3-1.2.8/src/ms3/_typing.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/annotations.py` & `ms3-1.2.8/src/ms3/annotations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/bs4_measures.py` & `ms3-1.2.8/src/ms3/bs4_measures.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/bs4_parser.py` & `ms3-1.2.8/src/ms3/bs4_parser.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/cli.py` & `ms3-1.2.8/src/ms3/cli.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/corpus.py` & `ms3-1.2.8/src/ms3/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -2123,15 +2123,15 @@
             |   MuseScore will split and encode those beginning with a note name ( resulting in ms3-internal harmony_layer 3).
             | * 1 the labels are written into the staff's layer for Roman Numeral Analysis.
             | * 2 to have MuseScore interpret them as Nashville Numbers
         check_for_clashes : :obj:`bool`, optional
             By default, warnings are thrown when there already exists a label at a position (and in a notational
             layer) where a new one is attached. Pass False to deactivate these warnings.
         """
-        reached, goal = 0, 0
+        reached, goal, i = 0, 0, 0
         for i, (file, score) in enumerate(self.iter_parsed('scores', view_name=view_name), 1):
             r, g = score.attach_labels(key, staff=staff, voice=voice, harmony_layer=harmony_layer, check_for_clashes=check_for_clashes)
             self.logger.debug(f"{r}/{g} labels successfully added to {file}")
             reached += r
             goal += g
         self.logger.info(f"{reached}/{goal} labels successfully added to {i} files.")
         return reached, goal
```

### Comparing `ms3-1.2.7/src/ms3/expand_dcml.py` & `ms3-1.2.8/src/ms3/expand_dcml.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/ferocious_names.txt` & `ms3-1.2.8/src/ms3/ferocious_names.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/logger.py` & `ms3-1.2.8/src/ms3/logger.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/operations.py` & `ms3-1.2.8/src/ms3/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
           layer) where a new one is attached. Pass False to deactivate these warnings.
       print_info:
           By default, the ms3_object is displayed before and after parsing. Pass False to prevent this,
           for example when the object has many, many files.
     """
     logger = get_logger('ms3.add')
     facet = check_argument_against_literal_type(facet, AnnotationsFacet, logger=logger)
-    ms3_object.view.include('facets', 'scores', facet)
+    ms3_object.view.include('facets', 'scores', f"^{facet}$")
     ms3_object.disambiguate_facet(facet, ask_for_input=ask_for_input)
     ms3_object.disambiguate_facet('scores', ask_for_input=ask_for_input)
     ms3_object.view.fnames_with_incomplete_facets = False
     obj_name = type(ms3_object).__name__.upper()
     if print_info:
         print(f"VIEW ON THE {obj_name} BEFORE PARSING:")
         ms3_object.info()
```

### Comparing `ms3-1.2.7/src/ms3/parse.py` & `ms3-1.2.8/src/ms3/parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/piece.py` & `ms3-1.2.8/src/ms3/piece.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/score.py` & `ms3-1.2.8/src/ms3/score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/transformations.py` & `ms3-1.2.8/src/ms3/transformations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.7/src/ms3/utils.py` & `ms3-1.2.8/src/ms3/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 00000420: 7064 6174 655f 6366 672c 204c 6f67 4361  pdate_cfg, LogCa
 00000430: 7074 7572 6572 0a66 726f 6d20 2e5f 7479  pturer.from ._ty
 00000440: 7069 6e67 2069 6d70 6f72 7420 4669 6c65  ping import File
 00000450: 4469 6374 2c20 4661 6365 742c 2056 6965  Dict, Facet, Vie
 00000460: 7744 6963 742c 2046 696c 6544 6174 6166  wDict, FileDataf
 00000470: 7261 6d65 5475 706c 654d 6179 6265 0a0a  rameTupleMaybe..
 00000480: 4d53 335f 5645 5253 494f 4e20 3d20 2731  MS3_VERSION = '1
-00000490: 2e32 2e37 270a 4c41 5445 5354 5f4d 5553  .2.7'.LATEST_MUS
+00000490: 2e32 2e38 270a 4c41 5445 5354 5f4d 5553  .2.8'.LATEST_MUS
 000004a0: 4553 434f 5245 5f56 4552 5349 4f4e 203d  ESCORE_VERSION =
 000004b0: 2027 332e 362e 3227 0a43 4f4d 5055 5445   '3.6.2'.COMPUTE
 000004c0: 445f 4d45 5441 4441 5441 5f43 4f4c 554d  D_METADATA_COLUM
 000004d0: 4e53 203d 205b 2754 696d 6553 6967 272c  NS = ['TimeSig',
 000004e0: 2027 4b65 7953 6967 272c 2027 6c61 7374   'KeySig', 'last
 000004f0: 5f6d 6327 2c20 276c 6173 745f 6d6e 272c  _mc', 'last_mn',
 00000500: 2027 6c65 6e67 7468 5f71 6227 2c20 276c   'length_qb', 'l
```

### Comparing `ms3-1.2.7/src/ms3/view.py` & `ms3-1.2.8/src/ms3/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,37 +421,37 @@
             print(msg)
             return
         if not self.fnames_in_metadata:
             msg_components.append("excludes fnames that are contained in the metadata")
         if not self.fnames_not_in_metadata:
             msg_components.append("excludes fnames that are not contained in the metadata")
         if not self.fnames_with_incomplete_facets:
-            msg_components.append("excludes pieces that do not have at least one file per selected facet")
+            msg_components.append(f"excludes pieces that do not have at least one file per selected facet ({', '.join(self.selected_facets)})")
         if not self.include_convertible:
             msg_components.append("filters out file extensions requiring conversion (such as .xml)")
         if not self.include_tsv:
             msg_components.append("disregards all TSV files")
         if self.exclude_review:
             msg_components.append("excludes review files and folders")
         included_re = {what_to_include: [rgx for rgx in regexes if rgx not in self.registered_regexes]
                        for what_to_include, regexes in self.including.items()}
         excluded_re = {what_to_exclude: [rgx for rgx in regexes if rgx not in self.registered_regexes]
                        for what_to_exclude, regexes in self.excluding.items()}
-        for what_to_exclude, re_strings in included_re.items():
+        for what_to_include, re_strings in included_re.items():
             n_included = len(re_strings)
             if n_included == 0:
                 continue
             if n_included == 1:
                 included = f"'{re_strings[0]}'"
             elif n_included < 11:
                 included = 'one of ' + str(re_strings)
             else:
                 included = 'one of [' + ', '.join(f"'{regex}'" for regex in re_strings[:10]) + '... '
                 included += f" ({n_included - 10} more, see filtering_report()))"
-            msg_components.append(f"includes only {what_to_exclude} containing {included}")
+            msg_components.append(f"includes only {what_to_include} containing {included}")
         for what_to_exclude, re_strings in excluded_re.items():
             n_excluded = len(re_strings)
             if n_excluded == 0:
                 continue
             if n_excluded == 1:
                 excluded = f"'{re_strings[0]}'"
             elif n_excluded < 11:
```

### Comparing `ms3-1.2.7/src/ms3.egg-info/PKG-INFO` & `ms3-1.2.8/src/ms3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms3
-Version: 1.2.7
+Version: 1.2.8
 Summary: A parser for annotated MuseScore 3 files.
 Home-page: https://github.com/johentsch/ms3
 Author: Johannes Hentschel
 Author-email: johannes.hentschel@epfl.ch
 License: gpl3
 Project-URL: Documentation, https://johentsch.github.io/ms3/
 Platform: any
```

### Comparing `ms3-1.2.7/src/ms3.egg-info/SOURCES.txt` & `ms3-1.2.8/src/ms3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

