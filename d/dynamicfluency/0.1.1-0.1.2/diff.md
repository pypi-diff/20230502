# Comparing `tmp/dynamicfluency-0.1.1.tar.gz` & `tmp/dynamicfluency-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicfluency-0.1.1.tar", last modified: Fri Apr 28 11:43:21 2023, max compression
+gzip compressed data, was "dynamicfluency-0.1.2.tar", last modified: Mon May  1 22:51:12 2023, max compression
```

## Comparing `dynamicfluency-0.1.1.tar` & `dynamicfluency-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/
--rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/LICENSE
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1747 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1092 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/README.md
--rw-r--r--   0 jjw       (1000) jjw       (1000)      986 2023-04-16 08:34:15.000000 dynamicfluency-0.1.1/pyproject.toml
--rw-r--r--   0 jjw       (1000) jjw       (1000)      104 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/requirements.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/setup.cfg
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.027801 dynamicfluency-0.1.1/src/
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.028801 dynamicfluency-0.1.1/src/dynamicfluency/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      325 2023-04-10 14:17:26.000000 dynamicfluency-0.1.1/src/dynamicfluency/__init__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1952 2023-04-10 15:07:55.000000 dynamicfluency-0.1.1/src/dynamicfluency/aeneas_conversion.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.029801 dynamicfluency-0.1.1/src/dynamicfluency/data/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      248 2023-04-16 12:15:52.000000 dynamicfluency-0.1.1/src/dynamicfluency/data/__init__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      122 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/src/dynamicfluency/data/valid_pos_tags.csv
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.029801 dynamicfluency-0.1.1/src/dynamicfluency/helpers/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      642 2023-04-16 10:28:22.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/__init__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1416 2023-04-16 12:15:52.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/conversions.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      331 2023-04-10 14:16:43.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/database_extensions.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      363 2023-04-10 14:16:45.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/filepath_extensions.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2071 2023-04-16 20:30:14.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/textgridtier_extensions.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1879 2023-04-16 20:50:04.000000 dynamicfluency-0.1.1/src/dynamicfluency/pos_tagging.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2004 2023-04-16 20:50:43.000000 dynamicfluency-0.1.1/src/dynamicfluency/repetitions.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.030801 dynamicfluency-0.1.1/src/dynamicfluency/scripts/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     3010 2023-04-28 11:08:32.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/add_frequency_dictionary.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1614 2023-04-28 10:57:56.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      670 2023-04-10 14:16:47.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/download_nltk_requirements.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2111 2023-04-28 11:01:57.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/get_database_columns.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     3377 2023-04-28 11:01:32.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2028 2023-04-28 11:02:38.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2401 2023-04-28 11:03:42.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1510 2023-04-28 11:08:07.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2054 2023-04-16 20:30:14.000000 dynamicfluency-0.1.1/src/dynamicfluency/syntactic_analysis.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     3071 2023-04-16 20:51:26.000000 dynamicfluency-0.1.1/src/dynamicfluency/word_frequencies.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.029801 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1747 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1419 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/SOURCES.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/dependency_links.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)      103 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/requires.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       15 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/top_level.txt
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/tests/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     4917 2023-04-16 20:33:22.000000 dynamicfluency-0.1.1/tests/test_aeneas.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      588 2023-04-16 12:15:52.000000 dynamicfluency-0.1.1/tests/test_data.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)    15320 2023-04-16 20:41:28.000000 dynamicfluency-0.1.1/tests/test_helpers.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)    10068 2023-04-16 21:10:06.000000 dynamicfluency-0.1.1/tests/test_sql.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     6323 2023-04-25 08:32:12.000000 dynamicfluency-0.1.1/tests/test_tier_generation.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-01 22:51:12.224223 dynamicfluency-0.1.2/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2023-03-30 11:30:10.000000 dynamicfluency-0.1.2/LICENSE
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1913 2023-05-01 22:51:12.224223 dynamicfluency-0.1.2/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1259 2023-05-01 14:57:24.000000 dynamicfluency-0.1.2/README.md
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1134 2023-05-01 22:44:26.000000 dynamicfluency-0.1.2/pyproject.toml
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       60 2023-05-01 14:28:42.000000 dynamicfluency-0.1.2/requirements.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-05-01 22:51:12.224223 dynamicfluency-0.1.2/setup.cfg
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-01 22:51:12.220223 dynamicfluency-0.1.2/src/
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-01 22:51:12.221223 dynamicfluency-0.1.2/src/dynamicfluency/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      325 2023-05-01 22:44:36.000000 dynamicfluency-0.1.2/src/dynamicfluency/__init__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1952 2023-04-10 15:07:55.000000 dynamicfluency-0.1.2/src/dynamicfluency/aeneas_conversion.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-01 22:51:12.222223 dynamicfluency-0.1.2/src/dynamicfluency/helpers/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      642 2023-04-16 10:28:22.000000 dynamicfluency-0.1.2/src/dynamicfluency/helpers/__init__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1416 2023-04-16 12:15:52.000000 dynamicfluency-0.1.2/src/dynamicfluency/helpers/conversions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      331 2023-04-10 14:16:43.000000 dynamicfluency-0.1.2/src/dynamicfluency/helpers/database_extensions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      363 2023-04-10 14:16:45.000000 dynamicfluency-0.1.2/src/dynamicfluency/helpers/filepath_extensions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2071 2023-04-16 20:30:14.000000 dynamicfluency-0.1.2/src/dynamicfluency/helpers/textgridtier_extensions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2009 2023-05-01 17:50:44.000000 dynamicfluency-0.1.2/src/dynamicfluency/model_data.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2247 2023-05-01 15:58:37.000000 dynamicfluency-0.1.2/src/dynamicfluency/pos_tagging.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2004 2023-04-16 20:50:43.000000 dynamicfluency-0.1.2/src/dynamicfluency/repetitions.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-01 22:51:12.223223 dynamicfluency-0.1.2/src/dynamicfluency/scripts/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3044 2023-04-28 14:03:25.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/add_frequency_dictionary.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1614 2023-04-28 10:57:56.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      670 2023-04-10 14:16:47.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/download_nltk_requirements.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2203 2023-05-01 21:09:43.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/get_database_columns.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3670 2023-05-01 21:24:01.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2680 2023-05-01 18:50:21.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2401 2023-04-28 11:03:42.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2079 2023-05-01 17:01:21.000000 dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2165 2023-05-01 18:03:20.000000 dynamicfluency-0.1.2/src/dynamicfluency/syntactic_analysis.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3092 2023-05-01 20:52:36.000000 dynamicfluency-0.1.2/src/dynamicfluency/word_frequencies.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-01 22:51:12.222223 dynamicfluency-0.1.2/src/dynamicfluency.egg-info/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1913 2023-05-01 22:51:12.000000 dynamicfluency-0.1.2/src/dynamicfluency.egg-info/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1395 2023-05-01 22:51:12.000000 dynamicfluency-0.1.2/src/dynamicfluency.egg-info/SOURCES.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-05-01 22:51:12.000000 dynamicfluency-0.1.2/src/dynamicfluency.egg-info/dependency_links.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       58 2023-05-01 22:51:12.000000 dynamicfluency-0.1.2/src/dynamicfluency.egg-info/requires.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       15 2023-05-01 22:51:12.000000 dynamicfluency-0.1.2/src/dynamicfluency.egg-info/top_level.txt
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-01 22:51:12.224223 dynamicfluency-0.1.2/tests/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     4917 2023-04-16 20:33:22.000000 dynamicfluency-0.1.2/tests/test_aeneas.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1050 2023-05-01 15:57:52.000000 dynamicfluency-0.1.2/tests/test_data.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    15320 2023-04-16 20:41:28.000000 dynamicfluency-0.1.2/tests/test_helpers.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      727 2023-05-01 17:56:01.000000 dynamicfluency-0.1.2/tests/test_scripts.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    10071 2023-05-01 20:52:36.000000 dynamicfluency-0.1.2/tests/test_sql.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     6349 2023-05-01 16:09:09.000000 dynamicfluency-0.1.2/tests/test_tier_generation.py
```

### Comparing `dynamicfluency-0.1.1/LICENSE` & `dynamicfluency-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/PKG-INFO` & `dynamicfluency-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicfluency
-Version: 0.1.1
+Version: 0.1.2
 Summary: The base python package for DynamicFluency: Monitor and understand the dynamicity of linguistic aspects in (L2) speech.
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/bare_python_publish
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/bare_python_publish/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -26,8 +26,10 @@
 
 ## Tests
 
 Running the development tests can be done with the following command:
 ```
 pytest --cov=dynamicfluency tests/
 ```
