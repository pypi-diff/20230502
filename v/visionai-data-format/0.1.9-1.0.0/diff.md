# Comparing `tmp/visionai-data-format-0.1.9.tar.gz` & `tmp/visionai-data-format-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-0.1.9.tar", last modified: Mon Mar 27 03:35:10 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.0.tar", last modified: Tue May  2 07:40:22 2023, max compression
```

## Comparing `visionai-data-format-0.1.9.tar` & `visionai-data-format-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,73 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.735639 visionai-data-format-0.1.9/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.710233 visionai-data-format-0.1.9/.github/
--rw-r--r--   0 christian   (501) staff       (20)      472 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 christian   (501) staff       (20)      288 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/.github/labels.yml
--rw-r--r--   0 christian   (501) staff       (20)       16 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/.github/semantic.yml
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.710690 visionai-data-format-0.1.9/.github/workflows/
--rw-r--r--   0 christian   (501) staff       (20)      699 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/.github/workflows/test.yml
--rw-r--r--   0 christian   (501) staff       (20)     3080 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/.gitignore
--rw-r--r--   0 christian   (501) staff       (20)     1741 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 christian   (501) staff       (20)     1507 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/Makefile
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-03-27 03:35:10.735196 visionai-data-format-0.1.9/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)       69 2022-11-09 05:29:43.000000 visionai-data-format-0.1.9/README.md
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.712691 visionai-data-format-0.1.9/ci/
--rw-r--r--   0 christian   (501) staff       (20)      965 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/ci/.commitlint.yaml
--rw-r--r--   0 christian   (501) staff       (20)     1465 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/ci/COMMIT_MESSAGE_TEMPLATE
--rw-r--r--   0 christian   (501) staff       (20)       63 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/ci/dev.txt
--rw-r--r--   0 christian   (501) staff       (20)      312 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/ci/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)       38 2023-03-27 03:35:10.735792 visionai-data-format-0.1.9/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      577 2023-03-27 03:32:46.000000 visionai-data-format-0.1.9/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.713249 visionai-data-format-0.1.9/tests/
--rw-r--r--   0 christian   (501) staff       (20)     2228 2023-03-14 09:30:26.000000 visionai-data-format-0.1.9/tests/test_schemas.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.717295 visionai-data-format-0.1.9/visionai_data_format/
--rw-r--r--   0 christian   (501) staff       (20)     1609 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/Readme.md
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     1400 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 christian   (501) staff       (20)     7742 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.727322 visionai-data-format-0.1.9/visionai_data_format/schemas/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     2142 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 christian   (501) staff       (20)     1057 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/schemas/common.py
--rw-r--r--   0 christian   (501) staff       (20)    18209 2023-03-14 09:30:26.000000 visionai-data-format-0.1.9/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.734417 visionai-data-format-0.1.9/visionai_data_format/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      495 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/utils/calculation.py
--rw-r--r--   0 christian   (501) staff       (20)    10506 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/utils/checker.py
--rw-r--r--   0 christian   (501) staff       (20)      761 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/utils/classes.py
--rw-r--r--   0 christian   (501) staff       (20)      335 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/utils/common.py
--rw-r--r--   0 christian   (501) staff       (20)     7209 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/utils/converter.py
--rw-r--r--   0 christian   (501) staff       (20)     4059 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/utils/resize.py
--rw-r--r--   0 christian   (501) staff       (20)     1986 2023-03-27 03:32:46.000000 visionai-data-format-0.1.9/visionai_data_format/utils/validator.py
--rw-r--r--   0 christian   (501) staff       (20)     2274 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 christian   (501) staff       (20)     6237 2023-03-14 09:30:19.000000 visionai-data-format-0.1.9/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-03-27 03:35:10.720454 visionai-data-format-0.1.9/visionai_data_format.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-03-27 03:35:10.000000 visionai-data-format-0.1.9/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1206 2023-03-27 03:35:10.000000 visionai-data-format-0.1.9/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-03-27 03:35:10.000000 visionai-data-format-0.1.9/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       40 2023-03-27 03:35:10.000000 visionai-data-format-0.1.9/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)       21 2023-03-27 03:35:10.000000 visionai-data-format-0.1.9/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.374957 visionai-data-format-1.0.0/
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.295626 visionai-data-format-1.0.0/.github/
+-rw-r--r--   0 christian   (501) staff       (20)      472 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 christian   (501) staff       (20)      288 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/labels.yml
+-rw-r--r--   0 christian   (501) staff       (20)       16 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/semantic.yml
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.297401 visionai-data-format-1.0.0/.github/workflows/
+-rw-r--r--   0 christian   (501) staff       (20)      699 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0 christian   (501) staff       (20)     3080 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.gitignore
+-rw-r--r--   0 christian   (501) staff       (20)     1741 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 christian   (501) staff       (20)     1507 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/Makefile
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-02 07:40:22.373495 visionai-data-format-1.0.0/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)       69 2022-11-09 05:29:43.000000 visionai-data-format-1.0.0/README.md
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.300660 visionai-data-format-1.0.0/ci/
+-rw-r--r--   0 christian   (501) staff       (20)      965 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/.commitlint.yaml
+-rw-r--r--   0 christian   (501) staff       (20)     1465 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/COMMIT_MESSAGE_TEMPLATE
+-rw-r--r--   0 christian   (501) staff       (20)       63 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/dev.txt
+-rw-r--r--   0 christian   (501) staff       (20)      312 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/ci/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)     3658 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/conftest.py
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-05-02 07:40:22.375105 visionai-data-format-1.0.0/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      577 2023-05-02 07:39:07.000000 visionai-data-format-1.0.0/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.302478 visionai-data-format-1.0.0/tests/
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.332330 visionai-data-format-1.0.0/tests/test_data/
+-rw-r--r--   0 christian   (501) staff       (20)     2549 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_contexts_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     7424 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar.json
+-rw-r--r--   0 christian   (501) staff       (20)     5850 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_class.json
+-rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_objects_frame_intervals.json
+-rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_single_lidar_wrong_visionai_frame_intervals.json
+-rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_wrong_frame_properties_sensor.json
+-rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_data_wrong_visionai_streams_sensor.json
+-rw-r--r--   0 christian   (501) staff       (20)    26678 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation.json
+-rw-r--r--   0 christian   (501) staff       (20)    25431 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation_without_tags.json
+-rw-r--r--   0 christian   (501) staff       (20)    26676 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_objects_semantic_segmentation_wrong_tags_classes.json
+-rw-r--r--   0 christian   (501) staff       (20)     4796 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/fake_raw_data.json
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_visionai_classification_ontology.json
+-rw-r--r--   0 christian   (501) staff       (20)     5885 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_visionai_ontology.json
+-rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_data/fake_visionai_semantic_ontology.json
+-rw-r--r--   0 christian   (501) staff       (20)     7052 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/generated_objects_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     4424 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_data/generated_raw_data.json
+-rw-r--r--   0 christian   (501) staff       (20)     2177 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4727 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.343932 visionai-data-format-1.0.0/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)     1609 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/Readme.md
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     1400 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7697 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.352959 visionai-data-format-1.0.0/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2142 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1062 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.355971 visionai-data-format-1.0.0/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-02 07:39:07.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    39422 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    26771 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.371650 visionai-data-format-1.0.0/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      495 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)     6877 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1992 2023-05-02 06:36:09.000000 visionai-data-format-1.0.0/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2274 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-04-25 09:32:08.000000 visionai-data-format-1.0.0/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-02 07:40:22.348421 visionai-data-format-1.0.0/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     2353 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       40 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-05-02 07:40:22.000000 visionai-data-format-1.0.0/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-0.1.9/.github/workflows/test.yml` & `visionai-data-format-1.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/.gitignore` & `visionai-data-format-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/.pre-commit-config.yaml` & `visionai-data-format-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/Makefile` & `visionai-data-format-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/ci/.commitlint.yaml` & `visionai-data-format-1.0.0/ci/.commitlint.yaml`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/ci/COMMIT_MESSAGE_TEMPLATE` & `visionai-data-format-1.0.0/ci/COMMIT_MESSAGE_TEMPLATE`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/setup.py` & `visionai-data-format-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "0.1.9"
+PACKAGE_VERSION = "1.0.0"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-0.1.9/tests/test_schemas.py` & `visionai-data-format-1.0.0/tests/test_schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import pytest
+
 from visionai_data_format.schemas.bdd_schema import BDDSchema
 from visionai_data_format.schemas.coco_schema import Coco
