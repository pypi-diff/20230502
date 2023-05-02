# Comparing `tmp/deeplabel-sdk-0.4.8.tar.gz` & `tmp/deeplabel-sdk-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplabel-sdk-0.4.8.tar", last modified: Mon Dec 19 11:03:31 2022, max compression
+gzip compressed data, was "deeplabel-sdk-0.4.9.tar", last modified: Wed Dec 28 12:41:07 2022, max compression
```

## Comparing `deeplabel-sdk-0.4.8.tar` & `deeplabel-sdk-0.4.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1033 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/PKG-INFO
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/README.md
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      232 2022-12-19 11:03:16.000000 deeplabel-sdk-0.4.8/deeplabel/__init__.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/auth/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       27 2022-11-02 10:15:59.000000 deeplabel-sdk-0.4.8/deeplabel/auth/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2143 2022-11-09 13:59:06.000000 deeplabel-sdk-0.4.8/deeplabel/auth/tokens.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1390 2022-11-09 13:37:54.000000 deeplabel-sdk-0.4.8/deeplabel/auth/users.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1272 2022-11-09 13:36:50.000000 deeplabel-sdk-0.4.8/deeplabel/basemodel.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     6693 2022-12-19 10:18:35.000000 deeplabel-sdk-0.4.8/deeplabel/client.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/contrib/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-11-02 10:16:14.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/__init__.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/contrib/downloaders/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-11-02 10:16:31.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/downloaders/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3813 2022-11-02 10:16:28.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/downloaders/frame_downloader.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     5759 2022-11-02 10:10:51.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/ava.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)    13822 2022-12-19 11:03:11.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/coco.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)    10748 2022-11-02 10:10:51.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/pascal_voc.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/contrib/importers/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/importers/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     8187 2022-09-06 08:27:47.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/importers/pascalvoc.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      814 2022-11-02 10:17:11.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/importers/utils.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1302 2022-12-12 09:27:26.000000 deeplabel-sdk-0.4.8/deeplabel/contrib/utils.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2302 2022-11-17 13:08:32.000000 deeplabel-sdk-0.4.8/deeplabel/exceptions.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/feedback/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/feedback/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3451 2022-11-02 10:17:19.000000 deeplabel-sdk-0.4.8/deeplabel/feedback/videos.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/infer/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/infer/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3353 2022-11-02 10:17:23.000000 deeplabel-sdk-0.4.8/deeplabel/infer/folders.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/infer/gallery/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3177 2022-12-19 10:59:04.000000 deeplabel-sdk-0.4.8/deeplabel/infer/gallery/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3662 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.8/deeplabel/infer/gallery/detections.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4286 2022-12-03 14:13:25.000000 deeplabel-sdk-0.4.8/deeplabel/infer/gallery/gallery_graphs.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     6374 2022-11-04 12:45:18.000000 deeplabel-sdk-0.4.8/deeplabel/infer/gallery/gallery_tasks.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2376 2022-12-19 10:41:21.000000 deeplabel-sdk-0.4.8/deeplabel/infer/gallery/images.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/infer/graphs/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2123 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/infer/graphs/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2556 2022-11-02 10:17:58.000000 deeplabel-sdk-0.4.8/deeplabel/infer/graphs/graph_edges.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2624 2022-11-02 10:18:03.000000 deeplabel-sdk-0.4.8/deeplabel/infer/graphs/graph_nodes.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1162 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/infer/notebooks.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      797 2022-12-19 10:40:29.000000 deeplabel-sdk-0.4.8/deeplabel/infer/presign.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      268 2022-11-02 10:17:27.000000 deeplabel-sdk-0.4.8/deeplabel/infer/types.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/infer/videos/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     5438 2022-11-29 13:49:27.000000 deeplabel-sdk-0.4.8/deeplabel/infer/videos/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3627 2022-11-02 10:18:11.000000 deeplabel-sdk-0.4.8/deeplabel/infer/videos/detections.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4109 2022-10-07 12:22:26.000000 deeplabel-sdk-0.4.8/deeplabel/infer/videos/video_graphs.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     8341 2022-11-04 09:20:37.000000 deeplabel-sdk-0.4.8/deeplabel/infer/videos/video_tasks.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/label/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-11-02 10:18:20.000000 deeplabel-sdk-0.4.8/deeplabel/label/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3126 2022-11-09 07:09:53.000000 deeplabel-sdk-0.4.8/deeplabel/label/dl_models.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3399 2022-12-19 05:19:11.000000 deeplabel-sdk-0.4.8/deeplabel/label/folders.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.967079 deeplabel-sdk-0.4.8/deeplabel/label/gallery/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4634 2022-11-02 10:19:03.000000 deeplabel-sdk-0.4.8/deeplabel/label/gallery/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2774 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.8/deeplabel/label/gallery/detections.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3323 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.8/deeplabel/label/gallery/images.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1420 2022-11-02 10:18:49.000000 deeplabel-sdk-0.4.8/deeplabel/label/label_maps.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2026 2022-11-02 10:18:56.000000 deeplabel-sdk-0.4.8/deeplabel/label/labels.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/deeplabel/label/videos/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     9738 2022-12-06 10:30:45.000000 deeplabel-sdk-0.4.8/deeplabel/label/videos/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3076 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.8/deeplabel/label/videos/detections.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2052 2022-11-02 10:19:33.000000 deeplabel-sdk-0.4.8/deeplabel/label/videos/frames.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2913 2022-11-02 10:19:37.000000 deeplabel-sdk-0.4.8/deeplabel/label/videos/video_tasks.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2083 2022-11-02 10:15:55.000000 deeplabel-sdk-0.4.8/deeplabel/projects.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/deeplabel/types/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/types/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4126 2022-11-17 12:50:08.000000 deeplabel-sdk-0.4.8/deeplabel/types/bounding_box.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      639 2022-11-02 10:19:44.000000 deeplabel-sdk-0.4.8/deeplabel/types/polygon.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/deeplabel/utils/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/utils/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      901 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.8/deeplabel/utils/videos.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1033 2022-12-19 11:03:31.000000 deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2056 2022-12-19 11:03:31.000000 deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        1 2022-12-19 11:03:31.000000 deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      139 2022-12-19 11:03:31.000000 deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/requires.txt
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       16 2022-12-19 11:03:31.000000 deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/top_level.txt
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       38 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/setup.cfg
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     8644 2022-12-19 11:03:16.000000 deeplabel-sdk-0.4.8/setup.py
-drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-19 11:03:31.971079 deeplabel-sdk-0.4.8/tests/
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.8/tests/__init__.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      339 2022-12-19 11:03:12.000000 deeplabel-sdk-0.4.8/tests/conftest.py
--rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      556 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.8/tests/test_project.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.701275 deeplabel-sdk-0.4.9/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1033 2022-12-28 12:41:07.701275 deeplabel-sdk-0.4.9/PKG-INFO
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/README.md
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.209276 deeplabel-sdk-0.4.9/deeplabel/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      232 2022-12-28 12:40:28.000000 deeplabel-sdk-0.4.9/deeplabel/__init__.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.249276 deeplabel-sdk-0.4.9/deeplabel/auth/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       27 2022-11-02 10:15:59.000000 deeplabel-sdk-0.4.9/deeplabel/auth/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2143 2022-11-09 13:59:06.000000 deeplabel-sdk-0.4.9/deeplabel/auth/tokens.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1390 2022-11-09 13:37:54.000000 deeplabel-sdk-0.4.9/deeplabel/auth/users.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1272 2022-11-09 13:36:50.000000 deeplabel-sdk-0.4.9/deeplabel/basemodel.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     6693 2022-12-19 10:18:35.000000 deeplabel-sdk-0.4.9/deeplabel/client.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.285276 deeplabel-sdk-0.4.9/deeplabel/contrib/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-11-02 10:16:14.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/__init__.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.297276 deeplabel-sdk-0.4.9/deeplabel/contrib/downloaders/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-11-02 10:16:31.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/downloaders/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3813 2022-11-02 10:16:28.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/downloaders/frame_downloader.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.341276 deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     5759 2022-11-02 10:10:51.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/ava.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)    13822 2022-12-28 12:40:27.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/coco.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)    10748 2022-11-02 10:10:51.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/pascal_voc.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.365276 deeplabel-sdk-0.4.9/deeplabel/contrib/importers/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/importers/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     8187 2022-09-06 08:27:47.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/importers/pascalvoc.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      814 2022-11-02 10:17:11.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/importers/utils.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1302 2022-12-12 09:27:26.000000 deeplabel-sdk-0.4.9/deeplabel/contrib/utils.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2302 2022-11-17 13:08:32.000000 deeplabel-sdk-0.4.9/deeplabel/exceptions.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.393276 deeplabel-sdk-0.4.9/deeplabel/feedback/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/feedback/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3451 2022-11-02 10:17:19.000000 deeplabel-sdk-0.4.9/deeplabel/feedback/videos.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.441276 deeplabel-sdk-0.4.9/deeplabel/infer/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/infer/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3353 2022-11-02 10:17:23.000000 deeplabel-sdk-0.4.9/deeplabel/infer/folders.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.497275 deeplabel-sdk-0.4.9/deeplabel/infer/gallery/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3177 2022-12-19 10:59:04.000000 deeplabel-sdk-0.4.9/deeplabel/infer/gallery/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3662 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.9/deeplabel/infer/gallery/detections.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4286 2022-12-03 14:13:25.000000 deeplabel-sdk-0.4.9/deeplabel/infer/gallery/gallery_graphs.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     6374 2022-11-04 12:45:18.000000 deeplabel-sdk-0.4.9/deeplabel/infer/gallery/gallery_tasks.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2376 2022-12-19 10:41:21.000000 deeplabel-sdk-0.4.9/deeplabel/infer/gallery/images.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.517275 deeplabel-sdk-0.4.9/deeplabel/infer/graphs/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2123 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/infer/graphs/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2556 2022-11-02 10:17:58.000000 deeplabel-sdk-0.4.9/deeplabel/infer/graphs/graph_edges.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2624 2022-11-02 10:18:03.000000 deeplabel-sdk-0.4.9/deeplabel/infer/graphs/graph_nodes.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1162 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/infer/notebooks.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      797 2022-12-19 10:40:29.000000 deeplabel-sdk-0.4.9/deeplabel/infer/presign.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      268 2022-11-02 10:17:27.000000 deeplabel-sdk-0.4.9/deeplabel/infer/types.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.545275 deeplabel-sdk-0.4.9/deeplabel/infer/videos/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     5438 2022-11-29 13:49:27.000000 deeplabel-sdk-0.4.9/deeplabel/infer/videos/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3627 2022-11-02 10:18:11.000000 deeplabel-sdk-0.4.9/deeplabel/infer/videos/detections.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4109 2022-10-07 12:22:26.000000 deeplabel-sdk-0.4.9/deeplabel/infer/videos/video_graphs.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     8341 2022-11-04 09:20:37.000000 deeplabel-sdk-0.4.9/deeplabel/infer/videos/video_tasks.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.577275 deeplabel-sdk-0.4.9/deeplabel/label/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       15 2022-11-02 10:18:20.000000 deeplabel-sdk-0.4.9/deeplabel/label/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3762 2022-12-27 09:34:26.000000 deeplabel-sdk-0.4.9/deeplabel/label/dl_models.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3399 2022-12-19 05:19:11.000000 deeplabel-sdk-0.4.9/deeplabel/label/folders.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.585275 deeplabel-sdk-0.4.9/deeplabel/label/gallery/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4634 2022-11-02 10:19:03.000000 deeplabel-sdk-0.4.9/deeplabel/label/gallery/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2774 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.9/deeplabel/label/gallery/detections.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3323 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.9/deeplabel/label/gallery/images.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1420 2022-11-02 10:18:49.000000 deeplabel-sdk-0.4.9/deeplabel/label/label_maps.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2026 2022-11-02 10:18:56.000000 deeplabel-sdk-0.4.9/deeplabel/label/labels.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.605275 deeplabel-sdk-0.4.9/deeplabel/label/videos/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     9738 2022-12-06 10:30:45.000000 deeplabel-sdk-0.4.9/deeplabel/label/videos/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     3076 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.9/deeplabel/label/videos/detections.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2052 2022-11-02 10:19:33.000000 deeplabel-sdk-0.4.9/deeplabel/label/videos/frames.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2913 2022-11-02 10:19:37.000000 deeplabel-sdk-0.4.9/deeplabel/label/videos/video_tasks.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2083 2022-11-02 10:15:55.000000 deeplabel-sdk-0.4.9/deeplabel/projects.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.633275 deeplabel-sdk-0.4.9/deeplabel/types/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/types/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     4126 2022-12-26 19:35:08.000000 deeplabel-sdk-0.4.9/deeplabel/types/bounding_box.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      639 2022-11-02 10:19:44.000000 deeplabel-sdk-0.4.9/deeplabel/types/polygon.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.653275 deeplabel-sdk-0.4.9/deeplabel/utils/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/utils/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      901 2022-08-23 11:25:38.000000 deeplabel-sdk-0.4.9/deeplabel/utils/videos.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.661275 deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     1033 2022-12-28 12:41:06.000000 deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     2056 2022-12-28 12:41:06.000000 deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        1 2022-12-28 12:41:06.000000 deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      139 2022-12-28 12:41:06.000000 deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/requires.txt
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       16 2022-12-28 12:41:06.000000 deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)       38 2022-12-28 12:41:07.701275 deeplabel-sdk-0.4.9/setup.cfg
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)     8644 2022-12-28 12:40:28.000000 deeplabel-sdk-0.4.9/setup.py
+drwxrwxr-x   0 sufiyan   (1004) sufiyan   (1006)        0 2022-12-28 12:41:07.661275 deeplabel-sdk-0.4.9/tests/
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)        0 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.9/tests/__init__.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      339 2022-12-28 12:40:27.000000 deeplabel-sdk-0.4.9/tests/conftest.py
+-rw-rw-r--   0 sufiyan   (1004) sufiyan   (1006)      556 2022-11-17 07:25:44.000000 deeplabel-sdk-0.4.9/tests/test_project.py
```

### Comparing `deeplabel-sdk-0.4.8/PKG-INFO` & `deeplabel-sdk-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplabel-sdk
-Version: 0.4.8
+Version: 0.4.9
 Summary: python sdk to get data from deeplabel
 Home-page: https://github.com/streamingo/deeplabel
 Author: Streamingo Solutions
 Author-email: deeplabel-team@streamingo.ai
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/streamingo/deeplabel/issues
 Project-URL: Source, https://github.com/streamingo/deeplabel/
