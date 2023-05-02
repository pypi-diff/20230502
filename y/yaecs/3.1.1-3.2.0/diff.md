# Comparing `tmp/yaecs-3.1.1.tar.gz` & `tmp/yaecs-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-3.1.1.tar", last modified: Fri Apr 28 10:42:20 2023, max compression
+gzip compressed data, was "yaecs-3.2.0.tar", last modified: Tue May  2 15:06:36 2023, max compression
```

## Comparing `yaecs-3.1.1.tar` & `yaecs-3.2.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.654179 yaecs-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 10:42:04.000000 yaecs-3.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.634178 yaecs-3.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.642178 yaecs-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 10:42:04.000000 yaecs-3.1.1/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-28 10:42:04.000000 yaecs-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-04-28 10:42:04.000000 yaecs-3.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-28 10:42:04.000000 yaecs-3.1.1/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-28 10:42:04.000000 yaecs-3.1.1/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-04-28 10:42:04.000000 yaecs-3.1.1/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-28 10:42:04.000000 yaecs-3.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 10:42:04.000000 yaecs-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-28 10:42:20.654179 yaecs-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-28 10:42:04.000000 yaecs-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-28 10:42:04.000000 yaecs-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 10:42:04.000000 yaecs-3.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.642178 yaecs-3.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-04-28 10:42:04.000000 yaecs-3.1.1/resources/yaecs_constructor_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:42:20.654179 yaecs-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 10:42:04.000000 yaecs-3.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-28 10:42:04.000000 yaecs-3.1.1/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.638178 yaecs-3.1.1/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-28 10:42:04.000000 yaecs-3.1.1/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    34035 2023-04-28 10:42:04.000000 yaecs-3.1.1/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 10:42:04.000000 yaecs-3.1.1/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.646179 yaecs-3.1.1/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.650179 yaecs-3.1.1/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 10:42:04.000000 yaecs-3.1.1/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.650179 yaecs-3.1.1/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.654179 yaecs-3.1.1/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43910 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17162 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-28 10:42:04.000000 yaecs-3.1.1/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:42:20.654179 yaecs-3.1.1/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 10:42:20.000000 yaecs-3.1.1/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.862839 yaecs-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 15:06:19.000000 yaecs-3.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.854838 yaecs-3.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-02 15:06:19.000000 yaecs-3.2.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-02 15:06:19.000000 yaecs-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-02 15:06:19.000000 yaecs-3.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-02 15:06:19.000000 yaecs-3.2.0/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-02 15:06:19.000000 yaecs-3.2.0/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-02 15:06:19.000000 yaecs-3.2.0/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-02 15:06:19.000000 yaecs-3.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 15:06:19.000000 yaecs-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-02 15:06:36.862839 yaecs-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-02 15:06:19.000000 yaecs-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-02 15:06:19.000000 yaecs-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:06:19.000000 yaecs-3.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-02 15:06:19.000000 yaecs-3.2.0/resources/yaecs_constructor_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:06:36.862839 yaecs-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-02 15:06:19.000000 yaecs-3.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-02 15:06:19.000000 yaecs-3.2.0/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.854838 yaecs-3.2.0/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-02 15:06:19.000000 yaecs-3.2.0/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-05-02 15:06:19.000000 yaecs-3.2.0/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-02 15:06:19.000000 yaecs-3.2.0/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-02 15:06:19.000000 yaecs-3.2.0/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 15:06:36.000000 yaecs-3.2.0/yaecs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.862839 yaecs-3.2.0/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47399 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/config_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34271 2023-05-02 15:06:19.000000 yaecs-3.2.0/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:06:36.858839 yaecs-3.2.0/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-02 15:06:36.000000 yaecs-3.2.0/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-02 15:06:36.000000 yaecs-3.2.0/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:06:36.000000 yaecs-3.2.0/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 15:06:36.000000 yaecs-3.2.0/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 15:06:36.000000 yaecs-3.2.0/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-3.1.1/.github/workflows/pipy_deployment.yaml` & `yaecs-3.2.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/.gitignore` & `yaecs-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/.pylintrc` & `yaecs-3.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/COPYING.LESSER.md` & `yaecs-3.2.0/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/COPYING.md` & `yaecs-3.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/DOCUMENTATION_WIP.md` & `yaecs-3.2.0/DOCUMENTATION_WIP.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/LICENSE.md` & `yaecs-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/PKG-INFO` & `yaecs-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.1.1
+Version: 3.2.0
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.1.1/README.md` & `yaecs-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/pyproject.toml` & `yaecs-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/resources/yaecs_constructor_overview.png` & `yaecs-3.2.0/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/setup.py` & `yaecs-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/short-readme.md` & `yaecs-3.2.0/short-readme.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/unittests/config/conftest.py` & `yaecs-3.2.0/unittests/config/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -205,7 +205,43 @@
         fil.write("param: 0.4")
     config2 = make_config(str(tmpdir / 'nd_first.yaml'),
                           str(tmpdir / 'nsave.yaml'),
                           additional_configs_suffix="_path",
                           variations_suffix="var*", grids_suffix="grid",
                           do_not_merge_command_line=True)
     yield config, config2
+
+
+@pytest.fixture
+def yaml_type_check(tmpdir):
+    index = len(os.listdir(tmpdir))
+    content = (f"root_path: '{tmpdir / f'default_second{index}.yaml'}'\nsubconfig: !subconfig\n  "
+               f"sub_path: '{tmpdir / f'default_second{index}.yaml'}'")
+    with open(tmpdir / f'default{index}.yaml', "w", encoding='utf-8') as fil:
+        fil.write(content)
+    content = ("param_int: !type:int 1\nparam_float: !type:float 0.1\nparam_str: !type:str abc\n"
+               "param_bool: !type:bool false\n"
+               "param_none: !type:none null\nparam_list: !type:list [0]\nparam_dict: !type:dict\n  a: 0\n"
+               "param_any: !type:Any null\nparam_tuple1: !type:(str,float) 0.4\nparam_tuple2: !type:(str,float) ab\n"
+               "param_optional1: !type:Optional[int] null\nparam_optional2: !type:Optional[int] 3\n"
+               "param_listint: !type:List[int] [0]\nparam_listintstr: !type:List[int,str] [0, ab]\n"
+               "param_dictlistoptionalint: !type:Dict[List[Optional[int]]]\n  a: [0, 1, null, 3]")
+    with open(tmpdir / f'default_second{index}.yaml', "w",
+              encoding='utf-8') as fil:
+        fil.write(content)
+    yield str(tmpdir / f'default{index}.yaml')
+
+
+@pytest.fixture
+def yaml_tag_assignment_check(tmpdir):
+    index = len(os.listdir(tmpdir))
+    content = (f"param1: !type:add_1 0.1\n--- !subconfig1\nparam2: 3.0\n---\n"
+               f"def_second_path: '{tmpdir / f'default_second{index}.yaml'}'\n"
+               "exp_second_path: null")
+    with open(tmpdir / f'default{index}.yaml', "w", encoding='utf-8') as fil:
+        fil.write(content)
+    content = ("--- !subconfig2\nparam3: 20.0\nsubconfig3: !subconfig3\n  "
+               "param4: !type:copy 'param1'")
+    with open(tmpdir / f'default_second{index}.yaml', "w",
+              encoding='utf-8') as fil:
+        fil.write(content)
+    yield str(tmpdir / f'default{index}.yaml')
```

### Comparing `yaecs-3.1.1/unittests/config/test_config.py` & `yaecs-3.2.0/unittests/config/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os.path as osp
 from pathlib import Path
 from typing import Any
 
 import pytest
 from utils import load_config, template
 
