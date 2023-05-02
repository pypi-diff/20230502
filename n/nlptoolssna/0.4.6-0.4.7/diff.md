# Comparing `tmp/nlptoolssna-0.4.6.tar.gz` & `tmp/nlptoolssna-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.4.6.tar", last modified: Mon May  1 12:52:33 2023, max compression
+gzip compressed data, was "nlptoolssna-0.4.7.tar", last modified: Tue May  2 17:28:57 2023, max compression
```

## Comparing `nlptoolssna-0.4.6.tar` & `nlptoolssna-0.4.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.788303 nlptoolssna-0.4.6/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-01 12:52:33.788303 nlptoolssna-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.719628 nlptoolssna-0.4.6/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.6/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.697225 nlptoolssna-0.4.6/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.698225 nlptoolssna-0.4.6/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.720631 nlptoolssna-0.4.6/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.6/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.726206 nlptoolssna-0.4.6/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.6/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.6/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.6/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.6/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.734206 nlptoolssna-0.4.6/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.735205 nlptoolssna-0.4.6/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.6/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.737204 nlptoolssna-0.4.6/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.739204 nlptoolssna-0.4.6/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.4.6/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.4.6/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.740204 nlptoolssna-0.4.6/docs/source/api/morph/
--rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.4.6/docs/source/api/morph/morph_tagger.rst
--rw-rw-rw-   0        0        0      208 2023-05-01 09:05:51.000000 nlptoolssna-0.4.6/docs/source/api/morph.rst
--rw-rw-rw-   0        0        0      161 2023-05-01 11:08:00.000000 nlptoolssna-0.4.6/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.6/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.6/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.6/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.6/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.744671 nlptoolssna-0.4.6/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.747673 nlptoolssna-0.4.6/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.6/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4019 2023-05-01 11:12:31.000000 nlptoolssna-0.4.6/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.754835 nlptoolssna-0.4.6/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.6/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.6/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.6/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.6/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.6/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.4.6/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.755879 nlptoolssna-0.4.6/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.6/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.760022 nlptoolssna-0.4.6/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.6/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.6/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.767022 nlptoolssna-0.4.6/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.4.6/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.6/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     7939 2023-05-01 12:37:15.000000 nlptoolssna-0.4.6/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.6/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.4.6/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.769021 nlptoolssna-0.4.6/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.6/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.6/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.772193 nlptoolssna-0.4.6/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.6/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.6/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.4.6/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.784193 nlptoolssna-0.4.6/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-01 12:52:33.000000 nlptoolssna-0.4.6/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2023-05-01 12:52:33.000000 nlptoolssna-0.4.6/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:52:33.000000 nlptoolssna-0.4.6/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-01 12:52:33.000000 nlptoolssna-0.4.6/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.6/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-01 12:52:33.000000 nlptoolssna-0.4.6/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 12:52:33.000000 nlptoolssna-0.4.6/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-01 12:52:33.789301 nlptoolssna-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:52:33.787280 nlptoolssna-0.4.6/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.6/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.661973 nlptoolssna-0.4.7/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.7/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.618506 nlptoolssna-0.4.7/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.618506 nlptoolssna-0.4.7/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.661973 nlptoolssna-0.4.7/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.7/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.669987 nlptoolssna-0.4.7/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.7/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.7/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.7/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.7/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.686735 nlptoolssna-0.4.7/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.686735 nlptoolssna-0.4.7/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.7/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.695137 nlptoolssna-0.4.7/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.695137 nlptoolssna-0.4.7/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.4.7/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.4.7/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.695137 nlptoolssna-0.4.7/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      142 2023-05-02 17:27:34.000000 nlptoolssna-0.4.7/docs/source/api/morphology/morph_tagger.rst
+-rw-rw-rw-   0        0        0      213 2023-05-02 17:28:00.000000 nlptoolssna-0.4.7/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.4.7/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.7/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.7/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.703608 nlptoolssna-0.4.7/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.703608 nlptoolssna-0.4.7/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.7/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4019 2023-05-01 11:12:31.000000 nlptoolssna-0.4.7/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.720626 nlptoolssna-0.4.7/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.7/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.7/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.7/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.7/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.7/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.4.7/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.720626 nlptoolssna-0.4.7/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.7/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.720626 nlptoolssna-0.4.7/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.7/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.7/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.737295 nlptoolssna-0.4.7/nlptools/morphology/
+-rw-rw-rw-   0        0        0      372 2023-05-02 13:24:43.000000 nlptoolssna-0.4.7/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.7/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     7538 2023-05-02 15:30:16.000000 nlptoolssna-0.4.7/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.7/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.4.7/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.737295 nlptoolssna-0.4.7/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.7/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.7/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.745279 nlptoolssna-0.4.7/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.7/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.7/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.4.7/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.753895 nlptoolssna-0.4.7/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1616 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.4.6/CONTRIBUTING.rst` & `nlptoolssna-0.4.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/LICENSE` & `nlptoolssna-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/PKG-INFO` & `nlptoolssna-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.6/README.rst` & `nlptoolssna-0.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/docs/Makefile` & `nlptoolssna-0.4.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/docs/build/html/_images/download.png` & `nlptoolssna-0.4.7/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/docs/build/html/_static/download.png` & `nlptoolssna-0.4.7/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/docs/make.bat` & `nlptoolssna-0.4.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/docs/source/_static/download.png` & `nlptoolssna-0.4.7/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/docs/source/conf.py` & `nlptoolssna-0.4.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/docs/source/installation.rst` & `nlptoolssna-0.4.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.4.7/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/arabiner/data.py` & `nlptoolssna-0.4.7/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/arabiner/datasets.py` & `nlptoolssna-0.4.7/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/arabiner/helpers.py` & `nlptoolssna-0.4.7/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/arabiner/infer.py` & `nlptoolssna-0.4.7/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/arabiner/transforms.py` & `nlptoolssna-0.4.7/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/data/my_data.pickle` & `nlptoolssna-0.4.7/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.4.7/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/morph/charsets.py` & `nlptoolssna-0.4.7/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.4.7/nlptools/morphology/morph_analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,180 +1,180 @@
 import pickle
