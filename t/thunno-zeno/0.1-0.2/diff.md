# Comparing `tmp/thunno-zeno-0.1.tar.gz` & `tmp/thunno-zeno-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno-zeno-0.1.tar", last modified: Tue May  2 13:56:00 2023, max compression
+gzip compressed data, was "thunno-zeno-0.2.tar", last modified: Tue May  2 13:58:04 2023, max compression
```

## Comparing `thunno-zeno-0.1.tar` & `thunno-zeno-0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-02 13:56:00.001341 thunno-zeno-0.1/
--rw-r--r--   0 nayak      (501) staff       (20)      939 2023-05-02 13:56:00.001218 thunno-zeno-0.1/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-02 13:56:00.001378 thunno-zeno-0.1/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1286 2023-05-02 13:55:14.000000 thunno-zeno-0.1/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-02 13:56:00.001047 thunno-zeno-0.1/thunno_zeno.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      939 2023-05-02 13:55:59.000000 thunno-zeno-0.1/thunno_zeno.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      220 2023-05-02 13:55:59.000000 thunno-zeno-0.1/thunno_zeno.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-02 13:55:59.000000 thunno-zeno-0.1/thunno_zeno.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       41 2023-05-02 13:55:59.000000 thunno-zeno-0.1/thunno_zeno.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)       15 2023-05-02 13:55:59.000000 thunno-zeno-0.1/thunno_zeno.egg-info/requires.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-02 13:55:59.000000 thunno-zeno-0.1/thunno_zeno.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-02 13:58:04.979997 thunno-zeno-0.2/
+-rw-r--r--   0 nayak      (501) staff       (20)      939 2023-05-02 13:58:04.979864 thunno-zeno-0.2/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-02 13:58:04.980037 thunno-zeno-0.2/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1286 2023-05-02 13:57:46.000000 thunno-zeno-0.2/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-02 13:58:04.979475 thunno-zeno-0.2/thunno_zeno.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      939 2023-05-02 13:58:04.000000 thunno-zeno-0.2/thunno_zeno.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      250 2023-05-02 13:58:04.000000 thunno-zeno-0.2/thunno_zeno.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-02 13:58:04.000000 thunno-zeno-0.2/thunno_zeno.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       41 2023-05-02 13:58:04.000000 thunno-zeno-0.2/thunno_zeno.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       15 2023-05-02 13:58:04.000000 thunno-zeno-0.2/thunno_zeno.egg-info/requires.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        5 2023-05-02 13:58:04.000000 thunno-zeno-0.2/thunno_zeno.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-02 13:58:04.979696 thunno-zeno-0.2/zeno/
+-rw-r--r--   0 nayak      (501) staff       (20)       19 2023-05-02 13:57:38.000000 thunno-zeno-0.2/zeno/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4076 2023-05-02 13:55:14.000000 thunno-zeno-0.2/zeno/main.py
```

### Comparing `thunno-zeno-0.1/PKG-INFO` & `thunno-zeno-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno-zeno
-Version: 0.1
+Version: 0.2
 Summary: Thunno 2 interpreter
 Home-page: https://github.com/Thunno/Zeno
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: CC0
-Download-URL: https://github.com/Thunno/Zeno/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/Thunno/Zeno/archive/refs/tags/v0.2.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno-zeno-0.1/setup.py` & `thunno-zeno-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-ZENO_VERSION = "0.1"
+ZENO_VERSION = "0.2"
 
 long_description = (
     "Zeno is an intepreter for Thunno 2. Read more at https://github.com/Thunno/Zeno"
 )
 
 setup(
     name="thunno-zeno",
```

### Comparing `thunno-zeno-0.1/thunno_zeno.egg-info/PKG-INFO` & `thunno-zeno-0.2/thunno_zeno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno-zeno
-Version: 0.1
+Version: 0.2
 Summary: Thunno 2 interpreter
 Home-page: https://github.com/Thunno/Zeno
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: CC0
-Download-URL: https://github.com/Thunno/Zeno/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/Thunno/Zeno/archive/refs/tags/v0.2.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

