# Comparing `tmp/pycognaize-1.3.8.tar.gz` & `tmp/pycognaize-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognaize-1.3.8.tar", last modified: Tue Mar 28 12:11:09 2023, max compression
+gzip compressed data, was "pycognaize-1.3.9.tar", last modified: Thu Mar 30 15:40:49 2023, max compression
```

## Comparing `pycognaize-1.3.8.tar` & `pycognaize-1.3.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-28 12:11:09.630287 pycognaize-1.3.8/
--rw-rw-r--   0 david     (1000) david     (1000)    30641 2023-03-28 12:10:24.000000 pycognaize-1.3.8/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)    35137 2023-01-20 10:59:34.000000 pycognaize-1.3.8/LICENSE.txt
--rw-rw-r--   0 david     (1000) david     (1000)    32409 2023-03-28 12:11:09.630287 pycognaize-1.3.8/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1310 2023-02-10 17:58:58.000000 pycognaize-1.3.8/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-28 12:11:09.626286 pycognaize-1.3.8/pycognaize/
--rw-rw-r--   0 david     (1000) david     (1000)      361 2023-03-28 12:10:24.000000 pycognaize-1.3.8/pycognaize/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2168 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/clidriver.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-28 12:11:09.626286 pycognaize-1.3.8/pycognaize/common/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/common/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2359 2023-03-09 16:00:53.000000 pycognaize-1.3.8/pycognaize/common/confidence.py
--rw-rw-r--   0 david     (1000) david     (1000)     1650 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/common/decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)     4893 2023-03-11 19:46:36.000000 pycognaize-1.3.8/pycognaize/common/enums.py
--rw-rw-r--   0 david     (1000) david     (1000)      394 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/common/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)     1750 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/common/field_collection.py
--rw-rw-r--   0 david     (1000) david     (1000)     2352 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/common/lazy_dict.py
--rw-rw-r--   0 david     (1000) david     (1000)     2096 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/common/lazy_group_dict.py
--rw-rw-r--   0 david     (1000) david     (1000)     6826 2023-02-10 17:58:58.000000 pycognaize-1.3.8/pycognaize/common/numeric_parser.py
--rw-rw-r--   0 david     (1000) david     (1000)     3899 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/common/table_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)    21720 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/common/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      285 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/common/white_pixel.jpeg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-28 12:11:09.626286 pycognaize-1.3.8/pycognaize/document/
--rw-rw-r--   0 david     (1000) david     (1000)      129 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/document/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    22604 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/document/document.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-28 12:11:09.626286 pycognaize-1.3.8/pycognaize/document/field/
--rw-rw-r--   0 david     (1000) david     (1000)      606 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/document/field/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3049 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/document/field/area_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2793 2023-02-10 17:58:58.000000 pycognaize-1.3.8/pycognaize/document/field/date_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2718 2023-02-10 17:58:58.000000 pycognaize-1.3.8/pycognaize/document/field/field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3520 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/document/field/numeric_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2928 2023-02-10 17:58:58.000000 pycognaize-1.3.8/pycognaize/document/field/section_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2486 2023-02-10 17:58:58.000000 pycognaize-1.3.8/pycognaize/document/field/span_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     5201 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/document/field/table_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3728 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/document/field/text_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     2707 2023-03-28 12:10:24.000000 pycognaize-1.3.8/pycognaize/document/html_info.py
--rw-rw-r--   0 david     (1000) david     (1000)    21421 2023-02-10 17:58:58.000000 pycognaize-1.3.8/pycognaize/document/page.py
--rw-rw-r--   0 david     (1000) david     (1000)     3098 2023-02-21 09:10:53.000000 pycognaize-1.3.8/pycognaize/document/snapshot.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-28 12:11:09.630287 pycognaize-1.3.8/pycognaize/document/tag/
--rw-rw-r--   0 david     (1000) david     (1000)      116 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/document/tag/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3449 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/document/tag/cell.py
--rw-rw-r--   0 david     (1000) david     (1000)     6090 2023-02-10 17:58:58.000000 pycognaize-1.3.8/pycognaize/document/tag/extraction_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)    13097 2023-02-21 11:37:37.000000 pycognaize-1.3.8/pycognaize/document/tag/html_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     2091 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/document/tag/section_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     1794 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/document/tag/span_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     8858 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/document/tag/table_tag.py
--rw-rw-r--   0 david     (1000) david     (1000)    14977 2023-02-21 11:37:51.000000 pycognaize-1.3.8/pycognaize/document/tag/tag.py
--rw-rw-r--   0 david     (1000) david     (1000)     2863 2023-01-20 10:59:34.000000 pycognaize-1.3.8/pycognaize/index.py
--rw-rw-r--   0 david     (1000) david     (1000)     3866 2023-02-21 09:10:53.000000 pycognaize-1.3.8/pycognaize/login.py
--rw-rw-r--   0 david     (1000) david     (1000)    21976 2023-03-28 12:10:24.000000 pycognaize-1.3.8/pycognaize/model.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-28 12:11:09.626286 pycognaize-1.3.8/pycognaize.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    32409 2023-03-28 12:11:09.000000 pycognaize-1.3.8/pycognaize.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1562 2023-03-28 12:11:09.000000 pycognaize-1.3.8/pycognaize.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-28 12:11:09.000000 pycognaize-1.3.8/pycognaize.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       47 2023-03-28 12:11:09.000000 pycognaize-1.3.8/pycognaize.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      147 2023-03-28 12:11:09.000000 pycognaize-1.3.8/pycognaize.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-03-28 12:11:09.000000 pycognaize-1.3.8/pycognaize.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      881 2023-03-28 12:11:09.630287 pycognaize-1.3.8/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      999 2023-01-20 10:59:34.000000 pycognaize-1.3.8/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/
+-rw-rw-r--   0 david     (1000) david     (1000)    30728 2023-03-30 15:40:15.000000 pycognaize-1.3.9/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)    35137 2023-01-20 10:59:34.000000 pycognaize-1.3.9/LICENSE.txt
+-rw-rw-r--   0 david     (1000) david     (1000)    32496 2023-03-30 15:40:49.360445 pycognaize-1.3.9/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1310 2023-02-10 17:58:58.000000 pycognaize-1.3.9/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/
+-rw-rw-r--   0 david     (1000) david     (1000)      361 2023-03-30 15:40:15.000000 pycognaize-1.3.9/pycognaize/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2168 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/clidriver.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/common/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2359 2023-03-09 16:00:53.000000 pycognaize-1.3.9/pycognaize/common/confidence.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1650 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4893 2023-03-11 19:46:36.000000 pycognaize-1.3.9/pycognaize/common/enums.py
+-rw-rw-r--   0 david     (1000) david     (1000)      394 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1750 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/field_collection.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2352 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/lazy_dict.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2096 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/lazy_group_dict.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6826 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/common/numeric_parser.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3899 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/common/table_utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21720 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/common/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)      285 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/common/white_pixel.jpeg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/document/
+-rw-rw-r--   0 david     (1000) david     (1000)      129 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22604 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/document.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/document/field/
+-rw-rw-r--   0 david     (1000) david     (1000)      606 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/field/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3049 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/area_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2793 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/date_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2718 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3520 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/numeric_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2928 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/section_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2486 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/field/span_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5201 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/table_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3728 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/field/text_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2882 2023-03-30 15:40:15.000000 pycognaize-1.3.9/pycognaize/document/html_info.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21421 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/page.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3098 2023-02-21 09:10:53.000000 pycognaize-1.3.9/pycognaize/document/snapshot.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize/document/tag/
+-rw-rw-r--   0 david     (1000) david     (1000)      116 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3449 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/cell.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6090 2023-02-10 17:58:58.000000 pycognaize-1.3.9/pycognaize/document/tag/extraction_tag.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13097 2023-02-21 11:37:37.000000 pycognaize-1.3.9/pycognaize/document/tag/html_tag.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2091 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/section_tag.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1794 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/span_tag.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8858 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/document/tag/table_tag.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14977 2023-02-21 11:37:51.000000 pycognaize-1.3.9/pycognaize/document/tag/tag.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2863 2023-01-20 10:59:34.000000 pycognaize-1.3.9/pycognaize/index.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3866 2023-02-21 09:10:53.000000 pycognaize-1.3.9/pycognaize/login.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21976 2023-03-28 12:10:24.000000 pycognaize-1.3.9/pycognaize/model.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-30 15:40:49.360445 pycognaize-1.3.9/pycognaize.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    32496 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1562 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       47 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      147 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-03-30 15:40:49.000000 pycognaize-1.3.9/pycognaize.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      881 2023-03-30 15:40:49.360445 pycognaize-1.3.9/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)      999 2023-01-20 10:59:34.000000 pycognaize-1.3.9/setup.py
```

### Comparing `pycognaize-1.3.8/CHANGELOG.md` & `pycognaize-1.3.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 ## [1.3]
 
