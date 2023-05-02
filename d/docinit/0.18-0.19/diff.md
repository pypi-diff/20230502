# Comparing `tmp/docinit-0.18.tar.gz` & `tmp/docinit-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docinit-0.18.tar", last modified: Tue Apr 25 17:30:34 2023, max compression
+gzip compressed data, was "docinit-0.19.tar", last modified: Tue May  2 14:50:06 2023, max compression
```

## Comparing `docinit-0.18.tar` & `docinit-0.19.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.007397 docinit-0.18/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:33.995396 docinit-0.18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:33.999396 docinit-0.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-25 17:30:15.000000 docinit-0.18/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-25 17:30:15.000000 docinit-0.18/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-25 17:30:15.000000 docinit-0.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 17:30:15.000000 docinit-0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 17:30:15.000000 docinit-0.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-04-25 17:30:34.007397 docinit-0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-04-25 17:30:15.000000 docinit-0.18/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.003397 docinit-0.18/docinit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:15.000000 docinit-0.18/docinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-25 17:30:15.000000 docinit-0.18/docinit/docinit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.003397 docinit-0.18/docinit/skeleton/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.003397 docinit-0.18/docinit/skeleton/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_ext/includefirst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.003397 docinit-0.18/docinit/skeleton/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_static/back.js
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_static/docinit.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.007397 docinit-0.18/docinit/skeleton/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.007397 docinit-0.18/docinit/skeleton/_templates/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_templates/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.007397 docinit-0.18/docinit/skeleton/_templates/autoapi/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_templates/autoapi/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/default.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-25 17:30:15.000000 docinit-0.18/docinit/skeleton/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.003397 docinit-0.18/docinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-04-25 17:30:33.000000 docinit-0.18/docinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-25 17:30:33.000000 docinit-0.18/docinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:30:33.000000 docinit-0.18/docinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 17:30:33.000000 docinit-0.18/docinit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 17:30:33.000000 docinit-0.18/docinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 17:30:33.000000 docinit-0.18/docinit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-25 17:30:15.000000 docinit-0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-25 17:30:34.007397 docinit-0.18/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:34.007397 docinit-0.18/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:30:15.000000 docinit-0.18/test/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-25 17:30:15.000000 docinit-0.18/test/test_docinit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.987977 docinit-0.19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.979977 docinit-0.19/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.983977 docinit-0.19/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 14:49:50.000000 docinit-0.19/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-02 14:49:50.000000 docinit-0.19/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-02 14:49:50.000000 docinit-0.19/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-02 14:49:50.000000 docinit-0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 14:49:50.000000 docinit-0.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-05-02 14:50:06.987977 docinit-0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-02 14:49:50.000000 docinit-0.19/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.983977 docinit-0.19/docinit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:50.000000 docinit-0.19/docinit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-05-02 14:49:50.000000 docinit-0.19/docinit/docinit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.983977 docinit-0.19/docinit/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.983977 docinit-0.19/docinit/skeleton/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_ext/includefirst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.983977 docinit-0.19/docinit/skeleton/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_static/back.js
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_static/docinit.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.987977 docinit-0.19/docinit/skeleton/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.987977 docinit-0.19/docinit/skeleton/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_templates/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.987977 docinit-0.19/docinit/skeleton/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/default.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-02 14:49:50.000000 docinit-0.19/docinit/skeleton/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.983977 docinit-0.19/docinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-05-02 14:50:06.000000 docinit-0.19/docinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-02 14:50:06.000000 docinit-0.19/docinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:50:06.000000 docinit-0.19/docinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-02 14:50:06.000000 docinit-0.19/docinit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 14:50:06.000000 docinit-0.19/docinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 14:50:06.000000 docinit-0.19/docinit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-02 14:49:50.000000 docinit-0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 14:50:06.987977 docinit-0.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:50:06.987977 docinit-0.19/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:50.000000 docinit-0.19/test/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-02 14:49:50.000000 docinit-0.19/test/test_docinit.py
```

### Comparing `docinit-0.18/.github/workflows/build.yml` & `docinit-0.19/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `docinit-0.18/.github/workflows/publish.yml` & `docinit-0.19/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `docinit-0.18/.gitignore` & `docinit-0.19/.gitignore`

 * *Files identical despite different names*

### Comparing `docinit-0.18/LICENSE` & `docinit-0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `docinit-0.18/PKG-INFO` & `docinit-0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docinit
-Version: 0.18
+Version: 0.19
 Summary: Bootstrap your Sphinx documentation
 Home-page: https://github.com/timeflux/docinit
 Author: Pierre Clisson
 Author-email: contact@timeflux.io
 License: MIT
 Project-URL: Source Code, https://github.com/mesca/docinit
 Project-URL: Bug Tracker, https://github.com/mesca/docinit/issues
```