-from yaecs import Configuration
+from yaecs import assign_yaml_tag, assign_order, Configuration, Priority
 from yaecs.yaecs_utils import compare_string_pattern
 from yaecs.user_utils import make_config
 
 
 def check_integrity(config, p_1: Any = 0.1, p_2: Any = 2.0, p_3: Any = 30.0,
                     p_4: Any = "string"):
     assert config["param1"] == p_1
@@ -623,14 +623,62 @@
 
     assert not compare_string_pattern("abcdefgh0123", "abcdefgh012")
     assert not compare_string_pattern("abcdefgh0123", "abcde*g0123")
     assert not compare_string_pattern("abcdefgh0123ffffh0123", "abcde*gh0123")
     assert not compare_string_pattern("abcdefgh0123", "*3*3*3")
 
 
+def test_typecheck(yaml_type_check):
+    load_config(default_config=yaml_type_check)
+
+
+def test_yaml_tag_assignment(yaml_tag_assignment_check):
+    template_class = template(default_config=yaml_tag_assignment_check)
+
+    @assign_yaml_tag("add_1", "post", "float")
+    def add_1(self, param):
+        return param + 1
+
+    template_class.add_1 = add_1
+    config = template_class.load_config(do_not_merge_command_line=True)
+    check_integrity(config, p_1=1.1, p_2=3.0, p_3=20.0, p_4=1.1)
+
+
+def test_yaml_order(yaml_default):
+    @assign_order(Priority.SITUATIONAL)
+    def add_1(value):
+        return value + 1
+
+    @assign_order(Priority.OFTEN_FIRST)
+    def double_value_first(value):
+        return value * 2
+
+    @assign_order(Priority.OFTEN_LAST)
+    def double_value_last(value):
+        return value * 2
+    postprocessing = {"param1": add_1, "param1 ": double_value_first}
+    config = load_config(default_config=yaml_default, postprocessing=postprocessing)
+    check_integrity(config, p_1=1.2, p_2=3.0, p_3=20.0)
+    postprocessing = {"param1": add_1, "param1 ": double_value_last}
+    config = load_config(default_config=yaml_default, postprocessing=postprocessing)
+    check_integrity(config, p_1=2.2, p_2=3.0, p_3=20.0)
+
+
+def test_compose(yaml_default):
+    def add_1(value):
+        return value + 1
+
+    def double_value(value):
+        return value * 2
+
+    postprocessing = {"param1": (add_1, double_value)}
+    config = load_config(default_config=yaml_default, postprocessing=postprocessing)
+    check_integrity(config, p_1=2.2, p_2=3.0, p_3=20.0)
+
+
 def test_warnings(caplog, tmp_file_name):
     # config = ConfigForTests(config_path_or_dictionary={
     #     "param": None, "lparam": [], "dparam": {"param2": 1}})
     # config.merge_from_command_line("--param=1 --lparam=[1] "
     #                                "--dparam={param2:2,param3:3}")
     # captured = capsys.readouterr()
     # assert captured.out.count("is None. It cannot be replaced from the") == 1
