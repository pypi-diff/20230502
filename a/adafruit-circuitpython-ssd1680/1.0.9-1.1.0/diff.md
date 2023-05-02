# Comparing `tmp/adafruit-circuitpython-ssd1680-1.0.9.tar.gz` & `tmp/adafruit-circuitpython-ssd1680-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1680-1.0.9.tar", last modified: Tue Aug  9 19:58:32 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1680-1.1.0.tar", last modified: Tue May  2 17:06:59 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1680-1.0.9.tar` & `adafruit-circuitpython-ssd1680-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.944716 adafruit-circuitpython-ssd1680-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-08-09 19:58:32.000000 adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-08-09 19:58:32.000000 adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:58:32.000000 adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-09 19:58:32.000000 adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-09 19:58:32.000000 adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     3025 2022-08-09 19:58:25.000000 adafruit-circuitpython-ssd1680-1.0.9/adafruit_ssd1680.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   360122 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-08-09 19:58:25.000000 adafruit-circuitpython-ssd1680-1.0.9/examples/ssd1680_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-08-09 19:58:25.000000 adafruit-circuitpython-ssd1680-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-09 19:58:18.000000 adafruit-circuitpython-ssd1680-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:58:32.948716 adafruit-circuitpython-ssd1680-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.033716 adafruit-circuitpython-ssd1680-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.033716 adafruit-circuitpython-ssd1680-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.033716 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3231 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_ssd1680.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   360122 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_2.13_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_2.13_tricolor_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_four_corners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1680-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/.gitignore` & `adafruit-circuitpython-ssd1680-1.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1680-1.1.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/.pylintrc` & `adafruit-circuitpython-ssd1680-1.1.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1680-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/LICENSE` & `adafruit-circuitpython-ssd1680-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1680-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1680-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1680-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/PKG-INFO` & `adafruit-circuitpython-ssd1680-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1680
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython `displayio` drivers for SSD1680-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1680
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1680,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/README.rst` & `adafruit-circuitpython-ssd1680-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1680
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython `displayio` drivers for SSD1680-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1680
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1680,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_ssd1680.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ssd1680.egg-info/PKG-INFO
 adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt
 adafruit_circuitpython_ssd1680.egg-info/dependency_links.txt
 adafruit_circuitpython_ssd1680.egg-info/requires.txt
@@ -30,8 +31,11 @@
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/display-ruler.bmp
 examples/display-ruler.bmp.license
+examples/ssd1680_2.13_featherwing.py
+examples/ssd1680_2.13_tricolor_breakout.py
+examples/ssd1680_four_corners.py
 examples/ssd1680_simpletest.py
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/adafruit_ssd1680.py` & `adafruit-circuitpython-ssd1680-1.1.0/adafruit_ssd1680.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 Implementation Notes
 --------------------
 
 **Hardware:**
 
 * `Adafruit 2.13" Tri-Color eInk Display Breakout <https://www.adafruit.com/product/4947>`_
 * `Adafruit 2.13" Tri-Color eInk Display FeatherWing <https://www.adafruit.com/product/4814>`_
+* `Adafruit 2.13" Mono eInk Display FeatherWing <https://www.adafruit.com/product/4195>`_
 
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.0.9"
+__version__ = "1.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1680.git"
 
 _START_SEQUENCE = (
     b"\x12\x80\x14"  # soft reset and wait 20ms
     b"\x11\x01\x03"  # Ram data entry mode
     b"\x3C\x01\x05"  # border color
     b"\x2c\x01\x36"  # Set vcom voltage
@@ -59,15 +60,17 @@
           Display width
         * *height* (``int``) --
           Display height
         * *rotation* (``int``) --
           Display rotation
     """
 
-    def __init__(self, bus, **kwargs):
+    def __init__(self, bus: displayio.Fourwire, **kwargs) -> None:
+        if "colstart" not in kwargs:
+            kwargs["colstart"] = 1
         stop_sequence = bytearray(_STOP_SEQUENCE)
         try:
             bus.reset()
         except RuntimeError:
             # No reset pin defined, so no deep sleeping
             stop_sequence = b""
 
@@ -91,10 +94,10 @@
             write_color_ram_command=0x26,
             black_bits_inverted=False,
             set_column_window_command=0x44,
             set_row_window_command=0x45,
             set_current_column_command=0x4E,
             set_current_row_command=0x4F,
             refresh_display_command=0x20,
-            colstart=1,
-            always_toggle_chip_select=True,
+            always_toggle_chip_select=False,
+            address_little_endian=True
         )
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1680-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/docs/conf.py` & `adafruit-circuitpython-ssd1680-1.1.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -41,15 +42,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit  CircuitPython SSD1680 Library"
-copyright = "2021 Melissa LeBlanc-Williams"
+creation_year = "2021"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Melissa LeBlanc-Williams"
 author = "Melissa LeBlanc-Williams"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/docs/index.rst` & `adafruit-circuitpython-ssd1680-1.1.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,22 @@
     :maxdepth: 3
 
     api
 
 .. toctree::
     :caption: Tutorials
 
+    Adafruit 2.13" eInk Display Breakouts and FeatherWings <https://learn.adafruit.com/adafruit-2-13-eink-display-breakouts-and-featherwings>
+
 .. toctree::
     :caption: Related Products
 
     Adafruit 2.13" 250x122 Tri-Color eInk / ePaper Display with SRAM - SSD1680 Driver <https://www.adafruit.com/product/4947>
     Adafruit 2.13" HD Tri-Color eInk / ePaper Display FeatherWing <https://www.adafruit.com/product/4814>
+    Adafruit 2.13" Mono eInk Display FeatherWing <https://www.adafruit.com/product/4195>
 
 .. toctree::
     :caption: Other Links
 
     Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_SSD1680/releases/latest>
     Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/examples/display-ruler.bmp` & `adafruit-circuitpython-ssd1680-1.1.0/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/examples/ssd1680_simpletest.py` & `adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_simpletest.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 """Simple test script for 2.13" 250x122 tri-color display.
 Supported products:
   * Adafruit 2.13" Tri-Color eInk Display Breakout
     * https://www.adafruit.com/product/4947
   * Adafruit 2.13" Tri-Color eInk Display FeatherWing
     * https://www.adafruit.com/product/4814
+  * Adafruit 2.13" Mono eInk Display FeatherWing
+    * https://www.adafruit.com/product/4195
+
+
 """
 
 import time
 import board
 import displayio
 import adafruit_ssd1680
 
@@ -26,23 +30,26 @@
 epd_busy = board.D7  # Set to None for FeatherWing
 
 display_bus = displayio.FourWire(
     spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset, baudrate=1000000
 )
 time.sleep(1)
 
+# For issues with display not updating top/bottom rows correctly set colstart to 8
 display = adafruit_ssd1680.SSD1680(
     display_bus,
+    colstart=1,
     width=250,
     height=122,
     busy_pin=epd_busy,
     highlight_color=0xFF0000,
     rotation=270,
 )
 
+
 g = displayio.Group()
 
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
     # CircuitPython 6 & 7 compatible
     t = displayio.TileGrid(
         pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
```

### Comparing `adafruit-circuitpython-ssd1680-1.0.9/pyproject.toml` & `adafruit-circuitpython-ssd1680-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1680"
 description = "CircuitPython `displayio` drivers for SSD1680-based ePaper displays"
-version = "1.0.9"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1680"}
 keywords = [
     "adafruit",
```

