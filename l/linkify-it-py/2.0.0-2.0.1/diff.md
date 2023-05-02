# Comparing `tmp/linkify-it-py-2.0.0.tar.gz` & `tmp/linkify-it-py-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linkify-it-py-2.0.0.tar", last modified: Sat May  7 07:00:30 2022, max compression
+gzip compressed data, was "/home/runner/work/linkify-it-py/linkify-it-py/dist/.tmp-ksdygp5z/linkify-it-py-2.0.1.tar", last modified: Mon May  1 17:49:38 2023, max compression
```

## Comparing `linkify-it-py-2.0.0.tar` & `linkify-it-py-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9361 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6656 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21327 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    20791 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/tlds.py
--rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/ucre.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9361 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/linkify_it/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/linkify_it/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21327 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/linkify_it/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/linkify_it/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/linkify_it/ucre.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/linkify_it_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/linkify_it_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/linkify_it_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/linkify_it_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/linkify_it_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/linkify_it_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:49:38.000000 linkify-it-py-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/test/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/test/test_linkify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 17:49:22.000000 linkify-it-py-2.0.1/tox.ini
```

### Comparing `linkify-it-py-2.0.0/CHANGELOG.md` & `linkify-it-py-2.0.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change Log
 
+## v2.0.1 (2023-05-02)
+
+- Update development tools
+- Fix sdist is missing tests
+
 ## v2.0.0 (2022-05-07)
 
 - Add `matchAtStart` method to match full URLs at the start of the string.
 - Fixed paired symbols (`()`, `{}`, `""`, etc.) after punctuation.
 - `---` option now affects parsing of emails  (e.g. `user@example.com---`)
 
 ## v1.0.3 (2021-12-18)
```

### Comparing `linkify-it-py-2.0.0/LICENSE` & `linkify-it-py-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linkify-it-py-2.0.0/README.md` & `linkify-it-py-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `linkify-it-py-2.0.0/linkify_it/main.py` & `linkify-it-py-2.0.1/linkify_it/main.py`

 * *Files identical despite different names*

### Comparing `linkify-it-py-2.0.0/linkify_it/tlds.py` & `linkify-it-py-2.0.1/linkify_it/tlds.py`

 * *Files identical despite different names*

### Comparing `linkify-it-py-2.0.0/linkify_it/ucre.py` & `linkify-it-py-2.0.1/linkify_it/ucre.py`

 * *Files identical despite different names*

