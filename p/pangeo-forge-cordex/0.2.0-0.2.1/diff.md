# Comparing `tmp/pangeo-forge-cordex-0.2.0.tar.gz` & `tmp/pangeo-forge-cordex-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.2.0.tar", last modified: Sun Apr 30 22:32:02 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.2.1.tar", last modified: Tue May  2 12:10:27 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.2.0.tar` & `pangeo-forge-cordex-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.390650 pangeo-forge-cordex-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.390650 pangeo-forge-cordex-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.390650 pangeo-forge-cordex-0.2.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-30 22:32:02.000000 pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:32:02.394650 pangeo-forge-cordex-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-30 22:31:49.000000 pangeo-forge-cordex-0.2.0/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.2.0/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.2.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.0/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.0/.gitignore` & `pangeo-forge-cordex-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.0/LICENSE` & `pangeo-forge-cordex-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.0/PKG-INFO` & `pangeo-forge-cordex-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.0
+Version: 0.2.1
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/esgf_access.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 import ssl
 
 import requests
-from pangeo_forge_recipes.patterns import pattern_from_file_sequence
-from pangeo_forge_recipes.recipes import XarrayZarrRecipe
-from pyesgf.logon import LogonManager
 
 from .utils import combine_response, parse_dataset_response, sort_files_by_dataset_id
 
 
 def logon():
+    from pyesgf.logon import LogonManager
+    
     lm = LogonManager(verify=True)
     if not lm.is_logged_on():
         myproxy_host = "esgf-data.dkrz.de"
         # if we find those in environment, use them.
         if "ESGF_USER" in os.environ and "ESGF_PASSWORD" in os.environ:
             lm.logon(
                 hostname=myproxy_host,
@@ -34,26 +33,14 @@
     # create SSL context
     sslcontext = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH)
     sslcontext.load_verify_locations(capath=lm.esgf_certs_dir)
     sslcontext.load_cert_chain(lm.esgf_credentials)
     return sslcontext
 
 
-def create_recipe(urls, recipe_kwargs=None, pattern_kwargs=None):
-    if recipe_kwargs is None:
-        recipe_kwargs = {}
-    if pattern_kwargs is None:
-        pattern_kwargs = {}
-    pattern = pattern_from_file_sequence(urls, "time", **pattern_kwargs)
-    if urls is not None:
-        return XarrayZarrRecipe(
-            pattern, xarray_concat_kwargs={"join": "exact"}, **recipe_kwargs
-        )
-
-
 def request(
     url="https://esgf-node.llnl.gov/esg-search/search",
     project="CORDEX",
     type="File",
     **search,
 ):
     version = search.get("version", None)
```

### Comparing `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/recipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,7 +67,22 @@
         iids = [iids]
     dset_responses = {}
     for iid in iids:
         facets = facets_from_iid(iid)
         dset_responses.update(esgf_search(**facets))
 
     return create_recipe_inputs(dset_responses, ssl)
+
+
+def create_recipe(urls, recipe_kwargs=None, pattern_kwargs=None):
+    from pangeo_forge_recipes.patterns import pattern_from_file_sequence
+    from pangeo_forge_recipes.recipes import XarrayZarrRecipe
+    
+    if recipe_kwargs is None:
+        recipe_kwargs = {}
+    if pattern_kwargs is None:
+        pattern_kwargs = {}
+    pattern = pattern_from_file_sequence(urls, "time", **pattern_kwargs)
+    if urls is not None:
+        return XarrayZarrRecipe(
+            pattern, xarray_concat_kwargs={"join": "exact"}, **recipe_kwargs
+        )
```

### Comparing `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.0
+Version: 0.2.1
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.0/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.0/setup.cfg` & `pangeo-forge-cordex-0.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 zip_safe = False
 python_requires = >=3.9
 packages = find:
 include_package_data = True
 install_requires = 
 	aiohttp
 	requests
+recipe = 
+	pangeo-forge-recipes = 0.9.0
+	esgf-pyclient
 
 [tool:pytest]
 python_files = test_*.py
 testpaths = tests
 filterwarnings = 
 	ignore:numpy.ufunc size changed, may indicate binary incompatibility.:RuntimeWarning
```

### Comparing `pangeo-forge-cordex-0.2.0/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.2.1/tests/test_recipe_creation.py`

 * *Files identical despite different names*

