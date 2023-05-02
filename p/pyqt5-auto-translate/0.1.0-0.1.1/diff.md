# Comparing `tmp/pyqt5_auto_translate-0.1.0.tar.gz` & `tmp/pyqt5_auto_translate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5_auto_translate-0.1.0.tar", last modified: Tue May  2 05:42:13 2023, max compression
+gzip compressed data, was "pyqt5_auto_translate-0.1.1.tar", last modified: Tue May  2 06:29:47 2023, max compression
```

## Comparing `pyqt5_auto_translate-0.1.0.tar` & `pyqt5_auto_translate-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 05:42:13.085254 pyqt5_auto_translate-0.1.0/
--rw-rw-rw-   0        0        0     1083 2023-05-02 05:25:28.000000 pyqt5_auto_translate-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4943 2023-05-02 05:42:13.082266 pyqt5_auto_translate-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3989 2023-05-02 05:32:57.000000 pyqt5_auto_translate-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 05:42:13.073241 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/
--rw-rw-rw-   0        0        0    10319 2023-05-02 05:06:03.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/TranslatedItems.py
--rw-rw-rw-   0        0        0      661 2023-05-02 05:06:03.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-05-02 04:47:16.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/example.ui
--rw-rw-rw-   0        0        0     2650 2023-05-02 04:00:28.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/translations.yml
-drwxrwxrwx   0        0        0        0 2023-05-02 05:42:13.079244 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate.egg-info/
--rw-rw-rw-   0        0        0     4943 2023-05-02 05:42:13.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-05-02 05:42:13.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 05:42:13.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-02 05:42:13.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 05:42:13.000000 pyqt5_auto_translate-0.1.0/pyqt5_auto_translate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 05:42:13.086249 pyqt5_auto_translate-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1255 2023-05-02 05:22:59.000000 pyqt5_auto_translate-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 06:29:47.903210 pyqt5_auto_translate-0.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-05-02 05:25:28.000000 pyqt5_auto_translate-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9500 2023-05-02 06:29:47.902209 pyqt5_auto_translate-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8546 2023-05-02 06:28:57.000000 pyqt5_auto_translate-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 06:29:47.893209 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/
+-rw-rw-rw-   0        0        0    10319 2023-05-02 05:57:20.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/TranslatedItems.py
+-rw-rw-rw-   0        0        0      661 2023-05-02 05:06:03.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/__init__.py
+-rw-rw-rw-   0        0        0     1594 2023-05-02 04:47:16.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/example.ui
+-rw-rw-rw-   0        0        0     2650 2023-05-02 04:00:28.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/translations.yml
+drwxrwxrwx   0        0        0        0 2023-05-02 06:29:47.900209 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate.egg-info/
+-rw-rw-rw-   0        0        0     9500 2023-05-02 06:29:47.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-05-02 06:29:47.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 06:29:47.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-02 06:29:47.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 06:29:47.000000 pyqt5_auto_translate-0.1.1/pyqt5_auto_translate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 06:29:47.903210 pyqt5_auto_translate-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2023-05-02 06:29:46.000000 pyqt5_auto_translate-0.1.1/setup.py
```

### Comparing `pyqt5_auto_translate-0.1.0/LICENSE` & `pyqt5_auto_translate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/TranslatedItems.py` & `pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/TranslatedItems.py`

 * *Files identical despite different names*

### Comparing `pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/__init__.py` & `pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/example.ui` & `pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/example.ui`

 * *Files identical despite different names*

### Comparing `pyqt5_auto_translate-0.1.0/pyqt5_auto_translate/translations.yml` & `pyqt5_auto_translate-0.1.1/pyqt5_auto_translate/translations.yml`

 * *Files identical despite different names*

### Comparing `pyqt5_auto_translate-0.1.0/setup.py` & `pyqt5_auto_translate-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyqt5_auto_translate",
-    version="0.1.0",
+    version="0.1.1",
     description="A lightweight and easy-to-use library for automating the translation of PyQt5 widgets.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="RunJi",
     author_email="ryanlee02@foxmail.com",
     url="https://github.com/LiRunJi/pyqt5_auto_translate",
     packages=find_packages(),
```

