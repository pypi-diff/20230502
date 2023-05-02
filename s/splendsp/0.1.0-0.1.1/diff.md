# Comparing `tmp/splendsp-0.1.0.tar.gz` & `tmp/splendsp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splendsp-0.1.0.tar", last modified: Wed Dec  7 16:43:05 2022, max compression
+gzip compressed data, was "splendsp-0.1.1.tar", last modified: Tue May  2 20:33:46 2023, max compression
```

## Comparing `splendsp-0.1.0.tar` & `splendsp-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-12-07 16:42:49.000000 splendsp-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2022-12-07 16:42:49.000000 splendsp-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-07 16:42:49.000000 splendsp-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2022-12-07 16:43:05.341559 splendsp-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-07 16:42:49.000000 splendsp-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-07 16:42:49.000000 splendsp-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-07 16:43:05.345559 splendsp-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-07 16:42:49.000000 splendsp-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/src/splendsp/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-07 16:43:05.000000 splendsp-0.1.0/src/splendsp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/src/splendsp/cut/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/cut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28326 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/cut/_cut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/src/splendsp/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/dsp/_de_pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)    60035 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/dsp/_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/dsp/_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/dsp/_of_pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2022-12-07 16:42:49.000000 splendsp-0.1.0/src/splendsp/dsp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 16:43:05.341559 splendsp-0.1.0/src/splendsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2022-12-07 16:43:05.000000 splendsp-0.1.0/src/splendsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-07 16:43:05.000000 splendsp-0.1.0/src/splendsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 16:43:05.000000 splendsp-0.1.0/src/splendsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 16:43:05.000000 splendsp-0.1.0/src/splendsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-07 16:43:05.000000 splendsp-0.1.0/src/splendsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-07 16:43:05.000000 splendsp-0.1.0/src/splendsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.522652 splendsp-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.518651 splendsp-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.522652 splendsp-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-02 20:33:30.000000 splendsp-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-02 20:33:30.000000 splendsp-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-02 20:33:30.000000 splendsp-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 20:33:46.522652 splendsp-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 20:33:30.000000 splendsp-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 20:33:30.000000 splendsp-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-02 20:33:46.522652 splendsp-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 20:33:30.000000 splendsp-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.518651 splendsp-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.522652 splendsp-0.1.1/src/splendsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 20:33:46.000000 splendsp-0.1.1/src/splendsp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.522652 splendsp-0.1.1/src/splendsp/cut/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/cut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28326 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/cut/_cut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.522652 splendsp-0.1.1/src/splendsp/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/dsp/_de_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60035 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/dsp/_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/dsp/_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/dsp/_of_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-02 20:33:30.000000 splendsp-0.1.1/src/splendsp/dsp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:33:46.522652 splendsp-0.1.1/src/splendsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 20:33:46.000000 splendsp-0.1.1/src/splendsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-02 20:33:46.000000 splendsp-0.1.1/src/splendsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:33:46.000000 splendsp-0.1.1/src/splendsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:33:46.000000 splendsp-0.1.1/src/splendsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 20:33:46.000000 splendsp-0.1.1/src/splendsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 20:33:46.000000 splendsp-0.1.1/src/splendsp.egg-info/top_level.txt
```

### Comparing `splendsp-0.1.0/.github/workflows/python-publish.yml` & `splendsp-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/.gitignore` & `splendsp-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/LICENSE` & `splendsp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/PKG-INFO` & `splendsp-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: splendsp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Splendid Digital Signal Processing of time series data for small physics experiments
 Home-page: https://github.com/splendor-collab/splendsp
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `splendsp`
 
-[![Python package](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml/badge.svg)](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendsp)](https://pypi.org/project/splendsp/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendsp)](https://github.com/splendor-collab/splendsp/blob/main/LICENSE)
+[![Python publish](https://github.com/splendor-collab/splendsp/actions/workflows/python-publish.yml/badge.svg)](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendsp)](https://pypi.org/project/splendsp/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendsp)](https://github.com/splendor-collab/splendsp/blob/main/LICENSE)
 
  Splendid Digital Signal Processing of time series data for small physics experiments.
```

### Comparing `splendsp-0.1.0/README.md` & `splendsp-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 # `splendsp`
 
-[![Python package](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml/badge.svg)](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendsp)](https://pypi.org/project/splendsp/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendsp)](https://github.com/splendor-collab/splendsp/blob/main/LICENSE)
+[![Python publish](https://github.com/splendor-collab/splendsp/actions/workflows/python-publish.yml/badge.svg)](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendsp)](https://pypi.org/project/splendsp/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendsp)](https://github.com/splendor-collab/splendsp/blob/main/LICENSE)
 
  Splendid Digital Signal Processing of time series data for small physics experiments.
- 
+
```

### Comparing `splendsp-0.1.0/setup.cfg` & `splendsp-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	scipy
 	matplotlib
+	astropy
 python_requires = >=3.6
 package_dir = 
 	= src
 zip_safe = False
 
 [options.packages.find]
 where = src
```

### Comparing `splendsp-0.1.0/src/splendsp/cut/_cut.py` & `splendsp-0.1.1/src/splendsp/cut/_cut.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/src/splendsp/dsp/_de_pileup.py` & `splendsp-0.1.1/src/splendsp/dsp/_de_pileup.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/src/splendsp/dsp/_fitting.py` & `splendsp-0.1.1/src/splendsp/dsp/_fitting.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/src/splendsp/dsp/_noise.py` & `splendsp-0.1.1/src/splendsp/dsp/_noise.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/src/splendsp/dsp/_of_pileup.py` & `splendsp-0.1.1/src/splendsp/dsp/_of_pileup.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/src/splendsp/dsp/_utils.py` & `splendsp-0.1.1/src/splendsp/dsp/_utils.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.1.0/src/splendsp.egg-info/PKG-INFO` & `splendsp-0.1.1/src/splendsp.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: splendsp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Splendid Digital Signal Processing of time series data for small physics experiments
 Home-page: https://github.com/splendor-collab/splendsp
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `splendsp`
 
-[![Python package](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml/badge.svg)](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendsp)](https://pypi.org/project/splendsp/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendsp)](https://github.com/splendor-collab/splendsp/blob/main/LICENSE)
+[![Python publish](https://github.com/splendor-collab/splendsp/actions/workflows/python-publish.yml/badge.svg)](https://github.com/splendor-collab/splendsp/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendsp)](https://pypi.org/project/splendsp/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendsp)](https://github.com/splendor-collab/splendsp/blob/main/LICENSE)
 
  Splendid Digital Signal Processing of time series data for small physics experiments.
```

### Comparing `splendsp-0.1.0/src/splendsp.egg-info/SOURCES.txt` & `splendsp-0.1.1/src/splendsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

