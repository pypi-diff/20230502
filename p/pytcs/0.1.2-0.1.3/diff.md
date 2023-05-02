# Comparing `tmp/pytcs-0.1.2.tar.gz` & `tmp/pytcs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytcs-0.1.2.tar", last modified: Mon Apr 17 13:02:54 2023, max compression
+gzip compressed data, was "pytcs-0.1.3.tar", last modified: Tue May  2 18:50:01 2023, max compression
```

## Comparing `pytcs-0.1.2.tar` & `pytcs-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 13:02:31.000000 pytcs-0.1.2/.github/workflows/static_analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-17 13:02:31.000000 pytcs-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-17 13:02:31.000000 pytcs-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-17 13:02:31.000000 pytcs-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-17 13:02:31.000000 pytcs-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 13:02:31.000000 pytcs-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-17 13:02:54.250518 pytcs-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-17 13:02:31.000000 pytcs-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/devtools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/devtools/conda.recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-17 13:02:31.000000 pytcs-0.1.2/devtools/conda.recipe/build_env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-17 13:02:31.000000 pytcs-0.1.2/devtools/conda.recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-17 13:02:31.000000 pytcs-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/pytcs/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 13:02:31.000000 pytcs-0.1.2/pytcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-17 13:02:31.000000 pytcs-0.1.2/pytcs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-04-17 13:02:31.000000 pytcs-0.1.2/pytcs/pytcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:02:54.250518 pytcs-0.1.2/pytcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 13:02:54.000000 pytcs-0.1.2/pytcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:02:54.250518 pytcs-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:50:01.627356 pytcs-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:50:01.627356 pytcs-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 18:49:39.000000 pytcs-0.1.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:50:01.627356 pytcs-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-02 18:49:39.000000 pytcs-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-02 18:49:39.000000 pytcs-0.1.3/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 18:49:39.000000 pytcs-0.1.3/.github/workflows/static_analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-02 18:49:39.000000 pytcs-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-02 18:49:39.000000 pytcs-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-02 18:49:39.000000 pytcs-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-02 18:49:39.000000 pytcs-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 18:49:39.000000 pytcs-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-05-02 18:50:01.627356 pytcs-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-02 18:49:39.000000 pytcs-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:50:01.623356 pytcs-0.1.3/devtools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:50:01.627356 pytcs-0.1.3/devtools/conda.recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 18:49:39.000000 pytcs-0.1.3/devtools/conda.recipe/build_env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-02 18:49:39.000000 pytcs-0.1.3/devtools/conda.recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-02 18:49:39.000000 pytcs-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:50:01.627356 pytcs-0.1.3/pytcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 18:49:39.000000 pytcs-0.1.3/pytcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 18:50:01.000000 pytcs-0.1.3/pytcs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-02 18:49:39.000000 pytcs-0.1.3/pytcs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28832 2023-05-02 18:49:39.000000 pytcs-0.1.3/pytcs/pytcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:50:01.627356 pytcs-0.1.3/pytcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-05-02 18:50:01.000000 pytcs-0.1.3/pytcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-02 18:50:01.000000 pytcs-0.1.3/pytcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:50:01.000000 pytcs-0.1.3/pytcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 18:50:01.000000 pytcs-0.1.3/pytcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 18:50:01.000000 pytcs-0.1.3/pytcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:50:01.627356 pytcs-0.1.3/setup.cfg
```

### Comparing `pytcs-0.1.2/.github/workflows/build.yml` & `pytcs-0.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.2/.github/workflows/pytest.yml` & `pytcs-0.1.3/.github/workflows/pytest.yml`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       matrix:
         os: [ubuntu-latest]
         py: ['3.8', '3.9', '3.10', '3.11']
         pandas: [ '1.*' ]
         include:
           - os: ubuntu-latest
             py: '3.10'
-            pandas: '1.3'
+            pandas: '1.4'
           - os: ubuntu-latest
             py: '3.10'
-            pandas: '1.4'
+            pandas: '2.*'
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: '0' # Fetch all history for all tags and branches
 
       - uses: CagtayFabry/pydeps2env@main
         with:
@@ -41,14 +41,15 @@
       - uses: mamba-org/provision-with-micromamba@v15
         with:
           environment-file: ./environment.yml
           environment-name: pytcs
           cache-env: true
           extra-specs: |
             python=${{ matrix.py }}
+            pandas=${{ matrix.pandas }}
 
       - name: activate env
         run: micromamba activate pytcs
 
       - name: pip installs
         run: |
           python -m pip install -e .
```

