# Comparing `tmp/photo_burst_detection-1.0.0.tar.gz` & `tmp/photo_burst_detection-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photo_burst_detection-1.0.0.tar", last modified: Sat Apr  1 07:59:46 2023, max compression
+gzip compressed data, was "photo_burst_detection-1.1.0.tar", last modified: Tue May  2 08:55:06 2023, max compression
```

## Comparing `photo_burst_detection-1.0.0.tar` & `photo_burst_detection-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:59:46.073042 photo_burst_detection-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-01 07:59:46.073042 photo_burst_detection-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:59:46.069042 photo_burst_detection-1.0.0/photo_burst_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:59:46.069042 photo_burst_detection-1.0.0/photo_burst_detection/static/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:59:46.073042 photo_burst_detection-1.0.0/photo_burst_detection/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/templates/burst.html
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/templates/naming.html
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/photo_burst_detection/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 07:59:46.069042 photo_burst_detection-1.0.0/photo_burst_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-01 07:59:46.000000 photo_burst_detection-1.0.0/photo_burst_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-01 07:59:46.000000 photo_burst_detection-1.0.0/photo_burst_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 07:59:46.000000 photo_burst_detection-1.0.0/photo_burst_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 07:59:46.000000 photo_burst_detection-1.0.0/photo_burst_detection.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-01 07:59:46.000000 photo_burst_detection-1.0.0/photo_burst_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-01 07:59:46.000000 photo_burst_detection-1.0.0/photo_burst_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 07:59:46.073042 photo_burst_detection-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-01 07:59:36.000000 photo_burst_detection-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:55:06.669518 photo_burst_detection-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-02 08:55:06.669518 photo_burst_detection-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:55:06.665518 photo_burst_detection-1.1.0/photo_burst_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:55:06.669518 photo_burst_detection-1.1.0/photo_burst_detection/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:55:06.669518 photo_burst_detection-1.1.0/photo_burst_detection/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/templates/burst.html
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/templates/naming.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/photo_burst_detection/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:55:06.669518 photo_burst_detection-1.1.0/photo_burst_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-02 08:55:06.000000 photo_burst_detection-1.1.0/photo_burst_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-02 08:55:06.000000 photo_burst_detection-1.1.0/photo_burst_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:55:06.000000 photo_burst_detection-1.1.0/photo_burst_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:55:06.000000 photo_burst_detection-1.1.0/photo_burst_detection.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 08:55:06.000000 photo_burst_detection-1.1.0/photo_burst_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 08:55:06.000000 photo_burst_detection-1.1.0/photo_burst_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:55:06.669518 photo_burst_detection-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 08:54:52.000000 photo_burst_detection-1.1.0/setup.py
```

### Comparing `photo_burst_detection-1.0.0/PKG-INFO` & `photo_burst_detection-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo_burst_detection
-Version: 1.0.0
+Version: 1.1.0
 Summary: Flask App for photo burst detection
 Home-page: https://gitlab.com/batou9150/photo_burst_detection
 Author: batou9150
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `photo_burst_detection-1.0.0/README.md` & `photo_burst_detection-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/auth.py` & `photo_burst_detection-1.1.0/photo_burst_detection/auth.py`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/conf.py` & `photo_burst_detection-1.1.0/photo_burst_detection/conf.py`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/scan.py` & `photo_burst_detection-1.1.0/photo_burst_detection/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         results = []
         for root, dirs, files in os.walk(self.path):
             if root != self.path and not root.lower().endswith('video') and len(files) > 0:
                 results.append({'directory': self.get_link(root),
                                 'prefix': {extract_prefix(f) for f in files if not f.startswith('.')},
                                 'extension': {os.path.splitext(f)[1] for f in files if not f.startswith('.')},
                                 })
-        return results
+        return sorted(results, key=lambda x: x['directory'])
 
     def get_bursts(self, path, seconds=2):
         prev_date = datetime(1970, 1, 1)
         prev_file = None
 
         pathname = self.get_fullpath(path, '*.jpg')
         self.logger.info(f'Scanner:get_bursts from {pathname}')
```

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/static/favicon.svg` & `photo_burst_detection-1.1.0/photo_burst_detection/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/static/style.css` & `photo_burst_detection-1.1.0/photo_burst_detection/static/style.css`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/templates/burst.html` & `photo_burst_detection-1.1.0/photo_burst_detection/templates/burst.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/templates/index.html` & `photo_burst_detection-1.1.0/photo_burst_detection/templates/index.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/templates/layout.html` & `photo_burst_detection-1.1.0/photo_burst_detection/templates/layout.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/templates/login.html` & `photo_burst_detection-1.1.0/photo_burst_detection/templates/login.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/templates/naming.html` & `photo_burst_detection-1.1.0/photo_burst_detection/templates/naming.html`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection/views.py` & `photo_burst_detection-1.1.0/photo_burst_detection/views.py`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection.egg-info/PKG-INFO` & `photo_burst_detection-1.1.0/photo_burst_detection.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo-burst-detection
-Version: 1.0.0
+Version: 1.1.0
 Summary: Flask App for photo burst detection
 Home-page: https://gitlab.com/batou9150/photo_burst_detection
 Author: batou9150
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `photo_burst_detection-1.0.0/photo_burst_detection.egg-info/SOURCES.txt` & `photo_burst_detection-1.1.0/photo_burst_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `photo_burst_detection-1.0.0/setup.py` & `photo_burst_detection-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
+import os
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='photo_burst_detection',
-    version='1.0.0',
+    version=os.environ.get('GITHUB_REF_NAME', '0.0.0'),
     author='batou9150',
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'flask',
         'flask-login',
```