-from visionai_data_format.schemas.visionai_schema import VisionAI, VisionAIModel
+from visionai_data_format.schemas.visionai_schema import VisionAIModel
 
 
 def test_coco():
     input_data = {
         "info": {
             "year": "",
             "version": "",
@@ -47,40 +49,34 @@
             "objects": {},
             "coordinate_systems": {},
             "streams": {},
             "tags": {},
             "metadata": {"schema_version": "1.0.0"},
         }
     }
+    with pytest.raises(Exception):
+        assert VisionAIModel(**input_data).dict() == generated_data
 
-    assert VisionAIModel(**input_data).dict() == generated_data
-
-
-def test_visionai():
-    input_data = {
-        "contexts": {},
-        "frame_intervals": [],
-        "frames": {},
-        "objects": {},
-        "coordinate_systems": {},
-        "streams": {},
-        "tags": {},
-    }
-    generated_data = {
-        "contexts": {},
-        "frame_intervals": [],
-        "frames": {},
-        "objects": {},
-        "coordinate_systems": {},
-        "streams": {},
-        "tags": {},
-        "metadata": {"schema_version": "1.0.0"},
-    }
 
-    assert VisionAI(**input_data).dict() == generated_data
+def test_visionai(
+    fake_raw_visionai_data,
+    fake_generated_raw_visionai_data,
+    fake_objects_visionai_data,
+    fake_generated_objects_visionai_data,
+):
+
+    assert (
+        VisionAIModel(**fake_raw_visionai_data).dict(exclude_unset=True)
+        == fake_generated_raw_visionai_data
+    )
+
+    assert (
+        VisionAIModel(**fake_objects_visionai_data).dict(exclude_unset=True)
+        == fake_generated_objects_visionai_data
+    )
 
 
 def test_bdd():
     input_data = {"frame_list": []}
     generated_data = {
         "bdd_version": "1.1.4",
         "company_code": None,
```

### Comparing `visionai-data-format-0.1.9/visionai_data_format/Readme.md` & `visionai-data-format-1.0.0/visionai_data_format/Readme.md`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.0/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.0/visionai_data_format/coco_to_vai.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import logging
 import os
 import shutil
 import uuid
 
 from visionai_data_format.schemas.visionai_schema import (
     Bbox,
+    DynamicObjectData,
     Frame,
     FrameInterval,
     FrameProperties,
     FramePropertyStream,
     Metadata,
     Object,
-    ObjectData,
     ObjectDataPointer,
     ObjectType,
     ObjectUnderFrame,
     SchemaVersion,
     Stream,
     StreamType,
     VisionAI,
@@ -105,21 +105,20 @@
         ]
         image_name = image_id_name_dict[str(anno["image_id"])]
 
         # to vision_ai: frames
         # assume there is only one sensor, so image_index always is 0
         objects_under_frames = {
             object_id: ObjectUnderFrame(
-                object_data=ObjectData(
+                object_data=DynamicObjectData(
                     bbox=[
                         Bbox(
                             name=BBOX_NAME,
                             val=bbox,
                             stream=sensor_name,
-                            coordinate_system=sensor_name,
                         )
                     ]
                 )
             )
         }
         frames[image_name].objects.update(objects_under_frames)
```

### Comparing `visionai-data-format-0.1.9/visionai_data_format/schemas/bdd_schema.py` & `visionai-data-format-1.0.0/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.0/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/schemas/common.py` & `visionai-data-format-1.0.0/visionai_data_format/schemas/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum, EnumMeta
-from typing import Any, Optional
+from typing import Any, Optional, Set
 
 
 class BaseEnumMeta(EnumMeta):
-    _value_set: Optional[set[Any]] = None
+    _value_set: Optional[Set[Any]] = None
 
     def __contains__(cls, item):
         if cls._value_set is None:
-            cls._value_set: set[Any] = {v.value for v in cls.__members__.values()}
+            cls._value_set: Set[Any] = {v.value for v in cls.__members__.values()}
 
         return item in cls._value_set
 
 
 class OntologyImageType(str, Enum, metaclass=BaseEnumMeta):
     _2D_BOUNDING_BOX = "2d_bounding_box"
     SEMANTIC_SEGMENTATION = "semantic_segmentation"
```

### Comparing `visionai-data-format-0.1.9/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.0/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.0/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.0/visionai_data_format/utils/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import logging
 import os
 from collections import defaultdict
 
 from visionai_data_format.schemas.bdd_schema import AtrributeSchema
 from visionai_data_format.schemas.visionai_schema import (
     Bbox,
+    DynamicObjectData,
     Frame,
     FrameInterval,
     FrameProperties,
     FramePropertyStream,
     Object,
-    ObjectData,
     ObjectDataPointer,
     ObjectType,
     ObjectUnderFrame,
     Stream,
     StreamType,
     VisionAI,
 )
@@ -118,15 +118,15 @@
             labels = frame["labels"]
             meta_ds = frame.get("meta_ds", None)
             url = meta_ds["coco_url"] if meta_ds else name
 
             frames: dict[str, Frame] = defaultdict(Frame)
             objects: dict[str, Object] = defaultdict(Object)
             frame_data: Frame = Frame(
-                objects=defaultdict(ObjectData),
+                objects=defaultdict(DynamicObjectData),
                 frame_properties=FrameProperties(
                     streams={sensor_name: FramePropertyStream(uri=url)}
                 ),
             )
             frame_intervals = [
                 FrameInterval(frame_end=frame_idx, frame_start=frame_idx)
             ]
@@ -144,21 +144,20 @@
 
                 category = label["category"]
                 obj_uuid = label["uuid"]
                 x, y, w, h = xyxy2xywh(label["box2d"])
                 confidence_score = label.get("meta_ds", {}).get("score", None)
                 object_under_frames = {
                     obj_uuid: ObjectUnderFrame(
-                        object_data=ObjectData(
+                        object_data=DynamicObjectData(
                             bbox=[
                                 Bbox(
                                     name="bbox_shape",
                                     val=[x, y, w, h],
                                     stream=sensor_name,
-                                    coordinate_system=sensor_name,
                                     confidence_score=confidence_score,
                                 )
                             ]
                         )
                     )
                 }
                 frame_data.objects.update(object_under_frames)
@@ -171,29 +170,21 @@
                         "bbox_shape": ObjectDataPointer(
                             type=ObjectType.bbox, frame_intervals=frame_intervals
                         )
                     },
                 )
             frames[frame_idx] = frame_data
             streams = {sensor_name: Stream(type=StreamType.camera)}