### Comparing `pytcs-0.1.2/.gitignore` & `pytcs-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.2/.pre-commit-config.yaml` & `pytcs-0.1.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,21 @@
           - mdformat-config
   # ----- Python formatting -----
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.263
     hooks:
       - id: ruff
         args:
           - --quiet
           - --fix
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.9.2
+    rev: 0.11.1
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.12.2
     hooks:
       - id: validate-pyproject
```

### Comparing `pytcs-0.1.2/CHANGELOG.md` & `pytcs-0.1.3/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # pytcs
 
+## v0.1.3
+
+### added
+
+- add experimental support for `pyarrow` pandas backend #18
+
+### fixed
+
+- fixed gzip support when reading from `BytesIO` #18
+
 ## v0.1.2
 
 ### added
 
-- add support for reading `StringIO` and `BytesIO` #10
+- add support for reading `StringIO` and `BytesIO` #11
 
 ### fixed
 
 - explicitly sort index in `ScopeFile.as_pandas` #16
 
 ## v0.1.1
```

### Comparing `pytcs-0.1.2/LICENSE` & `pytcs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.2/PKG-INFO` & `pytcs-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytcs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python API for processing TwinCAT Scope data files
 Author-email: Cagtay Fabry <cagtay.fabry@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Cagtay Fabry
         All rights reserved.
         
@@ -35,16 +35,16 @@
         
 Project-URL: bug_tracker, https://github.com/CagtayFabry/pytcs/issues
 Project-URL: repository, https://github.com/CagtayFabry/pytcs
 Keywords: file reader,TwinCAT,TwinCAT Scope
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `pytcs-0.1.2/README.md` & `pytcs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.2/devtools/conda.recipe/meta.yaml` & `pytcs-0.1.3/devtools/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.2/pyproject.toml` & `pytcs-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 ]
 license = {file = "LICENSE", name="BSD License"}
 authors = [
     {name="Cagtay Fabry", email="cagtay.fabry@bam.de"},
 ]
 requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: BSD License",
-    "Operating System :: OS Independent",
-    "Natural Language :: English",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
+  "Development Status :: 3 - Alpha",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: BSD License",
+  "Natural Language :: English",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
 dynamic = [
   # see: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
   "version", # version gets derived from git by setuptools_scm.
 ]
 dependencies = [
   "bidict",
   "numpy",
-  "pandas>=1.2",
+  "pandas>=1.4",
 ]
 [project.optional-dependencies]
 all = [
   "bottleneck>=1.3",
   "pint>=0.18",
   "xarray>=0.15",
 ]
@@ -46,14 +46,15 @@
 export = [
   # needed to create the test files using create_scope_configs.py
   "dicttoxml",
   "pyyaml",
 ]
 test = [
   # needed to run the test suite
+  "pyarrow",
   "pytest",
   "pytest-cov",
   "pytest-xdist",
 ]
 [project.urls]
 bug_tracker = "https://github.com/CagtayFabry/pytcs/issues"
 repository = "https://github.com/CagtayFabry/pytcs"
```

### Comparing `pytcs-0.1.2/pytcs/helpers.py` & `pytcs-0.1.3/pytcs/helpers.py`

 * *Files identical despite different names*

### Comparing `pytcs-0.1.2/pytcs/pytcs.py` & `pytcs-0.1.3/pytcs/pytcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """pytcs - Python API for reading TwinCAT Scope Files."""
 from __future__ import annotations
 
 import gzip
+import importlib
 from collections.abc import ItemsView, Iterator, ValuesView
 from dataclasses import dataclass, field
 from datetime import datetime
 from io import BytesIO, IOBase, StringIO
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, KeysView, Union
@@ -223,14 +224,16 @@
         usecols = self._get_usecols(channels)
 
         if not usecols:  # already loaded
             return
 
         if backend == "pandas":
             data_dict = self._read_pandas(usecols, native_dtypes)
+        elif backend == "pyarrow":
+            data_dict = self._read_pyarrow(usecols, native_dtypes)
         elif backend == "datatable":
             if native_dtypes:
                 warn(
                     "Ignoring option 'native_dtypes' with datatable backend.",
                     UserWarning,
                     stacklevel=2,
                 )
