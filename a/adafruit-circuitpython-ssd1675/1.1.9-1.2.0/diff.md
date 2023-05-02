# Comparing `tmp/adafruit-circuitpython-ssd1675-1.1.9.tar.gz` & `tmp/adafruit-circuitpython-ssd1675-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1675-1.1.9.tar", last modified: Fri Feb  4 20:33:37 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1675-1.2.0.tar", last modified: Tue May  2 17:04:38 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1675-1.1.9.tar` & `adafruit-circuitpython-ssd1675-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.268585 adafruit-circuitpython-ssd1675-1.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.264585 adafruit-circuitpython-ssd1675-1.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.264585 adafruit-circuitpython-ssd1675-1.1.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.264585 adafruit-circuitpython-ssd1675-1.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.264585 adafruit-circuitpython-ssd1675-1.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-02-04 20:33:37.268585 adafruit-circuitpython-ssd1675-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.264585 adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-02-04 20:33:37.000000 adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-02-04 20:33:37.000000 adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:33:37.000000 adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:33:37.000000 adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-04 20:33:37.000000 adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/adafruit_ssd1675.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.268585 adafruit-circuitpython-ssd1675-1.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.268585 adafruit-circuitpython-ssd1675-1.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:33:37.268585 adafruit-circuitpython-ssd1675-1.1.9/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)   360122 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/examples/ssd1675_2.13_monochrome.py
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/examples/ssd1675_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:33:37.268585 adafruit-circuitpython-ssd1675-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-02-04 20:33:26.000000 adafruit-circuitpython-ssd1675-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.697537 adafruit-circuitpython-ssd1675-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.689537 adafruit-circuitpython-ssd1675-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.693537 adafruit-circuitpython-ssd1675-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.693537 adafruit-circuitpython-ssd1675-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.693537 adafruit-circuitpython-ssd1675-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-02 17:04:38.697537 adafruit-circuitpython-ssd1675-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.693537 adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-02 17:04:38.000000 adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 17:04:38.000000 adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:04:38.000000 adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 17:04:38.000000 adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 17:04:38.000000 adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-02 17:04:31.000000 adafruit-circuitpython-ssd1675-1.2.0/adafruit_ssd1675.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.693537 adafruit-circuitpython-ssd1675-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.693537 adafruit-circuitpython-ssd1675-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:04:38.697537 adafruit-circuitpython-ssd1675-1.2.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   360122 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-02 17:04:31.000000 adafruit-circuitpython-ssd1675-1.2.0/examples/ssd1675_2.13_monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-02 17:04:31.000000 adafruit-circuitpython-ssd1675-1.2.0/examples/ssd1675_four_corners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 17:04:31.000000 adafruit-circuitpython-ssd1675-1.2.0/examples/ssd1675_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 17:04:31.000000 adafruit-circuitpython-ssd1675-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 17:04:22.000000 adafruit-circuitpython-ssd1675-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:04:38.697537 adafruit-circuitpython-ssd1675-1.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1675-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1675-1.2.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.15.5
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/.pylintrc` & `adafruit-circuitpython-ssd1675-1.2.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
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
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
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
@@ -248,86 +242,58 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
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

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1675-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/LICENSE` & `adafruit-circuitpython-ssd1675-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1675-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1675-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1675-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/PKG-INFO` & `adafruit-circuitpython-ssd1675-1.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,26 @@
-Metadata-Version: 2.1
-Name: adafruit-circuitpython-ssd1675
-Version: 1.1.9
-Summary: CircuitPython `displayio` drivers for SSD1675-based ePaper displays
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
-License: MIT
-Keywords: adafruit blinka circuitpython micropython ssd1675 displayio epd epaper
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1675/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ssd1675/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython `displayio` drivers for SSD1675-based ePaper displays
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -62,16 +47,16 @@
     sudo pip3 install adafruit-circuitpython-ssd1675
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ssd1675
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -120,20 +105,15 @@
     time.sleep(120)
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1675/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
-
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/README.rst` & `adafruit-circuitpython-ssd1675-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,44 @@
+Metadata-Version: 2.1
+Name: adafruit-circuitpython-ssd1675
+Version: 1.2.0
+Summary: CircuitPython `displayio` drivers for SSD1675-based ePaper displays
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
+License: MIT
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1675
+Keywords: adafruit,blinka,circuitpython,micropython,ssd1675,displayio,epd,epaper
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/x-rst
+Provides-Extra: optional
+License-File: LICENSE
+
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1675/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ssd1675/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython `displayio` drivers for SSD1675-based ePaper displays
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -43,16 +65,16 @@
     sudo pip3 install adafruit-circuitpython-ssd1675
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ssd1675
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -101,18 +123,15 @@
     time.sleep(120)
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1675/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1675
-Version: 1.1.9
+Version: 1.2.0
 Summary: CircuitPython `displayio` drivers for SSD1675-based ePaper displays
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython ssd1675 displayio epd epaper
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1675
+Keywords: adafruit,blinka,circuitpython,micropython,ssd1675,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1675/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ssd1675/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython `displayio` drivers for SSD1675-based ePaper displays
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -62,16 +65,16 @@
     sudo pip3 install adafruit-circuitpython-ssd1675
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ssd1675
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -120,20 +123,15 @@
     time.sleep(120)
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1675/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
-
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1675-1.2.0/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_ssd1675.py
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ssd1675.egg-info/PKG-INFO
 adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt
 adafruit_circuitpython_ssd1675.egg-info/dependency_links.txt
 adafruit_circuitpython_ssd1675.egg-info/requires.txt