-            coordinate_systems = {
-                sensor_name: {
-                    "type": "sensor_cs",
-                    "parent": "vehicle-iso8855",
-                    "children": [],
-                }
-            }
             vai_data = {
                 "visionai": {
                     "frame_intervals": frame_intervals,
                     "objects": objects,
                     "frames": frames,
                     "streams": streams,
                     "metadata": {"schema_version": "1.0.0"},
-                    "coordinate_systems": coordinate_systems,
                 }
             }
             vai_data = validate_vai(vai_data).dict(exclude_none=True)
             save_as_json(
                 vai_data,
                 folder_name=vai_dest_folder,
                 file_name=name + ".json",
```

### Comparing `visionai-data-format-0.1.9/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.0/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.0/visionai_data_format/utils/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import json
 import logging
 import os
-from typing import Union
+from typing import Dict, Union
 
 from visionai_data_format.schemas.bdd_schema import BDDSchema
 from visionai_data_format.schemas.visionai_schema import VisionAIModel
 
 logger = logging.getLogger(__name__)
 
 
-def validate_vai(data: dict) -> Union[VisionAIModel, None]:
+def validate_vai(data: Dict) -> Union[VisionAIModel, None]:
     try:
         vai = VisionAIModel(**data)
         logger.info("[validated_vai] Validate success")
         return vai
     except Exception as e:
         logger.error("[validated_vai] Validate failed : " + str(e))
         return None
 
 
-def validate_bdd(data: dict) -> Union[BDDSchema, None]:
+def validate_bdd(data: Dict) -> Union[BDDSchema, None]:
     try:
         bdd = BDDSchema(**data)
         logger.info("[validate_bdd] Validation success")
         return bdd
     except Exception as e:
         logger.error("[validate_bdd] Validation failed : " + str(e))
         return None
 
 
 def attribute_generator(
-    category: str, attribute: dict, ontology_class_attrs: dict
-) -> dict:
+    category: str, attribute: Dict, ontology_class_attrs: Dict
+) -> Dict:
 
     if not attribute:
         return dict()
 
     new_attribute = dict()
     category = category.upper()
     for attr_name, attr_value in attribute.items():
