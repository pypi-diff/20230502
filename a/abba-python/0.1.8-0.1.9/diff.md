# Comparing `tmp/abba_python-0.1.8.tar.gz` & `tmp/abba_python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-iymk9wfo\abba_python-0.1.8.tar", last modified: Tue May  2 13:01:54 2023, max compression
+gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-o61xhnfs\abba_python-0.1.9.tar", last modified: Tue May  2 13:11:01 2023, max compression
```

## Comparing `abba_python-0.1.8.tar` & `abba_python-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/
--rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1876 2023-05-02 13:01:54.000000 abba_python-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/docs/
--rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/Makefile
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/authors.rst
--rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.8/docs/conf.py
--rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/history.rst
--rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/index.rst
--rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.8/docs/usage.rst
--rw-rw-rw-   0        0        0      640 2023-05-02 13:01:54.000000 abba_python-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1406 2023-05-02 13:01:34.000000 abba_python-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/
--rw-rw-rw-   0        0        0      331 2023-05-02 13:01:34.000000 abba_python-0.1.8/src/abba_python/__init__.py
--rw-rw-rw-   0        0        0    41227 2023-05-02 13:01:01.000000 abba_python-0.1.8/src/abba_python/abba.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/abba_private/
--rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.1.8/src/abba_python/abba_private/AbbaAtlas.py
--rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.8/src/abba_python/abba_private/AbbaMap.py
--rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.8/src/abba_python/abba_private/AbbaOntology.py
--rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.1.8/src/abba_python/abba_private/DeepSliceProcessor.py
--rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.1.8/src/abba_python/abba_private/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/itk/
--rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.8/src/abba_python/itk/__init__.py
--rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.8/src/abba_python/itk/abba_itk.py
--rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.1.8/src/abba_python/run-abba-local-fiji.py
--rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.1.8/src/abba_python/run-abba.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/
--rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/__init__.py
--rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/command.py
--rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/jupyter_ui.py
--rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.8/src/abba_python/scijava_python_command/magic.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.8/src/abba_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 13:01:54.000000 abba_python-0.1.8/src/abba_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 13:01:54.000000 abba_python-0.1.8/tests/
--rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.8/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.8/tests/test_abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/
+-rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.9/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1876 2023-05-02 13:11:01.000000 abba_python-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/docs/
+-rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/authors.rst
+-rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.9/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/usage.rst
+-rw-rw-rw-   0        0        0      640 2023-05-02 13:11:01.000000 abba_python-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2023-05-02 13:08:31.000000 abba_python-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/
+-rw-rw-rw-   0        0        0      331 2023-05-02 13:08:31.000000 abba_python-0.1.9/src/abba_python/__init__.py
+-rw-rw-rw-   0        0        0    41581 2023-05-02 13:07:37.000000 abba_python-0.1.9/src/abba_python/abba.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/abba_private/
+-rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.1.9/src/abba_python/abba_private/AbbaAtlas.py
+-rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.9/src/abba_python/abba_private/AbbaMap.py
+-rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.9/src/abba_python/abba_private/AbbaOntology.py
+-rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.1.9/src/abba_python/abba_private/DeepSliceProcessor.py
+-rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.1.9/src/abba_python/abba_private/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/itk/
+-rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.9/src/abba_python/itk/__init__.py
+-rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.9/src/abba_python/itk/abba_itk.py
+-rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.1.9/src/abba_python/run-abba-local-fiji.py
+-rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.1.9/src/abba_python/run-abba.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/
+-rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/__init__.py
+-rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/command.py
+-rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/jupyter_ui.py
+-rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/magic.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/
+-rw-rw-rw-   0        0        0     1876 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.9/src/abba_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/tests/
+-rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.9/tests/test_abba_python.py
```

### Comparing `abba_python-0.1.8/CONTRIBUTING.rst` & `abba_python-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/LICENSE` & `abba_python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/PKG-INFO` & `abba_python-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba_python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.8/README.rst` & `abba_python-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/docs/Makefile` & `abba_python-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/docs/conf.py` & `abba_python-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/docs/installation.rst` & `abba_python-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/docs/make.bat` & `abba_python-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/setup.cfg` & `abba_python-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.8
+current_version = 0.1.9
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `abba_python-0.1.8/setup.py` & `abba_python-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='abba_python',
     name='abba_python',
     packages=find_packages(include=['abba_python', 'abba_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nicoKiaru/abba_python',
-    version='0.1.8',
+    version='0.1.9',
     zip_safe=False,
 )
```

