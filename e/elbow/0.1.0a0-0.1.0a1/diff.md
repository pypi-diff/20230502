# Comparing `tmp/elbow-0.1.0a0.tar.gz` & `tmp/elbow-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/clane/Projects/ScalableQC/code/loaders/dist/.tmp-aldpbby4/elbow-0.1.0a0.tar", last modified: Sun Apr 30 23:16:12 2023, max compression
+gzip compressed data, was "/Users/clane/Projects/ScalableQC/code/elbow/dist/.tmp-8rwcdlyd/elbow-0.1.0a1.tar", last modified: Tue May  2 19:11:24 2023, max compression
```

## Comparing `elbow-0.1.0a0.tar` & `elbow-0.1.0a1.tar`

### file list

```diff
@@ -1,23 +1,68 @@
-drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-04-30 23:16:12.000000 elbow-0.1.0a0/
-drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-04-30 23:16:12.000000 elbow-0.1.0a0/.github/
-drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-04-30 23:16:12.000000 elbow-0.1.0a0/.github/workflows/
--rw-------   0 clane      (501) staff       (20)      787 2023-04-30 22:09:19.000000 elbow-0.1.0a0/.github/workflows/ci.yaml
--rw-------   0 clane      (501) staff       (20)      312 2023-04-30 22:06:15.000000 elbow-0.1.0a0/.gitignore
--rw-------   0 clane      (501) staff       (20)      876 2023-04-30 21:13:45.000000 elbow-0.1.0a0/.pre-commit-config.yaml
--rw-------   0 clane      (501) staff       (20)    14287 2023-04-30 21:13:45.000000 elbow-0.1.0a0/.pylintrc
--rw-------   0 clane      (501) staff       (20)     1068 2023-04-30 21:42:18.000000 elbow-0.1.0a0/LICENSE
--rw-r--r--   0 clane      (501) staff       (20)     2813 2023-04-30 23:16:12.000000 elbow-0.1.0a0/PKG-INFO
--rw-r--r--   0 clane      (501) staff       (20)      732 2023-04-30 23:14:10.000000 elbow-0.1.0a0/README.md
-drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow/
--rw-r--r--   0 clane      (501) staff       (20)        0 2023-04-30 22:04:54.000000 elbow-0.1.0a0/elbow/__init__.py
--rw-r--r--   0 clane      (501) staff       (20)      162 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow/_version.py
-drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow.egg-info/
--rw-r--r--   0 clane      (501) staff       (20)     2813 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow.egg-info/PKG-INFO
--rw-r--r--   0 clane      (501) staff       (20)      311 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow.egg-info/SOURCES.txt
--rw-r--r--   0 clane      (501) staff       (20)        1 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow.egg-info/dependency_links.txt
--rw-r--r--   0 clane      (501) staff       (20)      134 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow.egg-info/requires.txt
--rw-r--r--   0 clane      (501) staff       (20)        6 2023-04-30 23:16:12.000000 elbow-0.1.0a0/elbow.egg-info/top_level.txt
--rw-r--r--   0 clane      (501) staff       (20)     1450 2023-04-30 23:09:12.000000 elbow-0.1.0a0/pyproject.toml
--rw-r--r--   0 clane      (501) staff       (20)      103 2023-04-30 23:16:12.000000 elbow-0.1.0a0/setup.cfg
-drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-04-30 23:16:12.000000 elbow-0.1.0a0/tests/
--rw-r--r--   0 clane      (501) staff       (20)        0 2023-04-30 22:08:28.000000 elbow-0.1.0a0/tests/__init__.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/.github/
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/.github/workflows/
+-rw-------   0 clane      (501) staff       (20)      775 2023-05-01 14:22:40.000000 elbow-0.1.0a1/.github/workflows/ci.yaml
+-rw-------   0 clane      (501) staff       (20)      312 2023-04-30 22:06:15.000000 elbow-0.1.0a1/.gitignore
+-rw-------   0 clane      (501) staff       (20)      875 2023-05-01 22:11:57.000000 elbow-0.1.0a1/.pre-commit-config.yaml
+-rw-------   0 clane      (501) staff       (20)    14287 2023-04-30 21:13:45.000000 elbow-0.1.0a1/.pylintrc
+-rw-------   0 clane      (501) staff       (20)     1068 2023-04-30 21:42:18.000000 elbow-0.1.0a1/LICENSE
+-rw-r--r--   0 clane      (501) staff       (20)     1887 2023-05-02 19:11:24.000000 elbow-0.1.0a1/PKG-INFO
+-rw-r--r--   0 clane      (501) staff       (20)     1031 2023-05-02 19:07:11.000000 elbow-0.1.0a1/README.md
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow/
+-rw-r--r--   0 clane      (501) staff       (20)      192 2023-05-02 02:25:33.000000 elbow-0.1.0a1/elbow/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)      162 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow/_version.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow/dtypes/
+-rw-------   0 clane      (501) staff       (20)      736 2023-05-01 13:52:30.000000 elbow-0.1.0a1/elbow/dtypes/__init__.py
+-rw-------   0 clane      (501) staff       (20)     3396 2023-04-30 23:56:18.000000 elbow-0.1.0a1/elbow/dtypes/_json.py
+-rw-------   0 clane      (501) staff       (20)     6595 2023-05-01 00:49:31.000000 elbow-0.1.0a1/elbow/dtypes/_ndarray.py
+-rw-------   0 clane      (501) staff       (20)     4143 2023-05-01 00:00:58.000000 elbow-0.1.0a1/elbow/dtypes/_pickle.py
+-rw-------   0 clane      (501) staff       (20)     3722 2023-04-30 23:24:53.000000 elbow-0.1.0a1/elbow/dtypes/base.py
+-rw-r--r--   0 clane      (501) staff       (20)     4935 2023-05-01 21:53:10.000000 elbow-0.1.0a1/elbow/dtypes/inference.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow/extractors/
+-rw-r--r--   0 clane      (501) staff       (20)       56 2023-05-01 21:07:12.000000 elbow-0.1.0a1/elbow/extractors/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)      649 2023-05-01 14:57:53.000000 elbow-0.1.0a1/elbow/extractors/base.py
+-rw-r--r--   0 clane      (501) staff       (20)      796 2023-05-01 22:12:08.000000 elbow-0.1.0a1/elbow/extractors/meta.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow/filters/
+-rw-r--r--   0 clane      (501) staff       (20)       93 2023-05-01 19:17:21.000000 elbow-0.1.0a1/elbow/filters/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)     1799 2023-05-01 22:01:40.000000 elbow-0.1.0a1/elbow/filters/meta.py
+-rw-r--r--   0 clane      (501) staff       (20)     1391 2023-05-02 00:38:35.000000 elbow-0.1.0a1/elbow/filters/partition.py
+-rw-r--r--   0 clane      (501) staff       (20)     1143 2023-05-02 13:31:13.000000 elbow-0.1.0a1/elbow/filters/patterns.py
+-rw-r--r--   0 clane      (501) staff       (20)     4607 2023-05-02 02:23:12.000000 elbow-0.1.0a1/elbow/loaders.py
+-rw-r--r--   0 clane      (501) staff       (20)     2270 2023-05-02 00:56:45.000000 elbow-0.1.0a1/elbow/pipeline.py
+-rw-r--r--   0 clane      (501) staff       (20)    10236 2023-05-02 02:26:39.000000 elbow-0.1.0a1/elbow/record.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow/sinks/
+-rw-r--r--   0 clane      (501) staff       (20)       31 2023-05-01 16:43:00.000000 elbow-0.1.0a1/elbow/sinks/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)     4335 2023-05-01 21:02:35.000000 elbow-0.1.0a1/elbow/sinks/parquet.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow/sources/
+-rw-r--r--   0 clane      (501) staff       (20)       34 2023-05-02 13:38:45.000000 elbow-0.1.0a1/elbow/sources/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)     1933 2023-05-02 13:41:58.000000 elbow-0.1.0a1/elbow/sources/filesystem.py
+-rw-------   0 clane      (501) staff       (20)      330 2023-05-02 00:50:41.000000 elbow-0.1.0a1/elbow/typing.py
+-rw-r--r--   0 clane      (501) staff       (20)     2493 2023-05-02 00:41:28.000000 elbow-0.1.0a1/elbow/utils.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow.egg-info/
+-rw-r--r--   0 clane      (501) staff       (20)     1887 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow.egg-info/PKG-INFO
+-rw-r--r--   0 clane      (501) staff       (20)     1250 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow.egg-info/SOURCES.txt
+-rw-r--r--   0 clane      (501) staff       (20)        1 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow.egg-info/dependency_links.txt
+-rw-r--r--   0 clane      (501) staff       (20)      166 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow.egg-info/requires.txt
+-rw-r--r--   0 clane      (501) staff       (20)        6 2023-05-02 19:11:24.000000 elbow-0.1.0a1/elbow.egg-info/top_level.txt
+-rw-r--r--   0 clane      (501) staff       (20)     1500 2023-05-02 19:10:40.000000 elbow-0.1.0a1/pyproject.toml
+-rw-r--r--   0 clane      (501) staff       (20)      103 2023-05-02 19:11:24.000000 elbow-0.1.0a1/setup.cfg
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/tests/
+-rw-r--r--   0 clane      (501) staff       (20)        0 2023-04-30 22:08:28.000000 elbow-0.1.0a1/tests/__init__.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/tests/test_dtypes/
+-rw-r--r--   0 clane      (501) staff       (20)        0 2023-05-01 00:02:09.000000 elbow-0.1.0a1/tests/test_dtypes/__init__.py
+-rw-------   0 clane      (501) staff       (20)     6941 2023-05-02 18:50:33.000000 elbow-0.1.0a1/tests/test_dtypes/test_extensions.py
+-rw-------   0 clane      (501) staff       (20)     1818 2023-05-01 21:51:46.000000 elbow-0.1.0a1/tests/test_dtypes/test_inference.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/tests/test_extractors/
+-rw-r--r--   0 clane      (501) staff       (20)        0 2023-05-01 20:49:34.000000 elbow-0.1.0a1/tests/test_extractors/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)      851 2023-05-01 21:07:12.000000 elbow-0.1.0a1/tests/test_extractors/test_meta.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/tests/test_filters/
+-rw-r--r--   0 clane      (501) staff       (20)        0 2023-05-01 21:09:03.000000 elbow-0.1.0a1/tests/test_filters/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)     1338 2023-05-01 22:04:59.000000 elbow-0.1.0a1/tests/test_filters/test_meta.py
+-rw-r--r--   0 clane      (501) staff       (20)      409 2023-05-02 00:37:53.000000 elbow-0.1.0a1/tests/test_filters/test_partition.py
+-rw-r--r--   0 clane      (501) staff       (20)      865 2023-05-02 13:34:28.000000 elbow-0.1.0a1/tests/test_filters/test_patterns.py
+-rw-r--r--   0 clane      (501) staff       (20)     3427 2023-05-02 13:43:18.000000 elbow-0.1.0a1/tests/test_loaders.py
+-rw-r--r--   0 clane      (501) staff       (20)     2829 2023-05-01 14:08:22.000000 elbow-0.1.0a1/tests/test_record.py
+drwxr-xr-x   0 clane      (501) staff       (20)        0 2023-05-02 19:11:24.000000 elbow-0.1.0a1/tests/test_sinks/
+-rw-r--r--   0 clane      (501) staff       (20)        0 2023-05-01 16:41:52.000000 elbow-0.1.0a1/tests/test_sinks/__init__.py
+-rw-r--r--   0 clane      (501) staff       (20)     1484 2023-05-02 01:55:46.000000 elbow-0.1.0a1/tests/test_sinks/test_parquet.py
+-rw-------   0 clane      (501) staff       (20)     2358 2023-05-02 00:49:45.000000 elbow-0.1.0a1/tests/test_utils.py
```

### Comparing `elbow-0.1.0a0/.github/workflows/ci.yaml` & `elbow-0.1.0a1/.github/workflows/ci.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -17,16 +17,16 @@
           python-version: "3.7"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install .[dev,test]
       - name: Check quality
         run: |
