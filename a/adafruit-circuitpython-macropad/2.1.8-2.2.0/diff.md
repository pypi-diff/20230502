# Comparing `tmp/adafruit-circuitpython-macropad-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-macropad-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-macropad-2.1.8.tar", last modified: Thu Sep 15 18:20:17 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-macropad-2.2.0.tar", last modified: Mon May  1 22:24:10 2023, max compression
```

## Comparing `adafruit-circuitpython-macropad-2.1.8.tar` & `adafruit-circuitpython-macropad-2.2.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.484221 adafruit-circuitpython-macropad-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.472220 adafruit-circuitpython-macropad-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.476220 adafruit-circuitpython-macropad-2.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.476220 adafruit-circuitpython-macropad-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.476220 adafruit-circuitpython-macropad-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18375 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4818 2022-09-15 18:20:17.484221 adafruit-circuitpython-macropad-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.476220 adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4818 2022-09-15 18:20:17.000000 adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-09-15 18:20:17.000000 adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 18:20:17.000000 adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-15 18:20:17.000000 adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-15 18:20:17.000000 adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    37304 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/adafruit_macropad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.480220 adafruit-circuitpython-macropad-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.480220 adafruit-circuitpython-macropad-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6168 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.480220 adafruit-circuitpython-macropad-2.1.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.480220 adafruit-circuitpython-macropad-2.1.8/examples/macropad_display_image/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_display_image/blinka.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_display_image/blinka.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_display_image/macropad_display_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_grid_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_keyboard_layout.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1713 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_keyboard_mouse.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_led_animation_example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:20:17.480220 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/
--rw-r--r--   0 runner    (1001) docker     (121)    13920 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/beats.mp3
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/beats.mp3.license
--rw-r--r--   0 runner    (1001) docker     (121)    24648 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/happy.mp3
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/happy.mp3.license
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/macropad_mp3.py
--rw-r--r--   0 runner    (1001) docker     (121)    12696 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/slow.mp3
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/slow.mp3.license
--rw-r--r--   0 runner    (1001) docker     (121)    35609 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/upbeats.mp3
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/upbeats.mp3.license
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_rainbow_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_rotation.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_simpletest_display.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_tone_keypad.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3535 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/examples/macropad_tone_keypad_extended.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-09-15 18:20:08.000000 adafruit-circuitpython-macropad-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-09-15 18:19:59.000000 adafruit-circuitpython-macropad-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 18:20:17.484221 adafruit-circuitpython-macropad-2.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.916957 adafruit-circuitpython-macropad-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.920958 adafruit-circuitpython-macropad-2.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.920958 adafruit-circuitpython-macropad-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.920958 adafruit-circuitpython-macropad-2.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.924958 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38207 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_macropad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.924958 adafruit-circuitpython-macropad-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.924958 adafruit-circuitpython-macropad-2.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/blinka.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/blinka.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/macropad_display_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_grid_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_layout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_led_animation_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/beats.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/beats.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/happy.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/happy.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/macropad_mp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/slow.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/slow.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/upbeats.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/upbeats.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_rainbow_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-macropad-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-macropad-2.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/.gitignore` & `adafruit-circuitpython-macropad-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-macropad-2.2.0/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-macropad-2.1.8/.pylintrc` & `adafruit-circuitpython-macropad-2.2.0/.pylintrc`

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

### Comparing `adafruit-circuitpython-macropad-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-macropad-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/LICENSE` & `adafruit-circuitpython-macropad-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-macropad-2.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-macropad-2.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/PKG-INFO` & `adafruit-circuitpython-macropad-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-macropad
-Version: 2.1.8
+Version: 2.2.0
 Summary: A helper library for the Adafruit MacroPad RP2040
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MacroPad
 Keywords: adafruit,macropad,rp2040,mechanical,keyboard,breakout,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-macropad-2.1.8/README.rst` & `adafruit-circuitpython-macropad-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/PKG-INFO` & `adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-macropad
-Version: 2.1.8
+Version: 2.2.0
 Summary: A helper library for the Adafruit MacroPad RP2040
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MacroPad
 Keywords: adafruit,macropad,rp2040,mechanical,keyboard,breakout,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-macropad-2.1.8/adafruit_circuitpython_macropad.egg-info/SOURCES.txt` & `adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_macropad.py
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
 LICENSES/CC-BY-SA-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_macropad.egg-info/PKG-INFO
 adafruit_circuitpython_macropad.egg-info/SOURCES.txt
 adafruit_circuitpython_macropad.egg-info/dependency_links.txt
