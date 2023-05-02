# Comparing `tmp/pandas-indexing-0.2.1.tar.gz` & `tmp/pandas-indexing-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.1.tar", last modified: Sat Apr  8 09:21:00 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.2.tar", last modified: Tue May  2 11:17:54 2023, max compression
```

## Comparing `pandas-indexing-0.2.1.tar` & `pandas-indexing-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:21:00.004042 pandas-indexing-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-08 09:21:00.004042 pandas-indexing-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:20:59.992041 pandas-indexing-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:20:59.996041 pandas-indexing-0.2.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 09:21:00.004042 pandas-indexing-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:20:59.984041 pandas-indexing-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:21:00.000042 pandas-indexing-0.2.1/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:21:00.004042 pandas-indexing-0.2.1/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-08 09:20:39.000000 pandas-indexing-0.2.1/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:21:00.000042 pandas-indexing-0.2.1/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-08 09:20:59.000000 pandas-indexing-0.2.1/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-08 09:20:59.000000 pandas-indexing-0.2.1/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 09:20:59.000000 pandas-indexing-0.2.1/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-08 09:20:59.000000 pandas-indexing-0.2.1/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 09:20:59.000000 pandas-indexing-0.2.1/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.900339 pandas-indexing-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.1/CHANGELOG.rst` & `pandas-indexing-0.2.2/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+* :py:func:`~core.assignlevel` takes labels from an optional positional dataframe :pull:`5`
+* Add :py:func:`~core.dropnalevel` to remove missing index entries :pull:`4`, :pull:`6`
+
 v0.2.1 (2023-04-08)
 ------------------------------------------------------------
 
 * Restore compatibility with python 3.8
 * Improve typing and add tests for :py:func:`~selectors.isin` and
   :py:func:`~selectors.ismatch`
```

### Comparing `pandas-indexing-0.2.1/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/CONTRIBUTING.rst` & `pandas-indexing-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/LICENSE` & `pandas-indexing-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/PKG-INFO` & `pandas-indexing-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.1
+Version: 0.2.2
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.1/README.rst` & `pandas-indexing-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/docs/api.rst` & `pandas-indexing-0.2.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/docs/conf.py` & `pandas-indexing-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.2/docs/notebooks/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/pyproject.toml` & `pandas-indexing-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.2/src/pandas_indexing/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from . import core, datasets
 from .arithmetics import add, divide, multiply, subtract
 from .core import (
     alignlevel,
     alignlevels,
     assignlevel,
+    dropnalevel,
     index_names,
     projectlevel,
     semijoin,
 )
 from .selectors import isin, ismatch
```

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2.2/src/pandas_indexing/accessors.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,52 +7,58 @@
 >>> df.idx.project(["model", "scenario"])
 
 >>> df.index.idx.assign(unit="Mt CO2")
 
 >>> df.idx.multiply(other, how="left")
 """
 
-from typing import Any, Literal, Sequence, Union
+from typing import Any, Literal, Optional, Sequence, Union
 
 import pandas as pd
 from pandas import DataFrame, Index, MultiIndex, Series
 
 from . import arithmetics
-from .core import assignlevel, projectlevel, semijoin
+from .core import Data, assignlevel, dropnalevel, projectlevel, semijoin
 
 
 class _IdxAccessor:
     """
     Convenience accessor for accessing `pandas-indexing` functions.
     """
 
     def __init__(self, pandas_obj):
         self._obj = pandas_obj
 
     def assign(
-        self, order: bool = False, axis: int = 0, **labels: Any
+        self,
+        frame: Optional[Data] = None,
+        order: bool = False,
+        axis: int = 0,
+        **labels: Any,
     ) -> Union[DataFrame, Series, MultiIndex]:
         """
         Add or overwrite levels on a multiindex.
 
         Parameters
         ----------
+        frame : Series|DataFrame, optional
+            Additional labels
         order : list of str, optional
             Level names in desired order or False, by default False
         axis : int, optional
             Axis where to update multiindex, by default 0
         **labels
             Labels for each new index level
 
         Returns
         -------
         df
             Series or DataFrame with changed index or new MultiIndex
         """
-        return assignlevel(self._obj, order=order, axis=axis, **labels)
+        return assignlevel(self._obj, frame=frame, order=order, axis=axis, **labels)
 
     def project(
         self,
         levels: Sequence[str],
         axis: Union[int, str] = 0,
     ) -> Union[DataFrame, Series, Index]:
         """
@@ -76,14 +82,47 @@
         --------
         pandas.MultiIndex.droplevel
         pandas.Series.droplevel
         pandas.DataFrame.droplevel
         """
         return projectlevel(self._obj, levels=levels, axis=axis)
 
+    def dropna(
+        self,
+        subset: Optional[Sequence[str]] = None,
+        how: Literal["any", "all"] = "any",
+        axis: Union[int, str] = 0,
+    ) -> Union[DataFrame, Series, Index]:
+        """
+        Remove missing index values.
+
+        Drops all index entries for which any or all (`how`) levels are
+        undefined.
+
+        Parameters
+        ----------
+        subset : Sequence[str], optional
+            Names of levels on which to check for NA values
+        how : "any" (default) or "all"
+            Whether to remove an entry if all levels are NA only a single one
+        axis : int, optional
+            Axis of DataFrame to check on, by default 0
+
+        Returns
+        -------
+        index_or_series : Index|MultiIndex|Series|DataFrame
+
+        See also
+        --------
+        pandas.DataFrame.dropna
+        pandas.Series.dropna
+        pandas.Index.dropna
+        """
+        return dropnalevel(self._obj, subset=subset, how=how, axis=axis)
+
 
 class _DataIdxAccessor(_IdxAccessor):
     def semijoin(
         self,
         other: Index,
         *,
         how: Literal["left", "right", "inner", "outer"] = "left",
```

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.2/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/core.py` & `pandas-indexing-0.2.2/src/pandas_indexing/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """
 Core module.
 """