```

### Comparing `deeplabel-sdk-0.4.8/deeplabel/auth/tokens.py` & `deeplabel-sdk-0.4.9/deeplabel/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/auth/users.py` & `deeplabel-sdk-0.4.9/deeplabel/auth/users.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/basemodel.py` & `deeplabel-sdk-0.4.9/deeplabel/basemodel.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/client.py` & `deeplabel-sdk-0.4.9/deeplabel/client.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/contrib/downloaders/frame_downloader.py` & `deeplabel-sdk-0.4.9/deeplabel/contrib/downloaders/frame_downloader.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/ava.py` & `deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/ava.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/coco.py` & `deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/coco.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/contrib/exporters/pascal_voc.py` & `deeplabel-sdk-0.4.9/deeplabel/contrib/exporters/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/contrib/importers/pascalvoc.py` & `deeplabel-sdk-0.4.9/deeplabel/contrib/importers/pascalvoc.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/contrib/importers/utils.py` & `deeplabel-sdk-0.4.9/deeplabel/contrib/importers/utils.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/contrib/utils.py` & `deeplabel-sdk-0.4.9/deeplabel/contrib/utils.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/exceptions.py` & `deeplabel-sdk-0.4.9/deeplabel/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/feedback/videos.py` & `deeplabel-sdk-0.4.9/deeplabel/feedback/videos.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/folders.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/folders.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/gallery/__init__.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/gallery/detections.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/gallery/detections.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/gallery/gallery_graphs.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/gallery/gallery_graphs.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/gallery/gallery_tasks.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/gallery/gallery_tasks.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/gallery/images.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/gallery/images.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/graphs/__init__.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/graphs/graph_edges.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/graphs/graph_edges.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/graphs/graph_nodes.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/graphs/graph_nodes.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/notebooks.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/notebooks.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/presign.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/presign.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/videos/__init__.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/videos/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/videos/detections.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/videos/detections.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/videos/video_graphs.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/videos/video_graphs.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/infer/videos/video_tasks.py` & `deeplabel-sdk-0.4.9/deeplabel/infer/videos/video_tasks.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/dl_models.py` & `deeplabel-sdk-0.4.9/deeplabel/label/dl_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -111,7 +111,23 @@
         resp = self.client.get(
             "/dlmodels/download",
             params={"dlModelId": self.dl_model_id, "modelNames": "true"},
         )
         self.extra["names"] = resp.json()["data"].splitlines()
         return self.extra["names"]
 
