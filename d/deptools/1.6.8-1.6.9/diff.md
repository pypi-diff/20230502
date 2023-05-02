# Comparing `tmp/deptools-1.6.8.tar.gz` & `tmp/deptools-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deptools-1.6.8.tar", last modified: Wed Sep  7 14:36:42 2022, max compression
+gzip compressed data, was "deptools-1.6.9.tar", last modified: Wed Sep  7 16:47:02 2022, max compression
```

## Comparing `deptools-1.6.8.tar` & `deptools-1.6.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 14:36:42.021387 deptools-1.6.8/
--rw-r--r--   0 root         (0) root         (0)     4255 2022-09-07 14:17:33.000000 deptools-1.6.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-03-16 19:51:28.000000 deptools-1.6.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      542 2022-09-07 14:36:42.021387 deptools-1.6.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      166 2022-03-16 19:51:28.000000 deptools-1.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 14:36:42.017387 deptools-1.6.8/deptools/
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-03-16 19:51:28.000000 deptools-1.6.8/deptools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20855 2022-04-28 16:14:00.000000 deptools-1.6.8/deptools/changelogparser.py
--rw-r--r--   0 root         (0) root         (0)     2951 2022-03-21 12:12:45.000000 deptools-1.6.8/deptools/createversionfile.py
--rw-rw-rw-   0 root         (0) root         (0)    13241 2022-03-16 19:51:28.000000 deptools-1.6.8/deptools/deploy.py
--rw-r--r--   0 root         (0) root         (0)     7906 2022-09-07 14:17:33.000000 deptools-1.6.8/deptools/register.py
--rw-rw-rw-   0 root         (0) root         (0)    13422 2022-03-16 19:51:28.000000 deptools-1.6.8/deptools/runclangformat.py
--rw-r--r--   0 root         (0) root         (0)     2287 2022-05-26 19:51:56.000000 deptools-1.6.8/deptools/spec.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2022-03-16 19:51:28.000000 deptools-1.6.8/deptools/versiontype.py
--rw-r--r--   0 root         (0) root         (0)     7686 2022-08-31 15:38:42.000000 deptools-1.6.8/deptools/windrvsign.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 14:36:42.021387 deptools-1.6.8/deptools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      542 2022-09-07 14:36:41.000000 deptools-1.6.8/deptools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      577 2022-09-07 14:36:41.000000 deptools-1.6.8/deptools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-07 14:36:41.000000 deptools-1.6.8/deptools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2022-09-07 14:36:41.000000 deptools-1.6.8/deptools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      109 2022-09-07 14:36:41.000000 deptools-1.6.8/deptools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-09-07 14:36:41.000000 deptools-1.6.8/deptools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-07 14:36:42.021387 deptools-1.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1414 2022-08-31 15:38:42.000000 deptools-1.6.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 14:36:42.021387 deptools-1.6.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-16 19:51:28.000000 deptools-1.6.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14090 2022-04-28 16:14:00.000000 deptools-1.6.8/tests/test_changelogparser.py
--rw-rw-rw-   0 root         (0) root         (0)      511 2022-03-16 19:51:28.000000 deptools-1.6.8/tests/test_deploy.py
--rw-r--r--   0 root         (0) root         (0)     1159 2022-09-07 14:17:33.000000 deptools-1.6.8/tests/test_register.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2022-03-16 19:51:28.000000 deptools-1.6.8/tests/test_versiontype.py
--rw-rw-rw-   0 root         (0) root         (0)        5 2022-09-07 14:34:13.000000 deptools-1.6.8/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 16:47:02.379573 deptools-1.6.9/
+-rw-rw-rw-   0 root         (0) root         (0)     4372 2022-09-07 16:38:58.000000 deptools-1.6.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-04-26 14:43:10.000000 deptools-1.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      542 2022-09-07 16:47:02.379573 deptools-1.6.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      166 2022-04-26 14:43:10.000000 deptools-1.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 16:47:02.378574 deptools-1.6.9/deptools/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-04-26 14:43:10.000000 deptools-1.6.9/deptools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20855 2022-04-28 17:22:13.000000 deptools-1.6.9/deptools/changelogparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2022-04-26 14:43:10.000000 deptools-1.6.9/deptools/createversionfile.py
+-rw-rw-rw-   0 root         (0) root         (0)    13241 2022-04-26 14:43:10.000000 deptools-1.6.9/deptools/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     7974 2022-09-07 16:38:58.000000 deptools-1.6.9/deptools/register.py
+-rw-rw-rw-   0 root         (0) root         (0)    13422 2022-04-26 14:43:10.000000 deptools-1.6.9/deptools/runclangformat.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2022-06-22 15:22:02.000000 deptools-1.6.9/deptools/spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2022-04-26 14:43:10.000000 deptools-1.6.9/deptools/versiontype.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2022-07-18 17:23:34.000000 deptools-1.6.9/deptools/windrvsign.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 16:47:02.378574 deptools-1.6.9/deptools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      542 2022-09-07 16:47:02.000000 deptools-1.6.9/deptools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      577 2022-09-07 16:47:02.000000 deptools-1.6.9/deptools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-07 16:47:02.000000 deptools-1.6.9/deptools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2022-09-07 16:47:02.000000 deptools-1.6.9/deptools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-07 16:47:02.000000 deptools-1.6.9/deptools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-09-07 16:47:02.000000 deptools-1.6.9/deptools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-07 16:47:02.379573 deptools-1.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1414 2022-06-22 15:22:02.000000 deptools-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 16:47:02.379573 deptools-1.6.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-26 14:43:10.000000 deptools-1.6.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14090 2022-04-28 17:22:13.000000 deptools-1.6.9/tests/test_changelogparser.py
+-rw-rw-rw-   0 root         (0) root         (0)      511 2022-04-26 14:43:10.000000 deptools-1.6.9/tests/test_deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2022-09-07 14:04:08.000000 deptools-1.6.9/tests/test_register.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2022-04-26 14:43:10.000000 deptools-1.6.9/tests/test_versiontype.py
+-rw-rw-rw-   0 root         (0) root         (0)        5 2022-09-07 16:45:40.000000 deptools-1.6.9/version.txt
```

### Comparing `deptools-1.6.8/CHANGELOG.md` & `deptools-1.6.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # AlazarTech Deployment Tools Change Log
 
 This file contains all important changes to the AlazarTech deployment tools
 