-from typing import Any, Literal, Sequence, TypeVar, Union
+from functools import reduce
+from itertools import chain
+from operator import and_, or_
+from typing import Any, Literal, Optional, Sequence, TypeVar, Union
 
 import numpy as np
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.core.indexes.frozen import FrozenList
 
 
 Data = Union[Series, DataFrame]
 T = TypeVar("T", bound=Union[Index, DataFrame, Series])
 S = TypeVar("S", bound=Union[DataFrame, Series])
 
 
-def _assignlevel(index: Index, order: bool = False, **labels: Any) -> MultiIndex:
+def _assignlevel(
+    index: Index, frame: Optional[Data] = None, order: bool = False, **labels: Any
+) -> MultiIndex:
     if isinstance(index, MultiIndex):
         new_levels = list(index.levels)
         new_codes = list(index.codes)
         new_names = list(index.names)
     else:
         level = index.unique().dropna()
         new_levels = [level]
         new_codes = [level.get_indexer(index)]
         new_names = [index.name]
 
+    if isinstance(frame, Series):
+        frame = frame.to_frame()
+    if isinstance(frame, DataFrame):
+        labels = dict(chain(frame.items(), labels.items()))
+
     for level, lbls in labels.items():
         if np.isscalar(lbls):
             lvl = [lbls]
             cde = np.full(len(index), 0)
         else:
             lvl = Index(lbls).unique().dropna()
             cde = lvl.get_indexer(lbls)
@@ -45,47 +55,55 @@
 
     if order:
         new_index = new_index.reorder_levels(order)
 
     return new_index
 
 
-def assignlevel(df: T, order: bool = False, axis: int = 0, **labels: Any) -> T:
+def assignlevel(
+    df: T,
+    frame: Optional[Data] = None,
+    order: bool = False,
+    axis: int = 0,
+    **labels: Any,
+) -> T:
     """
     Add or overwrite levels on a multiindex.
 
     Parameters
     ----------
     df : Series|DataFrame|MultiIndex
         Series or DataFrame on which to change index or index to change
+    frame : Series|DataFrame, optional
+        Additional labels
     order : list of str, optional
         Level names in desired order or False, by default False
     axis : int, optional
         Axis where to update multiindex, by default 0
     **labels
         Labels for each new index level
 
     Returns
     -------
     df
         Series or DataFrame with changed index or new MultiIndex
     """
     if isinstance(df, Index):
-        return _assignlevel(df, order=order, **labels)
+        return _assignlevel(df, frame=frame, order=order, **labels)
 
     if isinstance(df, Series):
         index = df.index
     elif isinstance(df, DataFrame):
         index = df.index if axis == 0 else df.columns
     else:
         raise TypeError(
             f"assignlevel expects an Index, Series or DataFrame ({type(df)=})"
         )
 
-    new_index = _assignlevel(index, order=order, **labels)
+    new_index = _assignlevel(index, frame=frame, order=order, **labels)
 
     return df.set_axis(new_index, axis=axis)
 
 
 def _projectlevel(index: Index, levels: Sequence[str]) -> Index:
     levels = np.atleast_1d(levels)
     if len(levels) == 1:
