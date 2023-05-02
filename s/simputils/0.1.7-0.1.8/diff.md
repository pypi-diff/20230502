# Comparing `tmp/simputils-0.1.7.tar.gz` & `tmp/simputils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simputils-0.1.7.tar", last modified: Sun Aug 14 19:58:24 2022, max compression
+gzip compressed data, was "simputils-0.1.8.tar", last modified: Tue May  2 15:31:36 2023, max compression
```

## Comparing `simputils-0.1.7.tar` & `simputils-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 19:58:24.578608 simputils-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-14 19:58:17.000000 simputils-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-08-14 19:58:24.578608 simputils-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-08-14 19:58:17.000000 simputils-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-14 19:58:17.000000 simputils-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-08-14 19:58:24.578608 simputils-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-14 19:58:17.000000 simputils-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 19:58:24.578608 simputils-0.1.7/simputils/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3736 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/algos.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/caching.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/dateutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/functional.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/inspection.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/math.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-14 19:58:17.000000 simputils-0.1.7/simputils/rnd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 19:58:24.578608 simputils-0.1.7/simputils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-08-14 19:58:24.000000 simputils-0.1.7/simputils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-08-14 19:58:24.000000 simputils-0.1.7/simputils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 19:58:24.000000 simputils-0.1.7/simputils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-14 19:58:24.000000 simputils-0.1.7/simputils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-14 19:58:24.000000 simputils-0.1.7/simputils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:31:36.470564 simputils-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-02 15:31:27.000000 simputils-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-02 15:31:36.470564 simputils-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-02 15:31:27.000000 simputils-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 15:31:27.000000 simputils-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 15:31:36.470564 simputils-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-02 15:31:27.000000 simputils-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:31:36.470564 simputils-0.1.8/simputils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/dateutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-02 15:31:27.000000 simputils-0.1.8/simputils/rnd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:31:36.470564 simputils-0.1.8/simputils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-02 15:31:36.000000 simputils-0.1.8/simputils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-02 15:31:36.000000 simputils-0.1.8/simputils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:31:36.000000 simputils-0.1.8/simputils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-02 15:31:36.000000 simputils-0.1.8/simputils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 15:31:36.000000 simputils-0.1.8/simputils.egg-info/top_level.txt
```

### Comparing `simputils-0.1.7/LICENSE` & `simputils-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simputils-0.1.7/README.md` & `simputils-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `simputils-0.1.7/setup.cfg` & `simputils-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `simputils-0.1.7/simputils/algos.py` & `simputils-0.1.8/simputils/algos.py`

 * *Files identical despite different names*

### Comparing `simputils-0.1.7/simputils/caching.py` & `simputils-0.1.8/simputils/caching.py`

 * *Files identical despite different names*

### Comparing `simputils-0.1.7/simputils/functional.py` & `simputils-0.1.8/simputils/functional.py`

 * *Files identical despite different names*

### Comparing `simputils-0.1.7/simputils/logging.py` & `simputils-0.1.8/simputils/logging.py`

 * *Files identical despite different names*

