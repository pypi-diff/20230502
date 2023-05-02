# Comparing `tmp/abba_python-0.1.7.tar.gz` & `tmp/abba_python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-3k30zqep\abba_python-0.1.7.tar", last modified: Tue May  2 12:51:58 2023, max compression
+gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-iymk9wfo\abba_python-0.1.8.tar", last modified: Tue May  2 13:01:54 2023, max compression
```

## Comparing `abba_python-0.1.7.tar` & `abba_python-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/
--rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.7/AUTHORS.rst
--rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.7/HISTORY.rst
--rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1876 2023-05-02 12:51:58.000000 abba_python-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/docs/
--rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/Makefile
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/authors.rst
--rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.7/docs/conf.py
--rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/history.rst
--rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/index.rst
--rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.7/docs/usage.rst
--rw-rw-rw-   0        0        0      640 2023-05-02 12:51:58.000000 abba_python-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1406 2023-05-02 12:51:35.000000 abba_python-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:57.000000 abba_python-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/src/abba_python/
--rw-rw-rw-   0        0        0      331 2023-05-02 12:51:35.000000 abba_python-0.1.7/src/abba_python/__init__.py
--rw-rw-rw-   0        0        0    40960 2023-05-02 12:50:50.000000 abba_python-0.1.7/src/abba_python/abba.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/src/abba_python/abba_private/
--rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.1.7/src/abba_python/abba_private/AbbaAtlas.py
--rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.7/src/abba_python/abba_private/AbbaMap.py
--rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.7/src/abba_python/abba_private/AbbaOntology.py
--rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.1.7/src/abba_python/abba_private/DeepSliceProcessor.py
--rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.1.7/src/abba_python/abba_private/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/src/abba_python/itk/
--rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.7/src/abba_python/itk/__init__.py
--rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.7/src/abba_python/itk/abba_itk.py
--rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.1.7/src/abba_python/run-abba-local-fiji.py
--rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.1.7/src/abba_python/run-abba.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/src/abba_python/scijava_python_command/
--rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.1.7/src/abba_python/scijava_python_command/__init__.py
--rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.7/src/abba_python/scijava_python_command/command.py
--rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.7/src/abba_python/scijava_python_command/jupyter_ui.py
--rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.7/src/abba_python/scijava_python_command/magic.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/src/abba_python.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-05-02 12:51:57.000000 abba_python-0.1.7/src/abba_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2023-05-02 12:51:57.000000 abba_python-0.1.7/src/abba_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:51:57.000000 abba_python-0.1.7/src/abba_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.7/src/abba_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2023-05-02 12:51:57.000000 abba_python-0.1.7/src/abba_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 12:51:57.000000 abba_python-0.1.7/src/abba_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 12:51:58.000000 abba_python-0.1.7/tests/
--rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.7/tests/test_abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/
+-rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.8/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.8/HISTORY.rst
+-rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1876 2023-05-02 13:01:54.000000 abba_python-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/docs/
+-rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/authors.rst
+-rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.8/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/usage.rst
+-rw-rw-rw-   0        0        0      640 2023-05-02 13:01:54.000000 abba_python-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2023-05-02 13:01:34.000000 abba_python-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/
+-rw-rw-rw-   0        0        0      331 2023-05-02 13:01:34.000000 abba_python-0.1.8/src/abba_python/__init__.py
+-rw-rw-rw-   0        0        0    41227 2023-05-02 13:01:01.000000 abba_python-0.1.8/src/abba_python/abba.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/abba_private/
+-rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.1.8/src/abba_python/abba_private/AbbaAtlas.py
+-rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.8/src/abba_python/abba_private/AbbaMap.py
+-rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.8/src/abba_python/abba_private/AbbaOntology.py
+-rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.1.8/src/abba_python/abba_private/DeepSliceProcessor.py
+-rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.1.8/src/abba_python/abba_private/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/itk/
+-rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.8/src/abba_python/itk/__init__.py
+-rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.8/src/abba_python/itk/abba_itk.py
+-rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.1.8/src/abba_python/run-abba-local-fiji.py
+-rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.1.8/src/abba_python/run-abba.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/
+-rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/__init__.py
+-rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/command.py
+-rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/jupyter_ui.py
+-rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/magic.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/
+-rw-rw-rw-   0        0        0     1876 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.8/src/abba_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/tests/
+-rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.8/tests/test_abba_python.py
```

### Comparing `abba_python-0.1.7/CONTRIBUTING.rst` & `abba_python-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/LICENSE` & `abba_python-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/PKG-INFO` & `abba_python-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba_python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.7/README.rst` & `abba_python-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/docs/Makefile` & `abba_python-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/docs/conf.py` & `abba_python-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/docs/installation.rst` & `abba_python-0.1.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/docs/make.bat` & `abba_python-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/setup.cfg` & `abba_python-0.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.7
+current_version = 0.1.8
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `abba_python-0.1.7/setup.py` & `abba_python-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='abba_python',
     name='abba_python',
     packages=find_packages(include=['abba_python', 'abba_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nicoKiaru/abba_python',
-    version='0.1.7',
+    version='0.1.8',
     zip_safe=False,
 )
```