-          black --check loaders tests
-          isort --check-only loaders tests
-          flake8 loaders tests
-          pylint --fail-under 9.0 loaders
-          mypy loaders 
+          black --check elbow tests
+          isort --check-only elbow tests
+          flake8 elbow tests
+          pylint --fail-under 9.0 elbow
+          mypy elbow 
       - name: Run tests
-        run: pytest --cov=loaders tests
+        run: pytest --cov=elbow tests
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
```

### Comparing `elbow-0.1.0a0/.pre-commit-config.yaml` & `elbow-0.1.0a1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 exclude: 'build|third-party|.github'
 
 default_language_version:
     python: python3
 
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: check-ast
     -   id: check-merge-conflict
     # -   id: no-commit-to-branch
     #     args: ['--branch=main']
     -   id: end-of-file-fixer
 
 -   repo: https://github.com/psf/black
-    rev: 22.10.0 # Replace by any tag/version: https://github.com/psf/black/tags
+    rev: 23.3.0 # Replace by any tag/version: https://github.com/psf/black/tags
     hooks:
       - id: black
         language_version: python3 # Should be a command that runs python3.6+
 
 -   repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
     - id: flake8
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.10.1
+  rev: 5.11.5
   hooks:
     - id: isort
       name: isort (python)
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.982
+    rev: v1.2.0
     hooks:
     - id: mypy