-Please note that this requires pytest and pytest-cov to be installed. Additionally, `dynamicfluency` has to be installed, either with `pip install -e .` or trough other means if you want to compare versions. The code itself, as it is in `src/`, isn't recognised.  
+Please note that this requires pytest and pytest-cov to be installed. Additionally, `dynamicfluency` has to be installed, either with `pip install -e .` or trough other means if you want to compare versions. The code itself, as it is in `src/`, isn't recognized.
+
+These tests will download a lot of language models on the first go, as it tests all supported languages. This will take a few minutes the first time the tests are run
```

### Comparing `dynamicfluency-0.1.1/README.md` & `dynamicfluency-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 
 ## Tests
 
 Running the development tests can be done with the following command:
 ```
 pytest --cov=dynamicfluency tests/
 ```
-Please note that this requires pytest and pytest-cov to be installed. Additionally, `dynamicfluency` has to be installed, either with `pip install -e .` or trough other means if you want to compare versions. The code itself, as it is in `src/`, isn't recognised.  
+Please note that this requires pytest and pytest-cov to be installed. Additionally, `dynamicfluency` has to be installed, either with `pip install -e .` or trough other means if you want to compare versions. The code itself, as it is in `src/`, isn't recognized.
+
+These tests will download a lot of language models on the first go, as it tests all supported languages. This will take a few minutes the first time the tests are run
```

### Comparing `dynamicfluency-0.1.1/pyproject.toml` & `dynamicfluency-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynamicfluency"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="JJWRoeloffs", email="jelleroeloffs@gmail.com" },
 ]
 description = "The base python package for DynamicFluency: Monitor and understand the dynamicity of linguistic aspects in (L2) speech."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -29,7 +29,13 @@
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 "Homepage" = "https://github.com/JJWRoeloffs/bare_python_publish"
 "Bug Tracker" = "https://github.com/JJWRoeloffs/bare_python_publish/issues"
