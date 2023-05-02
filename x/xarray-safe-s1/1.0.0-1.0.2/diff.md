# Comparing `tmp/xarray-safe-s1-1.0.0.tar.gz` & `tmp/xarray-safe-s1-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-safe-s1-1.0.0.tar", last modified: Tue May  2 09:35:13 2023, max compression
+gzip compressed data, was "xarray-safe-s1-1.0.2.tar", last modified: Tue May  2 12:20:21 2023, max compression
```

## Comparing `xarray-safe-s1-1.0.0.tar` & `xarray-safe-s1-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 09:35:13.620565 xarray-safe-s1-1.0.0/
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      349 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.0/.flake8
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      210 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.0/.gitignore
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      958 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      418 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.0/.readthedocs.yml
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     1084 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.0/LICENSE
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      117 2023-05-02 09:35:13.620565 xarray-safe-s1-1.0.0/PKG-INFO
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     7357 2023-05-02 09:29:43.000000 xarray-safe-s1-1.0.0/README.md
-drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 09:35:13.556564 xarray-safe-s1-1.0.0/ci/
-drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 09:35:13.576565 xarray-safe-s1-1.0.0/ci/requirements/
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      146 2023-04-24 14:13:29.000000 xarray-safe-s1-1.0.0/ci/requirements/docs.yaml
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      534 2023-04-28 12:20:08.000000 xarray-safe-s1-1.0.0/ci/requirements/environment.yaml
-drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 09:35:13.592565 xarray-safe-s1-1.0.0/docs/
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      634 2023-04-28 13:19:21.000000 xarray-safe-s1-1.0.0/docs/Makefile
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      146 2023-05-02 08:16:18.000000 xarray-safe-s1-1.0.0/docs/api.rst
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     2569 2023-05-02 08:17:33.000000 xarray-safe-s1-1.0.0/docs/conf.py
-drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 09:35:13.596565 xarray-safe-s1-1.0.0/docs/examples/
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)    10471 2023-05-02 09:29:49.000000 xarray-safe-s1-1.0.0/docs/examples/simple_tutorial.ipynb
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     2292 2023-05-02 09:27:50.000000 xarray-safe-s1-1.0.0/docs/index.rst
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      698 2023-05-02 07:07:22.000000 xarray-safe-s1-1.0.0/docs/installing.rst
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      800 2023-04-28 13:19:21.000000 xarray-safe-s1-1.0.0/docs/make.bat
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)       36 2023-05-02 09:30:09.000000 xarray-safe-s1-1.0.0/docs/requirements.txt
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      670 2023-05-02 09:24:23.000000 xarray-safe-s1-1.0.0/pyproject.toml
-drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 09:35:13.608565 xarray-safe-s1-1.0.0/safe_s1/
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      162 2023-05-02 09:08:17.000000 xarray-safe-s1-1.0.0/safe_s1/__init__.py
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)    26996 2023-05-02 08:18:56.000000 xarray-safe-s1-1.0.0/safe_s1/metadata.py
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)    41424 2023-05-02 09:26:30.000000 xarray-safe-s1-1.0.0/safe_s1/sentinel1_xml_mappings.py
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     5503 2023-04-28 09:31:19.000000 xarray-safe-s1-1.0.0/safe_s1/xml_parser.py
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)       38 2023-05-02 09:35:13.624565 xarray-safe-s1-1.0.0/setup.cfg
-drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 09:35:13.620565 xarray-safe-s1-1.0.0/xarray_safe_s1.egg-info/
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      117 2023-05-02 09:35:13.000000 xarray-safe-s1-1.0.0/xarray_safe_s1.egg-info/PKG-INFO
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      583 2023-05-02 09:35:13.000000 xarray-safe-s1-1.0.0/xarray_safe_s1.egg-info/SOURCES.txt
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)        1 2023-05-02 09:35:13.000000 xarray-safe-s1-1.0.0/xarray_safe_s1.egg-info/dependency_links.txt
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      113 2023-05-02 09:35:13.000000 xarray-safe-s1-1.0.0/xarray_safe_s1.egg-info/requires.txt
--rw-r--r--   0 reynaudy (504160) ditiisi  (10004)        8 2023-05-02 09:35:13.000000 xarray-safe-s1-1.0.0/xarray_safe_s1.egg-info/top_level.txt
+drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 12:20:21.313159 xarray-safe-s1-1.0.2/
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      349 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.2/.flake8
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      210 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.2/.gitignore
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      958 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      418 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.2/.readthedocs.yml
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     1084 2023-04-19 13:51:55.000000 xarray-safe-s1-1.0.2/LICENSE
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      117 2023-05-02 12:20:21.313159 xarray-safe-s1-1.0.2/PKG-INFO
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     7356 2023-05-02 12:09:53.000000 xarray-safe-s1-1.0.2/README.md
+drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 12:20:21.225158 xarray-safe-s1-1.0.2/ci/
+drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 12:20:21.257158 xarray-safe-s1-1.0.2/ci/requirements/
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      146 2023-04-24 14:13:29.000000 xarray-safe-s1-1.0.2/ci/requirements/docs.yaml
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      534 2023-04-28 12:20:08.000000 xarray-safe-s1-1.0.2/ci/requirements/environment.yaml
+drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 12:20:21.273158 xarray-safe-s1-1.0.2/docs/
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      634 2023-04-28 13:19:21.000000 xarray-safe-s1-1.0.2/docs/Makefile
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      146 2023-05-02 08:16:18.000000 xarray-safe-s1-1.0.2/docs/api.rst
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     2569 2023-05-02 08:17:33.000000 xarray-safe-s1-1.0.2/docs/conf.py
+drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 12:20:21.277158 xarray-safe-s1-1.0.2/docs/examples/
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)    10471 2023-05-02 09:29:49.000000 xarray-safe-s1-1.0.2/docs/examples/simple_tutorial.ipynb
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     2292 2023-05-02 09:27:50.000000 xarray-safe-s1-1.0.2/docs/index.rst
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      698 2023-05-02 07:07:22.000000 xarray-safe-s1-1.0.2/docs/installing.rst
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      800 2023-04-28 13:19:21.000000 xarray-safe-s1-1.0.2/docs/make.bat
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)       36 2023-05-02 09:30:09.000000 xarray-safe-s1-1.0.2/docs/requirements.txt
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      670 2023-05-02 09:24:23.000000 xarray-safe-s1-1.0.2/pyproject.toml
+drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 12:20:21.297159 xarray-safe-s1-1.0.2/safe_s1/
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      162 2023-05-02 09:08:17.000000 xarray-safe-s1-1.0.2/safe_s1/__init__.py
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)    26996 2023-05-02 08:18:56.000000 xarray-safe-s1-1.0.2/safe_s1/metadata.py
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)    41424 2023-05-02 09:26:30.000000 xarray-safe-s1-1.0.2/safe_s1/sentinel1_xml_mappings.py
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)     5503 2023-04-28 09:31:19.000000 xarray-safe-s1-1.0.2/safe_s1/xml_parser.py
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)       38 2023-05-02 12:20:21.313159 xarray-safe-s1-1.0.2/setup.cfg
+drwxr-xr-x   0 reynaudy (504160) ditiisi  (10004)        0 2023-05-02 12:20:21.309159 xarray-safe-s1-1.0.2/xarray_safe_s1.egg-info/
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      117 2023-05-02 12:20:21.000000 xarray-safe-s1-1.0.2/xarray_safe_s1.egg-info/PKG-INFO
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      583 2023-05-02 12:20:21.000000 xarray-safe-s1-1.0.2/xarray_safe_s1.egg-info/SOURCES.txt
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)        1 2023-05-02 12:20:21.000000 xarray-safe-s1-1.0.2/xarray_safe_s1.egg-info/dependency_links.txt
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)      113 2023-05-02 12:20:21.000000 xarray-safe-s1-1.0.2/xarray_safe_s1.egg-info/requires.txt
+-rw-r--r--   0 reynaudy (504160) ditiisi  (10004)        8 2023-05-02 12:20:21.000000 xarray-safe-s1-1.0.2/xarray_safe_s1.egg-info/top_level.txt
```

### Comparing `xarray-safe-s1-1.0.0/.pre-commit-config.yaml` & `xarray-safe-s1-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/LICENSE` & `xarray-safe-s1-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/README.md` & `xarray-safe-s1-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ```
 conda create -n safe_s1
 conda activate safe_s1
 pip install xarray-safe-s1
 ```
 
 
