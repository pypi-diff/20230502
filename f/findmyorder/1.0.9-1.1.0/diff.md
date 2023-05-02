# Comparing `tmp/findmyorder-1.0.9.tar.gz` & `tmp/findmyorder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.0.9.tar", max compression
+gzip compressed data, was "findmyorder-1.1.0.tar", max compression
```

## Comparing `findmyorder-1.0.9.tar` & `findmyorder-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-27 08:02:56.393167 findmyorder-1.0.9/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-27 08:02:56.393167 findmyorder-1.0.9/README.md
--rw-r--r--   0        0        0      106 2023-04-27 08:02:57.129178 findmyorder-1.0.9/findmyorder/__init__.py
--rw-r--r--   0        0        0      723 2023-04-27 08:02:56.393167 findmyorder-1.0.9/findmyorder/config.py
--rw-r--r--   0        0        0      120 2023-04-27 08:02:56.393167 findmyorder-1.0.9/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3322 2023-04-27 08:02:56.393167 findmyorder-1.0.9/findmyorder/main.py
--rw-r--r--   0        0        0     1213 2023-04-27 08:02:57.125178 findmyorder-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 findmyorder-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-02 06:09:52.837325 findmyorder-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1925 2023-05-02 06:09:52.837325 findmyorder-1.1.0/README.md
+-rw-r--r--   0        0        0      113 2023-05-02 06:09:53.569324 findmyorder-1.1.0/findmyorder/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-02 06:09:52.837325 findmyorder-1.1.0/findmyorder/config.py
+-rw-r--r--   0        0        0      312 2023-05-02 06:09:52.837325 findmyorder-1.1.0/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3818 2023-05-02 06:09:52.837325 findmyorder-1.1.0/findmyorder/main.py
+-rw-r--r--   0        0        0     1223 2023-05-02 06:09:53.569324 findmyorder-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 findmyorder-1.1.0/PKG-INFO
```

### Comparing `findmyorder-1.0.9/LICENSE` & `findmyorder-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.0.9/pyproject.toml` & `findmyorder-1.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.0.9"
+version = "1.1.0"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-asyncio = ">=3.4.3"
 dynaconf = ">=3.1.12"
 pyparsing = ">=3.0.9"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
+pytest = "*"
+pytest-cov = "*"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 python_classes = [
   "Test*",
   "*Test"
 ]
```

### Comparing `findmyorder-1.0.9/PKG-INFO` & `findmyorder-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.0.9
+Version: 1.1.0
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: dynaconf (>=3.1.12)
 Requires-Dist: pyparsing (>=3.0.9)
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
-# Find my order. 
+# Find my order
 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and parse order for trade execution. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder) [![🐍Build](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8Dbuild.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8Dbuild.yml) | Find order <br> Parse order |
+|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![🐍Build](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8DBuild.yml/badge.svg?branch=main)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8DBuild.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 
 
 Key features:
 
-- tbd
+- Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
+- Parse and return a structured order with action and instrument as mandatory
+- Settings for custom option
 
 
 
 
 # Install
 `pip install findmyorder`
 
 # How to use it
 ```
-
+fmo = FindMyOrder()
+msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
+order = await fmo.get_order(msg_order)
+  
 ```
 ## Example
 [example](https://github.com/mraniki/findmyorder/blob/main/examples/example.py)
 
 ## Real use case
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
```