@@ -30,8 +32,9 @@
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/display-ruler.bmp
 examples/display-ruler.bmp.license
 examples/ssd1675_2.13_monochrome.py
+examples/ssd1675_four_corners.py
 examples/ssd1675_simpletest.py
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/adafruit_ssd1675.py` & `adafruit-circuitpython-ssd1675-1.2.0/adafruit_ssd1675.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware (version 5+) for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1675.git"
 
 _START_SEQUENCE = (
     b"\x12\x80\x02"  # Software reset, 2ms delay
     b"\x74\x01\x54"  # set analog block control
     b"\x7e\x01\x3b"  # set digital block control
     b"\x01\x03\xfa\x01\x00"  # driver output control
@@ -51,15 +51,15 @@
 
 _STOP_SEQUENCE = b"\x10\x01\x01"  # Enter deep sleep
 
 # pylint: disable=too-few-public-methods
 class SSD1675(displayio.EPaperDisplay):
     """SSD1675 driver"""
 
-    def __init__(self, bus, **kwargs):
+    def __init__(self, bus: displayio.FourWire, **kwargs) -> None:
         stop_sequence = _STOP_SEQUENCE
         try:
             bus.reset()
         except RuntimeError:
             stop_sequence = b""
         super().__init__(
             bus,
@@ -71,8 +71,9 @@
             set_column_window_command=0x44,
             set_row_window_command=0x45,
             set_current_column_command=0x4E,
             set_current_row_command=0x4F,
             write_black_ram_command=0x24,
             refresh_display_command=0x20,
             refresh_time=2.2,
+            address_little_endian=True
         )
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1675-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/docs/conf.py` & `adafruit-circuitpython-ssd1675-1.2.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -39,15 +40,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit SSD1675 Library"
-copyright = "2019 Scott Shawcroft"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Scott Shawcroft"
 author = "Scott Shawcroft"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -56,15 +64,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/docs/index.rst` & `adafruit-circuitpython-ssd1675-1.2.0/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     Adafruit 2.13" Monochrome ePaper Display Breakout <https://www.adafruit.com/product/4197>
     Adafruit 2.13" Black and White FeatherWing <https://www.adafruit.com/product/4195>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_SSD1675/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/examples/display-ruler.bmp` & `adafruit-circuitpython-ssd1675-1.2.0/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/examples/ssd1675_2.13_monochrome.py` & `adafruit-circuitpython-ssd1675-1.2.0/examples/ssd1675_2.13_monochrome.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.1.9/examples/ssd1675_simpletest.py` & `adafruit-circuitpython-ssd1675-1.2.0/examples/ssd1675_simpletest.py`

 * *Files identical despite different names*