+### [1.3.9] - 2023-03-30
+- Refactor HTML._validate_path() to include try-except block
+
 ### [1.3.8] - 2023-03-28
 - Improve html file path validation by adding a new check
 in HTML._validate_path()
 
 ### [1.3.7] - 2023-03-24
 - Match (xbrl) using xpath and indices in matches function of `model.py`
```

### Comparing `pycognaize-1.3.8/LICENSE.txt` & `pycognaize-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/PKG-INFO` & `pycognaize-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.3.8
+Version: 1.3.9
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -45,14 +45,17 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.3]
 
+### [1.3.9] - 2023-03-30
+- Refactor HTML._validate_path() to include try-except block
+
 ### [1.3.8] - 2023-03-28
 - Improve html file path validation by adding a new check
 in HTML._validate_path()
 
 ### [1.3.7] - 2023-03-24
 - Match (xbrl) using xpath and indices in matches function of `model.py`
```

### Comparing `pycognaize-1.3.8/README.md` & `pycognaize-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/clidriver.py` & `pycognaize-1.3.9/pycognaize/clidriver.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/confidence.py` & `pycognaize-1.3.9/pycognaize/common/confidence.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/decorators.py` & `pycognaize-1.3.9/pycognaize/common/decorators.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/enums.py` & `pycognaize-1.3.9/pycognaize/common/enums.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/field_collection.py` & `pycognaize-1.3.9/pycognaize/common/field_collection.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/lazy_dict.py` & `pycognaize-1.3.9/pycognaize/common/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/lazy_group_dict.py` & `pycognaize-1.3.9/pycognaize/common/lazy_group_dict.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/numeric_parser.py` & `pycognaize-1.3.9/pycognaize/common/numeric_parser.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/table_utils.py` & `pycognaize-1.3.9/pycognaize/common/table_utils.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/common/utils.py` & `pycognaize-1.3.9/pycognaize/common/utils.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/document.py` & `pycognaize-1.3.9/pycognaize/document/document.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/__init__.py` & `pycognaize-1.3.9/pycognaize/document/field/__init__.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/area_field.py` & `pycognaize-1.3.9/pycognaize/document/field/area_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/date_field.py` & `pycognaize-1.3.9/pycognaize/document/field/date_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/field.py` & `pycognaize-1.3.9/pycognaize/document/field/field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/numeric_field.py` & `pycognaize-1.3.9/pycognaize/document/field/numeric_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/section_field.py` & `pycognaize-1.3.9/pycognaize/document/field/section_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/span_field.py` & `pycognaize-1.3.9/pycognaize/document/field/span_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/table_field.py` & `pycognaize-1.3.9/pycognaize/document/field/table_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/field/text_field.py` & `pycognaize-1.3.9/pycognaize/document/field/text_field.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/html_info.py` & `pycognaize-1.3.9/pycognaize/document/html_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,26 @@
 
         :param path: path of the source document
         :param document_id: document id
         :return: valid path for the `source.html` file
             corresponding to the document id
         """
         valid_path = ''
-        joined_path = os.path.join(path, document_id)
-        if (
-                self.ci.isdir(joined_path)
-                and StorageEnum.html_file.value in self.ci.listdir(joined_path)
-        ):
-            valid_path = joined_path
-        elif StorageEnum.html_file.value in self.ci.listdir(path):
-            valid_path = path
+        try:
+            joined_path = os.path.join(path, document_id)
+            if (
+                    self.ci.isdir(joined_path)
+                    and StorageEnum.html_file.value
+                    in self.ci.listdir(joined_path)
+            ):
+                valid_path = joined_path
+            elif StorageEnum.html_file.value in self.ci.listdir(path):
+                valid_path = path
+        except Exception as e:
+            logging.debug(f"An error occurred while validating the path: {e}")
         return valid_path
 
     def _read_html(self, path: str) -> str:
         if self._html_file is None:
             with self.ci.open(path, 'r') as file:
                 self._html_file = file.read()
         return self._html_file
```

### Comparing `pycognaize-1.3.8/pycognaize/document/page.py` & `pycognaize-1.3.9/pycognaize/document/page.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/snapshot.py` & `pycognaize-1.3.9/pycognaize/document/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/tag/cell.py` & `pycognaize-1.3.9/pycognaize/document/tag/cell.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/tag/extraction_tag.py` & `pycognaize-1.3.9/pycognaize/document/tag/extraction_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/tag/html_tag.py` & `pycognaize-1.3.9/pycognaize/document/tag/html_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/tag/section_tag.py` & `pycognaize-1.3.9/pycognaize/document/tag/section_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/tag/span_tag.py` & `pycognaize-1.3.9/pycognaize/document/tag/span_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/tag/table_tag.py` & `pycognaize-1.3.9/pycognaize/document/tag/table_tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/document/tag/tag.py` & `pycognaize-1.3.9/pycognaize/document/tag/tag.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/index.py` & `pycognaize-1.3.9/pycognaize/index.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/login.py` & `pycognaize-1.3.9/pycognaize/login.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize/model.py` & `pycognaize-1.3.9/pycognaize/model.py`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/pycognaize.egg-info/PKG-INFO` & `pycognaize-1.3.9/pycognaize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycognaize
-Version: 1.3.8
+Version: 1.3.9
 Home-page: https://github.com/cognaize/pycognaize
 Author: Cognaize
 License: Apache License 2.0
 Project-URL: Source, https://github.com/cognaize/pycognaize
 Project-URL: Reference, https://pycognaize.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/cognaize/pycognaize/blob/master/CHANGELOG.md
 Requires-Python: >= 3.7
@@ -45,14 +45,17 @@
 Have a look at the [quick tutorial](http://pycognaize-docs.com.s3-website.us-east-2.amazonaws.com/tutorials/quick_tutorial.html) 
 for understanding main concepts of the SDK.
 
 # Changelog
 
 ## [1.3]
 
+### [1.3.9] - 2023-03-30
+- Refactor HTML._validate_path() to include try-except block
+
 ### [1.3.8] - 2023-03-28
 - Improve html file path validation by adding a new check
 in HTML._validate_path()
 
 ### [1.3.7] - 2023-03-24
 - Match (xbrl) using xpath and indices in matches function of `model.py`
```

### Comparing `pycognaize-1.3.8/pycognaize.egg-info/SOURCES.txt` & `pycognaize-1.3.9/pycognaize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/setup.cfg` & `pycognaize-1.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycognaize-1.3.8/setup.py` & `pycognaize-1.3.9/setup.py`

 * *Files identical despite different names*