@@ -572,32 +575,107 @@
     def _read_pandas(
         self, usecols: list[int], native_dtypes: bool
     ) -> dict[str, np.ndarray]:
         """Read data into dictionary using the pandas backend."""
         if isinstance(self._file, IOBase):  # read open streams from beginning
             self._file.seek(0)
 
+        compression = self._compression
+        if isinstance(self._file, BytesIO):  # assume gzip
+            compression = "gzip"
+
         df = pd.read_csv(
             self._file,
             delimiter=self._delimiter,
             skiprows=self._header_lines,
             decimal=self._decimal,
             header=None,
             usecols=usecols,
             names=self._get_cols(),
             index_col=False,
             encoding=self._encoding,
             na_values=[" ", "EOF"],
             skip_blank_lines=True,
             engine="c",
             low_memory=False,
-            compression=self._compression,
+            compression=compression,
+        )
+
+        if native_dtypes:
+            tc3_dtypes = get_tc3_dtypes()
+            dtypes_np = {
+                v.value_col: tc3_dtypes[v.info.get("Data-Type", "REAL64")][0]
+                for v in self._channels.values()
+            }
+            dtypes_times = {k: np.float64 for k in self._get_time_cols()}
+            dtypes_np.update(dtypes_times)
+            data_dict = {k: df[k].dropna().to_numpy(dtypes_np[k]) for k in df}
+        else:
+            data_dict = {k: df[k].dropna().to_numpy(np.float64) for k in df}
+
+        return data_dict
+
+    def _read_pyarrow(
+        self, usecols: list[int], native_dtypes: bool
+    ) -> dict[str, np.ndarray]:
+        """Read data into dictionary using the pyarrow backend of pandas."""
+        from itertools import groupby
+
+        if not importlib.util.find_spec("pyarrow"):
+            warn(
+                "'pyarrow' backend not found, using default pandas implementation.",
+                UserWarning,
+                stacklevel=2,
+            )
+            return self._read_pandas(usecols, native_dtypes)
+
+        def all_equal(iterable):
+            "Returns True if all the elements are equal to each other"
+            g = groupby(iterable)
+            return next(g, True) and not next(g, False)
+
+        if usecols:
+            warn(
+                """Channel selection is not supported with 'pyarrow' backend, """
+                """loading all channels.""",
+                UserWarning,
+                stacklevel=2,
+            )
+            usecols = None
+
+        if not all_equal(self[c].sample_time for c in self):
+            raise ValueError(
+                "Unsupported file format for 'pyarrow' backend. (unequal sample times)"
+            )
+
+        if isinstance(self._file, IOBase):  # read open streams from beginning
+            self._file.seek(0)
+
+        compression = self._compression
+        if isinstance(self._file, BytesIO):  # assume gzip
+            compression = "gzip"
+
+        df = pd.read_csv(
+            self._file,
+            delimiter=self._delimiter,
+            skiprows=self._header_lines,
+            # decimal=self._decimal, # unsupported with pyarrow
+            header=None,
+            usecols=usecols,
+            names=self._get_cols(),
+            # index_col=False,
+            encoding=self._encoding,
+            na_values=[" ", "EOF"],
+            skip_blank_lines=True,
+            engine="pyarrow",
+            # low_memory=False, # unsupported with pyarrow
+            compression=compression,
         )
 
-        # self._df = df  # debug
+        self._df = df
 
         if native_dtypes:
             tc3_dtypes = get_tc3_dtypes()
             dtypes_np = {
                 v.value_col: tc3_dtypes[v.info.get("Data-Type", "REAL64")][0]
                 for v in self._channels.values()
             }
```

### Comparing `pytcs-0.1.2/pytcs.egg-info/PKG-INFO` & `pytcs-0.1.3/pytcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytcs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python API for processing TwinCAT Scope data files
 Author-email: Cagtay Fabry <cagtay.fabry@bam.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Cagtay Fabry
         All rights reserved.
         
@@ -35,16 +35,16 @@
         
 Project-URL: bug_tracker, https://github.com/CagtayFabry/pytcs/issues
 Project-URL: repository, https://github.com/CagtayFabry/pytcs
 Keywords: file reader,TwinCAT,TwinCAT Scope
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

