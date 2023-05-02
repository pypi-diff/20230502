# Comparing `tmp/nlptoolssna-0.5.0.tar.gz` & `tmp/nlptoolssna-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.5.0.tar", last modified: Tue May  2 19:26:30 2023, max compression
+gzip compressed data, was "nlptoolssna-0.5.1.tar", last modified: Tue May  2 19:34:32 2023, max compression
```

## Comparing `nlptoolssna-0.5.0.tar` & `nlptoolssna-0.5.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.276736 nlptoolssna-0.5.0/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-02 19:26:30.277764 nlptoolssna-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:29.983683 nlptoolssna-0.5.0/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:29.915951 nlptoolssna-0.5.0/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:29.916945 nlptoolssna-0.5.0/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:29.992516 nlptoolssna-0.5.0/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.0/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.029826 nlptoolssna-0.5.0/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.0/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.0/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.0/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.0/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.064681 nlptoolssna-0.5.0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.070503 nlptoolssna-0.5.0/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.0/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.085700 nlptoolssna-0.5.0/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.088702 nlptoolssna-0.5.0/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.0/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.0/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.097739 nlptoolssna-0.5.0/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.0/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.0/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.5.0/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.0/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.5.0/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.0/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.111825 nlptoolssna-0.5.0/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.118674 nlptoolssna-0.5.0/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.0/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.0/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.147505 nlptoolssna-0.5.0/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.0/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.0/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.0/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.0/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.0/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.0/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.150501 nlptoolssna-0.5.0/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.0/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.159569 nlptoolssna-0.5.0/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.0/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.5.0/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.213736 nlptoolssna-0.5.0/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.0/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.0/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     8072 2023-05-02 19:26:08.000000 nlptoolssna-0.5.0/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.0/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.0/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.225522 nlptoolssna-0.5.0/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.0/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.5.0/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.236402 nlptoolssna-0.5.0/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.0/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.0/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.0/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.261649 nlptoolssna-0.5.0/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-02 19:26:29.000000 nlptoolssna-0.5.0/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-05-02 19:26:29.000000 nlptoolssna-0.5.0/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:26:29.000000 nlptoolssna-0.5.0/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-02 19:26:29.000000 nlptoolssna-0.5.0/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.0/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-02 19:26:29.000000 nlptoolssna-0.5.0/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 19:26:29.000000 nlptoolssna-0.5.0/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-02 19:26:30.279509 nlptoolssna-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:26:30.273301 nlptoolssna-0.5.0/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.0/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.062274 nlptoolssna-0.5.1/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-02 19:34:32.063271 nlptoolssna-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.896322 nlptoolssna-0.5.1/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.5.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.846323 nlptoolssna-0.5.1/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.851442 nlptoolssna-0.5.1/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.897320 nlptoolssna-0.5.1/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.1/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.903324 nlptoolssna-0.5.1/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.1/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.5.1/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.1/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.5.1/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.5.1/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.927290 nlptoolssna-0.5.1/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.928407 nlptoolssna-0.5.1/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.5.1/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.931407 nlptoolssna-0.5.1/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.933406 nlptoolssna-0.5.1/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.5.1/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.5.1/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.934404 nlptoolssna-0.5.1/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.5.1/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.5.1/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.5.1/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.5.1/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.5.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.5.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.5.1/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.938407 nlptoolssna-0.5.1/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.941530 nlptoolssna-0.5.1/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.5.1/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.5.1/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:31.955245 nlptoolssna-0.5.1/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.5.1/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.5.1/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.5.1/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.5.1/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.5.1/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.5.1/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.001057 nlptoolssna-0.5.1/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.5.1/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.008680 nlptoolssna-0.5.1/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.5.1/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.5.1/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.026244 nlptoolssna-0.5.1/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.5.1/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.5.1/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     8000 2023-05-02 19:34:19.000000 nlptoolssna-0.5.1/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.5.1/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.5.1/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.029475 nlptoolssna-0.5.1/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.5.1/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.5.1/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.032999 nlptoolssna-0.5.1/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.5.1/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.5.1/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.5.1/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.056284 nlptoolssna-0.5.1/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-02 19:34:31.000000 nlptoolssna-0.5.1/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-05-02 19:34:31.000000 nlptoolssna-0.5.1/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:34:31.000000 nlptoolssna-0.5.1/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-02 19:34:31.000000 nlptoolssna-0.5.1/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.5.1/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-02 19:34:31.000000 nlptoolssna-0.5.1/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 19:34:31.000000 nlptoolssna-0.5.1/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-02 19:34:32.064273 nlptoolssna-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:34:32.061310 nlptoolssna-0.5.1/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.5.1/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.5.0/CONTRIBUTING.rst` & `nlptoolssna-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/LICENSE` & `nlptoolssna-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/PKG-INFO` & `nlptoolssna-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.0/README.rst` & `nlptoolssna-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/docs/Makefile` & `nlptoolssna-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/docs/build/html/_images/download.png` & `nlptoolssna-0.5.1/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/docs/build/html/_static/download.png` & `nlptoolssna-0.5.1/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/docs/make.bat` & `nlptoolssna-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/docs/source/_static/download.png` & `nlptoolssna-0.5.1/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/docs/source/conf.py` & `nlptoolssna-0.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/docs/source/installation.rst` & `nlptoolssna-0.5.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.5.1/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/arabiner/data.py` & `nlptoolssna-0.5.1/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/arabiner/datasets.py` & `nlptoolssna-0.5.1/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/arabiner/helpers.py` & `nlptoolssna-0.5.1/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/arabiner/infer.py` & `nlptoolssna-0.5.1/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/arabiner/transforms.py` & `nlptoolssna-0.5.1/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/data/my_data.pickle` & `nlptoolssna-0.5.1/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.5.1/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/morphology/charsets.py` & `nlptoolssna-0.5.1/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.5.1/nlptools/morphology/morph_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,32 +120,32 @@
          if result_token != []:
                
                output_list.append(result_token)
          else:
             # if no solution is found
             output_list.append(solution)
         
-   output_list=filter_results(task, output_list)
-   return output_list 
+   return filter_results(task, output_list)
+   
 
 
 def _is_ar(word):
     return _IS_AR_RE.match(word) is not None
 
 
-def filter_results(task, output_list):
+def filter_results(task, lst):
     if task == 'lemmatizer':
               #[token, token+"_0",""]
-              [i.pop(2) for i in output_list]
-              return output_list
+              [i.pop(2) for i in lst]
+              return lst
     elif task == 'pos':
-              [i.pop(1) for i in output_list]
-              return output_list
+              [i.pop(1) for i in lst]
+              return lst
     else: 
-          return output_list         
+          return lst         
         
 # def tagger(text: str, task = 'full', language = 'MSA'):
 
 #     """
 #     This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
 #     There is no limit for the text size, but one should be resonable based on the available resources (computational power).
```

### Comparing `nlptoolssna-0.5.0/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.5.1/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/parse/parser.py` & `nlptoolssna-0.5.1/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/salma/implication.py` & `nlptoolssna-0.5.1/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.5.1/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.5.1/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.5.0/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.5.1/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/setup.cfg` & `nlptoolssna-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.5.0/setup.py` & `nlptoolssna-0.5.1/setup.py`

 * *Files identical despite different names*

