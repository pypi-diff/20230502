# Comparing `tmp/ape-ai-0.1.2.tar.gz` & `tmp/ape-ai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ai-0.1.2.tar", last modified: Tue May  2 05:59:04 2023, max compression
+gzip compressed data, was "ape-ai-0.1.3.tar", last modified: Tue May  2 06:37:15 2023, max compression
```

## Comparing `ape-ai-0.1.2.tar` & `ape-ai-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:59:04.051360 ape-ai-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 05:59:04.051360 ape-ai-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-02 05:58:34.000000 ape-ai-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:59:04.047360 ape-ai-0.1.2/ape/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:58:34.000000 ape-ai-0.1.2/ape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 05:58:34.000000 ape-ai-0.1.2/ape/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:59:04.047360 ape-ai-0.1.2/ape/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 05:58:34.000000 ape-ai-0.1.2/ape/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 05:58:34.000000 ape-ai-0.1.2/ape/optimization/evolution_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:59:04.047360 ape-ai-0.1.2/ape/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-02 05:58:34.000000 ape-ai-0.1.2/ape/tests/test_evolution_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 05:58:34.000000 ape-ai-0.1.2/ape/tests/test_read_me.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:59:04.047360 ape-ai-0.1.2/ape_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 05:59:04.000000 ape-ai-0.1.2/ape_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-02 05:59:04.000000 ape-ai-0.1.2/ape_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:59:04.000000 ape-ai-0.1.2/ape_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 05:59:04.000000 ape-ai-0.1.2/ape_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 05:59:04.000000 ape-ai-0.1.2/ape_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 05:58:34.000000 ape-ai-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:59:04.051360 ape-ai-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:37:14.995870 ape-ai-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 06:37:14.995870 ape-ai-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-02 06:36:44.000000 ape-ai-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:37:14.995870 ape-ai-0.1.3/ape/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 06:36:44.000000 ape-ai-0.1.3/ape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 06:36:44.000000 ape-ai-0.1.3/ape/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 06:37:14.995870 ape-ai-0.1.3/ape/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:37:14.995870 ape-ai-0.1.3/ape/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 06:36:44.000000 ape-ai-0.1.3/ape/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 06:36:44.000000 ape-ai-0.1.3/ape/optimization/evolution_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:37:14.995870 ape-ai-0.1.3/ape/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-02 06:36:44.000000 ape-ai-0.1.3/ape/tests/test_evolution_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 06:36:44.000000 ape-ai-0.1.3/ape/tests/test_read_me.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:37:14.995870 ape-ai-0.1.3/ape_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 06:37:14.000000 ape-ai-0.1.3/ape_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-02 06:37:14.000000 ape-ai-0.1.3/ape_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:37:14.000000 ape-ai-0.1.3/ape_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 06:37:14.000000 ape-ai-0.1.3/ape_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 06:37:14.000000 ape-ai-0.1.3/ape_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-02 06:36:44.000000 ape-ai-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 06:37:14.995870 ape-ai-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 06:36:44.000000 ape-ai-0.1.3/setup.py
```

### Comparing `ape-ai-0.1.2/PKG-INFO` & `ape-ai-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ai
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python framework for AI
 Author-email: Guilherme Kowalczuk <guilhermekowalczuk@gmail.com>
 Project-URL: repository, https://github.com/kowalks/ape-ai
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `ape-ai-0.1.2/README.md` & `ape-ai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ape-ai-0.1.2/ape/optimization/evolution_strategy.py` & `ape-ai-0.1.3/ape/optimization/evolution_strategy.py`

 * *Files identical despite different names*

### Comparing `ape-ai-0.1.2/ape_ai.egg-info/PKG-INFO` & `ape-ai-0.1.3/ape_ai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ai
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python framework for AI
 Author-email: Guilherme Kowalczuk <guilhermekowalczuk@gmail.com>
 Project-URL: repository, https://github.com/kowalks/ape-ai
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

