# Comparing `tmp/pixano-0.1.0.tar.gz` & `tmp/pixano-0.1.1.tar.gz`

## Comparing `pixano-0.1.0.tar` & `pixano-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/__version__.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/analytics/__init__.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/analytics/feature_statistics.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/README.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/__init__.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/db_utils.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/main.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/serve.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/dist/index.html
--rw-r--r--   0        0        0  1079144 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/dist/assets/index-275a5f8e.js
--rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/dist/assets/index-ab1a97a8.css
--rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/apps/explorer/dist/assets/pixano-354ac9df.png
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/__init__.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/dataset.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/dataset_test.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/models.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/arrow_types/__init__.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/arrow_types/features.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/arrow_types/image.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/core/arrow_types/image_test.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/data/__init__.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/data/coco_loader.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/data/data_loader.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/data/models.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/data/pixano_loader.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/inference/__init__.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/inference/inference_model.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/tools/converter/__init__.py
--rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/tools/converter/convert2parquet.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/transforms/__init__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/transforms/boxes.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/transforms/image.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 pixano-0.1.0/pixano/transforms/labels.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pixano-0.1.0/.gitignore
--rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 pixano-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pixano-0.1.0/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pixano-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pixano-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/__version__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/analytics/__init__.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/analytics/feature_statistics.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/README.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/__init__.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/db_utils.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/main.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/serve.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/dist/index.html
+-rw-r--r--   0        0        0  1079144 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/dist/assets/index-275a5f8e.js
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/dist/assets/index-ab1a97a8.css
+-rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/apps/explorer/dist/assets/pixano-354ac9df.png
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/__init__.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/dataset.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/dataset_test.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/models.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/arrow_types/__init__.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/arrow_types/features.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/arrow_types/image.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/core/arrow_types/image_test.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/data/__init__.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/data/coco_loader.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/data/data_loader.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/data/models.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/data/pixano_loader.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/inference/__init__.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/inference/inference_model.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/tools/converter/__init__.py
+-rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/tools/converter/convert2parquet.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/transforms/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/transforms/boxes.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/transforms/image.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 pixano-0.1.1/pixano/transforms/labels.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pixano-0.1.1/.gitignore
+-rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 pixano-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pixano-0.1.1/README.md
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pixano-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pixano-0.1.1/PKG-INFO
```

### Comparing `pixano-0.1.0/pixano/__init__.py` & `pixano-0.1.1/pixano/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/__version__.py` & `pixano-0.1.1/pixano/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # This software is governed by the CeCILL-C license under French law and
 # abiding by the rules of distribution of free software. You can use,
 # modify and/ or redistribute the software under the terms of the CeCILL-C
 # license as circulated by CEA, CNRS and INRIA at the following URL
 #
 # http://www.cecill.info
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `pixano-0.1.0/pixano/analytics/__init__.py` & `pixano-0.1.1/pixano/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/analytics/feature_statistics.py` & `pixano-0.1.1/pixano/analytics/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/__init__.py` & `pixano-0.1.1/pixano/apps/explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/db_utils.py` & `pixano-0.1.1/pixano/apps/explorer/db_utils.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/main.py` & `pixano-0.1.1/pixano/apps/explorer/main.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/serve.py` & `pixano-0.1.1/pixano/apps/explorer/serve.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/dist/index.html` & `pixano-0.1.1/pixano/apps/explorer/dist/index.html`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/dist/assets/index-275a5f8e.js` & `pixano-0.1.1/pixano/apps/explorer/dist/assets/index-275a5f8e.js`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/dist/assets/index-ab1a97a8.css` & `pixano-0.1.1/pixano/apps/explorer/dist/assets/index-ab1a97a8.css`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/apps/explorer/dist/assets/pixano-354ac9df.png` & `pixano-0.1.1/pixano/apps/explorer/dist/assets/pixano-354ac9df.png`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/__init__.py` & `pixano-0.1.1/pixano/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/dataset.py` & `pixano-0.1.1/pixano/core/dataset.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/dataset_test.py` & `pixano-0.1.1/pixano/core/dataset_test.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/models.py` & `pixano-0.1.1/pixano/core/models.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/arrow_types/__init__.py` & `pixano-0.1.1/pixano/core/arrow_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/arrow_types/features.py` & `pixano-0.1.1/pixano/core/arrow_types/features.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/arrow_types/image.py` & `pixano-0.1.1/pixano/core/arrow_types/image.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/core/arrow_types/image_test.py` & `pixano-0.1.1/pixano/core/arrow_types/image_test.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/data/__init__.py` & `pixano-0.1.1/pixano/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/data/coco_loader.py` & `pixano-0.1.1/pixano/data/coco_loader.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/data/data_loader.py` & `pixano-0.1.1/pixano/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/data/models.py` & `pixano-0.1.1/pixano/data/models.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/data/pixano_loader.py` & `pixano-0.1.1/pixano/data/pixano_loader.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/inference/__init__.py` & `pixano-0.1.1/pixano/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/inference/inference_model.py` & `pixano-0.1.1/pixano/inference/inference_model.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/tools/converter/__init__.py` & `pixano-0.1.1/pixano/tools/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/tools/converter/convert2parquet.py` & `pixano-0.1.1/pixano/tools/converter/convert2parquet.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/transforms/__init__.py` & `pixano-0.1.1/pixano/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/transforms/boxes.py` & `pixano-0.1.1/pixano/transforms/boxes.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/transforms/image.py` & `pixano-0.1.1/pixano/transforms/image.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pixano/transforms/labels.py` & `pixano-0.1.1/pixano/transforms/labels.py`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/LICENSE.txt` & `pixano-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pixano-0.1.0/pyproject.toml` & `pixano-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -3,64 +3,68 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pixano"
 dynamic = ["version"]
 description = 'Data-centric AI building blocks for computer vision applications' 
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = "CeCILL-C"
-authors = [
-  { name = "Pixano Developpers", email = "pixano@cea.fr" },
+authors = [{name = "Pixano Developers", email = "pixano@cea.fr"}]
+keywords = [
+  "machine learning",
+  "computer vision",
+  "data",
+  "visualization"
 ]
-
-keywords = ["machine learning", "computer vision", "data", "visualization"]
-
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.8", 
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-
 dependencies = [
-  "duckdb",
-  "etils",
-  "fastapi",
-  "fastapi-pagination",
-  "imageio",
-  "importlib-resources",
-  "jinja2",
-  "numpy",
-  "opencv-python",
-  "pandas",
-  "Pillow",
-  "pyarrow",
-  "pycocotools",
-  "tqdm"
+  "duckdb ~= 0.7.0",
+  "etils ~= 1.1.0",
+  "fastapi-pagination ~= 0.11.4",
+  "imageio ~= 2.25.0",
+  "importlib-resources ~= 5.12.0",
+  "numpy ~= 1.23.0",
+  "opencv-python ~= 4.7.0",
+  "pandas ~= 1.5.0",
+  "Pillow ~= 9.4.0",
+  "pyarrow ~= 11.0.0",
+  "pycocotools ~= 2.0.0",
+  "setuptools ~= 65.6.0",
+  "shortuuid ~= 1.0.0",
+  "tqdm ~= 4.64.0",
+  "uvicorn ~= 0.20.0"
+]
+
+[project.optional-dependencies]
+documentation = [
+  "mkdocs-material ~= 9.1.0",
+  "mkdocstrings-python ~= 0.9.0"
+]
+notebooks = [
+  "ipywidgets ~= 8.0.0"
 ]
 
 [project.urls]
 Documentation = "https://github.com/pixano/pixano#readme"
 Issues = "https://github.com/pixano/pixano/issues"
 Source = "https://github.com/pixano/pixano"
 
 [project.scripts]
 pixano-explorer = "pixano.apps.explorer.serve:main"
 
 [tool.hatch.build]
-include = [
-  "/pixano"
-]
-
-exclude = [
-  "__pycache__"
-]
-
-artifacts = [
-  "/pixano/apps/explorer/dist"
-]
+include = ["/pixano"]
+exclude = ["__pycache__"]
+artifacts = ["/pixano/apps/explorer/dist"]
 
 [tool.hatch.version]
 path = "pixano/__version__.py"
```

