# Comparing `tmp/sortedness-0.220803.1.tar.gz` & `tmp/sortedness-0.230501.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortedness-0.220803.1.tar", max compression
+gzip compressed data, was "sortedness-0.230501.6.tar", max compression
```

## Comparing `sortedness-0.220803.1.tar` & `sortedness-0.230501.6.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.220803.1/LICENSE
--rw-r--r--   0        0        0      816 2022-08-03 19:35:49.048206 sortedness-0.220803.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-23 23:33:48.000000 sortedness-0.220803.1/src/sortedness/__init__.py
--rw-r--r--   0        0        0     1301 2022-08-03 18:27:50.511755 sortedness-0.220803.1/src/sortedness/config.py
--rw-r--r--   0        0        0        0 2022-07-23 18:58:03.000000 sortedness-0.220803.1/src/sortedness/evaluation/__init__.py
--rw-r--r--   0        0        0     2153 2022-08-03 19:26:11.421193 sortedness-0.220803.1/src/sortedness/evaluation/plot.py
--rw-r--r--   0        0        0    10607 2022-07-26 02:25:33.000000 sortedness-0.220803.1/src/sortedness/global.py
--rw-r--r--   0        0        0     3645 2022-07-26 02:25:33.000000 sortedness-0.220803.1/src/sortedness/kruskal.py
--rw-r--r--   0        0        0    36444 2022-08-03 19:35:42.988132 sortedness-0.220803.1/src/sortedness/local.py
--rw-r--r--   0        0        0     7950 2022-07-26 02:25:33.000000 sortedness-0.220803.1/src/sortedness/rank.py
--rw-r--r--   0        0        0     4707 2022-08-03 19:35:35.816045 sortedness-0.220803.1/src/sortedness/trustworthiness.py
--rw-r--r--   0        0        0      851 2022-08-03 19:36:02.706881 sortedness-0.220803.1/setup.py
--rw-r--r--   0        0        0      476 2022-08-03 19:36:02.707060 sortedness-0.220803.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.230501.6/LICENSE
+-rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-0.230501.6/build.py
+-rw-r--r--   0        0        0     1107 2023-05-02 00:40:43.859932 sortedness-0.230501.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-03 19:59:46.000000 sortedness-0.230501.6/src/sortedness/__init__.py
+-rw-r--r--   0        0        0     1281 2023-05-01 23:25:35.123741 sortedness-0.230501.6/src/sortedness/config.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-0.230501.6/src/sortedness/evaluation/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-01 21:01:18.170347 sortedness-0.230501.6/src/sortedness/evaluation/plot.py
+-rw-r--r--   0        0        0     5145 2023-05-01 21:07:34.442703 sortedness-0.230501.6/src/sortedness/global.py
+-rw-r--r--   0        0        0    22749 2023-05-01 23:40:16.090062 sortedness-0.230501.6/src/sortedness/local.py
+-rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-0.230501.6/src/sortedness/matrices.py
+-rw-r--r--   0        0        0     2962 2023-05-01 23:15:42.252581 sortedness-0.230501.6/src/sortedness/parallel.py
+-rw-r--r--   0        0        0     7950 2022-08-03 19:59:46.000000 sortedness-0.230501.6/src/sortedness/rank.py
+-rw-r--r--   0        0        0     4707 2022-08-03 19:59:46.000000 sortedness-0.230501.6/src/sortedness/trustworthiness.py
+-rw-r--r--   0        0        0     3511 2023-05-01 23:16:29.848511 sortedness-0.230501.6/src/sortedness/wtau/__init__.py
+-rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-0.230501.6/src/sortedness/wtau/wtau.pyx
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 sortedness-0.230501.6/setup.py
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 sortedness-0.230501.6/PKG-INFO
```

### Comparing `sortedness-0.220803.1/LICENSE` & `sortedness-0.230501.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sortedness-0.220803.1/pyproject.toml` & `sortedness-0.230501.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 [tool.poetry]
 name = "sortedness"
-version = "0.220803.1"
+version = "0.230501.6"
 description = "Measures of projection quality"