-from nlptools.morph import settings 
+from nlptools.morphology import settings 
 import re
-from nlptools.morph.tokenizers_words import simple_word_tokenize
+from nlptools.morphology.tokenizers_words import simple_word_tokenize
 from nlptools.parse.parser import arStrip
 import os.path
 from nlptools.DataDownload import downloader
 
-def load_ALMA_dic():
-   # Open the Pickle file in binary mode
-    filename = 'ALMA27012000.pickle'
-    path =downloader.get_appdatadir()
-    file_path = os.path.join(path, filename)
+# def load_ALMA_dic():
+#    # Open the Pickle file in binary mode
+#     filename = 'ALMA27012000.pickle'
+#     path =downloader.get_appdatadir()
+#     file_path = os.path.join(path, filename)
     
 
-    with open(file_path, 'rb') as f:
-       #Load the serialized data from the file
-       ALMA_dic = pickle.load(f)
-       #print(ALMA_dic)
-       return ALMA_dic
+#     with open(file_path, 'rb') as f:
+#        #Load the serialized data from the file
+#        ALMA_dic = pickle.load(f)
+#        #print(ALMA_dic)
+#        return ALMA_dic
 
-def tag(token, language, task):
+def find_solution(token, language, task):
     """
-    Given a token, this method retrives the morphological solutions [token, lemma, pos, frequency, task and language] filterd by spesific language and task.
+    Given a token, this method finds the morphological solution lemma and/or pos based on a spesific language and task.
           
     Args:
-        - token (:obj:`str`): The Arabic token to be morphologcaly tagged.
-        - language (:obj:`str`): The language to filter the results by [MSA, Pal, Lebanese, Iraqi, Libyan, Syrian, Sudanese, Yemeni]. The defualt task if not specisifd is `MSA`.
-        - task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specisifd is `full`.
+        - token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
+        - language (:obj:`str`): In the current version, `MSA` is only supported. 
+        - task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
 
     Returns:
-        list (:obj:`list`): A list of [token, lemma, pos_ar, lemma_freq, language, task], where:
+        list (:obj:`list`): A list of [token, lemma, pos], where:
             - token: the original input token
-            - lemma: the lemma of the token
-            - pos_ar: the part of speech of the token in Arabic
-            - lemma_freq: the frequency of the lemma in the dictionary
-            - language: the input language 
-            - task: the input task 
-
+            - lemma: the lemma of the token 
+            - pos: the part-of-speech of the token 
             If no sloution is found for this token, an empty list is returned.
     """
     if token in settings.div_dic.keys():