@@ -44,15 +44,15 @@
         if attr_name in ontology_class_attrs[category]:
             new_attribute[attr_name] = attr_value
 
     logger.info(f"[datarow_attribute_generator] new_attribute : {new_attribute}")
     return new_attribute
 
 
-def save_as_json(data: dict, file_name: str, folder_name: str = "") -> None:
+def save_as_json(data: Dict, file_name: str, folder_name: str = "") -> None:
     try:
         if folder_name:
             os.makedirs(folder_name, exist_ok=True)
         file = open(os.path.join(folder_name, file_name), "w")
         logger.info(
             f"[save_as_json] Save file to {os.path.join(folder_name,file_name)} started "
         )
```

### Comparing `visionai-data-format-0.1.9/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.0/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.0/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-0.1.9/visionai_data_format.egg-info/SOURCES.txt` & `visionai-data-format-1.0.0/visionai_data_format.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,40 @@
 .gitignore
 .pre-commit-config.yaml
 Makefile
 README.md
+conftest.py
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/labels.yml
 .github/semantic.yml
 .github/workflows/test.yml
 ci/.commitlint.yaml
 ci/COMMIT_MESSAGE_TEMPLATE
 ci/dev.txt
 ci/setup.cfg
 tests/test_schemas.py
+tests/test_validators.py
+tests/test_data/fake_contexts_data.json
+tests/test_data/fake_objects_data.json
+tests/test_data/fake_objects_data_single_lidar.json
+tests/test_data/fake_objects_data_single_lidar_wrong_class.json
+tests/test_data/fake_objects_data_single_lidar_wrong_objects_frame_intervals.json
+tests/test_data/fake_objects_data_single_lidar_wrong_visionai_frame_intervals.json
+tests/test_data/fake_objects_data_wrong_frame_properties_sensor.json
+tests/test_data/fake_objects_data_wrong_visionai_streams_sensor.json
+tests/test_data/fake_objects_semantic_segmentation.json
+tests/test_data/fake_objects_semantic_segmentation_without_tags.json
+tests/test_data/fake_objects_semantic_segmentation_wrong_tags_classes.json
+tests/test_data/fake_raw_data.json
+tests/test_data/fake_visionai_classification_ontology.json
+tests/test_data/fake_visionai_ontology.json
+tests/test_data/fake_visionai_semantic_ontology.json
+tests/test_data/generated_objects_data.json
+tests/test_data/generated_raw_data.json
 visionai_data_format/Readme.md
 visionai_data_format/__init__.py
 visionai_data_format/bdd_to_vai.py
 visionai_data_format/coco_to_vai.py
 visionai_data_format/vai_to_bdd.py
 visionai_data_format/vai_to_coco.py
 visionai_data_format.egg-info/PKG-INFO
@@ -23,15 +42,18 @@
 visionai_data_format.egg-info/dependency_links.txt
 visionai_data_format.egg-info/requires.txt
 visionai_data_format.egg-info/top_level.txt
 visionai_data_format/schemas/__init__.py
 visionai_data_format/schemas/bdd_schema.py
 visionai_data_format/schemas/coco_schema.py
 visionai_data_format/schemas/common.py
+visionai_data_format/schemas/ontology.py
 visionai_data_format/schemas/visionai_schema.py
+visionai_data_format/schemas/utils/__init__.py
+visionai_data_format/schemas/utils/validators.py
 visionai_data_format/utils/__init__.py
 visionai_data_format/utils/calculation.py
 visionai_data_format/utils/checker.py
 visionai_data_format/utils/classes.py
 visionai_data_format/utils/common.py
 visionai_data_format/utils/converter.py
 visionai_data_format/utils/resize.py
```