```

### Comparing `elbow-0.1.0a0/.pylintrc` & `elbow-0.1.0a1/.pylintrc`

 * *Files identical despite different names*

### Comparing `elbow-0.1.0a0/LICENSE` & `elbow-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `elbow-0.1.0a0/PKG-INFO` & `elbow-0.1.0a1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 Metadata-Version: 2.1
 Name: elbow
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Extract data from a bunch of files and load into a table
 Author-email: Connor Lane <connor.lane858@gmail.com>
 License: MIT License
-        
-        Copyright (c) 2023 Connor Lane
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://github.com/clane9/elbow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -40,32 +19,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Elbow
 
-Elbow is a library for extracting data from a bunch of files and loading into table (and that's it).
+Elbow is a library for extracting data from a bunch of files and loading into a table (and that's it).
 
 ## Examples
 
 ```python
 import json
 
 from elbow import load_table, load_parquet
 
-
 # Extract records from JSON-lines
 def extract(path):
     with open(path) as f:
-        for line in path:
+        for line in f:
             record = json.loads(line)
             yield record
 
-
 # Load as a pandas dataframe
 df = load_table(
     pattern="**/*.json",
     extract=extract,
 )
 
 # Load as a parquet dataset (in parallel)
@@ -78,9 +55,18 @@
 ```
 
 ## Installation
 
 A pre-release version can be installed with
 
 ```