+    @property
+    def names_filter(self) -> List[str]:
+        """Get dlmodel labels from model.names.filter or model.names.include file.
+        eg. ['labelA', 'labelC']
+        raises InvalidApiResponse if the neigher of the file exist.
+        So use with caution 
+        """
+        if "names_filter" in self.extra:
+            return self.extra["names_filter"]
+        resp = self.client.get(
+            "/dlmodels/download",
+            params={"dlModelId": self.dl_model_id, "modelNamesFilter": "true"},
+        )
+        self.extra["names_filter"] = resp.json()["data"].splitlines()
+        return self.extra["names_filter"]
+
```

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/folders.py` & `deeplabel-sdk-0.4.9/deeplabel/label/folders.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/gallery/__init__.py` & `deeplabel-sdk-0.4.9/deeplabel/label/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/gallery/detections.py` & `deeplabel-sdk-0.4.9/deeplabel/label/gallery/detections.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/gallery/images.py` & `deeplabel-sdk-0.4.9/deeplabel/label/gallery/images.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/label_maps.py` & `deeplabel-sdk-0.4.9/deeplabel/label/label_maps.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/labels.py` & `deeplabel-sdk-0.4.9/deeplabel/label/labels.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/videos/__init__.py` & `deeplabel-sdk-0.4.9/deeplabel/label/videos/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/videos/detections.py` & `deeplabel-sdk-0.4.9/deeplabel/label/videos/detections.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/videos/frames.py` & `deeplabel-sdk-0.4.9/deeplabel/label/videos/frames.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/label/videos/video_tasks.py` & `deeplabel-sdk-0.4.9/deeplabel/label/videos/video_tasks.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/projects.py` & `deeplabel-sdk-0.4.9/deeplabel/projects.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/types/bounding_box.py` & `deeplabel-sdk-0.4.9/deeplabel/types/bounding_box.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/types/polygon.py` & `deeplabel-sdk-0.4.9/deeplabel/types/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel/utils/videos.py` & `deeplabel-sdk-0.4.9/deeplabel/utils/videos.py`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/PKG-INFO` & `deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplabel-sdk
-Version: 0.4.8
+Version: 0.4.9
 Summary: python sdk to get data from deeplabel
 Home-page: https://github.com/streamingo/deeplabel
 Author: Streamingo Solutions
 Author-email: deeplabel-team@streamingo.ai
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/streamingo/deeplabel/issues
 Project-URL: Source, https://github.com/streamingo/deeplabel/
```

### Comparing `deeplabel-sdk-0.4.8/deeplabel_sdk.egg-info/SOURCES.txt` & `deeplabel-sdk-0.4.9/deeplabel_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplabel-sdk-0.4.8/setup.py` & `deeplabel-sdk-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.4.8',  # Required
+    version='0.4.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='python sdk to get data from deeplabel',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `deeplabel-sdk-0.4.8/tests/test_project.py` & `deeplabel-sdk-0.4.9/tests/test_project.py`

 * *Files identical despite different names*

