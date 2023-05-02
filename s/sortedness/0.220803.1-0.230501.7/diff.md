# Comparing `tmp/sortedness-0.220803.1.tar.gz` & `tmp/sortedness-0.230501.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortedness-0.220803.1.tar", max compression
+gzip compressed data, was "sortedness-0.230501.7.tar", max compression
```

## Comparing `sortedness-0.220803.1.tar` & `sortedness-0.230501.7.tar`

### file list

```diff
@@ -1,13 +1,18 @@
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
+-rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.230501.7/LICENSE
+-rw-r--r--   0        0        0     4291 2023-05-01 23:09:49.897114 sortedness-0.230501.7/README.md
+-rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-0.230501.7/build.py
+-rw-r--r--   0        0        0     1188 2023-05-02 00:50:25.603399 sortedness-0.230501.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-03 19:59:46.000000 sortedness-0.230501.7/src/sortedness/__init__.py
+-rw-r--r--   0        0        0     1281 2023-05-01 23:25:35.123741 sortedness-0.230501.7/src/sortedness/config.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-0.230501.7/src/sortedness/evaluation/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-01 21:01:18.170347 sortedness-0.230501.7/src/sortedness/evaluation/plot.py
+-rw-r--r--   0        0        0     5145 2023-05-01 21:07:34.442703 sortedness-0.230501.7/src/sortedness/global.py
+-rw-r--r--   0        0        0    22749 2023-05-01 23:40:16.090062 sortedness-0.230501.7/src/sortedness/local.py
+-rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-0.230501.7/src/sortedness/matrices.py
+-rw-r--r--   0        0        0     2962 2023-05-01 23:15:42.252581 sortedness-0.230501.7/src/sortedness/parallel.py
+-rw-r--r--   0        0        0     7950 2022-08-03 19:59:46.000000 sortedness-0.230501.7/src/sortedness/rank.py
+-rw-r--r--   0        0        0     4707 2022-08-03 19:59:46.000000 sortedness-0.230501.7/src/sortedness/trustworthiness.py
+-rw-r--r--   0        0        0     3511 2023-05-01 23:16:29.848511 sortedness-0.230501.7/src/sortedness/wtau/__init__.py
+-rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-0.230501.7/src/sortedness/wtau/wtau.pyx
+-rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 sortedness-0.230501.7/setup.py
+-rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 sortedness-0.230501.7/PKG-INFO
```

### Comparing `sortedness-0.220803.1/LICENSE` & `sortedness-0.230501.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sortedness-0.220803.1/src/sortedness/config.py` & `sortedness-0.230501.7/src/sortedness/config.py`

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

### Comparing `sortedness-0.220803.1/src/sortedness/evaluation/plot.py` & `sortedness-0.230501.7/src/sortedness/evaluation/plot.py`

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

### Comparing `sortedness-0.220803.1/src/sortedness/rank.py` & `sortedness-0.230501.7/src/sortedness/rank.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.220803.1/src/sortedness/trustworthiness.py` & `sortedness-0.230501.7/src/sortedness/trustworthiness.py`

 * *Files identical despite different names*