-```python
+```pycon
 >>> from safe_s1 import Sentinel1Reader, sentinel1_xml_mappings
 >>> filename = sentinel1_xml_mappings.get_test_file('S1A_IW_GRDH_1SDV_20170907T103020_20170907T103045_018268_01EB76_Z010.SAFE')
 >>> Sentinel1Reader(filename).datatree
 
 DataTree('None', parent=None)
 ├── DataTree('geolocationGrid')
 │       Dimensions:         (line: 10, sample: 21)
```

### Comparing `xarray-safe-s1-1.0.0/ci/requirements/environment.yaml` & `xarray-safe-s1-1.0.2/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/docs/Makefile` & `xarray-safe-s1-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/docs/conf.py` & `xarray-safe-s1-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/docs/examples/simple_tutorial.ipynb` & `xarray-safe-s1-1.0.2/docs/examples/simple_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/docs/index.rst` & `xarray-safe-s1-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/docs/installing.rst` & `xarray-safe-s1-1.0.2/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/docs/make.bat` & `xarray-safe-s1-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/pyproject.toml` & `xarray-safe-s1-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/safe_s1/metadata.py` & `xarray-safe-s1-1.0.2/safe_s1/metadata.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/safe_s1/sentinel1_xml_mappings.py` & `xarray-safe-s1-1.0.2/safe_s1/sentinel1_xml_mappings.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/safe_s1/xml_parser.py` & `xarray-safe-s1-1.0.2/safe_s1/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-1.0.0/xarray_safe_s1.egg-info/SOURCES.txt` & `xarray-safe-s1-1.0.2/xarray_safe_s1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

