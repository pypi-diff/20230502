# Comparing `tmp/dask_sphinx_theme-3.0.3.tar.gz` & `tmp/dask_sphinx_theme-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dask_sphinx_theme-3.0.3.tar", last modified: Thu Jun 16 17:16:15 2022, max compression
+gzip compressed data, was "dist/dask_sphinx_theme-3.0.4.tar", last modified: Tue May  2 18:43:36 2023, max compression
```

## Comparing `dask_sphinx_theme-3.0.3.tar` & `dask_sphinx_theme-3.0.4.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/_pygments/
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/_pygments/style.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/ext/
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/ext/dask_config_sphinx_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     5313 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/background-grid.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/dask-horizontal-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)    15086 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/icon-download.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/icon-expand.svg
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/icon-menu.svg
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 17:16:09.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-06-16 17:16:15.000000 dask_sphinx_theme-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80044 2022-06-16 17:15:56.000000 dask_sphinx_theme-3.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/_pygments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/_pygments/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/ext/dask_config_sphinx_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/background-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/dask-horizontal-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-menu.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/js/custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:43:23.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 18:43:36.000000 dask_sphinx_theme-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-02 18:43:18.000000 dask_sphinx_theme-3.0.4/versioneer.py
```

### Comparing `dask_sphinx_theme-3.0.3/LICENSE.txt` & `dask_sphinx_theme-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/PKG-INFO` & `dask_sphinx_theme-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: dask_sphinx_theme
-Version: 3.0.3
+Version: 3.0.4
 Summary: Dask theme for Sphinx
 Home-page: https://github.com/dask/dask-sphinx-theme/
 Author: Dask Developers
 Author-email: UNKNOWN
 License: BSD
 Description: Dask Sphinx Theme
         =================
```

### Comparing `dask_sphinx_theme-3.0.3/README.rst` & `dask_sphinx_theme-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/_pygments/style.py` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/_pygments/style.py`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/ext/dask_config_sphinx_ext.py` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/ext/dask_config_sphinx_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 def get_remote_yaml(url):
     r = requests.get(url)
     return yaml.safe_load(r.text)
 
 
 class DaskConfigDirective(Directive):
-
     option_spec = {
         "location": directives.unchanged,
         "schema": directives.uri,
         "config": directives.uri,
     }
 
     def run(self):
@@ -60,15 +59,14 @@
                 )
                 for k, v in value.items()
             ),
             [],
         )
 
     else:
-
         try:
             description = schema["description"]
             description = description.strip()
         except KeyError:
             description = "No Comment"
 
         if "dask." in prefix:
```

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/layout.html` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/css/style.css` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/css/style.css`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/background-grid.svg` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/background-grid.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/dask-horizontal-white.svg` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/dask-horizontal-white.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/favicon.ico` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/favicon.svg` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/icon-download.svg` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-download.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/icon-expand.svg` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-expand.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme/static/images/icon-menu.svg` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme/static/images/icon-menu.svg`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/PKG-INFO` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: dask-sphinx-theme
-Version: 3.0.3
+Version: 3.0.4
 Summary: Dask theme for Sphinx
 Home-page: https://github.com/dask/dask-sphinx-theme/
 Author: Dask Developers
 Author-email: UNKNOWN
 License: BSD
 Description: Dask Sphinx Theme
         =================
```

### Comparing `dask_sphinx_theme-3.0.3/dask_sphinx_theme.egg-info/SOURCES.txt` & `dask_sphinx_theme-3.0.4/dask_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 dask_sphinx_theme/static/css/style.css
 dask_sphinx_theme/static/images/background-grid.svg
 dask_sphinx_theme/static/images/dask-horizontal-white.svg
 dask_sphinx_theme/static/images/favicon.ico
 dask_sphinx_theme/static/images/favicon.svg
 dask_sphinx_theme/static/images/icon-download.svg
 dask_sphinx_theme/static/images/icon-expand.svg
-dask_sphinx_theme/static/images/icon-menu.svg
+dask_sphinx_theme/static/images/icon-menu.svg
+dask_sphinx_theme/static/js/custom.js
```

### Comparing `dask_sphinx_theme-3.0.3/setup.py` & `dask_sphinx_theme-3.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `dask_sphinx_theme-3.0.3/versioneer.py` & `dask_sphinx_theme-3.0.4/versioneer.py`

 * *Files identical despite different names*