+
+[tool.pytest.ini_options]
+# Spacy uses some deprecated parts of Tensorflow
+filterwarnings = [
+    'ignore:.*U.*is deprecated:DeprecationWarning'
+]
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/aeneas_conversion.py` & `dynamicfluency-0.1.2/src/dynamicfluency/aeneas_conversion.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/helpers/__init__.py` & `dynamicfluency-0.1.2/src/dynamicfluency/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/helpers/conversions.py` & `dynamicfluency-0.1.2/src/dynamicfluency/helpers/conversions.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/helpers/textgridtier_extensions.py` & `dynamicfluency-0.1.2/src/dynamicfluency/helpers/textgridtier_extensions.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/pos_tagging.py` & `dynamicfluency-0.1.2/src/dynamicfluency/pos_tagging.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 from __future__ import annotations
 
-from collections import namedtuple
-from typing import List, Union
+from typing import List, Tuple
 
 import nltk
 from praatio.data_classes.interval_tier import IntervalTier
+from praatio.utilities.utils import Interval
 
 from dynamicfluency.helpers import entrylist_labels_to_string, make_lowercase_entrylist
+from dynamicfluency.model_data import (
+    NLTK_TAGGERS,
+    SPACY_MODELS,
+    assert_valid_language,
+    load_nltk_model,
+    load_spacy_model,
+)
 
 
 def generate_tags_from_entrylist(
-    entryList: List[namedtuple], *, lang: str = "eng"
-) -> List[Union[str, str]]:
+    entryList: List[Interval], *, lang: str = "en"
+) -> List[Tuple[str, str]]:
+    assert_valid_language(lang)
     text = entrylist_labels_to_string(entryList)
-    tokens: List[str] = nltk.word_tokenize(text)
-    return nltk.pos_tag(tokens=tokens, lang=lang)
+    if lang in NLTK_TAGGERS.keys():
+        load_nltk_model(NLTK_TAGGERS[lang])
+        tokens: List[str] = nltk.word_tokenize(text)
+        return nltk.pos_tag(tokens=tokens, lang=NLTK_TAGGERS[lang])
+    else:
+        nlp = load_spacy_model(SPACY_MODELS[lang])
+        return [(token.text, token.pos_) for token in nlp(text)]
 
 
 # Jankyness needed because the NLTK tokenise split sometimes splits words into smaller sub-sections
 def allign_tags(
-    tags: List[Union[str, str]], entryList: List[namedtuple]
-) -> List[namedtuple]:
-    """Make an alligned entrylist out of NLTK generated pos_tags and the entryList those were generated from."""
+    tags: List[Tuple[str, str]], entryList: List[Interval]
+) -> List[Interval]:
+    """Make an alligned entrylist out of NLTK/SpaCy generated pos_tags and the entryList those were generated from."""
 
     new_entryList = []
     for entry in entryList:
         if not entry.label:
             new_entryList.append(entry._replace(label=""))
             continue
         word = ""
