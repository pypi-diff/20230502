# Comparing `tmp/scooby-0.7.1.tar.gz` & `tmp/scooby-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scooby-0.7.1.tar", last modified: Wed Jan 25 00:33:42 2023, max compression
+gzip compressed data, was "scooby-0.7.2.tar", last modified: Tue May  2 16:21:22 2023, max compression
```

## Comparing `scooby-0.7.1.tar` & `scooby-0.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:33:42.527969 scooby-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-25 00:33:32.000000 scooby-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-01-25 00:33:42.527969 scooby-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-01-25 00:33:32.000000 scooby-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:33:42.527969 scooby-0.7.1/scooby/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-25 00:33:32.000000 scooby-0.7.1/scooby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-01-25 00:33:32.000000 scooby-0.7.1/scooby/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-01-25 00:33:32.000000 scooby-0.7.1/scooby/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-01-25 00:33:32.000000 scooby-0.7.1/scooby/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-01-25 00:33:32.000000 scooby-0.7.1/scooby/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-25 00:33:42.000000 scooby-0.7.1/scooby/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:33:42.527969 scooby-0.7.1/scooby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-01-25 00:33:42.000000 scooby-0.7.1/scooby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-25 00:33:42.000000 scooby-0.7.1/scooby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 00:33:42.000000 scooby-0.7.1/scooby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-25 00:33:42.000000 scooby-0.7.1/scooby.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-25 00:33:42.000000 scooby-0.7.1/scooby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-25 00:33:42.000000 scooby-0.7.1/scooby.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 00:33:42.527969 scooby-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-01-25 00:33:32.000000 scooby-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:21:22.640624 scooby-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-02 16:21:06.000000 scooby-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-02 16:21:22.640624 scooby-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-05-02 16:21:06.000000 scooby-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:21:22.640624 scooby-0.7.2/scooby/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-02 16:21:06.000000 scooby-0.7.2/scooby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-02 16:21:06.000000 scooby-0.7.2/scooby/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-02 16:21:06.000000 scooby-0.7.2/scooby/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-05-02 16:21:06.000000 scooby-0.7.2/scooby/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-02 16:21:06.000000 scooby-0.7.2/scooby/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 16:21:22.000000 scooby-0.7.2/scooby/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:21:22.640624 scooby-0.7.2/scooby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-02 16:21:22.000000 scooby-0.7.2/scooby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-02 16:21:22.000000 scooby-0.7.2/scooby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:21:22.000000 scooby-0.7.2/scooby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 16:21:22.000000 scooby-0.7.2/scooby.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 16:21:22.000000 scooby-0.7.2/scooby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 16:21:22.000000 scooby-0.7.2/scooby.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:21:22.640624 scooby-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-02 16:21:06.000000 scooby-0.7.2/setup.py
```

### Comparing `scooby-0.7.1/LICENSE` & `scooby-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scooby-0.7.1/PKG-INFO` & `scooby-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: scooby
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Great Dane turned Python environment detective
 Home-page: https://github.com/banesullivan/scooby
 Author: Dieter Werthmüller, Bane Sullivan, Alex Kaszynski, and contributors
 Author-email: info@pyvista.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
 License-File: LICENSE
 
 # 🐶🕵️ Scooby
 
 [![Tests](https://github.com/banesullivan/scooby/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/banesullivan/scooby/actions/workflows/pythonpackage.yml)
```

### Comparing `scooby-0.7.1/README.md` & `scooby-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `scooby-0.7.1/scooby/__init__.py` & `scooby-0.7.2/scooby/__init__.py`

 * *Files identical despite different names*

### Comparing `scooby-0.7.1/scooby/__main__.py` & `scooby-0.7.2/scooby/__main__.py`

 * *Files identical despite different names*

### Comparing `scooby-0.7.1/scooby/knowledge.py` & `scooby-0.7.2/scooby/knowledge.py`

 * *Files identical despite different names*

### Comparing `scooby-0.7.1/scooby/report.py` & `scooby-0.7.2/scooby/report.py`

 * *Files identical despite different names*

### Comparing `scooby-0.7.1/scooby/tracker.py` & `scooby-0.7.2/scooby/tracker.py`

 * *Files identical despite different names*

### Comparing `scooby-0.7.1/scooby.egg-info/PKG-INFO` & `scooby-0.7.2/scooby.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: scooby
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Great Dane turned Python environment detective
 Home-page: https://github.com/banesullivan/scooby
 Author: Dieter Werthmüller, Bane Sullivan, Alex Kaszynski, and contributors
 Author-email: info@pyvista.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
 License-File: LICENSE
 
 # 🐶🕵️ Scooby
 
 [![Tests](https://github.com/banesullivan/scooby/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/banesullivan/scooby/actions/workflows/pythonpackage.yml)
```

### Comparing `scooby-0.7.1/setup.py` & `scooby-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,24 @@
     url="https://github.com/banesullivan/scooby",
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
             "scooby=scooby.__main__:main",
         ],
     },
-    classifiers=(
+    classifiers=[
         "Programming Language :: Python",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        'Intended Audience :: Science/Research',
-        'Natural Language :: English',
-    ),
-    python_requires='>=3.7.*',
+        "Intended Audience :: Science/Research",
+        "Natural Language :: English",
+    ],
+    python_requires=">=3.7",
     extras_require={
-        'cpu': ['psutil', 'mkl'],
-        # 'gpu': [], # TODO: what's needed?
+        "cpu": ["psutil", "mkl"],
     },
     use_scm_version={
         "root": ".",
         "relative_to": __file__,
         "write_to": os.path.join("scooby", "version.py"),
     },
     setup_requires=["setuptools_scm"],
```

