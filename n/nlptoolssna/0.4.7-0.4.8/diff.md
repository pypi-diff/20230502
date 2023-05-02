# Comparing `tmp/nlptoolssna-0.4.7.tar.gz` & `tmp/nlptoolssna-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.4.7.tar", last modified: Tue May  2 17:28:57 2023, max compression
+gzip compressed data, was "nlptoolssna-0.4.8.tar", last modified: Tue May  2 19:06:51 2023, max compression
```

## Comparing `nlptoolssna-0.4.7.tar` & `nlptoolssna-0.4.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.661973 nlptoolssna-0.4.7/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.7/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.618506 nlptoolssna-0.4.7/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.618506 nlptoolssna-0.4.7/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.661973 nlptoolssna-0.4.7/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.7/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.669987 nlptoolssna-0.4.7/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.7/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.7/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.7/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.7/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.7/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.686735 nlptoolssna-0.4.7/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.686735 nlptoolssna-0.4.7/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.7/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.695137 nlptoolssna-0.4.7/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.695137 nlptoolssna-0.4.7/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.4.7/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.4.7/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.695137 nlptoolssna-0.4.7/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      142 2023-05-02 17:27:34.000000 nlptoolssna-0.4.7/docs/source/api/morphology/morph_tagger.rst
--rw-rw-rw-   0        0        0      213 2023-05-02 17:28:00.000000 nlptoolssna-0.4.7/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.4.7/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.7/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.7/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.7/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.7/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.703608 nlptoolssna-0.4.7/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.703608 nlptoolssna-0.4.7/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.7/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4019 2023-05-01 11:12:31.000000 nlptoolssna-0.4.7/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.720626 nlptoolssna-0.4.7/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.7/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.7/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.7/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.7/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.7/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.4.7/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.720626 nlptoolssna-0.4.7/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.7/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.720626 nlptoolssna-0.4.7/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.7/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.7/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.737295 nlptoolssna-0.4.7/nlptools/morphology/
--rw-rw-rw-   0        0        0      372 2023-05-02 13:24:43.000000 nlptoolssna-0.4.7/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.7/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     7538 2023-05-02 15:30:16.000000 nlptoolssna-0.4.7/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.7/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.4.7/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.737295 nlptoolssna-0.4.7/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.7/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.7/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.745279 nlptoolssna-0.4.7/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.7/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.7/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.4.7/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.753895 nlptoolssna-0.4.7/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1616 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 17:28:57.000000 nlptoolssna-0.4.7/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:28:57.762077 nlptoolssna-0.4.7/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.7/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.630560 nlptoolssna-0.4.8/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-02 19:06:51.630560 nlptoolssna-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.529052 nlptoolssna-0.4.8/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.8/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.480575 nlptoolssna-0.4.8/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.482584 nlptoolssna-0.4.8/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.531052 nlptoolssna-0.4.8/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.8/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.539393 nlptoolssna-0.4.8/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.8/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.8/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.8/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.8/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.8/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.552946 nlptoolssna-0.4.8/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.553947 nlptoolssna-0.4.8/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.8/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.558340 nlptoolssna-0.4.8/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.561340 nlptoolssna-0.4.8/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.4.8/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.4.8/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.562341 nlptoolssna-0.4.8/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.4.8/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.4.8/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      166 2023-05-02 17:27:43.000000 nlptoolssna-0.4.8/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.8/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.8/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.8/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.8/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.567703 nlptoolssna-0.4.8/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.570908 nlptoolssna-0.4.8/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.8/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.4.8/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.581917 nlptoolssna-0.4.8/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.8/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.8/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.8/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.8/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.8/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.4.8/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.583963 nlptoolssna-0.4.8/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.8/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.586961 nlptoolssna-0.4.8/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.8/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.8/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.602438 nlptoolssna-0.4.8/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.4.8/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.8/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     8006 2023-05-02 19:05:46.000000 nlptoolssna-0.4.8/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.8/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.4.8/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.605409 nlptoolssna-0.4.8/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.8/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.8/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.612075 nlptoolssna-0.4.8/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.8/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.8/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      541 2023-05-02 13:53:44.000000 nlptoolssna-0.4.8/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.625225 nlptoolssna-0.4.8/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-02 19:06:51.000000 nlptoolssna-0.4.8/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-05-02 19:06:51.000000 nlptoolssna-0.4.8/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:06:51.000000 nlptoolssna-0.4.8/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-02 19:06:51.000000 nlptoolssna-0.4.8/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.8/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-02 19:06:51.000000 nlptoolssna-0.4.8/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 19:06:51.000000 nlptoolssna-0.4.8/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-02 19:06:51.631559 nlptoolssna-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     2111 2023-05-01 12:52:22.000000 nlptoolssna-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:06:51.628564 nlptoolssna-0.4.8/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.8/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.4.7/CONTRIBUTING.rst` & `nlptoolssna-0.4.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/LICENSE` & `nlptoolssna-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/PKG-INFO` & `nlptoolssna-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.7/README.rst` & `nlptoolssna-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/docs/Makefile` & `nlptoolssna-0.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/docs/build/html/_images/download.png` & `nlptoolssna-0.4.8/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/docs/build/html/_static/download.png` & `nlptoolssna-0.4.8/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/docs/make.bat` & `nlptoolssna-0.4.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/docs/source/_static/download.png` & `nlptoolssna-0.4.8/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/docs/source/conf.py` & `nlptoolssna-0.4.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/docs/source/installation.rst` & `nlptoolssna-0.4.8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.4.8/nlptools/DataDownload/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import sys
 from pathlib import Path
 import requests  
 import zipfile
 from tqdm import tqdm
 
 urls = {
-    'morph':'https://portal.sina.birzeit.edu/ALMA27012000.pickle',
-    'ner': 'http://portal.sina.birzeit.edu/Wj27012000.zip',
-    'salma': 'http://portal.sina.birzeit.edu/SALMA27012000.zip',
-    'salma2021': 'http://portal.sina.birzeit.edu/SALMA_v2.zip'
+    'morph':'https://portal.sina.birzeit.edu/ALMA27012000.pickle'
+    # 'ner': 'http://portal.sina.birzeit.edu/Wj27012000.zip',
+#     'salma': 'http://portal.sina.birzeit.edu/SALMA27012000.zip',
+#     'salma2021': 'http://portal.sina.birzeit.edu/SALMA_v2.zip'
+# 
 }
 
 def get_appdatadir():
     """
     Returns the path to the directory where the application data is stored.
 
     Returns:
```

### Comparing `nlptoolssna-0.4.7/nlptools/arabiner/data.py` & `nlptoolssna-0.4.8/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/arabiner/datasets.py` & `nlptoolssna-0.4.8/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/arabiner/helpers.py` & `nlptoolssna-0.4.8/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/arabiner/infer.py` & `nlptoolssna-0.4.8/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/arabiner/transforms.py` & `nlptoolssna-0.4.8/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/data/my_data.pickle` & `nlptoolssna-0.4.8/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.4.8/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/morphology/charsets.py` & `nlptoolssna-0.4.8/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.4.8/nlptools/morphology/morph_analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import pickle
 from nlptools.morphology import settings 
 import re
 from nlptools.morphology.tokenizers_words import simple_word_tokenize
 from nlptools.parse.parser import arStrip
 import os.path
 from nlptools.DataDownload import downloader
-
+from nlptools.morphology.charsets import AR_CHARSET, AR_DIAC_CHARSET
 # def load_ALMA_dic():
 #    # Open the Pickle file in binary mode
 #     filename = 'ALMA27012000.pickle'
 #     path =downloader.get_appdatadir()
 #     file_path = os.path.join(path, filename)
     
 
 #     with open(file_path, 'rb') as f:
 #        #Load the serialized data from the file
 #        ALMA_dic = pickle.load(f)
 #        #print(ALMA_dic)
 #        return ALMA_dic
-
+_IS_AR_RE = re.compile(u'^[' + re.escape(u''.join(AR_CHARSET)) + u']+$')
 def find_solution(token, language, task):
     """
     Given a token, this method finds the morphological solution lemma and/or pos based on a spesific language and task.
           
     Args:
         - token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
         - language (:obj:`str`): In the current version, `MSA` is only supported. 
