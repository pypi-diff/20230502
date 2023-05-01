# Comparing `tmp/pydetex-0.9.9.tar.gz` & `tmp/pydetex-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydetex-0.9.9.tar", last modified: Wed Mar  8 21:59:56 2023, max compression
+gzip compressed data, was "pydetex-1.0.0.tar", last modified: Mon May  1 22:29:35 2023, max compression
```

## Comparing `pydetex-0.9.9.tar` & `pydetex-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 21:59:55.920000 pydetex-0.9.9/
--rw-rw-rw-   0        0        0     1073 2021-10-03 21:53:42.000000 pydetex-0.9.9/LICENSE
--rw-rw-rw-   0        0        0      406 2021-11-01 21:25:22.000000 pydetex-0.9.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5567 2023-03-08 21:59:58.000000 pydetex-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     4496 2023-01-06 13:37:32.000000 pydetex-0.9.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-08 21:59:55.940000 pydetex-0.9.9/pydetex/
--rw-rw-rw-   0        0        0      721 2022-02-03 13:19:14.000000 pydetex-0.9.9/pydetex/__init__.py
--rw-rw-rw-   0        0        0     1314 2021-11-14 20:58:54.000000 pydetex-0.9.9/pydetex/_fonts.py
--rw-rw-rw-   0        0        0    24925 2022-12-05 13:17:22.000000 pydetex-0.9.9/pydetex/_gui_settings.py
--rw-rw-rw-   0        0        0    45460 2023-02-15 12:36:58.000000 pydetex-0.9.9/pydetex/_gui_utils.py
--rw-rw-rw-   0        0        0    23415 2022-05-13 22:07:20.000000 pydetex-0.9.9/pydetex/_symbols.py
--rw-rw-rw-   0        0        0     9705 2023-02-15 12:36:20.000000 pydetex-0.9.9/pydetex/_utils_lang.py
--rw-rw-rw-   0        0        0    23887 2023-02-15 12:36:20.000000 pydetex-0.9.9/pydetex/_utils_tex.py
--rw-rw-rw-   0        0        0    30942 2022-05-13 22:07:20.000000 pydetex-0.9.9/pydetex/gui.py
--rw-rw-rw-   0        0        0    46650 2023-03-08 21:59:08.000000 pydetex-0.9.9/pydetex/parsers.py
--rw-rw-rw-   0        0        0     2941 2023-02-15 12:36:20.000000 pydetex-0.9.9/pydetex/pipelines.py
-drwxrwxrwx   0        0        0        0 2023-03-08 21:59:55.990000 pydetex-0.9.9/pydetex/res/
--rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-0.9.9/pydetex/res/cog.ico
--rw-rw-rw-   0        0        0     4286 2021-10-18 04:07:18.000000 pydetex-0.9.9/pydetex/res/dictionary.ico
--rw-rw-rw-   0        0        0    13224 2021-09-14 16:31:46.000000 pydetex-0.9.9/pydetex/res/icon.gif
--rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-0.9.9/pydetex/res/icon.ico
--rw-rw-rw-   0        0        0      554 2021-11-14 20:58:54.000000 pydetex-0.9.9/pydetex/res/placeholder_en.tex
--rw-rw-rw-   0        0        0      605 2021-11-14 20:58:54.000000 pydetex-0.9.9/pydetex/res/placeholder_es.tex
--rw-rw-rw-   0        0        0   184280 2021-10-16 20:19:00.000000 pydetex-0.9.9/pydetex/res/stopwords.json
--rw-rw-rw-   0        0        0      227 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_subscripts.txt
--rw-rw-rw-   0        0        0      416 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_superscripts.txt
--rw-rw-rw-   0        0        0     4861 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_symbols.txt
--rw-rw-rw-   0        0        0      427 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_textbb.txt
--rw-rw-rw-   0        0        0      900 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_textbf.txt
--rw-rw-rw-   0        0        0      364 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_textcal.txt
--rw-rw-rw-   0        0        0      359 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_textfrak.txt
--rw-rw-rw-   0        0        0      829 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_textit.txt
--rw-rw-rw-   0        0        0      434 2020-02-26 08:23:30.000000 pydetex-0.9.9/pydetex/res/u_textmono.txt
--rw-rw-rw-   0        0        0     8357 2022-12-05 13:17:22.000000 pydetex-0.9.9/pydetex/utils.py
--rw-rw-rw-   0        0        0      826 2023-03-08 21:59:08.000000 pydetex-0.9.9/pydetex/version.py
-drwxrwxrwx   0        0        0        0 2023-03-08 21:59:55.970000 pydetex-0.9.9/pydetex.egg-info/
--rw-rw-rw-   0        0        0     5567 2023-03-08 21:59:56.000000 pydetex-0.9.9/pydetex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-03-08 21:59:56.000000 pydetex-0.9.9/pydetex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 21:59:56.000000 pydetex-0.9.9/pydetex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      275 2023-03-08 21:59:56.000000 pydetex-0.9.9/pydetex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-08 21:59:56.000000 pydetex-0.9.9/pydetex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      181 2022-12-05 14:05:58.000000 pydetex-0.9.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-08 21:59:58.000000 pydetex-0.9.9/setup.cfg
--rw-rw-rw-   0        0        0     1932 2023-01-26 18:27:08.000000 pydetex-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.060000 pydetex-1.0.0/
+-rw-rw-rw-   0        0        0     1073 2021-10-03 21:53:42.000000 pydetex-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      406 2021-11-01 21:25:22.000000 pydetex-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5567 2023-05-01 22:29:36.000000 pydetex-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4370 2023-03-08 22:09:00.000000 pydetex-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.080000 pydetex-1.0.0/pydetex/
+-rw-rw-rw-   0        0        0      721 2022-02-03 13:19:14.000000 pydetex-1.0.0/pydetex/__init__.py
+-rw-rw-rw-   0        0        0     1314 2021-11-14 20:58:54.000000 pydetex-1.0.0/pydetex/_fonts.py
+-rw-rw-rw-   0        0        0    24925 2022-12-05 13:17:22.000000 pydetex-1.0.0/pydetex/_gui_settings.py
+-rw-rw-rw-   0        0        0    45460 2023-02-15 12:36:58.000000 pydetex-1.0.0/pydetex/_gui_utils.py
+-rw-rw-rw-   0        0        0    23415 2022-05-13 22:07:20.000000 pydetex-1.0.0/pydetex/_symbols.py
+-rw-rw-rw-   0        0        0     9705 2023-02-15 12:36:20.000000 pydetex-1.0.0/pydetex/_utils_lang.py
+-rw-rw-rw-   0        0        0    23887 2023-02-15 12:36:20.000000 pydetex-1.0.0/pydetex/_utils_tex.py
+-rw-rw-rw-   0        0        0    30942 2022-05-13 22:07:20.000000 pydetex-1.0.0/pydetex/gui.py
+-rw-rw-rw-   0        0        0    46650 2023-03-08 21:59:08.000000 pydetex-1.0.0/pydetex/parsers.py
+-rw-rw-rw-   0        0        0     2941 2023-02-15 12:36:20.000000 pydetex-1.0.0/pydetex/pipelines.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.120000 pydetex-1.0.0/pydetex/res/
+-rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.0/pydetex/res/cog.ico
+-rw-rw-rw-   0        0        0     4286 2021-10-18 04:07:18.000000 pydetex-1.0.0/pydetex/res/dictionary.ico
+-rw-rw-rw-   0        0        0    13224 2021-09-14 16:31:46.000000 pydetex-1.0.0/pydetex/res/icon.gif
+-rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.0/pydetex/res/icon.ico
+-rw-rw-rw-   0        0        0      554 2021-11-14 20:58:54.000000 pydetex-1.0.0/pydetex/res/placeholder_en.tex
+-rw-rw-rw-   0        0        0      605 2021-11-14 20:58:54.000000 pydetex-1.0.0/pydetex/res/placeholder_es.tex
+-rw-rw-rw-   0        0        0   184280 2021-10-16 20:19:00.000000 pydetex-1.0.0/pydetex/res/stopwords.json
+-rw-rw-rw-   0        0        0      227 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_subscripts.txt
+-rw-rw-rw-   0        0        0      416 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_superscripts.txt
+-rw-rw-rw-   0        0        0     4861 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_symbols.txt
+-rw-rw-rw-   0        0        0      427 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textbb.txt
+-rw-rw-rw-   0        0        0      900 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textbf.txt
+-rw-rw-rw-   0        0        0      364 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textcal.txt
+-rw-rw-rw-   0        0        0      359 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textfrak.txt
+-rw-rw-rw-   0        0        0      829 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textit.txt
+-rw-rw-rw-   0        0        0      434 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textmono.txt
+-rw-rw-rw-   0        0        0     8357 2022-12-05 13:17:22.000000 pydetex-1.0.0/pydetex/utils.py
+-rw-rw-rw-   0        0        0      789 2023-05-01 22:29:30.000000 pydetex-1.0.0/pydetex/version.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.100000 pydetex-1.0.0/pydetex.egg-info/
+-rw-rw-rw-   0        0        0     5567 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      284 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      173 2023-05-01 22:26:04.000000 pydetex-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 22:29:36.000000 pydetex-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2023-04-13 16:52:48.000000 pydetex-1.0.0/setup.py
```

### Comparing `pydetex-0.9.9/LICENSE` & `pydetex-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/PKG-INFO` & `pydetex-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydetex
-Version: 0.9.9
+Version: 1.0.0
 Summary: An application that transforms LaTeX code to plain text
 Home-page: https://pydetex.readthedocs.io
 Author: Pablo Pizarro R.
 Author-email: pablo@ppizarror.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ppizarror/PyDetex/issues
 Project-URL: Documentation, https://pydetex.readthedocs.io
