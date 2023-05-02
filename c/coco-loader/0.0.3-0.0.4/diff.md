# Comparing `tmp/coco_loader-0.0.3.tar.gz` & `tmp/coco_loader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coco_loader-0.0.3.tar", max compression
+gzip compressed data, was "coco_loader-0.0.4.tar", max compression
```

## Comparing `coco_loader-0.0.3.tar` & `coco_loader-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-04-17 05:29:43.361653 coco_loader-0.0.3/LICENSE
--rw-r--r--   0        0        0     2406 2023-04-17 05:30:05.766619 coco_loader-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-04-06 01:21:23.643490 coco_loader-0.0.3/coco_loader/__init__.py
--rw-r--r--   0        0        0      638 2023-04-17 05:28:44.651914 coco_loader-0.0.3/coco_loader/bases.py
--rw-r--r--   0        0        0     1149 2023-04-17 05:44:03.178835 coco_loader-0.0.3/coco_loader/common.py
--rw-r--r--   0        0        0      391 2023-04-17 05:28:24.536399 coco_loader-0.0.3/coco_loader/imagecaptioning.py
--rw-r--r--   0        0        0      698 2023-04-17 05:28:24.536419 coco_loader-0.0.3/coco_loader/keypointdetection.py
--rw-r--r--   0        0        0      691 2023-04-17 05:28:24.536453 coco_loader-0.0.3/coco_loader/objectdetection.py
--rw-r--r--   0        0        0      832 2023-04-17 05:28:24.516831 coco_loader-0.0.3/coco_loader/panopticsegmentation.py
--rw-r--r--   0        0        0      627 2023-04-17 05:49:36.771323 coco_loader-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 coco_loader-0.0.3/setup.py
--rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 coco_loader-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 05:29:43.361653 coco_loader-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2406 2023-04-17 05:30:05.766619 coco_loader-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 01:21:23.643490 coco_loader-0.0.4/coco_loader/__init__.py
+-rw-r--r--   0        0        0      638 2023-04-17 05:28:44.651914 coco_loader-0.0.4/coco_loader/bases.py
+-rw-r--r--   0        0        0     1199 2023-05-02 01:14:33.860769 coco_loader-0.0.4/coco_loader/common.py
+-rw-r--r--   0        0        0      391 2023-04-17 05:28:24.536399 coco_loader-0.0.4/coco_loader/imagecaptioning.py
+-rw-r--r--   0        0        0      698 2023-04-18 02:02:02.060322 coco_loader-0.0.4/coco_loader/keypointdetection.py
+-rw-r--r--   0        0        0      691 2023-04-17 05:28:24.536453 coco_loader-0.0.4/coco_loader/objectdetection.py
+-rw-r--r--   0        0        0      832 2023-04-17 05:28:24.516831 coco_loader-0.0.4/coco_loader/panopticsegmentation.py
+-rw-r--r--   0        0        0      701 2023-05-02 01:18:05.524954 coco_loader-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 coco_loader-0.0.4/setup.py
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 coco_loader-0.0.4/PKG-INFO
```

### Comparing `coco_loader-0.0.3/LICENSE` & `coco_loader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.3/README.md` & `coco_loader-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.3/coco_loader/bases.py` & `coco_loader-0.0.4/coco_loader/bases.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.3/coco_loader/common.py` & `coco_loader-0.0.4/coco_loader/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,38 +12,42 @@
     year: int
     version: str
     description: str
     contributor: str
     url: str
     date_created: datetime = field(
         metadata=config(
-            encoder=lambda d: d.strftime('%Y/%m/%d'),
-            decoder=lambda s: datetime.strptime(s, '%Y/%m/%d'),
-            mm_field=fields.DateTime(format='%Y/%m/%d')
+            encoder=lambda d: d.strftime("%Y/%m/%d"),
+            decoder=lambda s: datetime.strptime(s, "%Y/%m/%d"),
+            mm_field=fields.DateTime(format="%Y/%m/%d"),
         )
     )
 
 
 @dataclass_json
 @dataclass
 class Image:
     id: int
     width: int
     height: int
     file_name: str
     license: int
     coco_url: str
-    flickr_url: Optional[str] = None
     date_captured: Optional[datetime] = field(
         metadata=config(
-            encoder=lambda d: d.strftime('%Y-%m-%d %H:%M:%S') if d is not None else None,
-            decoder=lambda s: datetime.strptime(s, '%Y-%m-%d %H:%M:%S') if s is not None else None,
-            mm_field=fields.DateTime(format='iso')
+            encoder=lambda d: d.strftime("%Y-%m-%d %H:%M:%S")
+            if d is not None
+            else None,
+            decoder=lambda s: datetime.strptime(s, "%Y-%m-%d %H:%M:%S")
+            if s is not None
+            else None,
+            mm_field=fields.DateTime(format="iso"),
         )
     )
+    flickr_url: Optional[str] = None
 
 
 @dataclass_json
 @dataclass
 class License:
     id: int
     name: str