@@ -73,29 +73,25 @@
 
    tokens = simple_word_tokenize(text)
 
    for token in tokens:
          result_token =[]
          token = arStrip(token , False , True , False , False , False , False) 
          token = re.sub('[ٱ]','ﺍ',token)
-
-         if task == 'lemmatizer':
-             solution =[token, token+"_0"]
-         elif task == 'pos':
-             solution=[token, ""]
-         else: 
-             solution=[token, token+"_0",""]
+         solution=[token, token+"_0",""]
 
          if token.isdigit():
             solution[2] = "digit" #pos
 
-
-         elif re.match("^[a-zA-Z]*$", token): 
+         elif not _is_ar(token):
             solution[2] = "Foreign" #pos
 
+        #  elif re.match("^[a-zA-Z]*$", token): 
+        #     solution[2] = "Foreign" #pos
+
          else:
             result_token = find_solution(token,language, task)
             
            
             if result_token == []:
                token_without_al = re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token))
                if len(token_without_al) > 5  :
@@ -118,20 +114,36 @@
 
             if result_token == []:
                # try with remove diac and unify alef
                word_undiac = arStrip(token , True , True , True , False, True , False) # diacs , smallDiacs , shaddah ,  alif
                result_token = find_solution(word_undiac, language, task)
 
          if result_token != []:
+               
                output_list.append(result_token)
          else:
             # if no solution is found
             output_list.append(solution)
+        
+   filter_results(task, output_list)
+   return output_list 
+
+
+def _is_ar(word):
+    return _IS_AR_RE.match(word) is not None
+
 
-   return output_list               
+def filter_results(task, output_list):
+    if task == 'lemmatizer':
+              #[token, token+"_0",""]
+              return [i.pop(2) for i in output_list]
+    elif task == 'pos':
+              return [i.pop(1) for i in output_list]
+    else: 
+          return output_list         
         
 # def tagger(text: str, task = 'full', language = 'MSA'):
 
 #     """
 #     This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
 #     There is no limit for the text size, but one should be resonable based on the available resources (computational power).
```

### Comparing `nlptoolssna-0.4.7/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.4.8/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/parse/parser.py` & `nlptoolssna-0.4.8/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/salma/implication.py` & `nlptoolssna-0.4.8/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.4.8/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.4.8/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.7/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.4.8/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/readme.rst
 docs/source/_static/download.png
 docs/source/api/DataDownload.rst
 docs/source/api/morphology.rst
 docs/source/api/DataDownload/downloader.rst
-docs/source/api/morphology/morph_tagger.rst
+docs/source/api/morphology/morph_analyzer.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
 nlptools/DataDownload/__init__.py
 nlptools/DataDownload/downloader.py
 nlptools/arabiner/__init__.py
 nlptools/arabiner/data.py
```

### Comparing `nlptoolssna-0.4.7/setup.cfg` & `nlptoolssna-0.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.7/setup.py` & `nlptoolssna-0.4.8/setup.py`

 * *Files identical despite different names*

