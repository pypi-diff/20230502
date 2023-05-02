# Comparing `tmp/pandarallel-1.6.4.tar.gz` & `tmp/pandarallel-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandarallel-1.6.4.tar", last modified: Sun Jan 15 19:58:06 2023, max compression
+gzip compressed data, was "pandarallel-1.6.5.tar", last modified: Sat Apr 29 12:10:51 2023, max compression
```

## Comparing `pandarallel-1.6.4.tar` & `pandarallel-1.6.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-01-15 19:58:06.446479 pandarallel-1.6.4/
--rw-r--r--   0 manu       (501) staff       (20)     1511 2022-08-02 22:41:46.000000 pandarallel-1.6.4/LICENSE
--rw-r--r--   0 manu       (501) staff       (20)       16 2022-08-02 22:41:46.000000 pandarallel-1.6.4/MANIFEST.in
--rw-r--r--   0 manu       (501) staff       (20)     2272 2023-01-15 19:58:06.446549 pandarallel-1.6.4/PKG-INFO
--rw-r--r--   0 manu       (501) staff       (20)     1636 2022-11-27 20:05:11.000000 pandarallel-1.6.4/README.md
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-01-15 19:58:06.443764 pandarallel-1.6.4/pandarallel/
--rw-r--r--   0 manu       (501) staff       (20)       53 2023-01-15 19:57:53.000000 pandarallel-1.6.4/pandarallel/__init__.py
--rw-r--r--   0 manu       (501) staff       (20)    19140 2023-01-15 19:27:29.000000 pandarallel-1.6.4/pandarallel/core.py
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-01-15 19:58:06.446242 pandarallel-1.6.4/pandarallel/data_types/
--rw-r--r--   0 manu       (501) staff       (20)      272 2023-01-15 19:27:29.000000 pandarallel-1.6.4/pandarallel/data_types/__init__.py
--rw-r--r--   0 manu       (501) staff       (20)     2562 2022-08-09 09:51:49.000000 pandarallel-1.6.4/pandarallel/data_types/dataframe.py
--rw-r--r--   0 manu       (501) staff       (20)     3126 2022-08-02 23:12:53.000000 pandarallel-1.6.4/pandarallel/data_types/dataframe_groupby.py
--rw-r--r--   0 manu       (501) staff       (20)     3380 2022-08-02 22:41:46.000000 pandarallel-1.6.4/pandarallel/data_types/expanding_groupby.py
--rw-r--r--   0 manu       (501) staff       (20)      879 2022-08-02 23:14:03.000000 pandarallel-1.6.4/pandarallel/data_types/generic.py
--rw-r--r--   0 manu       (501) staff       (20)     3366 2022-08-02 22:41:46.000000 pandarallel-1.6.4/pandarallel/data_types/rolling_groupby.py
--rw-r--r--   0 manu       (501) staff       (20)     1886 2022-11-27 20:05:11.000000 pandarallel-1.6.4/pandarallel/data_types/series.py
--rw-r--r--   0 manu       (501) staff       (20)     1633 2022-08-02 22:41:46.000000 pandarallel-1.6.4/pandarallel/data_types/series_rolling.py
--rw-r--r--   0 manu       (501) staff       (20)     6235 2023-01-15 18:08:27.000000 pandarallel-1.6.4/pandarallel/progress_bars.py
--rw-r--r--   0 manu       (501) staff       (20)     2636 2022-08-02 23:14:43.000000 pandarallel-1.6.4/pandarallel/utils.py
-drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-01-15 19:58:06.444524 pandarallel-1.6.4/pandarallel.egg-info/
--rw-r--r--   0 manu       (501) staff       (20)     2272 2023-01-15 19:58:06.000000 pandarallel-1.6.4/pandarallel.egg-info/PKG-INFO
--rw-r--r--   0 manu       (501) staff       (20)      625 2023-01-15 19:58:06.000000 pandarallel-1.6.4/pandarallel.egg-info/SOURCES.txt
--rw-r--r--   0 manu       (501) staff       (20)        1 2023-01-15 19:58:06.000000 pandarallel-1.6.4/pandarallel.egg-info/dependency_links.txt
--rw-r--r--   0 manu       (501) staff       (20)       83 2023-01-15 19:58:06.000000 pandarallel-1.6.4/pandarallel.egg-info/requires.txt
--rw-r--r--   0 manu       (501) staff       (20)       12 2023-01-15 19:58:06.000000 pandarallel-1.6.4/pandarallel.egg-info/top_level.txt
--rw-r--r--   0 manu       (501) staff       (20)      822 2023-01-15 19:58:06.446847 pandarallel-1.6.4/setup.cfg
--rw-r--r--   0 manu       (501) staff       (20)       38 2022-08-02 22:41:46.000000 pandarallel-1.6.4/setup.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-04-29 12:10:51.269602 pandarallel-1.6.5/
+-rw-r--r--   0 manu       (501) staff       (20)     1511 2022-08-02 22:41:46.000000 pandarallel-1.6.5/LICENSE
+-rw-r--r--   0 manu       (501) staff       (20)       16 2022-08-02 22:41:46.000000 pandarallel-1.6.5/MANIFEST.in
+-rw-r--r--   0 manu       (501) staff       (20)     2275 2023-04-29 12:10:51.269673 pandarallel-1.6.5/PKG-INFO
+-rw-r--r--   0 manu       (501) staff       (20)     1636 2022-11-27 20:05:11.000000 pandarallel-1.6.5/README.md
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-04-29 12:10:51.267628 pandarallel-1.6.5/pandarallel/
+-rw-r--r--   0 manu       (501) staff       (20)       53 2023-04-29 12:10:36.000000 pandarallel-1.6.5/pandarallel/__init__.py
+-rw-r--r--   0 manu       (501) staff       (20)    19173 2023-04-29 12:09:24.000000 pandarallel-1.6.5/pandarallel/core.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-04-29 12:10:51.269263 pandarallel-1.6.5/pandarallel/data_types/
+-rw-r--r--   0 manu       (501) staff       (20)      272 2023-01-15 19:27:29.000000 pandarallel-1.6.5/pandarallel/data_types/__init__.py
+-rw-r--r--   0 manu       (501) staff       (20)     2562 2022-08-09 09:51:49.000000 pandarallel-1.6.5/pandarallel/data_types/dataframe.py
+-rw-r--r--   0 manu       (501) staff       (20)     3076 2023-04-29 12:09:24.000000 pandarallel-1.6.5/pandarallel/data_types/dataframe_groupby.py
+-rw-r--r--   0 manu       (501) staff       (20)     3380 2022-08-02 22:41:46.000000 pandarallel-1.6.5/pandarallel/data_types/expanding_groupby.py
+-rw-r--r--   0 manu       (501) staff       (20)      879 2022-08-02 23:14:03.000000 pandarallel-1.6.5/pandarallel/data_types/generic.py
+-rw-r--r--   0 manu       (501) staff       (20)     3366 2022-08-02 22:41:46.000000 pandarallel-1.6.5/pandarallel/data_types/rolling_groupby.py
+-rw-r--r--   0 manu       (501) staff       (20)     1886 2022-11-27 20:05:11.000000 pandarallel-1.6.5/pandarallel/data_types/series.py
+-rw-r--r--   0 manu       (501) staff       (20)     1633 2022-08-02 22:41:46.000000 pandarallel-1.6.5/pandarallel/data_types/series_rolling.py
+-rw-r--r--   0 manu       (501) staff       (20)     6235 2023-04-29 12:09:20.000000 pandarallel-1.6.5/pandarallel/progress_bars.py
+-rw-r--r--   0 manu       (501) staff       (20)     2636 2022-08-02 23:14:43.000000 pandarallel-1.6.5/pandarallel/utils.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-04-29 12:10:51.268190 pandarallel-1.6.5/pandarallel.egg-info/
+-rw-r--r--   0 manu       (501) staff       (20)     2275 2023-04-29 12:10:51.000000 pandarallel-1.6.5/pandarallel.egg-info/PKG-INFO
+-rw-r--r--   0 manu       (501) staff       (20)      651 2023-04-29 12:10:51.000000 pandarallel-1.6.5/pandarallel.egg-info/SOURCES.txt
+-rw-r--r--   0 manu       (501) staff       (20)        1 2023-04-29 12:10:51.000000 pandarallel-1.6.5/pandarallel.egg-info/dependency_links.txt
+-rw-r--r--   0 manu       (501) staff       (20)       83 2023-04-29 12:10:51.000000 pandarallel-1.6.5/pandarallel.egg-info/requires.txt
+-rw-r--r--   0 manu       (501) staff       (20)       12 2023-04-29 12:10:51.000000 pandarallel-1.6.5/pandarallel.egg-info/top_level.txt
+-rw-r--r--   0 manu       (501) staff       (20)      846 2023-04-29 12:10:51.269953 pandarallel-1.6.5/setup.cfg
+-rw-r--r--   0 manu       (501) staff       (20)       38 2022-08-02 22:41:46.000000 pandarallel-1.6.5/setup.py
+drwxr-xr-x   0 manu       (501) staff       (20)        0 2023-04-29 12:10:51.269473 pandarallel-1.6.5/tests/
+-rw-r--r--   0 manu       (501) staff       (20)    10361 2023-04-29 12:09:24.000000 pandarallel-1.6.5/tests/test_pandarallel.py
```

### Comparing `pandarallel-1.6.4/LICENSE` & `pandarallel-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/PKG-INFO` & `pandarallel-1.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pandarallel
-Version: 1.6.4
+Version: 1.6.5
 Summary: An easy to use library to speed up computation (by parallelizing on multi CPUs) with pandas.
 Home-page: https://nalepae.github.io/pandarallel
 Author: Manu NALEPA
 Author-email: nalepae@gmail.com
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # Pandaral·lel
 
