# Comparing `tmp/ml_plugins-0.0.7.tar.gz` & `tmp/ml_plugins-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_plugins-0.0.7.tar", last modified: Mon May  1 06:43:31 2023, max compression
+gzip compressed data, was "ml_plugins-0.0.8.tar", last modified: Tue May  2 04:09:17 2023, max compression
```

## Comparing `ml_plugins-0.0.7.tar` & `ml_plugins-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.875936 ml_plugins-0.0.7/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:43:31.875558 ml_plugins-0.0.7/PKG-INFO
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.872317 ml_plugins-0.0.7/ml_plugins.egg-info/
--rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/PKG-INFO
--rw-r--r--   0 grace.han   (503) staff       (20)      324 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 grace.han   (503) staff       (20)       23 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/requires.txt
--rw-r--r--   0 grace.han   (503) staff       (20)       19 2023-05-01 06:43:31.000000 ml_plugins-0.0.7/ml_plugins.egg-info/top_level.txt
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.872717 ml_plugins-0.0.7/plugins/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 06:13:56.000000 ml_plugins-0.0.7/plugins/__init__.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.873556 ml_plugins-0.0.7/plugins/pip/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.7/plugins/pip/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.7/plugins/pip/pip.py
-drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-01 06:43:31.874903 ml_plugins-0.0.7/plugins/poetry/
--rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.7/plugins/poetry/__init__.py
--rw-r--r--   0 grace.han   (503) staff       (20)       56 2023-05-01 00:54:16.000000 ml_plugins-0.0.7/plugins/poetry/example.py
--rw-r--r--   0 grace.han   (503) staff       (20)      448 2023-05-01 06:38:58.000000 ml_plugins-0.0.7/plugins/poetry/plugin.py
--rw-r--r--   0 grace.han   (503) staff       (20)      281 2023-05-01 06:43:22.000000 ml_plugins-0.0.7/pyproject.toml
--rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-01 06:43:31.876091 ml_plugins-0.0.7/setup.cfg
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-02 04:09:17.219829 ml_plugins-0.0.8/
+-rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-02 04:09:17.218495 ml_plugins-0.0.8/PKG-INFO
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-02 04:09:17.210696 ml_plugins-0.0.8/ml_plugins.egg-info/
+-rw-r--r--   0 grace.han   (503) staff       (20)       54 2023-05-02 04:09:17.000000 ml_plugins-0.0.8/ml_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 grace.han   (503) staff       (20)      362 2023-05-02 04:09:17.000000 ml_plugins-0.0.8/ml_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)        1 2023-05-02 04:09:17.000000 ml_plugins-0.0.8/ml_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)       23 2023-05-02 04:09:17.000000 ml_plugins-0.0.8/ml_plugins.egg-info/requires.txt
+-rw-r--r--   0 grace.han   (503) staff       (20)       19 2023-05-02 04:09:17.000000 ml_plugins-0.0.8/ml_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-02 04:09:17.211643 ml_plugins-0.0.8/plugins/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 06:13:56.000000 ml_plugins-0.0.8/plugins/__init__.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-02 04:09:17.212832 ml_plugins-0.0.8/plugins/pip/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:15.000000 ml_plugins-0.0.8/plugins/pip/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-05-01 05:47:20.000000 ml_plugins-0.0.8/plugins/pip/pip.py
+drwxr-xr-x   0 grace.han   (503) staff       (20)        0 2023-05-02 04:09:17.216144 ml_plugins-0.0.8/plugins/poetry/
+-rw-r--r--   0 grace.han   (503) staff       (20)        0 2023-04-27 03:29:10.000000 ml_plugins-0.0.8/plugins/poetry/__init__.py
+-rw-r--r--   0 grace.han   (503) staff       (20)     1942 2023-05-02 04:08:42.000000 ml_plugins-0.0.8/plugins/poetry/example.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      460 2023-05-02 04:03:34.000000 ml_plugins-0.0.8/plugins/poetry/plugin.py
+-rw-r--r--   0 grace.han   (503) staff       (20)     1826 2023-05-02 00:59:01.000000 ml_plugins-0.0.8/plugins/poetry/test-batch-metaflow.py
+-rw-r--r--   0 grace.han   (503) staff       (20)      281 2023-05-02 04:09:10.000000 ml_plugins-0.0.8/pyproject.toml
+-rw-r--r--   0 grace.han   (503) staff       (20)       38 2023-05-02 04:09:17.220341 ml_plugins-0.0.8/setup.cfg
```