@@ -652,15 +700,15 @@
         logging.getLogger("yaecs").propagate = True
         config = make_config({"param": 1}, do_not_merge_command_line=True)
         config.merge({"*d": 1})
     assert caplog.text.count("will be ignored : it does not match any") == 1
 
 
 def test_errors(caplog, yaml_default_unlinked, yaml_default_sub_variations,
-                yaml_default_set_twice, yaml_default):
+                yaml_default_set_twice, yaml_default, yaml_type_check):
     caplog.clear()
     with caplog.at_level(logging.WARNING):
         logging.getLogger("yaecs").propagate = True
         with pytest.raises(
                 Exception, match="'overwriting_regime' needs to be "
                                  "either 'auto-save', 'locked' or 'unsafe'."):
             _ = make_config({"param": 1}, do_not_merge_command_line=True,
@@ -759,7 +807,25 @@
         config = make_config({"subconfig": subconfig})  # don't do this at home
         config.merge({"subconfig": 1})
     with pytest.raises(Exception, match=".* was set twice.*"):
         _ = make_config({
             "param": 1,
             "set_twice_path": yaml_default_set_twice
         }, config_class=template())
+    replacements = {
+        "param_int": 1.2,
+        "param_float": "q",
+        "param_str": None,
+        "param_none": [],
+        "param_bool": {},
+        "param_list": True,
+        "param_dict": 5,
+        "param_listint": [0, 2, "3"],
+        "param_listintstr": ["q", 1],
+        "param_dictlistoptionalint": {"a": [None], "b": [1, None, 2.5]}
+    }
+    for k, v in replacements.items():
+        for prefix in ["", "subconfig."]:
+            with pytest.raises(Exception, match=".*has incorrect type '.*"):
+                print(f"Testing for {prefix + k}")
+                c = load_config(default_config=yaml_type_check)
+                c.merge({prefix + k: v})
```

### Comparing `yaecs-3.1.1/unittests/config/utils.py` & `yaecs-3.2.0/unittests/config/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/usage_example/configs/project_config.py` & `yaecs-3.2.0/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/usage_example/main.py` & `yaecs-3.2.0/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/usage_example/project_utils/utils.py` & `yaecs-3.2.0/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/yaecs/__init__.py` & `yaecs-3.2.0/yaecs/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,17 +35,22 @@
 from .config_history import ConfigHistory  # pylint: disable=wrong-import-position # noqa: E402
 from .experiment import Experiment  # pylint: disable=wrong-import-position # noqa: E402
 from .user_utils import (  # pylint: disable=wrong-import-position # noqa: E402
     get_template_class,
     make_config,
     tqdm_file,
 )
+from .yaecs_utils import (  # pylint: disable=wrong-import-position # noqa: E402
+    assign_order,
+    assign_yaml_tag,
+    Priority,
+)
 
 try:
     from ._version import version as __version__
     from ._version import version_tuple
 except ImportError:
     __version__ = "unknown version"
     version_tuple = (0, 0, "unknown_version")
 
-__all__ = ['__version__', 'version_tuple', 'ConfigHistory', 'Configuration', 'Experiment', 'get_template_class',
-           'make_config', 'tqdm_file']
+__all__ = ['__version__', 'assign_order', 'assign_yaml_tag', 'ConfigHistory', 'Configuration', 'Experiment',
+           'get_template_class', 'make_config', 'Priority', 'tqdm_file', 'version_tuple']
```

### Comparing `yaecs-3.1.1/yaecs/config/config.py` & `yaecs-3.2.0/yaecs/config/config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/yaecs/config/config_base.py` & `yaecs-3.2.0/yaecs/config/config_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,46 +12,54 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+from collections.abc import Iterable
 import copy
 from functools import partial
 import logging
+from numbers import Real
 import os
 from pathlib import Path
 import sys
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TYPE_CHECKING
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TYPE_CHECKING, Union
 import yaml
 
 from .config_getters import ConfigGettersMixin
 from .config_hooks import ConfigHooksMixin
 from .config_setters import ConfigSettersMixin
 from .config_convenience import ConfigConvenienceMixin
 from .config_processing_functions import ConfigProcessingFunctionsMixin
-from ..yaecs_utils import (adapt_to_type, are_same_sub_configs, compare_string_pattern, ConfigDeclarator, format_str,
-                           is_type_valid, parse_type, recursive_set_attribute, TypeHint, update_state, YAML_EXPRESSIONS)
+
+from ..yaecs_utils import (adapt_to_type, are_same_sub_configs, compare_string_pattern, compose, ConfigDeclarator,
+                           format_str, is_type_valid, parse_type, recursive_set_attribute, TypeHint, update_state,
+                           YAML_EXPRESSIONS)
+
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class _ConfigurationBase(ConfigHooksMixin, ConfigGettersMixin, ConfigSettersMixin, ConfigConvenienceMixin,
                          ConfigProcessingFunctionsMixin):
     """ Base class for YAECS configurations. Defines its basic behaviour, such as creation and merging operations,
     including processing- and type checking-related logic, but not its constructors (see Configuration class for those,
     and its docstring for more details about the composition of the Configuration superclass). """
 
+    add_processing_function: Callable[[str, Callable, str], None]
+    add_processing_function_all: Callable[[str, Callable, str], None]
     config_metadata: dict
     parameters_pre_processing: Callable[[], Dict[str, Callable]]
     parameters_post_processing: Callable[[], Dict[str, Callable]]
     _get_instance: Callable
+    _get_tagged_methods_info: Callable[[], List[Tuple[Union[str, Callable]]]]
     _main_config: 'Configuration'
     _methods: List[str]
     _nesting_hierarchy: List[str]
     _operating_creation_or_merging: bool
     _protected_attributes: List[str]
     _state: List[str]
     _verbose: bool
@@ -64,19 +72,24 @@
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :raises ValueError: if the overwriting regime is not valid
         :return: none
         """
 
         # PROTECTED ATTRIBUTES
+        self._assigned_as_yaml_tags = {processor[0]: (processor[3], processor[1], processor[2])
+                                       for processor in self._get_tagged_methods_info()}
         self._former_saving_time = None
         self._from_argv = from_argv
         self._modified_buffer = []
         self._post_process_master_switch = not do_not_post_process
         self._pre_process_master_switch = not do_not_pre_process
+        for process_type in ["pre", "post"]:
+            setattr(self, f"_{process_type}_processing_functions", {})
+            self._prepare_processing_functions(process_type)
         self._pre_postprocessing_values = {}
         self._reference_folder = None
         self._sub_configs_list = []
         self._type_hints = {}
         self._was_last_saved_as = None
         super().__init__()
 
@@ -168,32 +181,25 @@
                     for v_to_check, t_to_check in zip(value, type_to_check):
                         _check_type(v_to_check, t_to_check, original_type)
                 else:
                     types = type_to_check[0] if type_to_check else 0
                     for i in value:
                         _check_type(i, types, original_type)
 
-            elif isinstance(type_to_check, (set, dict)):
+            elif isinstance(type_to_check, dict):
                 if not isinstance(value, dict):
                     _wrong_type()
-                if isinstance(type_to_check, dict):
-                    if type_to_check.keys():
-                        if type_to_check.keys() != value.keys():
-                            raise ValueError("When providing a dict of types, its keys must match those of the value.")
-                        for i in type_to_check:
-                            _check_type(value[i], type_to_check[i], original_type)
-                else:
-                    if not type_to_check:
-                        raise ValueError("Undefined behaviour for empty sets. Maybe you meant to use an empty list or "
-                                         "dict ?")
-                    if len(type_to_check) > 1:
-                        raise ValueError("When providing a set of types, its length must be 1. Maybe you meant to use a"
-                                         " tuple ?")
-                    for i in value:
-                        _check_type(value[i], list(type_to_check)[0], original_type)
+                if not type_to_check:
+                    raise ValueError("Undefined behaviour for empty dicts. Maybe you meant to use an empty list or "
+                                     "{\"type\": ...} ?")
+                if len(type_to_check) > 1:
+                    raise ValueError("When providing a dict of types, its length must be 1. Maybe you meant to use a"
+                                     " tuple ?")
+                for i in value:
+                    _check_type(value[i], type_to_check[list(type_to_check.keys())[0]], original_type)
 
             elif type_to_check != 0 and type_to_check is not None and not isinstance(value, type_to_check):
                 if not (type_to_check is float and isinstance(value, int)):
                     _wrong_type()
 
             elif type_to_check is None and value is not None:
                 _wrong_type()
@@ -351,15 +357,21 @@
 
             if tag[1:].lower().startswith("type:"):
                 if not yaml_loader.constructed_objects:
                     raise RuntimeError(f"'{tag[1:]}' is not a valid sub-config name.")
                 if not any(state.startswith("setup") for state in self._state):
                     raise RuntimeError("Type-hinting is only allowed in the default config.")
                 name = yaml_loader.constructed_objects[list(yaml_loader.constructed_objects.keys())[-1]]
-                self._main_config.add_type_hint(self._get_full_path(name), parse_type(tag[6:]))
+                name = self._get_full_path(name)
+                type_hint = tag[6:]
+                if type_hint in self._assigned_as_yaml_tags:
+                    _, processor_type, new_type_hint = self._assigned_as_yaml_tags[type_hint]
+                    self.add_processing_function_all(name, f"_tagged_method_{type_hint}", processor_type)
+                    type_hint = new_type_hint
+                self._main_config.add_type_hint(name, parse_type(type_hint))
                 if isinstance(node, yaml.ScalarNode):
                     if node.value == "":
                         def _can_be_str(parsed_type):
                             if parsed_type is str:
                                 return True
                             if isinstance(parsed_type, tuple):
                                 if str in parsed_type:
@@ -715,55 +727,91 @@
             self._get_full_path(self._modified_buffer.pop(0))
             for _ in range(len(self._modified_buffer))
         ]
         for subconfig in self.get_all_linked_sub_configs():
             modified_buffer = subconfig.get_modified_buffer()
             for _ in range(len(modified_buffer)):
                 modified.append(".".join(subconfig.get_nesting_hierarchy() + [modified_buffer.pop(0)]))
-        for name in modified:
-            split = name.split(".")[len(self._nesting_hierarchy):]
-            name = ".".join(split)
-            recursive_set_attribute(self,
-                                    ".".join(split[:-1] + ["___" + split[-1]]) if split[-1] in self._methods else name,
-                                    self._process_parameter(name, self[name], "post"),
-                                    )
+        processors = [(proc if isinstance(proc, Callable)
+                       else self._assigned_as_yaml_tags[proc[len("_tagged_method_"):]][0])
+                      for proc in self._post_processing_functions.values()]
+        orders = sorted(list({func.order for func in processors}))
+        splits = [name.split(".")[len(self._nesting_hierarchy):] for name in modified]
+        names = [(".".join(s), ".".join(s[:-1] + ["___" + s[-1]]) if s[-1] in self._methods else ".".join(s))
+                 for s in splits]
+        for order in orders:
+            for name, set_name in names:
+                recursive_set_attribute(self, set_name, self._process_parameter(name, self[name], "post", order))
         post_processed = [param for param in modified if param in self._pre_postprocessing_values]
         if post_processed and self._verbose:
             YAECS_LOGGER.info(f"Performed post-processing for modified parameters {post_processed}.")
 
+    def _prepare_processing_functions(self, processing_type: str) -> None:
+        """ Sets self._pre/post_processing_functions from the user-provided functions. """
+        processing_functions = getattr(self, f"parameters_{processing_type}_processing")()
+        for key, value in processing_functions.items():
+            if not isinstance(value, (Callable, Iterable)):
+                raise TypeError(f"Invalid {processing_type}-processing functions defined for param '{key}' : "
+                                "the function should be declared as either a function or an iterable of functions, "
+                                "optionally containing one order value.")
+            if isinstance(value, Iterable) and not (isinstance(value, str) and value.startswith("_tagged_method_")):
+                if any(not isinstance(element, (Callable, Real)) for element in value):
+                    raise TypeError(f"Invalid {processing_type}-processing functions defined for param '{key}' : "
+                                    "if function is declared as iterable, only functions and one order value can "
+                                    "be provided.")
+                order = [i for i in value if isinstance(i, Real)]
+                if len(order) > 1:
+                    raise ValueError(f"Ambiguous order for {processing_type}-processing functions defined for param "
+                                     f"'{key}' : multiple orders defined ({order}).")
+                processing_function = compose(*[i for i in value if isinstance(i, Callable)])
+                order = order[0] if order else getattr(processing_function, "order", 0)
+            elif isinstance(value, Iterable):  # case where the method is added from a YAML tag
+                self.add_processing_function(key, value, processing_type)
+                continue
+            else:
+                processing_function = value
+                order = getattr(processing_function, "order", 0)
+            processing_function.__dict__["order"] = order
+            self.add_processing_function(key, processing_function, processing_type)
+
     @update_state("processing;_name")
-    def _process_parameter(self, name: str, parameter: Any, processing_type: str) -> Any:
+    def _process_parameter(self, name: str, parameter: Any, processing_type: str, order: Optional[Real] = None) -> Any:
         """ This method checks if a processing function has been defined for given name, then returns the processed
         value when that is the case. """
         if processing_type not in ["pre", "post"]:
             raise ValueError(f"Unknown processing_type : '{processing_type}'. Valid types are 'pre' or 'post'.")
         total_name = self._get_full_path(name)
-        if self._main_config.get_master_switch(processing_type):
+        main = self.get_main_config()
+        if processing_type == "pre":
+            main.remove_value_before_postprocessing(total_name)
+        if main.get_master_switch(processing_type):
             old_value = None
             if processing_type == "pre":
-                self.check_type(self.get_type_hint(name))(parameter)
-                transformation_dict = self.parameters_pre_processing()
+                self.check_type(main.get_type_hint(total_name))(parameter)
             else:
                 old_value = copy.deepcopy(parameter)
-                transformation_dict = self.parameters_post_processing()
-            was_processed = False
-            for key, item in transformation_dict.items():
-                if compare_string_pattern(total_name, key):
-                    was_processed = True
-                    try:
-                        parameter = item(parameter)
-                    except Exception:
-                        YAECS_LOGGER.error(f"ERROR while {processing_type}-processing param '{total_name}' :")
-                        raise
+            processors = [proc for key, proc in getattr(self, f"_{processing_type}_processing_functions").items()
+                          if compare_string_pattern(total_name, key)]
+            processors = [(proc if isinstance(proc, Callable)
+                           else self._assigned_as_yaml_tags[proc[len("_tagged_method_"):]][0]) for proc in processors]
+            processors = sorted([p for p in processors if order is None or p.order == order], key=lambda x: x.order)
+            was_processed = bool(processors)
+            for processor in processors:
+                try:
+                    parameter = processor(parameter)
+                except Exception:
+                    YAECS_LOGGER.error(f"ERROR while {processing_type}-processing param '{total_name}' :")
+                    raise
             if processing_type == "pre" and not is_type_valid(parameter, _ConfigurationBase):
                 raise RuntimeError(f"ERROR while pre-processing param '{total_name}' : "
                                    "pre-processing functions that change the type of a "
                                    "param to a non-native YAML type are forbidden because "
                                    "they cannot be saved. Please use a parameter "
                                    "post-processing instead.")
             if processing_type == "post" and was_processed:
-                self.get_main_config().save_value_before_postprocessing(self._get_full_path(name), old_value)
+                main.save_value_before_postprocessing(self._get_full_path(name), old_value)
         elif processing_type == "pre":
-            for key, item in self.parameters_pre_processing().items():
+            for key, item in self._pre_processing_functions.items():
                 if compare_string_pattern(total_name, key) and item.__name__.startswith("yaecs_config_hook__"):
-                    self.add_currently_processed_param_as_hook(item.__name__.split("__")[1])
+                    for hook_name in item.__name__.split("__")[1].split(","):
+                        self.add_currently_processed_param_as_hook(hook_name)
         return parameter
```

### Comparing `yaecs-3.1.1/yaecs/config/config_convenience.py` & `yaecs-3.2.0/yaecs/config/config_convenience.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     _get_user_defined_attributes: Callable[[], List[str]]
     _methods: List[str]
     _nesting_hierarchy: List[str]
     _protected_attributes: List[str]
     _verbose: bool
     _was_last_saved_as: Optional[str]
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, ConfigConvenienceMixin):
             return False
         for param in self._get_user_defined_attributes():
             try:
                 if self[param] != other[param]:
                     return False
```

### Comparing `yaecs-3.1.1/yaecs/config/config_getters.py` & `yaecs-3.2.0/yaecs/config/config_getters.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import logging
-from typing import Any, Callable, Dict, List, Union, TYPE_CHECKING, Optional
+from typing import Any, Callable, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 
 from ..yaecs_utils import get_param_as_parsable_string, escape_symbols, TypeHint
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
@@ -41,14 +41,17 @@
     _reference_folder: Optional[str]
     _state: List[str]
     _sub_configs_list: List['Configuration']
     _type_hints: Dict[str, TypeHint]
     _variation_name: str
     _was_last_saved_as: Optional[str]
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
     def get(self, parameter_name: str, default_value: Any) -> Any:
         """
         Behaves similarly to dict.get(parameter_name, default_value)
         :param parameter_name: parameter to query
         :param default_value: value to return if the parameter does not exist
         :return: queried value
         """
@@ -263,14 +266,20 @@
                     raise ValueError("How did you even manage to raise this ?")
                 name = state.split(";arg0=")[-1]
                 break
         if name is None:
             raise RuntimeError("Processing function was called outside a processing phase.")
         return name
 
+    def _get_tagged_methods_info(self) -> List[Tuple[Union[str, Callable]]]:
+        """ Returns a list of info on the methods which were assigned a YAML tag. """
+        all_methods = [getattr(self, name) for name in self._methods]
+        return [getattr(method, "assigned_yaml_tag") + (method,)
+                for method in all_methods if hasattr(method, "assigned_yaml_tag")]
+
     def _get_user_defined_attributes(self, no_sub_config: bool = False) -> List[str]:
         """ Frequently used to get a list of the names of all the parameters that were in the user's config. """
         return [
             i[3:] if i.startswith("___") else i
             for i in self.__dict__
             if (i not in self._protected_attributes + ["config_metadata"]
                 and not (no_sub_config and isinstance(self[i], ConfigGettersMixin)))
```

### Comparing `yaecs-3.1.1/yaecs/config/config_hooks.py` & `yaecs-3.2.0/yaecs/config/config_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import logging
 import os
 from typing import Any, Callable, List, Optional, Tuple, Union
 
-from ..yaecs_utils import ConfigDeclarator, hook, Hooks, VariationDeclarator
+from ..yaecs_utils import assign_order, assign_yaml_tag, ConfigDeclarator, hook, Hooks, Priority, VariationDeclarator
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigHooksMixin:
     """ Hooks Mixin class for YAECS configurations. Implements processing functions whose name start with "register_as_"
     and are decorated by the yaecs_utils.hook decorator. Users can use those processing either as pre- or
@@ -36,16 +36,17 @@
     get_variation_name: Callable[[], str]
     init_from_config: Callable[[ConfigDeclarator], None]
     _configuration_variations: List[Tuple[str, List[ConfigDeclarator]]]
     _configuration_variations_names: List[Tuple[str, List[str]]]
     _grids: List[List[str]]
     _nesting_hierarchy: List[str]
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         self._hooks = {}
+        super().__init__(*args, **kwargs)
 
     def add_currently_processed_param_as_hook(self, hook_name: str) -> None:
         """
         Used within _ConfigurationBase._process_parameter to add the param currently being processed as a hook with
         given name. Instead of using this directly, users should consider decorating their hooking function with the
         yaecs_utils.hook decorator.
         :param hook_name: name of the hook to add.
@@ -79,34 +80,46 @@
         :return: list of hooked parameter names
         """
         if hook_name is None:
             return self._hooks
         return self._hooks[hook_name] if hook_name in self._hooks else []
 
     @hook("additional_config_file")
+    @assign_order(Priority.OFTEN_LAST)  # processing this param after this function makes it unclear which file was used
+    @assign_yaml_tag("additional_config_file", "pre", "Optional[Union[str,List[str]]]")
     def register_as_additional_config_file(self, path: Union[str, List[str]]) -> Union[str, List[str]]:
         """
         Pre-processing function used to register the corresponding parameter as a path to another config file. The new
         config file will then also be used to build the config currently being built.
+
+        Priority : OFTEN_LAST (10)
+        YAML tag : additional_config_file
+
         :param path: config's path or list of paths
         :return: the same path as the input once the parameters from the new config have been added
         """
         if isinstance(path, list):
             for individual_path in path:
                 self.init_from_config(individual_path)
         else:
             self.init_from_config(path)
         return path
 
     @hook("config_variations")
+    @assign_order(Priority.INDIFFERENT)  # does not depend on or change parameter value, only processes parameter name
+    @assign_yaml_tag("config_variations", "pre", "Optional[Union[List[Union[str,dict]],Dict[Union[str,dict]]]]")
     def register_as_config_variations(
             self, variation_to_register: Optional[VariationDeclarator]) -> Optional[VariationDeclarator]:
         """
         Pre-processing function used to register the corresponding parameter as a variation for the current config.
         Please note that config variations need to be declared in the root config.
+
+        Priority : INDIFFERENT (0)
+        YAML tag : config_variations
+
         :param variation_to_register: list of configs
         :return: the same list of configs once the configs have been added to the internal variation tracker
         :raises RuntimeError: register_as_config_variations is called outside _pre_process_parameter
         :raises RuntimeError: variation name invalid in sub-config
         :raises TypeError: type of variation is not list or dict of configs
         """
         name = self.get_processed_param_name(full_path=False)
@@ -139,21 +152,27 @@
             raise TypeError("Variations parsing failed : variations parameters must "
                             "be a list of configs or a dict containing only configs. "
                             f"Instead, got : {variation_to_register}")
 
         return variation_to_register
 
     @hook("experiment_path")
-    def register_as_experiment_path(self, path: str) -> str:
+    @assign_order(Priority.OFTEN_FIRST)  # other params might depend on this being done (eg. for folder_in_experiment)
+    @assign_yaml_tag("experiment_path", "post", "Optional[str]")
+    def register_as_experiment_path(self, path: Optional[str]) -> Optional[str]:
         """
         Pre-processing function used to register the corresponding parameter as the folder used for the current
         experiment. This will automatically create the relevant folder structure and append an experiment index at the
         end of the folder name to avoid any overwriting. The path needs to be either None or an empty string (in which
         case the pre-processing does not happen), or an absolute path, or a path relative to the current working
         directory.
+
+        Priority : OFTEN_FIRST (-10)
+        YAML tag : experiment_path
+
         :param path: None, '', absolute path or path relative to the current working directory
         :return: the actual created path with its appended index
         """
         if not path:
             return path
         folder, experiment = (os.path.dirname(path), os.path.basename(path))
         if not folder:
@@ -172,37 +191,49 @@
         else:
             path = os.path.join(folder, f"{experiment}_{max(run_ids)}", self.get_variation_name())
         if new_folder:
             os.makedirs(path, exist_ok=True)
         return path
 
     @hook("grid")
+    @assign_order(Priority.INDIFFERENT)  # does not depend on or change parameter value, only processes parameter name
+    @assign_yaml_tag("grid", "pre", "Optional[List[str]]")
     def register_as_grid(self, list_to_register: Optional[List[str]]) -> Optional[List[str]]:
         """
         Pre-processing function used to register the corresponding parameter as a grid for the current config. Grids are
         made of several parameters registered as variations. Instead of adding the variations in those parameters to the
         list of variations for this config, a grid will be created and all its components will be added instead.
+
+        Priority : INDIFFERENT (0)
+        YAML tag : grid
+
         :param list_to_register: list of parameters composing the grid
         :raises TypeError: list_to_register is not recognised as a valid grid
         :return: the same list of parameters once the grid has been added to the internal grid tracker
         """
         if isinstance(list_to_register, list) and all(isinstance(param, str) for param in list_to_register):
             self._grids.append(list_to_register)
         elif list_to_register is not None:
             raise TypeError("Grid parsing failed : unrecognised grid declaration : "
                             f"{list_to_register}")
         return list_to_register
 
     @hook("tracker_config")
+    @assign_order(Priority.INDIFFERENT)  # does not depend on or change parameter value, only processes parameter name
+    @assign_yaml_tag("tracker_config", "pre", "dict")
     def register_as_tracker_config(self, tracker_config: dict) -> dict:  # pylint: disable=no-self-use
         """
         Pre-processing function used to register the corresponding parameter as the tracker config. The tracker config
         is a dict that contains at least one key : 'type'. Valid types are given by the 'ACCEPTED_TRACKERS' variable in
         experiment.py and refer to the type of tracker used. Other keys in the dict depend on the parameters required by
         corresponding tracker type.
+
+        Priority : INDIFFERENT (0)
+        YAML tag : tracker_config
+
         :param tracker_config: dict corresponding to the tracker config
         :raises: ValueError: if the tracker config is not a dict or does not contain at least a parameter called 'type'
         which is a string
         :raises: ValueError: if the 'type' is not recognised
         :raises: ValueError: if there are missing required keys for this 'type'
         :return: the same dict
         """
```

### Comparing `yaecs-3.1.1/yaecs/config/config_setters.py` & `yaecs-3.2.0/yaecs/config/config_setters.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,83 +13,113 @@
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 from functools import partial
 import logging
-from typing import Any, Callable, Dict, TYPE_CHECKING
+from typing import Any, Callable, Dict, TYPE_CHECKING, Union
 
-from ..yaecs_utils import TypeHint
+from ..yaecs_utils import Priority, TypeHint
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigSettersMixin:
     """ Setters Mixin class for YAECS configurations. """
 
     _main_config: 'Configuration'
     _pre_postprocessing_values: Dict[str, Any]
     _type_hints: Dict[str, TypeHint]
 
-    def add_processing_function(self, param_name: str, function_to_add: Callable, processing_type: str) -> None:
-        """
-        If given parameter does not already have a post-processing function with the same name, adds given function as
-        a post-processing function to parameters with the given name.
-        :param param_name: parameter(s) to which to add a postprocessing function
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def add_processing_function(self, param_name: str, function_to_add: Union[str, Callable], processing_type: str
+                                ) -> None:
+        """ If given parameter does not already have a post-processing function with the same name, adds given function
+        as a post-processing function to parameters with the given name. """
+        attribute = f"_{processing_type}_processing_functions"
+        current_processing = object.__getattribute__(self, attribute)
+        set_name = param_name
+        while set_name in current_processing:
+            set_name = set_name + " "
+        new_processing = {set_name: function_to_add, **current_processing}
+        object.__setattr__(self, attribute, new_processing)
+
+    def add_processing_function_all(self, param_name: str, function_to_add: Union[str, Callable], processing_type: str
+                                    ) -> None:
+        """
+        Triggers add_processing_function on the main config and all defined and future sub-configs.
+        :param param_name: parameter(s) to which to add a postprocessing function. Expects paths with respect to the
+        main config.
         :param function_to_add: postprocessing function to add, using the generic name "function" if it has no name
         :param processing_type: choose between 'pre' to add a pre-processing function or 'post' to add a post-processing
         function
         """
-        function_name = function_to_add.__name__ if hasattr(function_to_add, "__name__") else "function"
-        method = f"parameters_{processing_type}_processing"
-        current_processing = object.__getattribute__(self._main_config, method)()
-        param_matches = self.match_params(param_name)
-        if not any((all(i in self._main_config.match_params(k) for i in param_matches) and v.__name__ == function_name)
-                   for k, v in current_processing.items()):
-            if param_name in current_processing:
-                def _composition(x, processing_dict, name, func):
-                    return processing_dict[name](func(x))
-                _composition = partial(_composition,
-                                       processing_dict=current_processing, name=param_name, func=function_to_add)
-                _composition.__name__ = "function_name"
-                del current_processing[param_name]
-                new_processing = {param_name: _composition, **current_processing}
-            else:
-                new_processing = {param_name: function_to_add, **current_processing}
-            object.__setattr__(self._main_config.__class__, method, lambda x: new_processing)
+        if isinstance(function_to_add, str):
+            check_function = getattr(self.__class__, function_to_add[len("_tagged_method_"):])
         else:
-            YAECS_LOGGER.warning(f"WARNING : Parameter '{param_name}' already has a post-processing function with the "
-                                 f"name '{function_name}'. Processing function will not be added again.")
+            check_function = function_to_add
+        if not hasattr(check_function, "order"):
+            check_function.__dict__["order"] = Priority.INDIFFERENT
+        if hasattr(check_function, "assigned_yaml_tag"):
+            if check_function.assigned_yaml_tag[1] != processing_type:
+                name = "unknown_function" if not hasattr(check_function, "__name__") else check_function.__name__
+                YAECS_LOGGER.warning(f"WARNING : processing function {name} is recommended to use "
+                                     f"as {check_function.assigned_yaml_tag[1]}-processing function, "
+                                     f"but was declared as {processing_type}-processing function.")
+        # Add to main config
+        self._main_config.add_processing_function(param_name, function_to_add, processing_type)
+        # Add to current sub-configs
+        for subconfig in self._main_config.get_all_sub_configs():
+            subconfig.add_processing_function(param_name, function_to_add, processing_type)
+        # Add to future sub-configs
+        attribute = f"parameters_{processing_type}_processing"
+        current_processing = object.__getattribute__(self, attribute)()
+        set_name = param_name
+        while set_name in current_processing:
+            set_name = set_name + " "
+        new_processing = {set_name: function_to_add, **current_processing}
+        setattr(self.__class__, attribute, lambda self: new_processing)
 
     def add_type_hint(self, name: str, type_hint: TypeHint) -> None:
         """
         Adds a type hint for a parameter to the list of type hints for automatic type checks.
         :param name: full path of the param in the main config
         :param type_hint: type of the param
         """
         self._type_hints[name] = type_hint
 
+    def remove_value_before_postprocessing(self, name: str) -> None:
+        """
+        Function used for bookkeeping : it remove a parameter from the pre-post-processing archive.
+        :param name: name of the parameter using the dot convention
+        """
+        if name in self._pre_postprocessing_values:
+            del self._pre_postprocessing_values[name]
+
     def remove_type_hint(self, param_name: str) -> None:
         """
         Removes a registered type hint from a param with given name
         :param param_name: param from which to remove the type hint
         """
         if param_name in self._type_hints:
             del self._type_hints[param_name]
 
     def save_value_before_postprocessing(self, name: str, value: Any) -> None:
         """
         Function used for bookkeeping : it saves the value a parameter had before its post-processing.
         :param name: name of the parameter using the dot convention
         :param value: value of the parameter before post-processing
         """
-        self._pre_postprocessing_values[name] = value
+        if name not in self._pre_postprocessing_values:
+            self._pre_postprocessing_values[name] = value
 
     def set_post_processing(self, value: bool = True) -> None:
         """
         Sets the state of the master switch for pre-processing across the entire config object. Calling this for a
         sub-config will also affect the main config and all other sub-configs.
         :param value: value to set the pre-processing to
         """
```

### Comparing `yaecs-3.1.1/yaecs/config_history.py` & `yaecs-3.2.0/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/yaecs/experiment.py` & `yaecs-3.2.0/yaecs/experiment.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/yaecs/pytorch_lightning_utils.py` & `yaecs-3.2.0/yaecs/pytorch_lightning_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/yaecs/user_utils.py` & `yaecs-3.2.0/yaecs/user_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.1.1/yaecs/yaecs_utils.py` & `yaecs-3.2.0/yaecs/yaecs_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,25 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-import sys
 import functools
 import importlib.util
 import io
 import logging
 import os
 import re
+import sys
+from enum import Enum
 from bisect import bisect
 from collections.abc import Mapping
+from numbers import Real
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Union
 
 YAECS_LOGGER = logging.getLogger(__name__)
 ConfigDeclarator = Union[str, dict]
 Hooks = Union[Dict[str, List[str]], List[str]]
 TypeHint = Union[type, tuple, list, dict, set, int]
@@ -248,35 +250,93 @@
     """
     if first.get_name() != second.get_name():
         return False
     nh1, nh2 = first.get_nesting_hierarchy(), second.get_nesting_hierarchy()
     return len(nh1) == len(nh2) and all(nh1[i] == nh2[i] for i in range(len(nh1)))
 
 
+def assign_order(order: float = 0) -> Callable[[Callable], Callable]:
+    """
+    Decorator used to give an order to a processing function. If several processing functions would be called at a given
+    step, they are called in increasing order.
+    :param order: order to give the function
+    :return: decorated function
+    """
+    def decorator_order(func: Callable) -> Callable:
+        func.__dict__["order"] = order
+        return func
+
+    return decorator_order
+
+
+def assign_yaml_tag(processor_tag: str, processor_type: str,
+                    replacement_type_hint: str = "Any") -> Callable[[Callable], Callable]:
+    """
+    Decorator used to mark a function as a processor added automatically as pre or post processing function (as
+    defined by processor_type) to parameters tagged with !type:<processor_tag>. Their type hint will be replaced by
+    the type hint defined as replacement_type_hint.
+    :param processor_tag: tag to use to mark a param in YAML as auto-processed by this function
+    :param processor_type: 'pre' or 'post', type of processing function to add
+    :param replacement_type_hint: type hint to use for any param tagged with this auto-processor
+    :return: decorated function
+    """
+    def decorator_tag_assignment(func: Callable) -> Callable:
+        func.__dict__["assigned_yaml_tag"] = (processor_tag, processor_type, replacement_type_hint)
+        return func
+
+    return decorator_tag_assignment
+
+
 def compare_string_pattern(name: str, pattern: str) -> bool:
     """
     Returns True when string 'name' matches string 'pattern',
     with the '*' character matching any number of characters.
     :param name: name to compare
     :param pattern: pattern to match
     :return: result of comparison
     """
-    pattern = pattern.split("*")
+    pattern = pattern.strip(" ").split("*")
     if len(pattern) == 1:
         return pattern[0] == name
     if not (name.startswith(pattern[0]) and name.endswith(pattern[-1])):
         return False
     for fragment in pattern:
         index = name.find(fragment)
         if index == -1:
             return False
         name = name[index + len(fragment):]
     return True
 
 
+def compose(*functions: Callable) -> Callable:
+    """
+    Returns the composition of the functions given as argument. Functions are applied from left to right, ie :
+    compose(f, g, h)(x) = h(g(f(x))).
+    :param functions: all functions to compose, applied from left to right
+    :return: the composed function
+    """
+    def compose_2(function_1, function_2):
+        def composed(*args, **kwargs):
+            return function_2(function_1(*args, **kwargs))
+        orders = []
+        for func in [function_1, function_2]:
+            if hasattr(func, "order"):
+                orders.append(func.order)
+        if orders:
+            composed.__dict__["order"] = max(orders)
+        hooks = []
+        for func in [function_1, function_2]:
+            if func.__name__.startswith("yaecs_config_hook__"):
+                hooks += func.__name__.split("__")[1].split(",")
+        if hooks:
+            composed.__name__ = f"yaecs_config_hook__{','.join(list(set(hooks)))}__composed"
+        return composed
+    return functools.reduce(compose_2, functions, lambda x: x)
+
+
 def dict_apply(dictionary: dict, function: Callable) -> dict:
     """
     Returns a copy of dict 'dictionary' where function 'function'
     was applied to all values.
     :param dictionary: dictionary to copy
     :param function: function to map
     :return: copied dictionary
@@ -359,35 +419,47 @@
 def hook(hook_name: str) -> Callable[[Callable], Callable]:
     """
     Decorator used to keep track of registered params.
     :param hook_name: name of the hook to store
     :return: decorated function
     """
     def decorator_hook(func: Callable) -> Callable:
-        func.__name__ = f"yaecs_config_hook__{hook_name}__{func.__name__}"
+        if func.__name__.startswith("yaecs_config_hook__"):
+            hooks = func.__name__.split("__")[1].split(",")
+            if hook_name in hooks:
+                hook_name_in_func_name = ",".join(hooks)
+            else:
+                hook_name_in_func_name = ",".join(hooks + [hook_name])
+            original_name = "__".join(func.__name__.split("__")[2:])
+        else:
+            hook_name_in_func_name = hook_name
+            original_name = func.__name__
+        func.__name__ = f"yaecs_config_hook__{hook_name_in_func_name}__{original_name}"
 
         @functools.wraps(func)
         def wrapper_hook(self, *args, **kwargs):
             value = func(self, *args, **kwargs)
             self.add_currently_processed_param_as_hook(hook_name=hook_name)
             return value
 
+        for function_attribute in ["order", "assigned_yaml_tag"]:
+            if hasattr(func, function_attribute):
+                setattr(wrapper_hook, function_attribute, getattr(func, function_attribute))
         return wrapper_hook
-    if "__" in hook_name:
-        raise RuntimeError(f"Invalid hook name {hook_name} : '__' is not allowed in hook names.")
+    for invalid_pattern in ["__", ","]:
+        if invalid_pattern in hook_name:
+            raise RuntimeError(f"Invalid hook name {hook_name} : '{invalid_pattern}' is not allowed in hook names.")
     return decorator_hook
 
 
 def is_type_valid(value: Any, config_class: type) -> bool:
     """
-    Checks whether input 'value' can be saved in a YAML file by
-    Configuration's YAML Dumper.
+    Checks whether input 'value' can be saved in a YAML file by Configuration's YAML Dumper.
     :param value: value to check the type of
-    :param config_class: Configuration class, which must be passed as
-    argument to avoid circular imports :(
+    :param config_class: Configuration class, which must be passed as argument to avoid circular imports :(
     :return: result of the test
     """
     if isinstance(value, list):
         return all(is_type_valid(i, config_class) for i in value)
     if isinstance(value, (Mapping, config_class)):
         return all(is_type_valid(i, config_class) for i in value.values())
     return isinstance(value, (int, float, str)) or value is None
@@ -421,15 +493,15 @@
     :param end: suffix to add after the message
     :param file: file to print to, defaults to a logging to logging's root logger with level logging.INFO
     :param keywords: might contain 'flush', in which case raise an error
     :raises TypeError: when the keyword arguments contain 'flush'
     """
     if not os.getenv('NODE_RANK'):  # do not print if in a pytorch-lightning spawned process
         if "flush" in keywords:
-            raise TypeError("Because yaecs uses logging.info to log messages logged via the print function, the 'flush'"
+            raise TypeError("Because YAECS uses logging.info to log messages logged via the print function, the 'flush'"
                             " parameter is not supported for the print function within your main.")
         message = sep.join([str(a) for a in args]) + end.strip()
         if message.strip():
             if file is not None and file is not sys.stdout:
                 file.write(message)
             logging.getLogger("yaecs.print_catcher").info(message)
 
@@ -440,17 +512,21 @@
     Configuration.check_type function.
     :param string_to_process: string to parse for type
     :return: complex type
     """
     if not string_to_process:
         raise ValueError("Invalid type hint : empty type hint.")
     string = string_to_process.lower()
-    types = {"none": None, "int": int, "float": float, "bool": bool, "str": str, "list": list, "dict": dict}
-    mapping_starts = {"(": "tuple", "[": "list", "d": "set"}
-    mapping_ends = {")": "tuple", "]": "list", "/d": "set"}
+    mapping_starts = {"tuple_0": "(", "tuple_1": "union[", "nonetuple": "optional[",
+                      "list_0": "[", "list_1": "list[",
+                      "set_0": "d", "set_1": "dict["}
+    types = {"none": None, "int": int, "float": float, "bool": bool, "str": str, "list": list, "dict": dict, "any": 0}
+    mapping_ends = {"tuple_0": ")", "tuple_1": "]", "nonetuple": "]",
+                    "list_0": "]", "list_1": "]",
+                    "set_0": "/d", "set_1": "]"}
     to_return = ("root", [])
     current = []
     current_types = []
     i = 0
 
     def _get_sub_list(lists, path):
         list_to_get = lists
@@ -465,79 +541,144 @@
     def _enter_list(lists, path, path_types, path_type):
         list_to_enter = _get_sub_list(lists, path)
         path.append(len(list_to_enter)-1)
         path_types.append(path_type)
 
     while i < len(string):
         to_find = True
-        for key, value in types.items():
-            if to_find and string[i] == key[0]:
-                if string[i:i+len(key)] == key:
+        # Try to detect starts of mappings
+        for type_name, fragment in mapping_starts.items():
+            if to_find and string[i:i+len(fragment)] == fragment:
+                if not (fragment == "d" and string[i:i+len("dict")] == "dict"):
                     to_find = False
-                    _increment(to_return, current, value, "type")
-                    i += len(key)
-                elif string[i] == "d":
-                    pass
-                else:
-                    raise ValueError(f"Parsing error : unknown type starting from position {i} : "
-                                     f"{string_to_process}.")
+                    _increment(to_return, current, [], type_name)
+                    _enter_list(to_return, current, current_types, type_name)
+                    i += len(fragment)
+        # Try to detect simple types
+        for fragment, type_name in types.items():
+            if to_find and string[i:i+len(fragment)] == fragment:
+                to_find = False
+                _increment(to_return, current, type_name, "type")
+                i += len(fragment)
+        # Try to detect commas
         if to_find and string[i] == ",":
             to_find = False
             i += 1
-        for key, value in mapping_starts.items():
-            if to_find and string[i] == key[0]:
-                if string[i:i+len(key)] == key:
-                    to_find = False
-                    _increment(to_return, current, [], value)
-                    _enter_list(to_return, current, current_types, value)
-                    i += len(key)
-                else:
-                    raise ValueError(f"Parsing error : unknown mapping type starting from position {i} : "
-                                     f"{string_to_process}.")
-        for key, value in mapping_ends.items():
-            if to_find and string[i] == key[0]:
-                if string[i:i+len(key)] == key:
-                    if current_types[-1] != value:
-                        raise ValueError(f"Parsing error : did not expect symbol '{key}' at position {i} : "
-                                         f"{string_to_process}")
-                    to_find = False
-                    current = current[:-1]
-                    current_types = current_types[:-1]
-                    i += len(key)
-                else:
-                    raise ValueError(f"Parsing error : unknown mapping type ending at position {i} : "
-                                     f"{string_to_process}.")
+        # Try to detect ends of mappings
+        for type_name, fragment in mapping_ends.items():
+            if to_find and string[i:i+len(fragment)] == fragment and current_types[-1] == type_name:
+                to_find = False
+                current = current[:-1]
+                current_types = current_types[:-1]
+                i += len(fragment)
         if to_find:
-            raise ValueError(f"Unknown token at position {i} : {string_to_process}")
+            raise ValueError(f"Unexpected token at position {i} : {string_to_process}")
 
     if current:
         raise ValueError(f"Parsing error : unclosed brackets : {string_to_process}")
 
     def _struc_to_type(structured_list):
         list_to_consider = structured_list[1]
         if len(list_to_consider) != 1:
             raise ValueError("Parsing error : a source type must contain exactly 1 type (simple or complex) : "
                              f"{string_to_process}")
-        if list_to_consider[0][0] == "type":
+        if list_to_consider[0][0].startswith("type"):
             return list_to_consider[0][1]
-        if list_to_consider[0][0] == "tuple":
+        if list_to_consider[0][0].startswith("tuple"):
             if not list_to_consider[0][1]:
                 raise ValueError(f"Parsing error : empty tuples are not allowed : {string_to_process}")
             return tuple(_struc_to_type(("", [j])) for j in list_to_consider[0][1])
-        if list_to_consider[0][0] == "list":
+        if list_to_consider[0][0].startswith("nonetuple"):
+            if not list_to_consider[0][1]:
+                raise ValueError(f"Parsing error : empty tuples are not allowed : {string_to_process}")
+            return (None,) + tuple(_struc_to_type(("", [j])) for j in list_to_consider[0][1])
+        if list_to_consider[0][0].startswith("list"):
             if not list_to_consider[0][1]:
                 raise ValueError(f"Parsing error : empty lists are not allowed : {string_to_process}")
             return list(_struc_to_type(("", [j])) for j in list_to_consider[0][1])
-        if list_to_consider[0][0] == "set":
-            return {_struc_to_type(("", list_to_consider[0][1]))}
+        if list_to_consider[0][0].startswith("set"):
+            return {"type": _struc_to_type(("", list_to_consider[0][1]))}
         return None
 
     return _struc_to_type(to_return)
 
 
+class Priority(Enum):
+    """ Define priority levels which can be used to qualify when a processing function should be performed. """
+    ALWAYS_FIRST = -20
+    OFTEN_FIRST = -10
+    INDIFFERENT = 0
+    SITUATIONAL = 0
+    OFTEN_LAST = 10
+    ALWAYS_LAST = 20
+
+    def __hash__(self):
+        return hash(self.value)
+
+    def __gt__(self, other):
+        if self.__class__ is other.__class__:
+            return self.value > other.value
+        if isinstance(other, Real):
+            return self.value > other
+        if isinstance(other, str):
+            return self.value > getattr(self.__class__, other)
+        return NotImplemented
+
+    def __rgt__(self, other):
+        return self < other
+
+    def __lt__(self, other):
+        if self.__class__ is other.__class__:
+            return self.value < other.value
+        if isinstance(other, Real):
+            return self.value < other
+        if isinstance(other, str):
+            return self.value < getattr(self.__class__, other)
+        return NotImplemented
+
+    def __rlt__(self, other):
+        return self > other
+
+    def __ge__(self, other):
+        if self.__class__ is other.__class__:
+            return self.value >= other.value
+        if isinstance(other, Real):
+            return self.value >= other
+        if isinstance(other, str):
+            return self.value >= getattr(self.__class__, other)
+        return NotImplemented
+
+    def __rge__(self, other):
+        return self <= other
+
+    def __le__(self, other):
+        if self.__class__ is other.__class__:
+            return self.value <= other.value
+        if isinstance(other, Real):
+            return self.value <= other
+        if isinstance(other, str):
+            return self.value <= getattr(self.__class__, other)
+        return NotImplemented
+
+    def __rle__(self, other):
+        return self >= other
+
+    def __eq__(self, other):
+        if self.__class__ is other.__class__:
+            return self.value == other.value
+        if isinstance(other, Real):
+            return self.value == other
+        if isinstance(other, str):
+            return self.name == other
+        return NotImplemented
+
+    def __req__(self, other):
+        return self == other
+
+
 def recursive_set_attribute(obj: Any, key: str, value: Any) -> None:
     """
     Recursively gets attributes of 'obj' until object.__setattr__
     can be used to force-set parameter 'key' to value 'value'.
     :param obj: object where to set the key to the value
     :param key: attribute of the object to set recursively
     :param value: value to set
@@ -547,20 +688,17 @@
         recursive_set_attribute(obj[subconfig], key, value)
     else:
         object.__setattr__(obj, key, value)
 
 
 def update_state(state_descriptor: str) -> Callable[[Callable], Callable]:
     """
-    Decorator used to store useful information in Configuration._state
-    when using some recursive functions. Kind of a hack, but very useful
-    to keep track of the loading state and also
-    to debug.
-    :param state_descriptor: string indicating what to store in
-    Configuration._state
+    Decorator used to store useful information in Configuration._state when using some recursive functions. Kind of a
+    hack, but very useful to keep track of the loading state and also to debug.
+    :param state_descriptor: string indicating what to store in Configuration._state
     :return: decorated function
     """
 
     def decorator_update_state(func: Callable) -> Callable:
 
         @functools.wraps(func)
         def wrapper_update_state(self, *args, **kwargs):
```

### Comparing `yaecs-3.1.1/yaecs.egg-info/PKG-INFO` & `yaecs-3.2.0/yaecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.1.1
+Version: 3.2.0
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.1.1/yaecs.egg-info/SOURCES.txt` & `yaecs-3.2.0/yaecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

