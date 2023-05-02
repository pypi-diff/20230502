# Comparing `tmp/deeplake-3.3.2.tar.gz` & `tmp/deeplake-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.3.2.tar", last modified: Thu Apr 27 11:46:23 2023, max compression
+gzip compressed data, was "deeplake-3.4.0.tar", last modified: Tue May  2 17:49:27 2023, max compression
```

## Comparing `deeplake-3.3.2.tar` & `deeplake-3.4.0.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.294758 deeplake-3.3.2/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-04-27 11:39:34.000000 deeplake-3.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 11:39:34.000000 deeplake-3.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22282 2023-04-27 11:46:23.294758 deeplake-3.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21602 2023-04-27 11:39:34.000000 deeplake-3.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88813 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    79221 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23071 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7389 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7081 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12918 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5926 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17970 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     5936 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   108710 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   166287 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14750 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4242 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    18879 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    11242 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15953 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13294 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      441 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    18475 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    24900 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    48988 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7404 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    10122 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47159 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    28835 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5373 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     5774 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19402 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5745 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    28992 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4349 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    24153 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22695 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7073 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     5010 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.284758 deeplake-3.3.2/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.294758 deeplake-3.3.2/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.294758 deeplake-3.3.2/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    15328 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.294758 deeplake-3.3.2/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-27 11:42:32.000000 deeplake-3.3.2/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34379 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37298 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.294758 deeplake-3.3.2/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     6762 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.294758 deeplake-3.3.2/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    23774 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31017 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.294758 deeplake-3.3.2/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-04-27 11:39:34.000000 deeplake-3.3.2/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:46:23.274758 deeplake-3.3.2/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22282 2023-04-27 11:46:23.000000 deeplake-3.3.2/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10849 2023-04-27 11:46:23.000000 deeplake-3.3.2/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:46:23.000000 deeplake-3.3.2/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-27 11:46:23.000000 deeplake-3.3.2/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:46:23.000000 deeplake-3.3.2/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-27 11:46:23.000000 deeplake-3.3.2/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-27 11:46:23.000000 deeplake-3.3.2/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-27 11:46:23.294758 deeplake-3.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3289 2023-04-27 11:39:34.000000 deeplake-3.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-05-02 17:42:56.000000 deeplake-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-02 17:42:56.000000 deeplake-3.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25285 2023-05-02 17:49:27.270891 deeplake-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24578 2023-05-02 17:42:56.000000 deeplake-3.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.240891 deeplake-3.4.0/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94028 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    79381 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23071 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19220 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     6039 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   109338 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   167215 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14805 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11242 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13294 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25667 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49363 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7404 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    10116 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48095 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    28968 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6781 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4349 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25806 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22441 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     4986 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     5010 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.260891 deeplake-3.4.0/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    15328 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-02 17:46:40.000000 deeplake-3.4.0/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4477 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34379 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    23730 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31017 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.270891 deeplake-3.4.0/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-05-02 17:42:56.000000 deeplake-3.4.0/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:49:27.250891 deeplake-3.4.0/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25285 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10849 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-02 17:49:27.000000 deeplake-3.4.0/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-02 17:49:27.270891 deeplake-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-02 17:42:56.000000 deeplake-3.4.0/setup.py
```

### Comparing `deeplake-3.3.2/LICENSE` & `deeplake-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/PKG-INFO` & `deeplake-3.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.3.2
+Version: 3.4.0
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: audio
 Provides-Extra: av
 Provides-Extra: dicom
+Provides-Extra: enterprise
 Provides-Extra: gcp
 Provides-Extra: gdrive
 Provides-Extra: medical
 Provides-Extra: point_cloud
 Provides-Extra: video
 Provides-Extra: visualizer
 License-File: LICENSE
 
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
      <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
 </h1>
     </br>
-    <h1 align="center">Deep Lake: Data Lake for Deep Learning
+    <h1 align="center">Deep Lake: Vector Database for any AI data
  </h1>
 <p align="center">
     <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
     <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
     <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
      <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
      </a>
@@ -51,15 +52,17 @@
  </h3>
  
 
 *Read this in other languages: [简体中文](README.zh-cn.md)*
 
 ## About Deep Lake
 
-Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake includes the following features:
+Deep Lake is a Vector Database powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights and Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Google, Intel, Waymo, Matterport, Red Cross, Yale, & Oxford. 
+
+Deep Lake includes the following features:
 
 <details>
   <summary><b>Storage Agnostic API</b></summary>
 Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
 </details>
 <details>
   <summary><b>Native Compression with Lazy NumPy-like Indexing</b></summary>
@@ -70,16 +73,16 @@
 Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
 </details>
 <details>
   <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
 Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
 </details>
 <details>
-  <summary><b>Integrations with Popular Tools</b></summary>
-Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
+  <summary><b>Integrations with Powerful Tools</b></summary>
+Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> and <a href="https://github.com/jerryjliu/llama_index">LLamaIndex</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
 </details>
 <details>
   <summary><b>Distributed Transformations</b></summary>
 Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
 <details>
   <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
 Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
@@ -300,14 +303,36 @@
 | Storage for public datasets hosted by Activeloop     | 200GB Free    |
 | Storage for private datasets hosted by Activeloop    | 100GB Free    |
 
 
 
 ## 👩‍💻 Comparisons to Familiar Tools
 
+<details>
+  <summary><b>Deep Lake vs Chroma </b></summary>
+  
+Both Deep Lake & ChromaDB enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are architecturally very different. ChromaDB is a Vector Database that can be deployed locally or on a server using Docker and will offer a hosted solution shortly. Deep Lake is a serverless Vector Store deployed on the user’s own cloud, locally, or in-memory. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike ChromaDB, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. ChromaDB is limited to light metadata on top of the embeddings and has no visualization. Deep Lake datasets can be visualized and version controlled. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
+
+<details>
+  <summary><b>Deep Lake vs Pinecone</b></summary>
+  
+Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring serach for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
+<details>
+  <summary><b>Deep Lake vs Weaviate</b></summary>
+  
+Both Deep Lake and Weaviate enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Weaviate is a Vector Database that can be deployed in a managed service or by the user via Kubernetes or Docker. Deep Lake is serverless. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike Weaviate, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Weaviate is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
 
 <details>
   <summary><b>Deep Lake vs DVC</b></summary>
   
 Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
 
 </details>
```

#### html2text {}

```diff
@@ -1,53 +1,57 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.3.2 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.4.0 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
-Provides-Extra: gcp Provides-Extra: gdrive Provides-Extra: medical Provides-
-Extra: point_cloud Provides-Extra: video Provides-Extra: visualizer License-
-File: LICENSE [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-
-f711c4d35b82]
+Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
+Extra: medical Provides-Extra: point_cloud Provides-Extra: video Provides-
+Extra: visualizer License-File: LICENSE [https://static.scarf.sh/a.png?x-
+pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
-             ****** Deep Lake: Data Lake for Deep Learning ******
+           ****** Deep Lake: Vector Database for any AI data ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
-Lake Deep Lake (formerly known as Activeloop Hub) is a data lake for deep
-learning applications. Our open-source dataset format is optimized for rapid
-streaming and querying of data while training models at scale, and it includes
-a simple API for creating, storing, and collaborating on AI datasets of any
-size. It can be deployed locally or in the cloud, and it enables you to store
-all of your data in one place, ranging from simple annotations to large videos.
-Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep
-Lake includes the following features:  Storage Agnostic API Use one API to
-upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
-GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
-like Indexing Store images, audios and videos in their native compression.
-Slide, index, iterate and interact with your data like a collection of NumPy
-arrays in your system's memory. Deep Lake lazily loads data only when needed,
-e.g., when training a model.   Dataset Version Control Commits, branches,
-checkout - Concepts you are already familiar with in your code repositories can
-now be applied to your datasets as well!   Dataloaders for Popular Deep
-Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+Lake Deep Lake is a Vector Database powered by a unique storage format
+optimized for deep-learning and Large Language Model (LLM) based applications.
+It simplifies the deployment of enterprise-grade LLM-based products by offering
+storage for all data types (embeddings, audio, text, videos, images, pdfs,
+annotations, etc.), querying and vector search, data streaming while training
+models at scale, data versioning and lineage for all workloads, and
+integrations with popular tools such as LangChain, LlamaIndex, Weights and
+Biases, and many more. Deep Lake works with data of any size, it is serverless,
+and it enables you to store all of your data in once place. Deep Lake is used
+by Google, Intel, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake
+includes the following features:  Storage Agnostic API Use one API to upload,
+download, and stream datasets to/from AWS S3/S3-compatible storage, GCP,
+Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-like
+Indexing Store images, audios and videos in their native compression. Slide,
+index, iterate and interact with your data like a collection of NumPy arrays in
+your system's memory. Deep Lake lazily loads data only when needed, e.g., when
+training a model.   Dataset Version Control Commits, branches, checkout -
+Concepts you are already familiar with in your code repositories can now be
+applied to your datasets as well!   Dataloaders for Popular Deep Learning
+Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
 Tensorflow. Train your model with a few lines of code - we even take care of
-dataset shuffling. :)   Integrations with Popular Tools Deep Lake has
-integrations with Langchain as a vector store for LLM apps, Weights_&_Biases
-for data lineage during model training, and MMDetection for training object
-detection models.   Distributed Transformations Rapidly apply transformations
-on your datasets using multi-threading, multi-processing, or our built-in Ray
-integration.  100+ most-popular image, video, and audio datasets available in
-seconds Deep Lake community has uploaded 100+_image,_video_and_audio_datasets
-like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.    Instant Visualization
-Support in Activeloop_Platform Deep Lake datasets are instantly visualized with
-bounding boxes, masks, annotations, etc. in Deep_Lake_Visualizer (see below).
+dataset shuffling. :)   Integrations with Powerful Tools Deep Lake has
+integrations with Langchain and LLamaIndex as a vector store for LLM apps,
+Weights_&_Biases for data lineage during model training, and MMDetection for
+training object detection models.   Distributed Transformations Rapidly apply
+transformations on your datasets using multi-threading, multi-processing, or
+our built-in Ray integration.  100+ most-popular image, video, and audio
+datasets available in seconds Deep Lake community has uploaded 100+_image,
+video_and_audio_datasets like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.
+Instant Visualization Support in Activeloop_Platform Deep Lake datasets are
+instantly visualized with bounding boxes, masks, annotations, etc. in Deep_Lake
+Visualizer (see below).
                   [https://www.linkpicture.com/q/ReadMe.gif]
 ## ð Performance Deep Lake's efficient enterprise dataloaders built in C++
 speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022,
 Hambardzumyan et al. 2023)
                    [docs/source/_static/img/benchmarks.png]
 ## Getting Started with Deep Lake ### ð How to install Deep Lake Deep Lake's
 core is efficiently built in C++ and can be quickly installed using pip. ```sh
@@ -139,17 +143,50 @@
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
 Platform. Users can also create and store their own datasets and make them
 available to the public. Free storage of up to 300 GB is available for students
 and educators: |  |  | | ---------------------------------------------------- |
 ------------- | | Storage for public datasets hosted by Activeloop | 200GB Free
 | | Storage for private datasets hosted by Activeloop | 100GB Free | ##
-ð©âð» Comparisons to Familiar Tools  Deep Lake vs DVC Deep Lake and DVC
-offer dataset version control similar to git for data, but their methods for
-storing data differ significantly. Deep Lake converts and stores data as
+ð©âð» Comparisons to Familiar Tools  Deep Lake vs Chroma Both Deep Lake &
+ChromaDB enable users to store and search vectors (embeddings) and offer
+integrations with LangChain and LlamaIndex. However, they are architecturally
+very different. ChromaDB is a Vector Database that can be deployed locally or
+on a server using Docker and will offer a hosted solution shortly. Deep Lake is
+a serverless Vector Store deployed on the userâs own cloud, locally, or in-
+memory. All computations run client-side, which enables users to support
+lightweight production apps in seconds. Unlike ChromaDB, Deep Lakeâs data
+format can store raw data such as images, videos, and text, in addition to
+embeddings. ChromaDB is limited to light metadata on top of the embeddings and
+has no visualization. Deep Lake datasets can be visualized and version
+controlled. Deep Lake also has a performant dataloader for fine-tuning your
+Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
+enable users to store and search vectors (embeddings) and offer integrations
+with LangChain and LlamaIndex. However, they are architecturally very
+different. Pinecone is a fully-managed Vector Database that is optimized for
+highly demanding applications requiring serach for billions of vectors. Deep
+Lake is a serverless. All computations run client-side, which enables users to
+get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
+raw data such as images, videos, and text, in addition to embeddings. Deep Lake
+datasets can be visualized and version controlled. Pinecone is limited to light
+metadata on top of the embeddings and has no visualization. Deep Lake also has
+a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
+vs Weaviate Both Deep Lake and Weaviate enable users to store and search
+vectors (embeddings) and offer integrations with LangChain and LlamaIndex.
+However, they are architecturally very different. Weaviate is a Vector Database
+that can be deployed in a managed service or by the user via Kubernetes or
+Docker. Deep Lake is serverless. All computations run client-side, which
+enables users to support lightweight production apps in seconds. Unlike
+Weaviate, Deep Lakeâs data format can store raw data such as images, videos,
+and text, in addition to embeddings. Deep Lake datasets can be visualized and
+version controlled. Weaviate is limited to light metadata on top of the
+embeddings and has no visualization. Deep Lake also has a performant dataloader
+for fine-tuning your Large Language Models.   Deep Lake vs DVC Deep Lake and
+DVC offer dataset version control similar to git for data, but their methods
+for storing data differ significantly. Deep Lake converts and stores data as
 chunked compressed arrays, which enables rapid streaming to ML models, whereas
 DVC operates on top of data stored in less efficient traditional file
 structures. The Deep Lake format makes dataset versioning significantly easier
 compared to traditional file structures by DVC when datasets are composed of
 many files (i.e., many images). An additional distinction is that DVC primarily
 uses a command-line interface, whereas Deep Lake is a Python package. Lastly,
 Deep Lake offers an API to easily connect datasets to ML frameworks and other
```

### Comparing `deeplake-3.3.2/README.md` & `deeplake-3.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
      <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
 </h1>
     </br>
-    <h1 align="center">Deep Lake: Data Lake for Deep Learning
+    <h1 align="center">Deep Lake: Vector Database for any AI data
  </h1>
 <p align="center">
     <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
     <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
     <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
      <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
      </a>
@@ -26,15 +26,17 @@
  </h3>
  
 
 *Read this in other languages: [简体中文](README.zh-cn.md)*
 
 ## About Deep Lake
 
-Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake includes the following features:
+Deep Lake is a Vector Database powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights and Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Google, Intel, Waymo, Matterport, Red Cross, Yale, & Oxford. 
+
+Deep Lake includes the following features:
 
 <details>
   <summary><b>Storage Agnostic API</b></summary>
 Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
 </details>
 <details>
   <summary><b>Native Compression with Lazy NumPy-like Indexing</b></summary>
@@ -45,16 +47,16 @@
 Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
 </details>
 <details>
   <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
 Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
 </details>
 <details>
-  <summary><b>Integrations with Popular Tools</b></summary>
-Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
+  <summary><b>Integrations with Powerful Tools</b></summary>
+Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> and <a href="https://github.com/jerryjliu/llama_index">LLamaIndex</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
 </details>
 <details>
   <summary><b>Distributed Transformations</b></summary>
 Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
 <details>
   <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
 Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
@@ -275,14 +277,36 @@
 | Storage for public datasets hosted by Activeloop     | 200GB Free    |
 | Storage for private datasets hosted by Activeloop    | 100GB Free    |
 
 
 
 ## 👩‍💻 Comparisons to Familiar Tools
 
+<details>
+  <summary><b>Deep Lake vs Chroma </b></summary>
+  
+Both Deep Lake & ChromaDB enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are architecturally very different. ChromaDB is a Vector Database that can be deployed locally or on a server using Docker and will offer a hosted solution shortly. Deep Lake is a serverless Vector Store deployed on the user’s own cloud, locally, or in-memory. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike ChromaDB, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. ChromaDB is limited to light metadata on top of the embeddings and has no visualization. Deep Lake datasets can be visualized and version controlled. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
+
+<details>
+  <summary><b>Deep Lake vs Pinecone</b></summary>
+  
+Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring serach for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
+<details>
+  <summary><b>Deep Lake vs Weaviate</b></summary>
+  
+Both Deep Lake and Weaviate enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Weaviate is a Vector Database that can be deployed in a managed service or by the user via Kubernetes or Docker. Deep Lake is serverless. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike Weaviate, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Weaviate is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
 
 <details>
   <summary><b>Deep Lake vs DVC</b></summary>
   
 Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
 
 </details>
