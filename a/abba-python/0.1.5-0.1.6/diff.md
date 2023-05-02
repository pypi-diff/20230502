# Comparing `tmp/abba_python-0.1.5.tar.gz` & `tmp/abba_python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-90az36ow\abba_python-0.1.5.tar", last modified: Mon May  1 15:51:31 2023, max compression
+gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-kfra4w77\abba_python-0.1.6.tar", last modified: Tue May  2 12:28:40 2023, max compression
```

## Comparing `abba_python-0.1.5.tar` & `abba_python-0.1.6.tar`

### file list

```diff
@@ -1,61 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/
--rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.5/HISTORY.rst
--rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1876 2023-05-01 15:51:31.000000 abba_python-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/docs/
--rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/Makefile
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/authors.rst
--rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.5/docs/conf.py
--rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/history.rst
--rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/index.rst
--rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.5/docs/usage.rst
--rw-rw-rw-   0        0        0      621 2023-05-01 15:51:31.000000 abba_python-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1386 2023-05-01 15:51:02.000000 abba_python-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python/
--rw-rw-rw-   0        0        0      175 2023-05-01 15:51:03.000000 abba_python-0.1.5/src/abba_python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python/abba_private/
--rw-rw-rw-   0        0        0     1810 2023-03-22 16:22:22.000000 abba_python-0.1.5/src/abba_python/abba_private/AbbaAtlas.py
--rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.5/src/abba_python/abba_private/AbbaMap.py
--rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.5/src/abba_python/abba_private/AbbaOntology.py
--rw-rw-rw-   0        0        0     2115 2023-03-22 16:24:20.000000 abba_python-0.1.5/src/abba_python/abba_private/DeepSliceProcessor.py
--rw-rw-rw-   0        0        0      230 2023-02-13 21:48:20.000000 abba_python-0.1.5/src/abba_python/abba_private/__init__.py
--rw-rw-rw-   0        0        0    40376 2023-05-01 14:50:10.000000 abba_python-0.1.5/src/abba_python/abba_python.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python/deepslice/
--rw-rw-rw-   0        0        0    20688 2023-03-22 15:57:33.000000 abba_python-0.1.5/src/abba_python/deepslice/DeepSlice.py
--rw-rw-rw-   0        0        0       48 2023-03-22 15:57:33.000000 abba_python-0.1.5/src/abba_python/deepslice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python/deepslice/utilities/
--rw-rw-rw-   0        0        0     5025 2022-09-25 13:45:55.000000 abba_python-0.1.5/src/abba_python/deepslice/utilities/QuickNII_functions.py
--rw-rw-rw-   0        0        0        0 2023-01-07 21:45:39.000000 abba_python-0.1.5/src/abba_python/deepslice/utilities/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-03-22 15:57:33.000000 abba_python-0.1.5/src/abba_python/deepslice/utilities/neuron_tools.py
--rw-rw-rw-   0        0        0    12364 2022-09-25 13:45:55.000000 abba_python-0.1.5/src/abba_python/deepslice/utilities/plane_alignment.py
--rw-rw-rw-   0        0        0    13145 2022-09-25 13:45:55.000000 abba_python-0.1.5/src/abba_python/deepslice/utilities/plane_alignment_rat.py
--rw-rw-rw-   0        0        0        0 2022-09-25 13:45:55.000000 abba_python-0.1.5/src/abba_python/deepslice/utilities/render_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python/itk/
--rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.5/src/abba_python/itk/__init__.py
--rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.5/src/abba_python/itk/abba_itk.py
--rw-rw-rw-   0        0        0     2839 2023-05-01 14:31:10.000000 abba_python-0.1.5/src/abba_python/run-abba-local-fiji.py
--rw-rw-rw-   0        0        0      979 2023-05-01 15:49:49.000000 abba_python-0.1.5/src/abba_python/run-abba.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python/scijava_python_command/
--rw-rw-rw-   0        0        0      308 2022-10-31 22:05:25.000000 abba_python-0.1.5/src/abba_python/scijava_python_command/__init__.py
--rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.5/src/abba_python/scijava_python_command/command.py
--rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.5/src/abba_python/scijava_python_command/jupyter_ui.py
--rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.5/src/abba_python/scijava_python_command/magic.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1543 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.5/src/abba_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 15:51:31.000000 abba_python-0.1.5/src/abba_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 15:51:31.000000 abba_python-0.1.5/tests/
--rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.5/tests/test_abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/
+-rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.6/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.6/HISTORY.rst
+-rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1876 2023-05-02 12:28:40.000000 abba_python-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/docs/
+-rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/authors.rst
+-rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.6/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.6/docs/usage.rst
+-rw-rw-rw-   0        0        0      640 2023-05-02 12:28:40.000000 abba_python-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2023-05-02 12:28:04.000000 abba_python-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python/
+-rw-rw-rw-   0        0        0      331 2023-05-02 12:28:04.000000 abba_python-0.1.6/src/abba_python/__init__.py
+-rw-rw-rw-   0        0        0    40686 2023-05-01 20:10:06.000000 abba_python-0.1.6/src/abba_python/abba.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python/abba_private/
+-rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.1.6/src/abba_python/abba_private/AbbaAtlas.py
+-rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.6/src/abba_python/abba_private/AbbaMap.py
+-rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.6/src/abba_python/abba_private/AbbaOntology.py
+-rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.1.6/src/abba_python/abba_private/DeepSliceProcessor.py
+-rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.1.6/src/abba_python/abba_private/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python/itk/
+-rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.6/src/abba_python/itk/__init__.py
+-rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.6/src/abba_python/itk/abba_itk.py
+-rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.1.6/src/abba_python/run-abba-local-fiji.py
+-rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.1.6/src/abba_python/run-abba.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python/scijava_python_command/
+-rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.1.6/src/abba_python/scijava_python_command/__init__.py
+-rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.6/src/abba_python/scijava_python_command/command.py
+-rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.6/src/abba_python/scijava_python_command/jupyter_ui.py
+-rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.6/src/abba_python/scijava_python_command/magic.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python.egg-info/
+-rw-rw-rw-   0        0        0     1876 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.6/src/abba_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 12:28:40.000000 abba_python-0.1.6/src/abba_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 12:28:40.000000 abba_python-0.1.6/tests/
+-rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.6/tests/test_abba_python.py
```

### Comparing `abba_python-0.1.5/CONTRIBUTING.rst` & `abba_python-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/LICENSE` & `abba_python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/PKG-INFO` & `abba_python-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba_python
-Version: 0.1.5
+Version: 0.1.6
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `abba_python-0.1.5/README.rst` & `abba_python-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/docs/Makefile` & `abba_python-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/docs/conf.py` & `abba_python-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/docs/installation.rst` & `abba_python-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/docs/make.bat` & `abba_python-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/setup.cfg` & `abba_python-0.1.6/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.5
+current_version = 0.1.6
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -25,14 +25,15 @@
 [options.packages.find]
 where = src
 install_requires = 
 	numpy
 	pandas
 	pyimagej
 	bg-atlasapi
+	DeepSlice==1.1.2
 python_requires = >=3.7
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `abba_python-0.1.5/setup.py` & `abba_python-0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['numpy', 'pandas', 'pyimagej', 'bg-atlasapi']
+requirements = ['numpy', 'pandas', 'pyimagej', 'bg-atlasapi', 'DeepSlice==1.1.2']
 
 test_requirements = [ ]
 
 setup(
     author="Nicolas Chiaruttini",
     author_email='nicolas.chiaruttini@epfl.ch',
     python_requires='>=3.6',
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='abba_python',
     name='abba_python',
     packages=find_packages(include=['abba_python', 'abba_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nicoKiaru/abba_python',
-    version='0.1.5',
+    version='0.1.6',
     zip_safe=False,
 )
```

### Comparing `abba_python-0.1.5/src/abba_python/abba_private/AbbaAtlas.py` & `abba_python-0.1.6/src/abba_python/abba_private/AbbaAtlas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bg_atlasapi import BrainGlobeAtlas
 from scyjava import jimport
 from jpype import JImplements, JOverride
 from jpype.types import JString
-from .AbbaOntology import AbbaOntology
-from .AbbaMap import AbbaMap
+from abba_python.abba_private.AbbaOntology import AbbaOntology
+from abba_python.abba_private.AbbaMap import AbbaMap
 
 ArrayList = jimport('java.util.ArrayList')
 Atlas = jimport('ch.epfl.biop.atlas.struct.Atlas')
 
 
 @JImplements(Atlas)
 class AbbaAtlas(object):
```

### Comparing `abba_python-0.1.5/src/abba_python/abba_private/AbbaMap.py` & `abba_python-0.1.6/src/abba_python/abba_private/AbbaMap.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/src/abba_python/abba_private/AbbaOntology.py` & `abba_python-0.1.6/src/abba_python/abba_private/AbbaOntology.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/src/abba_python/abba_python.py` & `abba_python-0.1.6/src/abba_python/abba.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,23 @@
         available_atlases_nodict = get_downloaded_atlases()
         available_atlases = dict()
         for atlas in available_atlases_nodict:
             print(atlas)
             available_atlases[atlas] = get_local_atlas_version(atlas)
 
     AtlasChooserCommand = jimport('ch.epfl.biop.atlas.scijava.AtlasChooserCommand')
-    from abba_private.AbbaAtlas import AbbaAtlas  # delayed import because the jvm should be set first
+    try:
+        from abba_python.abba_private.AbbaAtlas import AbbaAtlas  # delayed import because the jvm should be set first
+    except:
+        try:
+            from .abba_private.AbbaAtlas import \
+                AbbaAtlas  # delayed import because the jvm should be set first
+        except:
+            print("Could not import AbbaAtlas because the dev do not understand python modules and submodules.")
+
     from jpype import JImplements, JOverride
     Supplier = jimport('java.util.function.Supplier')
 
     # initialized
 
     @JImplements(Supplier)
     class AtlasSupplier(object):
```

### Comparing `abba_python-0.1.5/src/abba_python/itk/abba_itk.py` & `abba_python-0.1.6/src/abba_python/itk/abba_itk.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/src/abba_python/run-abba-local-fiji.py` & `abba_python-0.1.6/src/abba_python/run-abba-local-fiji.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # core dependencies
 import time
 
-from abba_python.abba_python import enable_python_hooks, add_brainglobe_atlases
+from abba import enable_python_hooks, add_brainglobe_atlases
 # in order to wait for a jvm shutdown
 import jpype
 import imagej
 
 import os
 
 # THIS FILE SETS MANY PATHS EXPLICITLY WHEN ABBA IS INSTALLED FROM THE INSTALLER!
```

### Comparing `abba_python-0.1.5/src/abba_python/run-abba.py` & `abba_python-0.1.6/src/abba_python/run-abba.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # core dependencies
 import time
-from abba_python import start_imagej
+from abba import start_imagej
 
 # in order to wait for a jvm shutdown
 import jpype
 
 
 if __name__ == '__main__':
+    # from DeepSlice import DSModel
+    # model = DSModel("mouse")
 
+    # model.predict(image_directory="C:/Users/nicol/AppData/Local/Temp/temp/deepslice", ensemble=False)
+    # model.save_predictions("C:/Users/nicol/AppData/Local/Temp/temp/deepslice/results")
     # MAC ISSUE
     # https: // github.com / imagej / pyimagej / issues / 23
     # -- FOR DEBUGGING
     # import imagej.doctor
     # imagej.doctor.checkup()
     # imagej.doctor.debug_to_stderr()
     # -- Atlas
```

### Comparing `abba_python-0.1.5/src/abba_python/scijava_python_command/command.py` & `abba_python-0.1.6/src/abba_python/scijava_python_command/command.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/src/abba_python/scijava_python_command/jupyter_ui.py` & `abba_python-0.1.6/src/abba_python/scijava_python_command/jupyter_ui.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/src/abba_python/scijava_python_command/magic.py` & `abba_python-0.1.6/src/abba_python/scijava_python_command/magic.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.5/src/abba_python.egg-info/PKG-INFO` & `abba_python-0.1.6/src/abba_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abba-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: Aligning Big Brains and Atlases, controlled from Python.
 Home-page: https://github.com/nicoKiaru/abba_python
 Author: Nicolas Chiaruttini
 Author-email: nicolas.chiaruttini@epfl.ch
 License: GNU General Public License v3
 Keywords: abba_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