@@ -148,10 +148,10 @@
 
 - Add synthax checking for several languages, like `language-check <https://github.com/myint/language-check>`_.
 - Custom support for environments, such as *table*.
 
 Author
 ------
 
-`Pablo Pizarro R. <https://ppizarror.com>`_ | 2021 - 2022
+`Pablo Pizarro R. <https://ppizarror.com>`_ | 2021 - 2023
```

### Comparing `pydetex-0.9.9/README.rst` & `pydetex-1.0.0/pydetex.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: pydetex
+Version: 1.0.0
+Summary: An application that transforms LaTeX code to plain text
+Home-page: https://pydetex.readthedocs.io
+Author: Pablo Pizarro R.
+Author-email: pablo@ppizarror.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/ppizarror/PyDetex/issues
+Project-URL: Documentation, https://pydetex.readthedocs.io
+Project-URL: Source Code, https://github.com/ppizarror/PyDetex
+Keywords: latex detex parser gui
+Platform: any
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Text Processing
+Requires-Python: >=3.7, <4
+Provides-Extra: docs
+Provides-Extra: installer
+Provides-Extra: test
+License-File: LICENSE
+
 =======
 PyDetex
 =======
 
 .. image:: https://img.shields.io/badge/author-Pablo%20Pizarro%20R.-lightgray.svg
     :target: https://ppizarror.com
     :alt: @ppizarror