```

#### html2text {}

```diff
@@ -1,43 +1,47 @@
 [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
-             ****** Deep Lake: Data Lake for Deep Learning ******
+           ****** Deep Lake: Vector Database for any AI data ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
-Lake Deep Lake (formerly known as Activeloop Hub) is a data lake for deep
-learning applications. Our open-source dataset format is optimized for rapid
-streaming and querying of data while training models at scale, and it includes
-a simple API for creating, storing, and collaborating on AI datasets of any
-size. It can be deployed locally or in the cloud, and it enables you to store
-all of your data in one place, ranging from simple annotations to large videos.
-Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep
-Lake includes the following features:  Storage Agnostic API Use one API to
-upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
-GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
-like Indexing Store images, audios and videos in their native compression.
-Slide, index, iterate and interact with your data like a collection of NumPy
-arrays in your system's memory. Deep Lake lazily loads data only when needed,
-e.g., when training a model.   Dataset Version Control Commits, branches,
-checkout - Concepts you are already familiar with in your code repositories can
-now be applied to your datasets as well!   Dataloaders for Popular Deep
-Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+Lake Deep Lake is a Vector Database powered by a unique storage format
+optimized for deep-learning and Large Language Model (LLM) based applications.
+It simplifies the deployment of enterprise-grade LLM-based products by offering
+storage for all data types (embeddings, audio, text, videos, images, pdfs,
+annotations, etc.), querying and vector search, data streaming while training
+models at scale, data versioning and lineage for all workloads, and
+integrations with popular tools such as LangChain, LlamaIndex, Weights and
+Biases, and many more. Deep Lake works with data of any size, it is serverless,
+and it enables you to store all of your data in once place. Deep Lake is used
+by Google, Intel, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake
+includes the following features:  Storage Agnostic API Use one API to upload,
+download, and stream datasets to/from AWS S3/S3-compatible storage, GCP,
+Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-like
+Indexing Store images, audios and videos in their native compression. Slide,
+index, iterate and interact with your data like a collection of NumPy arrays in
+your system's memory. Deep Lake lazily loads data only when needed, e.g., when
+training a model.   Dataset Version Control Commits, branches, checkout -
+Concepts you are already familiar with in your code repositories can now be
+applied to your datasets as well!   Dataloaders for Popular Deep Learning
+Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
 Tensorflow. Train your model with a few lines of code - we even take care of
-dataset shuffling. :)   Integrations with Popular Tools Deep Lake has
-integrations with Langchain as a vector store for LLM apps, Weights_&_Biases
-for data lineage during model training, and MMDetection for training object
-detection models.   Distributed Transformations Rapidly apply transformations
-on your datasets using multi-threading, multi-processing, or our built-in Ray
-integration.  100+ most-popular image, video, and audio datasets available in
-seconds Deep Lake community has uploaded 100+_image,_video_and_audio_datasets
-like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.    Instant Visualization
-Support in Activeloop_Platform Deep Lake datasets are instantly visualized with
-bounding boxes, masks, annotations, etc. in Deep_Lake_Visualizer (see below).
+dataset shuffling. :)   Integrations with Powerful Tools Deep Lake has
+integrations with Langchain and LLamaIndex as a vector store for LLM apps,
+Weights_&_Biases for data lineage during model training, and MMDetection for
+training object detection models.   Distributed Transformations Rapidly apply
+transformations on your datasets using multi-threading, multi-processing, or
+our built-in Ray integration.  100+ most-popular image, video, and audio
+datasets available in seconds Deep Lake community has uploaded 100+_image,
+video_and_audio_datasets like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.
+Instant Visualization Support in Activeloop_Platform Deep Lake datasets are
+instantly visualized with bounding boxes, masks, annotations, etc. in Deep_Lake
+Visualizer (see below).
                   [https://www.linkpicture.com/q/ReadMe.gif]
 ## ð Performance Deep Lake's efficient enterprise dataloaders built in C++
 speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022,
 Hambardzumyan et al. 2023)
                    [docs/source/_static/img/benchmarks.png]
 ## Getting Started with Deep Lake ### ð How to install Deep Lake Deep Lake's
 core is efficiently built in C++ and can be quickly installed using pip. ```sh
@@ -129,17 +133,50 @@
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
 Platform. Users can also create and store their own datasets and make them
 available to the public. Free storage of up to 300 GB is available for students
 and educators: |  |  | | ---------------------------------------------------- |
 ------------- | | Storage for public datasets hosted by Activeloop | 200GB Free
 | | Storage for private datasets hosted by Activeloop | 100GB Free | ##
-ð©âð» Comparisons to Familiar Tools  Deep Lake vs DVC Deep Lake and DVC
-offer dataset version control similar to git for data, but their methods for
-storing data differ significantly. Deep Lake converts and stores data as
+ð©âð» Comparisons to Familiar Tools  Deep Lake vs Chroma Both Deep Lake &
+ChromaDB enable users to store and search vectors (embeddings) and offer
+integrations with LangChain and LlamaIndex. However, they are architecturally
+very different. ChromaDB is a Vector Database that can be deployed locally or
+on a server using Docker and will offer a hosted solution shortly. Deep Lake is
+a serverless Vector Store deployed on the userâs own cloud, locally, or in-
+memory. All computations run client-side, which enables users to support
+lightweight production apps in seconds. Unlike ChromaDB, Deep Lakeâs data
+format can store raw data such as images, videos, and text, in addition to
+embeddings. ChromaDB is limited to light metadata on top of the embeddings and
+has no visualization. Deep Lake datasets can be visualized and version
+controlled. Deep Lake also has a performant dataloader for fine-tuning your
+Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
+enable users to store and search vectors (embeddings) and offer integrations
+with LangChain and LlamaIndex. However, they are architecturally very
+different. Pinecone is a fully-managed Vector Database that is optimized for
+highly demanding applications requiring serach for billions of vectors. Deep
+Lake is a serverless. All computations run client-side, which enables users to
+get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
+raw data such as images, videos, and text, in addition to embeddings. Deep Lake
+datasets can be visualized and version controlled. Pinecone is limited to light
+metadata on top of the embeddings and has no visualization. Deep Lake also has
+a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
+vs Weaviate Both Deep Lake and Weaviate enable users to store and search
+vectors (embeddings) and offer integrations with LangChain and LlamaIndex.
+However, they are architecturally very different. Weaviate is a Vector Database
+that can be deployed in a managed service or by the user via Kubernetes or
+Docker. Deep Lake is serverless. All computations run client-side, which
+enables users to support lightweight production apps in seconds. Unlike
+Weaviate, Deep Lakeâs data format can store raw data such as images, videos,
+and text, in addition to embeddings. Deep Lake datasets can be visualized and
+version controlled. Weaviate is limited to light metadata on top of the
+embeddings and has no visualization. Deep Lake also has a performant dataloader
+for fine-tuning your Large Language Models.   Deep Lake vs DVC Deep Lake and
+DVC offer dataset version control similar to git for data, but their methods
+for storing data differ significantly. Deep Lake converts and stores data as
 chunked compressed arrays, which enables rapid streaming to ML models, whereas
 DVC operates on top of data stored in less efficient traditional file
 structures. The Deep Lake format makes dataset versioning significantly easier
 compared to traditional file structures by DVC when datasets are composed of
 many files (i.e., many images). An additional distinction is that DVC primarily
 uses a command-line interface, whereas Deep Lake is a Python package. Lastly,
 Deep Lake offers an API to easily connect datasets to ML frameworks and other
```

### Comparing `deeplake-3.3.2/deeplake/__init__.py` & `deeplake-3.4.0/deeplake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.3.2"
+__version__ = "3.4.0"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.3.2/deeplake/api/dataset.py` & `deeplake-3.4.0/deeplake/api/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
 
 class dataset:
     @staticmethod
     @spinner
     def init(
         path: Union[str, pathlib.Path],
+        runtime: Optional[Dict] = None,
         read_only: Optional[bool] = None,
         overwrite: bool = False,
         public: bool = False,
         memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE,
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
         creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
@@ -113,23 +114,25 @@
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
                 - Loading to a specific version:
 
                     - You can also specify a ``commit_id`` or ``branch`` to load the dataset to that version directly by using the ``@`` symbol.
                     - The path will then be of the form ``hub://username/dataset@{branch}`` or ``hub://username/dataset@{commit_id}``.
                     - See examples above.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             read_only (bool, optional): Opens dataset in read only mode if this is passed as ``True``. Defaults to ``False``.
                 Datasets stored on Deep Lake cloud that your account does not have write access to will automatically open in read mode.
             overwrite (bool): If set to ``True`` this overwrites the dataset if it already exists. Defaults to ``False``.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``True``.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
-            creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             verbose (bool): If ``True``, logs will be printed. Defaults to ``True``.
             access_method (str): The access method to use for the dataset. Can be:
 
                     - 'stream'
 
@@ -186,17 +189,20 @@
 
         path, address = process_dataset_path(path)
         verify_dataset_name(path)
 
         if creds is None:
             creds = {}
 
+        db_engine = (runtime or {}).get("db_engine", {})
+
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
+                db_engine=db_engine,
                 read_only=read_only,
                 creds=creds,
                 token=token,
                 memory_cache_size=memory_cache_size,
                 local_cache_size=local_cache_size,
             )
 
@@ -263,32 +269,35 @@
                     if isinstance(e, DatasetCorruptError):
                         raise DatasetCorruptError(
                             message=e.message,
                             action="Try using `reset=True` to reset HEAD changes and load the previous commit.",
                             cause=e.__cause__,
                         )
                     raise DatasetCorruptError(
-                        "Exception occured (see Traceback). The dataset maybe corrupted. "
+                        "Exception occurred (see Traceback). The dataset maybe corrupted. "
                         "Try using `reset=True` to reset HEAD changes and load the previous commit."
                     ) from e
                 return dataset._reset_and_load(
                     cache_chain, access_method, dataset_kwargs, address, e
                 )
 
     @staticmethod
     def exists(
         path: Union[str, pathlib.Path],
-        creds: Optional[dict] = None,
+        creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
     ) -> bool:
         """Checks if a dataset exists at the given ``path``.
 
         Args:
             path (str, pathlib.Path): the path which needs to be checked.
-            creds (dict, optional): A dictionary containing credentials used to access the dataset at the path.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
+                - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
+                - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
 
         Returns:
             A boolean confirming whether the dataset exists or not at the given path.
 
         Raises:
             ValueError: If version is specified in the path
@@ -315,38 +324,41 @@
             # Cloud Dataset does not exist
             return False
         return dataset_exists(storage)
 
     @staticmethod
     def empty(
         path: Union[str, pathlib.Path],
+        runtime: Optional[dict] = None,
         overwrite: bool = False,
         public: bool = False,
         memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE,
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
-        creds: Optional[dict] = None,
+        creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
     ) -> Dataset:
         """Creates an empty dataset
 
         Args:
             path (str, pathlib.Path): - The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             overwrite (bool): If set to ``True`` this overwrites the dataset if it already exists. Defaults to ``False``.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``False``.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
-            creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             verbose (bool): If True, logs will be printed. Defaults to True.
 
         Returns:
             Dataset: Dataset created using the arguments provided.
 
@@ -357,28 +369,30 @@
             TokenPermissionError: When there are permission or other errors related to token
             ValueError: If version is specified in the path
 
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if it exists! Be very careful when setting this parameter.
         """
         path, address = process_dataset_path(path)
+        db_engine = (runtime or {}).get("db_engine", False)
 
         if address:
             raise ValueError(
                 "deeplake.empty does not accept version address in the dataset path."
             )
 
         verify_dataset_name(path)
 
         if creds is None:
             creds = {}
 
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
+                db_engine=db_engine,
                 read_only=False,
                 creds=creds,
                 token=token,
                 memory_cache_size=memory_cache_size,
                 local_cache_size=local_cache_size,
             )
 
@@ -412,15 +426,15 @@
     @staticmethod
     @spinner
     def load(
         path: Union[str, pathlib.Path],
         read_only: Optional[bool] = None,
         memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE,
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
-        creds: Optional[dict] = None,
+        creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         access_method: str = "stream",
         reset: bool = False,
     ) -> Dataset:
         """Loads an existing dataset
@@ -450,17 +464,18 @@
                         - You can also specify a ``commit_id`` or ``branch`` to load the dataset to that version directly by using the ``@`` symbol.
                         - The path will then be of the form ``hub://username/dataset@{branch}`` or ``hub://username/dataset@{commit_id}``.
                         - See examples above.
             read_only (bool, optional): Opens dataset in read only mode if this is passed as ``True``. Defaults to ``False``.
                 Datasets stored on Deep Lake cloud that your account does not have write access to will automatically open in read mode.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
-            creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             verbose (bool): If ``True``, logs will be printed. Defaults to ``True``.
             access_method (str): The access method to use for the dataset. Can be:
 
                     - 'stream'
 
@@ -575,15 +590,15 @@
                     if isinstance(e, DatasetCorruptError):
                         raise DatasetCorruptError(
                             message=e.message,
                             action="Try using `reset=True` to reset HEAD changes and load the previous commit.",
                             cause=e.__cause__,
                         )
                     raise DatasetCorruptError(
-                        "Exception occured (see Traceback). The dataset maybe corrupted. "
+                        "Exception occurred (see Traceback). The dataset maybe corrupted. "
                         "Try using `reset=True` to reset HEAD changes and load the previous commit. "
                         "This will delete all uncommitted changes on the branch you are trying to load."
                     ) from e
                 return dataset._reset_and_load(
                     cache_chain, access_method, dataset_kwargs, address, e
                 )
             raise e
@@ -651,30 +666,31 @@
             ret = get_local_dataset(**dataset_kwargs)
         return ret
 
     @staticmethod
     def rename(
         old_path: Union[str, pathlib.Path],
         new_path: Union[str, pathlib.Path],
-        creds: Optional[dict] = None,
+        creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
     ) -> Dataset:
         """Renames dataset at ``old_path`` to ``new_path``.
 
         Examples:
 
             >>> deeplake.rename("hub://username/image_ds", "hub://username/new_ds")
             >>> deeplake.rename("s3://mybucket/my_ds", "s3://mybucket/renamed_ds")
 
         Args:
             old_path (str, pathlib.Path): The path to the dataset to be renamed.
             new_path (str, pathlib.Path): Path to the dataset after renaming.
-            creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
-                - This takes precedence over credentials present in the environment. Currently only works with s3 paths.
-                - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url' and 'aws_region' as keys.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
+                - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
+                - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
 
         Returns:
             Dataset: The renamed Dataset.
 
         Raises:
             DatasetHandlerError: If a Dataset does not exist at the given path or if new path is to a different directory.
@@ -694,28 +710,29 @@
 
     @staticmethod
     @spinner
     def delete(
         path: Union[str, pathlib.Path],
         force: bool = False,
         large_ok: bool = False,
-        creds: Optional[dict] = None,
+        creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         verbose: bool = False,
     ) -> None:
         """Deletes a dataset at a given path.
 
         Args:
             path (str, pathlib.Path): The path to the dataset to be deleted.
             force (bool): Delete data regardless of whether
                 it looks like a deeplake dataset. All data at the path will be removed if set to ``True``.
             large_ok (bool): Delete datasets larger than 1GB. Disabled by default.
-            creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             verbose (bool): If True, logs will be printed. Defaults to True.
 
         Raises:
             DatasetHandlerError: If a Dataset does not exist at the given path and ``force = False``.
             UserNotLoggedInException: When user is not logged in.
             NotImplementedError: When attempting to delete a managed view.