```

### Comparing `adafruit-circuitpython-macropad-2.1.8/adafruit_macropad.py` & `adafruit-circuitpython-macropad-2.2.0/adafruit_macropad.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     from typing import Tuple, Optional, Union, Iterator
     from neopixel import NeoPixel
     from keypad import Keys
     import adafruit_hid  # pylint:disable=ungrouped-imports
 except ImportError:
     pass
 
-__version__ = "2.1.8"
+__version__ = "2.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MacroPad.git"
 
 ROTATED_KEYMAP_0 = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11)
 ROTATED_KEYMAP_90 = (2, 5, 8, 11, 1, 4, 7, 10, 0, 3, 6, 9)
 ROTATED_KEYMAP_180 = (11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0)
 ROTATED_KEYMAP_270 = (9, 6, 3, 0, 10, 7, 4, 1, 11, 8, 5, 2)
 
@@ -239,15 +239,14 @@
         self,
         rotation: int = 0,
         midi_in_channel: int = 1,
         midi_out_channel: int = 1,
         layout_class: type[KeyboardLayoutBase] = KeyboardLayoutUS,
         keycode_class: type[Keycode] = Keycode,
     ):
-
         if rotation not in (0, 90, 180, 270):
             raise ValueError("Only 90 degree rotations are supported.")
 
         # Define LEDs:
         self._pixels = neopixel.NeoPixel(board.NEOPIXEL, 12)
         self._led = digitalio.DigitalInOut(board.LED)
         self._led.switch_to_output()
@@ -287,14 +286,15 @@
         self._encoder_switch.switch_to_input(pull=digitalio.Pull.UP)
         self._debounced_switch = Debouncer(self._encoder_switch)
 
         # Define display:
         if not isinstance(board.DISPLAY, type(None)):
             self.display = board.DISPLAY
             self.display.rotation = rotation
+        self._display_sleep = False
 
         # Define audio:
         self._speaker_enable = digitalio.DigitalInOut(board.SPEAKER_ENABLE)
         self._speaker_enable.switch_to_output(value=False)
         self._sample = None
         self._sine_wave = None
         self._sine_wave_sample = None
@@ -321,14 +321,38 @@
                 out_channel=midi_out_channel - 1,
             )
         except IndexError:
             # No MIDI ports available.
             self._midi = None
 
     @property
+    def display_sleep(self) -> bool:
+        """The power saver mode of the display. Set it to put the display to
+        sleep or wake it up again.
+
+        If the display is put to sleep, it stops the OLED drive and greatly
+        reduces its power usage. The display mode and current content of the
+        display are still kept in the memory of the displays microprocessor and
+        can be updated nevertheless.
+        """
+        return self._display_sleep
+
+    @display_sleep.setter
+    def display_sleep(self, sleep: bool) -> None:
+        if self._display_sleep == sleep:
+            return
+        # See https://cdn-shop.adafruit.com/product-files/5228/5223-ds.pdf#page=13
+        if sleep:
+            command = 0xAE
+        else:
+            command = 0xAF
+        self.display.bus.send(command, b"")
+        self._display_sleep = sleep
+
+    @property
     def pixels(self) -> Optional[_PixelMapLite]:
         """Sequence-like object representing the twelve NeoPixel LEDs in a 3 x 4 grid on the
         MacroPad. Each pixel is at a certain index in the sequence, numbered 0-11. Colors can be an
         RGB tuple like (255, 0, 0) where (R, G, B), or an RGB hex value like 0xFF0000 for red where
         each two digits are a color (0xRRGGBB). Set the global brightness using any number from 0
         to 1 to represent a percentage, i.e. 0.3 sets global brightness to 30%. Brightness defaults
         to 1.
```

### Comparing `adafruit-circuitpython-macropad-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-macropad-2.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/docs/conf.py` & `adafruit-circuitpython-macropad-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/docs/index.rst` & `adafruit-circuitpython-macropad-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_display_image/blinka.bmp` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/blinka.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_grid_layout.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_grid_layout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_keyboard_layout.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_layout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_keyboard_mouse.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_mouse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/beats.mp3` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/beats.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/happy.mp3` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/happy.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/macropad_mp3.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/macropad_mp3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/slow.mp3` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/slow.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_mp3/upbeats.mp3` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/upbeats.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_rainbow_keys.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_rainbow_keys.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_rotation.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_rotation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_simpletest.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_simpletest_display.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest_display.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_tone_keypad.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/examples/macropad_tone_keypad_extended.py` & `adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad_extended.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.1.8/pyproject.toml` & `adafruit-circuitpython-macropad-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-macropad"
 description = "A helper library for the Adafruit MacroPad RP2040"
-version = "2.1.8"
+version = "2.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MacroPad"}
 keywords = [
     "adafruit",
```