@@ -119,8 +148,10 @@
 
 - Add synthax checking for several languages, like `language-check <https://github.com/myint/language-check>`_.
 - Custom support for environments, such as *table*.
 
 Author
 ------
 
-`Pablo Pizarro R. <https://ppizarror.com>`_ | 2021 - 2022
+`Pablo Pizarro R. <https://ppizarror.com>`_ | 2021 - 2023
+
+
```

### Comparing `pydetex-0.9.9/pydetex/__init__.py` & `pydetex-1.0.0/pydetex/__init__.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/_fonts.py` & `pydetex-1.0.0/pydetex/_fonts.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/_gui_settings.py` & `pydetex-1.0.0/pydetex/_gui_settings.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/_gui_utils.py` & `pydetex-1.0.0/pydetex/_gui_utils.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/_symbols.py` & `pydetex-1.0.0/pydetex/_symbols.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/_utils_lang.py` & `pydetex-1.0.0/pydetex/_utils_lang.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/_utils_tex.py` & `pydetex-1.0.0/pydetex/_utils_tex.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/gui.py` & `pydetex-1.0.0/pydetex/gui.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/parsers.py` & `pydetex-1.0.0/pydetex/parsers.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/pipelines.py` & `pydetex-1.0.0/pydetex/pipelines.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/cog.ico` & `pydetex-1.0.0/pydetex/res/cog.ico`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/dictionary.ico` & `pydetex-1.0.0/pydetex/res/dictionary.ico`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/icon.gif` & `pydetex-1.0.0/pydetex/res/icon.gif`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/icon.ico` & `pydetex-1.0.0/pydetex/res/icon.ico`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/placeholder_en.tex` & `pydetex-1.0.0/pydetex/res/placeholder_en.tex`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/placeholder_es.tex` & `pydetex-1.0.0/pydetex/res/placeholder_es.tex`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/stopwords.json` & `pydetex-1.0.0/pydetex/res/stopwords.json`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/u_symbols.txt` & `pydetex-1.0.0/pydetex/res/u_symbols.txt`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/u_textbf.txt` & `pydetex-1.0.0/pydetex/res/u_textbf.txt`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/res/u_textit.txt` & `pydetex-1.0.0/pydetex/res/u_textit.txt`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex/utils.py` & `pydetex-1.0.0/pydetex/utils.py`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/pydetex.egg-info/PKG-INFO` & `pydetex-1.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,157 +1,126 @@
-Metadata-Version: 2.1
-Name: pydetex
-Version: 0.9.9
-Summary: An application that transforms LaTeX code to plain text
-Home-page: https://pydetex.readthedocs.io
-Author: Pablo Pizarro R.
-Author-email: pablo@ppizarror.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/ppizarror/PyDetex/issues
-Project-URL: Documentation, https://pydetex.readthedocs.io
-Project-URL: Source Code, https://github.com/ppizarror/PyDetex
-Keywords: latex detex parser gui
-Platform: any
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python
-Classifier: Topic :: Multimedia
-Classifier: Topic :: Text Processing
-Requires-Python: >=3.7, <4
-Provides-Extra: docs
-Provides-Extra: installer
-Provides-Extra: test
-License-File: LICENSE
-
-=======
-PyDetex
-=======
-
-.. image:: https://img.shields.io/badge/author-Pablo%20Pizarro%20R.-lightgray.svg
-    :target: https://ppizarror.com
-    :alt: @ppizarror
-
-.. image:: https://img.shields.io/badge/license-MIT-blue.svg
-    :target: https://opensource.org/licenses/MIT
-    :alt: License MIT
-
-.. image:: https://img.shields.io/badge/python-3.7+-red.svg
-    :target: https://www.python.org/downloads
-    :alt: Python 3.7+
-
-.. image:: https://badge.fury.io/py/pydetex.svg
-    :target: https://pypi.org/project/pydetex
-    :alt: PyPi package
-
-.. image:: https://img.shields.io/github/actions/workflow/status/ppizarror/PyDetex/ci.yml?branch=master
-    :target: https://github.com/ppizarror/PyDetex/actions/workflows/ci.yml
-    :alt: Build status
-    
-.. image:: https://app.fossa.com/api/projects/git%2Bgithub.com%2Fppizarror%2FPyDetex.svg?type=shield
-    :target: https://app.fossa.com/projects/git%2Bgithub.com%2Fppizarror%2FPyDetex?ref=badge_shield
-    :alt: FOSSA Status
-    
-.. image:: https://readthedocs.org/projects/pydetex/badge/?version=latest
-    :target: https://pydetex.readthedocs.io
-    :alt: Documentation Status
-
-.. image:: https://codecov.io/gh/ppizarror/PyDetex/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/ppizarror/PyDetex
-    :alt: Codecov
-
-.. image:: https://img.shields.io/github/issues/ppizarror/PyDetex
-    :target: https://github.com/ppizarror/PyDetex/issues
-    :alt: Open issues
-
-.. image:: https://img.shields.io/pypi/dm/pydetex?color=purple
-    :target: https://pypi.org/project/pydetex
-    :alt: PyPi downloads
-
-.. image:: https://static.pepy.tech/personalized-badge/pydetex?period=total&units=international_system&left_color=grey&right_color=lightgrey&left_text=total%20downloads
-    :target: https://pepy.tech/project/pydetex
-    :alt: Total downloads
-    
-.. image:: https://img.shields.io/badge/buy%20me%20a-Ko--fi-02b9fe
-    :target: https://ko-fi.com/ppizarror
-    :alt: Buy me a Ko-fi
-
-Source repo on `GitHub <https://github.com/ppizarror/PyDetex>`_, 
-and run it on `Repl.it <https://repl.it/github/ppizarror/PyDetex>`_
-
-Introduction
-------------
-
-PyDetex is a Python application that transforms LaTeX code to plain text. It has multiple
-language support (15+), detects repeated words, offers a dictionary (synonyms, antonyms,
-definitions), and many things more to come!
-
-Comprehensive documentation for the latest version (if you plan to use the API)
-is available at https://pydetex.readthedocs.io
-
-Install Instructions
---------------------
-
-PyDetex can be installed via pip, for both MacOS, Windows & Linux. Simply run:
-
-.. code-block:: bash
-
-    $> python3 pip install pydetex -U
-
-Also, there're compiled binaries for Windows (x64) and macOS available through GitHub releases.
-
-Launch the GUI, or use the library
-----------------------------------
-
-Simply run this command anywhere to execute the application.
-
-.. code-block:: bash
-
-    $> python3 -m pydetex.gui
-
-.. figure:: https://raw.githubusercontent.com/ppizarror/pydetex/master/docs/_static/example_simple.png
-    :scale: 40%
-    :align: center
-
-    **(Simple Pipeline)** Tadada... !!! A simple GUI to process your LaTex, and paste into Google Docs, an email, or Grammarly ＼(^o^)／
-
-.. figure:: https://raw.githubusercontent.com/ppizarror/pydetex/master/docs/_static/example_strict.png
-    :scale: 40%
-    :align: center
-
-    **(Strict Pipeline)** The strict pipeline removes all commands, or replaces by some known tags.
-    
-
-.. figure:: https://raw.githubusercontent.com/ppizarror/pydetex/master/docs/_static/pydetex_windows.png
-    :scale: 40%
-    :align: center
-
-    Multiple options to configure: Check repeated words, highlight undetected code, or use different pipelines.
-
-You can also import the library, and use the parsers (methods that take latex code
-and perform a single task) or the pipelines (combination of parsers). For more
-information, visit the `documentation <https://pydetex.readthedocs.io>`_.
-
-.. code-block:: python
-
-    import pydetex.pipelines as pip
-    text = "This is a \\textbf{LaTex} code..."
-    out = pip.simple(text)
-
-TO-DOs
-------
-
-Currently, many things must be improved:
-
-- Add synthax checking for several languages, like `language-check <https://github.com/myint/language-check>`_.
-- Custom support for environments, such as *table*.
-
-Author
-------
-
-`Pablo Pizarro R. <https://ppizarror.com>`_ | 2021 - 2022
-
-
+=======
+PyDetex
+=======
+
+.. image:: https://img.shields.io/badge/author-Pablo%20Pizarro%20R.-lightgray.svg
+    :target: https://ppizarror.com
+    :alt: @ppizarror
+
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://opensource.org/licenses/MIT
+    :alt: License MIT
+
+.. image:: https://img.shields.io/badge/python-3.7+-red.svg
+    :target: https://www.python.org/downloads
+    :alt: Python 3.7+
+
+.. image:: https://badge.fury.io/py/pydetex.svg
+    :target: https://pypi.org/project/pydetex
+    :alt: PyPi package
+
+.. image:: https://img.shields.io/github/actions/workflow/status/ppizarror/PyDetex/ci.yml?branch=master
+    :target: https://github.com/ppizarror/PyDetex/actions/workflows/ci.yml
+    :alt: Build status
+    
+.. image:: https://app.fossa.com/api/projects/git%2Bgithub.com%2Fppizarror%2FPyDetex.svg?type=shield
+    :target: https://app.fossa.com/projects/git%2Bgithub.com%2Fppizarror%2FPyDetex?ref=badge_shield
+    :alt: FOSSA Status
+    
+.. image:: https://readthedocs.org/projects/pydetex/badge/?version=latest
+    :target: https://pydetex.readthedocs.io
+    :alt: Documentation Status
+
+.. image:: https://codecov.io/gh/ppizarror/PyDetex/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/ppizarror/PyDetex
+    :alt: Codecov
+
+.. image:: https://img.shields.io/github/issues/ppizarror/PyDetex
+    :target: https://github.com/ppizarror/PyDetex/issues
+    :alt: Open issues
+
+.. image:: https://img.shields.io/pypi/dm/pydetex?color=purple
+    :target: https://pypi.org/project/pydetex
+    :alt: PyPi downloads
+
+.. image:: https://static.pepy.tech/personalized-badge/pydetex?period=total&units=international_system&left_color=grey&right_color=lightgrey&left_text=total%20downloads
+    :target: https://pepy.tech/project/pydetex
+    :alt: Total downloads
+    
+.. image:: https://img.shields.io/badge/buy%20me%20a-Ko--fi-02b9fe
+    :target: https://ko-fi.com/ppizarror
+    :alt: Buy me a Ko-fi
+
+Source repo on `GitHub <https://github.com/ppizarror/PyDetex>`_, 
+and run it on `Repl.it <https://repl.it/github/ppizarror/PyDetex>`_
+
+Introduction
+------------
+
+PyDetex is a Python application that transforms LaTeX code to plain text. It has multiple
+language support (15+), detects repeated words, offers a dictionary (synonyms, antonyms,
+definitions), and many things more to come!
+
+Comprehensive documentation for the latest version (if you plan to use the API)
+is available at https://pydetex.readthedocs.io
+
+Install Instructions
+--------------------
+
+PyDetex can be installed via pip, for both MacOS, Windows & Linux. Simply run:
+
+.. code-block:: bash
+
+    $> python3 pip install pydetex -U
+
+Also, there're compiled binaries for Windows (x64) and macOS available through GitHub releases.
+
+Launch the GUI, or use the library
+----------------------------------
+
+Simply run this command anywhere to execute the application.
+
+.. code-block:: bash
+
+    $> python3 -m pydetex.gui
+
+.. figure:: https://raw.githubusercontent.com/ppizarror/pydetex/master/docs/_static/example_simple.png
+    :scale: 40%
+    :align: center
+
+    **(Simple Pipeline)** Tadada... !!! A simple GUI to process your LaTex, and paste into Google Docs, an email, or Grammarly ＼(^o^)／
+
+.. figure:: https://raw.githubusercontent.com/ppizarror/pydetex/master/docs/_static/example_strict.png
+    :scale: 40%
+    :align: center
+
+    **(Strict Pipeline)** The strict pipeline removes all commands, or replaces by some known tags.
+    
+
+.. figure:: https://raw.githubusercontent.com/ppizarror/pydetex/master/docs/_static/pydetex_windows.png
+    :scale: 40%
+    :align: center
+
+    Multiple options to configure: Check repeated words, highlight undetected code, or use different pipelines.
+
+You can also import the library, and use the parsers (methods that take latex code
+and perform a single task) or the pipelines (combination of parsers). For more
+information, visit the `documentation <https://pydetex.readthedocs.io>`_.
+
+.. code-block:: python
+
+    import pydetex.pipelines as pip
+    text = "This is a \\textbf{LaTex} code..."
+    out = pip.simple(text)
+
+TO-DOs
+------
+
+Currently, many things must be improved:
+
+- Add synthax checking for several languages, like `language-check <https://github.com/myint/language-check>`_.
+- Custom support for environments, such as *table*.
+
+Author
+------
+
+`Pablo Pizarro R. <https://ppizarror.com>`_ | 2021 - 2023
```

### Comparing `pydetex-0.9.9/pydetex.egg-info/SOURCES.txt` & `pydetex-1.0.0/pydetex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydetex-0.9.9/setup.py` & `pydetex-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""
-PyDetex
-https://github.com/ppizarror/PyDetex
-
-SETUP DISTRIBUTION
-Create setup for PyPI.
-"""
-
-from setuptools import setup, find_packages
-import pydetex
-
-# Load readme
-with open('README.rst', encoding='utf-8') as f:
-    long_description = f.read()
-
-# Load requirements
-with open('requirements.txt', encoding='utf-8') as f:
-    requirements = []
-    for line in f:
-        requirements.append(line.strip())
-
-# Setup library
-setup(
-    name=pydetex.__module_name__,
-    version=pydetex.__version__,
-    author=pydetex.__author__,
-    author_email=pydetex.__email__,
-    description=pydetex.__description__,
-    long_description=long_description,
-    url=pydetex.__url__,
-    project_urls={
-        'Bug Tracker': pydetex.__url_bug_tracker__,
-        'Documentation': pydetex.__url_documentation__,
-        'Source Code': pydetex.__url_source_code__
-    },
-    license=pydetex.__license__,
-    platforms=['any'],
-    keywords=pydetex.__keywords__,
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python',
-        'Topic :: Multimedia',
-        'Topic :: Text Processing'
-    ],
-    include_package_data=True,
-    packages=find_packages(exclude=['test']),
-    python_requires='>=3.7, <4',
-    install_requires=requirements,
-    extras_require={
-        'docs': ['sphinx', 'sphinx-autodoc-typehints>=1.2.0', 'sphinx-rtd-theme'],
-        'installer': ['pyinstaller==4.10'],
-        'test': ['codecov', 'nose2']
-    },
-    setup_requires=[
-        'setuptools',
-    ],
-    options={
-        'bdist_wheel': {'universal': False}
-    }
-)
+"""
+PyDetex
+https://github.com/ppizarror/PyDetex
+
+SETUP DISTRIBUTION
+Create setup for PyPI.
+"""
+
+from setuptools import setup, find_packages
+import pydetex
+
+# Load readme
+with open('README.rst', encoding='utf-8') as f:
+    long_description = f.read()
+
+# Load requirements
+with open('requirements.txt', encoding='utf-8') as f:
+    requirements = []
+    for line in f:
+        requirements.append(line.strip())
+
+# Setup library
+setup(
+    name=pydetex.__module_name__,
+    version=pydetex.__version__,
+    author=pydetex.__author__,
+    author_email=pydetex.__email__,
+    description=pydetex.__description__,
+    long_description=long_description,
+    url=pydetex.__url__,
+    project_urls={
+        'Bug Tracker': pydetex.__url_bug_tracker__,
+        'Documentation': pydetex.__url_documentation__,
+        'Source Code': pydetex.__url_source_code__
+    },
+    license=pydetex.__license__,
+    platforms=['any'],
+    keywords=pydetex.__keywords__,
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python',
+        'Topic :: Multimedia',
+        'Topic :: Text Processing'
+    ],
+    include_package_data=True,
+    packages=find_packages(exclude=['test']),
+    python_requires='>=3.7, <4',
+    install_requires=requirements,
+    extras_require={
+        'docs': ['sphinx', 'sphinx-autodoc-typehints>=1.2.0', 'sphinx-rtd-theme'],
+        'installer': ['pyinstaller==4.10'],
+        'test': ['nose2[coverage_plugin]']
+    },
+    setup_requires=[
+        'setuptools',
+    ],
+    options={
+        'bdist_wheel': {'universal': False}
+    }
+)
```

