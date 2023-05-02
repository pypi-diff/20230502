# Comparing `tmp/xcpcio_board_spider-0.0.5.tar.gz` & `tmp/xcpcio_board_spider-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcpcio_board_spider-0.0.5.tar", max compression
+gzip compressed data, was "xcpcio_board_spider-0.0.7.tar", max compression
```

## Comparing `xcpcio_board_spider-0.0.5.tar` & `xcpcio_board_spider-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/LICENSE
--rw-r--r--   0        0        0      538 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/README.md
--rw-r--r--   0        0        0      977 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/__init__.py
--rw-r--r--   0        0        0     2160 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/config.py
--rw-r--r--   0        0        0      303 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/constants.py
--rw-r--r--   0        0        0      377 2023-04-30 15:29:30.966794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/logger.py
--rw-r--r--   0        0        0     1074 2023-04-30 15:29:30.970794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/logo.py
--rw-r--r--   0        0        0     2885 2023-04-30 15:29:30.970794 xcpcio_board_spider-0.0.5/xcpcio_board_spider/utils.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-02 16:10:27.416997 xcpcio_board_spider-0.0.7/LICENSE
+-rw-r--r--   0        0        0      538 2023-05-02 16:10:27.416997 xcpcio_board_spider-0.0.7/README.md
+-rw-r--r--   0        0        0     1004 2023-05-02 16:10:27.420997 xcpcio_board_spider-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/logger.py
+-rw-r--r--   0        0        0     1074 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/logo.py
+-rw-r--r--   0        0        0     1863 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/domjudge/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-02 16:10:27.464997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/domjudge/v2/__init__.py
+-rw-r--r--   0        0        0     5319 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/spider/domjudge/v2/domjudge.py
+-rw-r--r--   0        0        0      113 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/__init__.py
+-rw-r--r--   0        0        0      303 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/constants.py
+-rw-r--r--   0        0        0     2492 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/contest.py
+-rw-r--r--   0        0        0     1041 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/submission.py
+-rw-r--r--   0        0        0     1585 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/team.py
+-rw-r--r--   0        0        0      262 2023-05-02 16:10:27.468997 xcpcio_board_spider-0.0.7/xcpcio_board_spider/type/type.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.7/PKG-INFO
```

### Comparing `xcpcio_board_spider-0.0.5/LICENSE` & `xcpcio_board_spider-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.5/README.md` & `xcpcio_board_spider-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.5/pyproject.toml` & `xcpcio_board_spider-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcpcio-board-spider"
-version = "0.0.5"
+version = "0.0.7"
 description = "XCPCIO Board Spider"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -28,11 +28,12 @@
 xlrd = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 flake8 = "^6.0.0"
 pyright = "^1.1.305"
 autopep8 = "^2.0.2"
+pytest-snapshot = "^0.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xcpcio_board_spider-0.0.5/xcpcio_board_spider/logo.py` & `xcpcio_board_spider-0.0.7/xcpcio_board_spider/core/logo.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.5/PKG-INFO` & `xcpcio_board_spider-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcpcio-board-spider
-Version: 0.0.5
+Version: 0.0.7
 Summary: XCPCIO Board Spider
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