```

### Comparing `coco_loader-0.0.3/coco_loader/keypointdetection.py` & `coco_loader-0.0.4/coco_loader/keypointdetection.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.3/coco_loader/objectdetection.py` & `coco_loader-0.0.4/coco_loader/objectdetection.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.3/coco_loader/panopticsegmentation.py` & `coco_loader-0.0.4/coco_loader/panopticsegmentation.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.3/pyproject.toml` & `coco_loader-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 [tool.poetry]
 name = "coco-loader"
-version = "0.0.3"
+version = "0.0.4"
 description = "COCO dataset loader."
 license = "MIT"
 authors = ["Jinhyuck Cha <jhcha@superb-ai.com>"]
 maintainers = ["Jinhyuck Cha <jhcha@superb-ai.com>"]
 readme = "README.md"
 homepage = "https://github.com/jinhyuckcha/coco-loader"
 repository = "https://github.com/jinhyuckcha/coco-loader"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 dataclasses-json = "^0.5.4"
 
-[tool.poetry.dev-dependencies]
-
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/jinhyuckcha/coco-loader/issues"
 
+[tool.poetry.group.dev.dependencies]
+jupyter = "^1.0.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+pythonpath = [
+  "."
+]
```

### Comparing `coco_loader-0.0.3/setup.py` & `coco_loader-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['dataclasses-json>=0.5.4,<0.6.0']
 
 setup_kwargs = {
     'name': 'coco-loader',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'COCO dataset loader.',
     'long_description': "# coco-loader\n\nCOCO dataset loader.\nProvides serializable native Python bindings for several COCO dataset formats.\n\nSupported bindings and their corresponding modules:\n\n- Object Detection: `objectdetection`\n- Keypoint Detection: `keypointdetection`\n- Panoptic Segmentation: `panopticsegmentation`\n- Image Captioning: `imagecaptioning`\n\n## Installation\n\n`coco-loader` is available on PyPI:\n\n```bash\npip install coco-loader\n```\n\n## Usage\n\n### Creating a dataset (Object Detection)\n\n```python\n>>> from coco_loader.common import Info, Image, License\n>>> from coco_loader.objectdetection import ObjectDetectionAnnotation, \\\n...                                      ObjectDetectionCategory, \\\n...                                      ObjectDetectionDataset\n>>> from datetime import datetime\n>>> info = Info(  # Describe the dataset\n...    year=datetime.now().year,\n...    version='1.0',\n...    description='This is a test dataset',\n...    contributor='Test',\n...    url='https://test',\n...    date_created=datetime.now()\n... )\n>>> mit_license = License(  # Set the license\n...     id=0,\n...     name='MIT',\n...     url='https://opensource.org/licenses/MIT'\n... )\n>>> images = [  # Describe the images\n...     Image(\n...         id=0,\n...         width=640, height=480,\n...         file_name='test.jpg',\n...         license=mit_license.id,\n...         flickr_url='',\n...         coco_url='',\n...         date_captured=datetime.now()\n...     ),\n...     ...\n... ]\n>>> categories = [  # Describe the categories\n...     ObjectDetectionCategory(\n...         id=0,\n...         name='pedestrian',\n...         supercategory=''\n...     ),\n...     ...\n... ]\n>>> annotations = [  # Describe the annotations\n...     ObjectDetectionAnnotation(\n...         id=0,\n...         image_id=0,\n...         category_id=0,\n...         segmentation=[],\n...         area=800.0,\n...         bbox=[300.0, 100.0, 20.0, 40.0],\n...         is_crowd=0\n...     ),\n...     ...\n... ]\n>>> dataset = ObjectDetectionDataset(  # Create the dataset\n...     info=info,\n...     images=images,\n...     licenses=[mit_license],\n...     categories=categories,\n...     annotations=annotations\n... )\n>>> dataset.save('test_dataset.json', indent=2)  # Save the dataset\n```\n\n### Loading a dataset\n\n```python\n>>> from coco_loader.objectdetection import ObjectDetectionDataset\n>>> dataset = ObjectDetectionDataset.load('test_dataset.json')  # Load the dataset\n```\n",
     'author': 'Jinhyuck Cha',
     'author_email': 'jhcha@superb-ai.com',
     'maintainer': 'Jinhyuck Cha',
     'maintainer_email': 'jhcha@superb-ai.com',
     'url': 'https://github.com/jinhyuckcha/coco-loader',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `coco_loader-0.0.3/PKG-INFO` & `coco_loader-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: coco-loader
-Version: 0.0.3
+Version: 0.0.4
 Summary: COCO dataset loader.
 Home-page: https://github.com/jinhyuckcha/coco-loader
 License: MIT
 Author: Jinhyuck Cha
 Author-email: jhcha@superb-ai.com
 Maintainer: Jinhyuck Cha
 Maintainer-email: jhcha@superb-ai.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.4,<0.6.0)
 Project-URL: Bug Tracker, https://github.com/jinhyuckcha/coco-loader/issues
```