-pip install git+https://github.com/clane9/elbow
+pip install elbow
 ```
+
+## Other (better) projects
+
+- [AirByte](https://github.com/airbytehq/airbyte)
+- [Meltano](https://github.com/meltano/meltano)
+- [Singer](https://github.com/singer-io/getting-started)
+- [Mage](https://github.com/mage-ai/mage-ai)
+- [Orchest](https://github.com/orchest/orchest)
+- [Streamz](https://github.com/python-streamz/streamz)
```

### Comparing `elbow-0.1.0a0/elbow.egg-info/PKG-INFO` & `elbow-0.1.0a1/elbow.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 Metadata-Version: 2.1
 Name: elbow
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Extract data from a bunch of files and load into a table
 Author-email: Connor Lane <connor.lane858@gmail.com>
 License: MIT License
-        
-        Copyright (c) 2023 Connor Lane
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://github.com/clane9/elbow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -40,32 +19,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Elbow
 
-Elbow is a library for extracting data from a bunch of files and loading into table (and that's it).
+Elbow is a library for extracting data from a bunch of files and loading into a table (and that's it).
 
 ## Examples
 
 ```python
 import json
 
 from elbow import load_table, load_parquet
 
-
 # Extract records from JSON-lines
 def extract(path):
     with open(path) as f:
-        for line in path:
+        for line in f:
             record = json.loads(line)
             yield record
 
-
 # Load as a pandas dataframe
 df = load_table(
     pattern="**/*.json",
     extract=extract,
 )
 
 # Load as a parquet dataset (in parallel)
@@ -78,9 +55,18 @@
 ```
 
 ## Installation
 
 A pre-release version can be installed with
 
 ```
-pip install git+https://github.com/clane9/elbow
+pip install elbow
 ```
+
+## Other (better) projects
+
+- [AirByte](https://github.com/airbytehq/airbyte)
+- [Meltano](https://github.com/meltano/meltano)
+- [Singer](https://github.com/singer-io/getting-started)
+- [Mage](https://github.com/mage-ai/mage-ai)
+- [Orchest](https://github.com/orchest/orchest)
+- [Streamz](https://github.com/python-streamz/streamz)
```

### Comparing `elbow-0.1.0a0/pyproject.toml` & `elbow-0.1.0a1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,46 +6,48 @@
 name = "elbow"
 description = "Extract data from a bunch of files and load into a table"
 authors = [
     {name = "Connor Lane", email = "connor.lane858@gmail.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
-license = {file = "LICENSE"}
+license = {text = "MIT License"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
+    "typing_extensions",
     "numpy",
     "pandas",
     "pyarrow",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
 ]
 dev = [
-    "black==22.10.0",
+    "black==23.3.0",
     "flake8==5.0.4",
-    "isort==5.10.1",
-    "mypy==0.982",
+    "isort==5.11.5",
+    "mypy==1.2.0",
     "pre-commit",
     "pylint>=2.5.0",
+    "setuptools-scm",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/clane9/elbow"
 
 [tool.setuptools_scm]
 write_to = "elbow/_version.py"
```