@@ -35,20 +48,20 @@
             label = " ".join([label, "_".join(tags[0])])
             tags.pop(0)
         new_entryList.append(entry._replace(label=label.strip()))
     return new_entryList
 
 
 def make_pos_tier(
-    words_tier: IntervalTier, *, name: str = "POStags", lang: str = "eng"
+    words_tier: IntervalTier, *, name: str = "POStags", lang: str = "en"
 ) -> IntervalTier:
     """Makes a POS tagged tier from a textgrid tier with alligned words"""
+    assert_valid_language(lang)
 
     nltk.download("punkt", quiet=True, halt_on_error=True)
-    nltk.download("averaged_perceptron_tagger", quiet=True, halt_on_error=True)
 
     lowercase_entryList = make_lowercase_entrylist(words_tier.entryList)
 
     tags = generate_tags_from_entrylist(lowercase_entryList, lang=lang)
     tag_entryList = allign_tags(tags, lowercase_entryList)
 
     return words_tier.new(name=name, entryList=tag_entryList)
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/repetitions.py` & `dynamicfluency-0.1.2/src/dynamicfluency/repetitions.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/add_frequency_dictionary.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/add_frequency_dictionary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import argparse
 import sys
+import csv
 import sqlite3
 from pathlib import Path
 
 import pandas
 
 
+# Allow for reading very big files
+MAXSIZE = sys.maxsize
+while True:
+    try:
+        csv.field_size_limit(MAXSIZE)
+        break
+    except Exception:
+        MAXSIZE //= 2
+
+
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description="Creates a SQLite3 database from a csv-like file"
     )
     requiredNamed = parser.add_argument_group("Required named arguments")
 
     requiredNamed.add_argument(
@@ -48,21 +59,21 @@
         choices=["fail", "replace"],
         nargs="?",
         default="fail",
         help='What to do if a table with the specified name already exists in the database. Either "fail" or "replace"',
     )
     args = parser.parse_args()
 
-    if args.table_name == "default":
+    if args.table_name.lower() == "default":
         parser.error(
             "Table name cannot be 'default'. This would cause naming conflicts"
         )
 
-    if not Path(args.database).exists():
-        parser.error(f"{args.database} does not exist")
+    if not Path(args.database_file).exists():
+        parser.error(f"{args.database_file} does not exist")
 
     if not Path(args.dictionary_file).exists():
         parser.error(f"{args.dictionary_file} does not exist")
 
     return args
 
 
@@ -83,24 +94,16 @@
         sys.exit()
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
     df: pandas.DataFrame = read_file(args.dictionary_file, sep=args.seperator)
 
-    try:
-        database: sqlite3.Connection = sqlite3.connect(args.database_file)
+    with sqlite3.connect(args.database_file) as database:
         try:
             df.to_sql(args.table_name, database, if_exists=args.if_exists)
         except ValueError as error:
             print("Cannot write to SQL Database\n", error)
 
-    except sqlite3.Error as error:
-        print("SQL Error occured - ", error)
-
-    finally:
-        if database:
-            database.close()
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/download_nltk_requirements.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/download_nltk_requirements.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/get_database_columns.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/get_database_columns.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,17 +58,19 @@
         return
 
     with sqlite3.connect(args.database) as connection:
         cursor = get_row_cursor(connection)
         names = get_column_names(cursor, table_name=args.table_name)
 
     if not names:
-        names = ["#FAIL - Incorrect table name?"]
-    if not "WordForm" in names:
-        names = ['#FAIL - No column "WordForm" found.']
+        names = ["DYNAMICFLUENCY-ERROR - Incorrect table name?"]
+    elif not "WordForm" in names:
+        names = ["DYNAMICFLUENCY-ERROR - No column 'WordForm' found."]
+
+    names = [name for name in names if name != "WordForm"]
 
     with filepath.open("w", encoding="utf-8") as f:
         csv.writer(f).writerow(names)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     requiredNamed.add_argument(
         "-t", "--table_name", help="Name of the table to be read from.", required=True
     )
     requiredNamed.add_argument(
         "-a",
         "--allignment",
-        help="The type of allignment textgrid, either 'maus' or 'aeneas'",
+        help="The type of allignment textgrid, 'maus' or 'aeneas' or 'whisper'",
         required=True,
     )
 
     parser.add_argument(
         "-b",
         "--database",
         nargs="?",
@@ -45,24 +45,32 @@
     parser.add_argument(
         "-i",
         "--to_ignore",
         nargs="?",
         help="The words to ignore and not assign any value, seperated by commas.",
     )
     parser.add_argument(
-        "-r",
-        "--rows",
+        "-c",
+        "--columns",
         nargs="?",
         default="",
-        help="The Rows to read from the database table, seperated by commas",
+        help="The Columns to read from the database table, seperated by commas",
     )
 
     args: argparse.Namespace = parser.parse_args()
+
     args.to_ignore = args.to_ignore.split(",") if args.to_ignore is not None else None
-    args.rows = args.rows.split(",") if args.rows else None
+
+    if args.columns == "DYNAMICFLUENCY-DEFAULT":
+        args.columns = None
+
+    args.columns = args.columns.split(",") if args.columns else None
+
+    if args.columns is not None and not "WordForm" in args.columns:
+        args.columns.append("WordForm")
 
     if not Path(args.database).exists():
         parser.error(f"{args.database} does not exist")
 
     if not Path(args.directory).exists():
         parser.error(f"{args.directory} does not exist")
 
@@ -72,14 +80,16 @@
 def main():
     args: argparse.Namespace = parse_arguments()
 
     if args.allignment == "maus":
         tokentier_name = "ORT-MAU"
     elif args.allignment == "aeneas":
         tokentier_name = "Words"
+    elif args.allignment == "whisper":
+        tokentier_name = "words_text"
     else:
         raise ValueError(f"Unknown allignment type found: {args.allignment}")
 
     allignment_files = get_local_glob(args.directory, glob="*.allignment.TextGrid")
 
     for file in allignment_files:
         allignment_grid = tg.openTextgrid(str(file), includeEmptyIntervals=True)
@@ -92,15 +102,15 @@
         with sqlite3.connect(args.database) as connection:
             cursor = get_row_cursor(connection)
             frequency_grid = create_frequency_grid(
                 word_form_tier=tier,
                 cursor=cursor,
                 table_name=args.table_name,
                 to_ignore=args.to_ignore,
-                rows=args.rows,
+                columns=args.columns,
             )
 
         frequency_grid.removeTier("WordForm")
 
         name = str(file).replace(".allignment.TextGrid", ".frequencies.TextGrid")
         frequency_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from pathlib import Path
 import argparse
 
 from praatio import textgrid as tg
 from praatio.data_classes.textgrid import Textgrid
 from praatio.data_classes.interval_tier import IntervalTier
+from dynamicfluency.model_data import VALID_LANGUAGES
 
 from dynamicfluency.pos_tagging import make_pos_tier
 from dynamicfluency.helpers import get_local_glob
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
@@ -22,46 +23,62 @@
         nargs="?",
         default="output",
         help="The directory the tokens and phases is expected in, and the output is saved to",
     )
     parser.add_argument(
         "-a",
         "--allignment",
-        help="The type of allignment textgrid, either 'maus' or 'aeneas'",
+        help="The type of allignment textgrid, 'maus' or 'aeneas' or 'whisper'",
+    )
+    parser.add_argument(
+        "-l",
+        "--language",
+        help="The language to get the tagging model of",
+        choices=[x for k, v in VALID_LANGUAGES.items() for x in (k, v)],
+        nargs="?",
+        default="en",
     )
 
     args = parser.parse_args()
 
     if not Path(args.directory).exists():
         parser.error(f"{args.directory} does not exist")
 
+    if args.language in VALID_LANGUAGES.values():
+        [args.language] = [k for k, v in VALID_LANGUAGES.items() if v == args.language]
+
+    if args.language not in VALID_LANGUAGES.keys():
+        parser.error(f"{args.language} is not a valid language")
+
     return args
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
 
     if args.allignment == "maus":
         tokentier_name = "ORT-MAU"
     elif args.allignment == "aeneas":
         tokentier_name = "Words"
+    elif args.allignment == "whisper":
+        tokentier_name = "words_text"
     else:
         raise ValueError(f"Unknown allignment type found: {args.allignment}")
 
     allignment_files = get_local_glob(args.directory, glob="*.allignment.TextGrid")
 
     for file in allignment_files:
         allignment_grid = tg.openTextgrid(str(file), includeEmptyIntervals=True)
 
         if not isinstance(
             tier := allignment_grid.tierDict[tokentier_name], IntervalTier
         ):
             raise ValueError("Cannot read Allignment: Not an interval tier")
 