-
-        soluation =settings.div_dic[token][1]
-        if task =='full' and soluation[-2] == language:
-            return  [token, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
-        elif soluation[-2] == language and soluation[-1] ==task:
-            return [token, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
+        soluation =settings.div_dic[token]
+        if task =='full' :          
+            return  [token, soluation[0], soluation[1]]               
+        elif  task == 'pos':                       
+            return  [token, soluation[1]]
+        elif  task == 'lemmatizer':                       
+            return  [token, soluation[0]]       
         return []
     else:
         return []
 
-def analyze_morphology(text ,language, task):
+def analyze(text, language ='MSA', task ='full'):
    """
     This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that,
     if:
          - the task is lemmatizer, then the morphological soltuion is only the lemma.
          - the task is pos, then the morphological soltuion is only the pos.
          - the task is full, the the morphological soltuion is both the lemma and the pos.
      
-    The language argument helps the morphological analysis to return more accurate solutions based on the specific variety of Arabic used in the input text, including MSA and various dialects such as Pal, Lebanese, Iraqi, Libyan, Syrian, Sudanese, and Yemeni. 
-
     Args:
-         - text (:obj:`str`): The input text to be morphologicaly analyzed.
-         - language (:obj:`str`): The language of the input text including MSA and various dialects such as Pal, Lebanese, Iraqi, Libyan, Syrian, Sudanese, and Yemeni.
-         - task (:obj:`str`): The type of task being performed (e.g., `lemmatizer`, `pos`, or `full`).
+        - token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
+        - language (:obj:`str`): In the current version, `MSA` is only supported. 
+        - task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specified is `full`.
          
     Returns:
-          - output_list (:obj:`list`): A list of morphological solution for each token in the input text.
-    """
+        list (:obj:`list`): A list of [token, lemma, pos], based on the spesified task, where:
+            - token: the original input token
+            - lemma: the lemma of the token 
+            - pos: the part-of-speech of the token 
 
+    """
+  
+   #@check if the init does not load data correctly, call load_alma inside
    output_list = []
-   # tokenize sentence into words
+
    tokens = simple_word_tokenize(text)
 
-   # for each token 
    for token in tokens:
          result_token =[]
-         # Trim spaces 
-         token = token.strip()
-         # Remove smallDiac
          token = arStrip(token , False , True , False , False , False , False) 
-         # Unify ٱ 
          token = re.sub('[ٱ]','ﺍ',token)
 
-         # Initialize solution [token, lemma, pos]
-         solution =[token, token+"_0", 0,  "", ""]
-         
-         # if token is digit, update pos to be digit 
+         if task == 'lemmatizer':
+             solution =[token, token+"_0"]
+         elif task == 'pos':
+             solution=[token, ""]
+         else: 
+             solution=[token, token+"_0",""]
+
          if token.isdigit():
-            solution[2] = "digit"
+            solution[2] = "digit" #pos
 
-         # if token is english, update pos to be ENGLISH
-         elif re.match("^[a-zA-Z]*$", token):
-            solution[2] = "ENGLISH"
+
+         elif re.match("^[a-zA-Z]*$", token): 
+            solution[2] = "Foreign" #pos
 
          else:
-            # search for a token (as is) in the dictionary   
-            result_token = tag(token,language, task)
+            result_token = find_solution(token,language, task)
             
-            if len(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token))) > 5 and result_token == []:
-               # try with remove AL
-               result_token = tag(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token)), language, task)
+           
+            if result_token == []:
+               token_without_al = re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token))
+               if len(token_without_al) > 5  :
+                  result_token = find_solution(token_without_al, language, task)
 
             if result_token == []:
               # try with replace ﻩ with ﺓ
-               result_token = tag(re.sub(r'[ﻩ]$','ﺓ',token), language, task)
+               result_token = find_solution(re.sub(r'[ﻩ]$','ﺓ',token), language, task)
+               
 
             if result_token == []:
                # try with unify Alef
                word_with_unify_alef = arStrip(token , False , False , False , False , True , False) # Unify Alef
-               result_token = tag(word_with_unify_alef, language, task)
+               result_token = find_solution(word_with_unify_alef, language, task)
             
             if result_token == []:
                # try with remove diac
                word_undiac = arStrip(token , True , False , True , True , False , False) # remove diacs, shaddah ,  digit
-               result_token = tag(word_undiac, language, task)
+               result_token = find_solution(word_undiac, language, task)
 
             if result_token == []:
                # try with remove diac and unify alef
                word_undiac = arStrip(token , True , True , True , False, True , False) # diacs , smallDiacs , shaddah ,  alif
-               result_token = tag(word_undiac, language, task)
+               result_token = find_solution(word_undiac, language, task)
 
          if result_token != []:
                output_list.append(result_token)
          else:
             # if no solution is found
             output_list.append(solution)
 
    return output_list               
         
-def tagger(text: str, task = 'full', language = 'MSA'):
+# def tagger(text: str, task = 'full', language = 'MSA'):
 
-    """
-    This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
-    There is no limit for the text size, but one should be resonable based on the available resources (computational power).
+#     """
+#     This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
+#     There is no limit for the text size, but one should be resonable based on the available resources (computational power).
     
-        Args:
-            - text (:obj:`str`): The input Arabic text to be morphologically analyzed and tagged.
-            - task (:obj:`str`): The type of morphological analysis and tagging to be performed (the default is `full`).
-            - language (:obj:`str`): The language of the input text (the default is 'MSA' (Modern Standard Arabic)).
+#         Args:
+#             - text (:obj:`str`): The input Arabic text to be morphologically analyzed and tagged.
+#             - task (:obj:`str`): The type of morphological analysis and tagging to be performed (the default is `full`).
+#             - language (:obj:`str`): The language of the input text (the default is 'MSA' (Modern Standard Arabic)).
         
-    Returns:
-           - output_list list(:obj:`list`): A list of lists, where each sublist contains information about a token in the input text, including the original token, its lemma, its part of speech (POS) tag, its lemma frequency, the task and the language.
+#     Returns:
+#            - output_list list(:obj:`list`): A list of lists, where each sublist contains information about a token in the input text, including the original token, its lemma, its part of speech (POS) tag, its lemma frequency, the task and the language.
 
-    **Example:**
+#     **Example:**
 
-    .. highlight:: python
-    .. code-block:: python
+#     .. highlight:: python
+#     .. code-block:: python
 
-         from nlptools.morph import morph_tagger
+#          from nlptools.morph import morph_tagger
       
-         # Return the morpological solution for each token in this text
-         morph_tagger.tagger('ذهب الولد الى المدرسة')
+#          # Return the morpological solution for each token in this text
+#          morph_tagger.tagger('ذهب الولد الى المدرسة')
 
-         # the output
-            [['ذهب', 349890, 'فعل', 'MSA'],
-            ['الولد', 320244, 'اسم', 'MSA'],
-            ['الى', 20215999, 'كلمة وظيفية', 'MSA'],
-            ['المدرسة', 561184, 'اسم', 'MSA']]
-    """
+#          # the output
+#             [['ذهب', 'فعل', 349890, 'MSA', 'lemmatizer'],
+#             ['الولد', 'اسم', 320244, 'MSA', 'lemmatizer'],
+#             ['الى', 'كلمة وظيفية', 20215999, 'MSA', 'lemmatizer'],
+#             ['المدرسة', 'اسم', 561184, 'MSA', 'lemmatizer']]
+#     """
     
-    # Check if the ALMA dictionary has been loaded
-    if settings.flag == True:
-        settings.flag = False
-        settings.div_dic = load_ALMA_dic()
+#     # Check if the ALMA dictionary has been loaded
+#     if settings.flag == True:
+#         settings.flag = False
+#         settings.div_dic = load_ALMA_dic()
    
     
-    # Perform morphological tagging for the input text
-    output_list = analyze_morphology(text,language, task)
+#     # Perform morphological tagging for the input text
+#     output_list = morph_tagger(text,language, task)
     
-    # Return a list of morphological solution for each token in the input text
-    return output_list
+#     # Return a list of morphological solution for each token in the input text
+#     return output_list
```

### Comparing `nlptoolssna-0.4.6/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.4.7/nlptools/morphology/tokenizers_words.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This code was taken from Camel tools without any change
 
 # -*- coding: utf-8 -*-
 
 
 import re
-from nlptools.morph.charsets import UNICODE_PUNCT_SYMBOL_CHARSET
-from nlptools.morph.charsets import UNICODE_LETTER_MARK_NUMBER_CHARSET
+from nlptools.morphology.charsets import UNICODE_PUNCT_SYMBOL_CHARSET
+from nlptools.morphology.charsets import UNICODE_LETTER_MARK_NUMBER_CHARSET
 
 
 _ALL_PUNCT = u''.join(UNICODE_PUNCT_SYMBOL_CHARSET)
 _ALL_LETTER_MARK_NUMBER = u''.join(UNICODE_LETTER_MARK_NUMBER_CHARSET)
 _TOKENIZE_RE = re.compile(r'[' + re.escape(_ALL_PUNCT) + r']|[' +
                           re.escape(_ALL_LETTER_MARK_NUMBER) + r']+')
```

### Comparing `nlptoolssna-0.4.6/nlptools/parse/parser.py` & `nlptoolssna-0.4.7/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/salma/implication.py` & `nlptoolssna-0.4.7/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.4.7/nlptools/salma/tokenizers_words.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import re
 
-from nlptools.morph.charsets import UNICODE_PUNCT_SYMBOL_CHARSET
-from nlptools.morph.charsets import UNICODE_LETTER_MARK_NUMBER_CHARSET
+from nlptools.morphology.charsets import UNICODE_PUNCT_SYMBOL_CHARSET
+from nlptools.morphology.charsets import UNICODE_LETTER_MARK_NUMBER_CHARSET
 
 
 _ALL_PUNCT = u''.join(UNICODE_PUNCT_SYMBOL_CHARSET)
 _ALL_LETTER_MARK_NUMBER = u''.join(UNICODE_LETTER_MARK_NUMBER_CHARSET)
 _TOKENIZE_RE = re.compile(r'[' + re.escape(_ALL_PUNCT) + r']|[' +
                           re.escape(_ALL_LETTER_MARK_NUMBER) + r']+')
```

### Comparing `nlptoolssna-0.4.6/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.4.7/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.6/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.4.7/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,36 +17,36 @@
 docs/source/authors.rst
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/readme.rst
 docs/source/_static/download.png
 docs/source/api/DataDownload.rst
-docs/source/api/morph.rst
+docs/source/api/morphology.rst
 docs/source/api/DataDownload/downloader.rst
-docs/source/api/morph/morph_tagger.rst
+docs/source/api/morphology/morph_tagger.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
 nlptools/DataDownload/__init__.py
 nlptools/DataDownload/downloader.py
 nlptools/arabiner/__init__.py
 nlptools/arabiner/data.py
 nlptools/arabiner/datasets.py
 nlptools/arabiner/helpers.py
 nlptools/arabiner/infer.py
 nlptools/arabiner/transforms.py
 nlptools/data/my_data.pickle
 nlptools/jaccard/__init__.py
 nlptools/jaccard/jaccardFunction.py
-nlptools/morph/__init__.py
-nlptools/morph/charsets.py
-nlptools/morph/morph_tagger.py
-nlptools/morph/settings.py
-nlptools/morph/tokenizers_words.py
+nlptools/morphology/__init__.py
+nlptools/morphology/charsets.py
+nlptools/morphology/morph_analyzer.py
+nlptools/morphology/settings.py
+nlptools/morphology/tokenizers_words.py
 nlptools/parse/__init__.py
 nlptools/parse/parser.py
 nlptools/salma/__init__.py
 nlptools/salma/implication.py
 nlptools/salma/tokenizers_words.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
```

### Comparing `nlptoolssna-0.4.6/setup.cfg` & `nlptoolssna-0.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.6/setup.py` & `nlptoolssna-0.4.7/setup.py`

 * *Files identical despite different names*

