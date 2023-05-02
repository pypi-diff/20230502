# Comparing `tmp/langtable-0.0.61.tar.gz` & `tmp/langtable-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langtable-0.0.61.tar", last modified: Thu Nov 24 22:33:27 2022, max compression
+gzip compressed data, was "langtable-0.0.62.tar", last modified: Tue May  2 11:04:42 2023, max compression
```

## Comparing `langtable-0.0.61.tar` & `langtable-0.0.62.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2022-11-24 22:33:27.017652 langtable-0.0.61/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)    35147 2013-05-08 14:51:39.000000 langtable-0.0.61/COPYING
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)    17882 2022-11-24 15:06:26.000000 langtable-0.0.61/ChangeLog
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      163 2019-09-04 14:23:21.000000 langtable-0.0.61/MANIFEST.in
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2610 2022-11-23 10:25:25.000000 langtable-0.0.61/Makefile
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2424 2022-11-24 22:33:27.017652 langtable-0.0.61/PKG-INFO
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1790 2020-10-29 10:19:58.000000 langtable-0.0.61/README
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2022-11-24 22:33:27.015652 langtable-0.0.61/langtable/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      511 2019-09-04 14:23:21.000000 langtable-0.0.61/langtable/__init__.py
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2022-11-24 22:33:27.016652 langtable-0.0.61/langtable/data/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     5849 2022-04-21 10:45:07.000000 langtable-0.0.61/langtable/data/keyboards.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   400553 2022-11-23 11:11:39.000000 langtable-0.0.61/langtable/data/languages.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   479757 2022-11-23 11:11:51.000000 langtable-0.0.61/langtable/data/territories.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   374509 2022-11-23 11:11:58.000000 langtable-0.0.61/langtable/data/timezoneidparts.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3542 2022-01-25 07:22:23.000000 langtable-0.0.61/langtable/data/timezones.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   104616 2022-09-21 14:51:19.000000 langtable-0.0.61/langtable/langtable.py
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2022-11-24 22:33:27.017652 langtable-0.0.61/langtable/schemas/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1301 2019-09-04 14:23:21.000000 langtable-0.0.61/langtable/schemas/keyboards.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     4153 2019-09-04 14:23:21.000000 langtable-0.0.61/langtable/schemas/languages.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3482 2019-09-04 14:23:21.000000 langtable-0.0.61/langtable/schemas/territories.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      683 2019-09-04 14:23:21.000000 langtable-0.0.61/langtable/schemas/timezoneidparts.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      665 2019-09-04 14:23:21.000000 langtable-0.0.61/langtable/schemas/timezones.rng
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2022-11-24 22:33:27.015652 langtable-0.0.61/langtable.egg-info/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2424 2022-11-24 22:33:26.000000 langtable-0.0.61/langtable.egg-info/PKG-INFO
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      719 2022-11-24 22:33:26.000000 langtable-0.0.61/langtable.egg-info/SOURCES.txt
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2022-11-24 22:33:26.000000 langtable-0.0.61/langtable.egg-info/dependency_links.txt
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2022-11-24 22:15:52.000000 langtable-0.0.61/langtable.egg-info/not-zip-safe
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)       10 2022-11-24 22:33:26.000000 langtable-0.0.61/langtable.egg-info/top_level.txt
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)    16310 2022-11-23 11:11:27.000000 langtable-0.0.61/main.py
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)       38 2022-11-24 22:33:27.017652 langtable-0.0.61/setup.cfg
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     1811 2022-11-24 15:09:10.000000 langtable-0.0.61/setup.py
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   113358 2022-11-23 11:19:54.000000 langtable-0.0.61/test_cases.py
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2022-11-24 22:33:27.017652 langtable-0.0.61/tools/
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     5005 2019-12-20 16:08:11.000000 langtable-0.0.61/tools/compare_with_glib_source.py
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     2927 2019-09-04 14:23:21.000000 langtable-0.0.61/tools/list-missing-regions-and-languages.sh
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2933 2013-05-08 14:51:39.000000 langtable-0.0.61/unicode-license.txt
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2023-05-02 11:04:42.712787 langtable-0.0.62/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)    35147 2013-05-08 14:51:39.000000 langtable-0.0.62/COPYING
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)    18090 2023-05-02 10:46:11.000000 langtable-0.0.62/ChangeLog
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      163 2019-09-04 14:23:21.000000 langtable-0.0.62/MANIFEST.in
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2610 2022-11-24 22:52:40.000000 langtable-0.0.62/Makefile
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2424 2023-05-02 11:04:42.712787 langtable-0.0.62/PKG-INFO
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1790 2020-10-29 10:19:58.000000 langtable-0.0.62/README
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2023-05-02 11:04:42.710786 langtable-0.0.62/langtable/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      511 2019-09-04 14:23:21.000000 langtable-0.0.62/langtable/__init__.py
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2023-05-02 11:04:42.711786 langtable-0.0.62/langtable/data/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     5888 2023-05-02 10:21:23.000000 langtable-0.0.62/langtable/data/keyboards.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   400614 2023-05-02 10:39:16.000000 langtable-0.0.62/langtable/data/languages.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   479808 2023-05-02 10:39:23.000000 langtable-0.0.62/langtable/data/territories.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   374509 2022-11-24 22:52:40.000000 langtable-0.0.62/langtable/data/timezoneidparts.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3542 2022-01-25 07:22:23.000000 langtable-0.0.62/langtable/data/timezones.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   104616 2022-11-24 22:52:40.000000 langtable-0.0.62/langtable/langtable.py
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2023-05-02 11:04:42.711786 langtable-0.0.62/langtable/schemas/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1301 2019-09-04 14:23:21.000000 langtable-0.0.62/langtable/schemas/keyboards.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     4153 2019-09-04 14:23:21.000000 langtable-0.0.62/langtable/schemas/languages.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3482 2019-09-04 14:23:21.000000 langtable-0.0.62/langtable/schemas/territories.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      683 2019-09-04 14:23:21.000000 langtable-0.0.62/langtable/schemas/timezoneidparts.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      665 2019-09-04 14:23:21.000000 langtable-0.0.62/langtable/schemas/timezones.rng
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2023-05-02 11:04:42.710786 langtable-0.0.62/langtable.egg-info/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2424 2023-05-02 11:04:42.000000 langtable-0.0.62/langtable.egg-info/PKG-INFO
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      719 2023-05-02 11:04:42.000000 langtable-0.0.62/langtable.egg-info/SOURCES.txt
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2023-05-02 11:04:42.000000 langtable-0.0.62/langtable.egg-info/dependency_links.txt
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2023-05-02 10:46:51.000000 langtable-0.0.62/langtable.egg-info/not-zip-safe
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)       10 2023-05-02 11:04:42.000000 langtable-0.0.62/langtable.egg-info/top_level.txt
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)    16310 2023-05-02 10:40:18.000000 langtable-0.0.62/main.py
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)       38 2023-05-02 11:04:42.712787 langtable-0.0.62/setup.cfg
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     1811 2023-05-02 10:46:11.000000 langtable-0.0.62/setup.py
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   113359 2023-05-02 10:46:11.000000 langtable-0.0.62/test_cases.py
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2023-05-02 11:04:42.711786 langtable-0.0.62/tools/
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     5005 2019-12-20 16:08:11.000000 langtable-0.0.62/tools/compare_with_glib_source.py
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     2927 2019-09-04 14:23:21.000000 langtable-0.0.62/tools/list-missing-regions-and-languages.sh
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2933 2013-05-08 14:51:39.000000 langtable-0.0.62/unicode-license.txt
```

### Comparing `langtable-0.0.61/COPYING` & `langtable-0.0.62/COPYING`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/ChangeLog` & `langtable-0.0.62/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2023-05-02  Mike FABIAN  <mfabian@redhat.com>
+
+	* Add more translations from CLDR
+	* Get translation changes from CLDR
+	* Add Norwegian keyboard layout to keyboards.xml
+	* Add Hang script to Southern Aymara
+
 2022-11-24  Mike FABIAN  <mfabian@redhat.com>
 
 	* Add mnw_MM.UTF-8 and ckb_IQ.UTF-8
 	* Do not run test cases using Python2 anymore
 	* Add bih
 	* Add more translations from CLDR
```