-        tagged_tier = make_pos_tier(tier)
+        tagged_tier = make_pos_tier(tier, lang=args.language)
 
         tag_grid = Textgrid()
         tag_grid.addTier(tagged_tier)
 
         name = str(file).replace(".allignment.TextGrid", ".pos_tags.TextGrid")
         tag_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py` & `dynamicfluency-0.1.2/src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,63 @@
 from pathlib import Path
 
 from praatio import textgrid as tg
 from praatio.data_classes.interval_tier import IntervalTier
 
 from dynamicfluency.helpers import get_local_glob
 from dynamicfluency.syntactic_analysis import make_syntax_grid
+from dynamicfluency.model_data import VALID_LANGUAGES
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description="Creates textgrid with syntactic information already present in pos tags"
     )
     parser.add_argument(
         "-d",
         "--directory",
         nargs="?",
         default="output",
         help="The directory the tokens and phases is expected in, and the output is saved to",
     )
+    parser.add_argument(
+        "-l",
+        "--language",
+        help="The language to get the tagging model of",
+        choices=[x for k, v in VALID_LANGUAGES.items() for x in (k, v)],
+        nargs="?",
+        default="en",
+    )
 
     args = parser.parse_args()
 
     if not Path(args.directory).exists():
         parser.error(f"{args.directory} does not exist")
 
+    if args.language in VALID_LANGUAGES.values():
+        [args.language] = [k for k, v in VALID_LANGUAGES.items() if v == args.language]
+
+    if args.language not in VALID_LANGUAGES.keys():
+        parser.error(f"{args.language} is not a valid language")
+
     return args
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
 
     tagged_files = get_local_glob(args.directory, glob="*.pos_tags.TextGrid")
 
     for file in tagged_files:
         tagged_grid = tg.openTextgrid(str(file), includeEmptyIntervals=True)
 
         if not isinstance(tier := tagged_grid.tierDict["POStags"], IntervalTier):
             raise ValueError("Cannot read POStags: Not an interval tier")
 
-        syntax_grid = make_syntax_grid(pos_tier=tier)
+        syntax_grid = make_syntax_grid(pos_tier=tier, lang=args.language)
 
         name = str(file).replace(".pos_tags.TextGrid", ".syntax.TextGrid")
         syntax_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/syntactic_analysis.py` & `dynamicfluency-0.1.2/src/dynamicfluency/syntactic_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 from __future__ import annotations
 
-from typing import List
+from typing import Set
 
 from praatio.data_classes.textgrid import Textgrid
 from praatio.data_classes.interval_tier import IntervalTier
 from praatio.data_classes.point_tier import PointTier
 from praatio.utilities.constants import Point
 
 from dynamicfluency.helpers import split_pos_label, get_midpoint
-from dynamicfluency.data import get_valid_tags
+from dynamicfluency.model_data import get_valid_tags
 
-BASE_VERBS = ["VBZ", "VBP", "VBD", "VB"]
-CLAUSE_VERBS = ["VB", "VBD", "VBG", "VBN", "VBP", "VBZ"]
+# This can be seen as a temporairy solution
+BASE_VERBS = {"VBZ", "VBP", "VBD", "VB", "ROOT", "VC", "VE", "VP", "VERB"}
+CLAUSE_VERBS = {"VBG", "VBN", "AUX", "MD", "VV"}
 
 
-def label_contains_pos(lab: str, guard: List[str]) -> bool:
+def label_contains_pos(lab: str, guard: Set[str]) -> bool:
     return any(pos in guard for pos in split_pos_label(lab, get_pos=True).split())
 
 
