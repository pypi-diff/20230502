# Comparing `tmp/spatial_spec-0.1.0.tar.gz` & `tmp/spatial_spec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_spec-0.1.0.tar", max compression
+gzip compressed data, was "spatial_spec-0.1.1.tar", max compression
```

## Comparing `spatial_spec-0.1.0.tar` & `spatial_spec-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-04-27 08:46:19.173349 spatial_spec-0.1.0/LICENSE
--rw-r--r--   0        0        0      556 2023-05-02 17:46:12.275168 spatial_spec-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1035 2023-05-02 06:32:07.522473 spatial_spec-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 08:46:19.354929 spatial_spec-0.1.0/spatial_spec/__init__.py
--rw-r--r--   0        0        0    14014 2023-05-02 17:46:18.384931 spatial_spec-0.1.0/spatial_spec/automaton_planning.py
--rw-r--r--   0        0        0    26002 2023-04-27 13:01:43.283965 spatial_spec-0.1.0/spatial_spec/geometry.py
--rw-r--r--   0        0        0    26712 2023-05-02 17:46:19.981084 spatial_spec-0.1.0/spatial_spec/logic.py
--rw-r--r--   0        0        0     3572 2023-05-02 17:46:23.030954 spatial_spec-0.1.0/spatial_spec/ltlf2dfa_nx.py
--rw-r--r--   0        0        0     2078 2023-04-27 08:46:19.355929 spatial_spec-0.1.0/spatial_spec/spatial.lark
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 spatial_spec-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-27 08:46:19.173349 spatial_spec-0.1.1/LICENSE
+-rw-r--r--   0        0        0      556 2023-05-02 17:53:31.360808 spatial_spec-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1047 2023-05-02 17:53:22.085210 spatial_spec-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 08:46:19.354929 spatial_spec-0.1.1/spatial_spec/__init__.py
+-rw-r--r--   0        0        0    14014 2023-05-02 17:46:18.384931 spatial_spec-0.1.1/spatial_spec/automaton_planning.py
+-rw-r--r--   0        0        0    26002 2023-04-27 13:01:43.283965 spatial_spec-0.1.1/spatial_spec/geometry.py
+-rw-r--r--   0        0        0    26712 2023-05-02 17:46:19.981084 spatial_spec-0.1.1/spatial_spec/logic.py
+-rw-r--r--   0        0        0     3572 2023-05-02 17:46:23.030954 spatial_spec-0.1.1/spatial_spec/ltlf2dfa_nx.py
+-rw-r--r--   0        0        0     2078 2023-04-27 08:46:19.355929 spatial_spec-0.1.1/spatial_spec/spatial.lark
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 spatial_spec-0.1.1/PKG-INFO
```

### Comparing `spatial_spec-0.1.0/LICENSE` & `spatial_spec-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_spec-0.1.0/pyproject.toml` & `spatial_spec-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spatial_spec"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Georg Schuppe <georg.schuppe@gmail.com>", "Christian Pek <pek2@kth.se>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `spatial_spec-0.1.0/README.md` & `spatial_spec-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-# SpaTiaL - Library Code
+# SpaTiaL Specifications
 
-This is the source code for the library itself.
-
-## Installation from Source Code
+SpaTiaL is a framework to specify spatial and temporal relations between objects.
 
 We use [MONA](http://www.brics.dk/mona/) to convert LTLf formulae to DFA. If you want to use the automaton-based planning, install it first.
 Check the website for installation instructions or try to install with apt. **We are using `ltlf2dfa` to call MONA in python.
 That library currently does not work with Windows.**
 ```shell
 sudo apt install mona
 ```
 
+## Installation from Source
+
+`spatial-spec` is distributed on PyPI, but you can also install from source.
+
 1. Clone the repository and navigate into it:
     ```
     $ git clone https://github.com/KTH-RPL-Planiacs/SpaTiaL.git
     cd SpaTiaL
     cd spatial-lib
     ```
 2. This project uses [poetry](https://python-poetry.org/) to handle dependencies. Please make sure you have poetry installed and run:
     ```
     poetry install
     ```
 3. Try running the unit tests to see if everything works:
     ```
     poetry run python -m unittest discover
     ```
-
-## Repository Structure
-
-- [spatial](./spatial): source code
-- [tests](./tests): unittests
```

### Comparing `spatial_spec-0.1.0/spatial_spec/automaton_planning.py` & `spatial_spec-0.1.1/spatial_spec/automaton_planning.py`

 * *Files identical despite different names*

### Comparing `spatial_spec-0.1.0/spatial_spec/geometry.py` & `spatial_spec-0.1.1/spatial_spec/geometry.py`

 * *Files identical despite different names*

### Comparing `spatial_spec-0.1.0/spatial_spec/logic.py` & `spatial_spec-0.1.1/spatial_spec/logic.py`

 * *Files identical despite different names*

### Comparing `spatial_spec-0.1.0/spatial_spec/ltlf2dfa_nx.py` & `spatial_spec-0.1.1/spatial_spec/ltlf2dfa_nx.py`

 * *Files identical despite different names*

### Comparing `spatial_spec-0.1.0/spatial_spec/spatial.lark` & `spatial_spec-0.1.1/spatial_spec/spatial.lark`

 * *Files identical despite different names*

### Comparing `spatial_spec-0.1.0/PKG-INFO` & `spatial_spec-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatial-spec
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: LICENSE
 Author: Georg Schuppe
 Author-email: georg.schuppe@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -16,27 +16,29 @@
 Requires-Dist: ltlf2dfa (>=1.0.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
-# SpaTiaL - Library Code
+# SpaTiaL Specifications
 
-This is the source code for the library itself.
-
-## Installation from Source Code
+SpaTiaL is a framework to specify spatial and temporal relations between objects.
 
 We use [MONA](http://www.brics.dk/mona/) to convert LTLf formulae to DFA. If you want to use the automaton-based planning, install it first.
 Check the website for installation instructions or try to install with apt. **We are using `ltlf2dfa` to call MONA in python.
 That library currently does not work with Windows.**
 ```shell
 sudo apt install mona
 ```
 
+## Installation from Source
+
+`spatial-spec` is distributed on PyPI, but you can also install from source.
+
 1. Clone the repository and navigate into it:
     ```
     $ git clone https://github.com/KTH-RPL-Planiacs/SpaTiaL.git
     cd SpaTiaL
     cd spatial-lib
     ```
 2. This project uses [poetry](https://python-poetry.org/) to handle dependencies. Please make sure you have poetry installed and run:
@@ -44,12 +46,7 @@
     poetry install
     ```
 3. Try running the unit tests to see if everything works:
     ```
     poetry run python -m unittest discover
     ```
 
-## Repository Structure
-
-- [spatial](./spatial): source code
-- [tests](./tests): unittests
-
```