@@ -57,9 +57,7 @@
 
 ## Examples
 
 An example of each available `pandas` API is available:
 
 - For [Mac & Linux](https://github.com/nalepae/pandarallel/blob/master/docs/examples_mac_linux.ipynb)
 - For [Windows](https://github.com/nalepae/pandarallel/blob/master/docs/examples_windows.ipynb)
-
-
```

### Comparing `pandarallel-1.6.4/README.md` & `pandarallel-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/core.py` & `pandarallel-1.6.5/pandarallel/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .progress_bars import ProgressBarsType, get_progress_bars, progress_wrapper
 from .utils import WorkerStatus
 
 ON_WINDOWS = os.name == "nt"
 CONTEXT = multiprocessing.get_context("spawn" if ON_WINDOWS else "fork")
 
 # Root of Memory File System
-MEMORY_FS_ROOT = "/dev/shm"
+MEMORY_FS_ROOT = os.environ.get("MEMORY_FS_ROOT", "/dev/shm")
 
 # By default, Pandarallel use all available CPUs
 NB_PHYSICAL_CORES = psutil.cpu_count(logical=False)
 
 # Prefix and suffix for files used with Memory File System
 PREFIX = "pandarallel"
 PREFIX_INPUT = f"{PREFIX}_input_"
@@ -325,15 +325,15 @@
                 return wrapped_reduce_function(
                     (Path(output_file.name) for output_file in output_files),
                     reduce_extra,
                 )
             except EOFError:
                 # Loading the files failed, this most likely means that there
                 # was some error during processing and the files were never
-                # saved at all. 
+                # saved at all.
                 results_promise.get()
 
                 # If the above statement does not raise an exception, that
                 # means the multiprocessing went well and we want to re-raise
                 # the original EOFError.
                 raise
```

### Comparing `pandarallel-1.6.4/pandarallel/data_types/dataframe.py` & `pandarallel-1.6.5/pandarallel/data_types/dataframe.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/data_types/dataframe_groupby.py` & `pandarallel-1.6.5/pandarallel/data_types/dataframe_groupby.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,11 +73,9 @@
             keys, values, mutated = zip(*results)
 
             keys = cast(List[int], keys)
             values = cast(List[pd.DataFrame], values)
             mutated = cast(List[bool], mutated)
 
             args = get_args(keys, values, df_groupby)
-
-            return df_groupby._wrap_applied_output(
-                *args, not_indexed_same=df_groupby.mutated or mutated
-            )
+  
+            return df_groupby._wrap_applied_output(*args, not_indexed_same=mutated)
```

### Comparing `pandarallel-1.6.4/pandarallel/data_types/expanding_groupby.py` & `pandarallel-1.6.5/pandarallel/data_types/expanding_groupby.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/data_types/generic.py` & `pandarallel-1.6.5/pandarallel/data_types/generic.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/data_types/rolling_groupby.py` & `pandarallel-1.6.5/pandarallel/data_types/rolling_groupby.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/data_types/series.py` & `pandarallel-1.6.5/pandarallel/data_types/series.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/data_types/series_rolling.py` & `pandarallel-1.6.5/pandarallel/data_types/series_rolling.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/progress_bars.py` & `pandarallel-1.6.5/pandarallel/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel/utils.py` & `pandarallel-1.6.5/pandarallel/utils.py`

 * *Files identical despite different names*

### Comparing `pandarallel-1.6.4/pandarallel.egg-info/PKG-INFO` & `pandarallel-1.6.5/pandarallel.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pandarallel
-Version: 1.6.4
+Version: 1.6.5
 Summary: An easy to use library to speed up computation (by parallelizing on multi CPUs) with pandas.
 Home-page: https://nalepae.github.io/pandarallel
 Author: Manu NALEPA
 Author-email: nalepae@gmail.com
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # Pandaral·lel
 
@@ -57,9 +57,7 @@
 
 ## Examples
 
 An example of each available `pandas` API is available:
 
 - For [Mac & Linux](https://github.com/nalepae/pandarallel/blob/master/docs/examples_mac_linux.ipynb)
 - For [Windows](https://github.com/nalepae/pandarallel/blob/master/docs/examples_windows.ipynb)
-
-
```

### Comparing `pandarallel-1.6.4/pandarallel.egg-info/SOURCES.txt` & `pandarallel-1.6.5/pandarallel.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 pandarallel/data_types/__init__.py
 pandarallel/data_types/dataframe.py
 pandarallel/data_types/dataframe_groupby.py
 pandarallel/data_types/expanding_groupby.py
 pandarallel/data_types/generic.py
 pandarallel/data_types/rolling_groupby.py
 pandarallel/data_types/series.py
-pandarallel/data_types/series_rolling.py
+pandarallel/data_types/series_rolling.py
+tests/test_pandarallel.py
```

### Comparing `pandarallel-1.6.4/setup.cfg` & `pandarallel-1.6.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://nalepae.github.io/pandarallel
 author = Manu NALEPA
 author_email = nalepae@gmail.com
 license = BSD
 license_file = LICENSE
-version = 1.6.4
+version = 1.6.5
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
+python_requires = >=3.7
 install_requires = 
 	dill >= 0.3.1
 	pandas >= 1
 	psutil
 
 [options.packages.find]
 exclude =
```