### Comparing `abba_python-0.1.7/src/abba_python/abba.py` & `abba_python-0.1.8/src/abba_python/abba.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,17 +179,24 @@
                                                               "image_name_prefix", JString('Section'),
                                                               "mp", view.msp,
                                                               "deepSliceProcessor", self.dsp._run_deep_slice,
                                                               "dataset_folder", JString(self.dsp.temp_folder)
                                                               )
 
                             print('5')
-                            BdvScijavaHelper.addActionToBdvHandleMenu(view.getBdvh(),
+                            dsplaceholder = DSPlaceHolder(ij)
+                            print('5A')
+                            edsp = ExecuteDeepSlicePython(dsplaceholder)
+                            print('5B')
+                            bdv_view = view.getBdvh()
+                            print('5C')
+
+                            BdvScijavaHelper.addActionToBdvHandleMenu(bdv_view,
                                                                       "Align>ABBA - DeepSlice Registration (Python)", 0,
-                                                                      ExecuteDeepSlicePython(DSPlaceHolder(ij)))
+                                                                      edsp)
                             print('6')
 
     @JImplements(Supplier)
     class IPyWidgetCommandPreprocessorSupplier(object):
         @JOverride
         def get(self):
             return IPyWidgetCommandPostProcessor()
```

### Comparing `abba_python-0.1.7/src/abba_python/abba_private/AbbaAtlas.py` & `abba_python-0.1.8/src/abba_python/abba_private/AbbaAtlas.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/abba_private/AbbaMap.py` & `abba_python-0.1.8/src/abba_python/abba_private/AbbaMap.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/abba_private/AbbaOntology.py` & `abba_python-0.1.8/src/abba_python/abba_private/AbbaOntology.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/abba_private/DeepSliceProcessor.py` & `abba_python-0.1.8/src/abba_python/abba_private/DeepSliceProcessor.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/itk/abba_itk.py` & `abba_python-0.1.8/src/abba_python/itk/abba_itk.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/run-abba-local-fiji.py` & `abba_python-0.1.8/src/abba_python/run-abba-local-fiji.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/run-abba.py` & `abba_python-0.1.8/src/abba_python/run-abba.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/scijava_python_command/command.py` & `abba_python-0.1.8/src/abba_python/scijava_python_command/command.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/scijava_python_command/jupyter_ui.py` & `abba_python-0.1.8/src/abba_python/scijava_python_command/jupyter_ui.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python/scijava_python_command/magic.py` & `abba_python-0.1.8/src/abba_python/scijava_python_command/magic.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.7/src/abba_python.egg-info/PKG-INFO` & `abba_python-0.1.8/src/abba_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.7/src/abba_python.egg-info/SOURCES.txt` & `abba_python-0.1.8/src/abba_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

