# Comparing `tmp/clarifai-9.3.4.tar.gz` & `tmp/clarifai-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.3.4.tar", last modified: Mon May  1 19:52:09 2023, max compression
+gzip compressed data, was "clarifai-9.4.0.tar", last modified: Tue May  2 21:26:34 2023, max compression
```

## Comparing `clarifai-9.3.4.tar` & `clarifai-9.4.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.750245 clarifai-9.3.4/
--rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.3.4/LICENSE
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.3.4/MANIFEST.in
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-05-01 19:52:09.750052 clarifai-9.3.4/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.3.4/README.md
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.732977 clarifai-9.3.4/clarifai/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.733959 clarifai-9.3.4/clarifai/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.734495 clarifai-9.3.4/clarifai/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.735123 clarifai-9.3.4/clarifai/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.738812 clarifai-9.3.4/clarifai/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.739722 clarifai-9.3.4/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.3.4/clarifai/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.3.4/clarifai/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.730231 clarifai-9.3.4/clarifai/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.739865 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.740229 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.740538 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.740702 clarifai-9.3.4/clarifai/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.740929 clarifai-9.3.4/clarifai/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.741204 clarifai-9.3.4/clarifai/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.742823 clarifai-9.3.4/clarifai/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.3.4/clarifai/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.743366 clarifai-9.3.4/clarifai/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.743598 clarifai-9.3.4/clarifai/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.4/clarifai/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.4/clarifai/urls/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.733698 clarifai-9.3.4/clarifai.egg-info/
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-05-01 19:52:09.000000 clarifai-9.3.4/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     4063 2023-05-01 19:52:09.000000 clarifai-9.3.4/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-05-01 19:52:09.000000 clarifai-9.3.4/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-05-01 19:52:09.000000 clarifai-9.3.4/clarifai.egg-info/requires.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-05-01 19:52:09.000000 clarifai-9.3.4/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.743842 clarifai-9.3.4/clarifai_utils/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.744068 clarifai-9.3.4/clarifai_utils/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.744455 clarifai-9.3.4/clarifai_utils/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.744829 clarifai-9.3.4/clarifai_utils/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.745480 clarifai-9.3.4/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.746302 clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.731512 clarifai-9.3.4/clarifai_utils/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.746439 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.746674 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.746924 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.747061 clarifai-9.3.4/clarifai_utils/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.747296 clarifai-9.3.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.747438 clarifai-9.3.4/clarifai_utils/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai_utils/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.748777 clarifai-9.3.4/clarifai_utils/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.3.4/clarifai_utils/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.4/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.749482 clarifai-9.3.4/clarifai_utils/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.4/clarifai_utils/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.4/clarifai_utils/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-01 19:52:09.749795 clarifai-9.3.4/clarifai_utils/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.4/clarifai_utils/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.4/clarifai_utils/urls/helper.py
--rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-05-01 19:52:09.750295 clarifai-9.3.4/setup.cfg
--rw-r--r--   0 zeiler     (503) staff       (20)      897 2023-05-01 19:51:47.000000 clarifai-9.3.4/setup.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.981151 clarifai-9.4.0/
+-rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.4.0/LICENSE
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.4.0/MANIFEST.in
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-05-02 21:26:34.980944 clarifai-9.4.0/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.4.0/README.md
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.961242 clarifai-9.4.0/clarifai/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.962119 clarifai-9.4.0/clarifai/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.962852 clarifai-9.4.0/clarifai/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.963352 clarifai-9.4.0/clarifai/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/data_upload/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.964347 clarifai-9.4.0/clarifai/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965206 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.954199 clarifai-9.4.0/clarifai/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965339 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965571 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965841 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.966006 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.966230 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.966497 clarifai-9.4.0/clarifai/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.968089 clarifai-9.4.0/clarifai/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.968659 clarifai-9.4.0/clarifai/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.968990 clarifai-9.4.0/clarifai/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.4.0/clarifai/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.4.0/clarifai/urls/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.961885 clarifai-9.4.0/clarifai.egg-info/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     4063 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/requires.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.969242 clarifai-9.4.0/clarifai_utils/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.969467 clarifai-9.4.0/clarifai_utils/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.969861 clarifai-9.4.0/clarifai_utils/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.970231 clarifai-9.4.0/clarifai_utils/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/data_upload/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.970875 clarifai-9.4.0/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.971671 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.955764 clarifai-9.4.0/clarifai_utils/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.971806 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972043 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972310 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972445 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972683 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.978487 clarifai-9.4.0/clarifai_utils/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.979930 clarifai-9.4.0/clarifai_utils/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai_utils/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.980455 clarifai-9.4.0/clarifai_utils/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.980715 clarifai-9.4.0/clarifai_utils/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.4.0/clarifai_utils/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.4.0/clarifai_utils/urls/helper.py
+-rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-05-02 21:26:34.981203 clarifai-9.4.0/setup.cfg
+-rw-r--r--   0 zeiler     (503) staff       (20)      897 2023-05-02 21:25:56.000000 clarifai-9.4.0/setup.py
```

### Comparing `clarifai-9.3.4/LICENSE` & `clarifai-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/PKG-INFO` & `clarifai-9.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.4
+Version: 9.4.0
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.4/README.md` & `clarifai-9.4.0/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/auth/helper.py` & `clarifai-9.4.0/clarifai/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/client/abc.py` & `clarifai-9.4.0/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/client/stub.py` & `clarifai-9.4.0/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/base.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/features.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/image.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/text.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/examples.py` & `clarifai-9.4.0/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/data_upload/upload.py` & `clarifai-9.4.0/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/dataset_export/dataset_export_inputs.py` & `clarifai-9.4.0/clarifai/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/concepts.py` & `clarifai-9.4.0/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/datasets.py` & `clarifai-9.4.0/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/inputs.py` & `clarifai-9.4.0/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/installed_module_versions.py` & `clarifai-9.4.0/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/lister.py` & `clarifai-9.4.0/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/models.py` & `clarifai-9.4.0/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/module_versions.py` & `clarifai-9.4.0/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/listing/modules.py` & `clarifai-9.4.0/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/modules/css.py` & `clarifai-9.4.0/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/modules/pages.py` & `clarifai-9.4.0/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/modules/style.css` & `clarifai-9.4.0/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai/urls/helper.py` & `clarifai-9.4.0/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai.egg-info/PKG-INFO` & `clarifai-9.4.0/clarifai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.4
+Version: 9.4.0
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.4/clarifai.egg-info/SOURCES.txt` & `clarifai-9.4.0/clarifai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/auth/helper.py` & `clarifai-9.4.0/clarifai_utils/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/client/abc.py` & `clarifai-9.4.0/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/client/stub.py` & `clarifai-9.4.0/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/examples.py` & `clarifai-9.4.0/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/data_upload/upload.py` & `clarifai-9.4.0/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/dataset_export/dataset_export_inputs.py` & `clarifai-9.4.0/clarifai_utils/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/concepts.py` & `clarifai-9.4.0/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/datasets.py` & `clarifai-9.4.0/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/inputs.py` & `clarifai-9.4.0/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.4.0/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/lister.py` & `clarifai-9.4.0/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/models.py` & `clarifai-9.4.0/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/module_versions.py` & `clarifai-9.4.0/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/listing/modules.py` & `clarifai-9.4.0/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/modules/css.py` & `clarifai-9.4.0/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/modules/pages.py` & `clarifai-9.4.0/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/modules/style.css` & `clarifai-9.4.0/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/clarifai_utils/urls/helper.py` & `clarifai-9.4.0/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.4/setup.py` & `clarifai-9.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.3.4",
+    version="9.4.0",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
@@ -20,10 +20,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     license="Apache 2.0",
     python_requires='>=3.8',
     install_requires=[
-        "clarifai-grpc>=9.3.0",
+        "clarifai-grpc>=9.4.0",
     ],
     include_package_data=True)
```