-def validate_pos(pos_tier: IntervalTier) -> bool:
-    valid_tags = get_valid_tags()
+def validate_pos(pos_tier: IntervalTier, lang: str) -> bool:
+    valid_tags = get_valid_tags(lang)
     return all(
         label_contains_pos(interval.label, valid_tags)
         for interval in pos_tier.entryList
         if interval.label
     )
 
 
 def create_clause_point_tier(pos_tier: IntervalTier) -> PointTier:
     entryList = [
         Point(get_midpoint(interval), "")
         for interval in pos_tier.entryList
-        if label_contains_pos(interval.label, CLAUSE_VERBS)
+        if label_contains_pos(interval.label, CLAUSE_VERBS.union(BASE_VERBS))
     ]
     return PointTier(
         name="Syntactic Clauses",
         entryList=entryList,
         minT=pos_tier.minTimestamp,
         maxT=pos_tier.maxTimestamp,
     )
 
 
 def create_phrase_point_tier(pos_tier: IntervalTier) -> PointTier:
     entryList = [
         Point(get_midpoint(interval), "")
         for interval in pos_tier.entryList
-        if split_pos_label(interval.label, get_pos=True) in BASE_VERBS
+        if label_contains_pos(interval.label, BASE_VERBS)
     ]
     return PointTier(
         name="Syntactic Phrases",
         entryList=entryList,
         minT=pos_tier.minTimestamp,
         maxT=pos_tier.maxTimestamp,
     )
 
 
-def make_syntax_grid(pos_tier: IntervalTier) -> Textgrid:
-    if not validate_pos(pos_tier):
+def make_syntax_grid(pos_tier: IntervalTier, lang: str) -> Textgrid:
+    if not validate_pos(pos_tier, lang):
         raise ValueError("POS_tier contains unreadable pos labels")
 
     syntax_grid = Textgrid(pos_tier.minTimestamp, pos_tier.maxTimestamp)
     syntax_grid.addTier(create_clause_point_tier(pos_tier))
     syntax_grid.addTier(create_phrase_point_tier(pos_tier))
     return syntax_grid
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency/word_frequencies.py` & `dynamicfluency-0.1.2/src/dynamicfluency/word_frequencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 def make_empty_frequency_grid(
     *,
     cursor: sqlite3.Cursor,
     table_name: str,
     base_tier: IntervalTier,
-    rows: Optional[List[str]] = None,
+    columns: Optional[List[str]] = None,
 ) -> Textgrid:
     """Makes an "empty" frequency grid.
     This is a grid that has all the tiers initialised according to the column names of the databse,
     but does not have any values in those tiers, all of them being copies from the base.
     """
-    if rows is None:
-        rows = get_column_names(cursor, table_name=table_name)
+    if columns is None:
+        columns = get_column_names(cursor, table_name=table_name)
     frequency_grid = Textgrid()
-    for name in rows:
+    for name in columns:
         tier = base_tier.new(name=name)
         frequency_grid.addTier(tier)
     return frequency_grid
 
 
 def set_labels_from_db(
     *,
@@ -69,21 +69,21 @@
 
 def create_frequency_grid(
     word_form_tier: IntervalTier,
     *,
     cursor: sqlite3.Cursor,
     table_name: str,
     to_ignore: Optional[List[str]] = None,
-    rows: Optional[List[str]] = None,
+    columns: Optional[List[str]] = None,
 ) -> Textgrid:
     """Create frequency grid from database connection"""
     to_ignore = [] if to_ignore is None else to_ignore
 
     frequency_grid = make_empty_frequency_grid(
-        cursor=cursor, table_name=table_name, base_tier=word_form_tier, rows=rows
+        cursor=cursor, table_name=table_name, base_tier=word_form_tier, columns=columns
     )
 
     for i, entry in enumerate(word_form_tier.entryList):
         if (
             (not entry.label)
             or (entry.label in to_ignore)
             or (split_pos_label(entry.label) in to_ignore)
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency.egg-info/PKG-INFO` & `dynamicfluency-0.1.2/src/dynamicfluency.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicfluency
-Version: 0.1.1
+Version: 0.1.2
 Summary: The base python package for DynamicFluency: Monitor and understand the dynamicity of linguistic aspects in (L2) speech.
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/bare_python_publish
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/bare_python_publish/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -26,8 +26,10 @@
 
 ## Tests
 
 Running the development tests can be done with the following command:
 ```
 pytest --cov=dynamicfluency tests/
 ```
-Please note that this requires pytest and pytest-cov to be installed. Additionally, `dynamicfluency` has to be installed, either with `pip install -e .` or trough other means if you want to compare versions. The code itself, as it is in `src/`, isn't recognised.  
+Please note that this requires pytest and pytest-cov to be installed. Additionally, `dynamicfluency` has to be installed, either with `pip install -e .` or trough other means if you want to compare versions. The code itself, as it is in `src/`, isn't recognized.
+
+These tests will download a lot of language models on the first go, as it tests all supported languages. This will take a few minutes the first time the tests are run
```

### Comparing `dynamicfluency-0.1.1/src/dynamicfluency.egg-info/SOURCES.txt` & `dynamicfluency-0.1.2/src/dynamicfluency.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 src/dynamicfluency/__init__.py
 src/dynamicfluency/aeneas_conversion.py
+src/dynamicfluency/model_data.py
 src/dynamicfluency/pos_tagging.py
 src/dynamicfluency/repetitions.py
 src/dynamicfluency/syntactic_analysis.py
 src/dynamicfluency/word_frequencies.py
 src/dynamicfluency.egg-info/PKG-INFO
 src/dynamicfluency.egg-info/SOURCES.txt
 src/dynamicfluency.egg-info/dependency_links.txt
 src/dynamicfluency.egg-info/requires.txt
 src/dynamicfluency.egg-info/top_level.txt
-src/dynamicfluency/data/__init__.py
-src/dynamicfluency/data/valid_pos_tags.csv
 src/dynamicfluency/helpers/__init__.py
 src/dynamicfluency/helpers/conversions.py
 src/dynamicfluency/helpers/database_extensions.py
 src/dynamicfluency/helpers/filepath_extensions.py
 src/dynamicfluency/helpers/textgridtier_extensions.py
 src/dynamicfluency/scripts/add_frequency_dictionary.py
 src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py
@@ -27,9 +26,10 @@
 src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py
 src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py
 src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py
 src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py
 tests/test_aeneas.py
 tests/test_data.py
 tests/test_helpers.py
+tests/test_scripts.py
 tests/test_sql.py
 tests/test_tier_generation.py
```

### Comparing `dynamicfluency-0.1.1/tests/test_aeneas.py` & `dynamicfluency-0.1.2/tests/test_aeneas.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/tests/test_helpers.py` & `dynamicfluency-0.1.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.1/tests/test_sql.py` & `dynamicfluency-0.1.2/tests/test_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             ).tierDict["TestTier"]
         ),
         cursor=create_mock_database_from_file(
             Path(__file__).parent.joinpath("data", "test_word_form.csv")
         ),
         table_name="Mock",
         to_ignore=["uhm", "aardvark"],