### Comparing `langtable-0.0.61/Makefile` & `langtable-0.0.62/Makefile`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/PKG-INFO` & `langtable-0.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langtable
-Version: 0.0.61
+Version: 0.0.62
 Summary: guess reasonable defaults for locale, keyboard, territory, ...
 Home-page: https://github.com/mike-fabian/langtable
 Author: Mike FABIAN
 Author-email: mfabian@redhat.com
 License: GPL-3.0-or-later
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `langtable-0.0.61/README` & `langtable-0.0.62/README`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable/data/timezoneidparts.xml.gz` & `langtable-0.0.62/langtable/data/timezoneidparts.xml.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timezoneidparts.xml", last modified: Wed Nov 23 11:11:58 2022, max compression, from Unix
+gzip compressed data, was "timezoneidparts.xml", last modified: Thu Nov 24 22:52:40 2022, max compression, from Unix
```

### Comparing `langtable-0.0.61/langtable/data/timezones.xml.gz` & `langtable-0.0.62/langtable/data/timezones.xml.gz`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable/langtable.py` & `langtable-0.0.62/langtable/langtable.py`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable/schemas/keyboards.rng` & `langtable-0.0.62/langtable/schemas/keyboards.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable/schemas/languages.rng` & `langtable-0.0.62/langtable/schemas/languages.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable/schemas/territories.rng` & `langtable-0.0.62/langtable/schemas/territories.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable/schemas/timezoneidparts.rng` & `langtable-0.0.62/langtable/schemas/timezoneidparts.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable/schemas/timezones.rng` & `langtable-0.0.62/langtable/schemas/timezones.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/langtable.egg-info/PKG-INFO` & `langtable-0.0.62/langtable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langtable
-Version: 0.0.61
+Version: 0.0.62
 Summary: guess reasonable defaults for locale, keyboard, territory, ...
 Home-page: https://github.com/mike-fabian/langtable
 Author: Mike FABIAN
 Author-email: mfabian@redhat.com
 License: GPL-3.0-or-later
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `langtable-0.0.61/langtable.egg-info/SOURCES.txt` & `langtable-0.0.62/langtable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/main.py` & `langtable-0.0.62/main.py`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/setup.py` & `langtable-0.0.62/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import codecs
 
 setuptools.setup(
     # do not zip the egg file to be able to access the *.xml.gz files
     # within the egg directory easily:
     zip_safe=False,
     name='langtable',
-    version='0.0.61',
+    version='0.0.62',
     packages=setuptools.find_packages(),
     description='guess reasonable defaults for locale, keyboard, territory, ...',
     long_description=codecs.open('README', encoding='UTF-8').read(),
     license="GPL-3.0-or-later",
     author='Mike FABIAN',
     author_email='mfabian@redhat.com',
     url='https://github.com/mike-fabian/langtable',
```

### Comparing `langtable-0.0.61/test_cases.py` & `langtable-0.0.62/test_cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -1337,15 +1337,15 @@
     >>> print(language_name(languageId="bem_ZM.utf8")) # doctest: +NORMALIZE_WHITESPACE
     Ichibemba (Zambia)
     >>> print(language_name(languageId="ber_DZ.utf8")) # doctest: +NORMALIZE_WHITESPACE
     Tamaziɣt (Lezzayer)
     >>> print(language_name(languageId="ber_MA.utf8")) # doctest: +NORMALIZE_WHITESPACE
     ⵜⴰⵎⴰⵣⵉⵖⵜ (ⵜⴰⴳⵍⴷⵉⵜ ⵏ ⵍⵎⵖⵔⵉⴱ)
     >>> print(language_name(languageId="rif_MA.utf8")) # doctest: +NORMALIZE_WHITESPACE
-    Tarifit (Lmerruk)
+    Tarifit (Lmuɣrib)
     >>> print(language_name(languageId="bg_BG.utf8")) # doctest: +NORMALIZE_WHITESPACE
     Български (България)
     >>> print(language_name(languageId="bhb_IN.utf8")) # doctest: +NORMALIZE_WHITESPACE
     भीली (भारत)
     >>> print(language_name(languageId="bho_IN.utf8")) # doctest: +NORMALIZE_WHITESPACE
     भोजपुरी (भारत)
     >>> print(language_name(languageId="bho_NP.utf8")) # doctest: +NORMALIZE_WHITESPACE
```

### Comparing `langtable-0.0.61/tools/compare_with_glib_source.py` & `langtable-0.0.62/tools/compare_with_glib_source.py`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/tools/list-missing-regions-and-languages.sh` & `langtable-0.0.62/tools/list-missing-regions-and-languages.sh`

 * *Files identical despite different names*

### Comparing `langtable-0.0.61/unicode-license.txt` & `langtable-0.0.62/unicode-license.txt`

 * *Files identical despite different names*

