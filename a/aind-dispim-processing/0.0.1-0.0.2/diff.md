# Comparing `tmp/aind_dispim_processing-0.0.1.tar.gz` & `tmp/aind_dispim_processing-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_dispim_processing-0.0.1.tar", last modified: Mon May  1 18:20:25 2023, max compression
+gzip compressed data, was "aind_dispim_processing-0.0.2.tar", last modified: Mon May  1 21:39:56 2023, max compression
```

## Comparing `aind_dispim_processing-0.0.1.tar` & `aind_dispim_processing-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.411288 aind_dispim_processing-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.411288 aind_dispim_processing-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/run
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.411288 aind_dispim_processing-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/src/aind_dispim_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 18:20:08.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing/converter_capsule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing/logging_capsule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing/registration_capsule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-01 18:20:25.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-01 18:20:25.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:20:25.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-01 18:20:25.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 18:20:25.000000 aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:25.415288 aind_dispim_processing-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 18:20:07.000000 aind_dispim_processing-0.0.1/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.105711 aind_dispim_processing-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.101711 aind_dispim_processing-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.101711 aind_dispim_processing-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.101711 aind_dispim_processing-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-01 21:39:56.105711 aind_dispim_processing-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.101711 aind_dispim_processing-0.0.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.101711 aind_dispim_processing-0.0.2/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.105711 aind_dispim_processing-0.0.2/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/run
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:39:56.105711 aind_dispim_processing-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.101711 aind_dispim_processing-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.105711 aind_dispim_processing-0.0.2/src/aind_dispim_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 21:39:40.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing/converter_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing/logging_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing/registration_capsule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.105711 aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-01 21:39:56.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-01 21:39:56.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:39:56.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 21:39:56.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 21:39:56.000000 aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:39:56.105711 aind_dispim_processing-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 21:39:39.000000 aind_dispim_processing-0.0.2/tests/test_example.py
```

### Comparing `aind_dispim_processing-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_dispim_processing-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_dispim_processing-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind_dispim_processing-0.0.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/.github/workflows/tag_and_publish.yml` & `aind_dispim_processing-0.0.2/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/.github/workflows/test_and_lint.yml` & `aind_dispim_processing-0.0.2/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/.gitignore` & `aind_dispim_processing-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/LICENSE` & `aind_dispim_processing-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/PKG-INFO` & `aind_dispim_processing-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_dispim_processing
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for Dispim Code Ocean Pipeline
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_dispim_processing-0.0.1/README.md` & `aind_dispim_processing-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/doc_template/Makefile` & `aind_dispim_processing-0.0.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/doc_template/make.bat` & `aind_dispim_processing-0.0.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/doc_template/source/_static/dark-logo.svg` & `aind_dispim_processing-0.0.2/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/doc_template/source/_static/favicon.ico` & `aind_dispim_processing-0.0.2/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/doc_template/source/_static/light-logo.svg` & `aind_dispim_processing-0.0.2/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/doc_template/source/conf.py` & `aind_dispim_processing-0.0.2/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/pyproject.toml` & `aind_dispim_processing-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
     'argschema', 
     'aind-data-transfer',
-    'aind-ng-link',
-    'boto3'
+    'aind-ng-link'
 ]
 
 [project.optional-dependencies]
 dev = [
     'black',
     'coverage',
     'flake8',
```

### Comparing `aind_dispim_processing-0.0.1/src/aind_dispim_processing/converter_capsule.py` & `aind_dispim_processing-0.0.2/src/aind_dispim_processing/converter_capsule.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 
     output_path = fld.String(
         required=True,
         metadata={"description": "Output path of registration xml"},
     )
 
 
-def write_json(bucket_name: str, path: str, json_data: dict):
-    """Writes json dict to bucket/path."""
-    s3 = boto3.resource("s3")
-    s3object = s3.Object(bucket_name, path)
-    s3object.put(Body=(bytes(json.dumps(json_data).encode("UTF-8"))))
+# def write_json(bucket_name: str, path: str, json_data: dict):
+#     """Writes json dict to bucket/path."""
+#     s3 = boto3.resource("s3")
+#     s3object = s3.Object(bucket_name, path)
+#     s3object.put(Body=(bytes(json.dumps(json_data).encode("UTF-8"))))
 
 
 def main():
     """Capsule Entrypoint."""
     parser = argschema.ArgSchemaParser(schema_type=ConversionSchema)
     args = dict(parser.args)
```

### Comparing `aind_dispim_processing-0.0.1/src/aind_dispim_processing/logging_capsule.py` & `aind_dispim_processing-0.0.2/src/aind_dispim_processing/logging_capsule.py`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/src/aind_dispim_processing/registration_capsule.py` & `aind_dispim_processing-0.0.2/src/aind_dispim_processing/registration_capsule.py`

 * *Files identical despite different names*

### Comparing `aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/PKG-INFO` & `aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-dispim-processing
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for Dispim Code Ocean Pipeline
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_dispim_processing-0.0.1/src/aind_dispim_processing.egg-info/SOURCES.txt` & `aind_dispim_processing-0.0.2/src/aind_dispim_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