### Comparing `abba_python-0.1.8/src/abba_python/abba.py` & `abba_python-0.1.9/src/abba_python/abba.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,19 @@
                             from jpype import JImplements, JOverride
                             print('2')
                             Runnable = jimport('java.lang.Runnable')
                             print('3')
 
                             class DSPlaceHolder(object):
                                 def __init__(self, ij):
+                                    print('ze temp')
                                     self.temp_folder = prepare_deepslice_temp_folder(self)
+                                    print('alors')
                                     self.ij = ij
+                                    print('heu')
 
                             print('4')
 
                             @JImplements(Runnable)
                             class ExecuteDeepSlicePython(object):
 
                                 def __init__(self, dsp):
@@ -179,14 +182,15 @@
                                                               "image_name_prefix", JString('Section'),
                                                               "mp", view.msp,
                                                               "deepSliceProcessor", self.dsp._run_deep_slice,
                                                               "dataset_folder", JString(self.dsp.temp_folder)
                                                               )
 
                             print('5')
+                            print('ij= '+str(ij))
                             dsplaceholder = DSPlaceHolder(ij)
                             print('5A')
                             edsp = ExecuteDeepSlicePython(dsplaceholder)
                             print('5B')
                             bdv_view = view.getBdvh()
                             print('5C')
 
@@ -202,35 +206,42 @@
             return IPyWidgetCommandPostProcessor()
 
     PyPostprocessor.register(IPyWidgetCommandPreprocessorSupplier())
     print('ABBA Python hooks enabled')
 
 
 def prepare_deepslice_temp_folder(self):
+    print('pdtf0')
     if not hasattr(self, '_run_deep_slice'):
         from src.abba_python.abba_private.DeepSliceProcessor import DeepSliceProcessor
         self._run_deep_slice = DeepSliceProcessor()
 
+    print('pdtf1')
     # TODO : fix potential multiple running instance issues
     temp_folder = tempfile.gettempdir() + '/temp/deepslice/'
 
+    print('pdtf2')
     # make sure that the folder exists
     if not os.path.exists(temp_folder):
         os.makedirs(temp_folder)
 
+    print('pdtf3')
     # clean folder : remove all previous files
     for filename in os.listdir(temp_folder):
+        print('pdtf3a')
         file_path = os.path.join(temp_folder, filename)
         try:
             if os.path.isfile(file_path) or os.path.islink(file_path):
                 os.unlink(file_path)
             # elif os.path.isdir(file_path):
             #    shutil.rmtree(file_path)
         except Exception as e:
+            print('pdtf3error')
             print('Failed to delete %s. Reason: %s' % (file_path, e))
+    print('pdtf4')
     # print('Temp folder = '+str(temp_folder))
     return temp_folder
 
 
 class Abba:
     """Abba object which can be used to register sections to a BrainGlobe atlas object
     Parameters
```

### Comparing `abba_python-0.1.8/src/abba_python/abba_private/AbbaAtlas.py` & `abba_python-0.1.9/src/abba_python/abba_private/AbbaAtlas.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/abba_private/AbbaMap.py` & `abba_python-0.1.9/src/abba_python/abba_private/AbbaMap.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/abba_private/AbbaOntology.py` & `abba_python-0.1.9/src/abba_python/abba_private/AbbaOntology.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/abba_private/DeepSliceProcessor.py` & `abba_python-0.1.9/src/abba_python/abba_private/DeepSliceProcessor.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/itk/abba_itk.py` & `abba_python-0.1.9/src/abba_python/itk/abba_itk.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/run-abba-local-fiji.py` & `abba_python-0.1.9/src/abba_python/run-abba-local-fiji.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/run-abba.py` & `abba_python-0.1.9/src/abba_python/run-abba.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/scijava_python_command/command.py` & `abba_python-0.1.9/src/abba_python/scijava_python_command/command.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/scijava_python_command/jupyter_ui.py` & `abba_python-0.1.9/src/abba_python/scijava_python_command/jupyter_ui.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python/scijava_python_command/magic.py` & `abba_python-0.1.9/src/abba_python/scijava_python_command/magic.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.8/src/abba_python.egg-info/PKG-INFO` & `abba_python-0.1.9/src/abba_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.8/src/abba_python.egg-info/SOURCES.txt` & `abba_python-0.1.9/src/abba_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

