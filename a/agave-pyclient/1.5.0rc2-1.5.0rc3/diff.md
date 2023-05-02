# Comparing `tmp/agave_pyclient-1.5.0rc2.tar.gz` & `tmp/agave_pyclient-1.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agave_pyclient-1.5.0rc2.tar", last modified: Tue May  2 15:09:30 2023, max compression
+gzip compressed data, was "agave_pyclient-1.5.0rc3.tar", last modified: Tue May  2 19:53:22 2023, max compression
```

## Comparing `agave_pyclient-1.5.0rc2.tar` & `agave_pyclient-1.5.0rc3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:09:30.379960 agave_pyclient-1.5.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-02 15:09:30.379960 agave_pyclient-1.5.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:09:30.379960 agave_pyclient-1.5.0rc2/agave_pyclient/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/agave_pyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/agave_pyclient/agave.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/agave_pyclient/commandbuffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:09:30.379960 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-02 15:09:30.000000 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-02 15:09:30.000000 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:09:30.000000 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:09:30.000000 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:09:30.000000 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-02 15:09:30.000000 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 15:09:30.000000 agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:09:30.379960 agave_pyclient-1.5.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/docs/agave_renderer.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5384 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 15:09:30.383960 agave_pyclient-1.5.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-02 15:09:20.000000 agave_pyclient-1.5.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/agave_pyclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/agave_pyclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/agave_pyclient/agave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/agave_pyclient/commandbuffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 19:53:22.000000 agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:22.735859 agave_pyclient-1.5.0rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/agave_renderer.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5384 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 19:53:22.739859 agave_pyclient-1.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-02 19:53:09.000000 agave_pyclient-1.5.0rc3/setup.py
```

### Comparing `agave_pyclient-1.5.0rc2/CONTRIBUTING.md` & `agave_pyclient-1.5.0rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/LICENSE` & `agave_pyclient-1.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/PKG-INFO` & `agave_pyclient-1.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agave_pyclient
-Version: 1.5.0rc2
+Version: 1.5.0rc3
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
 Platform: UNKNOWN
```

### Comparing `agave_pyclient-1.5.0rc2/README.md` & `agave_pyclient-1.5.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/agave_pyclient/agave.py` & `agave_pyclient-1.5.0rc3/agave_pyclient/agave.py`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/agave_pyclient/commandbuffer.py` & `agave_pyclient-1.5.0rc3/agave_pyclient/commandbuffer.py`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/PKG-INFO` & `agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agave-pyclient
-Version: 1.5.0rc2
+Version: 1.5.0rc3
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
 Platform: UNKNOWN
```

### Comparing `agave_pyclient-1.5.0rc2/agave_pyclient.egg-info/requires.txt` & `agave_pyclient-1.5.0rc3/agave_pyclient.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/docs/Makefile` & `agave_pyclient-1.5.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/docs/conf.py` & `agave_pyclient-1.5.0rc3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 author = u"Daniel Toloudis"
 
 # The version info for the project you"re documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The full version, including alpha/beta/rc tags
-release = "1.5.0-rc.2"
+release = "1.5.0-rc.3"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `agave_pyclient-1.5.0rc2/docs/index.rst` & `agave_pyclient-1.5.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/docs/make.bat` & `agave_pyclient-1.5.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.5.0rc2/setup.py` & `agave_pyclient-1.5.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,10 +79,10 @@
     setup_requires=setup_requirements,
     test_suite="agave_pyclient/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/allen-cell-animated/agave",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="1.5.0-rc.2",
+    version="1.5.0-rc.3",
     zip_safe=False,
 )
```