@@ -125,14 +143,69 @@
     if isinstance(index_or_series, Index):
         return _projectlevel(index_or_series, levels)
 
     index = index_or_series.index if axis in (0, "index") else index_or_series.columns
     return index_or_series.set_axis(_projectlevel(index, levels), axis=axis)
 
 
+def _notna(
+    index: Index,
+    subset: Optional[Sequence[str]] = None,
+    how: Literal["any", "all"] = "any",
+) -> np.ndarray:
+    index = ensure_multiindex(index)
+
+    subset = index.names if subset is None else np.atleast_1d(subset)
+    codes = [index.codes[index.names.index(n)] for n in subset]
+    op = and_ if how == "any" else or_
+    return reduce(op, [c != -1 for c in codes])
+
+
+def dropnalevel(
+    index_or_series: T,
+    subset: Optional[Sequence[str]] = None,
+    how: Literal["any", "all"] = "any",
+    axis: Union[int, str] = 0,
+) -> T:
+    """
+    Remove missing index values.
+
+    Drops all index entries for which any or all (`how`) levels are
+    undefined.
+
+    Parameters
+    ----------
+    index_or_series : MultiIndex|Series|DataFrame
+        MultiIndex, Series or DataFrame to project
+    subset : Sequence[str], optional
+        Names of levels on which to check for NA values
+    how : "any" (default) or "all"
+        Whether to remove an entry if all levels are NA only a single one
+    axis : int, optional
+        Axis of DataFrame to check on, by default 0
+
+    Returns
+    -------
+    index_or_series : Index|MultiIndex|Series|DataFrame
+
+    See also
+    --------
+    pandas.DataFrame.dropna
+    pandas.Series.dropna
+    pandas.Index.dropna
+    """
+    if isinstance(index_or_series, Index):
+        return index_or_series[_notna(index_or_series, subset, how)]
+
+    if axis in (0, "index"):
+        return index_or_series.loc[_notna(index_or_series.index, subset, how)]
+
+    return index_or_series.loc[:, _notna(index_or_series.columns, subset, how)]
+
+
 def index_names(s, raise_on_index=False):
     if isinstance(s, (Series, DataFrame)):
         s = s.index
 
     if isinstance(s, MultiIndex):
         names = s.names
     elif isinstance(s, Index):
```

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.2/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.2/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.2/src/pandas_indexing/selectors.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,14 +90,27 @@
 
 def isin(
     df: Optional[Data] = None, ignore_missing_levels: bool = False, **filters: Any
 ) -> Union[Isin, Series]:
     """
     Constructs a MultiIndex selector.
 
+    Arguments
+    ---------
+    df : Data, optional
+        Data on which to match, if missing an Isin object is returned
+    ignore_missing_levels : bool, default False
+        If set, levels missing in data index will be ignored
+    **filters
+        Filter to apply on given levels (lists are `or`ed, levels are `and`ed)
+
+    Returns
+    -------
+    Isin or Series
+
     Usage
     -----
     >>> df.loc[isin(region="World", gas=["CO2", "N2O"])]
 
     or with explicit df to get a boolean mask
 
     >>> isin(df, region="World", gas=["CO2", "N2O"])
@@ -162,14 +175,33 @@
     regex: bool = False,
     ignore_missing_levels: bool = False,
     **filters,
 ) -> Union[Ismatch, Series]:
     """
     Constructs an Index or MultiIndex selector based on pattern matching.
 
+    Arguments
+    ---------
+    df : Data, optional
+        Data on which to match, if missing an Isin object is returned.
+    singlefilter : str, optional
+        Filter to apply on a non-multiindex index (can also be handed into the `df`
+        argument)
+    regex : bool, default False
+        If set, filters are interpreted as plain regex strings, otherwise (by default) a
+        glob-like syntax is used
+    ignore_missing_levels : bool, default False
+        If set, levels missing in data index will be ignored
+    **filters
+        Filter to apply on given levels (lists are `or`ed, levels are `and`ed)
+
+    Returns
+    -------
+    Isin or Series
+
     Usage
     -----
     for a multiindex:
 
     >>> df.loc[ismatch(variable="Emissions|*|Fossil Fuel and Industry")]
 
     for a single index:
```

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing/utils.py` & `pandas-indexing-0.2.2/src/pandas_indexing/utils.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.2/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.1
+Version: 0.2.2
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.1/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.2/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

