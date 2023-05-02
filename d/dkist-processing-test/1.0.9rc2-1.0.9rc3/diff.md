# Comparing `tmp/dkist-processing-test-1.0.9rc2.tar.gz` & `tmp/dkist-processing-test-1.0.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-test-1.0.9rc2.tar", last modified: Mon Jan 30 20:33:57 2023, max compression
+gzip compressed data, was "dkist-processing-test-1.0.9rc3.tar", last modified: Mon Jan 30 22:30:23 2023, max compression
```

## Comparing `dkist-processing-test-1.0.9rc2.tar` & `dkist-processing-test-1.0.9rc3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/dkist_processing_test/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/dkist_processing_test/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/models/parameters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/fail.py
--rw-rw-rw-   0 root         (0) root         (0)     2292 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/fake_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/movie.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/noop.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2411 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    13359 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/test_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4418 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/common_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/end_to_end.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/fail.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/noop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-01-30 20:33:57.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-01-30 20:33:57.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-30 20:33:57.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-01-30 20:33:57.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 20:33:57.000000 dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-01-30 20:33:57.091383 dkist-processing-test-1.0.9rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-01-30 20:33:50.000000 dkist-processing-test-1.0.9rc2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/models/parameters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/fake_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/movie.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    13504 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4418 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/common_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/end_to_end.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/noop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-30 22:30:23.411895 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 22:30:23.000000 dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-01-30 22:30:23.415895 dkist-processing-test-1.0.9rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-01-30 22:30:16.000000 dkist-processing-test-1.0.9rc3/setup.py
```

### Comparing `dkist-processing-test-1.0.9rc2/.gitignore` & `dkist-processing-test-1.0.9rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/.pre-commit-config.yaml` & `dkist-processing-test-1.0.9rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/PKG-INFO` & `dkist-processing-test-1.0.9rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.0.9rc2
+Version: 1.0.9rc3
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.0.9rc2/README.rst` & `dkist-processing-test-1.0.9rc3/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/bitbucket-pipelines.yml` & `dkist-processing-test-1.0.9rc3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/models/parameters.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/exercise_numba.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/exercise_numba.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/fake_science.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/fake_science.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
                 with self.apm_processing_step("Doing some calculations"):
                     header["DSPSNUM"] = count
                     data = hdu.data
 
                     # Just do some weird crap. We don't use the loaded random array directly so that we
                     # don't have to care that the shapes are the same as the "real" data.
                     random_signal = rng.normal(*self.parameters.randomness, size=data.shape)
-                    data += random_signal
+                    data = (
+                        data + random_signal
+                    )  # Needs to be like this because data will start as int-type
                     data += self.parameters.constant
                     output_hdu = fits.PrimaryHDU(data=data, header=header)
 
                 with self.apm_writing_step("Writing data"):
                     output_hdul = fits.HDUList([output_hdu])
                     self.fits_data_write(
                         hdu_list=output_hdul,
```

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/movie.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/parse.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tasks/write_l1.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/conftest.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/test_parameters.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/tests/test_tasks.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/tests/test_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,17 @@
             dataset_shape=(number_of_frames, 512, 512),
             array_shape=(1, 512, 512),
             time_delta=10,
         )
         # load input data
         for idx, input_frame in enumerate(input_frame_set):
             hdu = input_frame.hdu()
+            hdu.data = (
+                np.ones(hdu.data.shape, dtype=int) * 10
+            )  # Because input data will be ints in test system
             hdu.header["DSPSNUM"] = 1
             hdul = fits.HDUList([hdu])
             file_name = f"input_{idx}.fits"
             task.fits_data_write(hdu_list=hdul, tags=Tag.input(), relative_path=file_name)
 
         # Write parameter file
         hdul = random_parameter_hdulist[0]
```

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/common_tasks.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/common_tasks.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/end_to_end.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/end_to_end.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test/workflows/noop.py` & `dkist-processing-test-1.0.9rc3/dkist_processing_test/workflows/noop.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/PKG-INFO` & `dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.0.9rc2
+Version: 1.0.9rc3
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.0.9rc2/dkist_processing_test.egg-info/SOURCES.txt` & `dkist-processing-test-1.0.9rc3/dkist_processing_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.0.9rc2/setup.cfg` & `dkist-processing-test-1.0.9rc3/setup.cfg`

 * *Files identical despite different names*

