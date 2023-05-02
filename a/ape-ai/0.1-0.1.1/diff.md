# Comparing `tmp/ape-ai-0.1.tar.gz` & `tmp/ape-ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ai-0.1.tar", last modified: Tue May  2 05:28:45 2023, max compression
+gzip compressed data, was "ape-ai-0.1.1.tar", last modified: Tue May  2 05:49:26 2023, max compression
```

## Comparing `ape-ai-0.1.tar` & `ape-ai-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:45.534510 ape-ai-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-02 05:28:45.530510 ape-ai-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-02 05:28:11.000000 ape-ai-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:45.530510 ape-ai-0.1/ape/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:28:11.000000 ape-ai-0.1/ape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 05:28:11.000000 ape-ai-0.1/ape/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:45.530510 ape-ai-0.1/ape/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 05:28:11.000000 ape-ai-0.1/ape/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 05:28:11.000000 ape-ai-0.1/ape/optimization/evolution_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:45.530510 ape-ai-0.1/ape/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-02 05:28:11.000000 ape-ai-0.1/ape/tests/test_evolution_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 05:28:11.000000 ape-ai-0.1/ape/tests/test_read_me.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:45.530510 ape-ai-0.1/ape_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-02 05:28:45.000000 ape-ai-0.1/ape_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 05:28:45.000000 ape-ai-0.1/ape_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:28:45.000000 ape-ai-0.1/ape_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 05:28:45.000000 ape-ai-0.1/ape_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 05:28:11.000000 ape-ai-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:28:45.534510 ape-ai-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:49:26.770963 ape-ai-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-02 05:49:26.770963 ape-ai-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-02 05:48:49.000000 ape-ai-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:49:26.766962 ape-ai-0.1.1/ape/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:48:49.000000 ape-ai-0.1.1/ape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 05:48:49.000000 ape-ai-0.1.1/ape/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:49:26.770963 ape-ai-0.1.1/ape/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 05:48:49.000000 ape-ai-0.1.1/ape/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 05:48:49.000000 ape-ai-0.1.1/ape/optimization/evolution_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:49:26.770963 ape-ai-0.1.1/ape/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-02 05:48:49.000000 ape-ai-0.1.1/ape/tests/test_evolution_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 05:48:49.000000 ape-ai-0.1.1/ape/tests/test_read_me.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:49:26.770963 ape-ai-0.1.1/ape_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-02 05:49:26.000000 ape-ai-0.1.1/ape_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 05:49:26.000000 ape-ai-0.1.1/ape_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:49:26.000000 ape-ai-0.1.1/ape_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 05:49:26.000000 ape-ai-0.1.1/ape_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-02 05:48:49.000000 ape-ai-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:49:26.770963 ape-ai-0.1.1/setup.cfg
```

### Comparing `ape-ai-0.1/PKG-INFO` & `ape-ai-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: ape-ai
-Version: 0.1
+Version: 0.1.1
+Summary: A Python framework for AI
 Author-email: Guilherme Kowalczuk <guilhermekowalczuk@gmail.com>
+Project-URL: repository, https://github.com/kowalks/ape-ai
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # ape-ai: a Python framework for AI
 
 ## What is it?
```

### Comparing `ape-ai-0.1/README.md` & `ape-ai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ape-ai-0.1/ape/optimization/evolution_strategy.py` & `ape-ai-0.1.1/ape/optimization/evolution_strategy.py`

 * *Files identical despite different names*

### Comparing `ape-ai-0.1/ape_ai.egg-info/PKG-INFO` & `ape-ai-0.1.1/ape_ai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: ape-ai
-Version: 0.1
+Version: 0.1.1
+Summary: A Python framework for AI
 Author-email: Guilherme Kowalczuk <guilhermekowalczuk@gmail.com>
+Project-URL: repository, https://github.com/kowalks/ape-ai
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # ape-ai: a Python framework for AI
 
 ## What is it?
```