-        rows=correct_word_form,
+        columns=correct_word_form,
     )
 
     def test_grid_timestamps(self):
         assert self.grid.minTimestamp == self.original_tier.minTimestamp == 0
         assert self.grid.maxTimestamp == self.original_tier.maxTimestamp == 7.2
 
     def test_tier_names(self):
```

### Comparing `dynamicfluency-0.1.1/tests/test_tier_generation.py` & `dynamicfluency-0.1.2/tests/test_tier_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     POINT_TIER,
 )
 
 from dynamicfluency.repetitions import make_freqdist_tier, make_repetitions_tier
 from dynamicfluency.pos_tagging import make_pos_tier
 from dynamicfluency.syntactic_analysis import make_syntax_grid
 from dynamicfluency.helpers import pos_tier_to_word_form_tier, split_pos_label
-from dynamicfluency.data import get_valid_tags
+from dynamicfluency.model_data import get_valid_tags
 
 from .helpers import get_test_tier
 
 
 class TestRepetitionsTier:
     original_tier = get_test_tier(
         Path(__file__).parent.joinpath("data", "testgrid_pos.TextGrid")
@@ -150,26 +150,26 @@
 
     def test_word_form_preservation_as_lowercase(self):
         word_forms = pos_tier_to_word_form_tier(self.tier)
         for new, original in zip(word_forms.entryList, self.original_tier.entryList):
             assert new.label == original.label.lower()
 
     def test_entry_pos_tags(self):
-        possible_tags = get_valid_tags()
+        possible_tags = get_valid_tags(lang="en")
         for entry in self.tier.entryList:
             tags = split_pos_label(entry.label, get_pos=True).split(" ")
             for tag in tags:
                 assert tag in possible_tags or entry.label == ""
 
 
 class TestSyntaxGrid:
     original_tier = get_test_tier(
         Path(__file__).parent.joinpath("data", "testgrid_pos.TextGrid")
     )
-    grid = make_syntax_grid(original_tier)
+    grid = make_syntax_grid(original_tier, lang="en")
     tier_phrase = grid.tierDict["Syntactic Phrases"]
     tier_clause = grid.tierDict["Syntactic Clauses"]
 
     def test_timestamps(self):
         for tier in (self.tier_phrase, self.tier_clause):
             assert tier.minTimestamp == self.original_tier.minTimestamp == 0
             assert tier.maxTimestamp == self.original_tier.maxTimestamp == 9.1
```