+## [1.6.9] - 2022-09-07
+### Fixed 
+- Fix issue introduced in v1.6.8 where name and arch were not passed to payload.
+
 ## [1.6.8] - 2022-09-06
 ### Fixed 
 - Add name and arch fields for website registration tool.
 
 ### Added
 - Add product ID for ATS9376, ATS9380, ATS9428, ATS9437, ATS9442, ATS9453 and
   ATS9473.
```

### Comparing `deptools-1.6.8/PKG-INFO` & `deptools-1.6.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deptools
-Version: 1.6.8
+Version: 1.6.9
 Summary: Application Deployment Tools
 Home-page: https://alazartech.com
 Author: Alazar Technologies
 Author-email: support@alazartech.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deptools-1.6.8/deptools/changelogparser.py` & `deptools-1.6.9/deptools/changelogparser.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/deptools/createversionfile.py` & `deptools-1.6.9/deptools/createversionfile.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/deptools/deploy.py` & `deptools-1.6.9/deptools/deploy.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/deptools/register.py` & `deptools-1.6.9/deptools/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,16 @@
         payload.append({
             "os": package.os,
             "product_id": package.product_id,
             "url": base_url + package.installer,
             "release_notes_url": base_url + package.readme,
             "version": version,
             "password": password,
+            "name": package.name,
+            "arch": package.arch,
         })
     return json.dumps(payload)
 
 
 def register(endpoint, development, passfile, specsfile, baseurl, version, dry_run):
     specs = get_specs_from_file(specsfile)
     files = [thing for spec in specs for thing in get_things(spec)]
```

### Comparing `deptools-1.6.8/deptools/runclangformat.py` & `deptools-1.6.9/deptools/runclangformat.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/deptools/spec.py` & `deptools-1.6.9/deptools/spec.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/deptools/versiontype.py` & `deptools-1.6.9/deptools/versiontype.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/deptools/windrvsign.py` & `deptools-1.6.9/deptools/windrvsign.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/deptools.egg-info/PKG-INFO` & `deptools-1.6.9/deptools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deptools
-Version: 1.6.8
+Version: 1.6.9
 Summary: Application Deployment Tools
 Home-page: https://alazartech.com
 Author: Alazar Technologies
 Author-email: support@alazartech.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deptools-1.6.8/deptools.egg-info/SOURCES.txt` & `deptools-1.6.9/deptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/setup.py` & `deptools-1.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/tests/test_changelogparser.py` & `deptools-1.6.9/tests/test_changelogparser.py`

 * *Files identical despite different names*

### Comparing `deptools-1.6.8/tests/test_register.py` & `deptools-1.6.9/tests/test_register.py`

 * *Files identical despite different names*