-authors = ["davips <dpsabc@gmail.com>"]
+authors = ["davips <dpsabc@gmail.com>", "tacito <tacito.neves@gmail.com>"]
 license = "GPLv3"
+build = "build.py"  # For Cython. apt-get package needed: python3-numpy
 
 [tool.poetry.dependencies]
 python = "^3.10,<4.0"
-scipy = {version = "^1.8.1", python = ">=3.8,<3.11"}
-lange = "^0.220727.5"
+scipy = {version = "^1.10.1", python = ">=3.8,<3.11"}
+lange = "^1.230203.1"
+pathos = "^0.3.0"
+shelchemy = "^0.220906.5"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-black = "^22.6.0"
+#[tool.poetry.dev-dependencies]
+#ipython = "^8.13.1"
+#openml = "^0.13.1"
+#pandas = "^2.0.1"
+#hoshmap = "^0.220808.0"
+#dash = "^2.9.3"
+##ranky = "^0.3.3"
+#sympy = "^1.10.1"
+#matplotlib = "^3.7.1"
+#PyQt5 = "^5.15.7"
+#PyMySQL = "^1.0.2"
+#lz4 = "^4.0.2"
+#cryptography = "^40.0.2"
+
+[tool.poetry.group.dev.dependencies]
+setuptools = "^67.7.2"
+Cython = "^0.29.27"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+black = "^23.3.0"
 pdoc3 = "^0.10.0"
-autoreadme = "^0.2102.20"
-ipython = "^8.4.0"
-scikit-learn = "^1.1.1"
-openml = "^0.12.2"
-pandas = "^1.4.3"
-hoshmap = "^0.220727.3"
-dash = "^2.6.0"
-ranky = "^0.2.9"
-sympy = "^1.10.1"
-matplotlib = "^3.5.2"
-PyQt5 = "^5.15.7"
-shelchemy = "^0.220726.8"
-PyMySQL = "^1.0.2"
-lazydf = "^0.220725.4"
-lz4 = "^4.0.2"
-cryptography = "^37.0.4"
+autoreadme = "^0.2302.3"
+scikit-learn = "^1.2.2"
+numpy = "^1.24.3"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0", "Cython>=0.29.27", "setuptools>=60.8.1", "numpy>=1.23.3", "scipy>=1.10.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sortedness-0.220803.1/src/sortedness/config.py` & `sortedness-0.230501.6/src/sortedness/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,12 @@
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 from configparser import ConfigParser
-from pathlib import Path
-
 
 config = ConfigParser()