### Comparing `docinit-0.18/README.rst` & `docinit-0.19/README.rst`

 * *Files identical despite different names*

### Comparing `docinit-0.18/docinit/docinit.py` & `docinit-0.19/docinit/docinit.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,22 +99,21 @@
         """
         value = value.strip(' \r')
         if section == 'options' and key.endswith('_requires') :
             return value
         if section == 'options.extras_require':
             return value
         if value.startswith('file:'):
-            # if isinstance(ConfigHandler.__dict__["_get_parser_compound"], classmethod):
-            #     # A quick hack to solve the following change:
-            #     # https://github.com/pypa/setuptools/commit/4e766834d72623f3b938f1d4148547ea73af1bf5
-            #     mock = type("", (object,), {"_referenced_files": set()})()
-            #     return ConfigHandler._parse_file(mock, value, root)
-            # else:
-            #     return ConfigHandler._parse_file(value, root)
-            return ConfigHandler._parse_file(value, root)
+            if isinstance(ConfigHandler.__dict__["_get_parser_compound"], classmethod):
+                # A quick hack to solve the following change:
+                # https://github.com/pypa/setuptools/commit/4e766834d72623f3b938f1d4148547ea73af1bf5
+                mock = type("", (object,), {"_referenced_files": set()})()
+                return ConfigHandler._parse_file(mock, value, root)
+            else:
+                return ConfigHandler._parse_file(value, root)
         if value.startswith('attr:'):
             return ConfigOptionsHandler._parse_attr(value)
         if value in ['find:', 'find_namespace:']:
             return _get_packages()
         if '=' in value:
             return cls._parse_dict(ConfigHandler._parse_dict(value))
         if ',' in value or '\n' in value:
```

### Comparing `docinit-0.18/docinit/skeleton/_ext/includefirst.py` & `docinit-0.19/docinit/skeleton/_ext/includefirst.py`

 * *Files identical despite different names*

### Comparing `docinit-0.18/docinit/skeleton/_templates/autoapi/python/module.rst` & `docinit-0.19/docinit/skeleton/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `docinit-0.18/docinit/skeleton/conf.py` & `docinit-0.19/docinit/skeleton/conf.py`

 * *Files identical despite different names*

### Comparing `docinit-0.18/docinit/skeleton/make.bat` & `docinit-0.19/docinit/skeleton/make.bat`

 * *Files identical despite different names*

### Comparing `docinit-0.18/docinit.egg-info/PKG-INFO` & `docinit-0.19/docinit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docinit
-Version: 0.18
+Version: 0.19
 Summary: Bootstrap your Sphinx documentation
 Home-page: https://github.com/timeflux/docinit
 Author: Pierre Clisson
 Author-email: contact@timeflux.io
 License: MIT
 Project-URL: Source Code, https://github.com/mesca/docinit
 Project-URL: Bug Tracker, https://github.com/mesca/docinit/issues
```

### Comparing `docinit-0.18/docinit.egg-info/SOURCES.txt` & `docinit-0.19/docinit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docinit-0.18/setup.cfg` & `docinit-0.19/setup.cfg`

 * *Files identical despite different names*

### Comparing `docinit-0.18/test/test_docinit.py` & `docinit-0.19/test/test_docinit.py`

 * *Files identical despite different names*

