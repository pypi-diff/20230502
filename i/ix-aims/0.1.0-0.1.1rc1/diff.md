# Comparing `tmp/ix_aims-0.1.0.tar.gz` & `tmp/ix_aims-0.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ix_aims-0.1.0.tar", max compression
+gzip compressed data, was "ix_aims-0.1.1rc1.tar", max compression
```

## Comparing `ix_aims-0.1.0.tar` & `ix_aims-0.1.1rc1.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.0/ix_aims/__init__.py
--rw-r--r--   0        0        0      123 2023-05-02 21:37:07.078194 ix_aims-0.1.0/ix_aims/cli.py
--rw-r--r--   0        0        0     3677 2023-05-02 21:39:12.578545 ix_aims-0.1.0/ix_aims/lib.py
--rw-r--r--   0        0        0      627 2023-05-02 21:36:45.294132 ix_aims-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 ix_aims-0.1.0/setup.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 ix_aims-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.1rc1/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.1rc1/ix_aims/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-02 21:37:07.078194 ix_aims-0.1.1rc1/ix_aims/cli.py
+-rw-r--r--   0        0        0     2134 2023-05-02 21:20:56.338365 ix_aims-0.1.1rc1/ix_aims/imgs/icon.png
+-rw-r--r--   0        0        0     1996 2023-05-02 21:20:56.338365 ix_aims-0.1.1rc1/ix_aims/imgs/noBtn.png
+-rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/plusTab.png
+-rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/processesBtn.png
+-rw-r--r--   0        0        0     1207 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/selectDirsBtn.png
+-rw-r--r--   0        0        0     1064 2023-05-02 21:20:56.338365 ix_aims-0.1.1rc1/ix_aims/imgs/winIcon.png
+-rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/yesBtn.png
+-rw-r--r--   0        0        0     3683 2023-05-02 21:52:32.596646 ix_aims-0.1.1rc1/ix_aims/lib.py
+-rw-r--r--   0        0        0      630 2023-05-02 21:52:27.800650 ix_aims-0.1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc1/setup.py
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc1/PKG-INFO
```

### Comparing `ix_aims-0.1.0/ix_aims/lib.py` & `ix_aims-0.1.1rc1/ix_aims/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Literal
 
 import arrow
 import pyautogui as g
 from hakai_api import Client
 
 g.PAUSE = 0.05
-IMG_DIR = "./imgs"
+IMG_DIR = "ix_aims/imgs"
 
 
 def move(img):
     if loc := g.locateOnScreen(img, grayscale=True, confidence=.95):
         g.moveTo(*g.center(loc))
```

### Comparing `ix_aims-0.1.0/pyproject.toml` & `ix_aims-0.1.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ix-aims"
-version = "0.1.0"
+version = "0.1.1rc1"
 description = "iX Capture automation with AIMS data"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ix_aims"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ix_aims-0.1.0/setup.py` & `ix_aims-0.1.1rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['ix_aims']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'ix_aims': ['imgs/*']}
 
 install_requires = \
 ['PyAutoGUI>=0.9.53,<0.10.0',
  'arrow>=1.2.3,<2.0.0',
  'hakai-api>=1.3.0,<2.0.0',
  'opencv-python>=4.7.0.72,<5.0.0.0',
  'pillow>=9.5.0,<10.0.0',
@@ -17,15 +17,15 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['autoix = ix_aims.cli:main']}
 
 setup_kwargs = {
     'name': 'ix-aims',
-    'version': '0.1.0',
+    'version': '0.1.1rc1',
     'description': 'iX Capture automation with AIMS data',
     'long_description': '# auto-ix-capture\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ix_aims-0.1.0/PKG-INFO` & `ix_aims-0.1.1rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ix-aims
-Version: 0.1.0
+Version: 0.1.1rc1
 Summary: iX Capture automation with AIMS data
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

