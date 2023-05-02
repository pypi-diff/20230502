# Comparing `tmp/tensorflow_dataset-0.4.1.tar.gz` & `tmp/tensorflow-dataset-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow_dataset-0.4.1.tar", last modified: Tue Apr 25 05:32:11 2023, max compression
+gzip compressed data, was "tensorflow-dataset-0.4.2.tar", last modified: Tue May  2 04:18:57 2023, max compression
```

## Comparing `tensorflow_dataset-0.4.1.tar` & `tensorflow-dataset-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 05:32:11.592982 tensorflow_dataset-0.4.1/
--rw-rw-rw-   0        0        0      121 2023-04-25 05:32:11.584993 tensorflow_dataset-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-25 05:32:11.592982 tensorflow_dataset-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      287 2023-04-25 05:31:55.000000 tensorflow_dataset-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 05:32:11.577000 tensorflow_dataset-0.4.1/tensorflow_dataset/
--rw-rw-rw-   0        0        0     3392 2023-04-25 05:31:41.000000 tensorflow_dataset-0.4.1/tensorflow_dataset/tensorflow_dataset.py
-drwxrwxrwx   0        0        0        0 2023-04-25 05:32:11.584993 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/
--rw-rw-rw-   0        0        0      121 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/
+-rw-rw-rw-   0        0        0      121 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      280 2023-05-02 04:18:41.000000 tensorflow-dataset-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/
+-rw-rw-rw-   0        0        0      121 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/tensorflow_datasets/
+-rw-rw-rw-   0        0        0    11799 2023-05-02 04:17:40.000000 tensorflow-dataset-0.4.2/tensorflow_datasets/__init__.py
```