-config.read(f"{Path.home()}/.sortedness-cache.config")
-local_cache_uri = config.get("storages", "local")
-remote_cache_uri = config.get("storages", "remote")
+# config.read(f"{Path.home()}/.sortedness-cache.config")
+# local_cache_uri = config.get("storages", "local")
+# remote_cache_uri = config.get("storages", "remote")
```

### Comparing `sortedness-0.220803.1/src/sortedness/evaluation/plot.py` & `sortedness-0.230501.6/src/sortedness/evaluation/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-#  Copyright (c) 2022. Davi Pereira dos Santos
-#  This file is part of the sortedness project.
-#  Please respect the license - more about this in the section (*) below.
-#
-#  sortedness is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  sortedness is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with sortedness.  If not, see <http://www.gnu.org/licenses/>.
-#
-#  (*) Removing authorship by any means, e.g. by distribution of derived
-#  works or verbatim, obfuscated, compiled or rewritten versions of any
-#  part of this work is illegal and it is unethical regarding the effort and
-#  time spent here.
-#
-
-from dataclasses import dataclass
-
-from hoshmap import idict
-
-colors = ["blue", "green", "red", "gray", "yellow", "black", "pink"]
-
-
-@dataclass
-class Plot:
-    d: idict
-    projection: str
-    xlabel: str
-    ylabel: str
-    legend: bool
-    plt: callable
-    fontsize: int = 18
-    marksize: int = 2
-
-    def __post_init__(self):
-        self.fig = self.plt.figure()
-        self.plt.title(f"{self.projection}", fontsize=self.fontsize)
-        self.ax = self.fig.gca()
-        # ax.set_yscale('log')
-
-    def __lshift__(self, other):
-        slabel, color = other
-        self.ax.scatter(self.d[self.xlabel], self.d[slabel], s=self.marksize, c=color, label=slabel)
-
-    def finish(self):
-        if self.legend:
-            self.ax.legend(fontsize=self.fontsize)
-        self.plt.xlabel(self.xlabel, fontsize=self.fontsize)
-        self.plt.ylabel(self.ylabel, fontsize=self.fontsize)
-        self.plt.tight_layout()
-        figManager = self.plt.get_current_fig_manager()
-        figManager.window.showMaximized()
-        figManager.window.setWindowTitle(f"{self.projection}     {self.xlabel}")
+# #  Copyright (c) 2022. Davi Pereira dos Santos
+# #  This file is part of the sortedness project.
+# #  Please respect the license - more about this in the section (*) below.
+# #
+# #  sortedness is free software: you can redistribute it and/or modify
+# #  it under the terms of the GNU General Public License as published by
+# #  the Free Software Foundation, either version 3 of the License, or
+# #  (at your option) any later version.
+# #
+# #  sortedness is distributed in the hope that it will be useful,
+# #  but WITHOUT ANY WARRANTY; without even the implied warranty of
+# #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# #  GNU General Public License for more details.
+# #
+# #  You should have received a copy of the GNU General Public License
+# #  along with sortedness.  If not, see <http://www.gnu.org/licenses/>.
+# #
+# #  (*) Removing authorship by any means, e.g. by distribution of derived
+# #  works or verbatim, obfuscated, compiled or rewritten versions of any
+# #  part of this work is illegal and it is unethical regarding the effort and
+# #  time spent here.
+# #
+#
+# from dataclasses import dataclass
+#
+#
+# colors = ["blue", "green", "red", "gray", "yellow", "black", "pink"]
+#
+#
+# @dataclass
+# class Plot:
+#     d: object
+#     projection: str
+#     xlabel: str
+#     ylabel: str
+#     legend: bool
+#     plt: callable
+#     fontsize: int = 18
+#     marksize: int = 2
+#
+#     def __post_init__(self):
+#         self.fig = self.plt.figure()
+#         self.plt.title(f"{self.projection}", fontsize=self.fontsize)
+#         self.ax = self.fig.gca()
+#         # ax.set_yscale('log')
+#
+#     def __lshift__(self, other):
+#         slabel, color = other
+#         self.ax.scatter(self.d[self.xlabel], self.d[slabel], s=self.marksize, c=color, label=slabel)
+#
+#     def finish(self):
+#         if self.legend:
+#             self.ax.legend(fontsize=self.fontsize)
+#         self.plt.xlabel(self.xlabel, fontsize=self.fontsize)
+#         self.plt.ylabel(self.ylabel, fontsize=self.fontsize)
+#         self.plt.tight_layout()
+#         figManager = self.plt.get_current_fig_manager()
+#         figManager.window.showMaximized()
+#         figManager.window.setWindowTitle(f"{self.projection}     {self.xlabel}")
```

### Comparing `sortedness-0.220803.1/src/sortedness/rank.py` & `sortedness-0.230501.6/src/sortedness/rank.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.220803.1/src/sortedness/trustworthiness.py` & `sortedness-0.230501.6/src/sortedness/trustworthiness.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.220803.1/setup.py` & `sortedness-0.230501.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['sortedness', 'sortedness.evaluation']
+['sortedness', 'sortedness.evaluation', 'sortedness.wtau']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['lange>=0.220727.5,<0.220728.0']
+['lange>=1.230203.1,<2.0.0',
+ 'pathos>=0.3.0,<0.4.0',
+ 'shelchemy>=0.220906.5,<0.220907.0']
 
 extras_require = \
-{':python_version >= "3.8" and python_version < "3.11"': ['scipy>=1.8.1,<2.0.0']}
+{':python_version >= "3.8" and python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'sortedness',
-    'version': '0.220803.1',
+    'version': '0.230501.6',
     'description': 'Measures of projection quality',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
-
+from build import *
+build(setup_kwargs)
 
 setup(**setup_kwargs)
```