@@ -774,32 +791,35 @@
                 raise
 
     @staticmethod
     @spinner
     def like(
         dest: Union[str, pathlib.Path],
         src: Union[str, Dataset, pathlib.Path],
+        runtime: Optional[Dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
-        creds: Optional[dict] = None,
+        creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         public: bool = False,
     ) -> Dataset:
         """Creates a new dataset by copying the ``source`` dataset's structure to a new location. No samples are copied,
         only the meta/info for the dataset and it's tensors.
 
         Args:
             dest: Empty Dataset or Path where the new dataset will be created.
             src (Union[str, Dataset]): Path or dataset object that will be used as the template for the new dataset.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             tensors (List[str], optional): Names of tensors (and groups) to be replicated. If not specified all tensors in source dataset are considered.
             overwrite (bool): If True and a dataset exists at `destination`, it will be overwritten. Defaults to False.
-            creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to False.
 
         Returns:
             Dataset: New dataset object.
         """
@@ -810,41 +830,44 @@
         feature_report_path(
             path,
             "like",
             {"Overwrite": overwrite, "Public": public, "Tensors": tensors},
             token=token,
         )
         return dataset._like(
-            dest, src, tensors, overwrite, creds, token, org_id, public
+            dest, src, runtime, tensors, overwrite, creds, token, org_id, public
         )
 
     @staticmethod
     def _like(  # (No reporting)
         dest,
         src: Union[str, Dataset],
+        runtime: Optional[Dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
-        creds: Optional[dict] = None,
+        creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         public: bool = False,
         unlink: Union[List[str], bool] = False,
     ) -> Dataset:
         """Copies the `source` dataset's structure to a new location. No samples are copied, only the meta/info for the dataset and it's tensors.
 
         Args:
             dest: Empty Dataset or Path where the new dataset will be created.
             src (Union[str, Dataset]): Path or dataset object that will be used as the template for the new dataset.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             tensors (List[str], optional): Names of tensors (and groups) to be replicated. If not specified all tensors in source dataset are considered.
             dest (str, pathlib.Path, Dataset): Empty Dataset or Path where the new dataset will be created.
             src (Union[str, pathlib.Path, Dataset]): Path or dataset object that will be used as the template for the new dataset.
             overwrite (bool): If True and a dataset exists at `destination`, it will be overwritten. Defaults to False.
-            creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``False``.
             unlink (Union[List[str], bool]): List of tensors to be unlinked. If ``True`` passed all tensors will be unlinked. Defaults to ``False``, no tensors are unlinked.
 
         Returns:
             Dataset: New dataset object.
@@ -853,14 +876,15 @@
         if isinstance(dest, Dataset):
             destination_ds = dest
             dest_path = dest.path
         else:
             dest_path = dest
             destination_ds = dataset.empty(
                 dest,
+                runtime=runtime,
                 creds=creds,
                 overwrite=overwrite,
                 token=token,
                 org_id=org_id,
                 public=public,
             )
         feature_report_path(
@@ -890,14 +914,15 @@
 
         return destination_ds
 
     @staticmethod
     def copy(
         src: Union[str, pathlib.Path, Dataset],
         dest: Union[str, pathlib.Path],
+        runtime: Optional[dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
         src_creds=None,
         token=None,
         dest_creds=None,
         num_workers: int = 0,
         scheduler="threaded",
@@ -905,19 +930,21 @@
         **kwargs,
     ):
         """Copies dataset at ``src`` to ``dest``. Version control history is not included.
 
         Args:
             src (Union[str, Dataset, pathlib.Path]): The Dataset or the path to the dataset to be copied.
             dest (str, pathlib.Path): Destination path to copy to.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             tensors (List[str], optional): Names of tensors (and groups) to be copied. If not specified all tensors are copied.
             overwrite (bool): If True and a dataset exists at ``dest``, it will be overwritten. Defaults to ``False``.
-            src_creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            src_creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             dest_creds (dict, optional): creds required to create / overwrite datasets at ``dest``.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
             scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
                 Defaults to 'threaded'.
             progressbar (bool): Displays a progress bar if True (default).
             **kwargs (dict): Additional keyword arguments
@@ -946,27 +973,29 @@
             src_ds = src
             src_ds.path = str(src_ds.path)
 
         dest = convert_pathlib_to_string_if_needed(dest)
 
         return src_ds.copy(
             dest,
+            runtime=runtime,
             tensors=tensors,
             overwrite=overwrite,
             creds=dest_creds,
             token=token,
             num_workers=num_workers,
             scheduler=scheduler,
             progressbar=progressbar,
         )
 
     @staticmethod
     def deepcopy(
         src: Union[str, pathlib.Path],
         dest: Union[str, pathlib.Path],
+        runtime: Optional[Dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
         src_creds=None,
         dest_creds=None,
         token=None,
         num_workers: int = 0,
         scheduler="threaded",
@@ -976,19 +1005,21 @@
         **kwargs,
     ):
         """Copies dataset at ``src`` to ``dest`` including version control history.
 
         Args:
             src (str, pathlib.Path): Path to the dataset to be copied.
             dest (str, pathlib.Path): Destination path to copy to.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             tensors (List[str], optional): Names of tensors (and groups) to be copied. If not specified all tensors are copied.
             overwrite (bool): If True and a dataset exists at `destination`, it will be overwritten. Defaults to False.
-            src_creds (dict, optional): - A dictionary containing credentials used to access the dataset at the path.
+            src_creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
+                - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             dest_creds (dict, optional): creds required to create / overwrite datasets at ``dest``.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
             scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
                 Defaults to 'threaded'.
             progressbar (bool): Displays a progress bar if True (default).
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``False``.
@@ -1045,16 +1076,18 @@
                 "The source dataset is corrupted.",
                 "You can try to fix this by loading the dataset with `reset=True` "
                 "which will attempt to reset uncommitted HEAD changes and load the previous version.",
                 e.__cause__,
             )
         src_storage = get_base_storage(src_ds.storage)
 
+        db_engine = (runtime or {}).get("db_engine", False)
         dest_storage, cache_chain = get_storage_and_cache_chain(
             dest,
+            db_engine=db_engine,
             creds=dest_creds,
             token=token,
             read_only=False,
             memory_cache_size=DEFAULT_MEMORY_CACHE_SIZE,
             local_cache_size=DEFAULT_LOCAL_CACHE_SIZE,
         )
 
@@ -1227,16 +1260,16 @@
         dest: Union[str, pathlib.Path],
         key_to_tensor_mapping: Optional[Dict] = None,
         file_to_group_mapping: Optional[Dict] = None,
         ignore_one_group: bool = True,
         ignore_keys: Optional[List[str]] = None,
         image_params: Optional[Dict] = None,
         image_creds_key: Optional[str] = None,
-        src_creds: Optional[Dict] = None,
-        dest_creds: Optional[Dict] = None,
+        src_creds: Optional[Union[str, Dict]] = None,
+        dest_creds: Optional[Union[str, Dict]] = None,
         inspect_limit: int = 1000000,
         progressbar: bool = True,
         shuffle: bool = False,
         num_workers: int = 0,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
@@ -1279,16 +1312,16 @@
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             key_to_tensor_mapping (Optional[Dict]): A one-to-one mapping between COCO keys and Dataset tensor names.
             file_to_group_mapping (Optional[Dict]): A one-to-one mapping between COCO annotation file names and Dataset group names.
             ignore_one_group (bool): Skip creation of group in case of a single annotation file. Set to ``False`` by default.
             ignore_keys (List[str]): A list of COCO keys to ignore.
             image_params (Optional[Dict]): A dictionary containing parameters for the images tensor.
             image_creds_key (Optional[str]): The name of the managed credentials to use for accessing the images in the linked tensor (is applicable).
-            src_creds (Optional[Dict]): Credentials to access the source data. If not provided, will be inferred from the environment.
-            dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
+            src_creds (Optional[Union[str, Dict]]): Credentials to access the source data. If not provided, will be inferred from the environment.
+            dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             inspect_limit (int): The maximum number of samples to inspect in the annotations json, in order to generate the set of COCO annotation keys. Set to ``1000000`` by default.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
             shuffle (bool): Shuffles the input data prior to ingestion. Set to ``False`` by default.
             num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
             token (Optional[str]): The token to use for accessing the dataset and/or connecting it to Deep Lake.
             connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.empty`.
@@ -1347,16 +1380,16 @@
         dest: Union[str, pathlib.Path],
         class_names_file: Optional[Union[str, pathlib.Path]] = None,
         annotations_directory: Optional[Union[str, pathlib.Path]] = None,
         allow_no_annotation: bool = False,
         image_params: Optional[Dict] = None,
         label_params: Optional[Dict] = None,
         coordinates_params: Optional[Dict] = None,
-        src_creds: Optional[Dict] = None,
-        dest_creds: Optional[Dict] = None,
+        src_creds: Optional[Union[str, Dict]] = None,
+        dest_creds: Optional[Union[str, Dict]] = None,
         image_creds_key: Optional[str] = None,
         inspect_limit: int = 1000,
         progressbar: bool = True,
         shuffle: bool = False,
         num_workers: int = 0,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
@@ -1393,16 +1426,16 @@
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             class_names_file: Path to the file containing the class names on separate lines. This is typically a file titled classes.names.
             annotations_directory (Optional[Union[str, pathlib.Path]]): Path to directory containing the annotations. If specified, the 'data_directory' will not be examined for annotations.
             allow_no_annotation (bool): Flag to determine whether missing annotations files corresponding to an image should be treated as empty annoations. Set to ``False`` by default.
             image_params (Optional[Dict]): A dictionary containing parameters for the images tensor.
             label_params (Optional[Dict]): A dictionary containing parameters for the labels tensor.
             coordinates_params (Optional[Dict]): A dictionary containing parameters for the ccoordinates tensor. This tensor either contains bounding boxes or polygons.
-            src_creds (Optional[Dict]): Credentials to access the source data. If not provided, will be inferred from the environment.
-            dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
+            src_creds (Optional[Union[str, Dict]]): Credentials to access the source data. If not provided, will be inferred from the environment.
+            dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             image_creds_key (Optional[str]): creds_key for linked tensors, applicable if the htype for the images tensor is specified as 'link[image]' in the 'image_params' input.
             inspect_limit (int): The maximum number of annotations to inspect, in order to infer whether they are bounding boxes of polygons. This in put is ignored if the htype is specfied in the 'coordinates_params'.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
             shuffle (bool): Shuffles the input data prior to ingestion. Set to ``False`` by default.
             num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
             token (Optional[str]): The token to use for accessing the dataset and/or connecting it to Deep Lake.
             connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
@@ -1472,15 +1505,15 @@
 
     @staticmethod
     def ingest_classification(
         src: Union[str, pathlib.Path],
         dest: Union[str, pathlib.Path],
         image_params: Optional[Dict] = None,
         label_params: Optional[Dict] = None,
-        dest_creds: Optional[Dict] = None,
+        dest_creds: Optional[Union[str, Dict]] = None,
         progressbar: bool = True,
         summary: bool = True,
         num_workers: int = 0,
         shuffle: bool = True,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
@@ -1492,15 +1525,15 @@
             dest (str, pathlib.Path): - The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://org_id/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             image_params (Optional[Dict]): A dictionary containing parameters for the images tensor.
             label_params (Optional[Dict]): A dictionary containing parameters for the labels tensor.
-            dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
+            dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             progressbar (bool): Enables or disables ingestion progress bar. Defaults to ``True``.
             summary (bool): If ``True``, a summary of skipped files will be printed after completion. Defaults to ``True``.
             num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
             shuffle (bool): Shuffles the input data prior to ingestion. Since data arranged in folders by class is highly non-random, shuffling is important in order to produce optimal results when training. Defaults to ``True``.
             token (Optional[str]): The token to use for accessing the dataset.
             connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function see :func:`deeplake.empty`.
@@ -1628,15 +1661,15 @@
     @staticmethod
     def ingest_kaggle(
         tag: str,
         src: Union[str, pathlib.Path],
         dest: Union[str, pathlib.Path],
         exist_ok: bool = False,
         images_compression: str = "auto",
-        dest_creds: Optional[Dict] = None,
+        dest_creds: Optional[Union[str, Dict]] = None,
         kaggle_credentials: Optional[dict] = None,
         progressbar: bool = True,
         summary: bool = True,
         shuffle: bool = True,
         **dataset_kwargs,
     ) -> Dataset:
         """Download and ingest a kaggle dataset and store it as a structured dataset to destination.
@@ -1647,15 +1680,15 @@
             dest (str, pathlib.Path): - The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             exist_ok (bool): If the kaggle dataset was already downloaded and ``exist_ok`` is ``True``, ingestion will proceed without error.
             images_compression (str): For image classification datasets, this compression will be used for the ``images`` tensor. If ``images_compression`` is "auto", compression will be automatically determined by the most common extension in the directory.
-            dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
+            dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             kaggle_credentials (dict): A dictionary containing kaggle credentials {"username":"YOUR_USERNAME", "key": "YOUR_KEY"}. If ``None``, environment variables/the kaggle.json file will be used if available.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
             summary (bool): Generates ingestion summary. Set to ``True`` by default.
             shuffle (bool): Shuffles the input data prior to ingestion. Since data arranged in folders by class is highly non-random, shuffling is important in order to produce optimal results when training. Defaults to ``True``.
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.dataset`.
 
         Returns:
@@ -1707,16 +1740,16 @@
         return ds
 
     @staticmethod
     def ingest_dataframe(
         src,
         dest: Union[str, pathlib.Path],
         column_params: Optional[Dict] = None,
-        src_creds: Optional[Dict] = None,
-        dest_creds: Optional[Dict] = None,
+        src_creds: Optional[Union[str, Dict]] = None,
+        dest_creds: Optional[Union[str, Dict]] = None,
         creds_key: Optional[Dict] = None,
         progressbar: bool = True,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
         **dataset_kwargs,
     ):
         """Convert pandas dataframe to a Deep Lake Dataset. The contents of the dataframe can be parsed literally, or can be treated as links to local or cloud files.
@@ -1746,16 +1779,16 @@
             dest (str, pathlib.Path):
                 - A Dataset or The full path to the dataset. Can be:
                 - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             column_params (Optional[Dict]): A dictionary containing parameters for the tensors corresponding to the dataframe columns.
-            src_creds (Optional[Dict]): Credentials to access the source data. If not provided, will be inferred from the environment.
-            dest_creds (Optional[Dict]): A dictionary containing credentials used to access the destination path of the dataset.
+            src_creds (Optional[Union[str, Dict]]): Credentials to access the source data. If not provided, will be inferred from the environment.
+            dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             creds_key (Optional[str]): creds_key for linked tensors, applicable if the htype any tensor is specified as 'link[...]' in the 'column_params' input.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
             token (Optional[str]): The token to use for accessing the dataset.
             connect_kwargs (Optional[Dict]): A dictionary containing arguments to be passed to the dataset connect method. See :meth:`Dataset.connect`.
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.empty`.
 
         Returns:
```

### Comparing `deeplake-3.3.2/deeplake/api/info.py` & `deeplake-3.4.0/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/link.py` & `deeplake-3.4.0/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/link_tiled.py` & `deeplake-3.4.0/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/read.py` & `deeplake-3.4.0/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_access_method.py` & `deeplake-3.4.0/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_agreement.py` & `deeplake-3.4.0/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_api.py` & `deeplake-3.4.0/deeplake/api/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from deeplake.core.dataset import Dataset
 from deeplake.core.tensor import Tensor
 from deeplake.tests.common import (
     assert_array_lists_equal,
     is_opt_true,
     get_dummy_data_path,
     requires_libdeeplake,
+    requires_torch,
 )
 from deeplake.tests.storage_fixtures import enabled_remote_storages
 from deeplake.core.storage import GCSProvider
 from deeplake.util.exceptions import (
     GroupInfoNotSupportedError,
     InvalidOperationError,
     SampleAppendError,
@@ -590,15 +591,16 @@
         keypoints=["arm", "leg", "torso"],
         connections=[[0, 2], [1, 2]],
     )
     point = memory_ds.create_tensor("point", htype="point")
     point_cloud = memory_ds.create_tensor(
         "point_cloud", htype="point_cloud", sample_compression="las"
     )
-    memory_ds.create_tensor("intrinsics", htype="intrinsics")
+    intrinsics = memory_ds.create_tensor("intrinsics", htype="intrinsics")
+    embedding = memory_ds.create_tensor("embedding", htype="embedding")
 
     image.append(np.ones((28, 28, 3), dtype=np.uint8))
     bbox.append(np.array([1.0, 1.0, 0.0, 0.5], dtype=np.float32))
     # label.append(5)
     label.append(np.array(5, dtype=np.uint32))
     with pytest.raises(SampleAppendError):
         video.append(np.ones((10, 28, 28, 3), dtype=np.uint8))
@@ -610,17 +612,18 @@
     point_cloud.append(
         deeplake.read(
             os.path.join(get_dummy_data_path("point_cloud"), "point_cloud.las")
         )
     )
     point_cloud_dummy_data_path = pathlib.Path(get_dummy_data_path("point_cloud"))
     point_cloud.append(deeplake.read(point_cloud_dummy_data_path / "point_cloud.las"))
-    # Along the forst direcection three matrices are concatenated, the first matrix is P,
+    # Along the first direcection three matrices are concatenated, the first matrix is P,
     # the second one is Tr and the third one is R
-    memory_ds.intrinsics.append(np.zeros((3, 4, 4), dtype=np.float32))
+    intrinsics.append(np.zeros((3, 4, 4), dtype=np.float32))
+    embedding.append(np.random.rand((100)))
 
 
 def test_dtype(memory_ds: Dataset):
     tensor = memory_ds.create_tensor("tensor")
     dtyped_tensor = memory_ds.create_tensor("dtyped_tensor", dtype="uint8")
     np_dtyped_tensor = memory_ds.create_tensor(
         "np_dtyped_tensor", dtype=MAX_FLOAT_DTYPE
@@ -1040,14 +1043,15 @@
     assert deeplake.htypes == [
         "audio",
         "bbox",
         "bbox.3d",
         "binary_mask",
         "class_label",
         "dicom",
+        "embedding",
         "generic",
         "image",
         "image.gray",
         "image.rgb",
         "instance_label",
         "intrinsics",
         "json",
```

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.4.0/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.4.0/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.4.0/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.4.0/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_dataset.py` & `deeplake-3.4.0/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_dicom.py` & `deeplake-3.4.0/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_downsample.py` & `deeplake-3.4.0/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_events.py` & `deeplake-3.4.0/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_grayscale.py` & `deeplake-3.4.0/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_info.py` & `deeplake-3.4.0/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.4.0/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_json.py` & `deeplake-3.4.0/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_link.py` & `deeplake-3.4.0/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.4.0/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_linking.py` & `deeplake-3.4.0/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_mesh.py` & `deeplake-3.4.0/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_meta.py` & `deeplake-3.4.0/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_nifti.py` & `deeplake-3.4.0/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_none.py` & `deeplake-3.4.0/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.4.0/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_pickle.py` & `deeplake-3.4.0/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.4.0/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_polygons.py` & `deeplake-3.4.0/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_pop.py` & `deeplake-3.4.0/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_readonly.py` & `deeplake-3.4.0/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_rechunk.py` & `deeplake-3.4.0/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_reset.py` & `deeplake-3.4.0/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_sample_info.py` & `deeplake-3.4.0/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_text.py` & `deeplake-3.4.0/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_update_samples.py` & `deeplake-3.4.0/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_video.py` & `deeplake-3.4.0/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tests/test_views.py` & `deeplake-3.4.0/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/api/tiled.py` & `deeplake-3.4.0/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/structured/base.py` & `deeplake-3.4.0/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/structured/dataframe.py` & `deeplake-3.4.0/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.4.0/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.4.0/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.4.0/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.4.0/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/base.py` & `deeplake-3.4.0/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.4.0/deeplake/auto/unstructured/coco/coco.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         annotation_files: Union[str, List[str]],
         key_to_tensor_mapping: Optional[Dict] = None,
         file_to_group_mapping: Optional[Dict] = None,
         ignore_one_group: bool = False,
         ignore_keys: Optional[List[str]] = None,
         image_params: Optional[Dict] = None,
         image_creds_key: Optional[str] = None,
-        creds: Optional[Dict] = None,
+        creds: Optional[Union[str, Dict]] = None,
     ):
         super().__init__(source)
         self._creds = creds
         self._image_creds_key = image_creds_key
         self.image_params = image_params or {}
         self.images = CocoImages(images_directory=source, creds=creds)
```

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.4.0/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.4.0/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.4.0/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.4.0/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.4.0/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/util.py` & `deeplake-3.4.0/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.4.0/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.4.0/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import deeplake
 
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 from deeplake.core.dataset import Dataset
 from deeplake.util.exceptions import IngestionError
 from deeplake.client.log import logger
 
 from ..base import UnstructuredDataset
 from ..util import DatasetStructure, TensorStructure
@@ -30,15 +30,15 @@
         annotations_directory: Optional[str] = None,
         image_params: Optional[Dict] = None,
         label_params: Optional[Dict] = None,
         coordinates_params: Optional[Dict] = None,
         allow_no_annotation: Optional[bool] = False,
         verify_class_names: Optional[bool] = True,
         inspect_limit: Optional[int] = 1000,
-        creds: Optional[Dict] = None,
+        creds: Optional[Union[str, Dict]] = None,
         image_creds_key: Optional[str] = None,
     ):
         """Container for access to Yolo Data, parsing of key information, and conversions to a Deep Lake dataset"""
 
         super().__init__(data_directory)
 
         self.class_names_file = class_names_file
```

### Comparing `deeplake-3.3.2/deeplake/cli/auth.py` & `deeplake-3.4.0/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/cli/test_cli.py` & `deeplake-3.4.0/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/client/client.py` & `deeplake-3.4.0/deeplake/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import deeplake
 import requests
-from typing import Optional
+from typing import Optional, List
 from deeplake.util.exceptions import (
     AgreementNotAcceptedError,
     AuthorizationException,
     LoginException,
     InvalidPasswordException,
     ManagedCredentialsNotFoundError,
     NotLoggedInAgreementError,
@@ -34,14 +34,15 @@
     CREATE_DATASET_SUFFIX,
     DATASET_SUFFIX,
     GET_USER_PROFILE,
     SEND_EVENT_SUFFIX,
     UPDATE_SUFFIX,
     GET_PRESIGNED_URL_SUFFIX,
     CONNECT_DATASET_SUFFIX,
+    REMOTE_QUERY_SUFFIX,
 )
 from deeplake.client.log import logger
 import jwt  # should add it to requirements.txt
 
 # for these codes, we will retry requests upto 3 times
 retry_status_codes = {502}
 
@@ -208,42 +209,51 @@
         self.request("POST", REGISTER_USER_SUFFIX, json=json)
 
     def get_dataset_credentials(
         self,
         org_id: str,
         ds_name: str,
         mode: Optional[str] = None,
+        db_engine: Optional[dict] = None,
         no_cache: bool = False,
     ):
         """Retrieves temporary 12 hour credentials for the required dataset from the backend.
 
         Args:
             org_id (str): The name of the user/organization to which the dataset belongs.
             ds_name (str): The name of the dataset being accessed.
             mode (str, optional): The mode in which the user has requested to open the dataset.
                 If not provided, the backend will set mode to 'a' if user has write permission, else 'r'.
+            db_engine (dict, optional): The database engine args to use for the dataset.
             no_cache (bool): If True, cached creds are ignored and new creds are returned. Default False.
 
         Returns:
             tuple: containing full url to dataset, credentials, mode and expiration time respectively.
 
         Raises:
             UserNotLoggedInException: When user is not logged in
             InvalidTokenException: If the specified token is invalid
             TokenPermissionError: when there are permission or other errors related to token
             AgreementNotAcceptedError: when user has not accepted the agreement
             NotLoggedInAgreementError: when user is not logged in and dataset has agreement which needs to be signed
         """
+        import json
+
+        db_engine = db_engine or {}
         relative_url = GET_DATASET_CREDENTIALS_SUFFIX.format(org_id, ds_name)
         try:
             response = self.request(
                 "GET",
                 relative_url,
                 endpoint=self.endpoint(),
-                params={"mode": mode, "no_cache": no_cache},
+                params={
+                    "mode": mode,
+                    "no_cache": no_cache,
+                    "db_engine": json.dumps(db_engine),
+                },
             ).json()
         except Exception as e:
             if isinstance(e, AuthorizationException):
                 authorization_exception_prompt = "You don't have permission"
                 response_data = e.response.json()
                 code = response_data.get("code")
                 if code == 1:
@@ -265,40 +275,44 @@
                         in response_data["description"].lower()
                         and decoded_token["id"] == "public"
                     ):
                         raise UserNotLoggedInException()
                     raise TokenPermissionError()
             raise
         full_url = response.get("path")
+        repository = response.get("repository")
         creds = response["creds"]
         mode = response["mode"]
         expiration = creds["expiration"]
-        return full_url, creds, mode, expiration
+        return full_url, creds, mode, expiration, repository
 
     def send_event(self, event_json: dict):
         """Sends an event to the backend.
 
         Args:
             event_json (dict): The event to be sent.
         """
         self.request("POST", SEND_EVENT_SUFFIX, json=event_json)
 
-    def create_dataset_entry(self, username, dataset_name, meta, public=True):
+    def create_dataset_entry(
+        self, username, dataset_name, meta, public=True, repository=None
+    ):
         tag = f"{username}/{dataset_name}"
-        repo = f"protected/{username}"
+        if repository is None:
+            repository = f"protected/{username}"
 
         response = self.request(
             "POST",
             CREATE_DATASET_SUFFIX,
             json={
                 "tag": tag,
-                "repository": repo,
                 "public": public,
                 "rewrite": True,
                 "meta": meta,
+                "repository": repository,
             },
             endpoint=self.endpoint(),
         )
 
         if response.status_code == 200:
             logger.info("Your Deep Lake dataset has been successfully created!")
             if public is False:
@@ -472,7 +486,32 @@
                 "ds_name": ds_name,
                 "creds_key": creds_key,
             },
             endpoint=self.endpoint(),
         ).json()
 
         return response["generated_id"]
+
+    def remote_query(self, org_id: str, ds_name: str, query_string: str) -> List[int]:
+        """Queries a remote dataset.
+
+        Args:
+            org_id (str): The organization to which the dataset belongs.
+            ds_name (str): The name of the dataset.
+            query_string (str): The query string.
+
+        Returns:
+            dict: The indicies matching the query.
+        """
+        response = self.request(
+            "POST",
+            REMOTE_QUERY_SUFFIX.format(org_id, ds_name),
+            json={"query": query_string},
+            endpoint=self.endpoint(),
+        ).json()
+
+        indicies = response["indices"]
+        if len(indicies) == 0:
+            return []
+
+        indicies = [int(i) for i in indicies.split(",")]
+        return indicies
```

### Comparing `deeplake-3.3.2/deeplake/client/config.py` & `deeplake-3.4.0/deeplake/client/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 DATASET_SUFFIX = "/api/dataset"
 UPDATE_SUFFIX = "/api/org/{}/dataset/{}"
 GET_MANAGED_CREDS_SUFFIX = "/api/org/{}/storage/name"
 ACCEPT_AGREEMENTS_SUFFIX = "/api/organization/{}/dataset/{}/agree"
 REJECT_AGREEMENTS_SUFFIX = "/api/organization/{}/dataset/{}/disagree"
 GET_USER_PROFILE = "/api/user/profile"
 CONNECT_DATASET_SUFFIX = "/api/dataset/connect"
+REMOTE_QUERY_SUFFIX = "/api/query/dataset/{}/{}"
 
 DEFAULT_REQUEST_TIMEOUT = 170
 
 DEEPLAKE_AUTH_TOKEN = "ACTIVELOOP_TOKEN"
```

### Comparing `deeplake-3.3.2/deeplake/client/log.py` & `deeplake-3.4.0/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/client/test_client.py` & `deeplake-3.4.0/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/client/utils.py` & `deeplake-3.4.0/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/compression.py` & `deeplake-3.4.0/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/constants.py` & `deeplake-3.4.0/deeplake/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,7 +179,11 @@
 LOCK_LOCAL_DATASETS = not PYTEST_ENABLED
 
 # Rechunk after transform if average chunk size is less than
 # this fraction of min chunk size
 TRANSFORM_RECHUNK_AVG_SIZE_BOUND = 0.1
 
 TIME_INTERVAL_FOR_CUDA_MEMORY_CLEANING = 10 * 60
+
+# Transform cache sizes
+DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE = 16
+TRANSFORM_CHUNK_CACHE_SIZE = 64 * MB
```

### Comparing `deeplake-3.3.2/deeplake/core/chunk/base_chunk.py` & `deeplake-3.4.0/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.4.0/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.4.0/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.4.0/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.4.0/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.4.0/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.4.0/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/chunk_engine.py` & `deeplake-3.4.0/deeplake/core/chunk_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,20 +485,25 @@
     def num_chunks(self) -> int:
         if not self.chunk_id_encoder_exists:
             return 0
         return self.chunk_id_encoder.num_chunks
 
     @property
     def num_samples(self) -> int:
-        """Returns the length of the primary axis of the tensor.
+        """Total length of tensor (includes samples in sequences)
         Ignores any applied indexing and returns the total length.
         """
         return self.tensor_meta.length
 
     @property
+    def tensor_length(self) -> int:
+        """Length of primary axis of tensor (does not include samples in sequences)"""
+        return self._sequence_length or self.tensor_meta.length
+
+    @property
     def last_chunk_key(self) -> str:
         last_chunk_name = self.last_appended_chunk_name
         commit_id, tkey = self.get_chunk_commit(last_chunk_name)
         return get_chunk_key(tkey, last_chunk_name, commit_id)
 
     def get_chunk_key_for_id(self, chunk_id) -> str:
         chunk_name = ChunkIdEncoder.name_from_id(chunk_id)
@@ -1873,15 +1878,15 @@
         sample = coalesce_tiles(tiles, tile_shape, None, self.tensor_meta.dtype)
         sample = sample[sample_index]
         return sample
 
     def get_single_sample(
         self, global_sample_index, index, fetch_chunks=False, pad_tensor=False
     ):
-        if pad_tensor and global_sample_index >= self.tensor_meta.length:
+        if pad_tensor and global_sample_index >= self.tensor_length:
             sample = self.get_empty_sample()
             try:
                 return sample[tuple(entry.value for entry in index.values[1:])]
             except IndexError:
                 return sample
 
         if not self._is_tiled_sample(global_sample_index):
@@ -1973,15 +1978,15 @@
             return samples
         return np.array(samples)
 
     def numpy_from_data_cache(self, index, length, aslist, pad_tensor=False):
         samples = []
         enc = self.chunk_id_encoder
         for global_sample_index in index.values[0].indices(length):
-            if pad_tensor and global_sample_index >= self.tensor_meta.length:
+            if pad_tensor and global_sample_index >= self.tensor_length:
                 sample = self.get_empty_sample()
                 try:
                     sample = sample[tuple(entry.value for entry in index.values[1:])]
                 except IndexError:
                     pass
             else:
                 if (
@@ -2103,14 +2108,15 @@
             "requires StorageProvider to be able to list all chunks"
         )
 
     def pop(
         self,
         global_sample_index: Optional[int] = None,
         link_callback: Optional[Callable] = None,
+        sample_id: Optional[int] = None,
     ):
         if global_sample_index is None:
             if self.is_sequence:
                 global_sample_index = self.sequence_encoder.num_samples - 1
             else:
                 global_sample_index = self.num_samples - 1
         self._write_initialization()
@@ -2125,15 +2131,15 @@
         initial_autoflush = self.cache.autoflush
         self.cache.autoflush = False
 
         # pop links
         if link_callback:
             link_callback(global_sample_index)
 
-        self.commit_diff.pop(global_sample_index)
+        self.commit_diff.pop(global_sample_index, sample_id)
         if self.is_sequence:
             # pop in reverse order else indices get shifted
             for idx in reversed(range(*self.sequence_encoder[global_sample_index])):
                 self.pop_item(idx)
             self.sequence_encoder.pop(global_sample_index)
         else:
             self.pop_item(global_sample_index)
@@ -2486,18 +2492,27 @@
                 max_ = length
         return min_, max_
 
     def check_link_ready(self):
         return
 
     def shape(
-        self, index: Index, sample_shape_provider: Optional[Callable] = None
+        self,
+        index: Index,
+        sample_shape_provider: Optional[Callable] = None,
+        pad_tensor: bool = False,
     ) -> Tuple[Optional[int], ...]:
-        shape = self.shape_interval(index).astuple()[1:]
         index_0, sample_index = index.values[0], index.values[1:]
+        if (
+            not index_0.subscriptable()
+            and pad_tensor
+            and index_0.value >= self.tensor_length  # type: ignore
+        ):
+            return self.get_empty_sample().shape
+        shape = self.shape_interval(index).astuple()[1:]
         sample_indices = list(
             index_0.indices(self._sequence_length or self.num_samples)
         )
         num_samples = len(sample_indices)
 
         if num_samples == 0:
             return (0, *shape)
@@ -2703,10 +2718,14 @@
 
     def get_avg_chunk_size(self):
         num_chunks, num_samples = self.num_chunks, self.num_samples
         max_shape = self.tensor_meta.max_shape
         dtype = self.tensor_meta.dtype
         if dtype in ("Any", "List", None):
             return None
-        nbytes = np.prod([num_samples] + max_shape) * np.dtype(dtype).itemsize
+        shape = [num_samples] + max_shape
+        nbytes = 1
+        for dim in shape:  # not using np.prod to avoid overflow
+            nbytes *= dim
+        nbytes = nbytes * np.dtype(dtype).itemsize
         avg_chunk_size = nbytes / num_chunks
         return avg_chunk_size
```

### Comparing `deeplake-3.3.2/deeplake/core/compression.py` & `deeplake-3.4.0/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/compute/process.py` & `deeplake-3.4.0/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/compute/provider.py` & `deeplake-3.4.0/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/compute/ray.py` & `deeplake-3.4.0/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/compute/serial.py` & `deeplake-3.4.0/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/compute/thread.py` & `deeplake-3.4.0/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/dataset/__init__.py` & `deeplake-3.4.0/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/dataset/dataset.py` & `deeplake-3.4.0/deeplake/core/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from deeplake.util.iteration_warning import (
     suppress_iteration_warning,
     check_if_iteration,
 )
 from deeplake.api.info import load_info
 from deeplake.client.log import logger
 from deeplake.client.utils import get_user_name
+from deeplake.client.client import DeepLakeBackendClient
 from deeplake.constants import (
     FIRST_COMMIT_ID,
     DEFAULT_MEMORY_CACHE_SIZE,
     DEFAULT_LOCAL_CACHE_SIZE,
     MB,
     SAMPLE_INFO_TENSOR_MAX_CHUNK_SIZE,
     DEFAULT_READONLY,
@@ -1953,24 +1954,24 @@
             save_result=save_result,
             result_path=result_path,
             result_ds_args=result_ds_args,
         )
         dataset_read(self)
         return ret
 
-    def query(self, query_string: str):
+    def query(self, query_string: str, runtime: Optional[Dict] = None):
         """Returns a sliced :class:`~deeplake.core.dataset.Dataset` with given query results. To use this, install deeplake with ``pip install deeplake[enterprise]``.
 
         It allows to run SQL like queries on dataset and extract results. See supported keywords and the Tensor Query Language documentation
         :ref:`here <tql>`.
 
 
         Args:
             query_string (str): An SQL string adjusted with new functionalities to run on the given :class:`~deeplake.core.dataset.Dataset` object
-
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
 
         Returns:
             Dataset: A :class:`~deeplake.core.dataset.Dataset` object.
 
         Examples:
 
             Query from dataset all the samples with lables other than ``5``
@@ -1987,14 +1988,20 @@
         **Restrictions**
 
         Querying datasets is part of our Growth and Enterprise Plan .
 
         - Users of our Community plan can only perform queries on Activeloop datasets ("hub://activeloop/..." datasets).
         - To run queries on your own datasets, `upgrade your organization's plan <https://www.activeloop.ai/pricing/>`_.
         """
+        if runtime is not None and runtime.get("db_engine", False):
+            client = DeepLakeBackendClient(token=self._token)
+            org_id, ds_name = self.path[6:].split("/")
+            indicies = client.remote_query(org_id, ds_name, query_string)
+            return self[indicies]
+
         from deeplake.enterprise import query
 
         return query(self, query_string)
 
     def sample_by(
         self,
         weights: Union[str, list, tuple],
@@ -3354,14 +3361,15 @@
                     self.version_state["tensor_names"],
                 )
         return ret
 
     def _copy(
         self,
         dest: Union[str, pathlib.Path],
+        runtime: Optional[Dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
         creds=None,
         token=None,
         num_workers: int = 0,
         scheduler="threaded",
         progressbar=True,
@@ -3369,14 +3377,15 @@
         unlink: bool = False,
         create_vds_index_tensor: bool = False,
     ):
         """Copies this dataset or dataset view to `dest`. Version control history is not included.
 
         Args:
             dest (str, pathlib.Path): Destination dataset or path to copy to. If a Dataset instance is provided, it is expected to be empty.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             tensors (List[str], optional): Names of tensors (and groups) to be copied. If not specified all tensors are copied.
             overwrite (bool): If ``True`` and a dataset exists at `destination`, it will be overwritten. Defaults to False.
             creds (dict, Optional): creds required to create / overwrite datasets at `dest`.
             token (str, Optional): token used to for fetching credentials to `dest`.
             num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
             scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
                 Defaults to 'threaded'.
@@ -3408,14 +3417,15 @@
         if path.startswith("hub://"):
             report_params["Dest"] = path
         feature_report_path(self.path, "copy", report_params, token=token)
 
         dest_ds = deeplake.api.dataset.dataset._like(
             dest,
             self,
+            runtime=runtime,
             tensors=tensors,
             creds=creds,
             token=token,
             overwrite=overwrite,
             public=public,
             unlink=[
                 t
@@ -3501,28 +3511,30 @@
                 dest_ds = dest_ds[0]
                 self.index.values[0] = old_first_index
         return dest_ds
 
     def copy(
         self,
         dest: Union[str, pathlib.Path],
+        runtime: Optional[dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
         creds=None,
         token=None,
         num_workers: int = 0,
         scheduler="threaded",
         progressbar=True,
         public: bool = False,
     ):
         """Copies this dataset or dataset view to ``dest``. Version control history is not included.
 
         Args:
             dest (str, pathlib.Path): Destination dataset or path to copy to. If a Dataset instance is provided, it is expected to be empty.
             tensors (List[str], optional): Names of tensors (and groups) to be copied. If not specified all tensors are copied.
+            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
             overwrite (bool): If ``True`` and a dataset exists at `destination`, it will be overwritten. Defaults to False.
             creds (dict, Optional): creds required to create / overwrite datasets at `dest`.
             token (str, Optional): token used to for fetching credentials to `dest`.
             num_workers (int): The number of workers to use for copying. Defaults to 0. When set to 0, it will always use serial processing, irrespective of the scheduler.
             scheduler (str): The scheduler to be used for copying. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
                 Defaults to 'threaded'.
             progressbar (bool): Displays a progress bar If ``True`` (default).
@@ -3532,14 +3544,15 @@
             Dataset: New dataset object.
 
         Raises:
             DatasetHandlerError: If a dataset already exists at destination path and overwrite is False.
         """
         return self._copy(
             dest,
+            runtime,
             tensors,
             overwrite,
             creds,
             token,
             num_workers,
             scheduler,
             progressbar,
@@ -4032,7 +4045,10 @@
                 "Random_split is not supported for datasets with variable length tensors."
             )
         return create_random_split_views(self, lengths)
 
     def _temp_write_access(self):
         # Defined in DeepLakeCloudDataset
         return memoryview(b"")  # No-op context manager
+
+    def _get_storage_repository(self) -> Optional[str]:
+        return getattr(self.base_storage, "repository", None)
```

### Comparing `deeplake-3.3.2/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.4.0/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         if self._is_sub_ds():
             return
         self.client.create_dataset_entry(
             self.org_id,
             self.ds_name,
             self.version_state["meta"].__getstate__(),
             public=self.public,
+            repository=self._get_storage_repository(),
         )
         self._send_dataset_creation_event()
 
     def _send_event(
         self,
         event_id: str,
         event_group: str,
```

### Comparing `deeplake-3.3.2/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.4.0/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.4.0/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/dataset/invalid_view.py` & `deeplake-3.4.0/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/dataset/view_entry.py` & `deeplake-3.4.0/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/fast_forwarding.py` & `deeplake-3.4.0/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/index/index.py` & `deeplake-3.4.0/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/io.py` & `deeplake-3.4.0/deeplake/core/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 from deeplake.core.storage import (
     LRUCache,
     MemoryProvider,
     StorageProvider,
     LocalProvider,
 )
 from deeplake.core.tiling.deserialize import combine_chunks
-from deeplake.integrations.pytorch.common import check_tensors, validate_decode_method
+from deeplake.integrations.pytorch.common import (
+    check_tensors,
+    find_additional_tensors_and_info,
+    get_htype_ndim_tensor_info_dicts,
+    convert_sample_to_data,
+    validate_decode_method,
+)
 from deeplake.util.exceptions import DatasetUnsupportedPytorch, ReadSampleFromChunkError
 from deeplake.util.keys import get_chunk_key, get_tensor_meta_key
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.storage import get_pytorch_local_storage
 from PIL import Image  # type: ignore
 
 
@@ -263,14 +269,15 @@
         self,
         dataset,
         tensors: Sequence[str],
         use_local_cache: bool = False,
         pad_tensors: bool = False,
         decode_method: Optional[Dict[str, str]] = None,
         tobytes: Union[bool, Sequence[str]] = False,
+        verbose: bool = True,
     ) -> None:
         super().__init__()
 
         self.dataset = dataset
         self.local_storage: Optional[LocalProvider] = (
             get_pytorch_local_storage(dataset) if use_local_cache else None
         )
@@ -281,32 +288,42 @@
             raise DatasetUnsupportedPytorch(
                 "The underlying storage is MemoryProvider which isn't supported."
             )
 
         self.tensors = tensors
         self.pad_tensors = pad_tensors
         self.decode_method = decode_method
-
         jpeg_png_compressed_tensors, json_tensors, list_tensors = check_tensors(
-            self.dataset, tensors
+            self.dataset, tensors, verbose
         )
         (
             raw_tensors,
             pil_compressed_tensors,
             json_tensors,
             list_tensors,
+            data_tensors,
         ) = validate_decode_method(
             self.decode_method,
             tensors,
             jpeg_png_compressed_tensors,
             json_tensors,
             list_tensors,
         )
+        sample_info_tensors, tensor_info_tensors = find_additional_tensors_and_info(
+            dataset, data_tensors
+        )
+        self.tensors += sample_info_tensors
+        (
+            self.htype_dict,
+            self.ndim_dict,
+            self.tensor_info_dict,
+        ) = get_htype_ndim_tensor_info_dicts(dataset, data_tensors, tensor_info_tensors)
         self.raw_tensors = set(raw_tensors)
         self.pil_compressed_tensors = set(pil_compressed_tensors)
+        self.data_tensors = set(data_tensors)
 
         self.chunk_engines: ChunkEngineMap = self._map_chunk_engines(self.tensors)
 
         self.local_caches: Optional[CachesMap] = (
             ({tensor: self._use_cache(self.local_storage) for tensor in self.tensors})
             if self.local_storage is not None
             else None
@@ -317,14 +334,19 @@
         self._group_index_length = group_index_length
 
     def read(self, schedule: Schedule) -> Iterator:
         for block in schedule._blocks:
             yield from self.stream(block)
 
     def stream(self, block: IOBlock):
+        htype_dict, ndim_dict, tensor_info_dict = (
+            self.htype_dict,
+            self.ndim_dict,
+            self.tensor_info_dict,
+        )
         for idx in block.indices():
             sample = dict()
             valid_sample_flag = True
 
             for keyid, (key, engine) in enumerate(self.chunk_engines.items()):
                 rel_key = key[self._group_index_length :]
                 decompress = key not in self.raw_tensors
@@ -380,14 +402,18 @@
                         f"Skipping corrupt {engine.tensor_meta.sample_compression} sample at dataset.{key}[{idx}]"
                     )
                     valid_sample_flag = False
                     break
 
             if valid_sample_flag:
                 sample["index"] = np.array([idx])
+                if self.data_tensors:
+                    convert_sample_to_data(
+                        sample, htype_dict, ndim_dict, tensor_info_dict
+                    )
                 yield sample
 
     def _get_block_for_single_sample(self, idx):
         chunks = []
         for engine in self.chunk_engines.values():
             enc = engine.chunk_id_encoder
             try:
```

### Comparing `deeplake-3.3.2/deeplake/core/ipc.py` & `deeplake-3.4.0/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/link_creds.py` & `deeplake-3.4.0/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/linked_chunk_engine.py` & `deeplake-3.4.0/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/linked_sample.py` & `deeplake-3.4.0/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/linked_tiled_sample.py` & `deeplake-3.4.0/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/lock.py` & `deeplake-3.4.0/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/dataset_meta.py` & `deeplake-3.4.0/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.4.0/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.4.0/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.4.0/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/creds.py` & `deeplake-3.4.0/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/pad.py` & `deeplake-3.4.0/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/sequence.py` & `deeplake-3.4.0/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/shape.py` & `deeplake-3.4.0/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.4.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/encode/tile.py` & `deeplake-3.4.0/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/meta/tensor_meta.py` & `deeplake-3.4.0/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/partial_reader.py` & `deeplake-3.4.0/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/partial_sample.py` & `deeplake-3.4.0/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/polygon.py` & `deeplake-3.4.0/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/query/autocomplete.py` & `deeplake-3.4.0/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/query/filter.py` & `deeplake-3.4.0/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/query/query.py` & `deeplake-3.4.0/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/sample.py` & `deeplake-3.4.0/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/serialize.py` & `deeplake-3.4.0/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.4.0/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/storage/gcs.py` & `deeplake-3.4.0/deeplake/core/storage/gcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,23 +267,27 @@
             NotADirectoryError,
             AttributeError,
             NotFound,
         )
         self._initialize_provider()
         self._presigned_urls: Dict[str, Tuple[str, float]] = {}
         self.expiration: Optional[str] = None
+        self.db_engine: bool = False
+        self.repository: Optional[str] = None
 
     def subdir(self, path: str, read_only: bool = False):
         sd = self.__class__(
             root=posixpath.join(self.root, path),
             token=self.token,
             project=self.project,
         )
         if self.expiration:
-            sd._set_hub_creds_info(self.hub_path, self.expiration)
+            sd._set_hub_creds_info(
+                self.hub_path, self.expiration, self.db_engine, self.repository
+            )
         sd.read_only = read_only
         return sd
 
     def _initialize_provider(self):
         self._set_bucket_and_path()
         if not self.token:
             self.token = None
@@ -312,25 +316,35 @@
     def _get_path_from_key(self, key):
         return posixpath.join(self.path, key)
 
     def _all_keys(self):
         self._blob_objects = self.client_bucket.list_blobs(prefix=self.path)
         return {posixpath.relpath(obj.name, self.path) for obj in self._blob_objects}
 
-    def _set_hub_creds_info(self, hub_path: str, expiration: str):
+    def _set_hub_creds_info(
+        self,
+        hub_path: str,
+        expiration: str,
+        db_engine: bool = True,
+        repository: Optional[str] = None,
+    ):
         """Sets the tag and expiration of the credentials. These are only relevant to datasets using Deep Lake storage.
         This info is used to fetch new credentials when the temporary 12 hour credentials expire.
 
         Args:
             hub_path (str): The deeplake cloud path to the dataset.
             expiration (str): The time at which the credentials expire.
+            db_engine (bool): Whether Activeloop DB Engine enabled.
+            repository (str, Optional): Backend repository where the dataset is stored.
         """
         self.hub_path = hub_path
         self.tag = hub_path[6:]  # removing the hub:// part from the path
         self.expiration = expiration
+        self.db_engine = db_engine
+        self.repository = repository
 
     def clear(self, prefix=""):
         """Remove all keys with given prefix below root - empties out mapping.
 
         Warning:
             Exercise caution!
         """
@@ -434,22 +448,26 @@
     def __getstate__(self):
         return (
             self.root,
             self.token,
             self.missing_exceptions,
             self.project,
             self.read_only,
+            self.db_engine,
+            self.repository,
         )
 
     def __setstate__(self, state):
         self.root = state[0]
         self.token = state[1]
         self.missing_exceptions = state[2]
         self.project = state[3]
         self.read_only = state[4]
+        self.db_engine = state[5]
+        self.repository = state[6]
         self._initialize_provider()
 
     def get_presigned_url(self, key, full=False):
         if full:
             root = _remove_protocol_from_path(key)
             split_root = root.split("/", 1)
             bucket = split_root[0]
```

### Comparing `deeplake-3.3.2/deeplake/core/storage/google_drive.py` & `deeplake-3.4.0/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/storage/local.py` & `deeplake-3.4.0/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/storage/lru_cache.py` & `deeplake-3.4.0/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/storage/memory.py` & `deeplake-3.4.0/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/storage/provider.py` & `deeplake-3.4.0/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/storage/s3.py` & `deeplake-3.4.0/deeplake/core/storage/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import deeplake
 from math import ceil
 import time
 import boto3
 import botocore  # type: ignore
 import posixpath
 from typing import Dict, Optional, Tuple, Type
+from datetime import datetime
 from botocore.session import ComponentLocator
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.core.storage.provider import StorageProvider
 from deeplake.util.exceptions import (
     S3GetAccessError,
     S3DeletionError,
     S3GetError,
@@ -111,22 +112,25 @@
         self.root = root
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.aws_session_token = aws_session_token
         self.aws_region: Optional[str] = aws_region
         self.endpoint_url: Optional[str] = endpoint_url
         self.expiration: Optional[str] = None
+        self.repository: Optional[str] = None
+        self.db_engine: bool = False
         self.tag: Optional[str] = None
         self.token: Optional[str] = token
         self.loaded_creds_from_environment = False
         self.client_config = deeplake.config["s3"]
         self.start_time = time.time()
         self.profile_name = profile_name
         self._initialize_s3_parameters()
         self._presigned_urls: Dict[str, Tuple[str, float]] = {}
+        self.creds_used: Optional[str] = None
 
     def async_supported(self) -> bool:
         return asyncio is not None
 
     def subdir(self, path: str, read_only: bool = False):
         sd = self.__class__(
             root=posixpath.join(self.root, path),
@@ -134,16 +138,17 @@
             aws_secret_access_key=self.aws_secret_access_key,
             aws_session_token=self.aws_session_token,
             aws_region=self.aws_region,
             endpoint_url=self.endpoint_url,
             token=self.token,
         )
         if self.expiration:
-            sd._set_hub_creds_info(self.hub_path, self.expiration)  # type: ignore
+            sd._set_hub_creds_info(self.hub_path, self.expiration, self.db_engine, self.repository)  # type: ignore
         sd.read_only = read_only
+        sd.creds_used = self.creds_used
         return sd
 
     def _set(self, path, content):
         self.client.put_object(
             Bucket=self.bucket,
             Body=content,
             Key=path,
@@ -431,19 +436,22 @@
             "aws_access_key_id",
             "aws_secret_access_key",
             "aws_session_token",
             "aws_region",
             "endpoint_url",
             "client_config",
             "expiration",
+            "db_engine",
+            "repository",
             "tag",
             "token",
             "loaded_creds_from_environment",
             "read_only",
             "profile_name",
+            "creds_used",
         }
 
     def __getstate__(self):
         return {key: getattr(self, key) for key in self._state_keys()}
 
     def __setstate__(self, state):
         assert set(state.keys()) == self._state_keys()
@@ -458,52 +466,66 @@
         if len(split_root) > 1:
             self.path = split_root[1]
         else:
             self.path = ""
         if not self.path.endswith("/"):
             self.path += "/"
 
-    def _set_hub_creds_info(self, hub_path: str, expiration: str):
+    def _set_hub_creds_info(
+        self,
+        hub_path: str,
+        expiration: str,
+        db_engine: bool = True,
+        repository: Optional[str] = None,
+    ):
         """Sets the tag and expiration of the credentials. These are only relevant to datasets using Deep Lake storage.
         This info is used to fetch new credentials when the temporary 12 hour credentials expire.
 
         Args:
-            hub_path (str): The Deep Lake cloud path to the dataset.
+            hub_path (str): The deeplake cloud path to the dataset.
             expiration (str): The time at which the credentials expire.
+            db_engine (bool): Whether Activeloop DB Engine enabled.
+            repository (str, Optional): Backend repository where the dataset is stored.
         """
         self.hub_path = hub_path
         self.tag = hub_path[6:]  # removing the hub:// part from the path
         self.expiration = expiration
+        self.db_engine = db_engine
+        self.repository = repository
 
     def _initialize_s3_parameters(self):
         self._set_bucket_and_path()
 
         if self.aws_access_key_id is None and self.aws_secret_access_key is None:
             self._locate_and_load_creds()
             self.loaded_creds_from_environment = True
 
         self._set_s3_client_and_resource()
 
     def _check_update_creds(self, force=False):
         """If the client has an expiration time, check if creds are expired and fetch new ones.
         This would only happen for datasets stored on Deep Lake storage for which temporary 12 hour credentials are generated.
         """
-        if self.expiration and (force or float(self.expiration) < time.time()):
+        if self.expiration and (
+            force or float(self.expiration) < datetime.utcnow().timestamp()
+        ):
             client = DeepLakeBackendClient(self.token)
             org_id, ds_name = self.tag.split("/")
 
             mode = "r" if self.read_only else "a"
 
-            url, creds, mode, expiration = client.get_dataset_credentials(
+            url, creds, mode, expiration, repo = client.get_dataset_credentials(
                 org_id,
                 ds_name,
                 mode,
+                {"enabled": self.db_engine},
                 True,
             )
             self.expiration = expiration
+            self.repository = repo
             self.aws_access_key_id = creds.get("aws_access_key_id")
             self.aws_secret_access_key = creds.get("aws_secret_access_key")
             self.aws_session_token = creds.get("aws_session_token")
             self._set_s3_client_and_resource()
 
     def _locate_and_load_creds(self):
         session = boto3.session.Session(profile_name=self.profile_name)._session
```

### Comparing `deeplake-3.3.2/deeplake/core/tensor.py` & `deeplake-3.4.0/deeplake/core/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -470,15 +470,17 @@
         sample_shape_provider = (
             self._sample_shape_provider(sample_shape_tensor)
             if sample_shape_tensor
             else None
         )
         shape: Tuple[Optional[int], ...]
         shape = self.chunk_engine.shape(
-            self.index, sample_shape_provider=sample_shape_provider
+            self.index,
+            sample_shape_provider=sample_shape_provider,
+            pad_tensor=self.pad_tensor,
         )
 
         if len(self.index.values) == 1 and not self.index.values[0].subscriptable():
             if np.sum(shape) == 0 and self.meta.max_shape:  # type: ignore
                 shape = (0,) * len(self.meta.max_shape)
         if self.meta.max_shape == [0, 0, 0]:
             shape = ()
@@ -578,17 +580,15 @@
         return self.shape_interval.is_dynamic
 
     @property
     def num_samples(self) -> int:
         """Returns the length of the primary axis of the tensor.
         Ignores any applied indexing and returns the total length.
         """
-        if self.is_sequence:
-            return self.chunk_engine._sequence_length
-        return self.chunk_engine.num_samples
+        return self.chunk_engine.tensor_length
 
     def __len__(self):
         """Returns the length of the primary axis of the tensor.
         Accounts for indexing into the tensor object.
 
         Examples:
             >>> len(tensor)
@@ -964,15 +964,18 @@
 
         Raises:
             ValueError: If the tensor has multiple samples.
         """
         if self.index.values[0].subscriptable() or len(self.index.values) > 1:
             raise ValueError("tobytes() can be used only on exactly 1 sample.")
         idx = self.index.values[0].value
-        ret = self.chunk_engine.read_bytes_for_sample(idx)  # type: ignore
+        if self.pad_tensor and idx >= self.num_samples:  # type: ignore
+            ret = self.chunk_engine.get_empty_sample().tobytes()
+        else:
+            ret = self.chunk_engine.read_bytes_for_sample(idx)  # type: ignore
         dataset_read(self.dataset)
         return ret
 
     def _extend_links(self, samples, flat: Optional[bool], progressbar: bool = False):
         has_shape_tensor = False
         for k, v in self.meta.links.items():
             if flat is None or v["flatten_sequence"] == flat:
@@ -1040,19 +1043,23 @@
                     else:
                         val = cast_to_type(val, tensor.dtype)
                         tensor[global_sample_index] = val
 
     @invalid_view_op
     def pop(self, index: Optional[int] = None):
         """Removes an element at the given index."""
-
+        sample_id_tensor = self._sample_id_tensor
+        if index is None:
+            index = self.num_samples - 1
+        sample_id = int(sample_id_tensor[index].numpy()) if sample_id_tensor else None
         self.chunk_engine.pop(
-            index, link_callback=self._pop_links if self.meta.links else None
+            index,
+            link_callback=self._pop_links if self.meta.links else None,
+            sample_id=sample_id,
         )
-
         self.invalidate_libdeeplake_dataset()
 
     def _pop_links(self, global_sample_index: int):
         # meta.links contain tensor keys not names
         rev_tensor_names = {v: k for k, v in self.dataset.meta.tensor_names.items()}
 
         if self.meta.is_sequence:
```

### Comparing `deeplake-3.3.2/deeplake/core/tensor_link.py` & `deeplake-3.4.0/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/test_serialize.py` & `deeplake-3.4.0/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tests/test_compression.py` & `deeplake-3.4.0/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tests/test_compute.py` & `deeplake-3.4.0/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.4.0/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,29 +100,29 @@
     view_path = view.save_view()
     view_id = view_path.split("/")[-1]
     view = deeplake_ds.load_view(view_id)
 
     dataloader = view[:3].dataloader().pytorch()
     iss = []
     for i, batch in enumerate(dataloader):
-        assert len(batch["label"][0]) == 10
+        assert len(batch["label"]) == 10
         iss.append(i)
 
     assert iss == [0, 1, 2]
     assert np.all(indra_ds.image.numpy() == deeplake_indra_ds.image.numpy())
 
     view = deeplake_ds[0:50].query(query_str)
     view_path = view.save_view()
     view_id = view_path.split("/")[-1]
     view = deeplake_ds.load_view(view_id)
 
     dataloader = view[:3].dataloader().pytorch()
     iss = []
     for i, batch in enumerate(dataloader):
-        assert len(batch["label"][0]) == 5
+        assert len(batch["label"]) == 5
         iss.append(i)
 
     assert iss == [0, 1, 2]
     assert np.all(indra_ds.image.numpy() == deeplake_indra_ds.image.numpy())
 
 
 @requires_libdeeplake
```

### Comparing `deeplake-3.3.2/deeplake/core/tests/test_io.py` & `deeplake-3.4.0/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tests/test_locking.py` & `deeplake-3.4.0/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tests/test_readonly.py` & `deeplake-3.4.0/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tests/test_serialize.py` & `deeplake-3.4.0/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tiling/deserialize.py` & `deeplake-3.4.0/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tiling/optimizer.py` & `deeplake-3.4.0/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.4.0/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tiling/serialize.py` & `deeplake-3.4.0/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.4.0/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/tiling/test_serialize.py` & `deeplake-3.4.0/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/transform/test_transform.py` & `deeplake-3.4.0/deeplake/core/transform/test_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1487,7 +1487,37 @@
         np.testing.assert_array_equal(
             ds.abc[i * 5 : (i + 1) * 5].numpy(), i * 2 * np.ones((5, 5, 5))
         )
         np.testing.assert_array_equal(
             ds.images[i * 5 : (i + 1) * 5].numpy(),
             np.tile(flower_arr - 1, (5, 1, 1, 1)),
         )
+
+
+def test_pad_data_in_bug(local_ds):
+    @deeplake.compute
+    def upload(stuff, ds):
+        append_dict = {}
+        for tensor in ds.tensors:
+            append_dict[tensor] = stuff[tensor]
+
+        ds.append(append_dict)
+
+    with local_ds as ds:
+        ds.create_tensor("abc", htype="class_label")
+        ds.create_tensor("xyz")
+
+        ds.abc.extend([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
+        ds.xyz.extend([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11])
+
+    ds2 = deeplake.empty(local_ds.path + "_2", overwrite=True)
+    ds2.create_tensor("abc", htype="class_label")
+    ds2.create_tensor("xyz")
+
+    upload().eval(ds, ds2, num_workers=TRANSFORM_TEST_NUM_WORKERS, pad_data_in=True)
+
+    assert len(ds2) == 11
+    np.testing.assert_array_equal(ds2.abc[:10].numpy(), ds.abc.numpy())
+    np.testing.assert_array_equal(ds2.abc[10].numpy(), np.zeros((0,)))
+    np.testing.assert_array_equal(ds2.xyz.numpy(), ds.xyz.numpy())
+
+    ds2.delete()
```

### Comparing `deeplake-3.3.2/deeplake/core/transform/transform.py` & `deeplake-3.4.0/deeplake/core/transform/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     HubComposeEmptyListError,
     HubComposeIncompatibleFunction,
     TransformError,
 )
 from deeplake.hooks import dataset_written, dataset_read
 from deeplake.util.version_control import auto_checkout
 from deeplake.util.class_label import sync_labels
+from deeplake.constants import DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE
 
 import posixpath
 
 
 class ComputeFunction:
     def __init__(self, func, args, kwargs, name: Optional[str] = None):
         """Creates a ComputeFunction object that can be evaluated using .eval or used as a part of a Pipeline."""
@@ -53,15 +54,15 @@
         num_workers: int = 0,
         scheduler: str = "threaded",
         progressbar: bool = True,
         skip_ok: bool = False,
         check_lengths: bool = True,
         pad_data_in: bool = False,
         read_only_ok: bool = False,
-        cache_size: int = 16,
+        cache_size: int = DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE,
         checkpoint_interval: int = 0,
         ignore_errors: bool = False,
         **kwargs,
     ):
         """Evaluates the ComputeFunction on data_in to produce an output dataset ds_out.
 
         Args:
@@ -131,15 +132,15 @@
         num_workers: int = 0,
         scheduler: str = "threaded",
         progressbar: bool = True,
         skip_ok: bool = False,
         check_lengths: bool = True,
         pad_data_in: bool = False,
         read_only_ok: bool = False,
-        cache_size: int = 16,
+        cache_size: int = DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE,
         checkpoint_interval: int = 0,
         ignore_errors: bool = False,
         **kwargs,
     ):
         """Evaluates the pipeline on ``data_in`` to produce an output dataset ``ds_out``.
 
         Args:
```

### Comparing `deeplake-3.3.2/deeplake/core/transform/transform_dataset.py` & `deeplake-3.4.0/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/transform/transform_tensor.py` & `deeplake-3.4.0/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.4.0/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/version_control/commit_diff.py` & `deeplake-3.4.0/deeplake/core/version_control/commit_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
     def __init__(self, first_index=0, created=False) -> None:
         self.is_dirty = created  # only put as dirty during init if created
         self.created = created
         self.data_added: List[int] = [first_index, first_index]
         self.data_updated: Set[int] = set()
         self.data_deleted: Set[int] = set()
+        self.data_deleted_ids: Set[int] = set()
         self.info_updated = False
         self.cleared = False
 
         # this is stored for in place transforms in which we no longer need to considered older diffs about added/updated data
         self.data_transformed = False
 
     def tobytes(self) -> bytes:
@@ -26,27 +27,29 @@
         3. The third byte is a boolean value indicating whether the data has been transformed using an inplace transform or not.
         4. The next 8 + 8 bytes are the two elements of the data_added list.
         5. The next 8 bytes are the number of elements in the data_updated set, let's call this m.
         6. The next 8 * m bytes are the elements of the data_updated set.
         7. The next byte is a boolean value indicating whether the tensor was cleared in the commit or not.
         8. The next 8 bytes are the number of elements in the data_deleted set, let's call this n.
         9. The next 8 * n bytes are the elements of the data_deleted set.
+        9. The next 8 * n bytes are the elements of the data_deleted_ids set.
         """
         return b"".join(
             [
                 self.created.to_bytes(1, "big"),
                 self.info_updated.to_bytes(1, "big"),
                 self.data_transformed.to_bytes(1, "big"),
                 self.data_added[0].to_bytes(8, "big"),
                 self.data_added[1].to_bytes(8, "big"),
                 len(self.data_updated).to_bytes(8, "big"),
                 *(idx.to_bytes(8, "big") for idx in self.data_updated),
                 self.cleared.to_bytes(1, "big"),
                 len(self.data_deleted).to_bytes(8, "big"),
                 *(idx.to_bytes(8, "big") for idx in self.data_deleted),
+                *(idx.to_bytes(8, "big") for idx in self.data_deleted_ids),
             ]
         )
 
     @classmethod
     def frombuffer(cls, data: bytes) -> "CommitDiff":
         """Creates a CommitDiff object from bytes"""
         commit_diff = cls()
@@ -63,23 +66,29 @@
             int.from_bytes(data[27 + i * 8 : 35 + i * 8], "big")
             for i in range(num_updates)
         }
         pos = 35 + (num_updates - 1) * 8
         commit_diff.cleared = bool(int.from_bytes(data[pos : pos + 1], "big"))
         commit_diff.is_dirty = False
         pos += 1
+        commit_diff.data_deleted = set()
+        commit_diff.data_deleted_ids = set()
         if len(data) > pos:
             num_deletes = int.from_bytes(data[pos : pos + 8], "big")
             pos += 8
             commit_diff.data_deleted = {
                 int.from_bytes(data[pos + i * 8 : pos + i * 8 + 8], "big")
                 for i in range(num_deletes)
             }
-        else:
-            commit_diff.data_deleted = set()
+            pos += num_deletes * 8
+            if len(data) > pos:
+                commit_diff.data_deleted_ids = {
+                    int.from_bytes(data[pos + i * 8 : pos + i * 8 + 8], "big")
+                    for i in range(num_deletes)
+                }
         return commit_diff
 
     @property
     def nbytes(self):
         """Returns number of bytes required to store the commit diff"""
         return 36 + 8 * (len(self.data_updated) + len(self.data_deleted))
 
@@ -115,27 +124,29 @@
         self.is_dirty = True
 
     def transform_data(self) -> None:
         """Stores information that the data has been transformed using an inplace transform."""
         self.data_transformed = True
         self.is_dirty = True
 
-    def pop(self, index) -> None:
+    def pop(self, index, id) -> None:
         index = self.translate_index(index)
         if index not in range(*self.data_added):
             self.data_deleted.add(index)
             self.data_added[0] -= 1
         self.data_added[1] -= 1
 
         if index in self.data_updated:
             self.data_updated.remove(index)
 
         self.data_updated = {
             idx - 1 if idx > index else idx for idx in self.data_updated
         }
+        if id is not None:
+            self.data_deleted_ids.add(id)
         self.is_dirty = True
 
     def translate_index(self, index):
         if not self.data_deleted:
             return index
         offset = sum(i < index for i in self.data_deleted)
         return index + offset
```

### Comparing `deeplake-3.3.2/deeplake/core/version_control/commit_node.py` & `deeplake-3.4.0/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.4.0/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/core/version_control/test_merge.py` & `deeplake-3.4.0/deeplake/core/version_control/test_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,7 +619,23 @@
         ds.checkout("branch2", create=True)
         ds.x[150] = 10
         ds.x[250] = 20
         ds.x[350] = 30
         ds.checkout("branch1")
         ds.merge("branch2")
         assert len(ds.x) == 304
+
+
+def test_merge_with_pop(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("x")
+        ds.x.extend([1, 2, 3, 4, 5])
+        cid = ds.commit()
+        ds.checkout("branch1", create=True)
+        ds.pop(2)
+        ds.checkout(cid)
+        ds.checkout("branch2", create=True)
+        ds.pop(3)
+        ds.x.append(6)
+        ds.checkout("branch1")
+        ds.merge("branch2")
+        np.testing.assert_array_equal(ds.x.numpy().flatten(), [1, 2, 4, 5, 6])
```

### Comparing `deeplake-3.3.2/deeplake/core/version_control/test_version_control.py` & `deeplake-3.4.0/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.4.0/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,38 +26,60 @@
 
 
 INDRA_INSTALLED = bool(importlib.util.find_spec("indra"))
 
 
 def dataset_to_libdeeplake(hub2_dataset):
     """Convert a hub 2.x dataset object to a libdeeplake dataset object."""
+    try_flushing(hub2_dataset)
+    api = import_indra_api()
+    path: str = hub2_dataset.path
     if hub2_dataset.libdeeplake_dataset is None:
-        api = import_indra_api()
-        try_flushing(hub2_dataset)
-        path: str = hub2_dataset.path
+        libdeeplake_dataset = None
         if path.startswith("gdrive://"):
             raise ValueError("Gdrive datasets are not supported for libdeeplake")
         elif path.startswith("mem://"):
             raise ValueError("In memory datasets are not supported for libdeeplake")
         elif path.startswith("hub://"):
             token = hub2_dataset._token
             provider = hub2_dataset.storage.next_storage
             if isinstance(provider, S3Provider):
-                provider._check_update_creds()
-                libdeeplake_dataset = api.dataset(
-                    path,
-                    origin_path=provider.root,
-                    token=token,
-                    aws_access_key_id=provider.aws_access_key_id,
-                    aws_secret_access_key=provider.aws_secret_access_key,
-                    aws_session_token=provider.aws_session_token,
-                    region_name=provider.aws_region,
-                    endpoint_url=provider.endpoint_url,
-                    expiration=str(provider.expiration),
-                )
+                creds_used = provider.creds_used
+                if creds_used == "PLATFORM":
+                    provider._check_update_creds()
+                    libdeeplake_dataset = api.dataset(
+                        path,
+                        origin_path=provider.root,
+                        token=token,
+                        aws_access_key_id=provider.aws_access_key_id,
+                        aws_secret_access_key=provider.aws_secret_access_key,
+                        aws_session_token=provider.aws_session_token,
+                        region_name=provider.aws_region,
+                        endpoint_url=provider.endpoint_url,
+                        expiration=str(provider.expiration),
+                    )
+                elif creds_used == "ENV":
+                    libdeeplake_dataset = api.dataset(
+                        path,
+                        origin_path=provider.root,
+                        token=token,
+                        profile_name=provider.profile_name,
+                    )
+                elif creds_used == "DICT":
+                    libdeeplake_dataset = api.dataset(
+                        path,
+                        origin_path=provider.root,
+                        token=token,
+                        aws_access_key_id=provider.aws_access_key_id,
+                        aws_secret_access_key=provider.aws_secret_access_key,
+                        aws_session_token=provider.aws_session_token,
+                        region_name=provider.aws_region,
+                        endpoint_url=provider.endpoint_url,
+                    )
+
             elif isinstance(provider, GCSProvider):
                 creds = provider.get_creds()
                 anon = creds.get("anon", "")
                 expiration = creds.get("expiration", "")
                 access_token = creds.get("access_token", "")
                 json_credentials = creds.get("json_credentials", "")
                 endpoint_override = creds.get("endpoint_override", "")
```

### Comparing `deeplake-3.3.2/deeplake/enterprise/dataloader.py` & `deeplake-3.4.0/deeplake/enterprise/dataloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 )
 from deeplake.hooks import dataset_read
 from deeplake.enterprise.libdeeplake_query import query, sample_by
 from deeplake.integrations.pytorch.common import (
     PytorchTransformFunction,
     check_tensors,
     validate_decode_method,
+    find_additional_tensors_and_info,
+    get_htype_ndim_tensor_info_dicts,
 )
 from deeplake.util.dataset import map_tensor_keys
 from functools import partial
 import importlib
 
 try:
     from torch.utils.data.dataloader import DataLoader, _InfiniteConstantSampler
@@ -571,40 +573,49 @@
         all_vars["_mode"] = mode
         all_vars["_persistent_workers"] = persistent_workers
         all_vars["_dataloader"] = None
         return self.__class__(**all_vars)
 
     def __iter__(self):
         if self._dataloader is None:
+            dataset = self._orig_dataset
             collate_fn = self.collate_fn
             upcast = self._mode == "pytorch"  # upcast to handle unsupported dtypes
 
             primary_tensor_name = self._primary_tensor_name
             buffer_size = self._buffer_size
 
-            tensors = self._tensors or map_tensor_keys(self._orig_dataset, None)
+            tensors = self._tensors or map_tensor_keys(dataset, None)
 
             jpeg_png_compressed_tensors, json_tensors, list_tensors = check_tensors(
-                self._orig_dataset, tensors
+                dataset, tensors
             )
             (
                 raw_tensors,
                 pil_compressed_tensors,
                 json_tensors,
                 list_tensors,
+                data_tensors,
             ) = validate_decode_method(
                 self._decode_method,
                 tensors,
                 jpeg_png_compressed_tensors,
                 json_tensors,
                 list_tensors,
             )
+            sample_info_tensors, tensor_info_tensors = find_additional_tensors_and_info(
+                dataset, data_tensors
+            )
+            tensors.extend(sample_info_tensors)
+            htype_dict, ndim_dict, tensor_info_dict = get_htype_ndim_tensor_info_dicts(
+                dataset, data_tensors, tensor_info_tensors
+            )
             if deeplake.constants.RETURN_DUMMY_DATA_FOR_DATALOADER:
                 self._dataloader = DummyDataloader(
-                    deeplake_dataset=self._orig_dataset,
+                    deeplake_dataset=dataset,
                     batch_size=self._batch_size,
                     shuffle=self._shuffle,
                     num_workers=self._num_workers,
                     collate_fn=collate_fn,
                     transform_fn=self._transform,
                     distributed=self._distributed,
                     prefetch_factor=self._prefetch_factor,
@@ -614,15 +625,15 @@
                     return_index=self._return_index,
                     raw_tensors=raw_tensors,
                     pil_compressed_tensors=pil_compressed_tensors,
                     persistent_workers=self._persistent_workers,
                 )
             else:
                 if not hasattr(self, "_indra_dataset"):
-                    indra_dataset = dataset_to_libdeeplake(self._orig_dataset)
+                    indra_dataset = dataset_to_libdeeplake(dataset)
                 else:
                     indra_dataset = self._indra_dataset
                 self._dataloader = INDRA_LOADER(
                     indra_dataset,
                     batch_size=self._batch_size,
                     num_threads=self._num_threads,
                     shuffle=self._shuffle,
@@ -638,14 +649,17 @@
                     primary_tensor=primary_tensor_name,
                     buffer_size=buffer_size,
                     raw_tensors=raw_tensors,
                     pil_compressed_tensors=pil_compressed_tensors,
                     json_tensors=json_tensors,
                     list_tensors=list_tensors,
                     persistent_workers=self._persistent_workers,
+                    htype_dict=htype_dict,
+                    ndim_dict=ndim_dict,
+                    tensor_info_dict=tensor_info_dict,
                 )
         dataset_read(self._orig_dataset)
         return iter(self._dataloader)
 
 
 def dataloader(dataset) -> DeepLakeDataLoader:
     """Returns a :class:`~deeplake.enterprise.dataloader.DeepLakeDataLoader` object which can be transformed to either pytorch dataloader or numpy.
```

### Comparing `deeplake-3.3.2/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.4.0/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.4.0/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/enterprise/test_pytorch.py` & `deeplake-3.4.0/deeplake/enterprise/test_pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 PYTORCH_TESTS_MAX_CHUNK_SIZE = 5 * KB
 
 
 def double(sample):
     return sample * 2
 
 
+def identity(batch):
+    return batch
+
+
 def identity_collate(batch):
     return batch
 
 
 def to_tuple(sample, t1, t2):
     return sample[t1], sample[t2]
 
@@ -252,18 +256,23 @@
         np.testing.assert_array_equal(c1[0], hub_cloud_ds.c.numpy()[i])
         np.testing.assert_array_equal(d1[0], hub_cloud_ds.d.numpy()[i])
 
 
 @requires_torch
 @requires_libdeeplake
 def test_readonly_with_two_workers(hub_cloud_ds):
-    hub_cloud_ds.create_tensor("images", max_chunk_size=PYTORCH_TESTS_MAX_CHUNK_SIZE)
-    hub_cloud_ds.create_tensor("labels", max_chunk_size=PYTORCH_TESTS_MAX_CHUNK_SIZE)
-    hub_cloud_ds.images.extend(np.ones((10, 12, 12)))
-    hub_cloud_ds.labels.extend(np.ones(10))
+    with hub_cloud_ds:
+        hub_cloud_ds.create_tensor(
+            "images", max_chunk_size=PYTORCH_TESTS_MAX_CHUNK_SIZE
+        )
+        hub_cloud_ds.create_tensor(
+            "labels", max_chunk_size=PYTORCH_TESTS_MAX_CHUNK_SIZE
+        )
+        hub_cloud_ds.images.extend(np.ones((10, 12, 12)))
+        hub_cloud_ds.labels.extend(np.ones(10))
 
     base_storage = get_base_storage(hub_cloud_ds.storage)
     base_storage.flush()
     base_storage.enable_readonly()
     ds = Dataset(
         storage=hub_cloud_ds.storage,
         token=hub_cloud_ds.token,
@@ -445,15 +454,15 @@
         hub_cloud_ds.image.extend(
             [deeplake.read(compressed_image_paths["jpeg"][0])] * 5
         )
 
     ptds = hub_cloud_ds.dataloader().pytorch(decode_method={"image": "tobytes"})
 
     for i, batch in enumerate(ptds):
-        image = batch["image"][0]
+        image = batch["image"]
         assert isinstance(image, bytes)
         if i < 5 and not compression:
             np.testing.assert_array_equal(
                 np.frombuffer(image, dtype=np.uint8).reshape(10, 10, 3),
                 i * np.ones((10, 10, 3), dtype=np.uint8),
             )
         elif i >= 5 and compression:
@@ -491,23 +500,14 @@
         np.testing.assert_array_equal(
             np.array(sample["red/green"]), np.array([[1, 2, 3, 4]])
         )
 
 
 @requires_torch
 @requires_libdeeplake
-def test_expiration_date_casting_to_string():
-    ds = deeplake.dataset("hub://activeloop/cifar100-train")[0:10:2]
-    loader = ds.dataloader().pytorch(return_index=False)
-    for _ in loader:
-        pass
-
-
-@requires_torch
-@requires_libdeeplake
 @pytest.mark.parametrize("num_workers", [0, 2])
 def test_indexes(hub_cloud_ds, num_workers):
     shuffle = False
     with hub_cloud_ds as ds:
         ds.create_tensor("xyz")
         for i in range(8):
             ds.xyz.append(i * np.ones((2, 2)))
@@ -536,15 +536,17 @@
         for i in range(8):
             ds.xyz.append(i * np.ones((2, 2)))
 
     ptds = (
         hub_cloud_ds.dataloader()
         .batch(4)
         .transform(index_transform)
-        .pytorch(num_workers=num_workers, return_index=True)
+        .pytorch(
+            num_workers=num_workers, return_index=True, collate_fn=identity_collate
+        )
     )
     if shuffle:
         ptds = ptds.shuffle()
 
     for batch in ptds:
         assert len(batch) == 4
         assert len(batch[0]) == 2
@@ -765,7 +767,58 @@
     dl = ds.dataloader().batch(2)
 
     for batch in dl:
         sample1 = batch[0]["list"]
         sample2 = batch[1]["list"]
         assert sample1.tolist() == l
         assert sample2.tolist() == l
+
+
+@requires_libdeeplake
+@requires_torch
+def test_pytorch_data_decode(hub_cloud_ds, cat_path):
+    with hub_cloud_ds as ds:
+        ds.create_tensor("generic")
+        for i in range(10):
+            ds.generic.append(i)
+        ds.create_tensor("text", htype="text")
+        for i in range(10):
+            ds.text.append(f"hello {i}")
+        ds.create_tensor("json", htype="json")
+        for i in range(10):
+            ds.json.append({"x": i})
+        ds.create_tensor("list", htype="list")
+        for i in range(10):
+            ds.list.append([i, i + 1])
+        ds.create_tensor("class_label", htype="class_label")
+        animals = [
+            "cat",
+            "dog",
+            "bird",
+            "fish",
+            "horse",
+            "cow",
+            "pig",
+            "sheep",
+            "goat",
+            "chicken",
+        ]
+        ds.class_label.extend(animals)
+        ds.create_tensor("image", htype="image", sample_compression="jpeg")
+        for i in range(10):
+            ds.image.append(deeplake.read(cat_path))
+
+    decode_method = {tensor: "data" for tensor in list(ds.tensors.keys())}
+    ptds = (
+        ds.dataloader()
+        .transform(identity)
+        .pytorch(decode_method=decode_method, collate_fn=identity_collate)
+    )
+    for i, batch in enumerate(ptds):
+        sample = batch[0]
+        assert sample["text"]["value"] == f"hello {i}"
+        assert sample["json"]["value"] == {"x": i}
+        assert sample["list"]["value"].tolist() == [i, i + 1]
+        assert sample["class_label"]["value"] == [i]
+        assert sample["class_label"]["text"] == [animals[i]]
+        assert sample["image"]["value"].shape == (900, 900, 3)
+        assert sample["generic"]["value"] == i
```

### Comparing `deeplake-3.3.2/deeplake/enterprise/test_query.py` & `deeplake-3.4.0/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.4.0/deeplake/enterprise/test_tensorflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -526,23 +526,14 @@
         np.testing.assert_array_equal(
             np.array(sample["red/green"]), np.array([[1, 2, 3, 4]])
         )
 
 
 @requires_tensorflow
 @requires_libdeeplake
-def test_expiration_date_casting_to_string():
-    ds = deeplake.dataset("hub://activeloop/cifar100-train")[0:10:2]
-    loader = ds.dataloader().tensorflow(return_index=False)
-    for _ in loader:
-        pass
-
-
-@requires_tensorflow
-@requires_libdeeplake
 @pytest.mark.parametrize("num_workers", [0, 2])
 def test_indexes(hub_cloud_ds, num_workers):
     shuffle = False
     with hub_cloud_ds as ds:
         ds.create_tensor("xyz")
         for i in range(8):
             ds.xyz.append(i * np.ones((2, 2)))
```

### Comparing `deeplake-3.3.2/deeplake/enterprise/util.py` & `deeplake-3.4.0/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/hooks.py` & `deeplake-3.4.0/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/htype.py` & `deeplake-3.4.0/deeplake/htype.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     LIST = "list"
     DICOM = "dicom"
     NIFTI = "nifti"
     POINT_CLOUD = "point_cloud"
     INTRINSICS = "intrinsics"
     POLYGON = "polygon"
     MESH = "mesh"
+    EMBEDDING = "embedding"
 
 
 # used for requiring the user to specify a value for htype properties. notates that the htype property has no default.
 REQUIRE_USER_SPECIFICATION = "require_user_specification"
 
 # used for `REQUIRE_USER_SPECIFICATION` enforcement. this should be used instead of `None` for default user method arguments.
 UNSPECIFIED = "unspecified"
@@ -92,14 +93,15 @@
     htype.TEXT: {"dtype": "str"},
     htype.DICOM: {"sample_compression": "dcm"},
     htype.NIFTI: {},
     htype.POINT_CLOUD: {"dtype": "float32"},
     htype.INTRINSICS: {"dtype": "float32"},
     htype.POLYGON: {"dtype": "float32"},
     htype.MESH: {"sample_compression": "ply"},
+    htype.EMBEDDING: {},
 }
 
 HTYPE_VERIFICATIONS: Dict[str, Dict] = {
     htype.BBOX: {"coords": {"type": dict, "keys": ["type", "mode"]}},
     htype.BBOX_3D: {"coords": {"type": dict, "keys": ["mode"]}},
 }
 
@@ -118,14 +120,15 @@
     htype.LIST: BYTE_COMPRESSIONS[:],
     htype.JSON: BYTE_COMPRESSIONS[:],
     htype.POINT_CLOUD: POINT_CLOUD_COMPRESSIONS[:],
     htype.DICOM: ["dcm"],
     htype.NIFTI: ["nii", "nii.gz"],
     htype.POLYGON: BYTE_COMPRESSIONS[:],
     htype.MESH: MESH_COMPRESSIONS[:],
+    htype.EMBEDDING: BYTE_COMPRESSIONS[:],
 }
 
 
 # these configs are added to every `htype`
 COMMON_CONFIGS = {
     "sample_compression": None,
     "chunk_compression": None,
```

### Comparing `deeplake-3.3.2/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.4.0/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.4.0/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/pytorch/common.py` & `deeplake-3.4.0/deeplake/integrations/pytorch/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import Callable, Dict, Optional
 import warnings
+from deeplake.util.class_label import convert_to_text
 from deeplake.util.exceptions import EmptyTensorError
 from deeplake.util.iterable_ordered_dict import IterableOrderedDict
+from deeplake.util.keys import get_sample_info_tensor_key
+from deeplake.util.object_3d.mesh import parse_mesh_to_dict
+from deeplake.util.object_3d.point_cloud import parse_point_cloud_to_dict
 from deeplake.core.polygon import Polygons
 import numpy as np
 import warnings
 
 
 def collate_fn(batch):
     import torch
@@ -22,15 +26,18 @@
     elif isinstance(elem, (tuple, list)) and len(elem) > 0 and isinstance(elem[0], str):
         batch = [it[0] for it in batch]
     elif isinstance(elem, Polygons):
         batch = [it.numpy() for it in batch]
     elif isinstance(elem, list) and all(
         map(lambda e: isinstance(e, np.ndarray), elem)
     ):  # special case for video query api
-        if elem[0].shape[1] not in [2, 3]:  # checking whether it is not a polygon
+        if len(elem[0].shape) > 1 and elem[0].shape[1] not in [
+            2,
+            3,
+        ]:  # checking whether it is not a polygon
             elem_type = type(elem)
             return [
                 elem_type([torch.tensor(item) for item in sample]) for sample in batch
             ]
     return default_collate(batch)
 
 
@@ -65,15 +72,15 @@
                 value = data_in[tensor]
                 data_out[tensor] = value if fn is None else fn(value)
             data_out = IterableOrderedDict(data_out)
             return data_out
         return data_in
 
 
-def check_tensors(dataset, tensors):
+def check_tensors(dataset, tensors, verbose=True):
     jpeg_png_compressed_tensors = []
     json_tensors = []
     list_tensors = []
     supported_image_compressions = {"png", "jpeg"}
     for tensor_name in tensors:
         tensor = dataset._get_tensor_from_root(tensor_name)
         if len(tensor) == 0:
@@ -86,15 +93,15 @@
         if meta.sample_compression in supported_image_compressions:
             jpeg_png_compressed_tensors.append(tensor_name)
         elif meta.htype == "json":
             json_tensors.append(tensor_name)
         elif meta.htype == "list":
             list_tensors.append(tensor_name)
 
-    if json_tensors or list_tensors:
+    if verbose and (json_tensors or list_tensors):
         json_list_tensors = set(json_tensors + list_tensors)
         warnings.warn(
             f"The following tensors have json or list htype: {json_list_tensors}. Collation of these tensors will fail by default. Ensure that these tensors are either transformed by specifying a transform or a custom collate_fn is specified to handle them."
         )
 
     return jpeg_png_compressed_tensors, json_tensors, list_tensors
 
@@ -104,30 +111,37 @@
     all_tensor_keys,
     jpeg_png_compressed_tensors,
     json_tensors,
     list_tensors,
 ):
     raw_tensors = []
     pil_compressed_tensors = []
+    data_tensors = []
     if decode_method is None:
         if len(jpeg_png_compressed_tensors) > 0:
             warnings.warn(
                 f"Decode method for tensors {jpeg_png_compressed_tensors} is defaulting to numpy. Please consider specifying a decode_method in .pytorch() that maximizes the data preprocessing speed based on your transformation."
             )
-        return raw_tensors, pil_compressed_tensors, json_tensors, list_tensors
+        return (
+            raw_tensors,
+            pil_compressed_tensors,
+            json_tensors,
+            list_tensors,
+            data_tensors,
+        )
 
     jpeg_png_compressed_tensors_set = set(jpeg_png_compressed_tensors)
     json_list_tensors_set = set(json_tensors + list_tensors)
-    generic_supported_decode_methods = {"numpy", "tobytes"}
-    jpeg_png_supported_decode_methods = {"numpy", "tobytes", "pil"}
-    json_list_supported_decode_methods = {"numpy"}
+    generic_supported_decode_methods = {"numpy", "tobytes", "data"}
+    jpeg_png_supported_decode_methods = {"numpy", "tobytes", "pil", "data"}
+    json_list_supported_decode_methods = {"numpy", "data"}
     for tensor_name, decode_method in decode_method.items():
         if tensor_name not in all_tensor_keys:
             raise ValueError(
-                f"decode_method tensor {tensor_name} not found in tensors."
+                "tensor {tensor_name} specified in decode_method not found in tensors."
             )
         if tensor_name in jpeg_png_compressed_tensors_set:
             if decode_method not in jpeg_png_supported_decode_methods:
                 raise ValueError(
                     f"decode_method {decode_method} not supported for tensor {tensor_name}. Supported methods for this tensor are {jpeg_png_supported_decode_methods}"
                 )
         elif tensor_name in json_list_tensors_set:
@@ -139,9 +153,93 @@
             raise ValueError(
                 f"decode_method {decode_method} not supported for tensor {tensor_name}. Supported methods for this tensor are {generic_supported_decode_methods}"
             )
         if decode_method == "tobytes":
             raw_tensors.append(tensor_name)
         elif decode_method == "pil":
             pil_compressed_tensors.append(tensor_name)
+        elif decode_method == "data":
+            data_tensors.append(tensor_name)
+    return raw_tensors, pil_compressed_tensors, json_tensors, list_tensors, data_tensors
+
+
+def find_additional_tensors_and_info(dataset, data_tensors):
+    sample_info_htypes = {
+        "image",
+        "image.rgb",
+        "image.gray",
+        "dicom",
+        "nifti",
+        "point_cloud",
+        "mesh",
+        "video",
+    }
+    tensor_info_htypes = {"class_label"}
+
+    sample_info_tensors = set()
+    tensor_info_tensors = set()
+    for tensor_name in data_tensors:
+        tensor = dataset._get_tensor_from_root(tensor_name)
+        htype = tensor.htype
+        if htype in sample_info_htypes:
+            info_tensor_name = get_sample_info_tensor_key(tensor_name)
+            if tensor._sample_info_tensor:
+                sample_info_tensors.add(info_tensor_name)
+        if htype in tensor_info_htypes:
+            tensor_info_tensors.add(tensor_name)
+        if htype == "video":
+            raise NotImplementedError(
+                "data decode method for video tensors isn't supported yet."
+            )
+    return sample_info_tensors, tensor_info_tensors
+
+
+def get_htype_ndim_tensor_info_dicts(dataset, data_tensors, tensor_info_tensors):
+    htype_dict = {}
+    ndim_dict = {}
+    tensor_info_dict = {}
+    for tensor_name in data_tensors:
+        tensor = dataset._get_tensor_from_root(tensor_name)
+        htype_dict[tensor_name] = tensor.htype
+        ndim_dict[tensor_name] = tensor.ndim
+        if tensor_name in tensor_info_tensors:
+            tensor_info_dict[tensor_name] = tensor.info._info
+    return htype_dict, ndim_dict, tensor_info_dict
+
+
+def convert_sample_to_data(sample: dict, htype_dict, ndim_dict, tensor_info_dict):
+    for tensor_name in htype_dict.keys():
+        value = sample[tensor_name]
+        htype = htype_dict[tensor_name]
+        ndim = ndim_dict[tensor_name]
+        tensor_info = tensor_info_dict.get(tensor_name)
+        sample_info = sample.pop(get_sample_info_tensor_key(tensor_name), None)
+        sample[tensor_name] = convert_value_to_data(
+            value, tensor_info, sample_info, htype, ndim
+        )
+
 
-    return raw_tensors, pil_compressed_tensors, json_tensors, list_tensors
+def convert_value_to_data(value, tensor_info, sample_info, htype, ndim):
+    if htype in {"text", "json"}:
+        if not isinstance(value, str):
+            value = value[0]
+        return {"value": value}
+    elif htype == "video":
+        raise NotImplementedError
+    if htype == "class_label":
+        labels = value
+        data = {"value": labels}
+        class_names = tensor_info.get("class_names") if tensor_info else None
+        if class_names:
+            data["text"] = convert_to_text(labels, class_names)
+        return data
+    if htype in ("image", "image.rgb", "image.gray", "dicom", "nifti"):
+        return {
+            "value": value,
+            "sample_info": sample_info[0] or {},
+        }
+    elif htype == "point_cloud":
+        return parse_point_cloud_to_dict(value, ndim, sample_info)
+    elif htype == "mesh":
+        return parse_mesh_to_dict(value, sample_info)
+    else:
+        return {"value": value}
```

### Comparing `deeplake-3.3.2/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.4.0/deeplake/integrations/pytorch/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,22 @@
         return tensor.astype(np.int64)
     if tensor.dtype == np.uint64:
         return tensor.astype(np.int64)
     return None  # if not casted, calling method might want to make a copy.
 
 
 def copy_tensor(x):
+    if isinstance(x, dict):
+        return x.copy()
     if isinstance(x, Sample):
         x = x.array
     if isinstance(x, Image.Image):
         return x
+    if isinstance(x, str):
+        return x
 
     try:
         copy = cast_type(x)
     except AttributeError:
         return bytes(x)
     if copy is None:
         copy = x.copy()
@@ -125,14 +129,15 @@
 
         streaming = SampleStreaming(
             dataset,
             tensors=self.tensors,  # type: ignore
             use_local_cache=use_local_cache,
             pad_tensors=self.pad_tensors,
             decode_method=self.decode_method,
+            verbose=False,
         )
 
         self.schedules: List[Schedule] = self.scheduler.schedule(
             streaming.list_blocks()
         )
 
     def __iter__(self):
```

### Comparing `deeplake-3.3.2/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.4.0/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.4.0/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/tf/common.py` & `deeplake-3.4.0/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.4.0/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.4.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/integrations/wandb/wandb.py` & `deeplake-3.4.0/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/tests/cache_fixtures.py` & `deeplake-3.4.0/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/tests/client_fixtures.py` & `deeplake-3.4.0/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/tests/common.py` & `deeplake-3.4.0/deeplake/tests/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,7 +135,16 @@
         self.name = name
 
     def __enter__(self):
         _register_link_transform(self.name, self.func)
 
     def __exit__(self, *args, **kwargs):
         _unregister_link_transform(self.name)
+
+
+def convert_data_according_to_torch_version(batch):
+    import torch
+
+    if torch.__version__ < "2.0.0":
+        return batch[0]
+    else:
+        return batch
```

### Comparing `deeplake-3.3.2/deeplake/tests/dataset_fixtures.py` & `deeplake-3.4.0/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/tests/path_fixtures.py` & `deeplake-3.4.0/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/tests/storage_fixtures.py` & `deeplake-3.4.0/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/access_method.py` & `deeplake-3.4.0/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/agreement.py` & `deeplake-3.4.0/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/array_list.py` & `deeplake-3.4.0/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/assert_byte_indexes.py` & `deeplake-3.4.0/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/auto.py` & `deeplake-3.4.0/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/bugout_reporter.py` & `deeplake-3.4.0/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/cache_chain.py` & `deeplake-3.4.0/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/casting.py` & `deeplake-3.4.0/deeplake/util/casting.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 
 def get_htype(val: Union[np.ndarray, Sequence, Sample]) -> str:
     """Get the htype of a non-uniform mixed dtype sequence of samples."""
     if isinstance(val, deeplake.core.tensor.Tensor):
         return val.meta.htype
     if hasattr(val, "shape"):  # covers numpy arrays, numpy scalars and hub samples.
         return "generic"
-    if isinstance(val, List) and len(val) > 0 and isinstance(val[0], LinkedSample):
+    if (
+        isinstance(val, list)
+        and len(val) > 0
+        and isinstance(val[0], (Sample, LinkedSample))
+    ):
         return "generic"
     types = set((map(type, val)))  # type: ignore
     if dict in types:
         return "json"
     if types == set((str,)):
         return "text"
     if object in [  # type: ignore
```

### Comparing `deeplake-3.3.2/deeplake/util/check_latest_version.py` & `deeplake-3.4.0/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/chunk_engine.py` & `deeplake-3.4.0/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/class_label.py` & `deeplake-3.4.0/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/compute.py` & `deeplake-3.4.0/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/connect_dataset.py` & `deeplake-3.4.0/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/dataset.py` & `deeplake-3.4.0/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/diff.py` & `deeplake-3.4.0/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/downsample.py` & `deeplake-3.4.0/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/encoder.py` & `deeplake-3.4.0/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/exceptions.py` & `deeplake-3.4.0/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/exif.py` & `deeplake-3.4.0/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/from_tfds.py` & `deeplake-3.4.0/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/htype.py` & `deeplake-3.4.0/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/image.py` & `deeplake-3.4.0/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/invalid_view_op.py` & `deeplake-3.4.0/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/iteration_warning.py` & `deeplake-3.4.0/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/json.py` & `deeplake-3.4.0/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/keys.py` & `deeplake-3.4.0/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/link.py` & `deeplake-3.4.0/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/logging.py` & `deeplake-3.4.0/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/merge.py` & `deeplake-3.4.0/deeplake/util/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,15 @@
     conflict_tensors = set()
     idxs = {
         tensor_name: find_new_updated_and_conflict_indexes(
             tensor_name, dataset, target_dataset, nodes
         )
         for tensor_name in tensor_names
     }
+
     all_new_idxs = set()
     for new_idxs, _, _ in idxs.values():
         all_new_idxs.update(new_idxs)
     for idx in all_new_idxs:
         non_pad_found = False
         for tensor_name in tensor_names:
             target_engine = target_dataset[tensor_name].chunk_engine
@@ -433,14 +434,17 @@
         - updated_indexes is a list of tuples of the form (original_idx, target_idx)
         - conflict_indexes is a list of tuples of the form (original_idx, target_idx)
     """
     id_tensor_name = get_sample_id_tensor_key(tensor_name)
     target_id_tensor = target_dataset[id_tensor_name]
     original_id_tensor = dataset[id_tensor_name]
 
+    commit_diff = dataset[tensor_name].chunk_engine.commit_diff
+    deleted_samples = commit_diff.data_deleted_ids if commit_diff else set()
+
     original_node = nodes["original"]
     target_node = nodes["target"]
     lca_node = nodes["lca"]
 
     target_id_changes_commit_map = get_changes_commit_ids_for_node(
         target_dataset, tensor_name, target_node, lca_node
     )
@@ -452,19 +456,18 @@
     original_ids = original_id_tensor.numpy().flatten()
     original_id_to_index_map = {id: idx for idx, id in enumerate(original_ids)}
 
     target_ids = target_id_tensor.numpy().flatten()
     target_id_to_index_map = {id: idx for idx, id in enumerate(target_ids)}
 
     new_elements_ids = set(target_ids) - set(original_ids)
-
+    new_elements_ids = new_elements_ids - deleted_samples
     new_indexes = get_indexes_from_ids(
         new_elements_ids, target_id_changes_commit_map, target_id_to_index_map
     )
-
     conflict_indexes: List[Tuple[int, int]] = []
     updated_indexes: List[Tuple[int, int]] = []
     updated_indexes, conflict_indexes = find_updated_and_conflicts(
         original_id_changes_commit_map,
         target_id_changes_commit_map,
         original_id_to_index_map,
         target_id_to_index_map,
```

### Comparing `deeplake-3.3.2/deeplake/util/modified.py` & `deeplake-3.4.0/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/notebook.py` & `deeplake-3.4.0/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/mesh.py` & `deeplake-3.4.0/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.4.0/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.4.0/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.4.0/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.4.0/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.4.0/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.4.0/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.4.0/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.4.0/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.4.0/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/path.py` & `deeplake-3.4.0/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/pretty_print.py` & `deeplake-3.4.0/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/remove_cache.py` & `deeplake-3.4.0/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/scheduling.py` & `deeplake-3.4.0/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/shape_interval.py` & `deeplake-3.4.0/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/spinner.py` & `deeplake-3.4.0/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/split.py` & `deeplake-3.4.0/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/storage.py` & `deeplake-3.4.0/deeplake/util/storage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from deeplake.core.storage.gcs import GCSProvider
 from deeplake.util.agreement import handle_dataset_agreements
 from deeplake.util.cache_chain import generate_chain
 from deeplake.constants import LOCAL_CACHE_PREFIX, MB
 from deeplake.util.exceptions import AgreementNotAcceptedError
 from deeplake.util.tag import process_hub_path
-from typing import Optional
+from typing import Optional, Union
 from deeplake.core.storage.provider import StorageProvider
 import os
 from deeplake.core.storage import (
     LocalProvider,
     S3Provider,
     MemoryProvider,
     GDriveProvider,
@@ -16,101 +16,113 @@
 from deeplake.client.client import DeepLakeBackendClient
 import posixpath
 from deeplake.constants import DEFAULT_READONLY
 
 
 def storage_provider_from_path(
     path: str,
-    creds: Optional[dict],
+    creds: Optional[Union[dict, str]] = None,
     read_only: bool = False,
     token: Optional[str] = None,
     is_hub_path: bool = False,
+    db_engine: bool = False,
 ):
     """Construct a StorageProvider given a path.
 
     Arguments:
         path (str): The full path to the Dataset.
         creds (dict): A dictionary containing credentials used to access the dataset at the url.
             This takes precedence over credentials present in the environment. Only used when url is provided. Currently only works with s3 urls.
         read_only (bool): Opens dataset in read only mode if this is passed as True. Defaults to False.
         token (str): token for authentication into activeloop.
-        is_hub_path (bool): whether the path points to a Deep Lake dataset.
+        is_hub_path (bool): Whether the path points to a Deep Lake dataset.
+        db_engine (bool): Whether to use Activeloop DB Engine. Only applicable for hub:// paths.
 
     Returns:
         If given a path starting with s3:// returns the S3Provider.
         If given a path starting with gcp:// or gcs:// returns the GCPProvider.
         If given a path starting with gdrive:// returns the GDriveProvider
         If given a path starting with mem:// returns the MemoryProvider.
         If given a path starting with hub:// returns the underlying cloud Provider.
         If given a valid local path, returns the LocalProvider.
 
     Raises:
         ValueError: If the given path is a local path to a file.
     """
     if creds is None:
         creds = {}
-    if path.startswith("s3://"):
-        key = creds.get("aws_access_key_id")
-        secret = creds.get("aws_secret_access_key")
-        session_token = creds.get("aws_session_token")
-        endpoint_url = creds.get("endpoint_url")
-        region = creds.get("aws_region") or creds.get("region")
-        profile = creds.get("profile_name")
-        storage: StorageProvider = S3Provider(
-            path,
-            key,
-            secret,
-            session_token,
-            endpoint_url,
-            region,
-            profile_name=profile,
-            token=token,
+    if path.startswith("hub://"):
+        storage: StorageProvider = storage_provider_from_hub_path(
+            path, read_only, db_engine=db_engine, token=token, creds=creds
         )
-    elif (
-        path.startswith("gcp://")
-        or path.startswith("gcs://")
-        or path.startswith("gs://")
-    ):
-        storage = GCSProvider(path, creds)
-    elif path.startswith("gdrive://"):
-        storage = GDriveProvider(path, creds)
-    elif path.startswith("mem://"):
-        storage = MemoryProvider(path)
-    elif path.startswith("hub://"):
-        storage = storage_provider_from_hub_path(path, read_only, token=token)
     else:
-        if not os.path.exists(path) or os.path.isdir(path):
-            storage = LocalProvider(path)
+        if isinstance(creds, str):
+            creds = {}
+        if path.startswith("s3://"):
+            key = creds.get("aws_access_key_id")
+            secret = creds.get("aws_secret_access_key")
+            session_token = creds.get("aws_session_token")
+            endpoint_url = creds.get("endpoint_url")
+            region = creds.get("aws_region") or creds.get("region")
+            profile = creds.get("profile_name")
+            storage = S3Provider(
+                path,
+                key,
+                secret,
+                session_token,
+                endpoint_url,
+                region,
+                profile_name=profile,
+                token=token,
+            )
+        elif (
+            path.startswith("gcp://")
+            or path.startswith("gcs://")
+            or path.startswith("gs://")
+        ):
+            storage = GCSProvider(path, creds)
+        elif path.startswith("gdrive://"):
+            storage = GDriveProvider(path, creds)
+        elif path.startswith("mem://"):
+            storage = MemoryProvider(path)
         else:
-            raise ValueError(f"Local path {path} must be a path to a local directory")
+            if not os.path.exists(path) or os.path.isdir(path):
+                storage = LocalProvider(path)
+            else:
+                raise ValueError(
+                    f"Local path {path} must be a path to a local directory"
+                )
     if not storage._is_hub_path:
         storage._is_hub_path = is_hub_path
 
     if read_only:
         storage.enable_readonly()
     return storage
 
 
 def storage_provider_from_hub_path(
-    path: str, read_only: bool = False, token: Optional[str] = None
+    path: str,
+    read_only: bool = False,
+    db_engine: bool = False,
+    token: Optional[str] = None,
+    creds: Optional[Union[dict, str]] = None,
 ):
     path, org_id, ds_name, subdir = process_hub_path(path)
     client = DeepLakeBackendClient(token=token)
 
     mode = "r" if read_only else None
-
     # this will give the proper url (s3, gcs, etc) and corresponding creds, depending on where the dataset is stored.
     try:
-        url, creds, mode, expiration = client.get_dataset_credentials(
-            org_id, ds_name, mode=mode
+        url, final_creds, mode, expiration, repo = client.get_dataset_credentials(
+            org_id, ds_name, mode=mode, db_engine={"enabled": db_engine}
         )
     except AgreementNotAcceptedError as e:
         handle_dataset_agreements(client, e.agreements, org_id, ds_name)
-        url, creds, mode, expiration = client.get_dataset_credentials(
-            org_id, ds_name, mode=mode
+        url, final_creds, mode, expiration, repo = client.get_dataset_credentials(
+            org_id, ds_name, mode=mode, db_engine={"enabled": db_engine}
         )
 
     if mode == "r":
         read_only = True
         if read_only is None and not DEFAULT_READONLY:
             # warns user about automatic mode change
             print(
@@ -118,41 +130,73 @@
             )
 
     if read_only is None:
         read_only = DEFAULT_READONLY
 
     url = posixpath.join(url, subdir)
 
+    creds_used = "PLATFORM"
+    if url.startswith("s3://"):
+        if creds == "ENV":
+            final_creds = {}
+            creds_used = "ENV"
+        elif isinstance(creds, dict) and set(creds.keys()) == {"profile_name"}:
+            final_creds = creds
+            creds_used = "ENV"
+        elif isinstance(creds, dict) and bool(creds):
+            final_creds = creds
+            creds_used = "DICT"
+
+    if creds_used != "PLATFORM":
+        msg = "Overriding platform credentials with"
+        if creds_used == "ENV":
+            msg += " credentials loaded from environment."
+        elif creds_used == "DICT":
+            msg += " credentials from user passed dictionary."
+        print(msg)
+
     storage = storage_provider_from_path(
-        path=url, creds=creds, read_only=read_only, is_hub_path=True, token=token
+        path=url, creds=final_creds, read_only=read_only, is_hub_path=True, token=token
     )
-    storage._set_hub_creds_info(path, expiration)
+    storage.creds_used = creds_used
+    if creds_used == "PLATFORM":
+        storage._set_hub_creds_info(path, expiration, db_engine, repo)
+
     return storage
 
 
 def get_storage_and_cache_chain(
-    path, read_only, creds, token, memory_cache_size, local_cache_size
+    path,
+    read_only,
+    creds,
+    token,
+    memory_cache_size,
+    local_cache_size,
+    db_engine=False,
 ):
     """
     Returns storage provider and cache chain for a given path, according to arguments passed.
 
     Args:
         path (str): The full path to the Dataset.
         creds (dict): A dictionary containing credentials used to access the dataset at the url.
             This takes precedence over credentials present in the environment. Only used when url is provided. Currently only works with s3 urls.
         read_only (bool): Opens dataset in read only mode if this is passed as True. Defaults to False.
         token (str): token for authentication into activeloop
         memory_cache_size (int): The size of the in-memory cache to use.
         local_cache_size (int): The size of the local cache to use.
+        db_engine (bool): Whether to use Activeloop DB Engine, only applicable for hub:// paths.
 
     Returns:
         A tuple of the storage provider and the storage chain.
     """
+
     storage = storage_provider_from_path(
         path=path,
+        db_engine=db_engine,
         creds=creds,
         read_only=read_only,
         token=token,
     )
     memory_cache_size_bytes = memory_cache_size * MB
     local_cache_size_bytes = local_cache_size * MB
     storage_chain = generate_chain(
```

### Comparing `deeplake-3.3.2/deeplake/util/tag.py` & `deeplake-3.4.0/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/testing.py` & `deeplake-3.4.0/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/tests/test_auto.py` & `deeplake-3.4.0/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.4.0/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.4.0/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/tests/test_read.py` & `deeplake-3.4.0/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.4.0/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/tests/test_split.py` & `deeplake-3.4.0/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/tests/test_version_control.py` & `deeplake-3.4.0/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/transform.py` & `deeplake-3.4.0/deeplake/util/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from deeplake.core.index import Index
 from deeplake.core.tensor import Tensor
 
 from deeplake.constants import (
     MB,
     TRANSFORM_PROGRESSBAR_UPDATE_INTERVAL,
     TRANSFORM_RECHUNK_AVG_SIZE_BOUND,
+    TRANSFORM_CHUNK_CACHE_SIZE,
 )
 from deeplake.util.dataset import try_flushing
 from deeplake.util.remove_cache import (
     get_base_storage,
     get_dataset_with_zero_size_cache,
 )
 from deeplake.util.keys import get_tensor_meta_key
@@ -335,27 +336,28 @@
     link_creds,
 ) -> Dict[str, ChunkEngine]:
     """Creates chunk engines corresponding to each storage for all tensors.
     These are created separately for each worker for parallel uploads.
     """
     all_chunk_engines: Dict[str, ChunkEngine] = {}
     num_tries = 1000
+    storage_cache = LRUCache(
+        MemoryProvider(), output_storage, TRANSFORM_CHUNK_CACHE_SIZE
+    )
+    storage_cache.autoflush = False
+    # TODO: replace this with simply a MemoryProvider once we get rid of cachable
+    memory_cache = LRUCache(
+        MemoryProvider(),
+        MemoryProvider(),
+        64 * MB,
+    )
+    memory_cache.autoflush = False
     for tensor in tensors:
         for i in range(num_tries):
             try:
-                # TODO: replace this with simply a MemoryProvider once we get rid of cachable
-                memory_cache = LRUCache(
-                    MemoryProvider(),
-                    MemoryProvider(),
-                    64 * MB,
-                )
-                memory_cache.autoflush = False
-                storage_cache = LRUCache(MemoryProvider(), output_storage, 64 * MB)
-                storage_cache.autoflush = False
-
                 # this chunk engine is used to retrieve actual tensor meta and chunk_size
                 storage_chunk_engine = ChunkEngine(tensor, storage_cache, version_state)
                 existing_meta = storage_chunk_engine.tensor_meta
 
                 chunk_size = storage_chunk_engine.max_chunk_size
                 tiling_threshold = storage_chunk_engine.tiling_threshold
                 new_tensor_meta = TensorMeta(
```

### Comparing `deeplake-3.3.2/deeplake/util/version_control.py` & `deeplake-3.4.0/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/util/video.py` & `deeplake-3.4.0/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/visualizer/video_streaming.py` & `deeplake-3.4.0/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake/visualizer/visualizer.py` & `deeplake-3.4.0/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake.egg-info/PKG-INFO` & `deeplake-3.4.0/deeplake.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.3.2
+Version: 3.4.0
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: audio
 Provides-Extra: av
 Provides-Extra: dicom
+Provides-Extra: enterprise
 Provides-Extra: gcp
 Provides-Extra: gdrive
 Provides-Extra: medical
 Provides-Extra: point_cloud
 Provides-Extra: video
 Provides-Extra: visualizer
 License-File: LICENSE
 
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
      <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
 </h1>
     </br>
-    <h1 align="center">Deep Lake: Data Lake for Deep Learning
+    <h1 align="center">Deep Lake: Vector Database for any AI data
  </h1>
 <p align="center">
     <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
     <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
     <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
      <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
      </a>
@@ -51,15 +52,17 @@
  </h3>
  
 
 *Read this in other languages: [简体中文](README.zh-cn.md)*
 
 ## About Deep Lake
 
-Deep Lake (formerly known as Activeloop Hub) is a data lake for deep learning applications. Our open-source dataset format is optimized for rapid streaming and querying of data while training models at scale, and it includes a simple API for creating, storing, and collaborating on AI datasets of any size. It can be deployed locally or in the cloud, and it enables you to store all of your data in one place, ranging from simple annotations to large videos. Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake includes the following features:
+Deep Lake is a Vector Database powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights and Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Google, Intel, Waymo, Matterport, Red Cross, Yale, & Oxford. 
+
+Deep Lake includes the following features:
 
 <details>
   <summary><b>Storage Agnostic API</b></summary>
 Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
 </details>
 <details>
   <summary><b>Native Compression with Lazy NumPy-like Indexing</b></summary>
@@ -70,16 +73,16 @@
 Commits, branches, checkout - Concepts you are already familiar with in your code repositories can now be applied to your datasets as well!
 </details>
 <details>
   <summary><b>Dataloaders for Popular Deep Learning Frameworks</b></summary>
 Deep Lake comes with built-in dataloaders for Pytorch and Tensorflow. Train your model with a few lines of code - we even take care of dataset shuffling. :)
 </details>
 <details>
-  <summary><b>Integrations with Popular Tools</b></summary>
-Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
+  <summary><b>Integrations with Powerful Tools</b></summary>
+Deep Lake has integrations with <a href="https://github.com/hwchase17/langchain">Langchain</a> and <a href="https://github.com/jerryjliu/llama_index">LLamaIndex</a> as a vector store for LLM apps, <a href="https://wandb.ai/">Weights & Biases</a> for data lineage during model training, and <a href="https://github.com/open-mmlab/mmdetection">MMDetection</a> for training object detection models.
 </details>
 <details>
   <summary><b>Distributed Transformations</b></summary>
 Rapidly apply transformations on your datasets using multi-threading, multi-processing, or our built-in <a href="https://www.ray.io/">Ray</a> integration.</details>
 <details>
   <summary><b>100+ most-popular image, video, and audio datasets available in seconds</b></summary>
 Deep Lake community has uploaded <a href="https://docs.activeloop.ai/datasets/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">100+ image, video and audio datasets</a> like <a href="https://docs.activeloop.ai/datasets/mnist/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">MNIST</a>, <a href="https://docs.activeloop.ai/datasets/coco-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">COCO</a>,  <a href="https://docs.activeloop.ai/datasets/imagenet-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">ImageNet</a>,  <a href="https://docs.activeloop.ai/datasets/cifar-10-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">CIFAR</a>,  <a href="https://docs.activeloop.ai/datasets/gtzan-genre-dataset/?utm_source=github&utm_medium=github&utm_campaign=github_readme&utm_id=readme">GTZAN</a> and others.
@@ -300,14 +303,36 @@
 | Storage for public datasets hosted by Activeloop     | 200GB Free    |
 | Storage for private datasets hosted by Activeloop    | 100GB Free    |
 
 
 
 ## 👩‍💻 Comparisons to Familiar Tools
 
+<details>
+  <summary><b>Deep Lake vs Chroma </b></summary>
+  
+Both Deep Lake & ChromaDB enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are architecturally very different. ChromaDB is a Vector Database that can be deployed locally or on a server using Docker and will offer a hosted solution shortly. Deep Lake is a serverless Vector Store deployed on the user’s own cloud, locally, or in-memory. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike ChromaDB, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. ChromaDB is limited to light metadata on top of the embeddings and has no visualization. Deep Lake datasets can be visualized and version controlled. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
+
+<details>
+  <summary><b>Deep Lake vs Pinecone</b></summary>
+  
+Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring serach for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
+<details>
+  <summary><b>Deep Lake vs Weaviate</b></summary>
+  
+Both Deep Lake and Weaviate enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Weaviate is a Vector Database that can be deployed in a managed service or by the user via Kubernetes or Docker. Deep Lake is serverless. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike Weaviate, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Weaviate is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+
+</details>
+
 
 <details>
   <summary><b>Deep Lake vs DVC</b></summary>
   
 Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
 
 </details>
```

#### html2text {}

```diff
@@ -1,53 +1,57 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.3.2 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.4.0 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
-Provides-Extra: gcp Provides-Extra: gdrive Provides-Extra: medical Provides-
-Extra: point_cloud Provides-Extra: video Provides-Extra: visualizer License-
-File: LICENSE [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-
-f711c4d35b82]
+Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
+Extra: medical Provides-Extra: point_cloud Provides-Extra: video Provides-
+Extra: visualizer License-File: LICENSE [https://static.scarf.sh/a.png?x-
+pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
-             ****** Deep Lake: Data Lake for Deep Learning ******
+           ****** Deep Lake: Vector Database for any AI data ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
-Lake Deep Lake (formerly known as Activeloop Hub) is a data lake for deep
-learning applications. Our open-source dataset format is optimized for rapid
-streaming and querying of data while training models at scale, and it includes
-a simple API for creating, storing, and collaborating on AI datasets of any
-size. It can be deployed locally or in the cloud, and it enables you to store
-all of your data in one place, ranging from simple annotations to large videos.
-Deep Lake is used by Google, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep
-Lake includes the following features:  Storage Agnostic API Use one API to
-upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
-GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
-like Indexing Store images, audios and videos in their native compression.
-Slide, index, iterate and interact with your data like a collection of NumPy
-arrays in your system's memory. Deep Lake lazily loads data only when needed,
-e.g., when training a model.   Dataset Version Control Commits, branches,
-checkout - Concepts you are already familiar with in your code repositories can
-now be applied to your datasets as well!   Dataloaders for Popular Deep
-Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+Lake Deep Lake is a Vector Database powered by a unique storage format
+optimized for deep-learning and Large Language Model (LLM) based applications.
+It simplifies the deployment of enterprise-grade LLM-based products by offering
+storage for all data types (embeddings, audio, text, videos, images, pdfs,
+annotations, etc.), querying and vector search, data streaming while training
+models at scale, data versioning and lineage for all workloads, and
+integrations with popular tools such as LangChain, LlamaIndex, Weights and
+Biases, and many more. Deep Lake works with data of any size, it is serverless,
+and it enables you to store all of your data in once place. Deep Lake is used
+by Google, Intel, Waymo, Matterport, Red Cross, Yale, & Oxford. Deep Lake
+includes the following features:  Storage Agnostic API Use one API to upload,
+download, and stream datasets to/from AWS S3/S3-compatible storage, GCP,
+Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-like
+Indexing Store images, audios and videos in their native compression. Slide,
+index, iterate and interact with your data like a collection of NumPy arrays in
+your system's memory. Deep Lake lazily loads data only when needed, e.g., when
+training a model.   Dataset Version Control Commits, branches, checkout -
+Concepts you are already familiar with in your code repositories can now be
+applied to your datasets as well!   Dataloaders for Popular Deep Learning
+Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
 Tensorflow. Train your model with a few lines of code - we even take care of
-dataset shuffling. :)   Integrations with Popular Tools Deep Lake has
-integrations with Langchain as a vector store for LLM apps, Weights_&_Biases
-for data lineage during model training, and MMDetection for training object
-detection models.   Distributed Transformations Rapidly apply transformations
-on your datasets using multi-threading, multi-processing, or our built-in Ray
-integration.  100+ most-popular image, video, and audio datasets available in
-seconds Deep Lake community has uploaded 100+_image,_video_and_audio_datasets
-like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.    Instant Visualization
-Support in Activeloop_Platform Deep Lake datasets are instantly visualized with
-bounding boxes, masks, annotations, etc. in Deep_Lake_Visualizer (see below).
+dataset shuffling. :)   Integrations with Powerful Tools Deep Lake has
+integrations with Langchain and LLamaIndex as a vector store for LLM apps,
+Weights_&_Biases for data lineage during model training, and MMDetection for
+training object detection models.   Distributed Transformations Rapidly apply
+transformations on your datasets using multi-threading, multi-processing, or
+our built-in Ray integration.  100+ most-popular image, video, and audio
+datasets available in seconds Deep Lake community has uploaded 100+_image,
+video_and_audio_datasets like MNIST, COCO, ImageNet, CIFAR, GTZAN and others.
+Instant Visualization Support in Activeloop_Platform Deep Lake datasets are
+instantly visualized with bounding boxes, masks, annotations, etc. in Deep_Lake
+Visualizer (see below).
                   [https://www.linkpicture.com/q/ReadMe.gif]
 ## ð Performance Deep Lake's efficient enterprise dataloaders built in C++
 speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et al. 2022,
 Hambardzumyan et al. 2023)
                    [docs/source/_static/img/benchmarks.png]
 ## Getting Started with Deep Lake ### ð How to install Deep Lake Deep Lake's
 core is efficiently built in C++ and can be quickly installed using pip. ```sh
@@ -139,17 +143,50 @@
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
 Platform. Users can also create and store their own datasets and make them
 available to the public. Free storage of up to 300 GB is available for students
 and educators: |  |  | | ---------------------------------------------------- |
 ------------- | | Storage for public datasets hosted by Activeloop | 200GB Free
 | | Storage for private datasets hosted by Activeloop | 100GB Free | ##
-ð©âð» Comparisons to Familiar Tools  Deep Lake vs DVC Deep Lake and DVC
-offer dataset version control similar to git for data, but their methods for
-storing data differ significantly. Deep Lake converts and stores data as
+ð©âð» Comparisons to Familiar Tools  Deep Lake vs Chroma Both Deep Lake &
+ChromaDB enable users to store and search vectors (embeddings) and offer
+integrations with LangChain and LlamaIndex. However, they are architecturally
+very different. ChromaDB is a Vector Database that can be deployed locally or
+on a server using Docker and will offer a hosted solution shortly. Deep Lake is
+a serverless Vector Store deployed on the userâs own cloud, locally, or in-
+memory. All computations run client-side, which enables users to support
+lightweight production apps in seconds. Unlike ChromaDB, Deep Lakeâs data
+format can store raw data such as images, videos, and text, in addition to
+embeddings. ChromaDB is limited to light metadata on top of the embeddings and
+has no visualization. Deep Lake datasets can be visualized and version
+controlled. Deep Lake also has a performant dataloader for fine-tuning your
+Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
+enable users to store and search vectors (embeddings) and offer integrations
+with LangChain and LlamaIndex. However, they are architecturally very
+different. Pinecone is a fully-managed Vector Database that is optimized for
+highly demanding applications requiring serach for billions of vectors. Deep
+Lake is a serverless. All computations run client-side, which enables users to
+get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
+raw data such as images, videos, and text, in addition to embeddings. Deep Lake
+datasets can be visualized and version controlled. Pinecone is limited to light
+metadata on top of the embeddings and has no visualization. Deep Lake also has
+a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
+vs Weaviate Both Deep Lake and Weaviate enable users to store and search
+vectors (embeddings) and offer integrations with LangChain and LlamaIndex.
+However, they are architecturally very different. Weaviate is a Vector Database
+that can be deployed in a managed service or by the user via Kubernetes or
+Docker. Deep Lake is serverless. All computations run client-side, which
+enables users to support lightweight production apps in seconds. Unlike
+Weaviate, Deep Lakeâs data format can store raw data such as images, videos,
+and text, in addition to embeddings. Deep Lake datasets can be visualized and
+version controlled. Weaviate is limited to light metadata on top of the
+embeddings and has no visualization. Deep Lake also has a performant dataloader
+for fine-tuning your Large Language Models.   Deep Lake vs DVC Deep Lake and
+DVC offer dataset version control similar to git for data, but their methods
+for storing data differ significantly. Deep Lake converts and stores data as
 chunked compressed arrays, which enables rapid streaming to ML models, whereas
 DVC operates on top of data stored in less efficient traditional file
 structures. The Deep Lake format makes dataset versioning significantly easier
 compared to traditional file structures by DVC when datasets are composed of
 many files (i.e., many images). An additional distinction is that DVC primarily
 uses a command-line interface, whereas Deep Lake is a Python package. Lastly,
 Deep Lake offers an API to easily connect datasets to ML frameworks and other
```

### Comparing `deeplake-3.3.2/deeplake.egg-info/SOURCES.txt` & `deeplake-3.4.0/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.3.2/deeplake.egg-info/requires.txt` & `deeplake-3.4.0/deeplake.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 IPython
 flask
 google-api-python-client~=2.31.0
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
 laspy
+libdeeplake==0.0.51
 nibabel
 oauth2client~=4.1.3
 pydicom
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
@@ -37,14 +38,18 @@
 [av:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [dicom]
 nibabel
 pydicom
 
+[enterprise]
+libdeeplake==0.0.51
+pyjwt
+
 [gcp]
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
 
 [gdrive]
 google-api-python-client~=2.31.0
```

### Comparing `deeplake-3.3.2/setup.py` & `deeplake-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,35 +45,35 @@
     "point_cloud": ["laspy"],
 }
 
 
 def libdeeplake_availabe():
     py_ver = sys.version_info
     if sys.platform == "linux":
-        if py_ver >= (3, 6) and py_ver <= (3, 10):
+        if py_ver >= (3, 6) and py_ver <= (3, 11):
             return True
     if sys.platform == "darwin":
         mac_ver = list(map(int, platform.mac_ver()[0].split(".")))
         if (
             (mac_ver[0] > 10 or mac_ver[0] == 10 and mac_ver[1] >= 12)
             and py_ver >= (3, 7)
-            and py_ver <= (3, 10)
+            and py_ver <= (3, 11)
         ):
             return True
     return False
 
 
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_availabe():
-    libdeeplake = "libdeeplake==0.0.47"
+    libdeeplake = "libdeeplake==0.0.51"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
 
 
 def get_property(prop):
```

